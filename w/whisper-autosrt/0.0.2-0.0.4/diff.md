# Comparing `tmp/whisper_autosrt-0.0.2.tar.gz` & `tmp/whisper_autosrt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_autosrt-0.0.2.tar", last modified: Sun May 28 10:45:49 2023, max compression
+gzip compressed data, was "whisper_autosrt-0.0.4.tar", last modified: Mon May 29 23:35:34 2023, max compression
```

## Comparing `whisper_autosrt-0.0.2.tar` & `whisper_autosrt-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 10:45:49.039622 whisper_autosrt-0.0.2/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2009 2023-05-28 10:45:49.040370 whisper_autosrt-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.0.2/README.md
--rw-rw-rw-   0        0        0      147 2023-05-28 10:45:49.044119 whisper_autosrt-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1466 2023-05-27 17:47:37.000000 whisper_autosrt-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:45:48.973850 whisper_autosrt-0.0.2/whisper_autosrt/
--rw-rw-rw-   0        0        0    78004 2023-05-27 17:33:39.000000 whisper_autosrt-0.0.2/whisper_autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:45:49.036625 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/
--rw-rw-rw-   0        0        0     2009 2023-05-28 10:45:48.000000 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-05-28 10:45:48.000000 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 10:45:48.000000 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-28 10:45:48.000000 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      122 2023-05-28 10:45:48.000000 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-28 10:45:48.000000 whisper_autosrt-0.0.2/whisper_autosrt.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-29 23:35:34.862686 whisper_autosrt-0.0.4/
+-rwxrwxrwx   0 root         (0) root         (0)     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.0.4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.0.4/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     1978 2023-05-29 23:35:34.862903 whisper_autosrt-0.0.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.0.4/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      136 2023-05-29 23:35:34.863713 whisper_autosrt-0.0.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1496 2023-05-29 23:35:00.000000 whisper_autosrt-0.0.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-29 23:35:34.858258 whisper_autosrt-0.0.4/whisper_autosrt/
+-rwxrwxrwx   0 root         (0) root         (0)    70797 2023-05-29 23:29:35.000000 whisper_autosrt-0.0.4/whisper_autosrt/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-29 23:35:34.862267 whisper_autosrt-0.0.4/whisper_autosrt.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1978 2023-05-29 23:35:34.000000 whisper_autosrt-0.0.4/whisper_autosrt.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      312 2023-05-29 23:35:34.000000 whisper_autosrt-0.0.4/whisper_autosrt.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-29 23:35:34.000000 whisper_autosrt-0.0.4/whisper_autosrt.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       57 2023-05-29 23:35:34.000000 whisper_autosrt-0.0.4/whisper_autosrt.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)      119 2023-05-29 23:35:34.000000 whisper_autosrt-0.0.4/whisper_autosrt.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       16 2023-05-29 23:35:34.000000 whisper_autosrt-0.0.4/whisper_autosrt.egg-info/top_level.txt
```

### Comparing `whisper_autosrt-0.0.2/LICENSE` & `whisper_autosrt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.0.2/PKG-INFO` & `whisper_autosrt-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: whisper_autosrt
-Version: 0.0.2
-Summary: a command line utility for automatic speech recognition and subtitle generation
-Home-page: https://github.com/botbahlul/whisper_autosrt
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 botbahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-
-whisper_autosrt is a utility for automatic speech recognition and subtitle generation.  It takes video or audio files as input, convert it to a temporary wav file then generatetranscriptions for that wav file, and optionally translates them to a different languageand finally saves the resulting subtitles file to disk.                                 It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+Metadata-Version: 2.1
+Name: whisper_autosrt
+Version: 0.0.4
+Summary: a command line utility for automatic speech recognition and subtitle generation
+Home-page: https://github.com/botbahlul/whisper_autosrt
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+        
+        Copyright (c) 2022 botbahlul
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+
+whisper_autosrt is a utility for automatic speech recognition and subtitle generation.  It takes video or audio files as input, convert it to a temporary wav file then generatetranscriptions for that wav file, and optionally translates them to a different languageand finally saves the resulting subtitles file to disk.                                 It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
```

### Comparing `whisper_autosrt-0.0.2/README.md` & `whisper_autosrt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.0.2/setup.py` & `whisper_autosrt-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 install_requires=[
     "requests>=2.3.0",
     "httpx>=0.24.0",
     "urllib3 >=1.26.0,<3.0",
     "pysrt>=1.0.1",
     "six>=1.11.0",
     "progressbar2>=3.34.3",
-    "openai_whisper>=20230314",
+    #"openai_whisper>=20230314",
+    "faster_whisper>=0.6.0",
 ]
 
 setup(
     name="whisper_autosrt",
     version=VERSION,
     description="a command line utility for automatic speech recognition and subtitle generation",
     long_description = long_description,
```

### Comparing `whisper_autosrt-0.0.2/whisper_autosrt/__init__.py` & `whisper_autosrt-0.0.4/whisper_autosrt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,4876 +1,4425 @@
-00000000: 2320 4f52 4947 494e 414c 2041 5554 4f53  # ORIGINAL AUTOS
-00000010: 5542 2049 4d50 4f52 5453 0d0a 6672 6f6d  UB IMPORTS..from
-00000020: 205f 5f66 7574 7572 655f 5f20 696d 706f   __future__ impo
-00000030: 7274 2061 6273 6f6c 7574 655f 696d 706f  rt absolute_impo
-00000040: 7274 2c20 7072 696e 745f 6675 6e63 7469  rt, print_functi
-00000050: 6f6e 2c20 756e 6963 6f64 655f 6c69 7465  on, unicode_lite
-00000060: 7261 6c73 0d0a 696d 706f 7274 2061 7267  rals..import arg
-00000070: 7061 7273 650d 0a69 6d70 6f72 7420 6175  parse..import au
-00000080: 6469 6f6f 700d 0a69 6d70 6f72 7420 6d61  dioop..import ma
-00000090: 7468 0d0a 696d 706f 7274 206d 756c 7469  th..import multi
-000000a0: 7072 6f63 6573 7369 6e67 0d0a 696d 706f  processing..impo
-000000b0: 7274 206f 730d 0a69 6d70 6f72 7420 7375  rt os..import su
-000000c0: 6270 726f 6365 7373 0d0a 696d 706f 7274  bprocess..import
-000000d0: 2073 7973 0d0a 696d 706f 7274 2074 656d   sys..import tem
-000000e0: 7066 696c 650d 0a69 6d70 6f72 7420 7761  pfile..import wa
-000000f0: 7665 0d0a 696d 706f 7274 206a 736f 6e0d  ve..import json.
-00000100: 0a69 6d70 6f72 7420 7265 7175 6573 7473  .import requests
-00000110: 0d0a 7472 793a 0d0a 2020 2020 6672 6f6d  ..try:..    from
-00000120: 206a 736f 6e2e 6465 636f 6465 7220 696d   json.decoder im
-00000130: 706f 7274 204a 534f 4e44 6563 6f64 6545  port JSONDecodeE
-00000140: 7272 6f72 0d0a 6578 6365 7074 2049 6d70  rror..except Imp
-00000150: 6f72 7445 7272 6f72 3a0d 0a20 2020 204a  ortError:..    J
-00000160: 534f 4e44 6563 6f64 6545 7272 6f72 203d  SONDecodeError =
-00000170: 2056 616c 7565 4572 726f 720d 0a66 726f   ValueError..fro
-00000180: 6d20 7072 6f67 7265 7373 6261 7220 696d  m progressbar im
-00000190: 706f 7274 2050 726f 6772 6573 7342 6172  port ProgressBar
-000001a0: 2c20 5065 7263 656e 7461 6765 2c20 4261  , Percentage, Ba
-000001b0: 722c 2045 5441 0d0a 696d 706f 7274 2070  r, ETA..import p
-000001c0: 7973 7274 0d0a 696d 706f 7274 2073 6978  ysrt..import six
-000001d0: 0d0a 2320 4144 4449 5449 4f4e 414c 2049  ..# ADDITIONAL I
-000001e0: 4d50 4f52 540d 0a66 726f 6d20 676c 6f62  MPORT..from glob
-000001f0: 2069 6d70 6f72 7420 676c 6f62 2c20 6573   import glob, es
-00000200: 6361 7065 0d0a 696d 706f 7274 2074 696d  cape..import tim
-00000210: 650d 0a66 726f 6d20 6461 7465 7469 6d65  e..from datetime
-00000220: 2069 6d70 6f72 7420 6461 7465 7469 6d65   import datetime
-00000230: 2c20 7469 6d65 6465 6c74 610d 0a66 726f  , timedelta..fro
-00000240: 6d20 7061 7468 6c69 6220 696d 706f 7274  m pathlib import
-00000250: 2050 6174 680d 0a69 6d70 6f72 7420 7761   Path..import wa
-00000260: 726e 696e 6773 0d0a 7761 726e 696e 6773  rnings..warnings
-00000270: 2e66 696c 7465 7277 6172 6e69 6e67 7328  .filterwarnings(
-00000280: 2269 676e 6f72 6522 2c20 6d65 7373 6167  "ignore", messag
-00000290: 653d 222e 2a54 6865 2027 6e6f 7079 7468  e=".*The 'nopyth
-000002a0: 6f6e 2720 6b65 7977 6f72 642e 2a22 290d  on' keyword.*").
-000002b0: 0a69 6d70 6f72 7420 7768 6973 7065 720d  .import whisper.
-000002c0: 0a0d 0a0d 0a56 4552 5349 4f4e 203d 2022  .....VERSION = "
-000002d0: 302e 302e 3222 0d0a 0d0a 233d 3d3d 3d3d  0.0.2"....#=====
-000002e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000002f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000300: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000310: 3d3d 3d20 6666 6d70 6567 5f70 726f 6772  === ffmpeg_progr
-00000320: 6573 735f 7969 656c 6420 3d3d 3d3d 3d3d  ess_yield ======
-00000330: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000340: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000360: 3d3d 230d 0a0d 0a69 6d70 6f72 7420 7265  ==#....import re
-00000370: 0d0a 2369 6d70 6f72 7420 7375 6270 726f  ..#import subpro
-00000380: 6365 7373 0d0a 6672 6f6d 2074 7970 696e  cess..from typin
-00000390: 6720 696d 706f 7274 2041 6e79 2c20 4361  g import Any, Ca
-000003a0: 6c6c 6162 6c65 2c20 4974 6572 6174 6f72  llable, Iterator
-000003b0: 2c20 4c69 7374 2c20 4f70 7469 6f6e 616c  , List, Optional
-000003c0: 2c20 556e 696f 6e0d 0a0d 0a0d 0a64 6566  , Union......def
-000003d0: 2074 6f5f 6d73 282a 2a6b 7761 7267 733a   to_ms(**kwargs:
-000003e0: 2055 6e69 6f6e 5b66 6c6f 6174 2c20 696e   Union[float, in
-000003f0: 742c 2073 7472 5d29 202d 3e20 696e 743a  t, str]) -> int:
-00000400: 0d0a 2020 2020 686f 7572 203d 2069 6e74  ..    hour = int
-00000410: 286b 7761 7267 732e 6765 7428 2268 6f75  (kwargs.get("hou
-00000420: 7222 2c20 3029 290d 0a20 2020 206d 696e  r", 0))..    min
-00000430: 7574 6520 3d20 696e 7428 6b77 6172 6773  ute = int(kwargs
-00000440: 2e67 6574 2822 6d69 6e22 2c20 3029 290d  .get("min", 0)).
-00000450: 0a20 2020 2073 6563 203d 2069 6e74 286b  .    sec = int(k
-00000460: 7761 7267 732e 6765 7428 2273 6563 222c  wargs.get("sec",
-00000470: 2030 2929 0d0a 2020 2020 6d73 203d 2069   0))..    ms = i
-00000480: 6e74 286b 7761 7267 732e 6765 7428 226d  nt(kwargs.get("m
-00000490: 7322 2c20 3029 290d 0a0d 0a20 2020 2072  s", 0))....    r
-000004a0: 6574 7572 6e20 2868 6f75 7220 2a20 3630  eturn (hour * 60
-000004b0: 202a 2036 3020 2a20 3130 3030 2920 2b20   * 60 * 1000) + 
-000004c0: 286d 696e 7574 6520 2a20 3630 202a 2031  (minute * 60 * 1
-000004d0: 3030 3029 202b 2028 7365 6320 2a20 3130  000) + (sec * 10
-000004e0: 3030 2920 2b20 6d73 0d0a 0d0a 0d0a 6465  00) + ms......de
-000004f0: 6620 5f70 726f 6265 5f64 7572 6174 696f  f _probe_duratio
-00000500: 6e28 636d 643a 204c 6973 745b 7374 725d  n(cmd: List[str]
-00000510: 2920 2d3e 204f 7074 696f 6e61 6c5b 696e  ) -> Optional[in
-00000520: 745d 3a0d 0a20 2020 2027 2727 0d0a 2020  t]:..    '''..  
-00000530: 2020 4765 7420 7468 6520 6475 7261 7469    Get the durati
-00000540: 6f6e 2076 6961 2066 6670 726f 6265 2066  on via ffprobe f
-00000550: 726f 6d20 696e 7075 7420 6d65 6469 6120  rom input media 
-00000560: 6669 6c65 0d0a 2020 2020 696e 2063 6173  file..    in cas
-00000570: 6520 6666 6d70 6567 2077 6173 2072 756e  e ffmpeg was run
-00000580: 2077 6974 6820 6c6f 676c 6576 656c 3d65   with loglevel=e
-00000590: 7272 6f72 2e0d 0a0d 0a20 2020 2041 7267  rror.....    Arg
-000005a0: 733a 0d0a 2020 2020 2020 2020 636d 6420  s:..        cmd 
-000005b0: 284c 6973 745b 7374 725d 293a 2041 206c  (List[str]): A l
-000005c0: 6973 7420 6f66 2063 6f6d 6d61 6e64 206c  ist of command l
-000005d0: 696e 6520 656c 656d 656e 7473 2c20 652e  ine elements, e.
-000005e0: 672e 205b 2266 666d 7065 6722 2c20 222d  g. ["ffmpeg", "-
-000005f0: 6922 2c20 2e2e 2e5d 0d0a 0d0a 2020 2020  i", ...]....    
-00000600: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
-00000610: 2020 4f70 7469 6f6e 616c 5b69 6e74 5d3a    Optional[int]:
-00000620: 2054 6865 2064 7572 6174 696f 6e20 696e   The duration in
-00000630: 206d 696c 6c69 7365 636f 6e64 732e 0d0a   milliseconds...
-00000640: 2020 2020 2727 270d 0a0d 0a20 2020 2064      '''....    d
-00000650: 6566 205f 6765 745f 6669 6c65 5f6e 616d  ef _get_file_nam
-00000660: 6528 636d 643a 204c 6973 745b 7374 725d  e(cmd: List[str]
-00000670: 2920 2d3e 204f 7074 696f 6e61 6c5b 7374  ) -> Optional[st
-00000680: 725d 3a0d 0a20 2020 2020 2020 2074 7279  r]:..        try
-00000690: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-000006a0: 6478 203d 2063 6d64 2e69 6e64 6578 2822  dx = cmd.index("
-000006b0: 2d69 2229 0d0a 2020 2020 2020 2020 2020  -i")..          
-000006c0: 2020 7265 7475 726e 2063 6d64 5b69 6478    return cmd[idx
-000006d0: 202b 2031 5d0d 0a20 2020 2020 2020 2065   + 1]..        e
-000006e0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
-000006f0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00000700: 6574 7572 6e20 4e6f 6e65 0d0a 0d0a 2020  eturn None....  
-00000710: 2020 6669 6c65 5f6e 616d 6520 3d20 5f67    file_name = _g
-00000720: 6574 5f66 696c 655f 6e61 6d65 2863 6d64  et_file_name(cmd
-00000730: 290d 0a20 2020 2069 6620 6669 6c65 5f6e  )..    if file_n
-00000740: 616d 6520 6973 204e 6f6e 653a 0d0a 2020  ame is None:..  
-00000750: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00000760: 650d 0a0d 0a20 2020 2074 7279 3a0d 0a20  e....    try:.. 
-00000770: 2020 2020 2020 2069 6620 7379 732e 706c         if sys.pl
-00000780: 6174 666f 726d 203d 3d20 2277 696e 3332  atform == "win32
-00000790: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-000007a0: 6f75 7470 7574 203d 2073 7562 7072 6f63  output = subproc
-000007b0: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
-000007c0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-000007d0: 2020 205b 0d0a 2020 2020 2020 2020 2020     [..          
-000007e0: 2020 2020 2020 2020 2020 2266 6670 726f            "ffpro
-000007f0: 6265 222c 0d0a 2020 2020 2020 2020 2020  be",..          
-00000800: 2020 2020 2020 2020 2020 222d 6c6f 676c            "-logl
-00000810: 6576 656c 222c 0d0a 2020 2020 2020 2020  evel",..        
-00000820: 2020 2020 2020 2020 2020 2020 222d 3122              "-1"
-00000830: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000840: 2020 2020 2020 2022 2d68 6964 655f 6261         "-hide_ba
-00000850: 6e6e 6572 222c 0d0a 2020 2020 2020 2020  nner",..        
-00000860: 2020 2020 2020 2020 2020 2020 222d 7368              "-sh
-00000870: 6f77 5f65 6e74 7269 6573 222c 0d0a 2020  ow_entries",..  
-00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000890: 2020 2266 6f72 6d61 743d 6475 7261 7469    "format=durati
-000008a0: 6f6e 222c 0d0a 2020 2020 2020 2020 2020  on",..          
-000008b0: 2020 2020 2020 2020 2020 222d 6f66 222c            "-of",
-000008c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000008d0: 2020 2020 2020 2264 6566 6175 6c74 3d6e        "default=n
-000008e0: 6f70 7269 6e74 5f77 7261 7070 6572 733d  oprint_wrappers=
-000008f0: 313a 6e6f 6b65 793d 3122 2c0d 0a20 2020  1:nokey=1",..   
-00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000910: 2066 696c 655f 6e61 6d65 2c0d 0a20 2020   file_name,..   
-00000920: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
-00000930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000940: 2075 6e69 7665 7273 616c 5f6e 6577 6c69   universal_newli
-00000950: 6e65 733d 5472 7565 2c0d 0a20 2020 2020  nes=True,..     
-00000960: 2020 2020 2020 2020 2020 2063 7265 6174             creat
-00000970: 696f 6e66 6c61 6773 3d73 7562 7072 6f63  ionflags=subproc
-00000980: 6573 732e 4352 4541 5445 5f4e 4f5f 5749  ess.CREATE_NO_WI
-00000990: 4e44 4f57 2c0d 0a20 2020 2020 2020 2020  NDOW,..         
-000009a0: 2020 2029 0d0a 2020 2020 2020 2020 656c     )..        el
-000009b0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-000009c0: 206f 7574 7075 7420 3d20 7375 6270 726f   output = subpro
-000009d0: 6365 7373 2e63 6865 636b 5f6f 7574 7075  cess.check_outpu
-000009e0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-000009f0: 2020 2020 5b0d 0a20 2020 2020 2020 2020      [..         
-00000a00: 2020 2020 2020 2020 2020 2022 6666 7072             "ffpr
-00000a10: 6f62 6522 2c0d 0a20 2020 2020 2020 2020  obe",..         
-00000a20: 2020 2020 2020 2020 2020 2022 2d6c 6f67             "-log
-00000a30: 6c65 7665 6c22 2c0d 0a20 2020 2020 2020  level",..       
-00000a40: 2020 2020 2020 2020 2020 2020 2022 2d31               "-1
-00000a50: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000a60: 2020 2020 2020 2020 222d 6869 6465 5f62          "-hide_b
-00000a70: 616e 6e65 7222 2c0d 0a20 2020 2020 2020  anner",..       
-00000a80: 2020 2020 2020 2020 2020 2020 2022 2d73               "-s
-00000a90: 686f 775f 656e 7472 6965 7322 2c0d 0a20  how_entries",.. 
-00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ab0: 2020 2022 666f 726d 6174 3d64 7572 6174     "format=durat
-00000ac0: 696f 6e22 2c0d 0a20 2020 2020 2020 2020  ion",..         
-00000ad0: 2020 2020 2020 2020 2020 2022 2d6f 6622             "-of"
-00000ae0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000af0: 2020 2020 2020 2022 6465 6661 756c 743d         "default=
-00000b00: 6e6f 7072 696e 745f 7772 6170 7065 7273  noprint_wrappers
-00000b10: 3d31 3a6e 6f6b 6579 3d31 222c 0d0a 2020  =1:nokey=1",..  
-00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b30: 2020 6669 6c65 5f6e 616d 652c 0d0a 2020    file_name,..  
-00000b40: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00000b50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000b60: 2020 756e 6976 6572 7361 6c5f 6e65 776c    universal_newl
-00000b70: 696e 6573 3d54 7275 652c 0d0a 2020 2020  ines=True,..    
-00000b80: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-00000b90: 2020 2020 2072 6574 7572 6e20 696e 7428       return int(
-00000ba0: 666c 6f61 7428 6f75 7470 7574 2e73 7472  float(output.str
-00000bb0: 6970 2829 2920 2a20 3130 3030 290d 0a20  ip()) * 1000).. 
-00000bc0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00000bd0: 696f 6e3a 0d0a 2020 2020 2020 2020 2320  ion:..        # 
-00000be0: 544f 444f 3a20 6164 6420 6c6f 6767 696e  TODO: add loggin
-00000bf0: 670d 0a20 2020 2020 2020 2072 6574 7572  g..        retur
-00000c00: 6e20 4e6f 6e65 0d0a 0d0a 0d0a 6465 6620  n None......def 
-00000c10: 5f75 7365 735f 6572 726f 725f 6c6f 676c  _uses_error_logl
-00000c20: 6576 656c 2863 6d64 3a20 4c69 7374 5b73  evel(cmd: List[s
-00000c30: 7472 5d29 202d 3e20 626f 6f6c 3a0d 0a20  tr]) -> bool:.. 
-00000c40: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00000c50: 2069 6478 203d 2063 6d64 2e69 6e64 6578   idx = cmd.index
-00000c60: 2822 2d6c 6f67 6c65 7665 6c22 290d 0a20  ("-loglevel").. 
-00000c70: 2020 2020 2020 2069 6620 636d 645b 6964         if cmd[id
-00000c80: 7820 2b20 315d 203d 3d20 2265 7272 6f72  x + 1] == "error
-00000c90: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-00000ca0: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
-00000cb0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00000cc0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00000cd0: 616c 7365 0d0a 2020 2020 6578 6365 7074  alse..    except
-00000ce0: 2056 616c 7565 4572 726f 723a 0d0a 2020   ValueError:..  
-00000cf0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00000d00: 7365 0d0a 0d0a 0d0a 636c 6173 7320 4666  se......class Ff
-00000d10: 6d70 6567 5072 6f67 7265 7373 3a0d 0a20  mpegProgress:.. 
-00000d20: 2020 2044 5552 5f52 4547 4558 203d 2072     DUR_REGEX = r
-00000d30: 652e 636f 6d70 696c 6528 0d0a 2020 2020  e.compile(..    
-00000d40: 2020 2020 7222 4475 7261 7469 6f6e 3a20      r"Duration: 
-00000d50: 283f 503c 686f 7572 3e5c 647b 327d 293a  (?P<hour>\d{2}):
-00000d60: 283f 503c 6d69 6e3e 5c64 7b32 7d29 3a28  (?P<min>\d{2}):(
-00000d70: 3f50 3c73 6563 3e5c 647b 327d 295c 2e28  ?P<sec>\d{2})\.(
-00000d80: 3f50 3c6d 733e 5c64 7b32 7d29 220d 0a20  ?P<ms>\d{2})".. 
-00000d90: 2020 2029 0d0a 2020 2020 5449 4d45 5f52     )..    TIME_R
-00000da0: 4547 4558 203d 2072 652e 636f 6d70 696c  EGEX = re.compil
-00000db0: 6528 0d0a 2020 2020 2020 2020 7222 6f75  e(..        r"ou
-00000dc0: 745f 7469 6d65 3d28 3f50 3c68 6f75 723e  t_time=(?P<hour>
-00000dd0: 5c64 7b32 7d29 3a28 3f50 3c6d 696e 3e5c  \d{2}):(?P<min>\
-00000de0: 647b 327d 293a 283f 503c 7365 633e 5c64  d{2}):(?P<sec>\d
-00000df0: 7b32 7d29 5c2e 283f 503c 6d73 3e5c 647b  {2})\.(?P<ms>\d{
-00000e00: 327d 2922 0d0a 2020 2020 290d 0a0d 0a20  2})"..    ).... 
-00000e10: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00000e20: 7365 6c66 2c20 636d 643a 204c 6973 745b  self, cmd: List[
-00000e30: 7374 725d 2c20 6472 795f 7275 6e3a 2062  str], dry_run: b
-00000e40: 6f6f 6c20 3d20 4661 6c73 6529 202d 3e20  ool = False) -> 
-00000e50: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2027  None:..        '
-00000e60: 2727 496e 6974 6961 6c69 7a65 2074 6865  ''Initialize the
-00000e70: 2046 666d 7065 6750 726f 6772 6573 7320   FfmpegProgress 
-00000e80: 636c 6173 732e 0d0a 0d0a 2020 2020 2020  class.....      
-00000e90: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-00000ea0: 2020 2020 2063 6d64 2028 4c69 7374 5b73       cmd (List[s
-00000eb0: 7472 5d29 3a20 4120 6c69 7374 206f 6620  tr]): A list of 
-00000ec0: 636f 6d6d 616e 6420 6c69 6e65 2065 6c65  command line ele
-00000ed0: 6d65 6e74 732c 2065 2e67 2e20 5b22 6666  ments, e.g. ["ff
-00000ee0: 6d70 6567 222c 2022 2d69 222c 202e 2e2e  mpeg", "-i", ...
-00000ef0: 5d0d 0a20 2020 2020 2020 2020 2020 2064  ]..            d
-00000f00: 7279 5f72 756e 2028 626f 6f6c 2c20 6f70  ry_run (bool, op
-00000f10: 7469 6f6e 616c 293a 204f 6e6c 7920 7368  tional): Only sh
-00000f20: 6f77 2077 6861 7420 776f 756c 6420 6265  ow what would be
-00000f30: 2064 6f6e 652e 2044 6566 6175 6c74 7320   done. Defaults 
-00000f40: 746f 2046 616c 7365 2e0d 0a20 2020 2020  to False...     
-00000f50: 2020 2027 2727 0d0a 2020 2020 2020 2020     '''..        
-00000f60: 7365 6c66 2e63 6d64 203d 2063 6d64 0d0a  self.cmd = cmd..
-00000f70: 2020 2020 2020 2020 7365 6c66 2e73 7464          self.std
-00000f80: 6572 723a 2055 6e69 6f6e 5b73 7472 2c20  err: Union[str, 
-00000f90: 4e6f 6e65 5d20 3d20 4e6f 6e65 0d0a 2020  None] = None..  
-00000fa0: 2020 2020 2020 7365 6c66 2e64 7279 5f72        self.dry_r
-00000fb0: 756e 203d 2064 7279 5f72 756e 0d0a 2020  un = dry_run..  
-00000fc0: 2020 2020 2020 7365 6c66 2e70 726f 6365        self.proce
-00000fd0: 7373 3a20 416e 7920 3d20 4e6f 6e65 0d0a  ss: Any = None..
-00000fe0: 2020 2020 2020 2020 7365 6c66 2e73 7464          self.std
-00000ff0: 6572 725f 6361 6c6c 6261 636b 3a20 556e  err_callback: Un
-00001000: 696f 6e5b 4361 6c6c 6162 6c65 5b5b 7374  ion[Callable[[st
-00001010: 725d 2c20 4e6f 6e65 5d2c 204e 6f6e 655d  r], None], None]
-00001020: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
-00001030: 2069 6620 7379 732e 706c 6174 666f 726d   if sys.platform
-00001040: 203d 3d20 2277 696e 3332 223a 0d0a 2020   == "win32":..  
-00001050: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00001060: 6173 655f 706f 7065 6e5f 6b77 6172 6773  ase_popen_kwargs
-00001070: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
-00001080: 2020 2020 2020 2273 7464 696e 223a 2073        "stdin": s
-00001090: 7562 7072 6f63 6573 732e 5049 5045 2c20  ubprocess.PIPE, 
-000010a0: 2023 2041 7070 6c79 2073 7464 696e 2069   # Apply stdin i
-000010b0: 736f 6c61 7469 6f6e 2062 7920 6372 6561  solation by crea
-000010c0: 7469 6e67 2073 6570 6172 6174 6520 7069  ting separate pi
-000010d0: 7065 2e0d 0a20 2020 2020 2020 2020 2020  pe...           
-000010e0: 2020 2020 2022 7374 646f 7574 223a 2073       "stdout": s
-000010f0: 7562 7072 6f63 6573 732e 5049 5045 2c0d  ubprocess.PIPE,.
-00001100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001110: 2022 7374 6465 7272 223a 2073 7562 7072   "stderr": subpr
-00001120: 6f63 6573 732e 5354 444f 5554 2c0d 0a20  ocess.STDOUT,.. 
-00001130: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001140: 756e 6976 6572 7361 6c5f 6e65 776c 696e  universal_newlin
-00001150: 6573 223a 2046 616c 7365 2c0d 0a20 2020  es": False,..   
-00001160: 2020 2020 2020 2020 2020 2020 2022 7368               "sh
-00001170: 656c 6c22 3a20 5472 7565 2c0d 0a20 2020  ell": True,..   
-00001180: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00001190: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000011a0: 2020 2020 2020 2073 656c 662e 6261 7365         self.base
-000011b0: 5f70 6f70 656e 5f6b 7761 7267 7320 3d20  _popen_kwargs = 
-000011c0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-000011d0: 2020 2022 7374 6469 6e22 3a20 7375 6270     "stdin": subp
-000011e0: 726f 6365 7373 2e50 4950 452c 2020 2320  rocess.PIPE,  # 
-000011f0: 4170 706c 7920 7374 6469 6e20 6973 6f6c  Apply stdin isol
-00001200: 6174 696f 6e20 6279 2063 7265 6174 696e  ation by creatin
-00001210: 6720 7365 7061 7261 7465 2070 6970 652e  g separate pipe.
-00001220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001230: 2020 2273 7464 6f75 7422 3a20 7375 6270    "stdout": subp
-00001240: 726f 6365 7373 2e50 4950 452c 0d0a 2020  rocess.PIPE,..  
-00001250: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00001260: 7464 6572 7222 3a20 7375 6270 726f 6365  tderr": subproce
-00001270: 7373 2e53 5444 4f55 542c 0d0a 2020 2020  ss.STDOUT,..    
-00001280: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
-00001290: 7665 7273 616c 5f6e 6577 6c69 6e65 7322  versal_newlines"
-000012a0: 3a20 4661 6c73 652c 0d0a 2020 2020 2020  : False,..      
-000012b0: 2020 2020 2020 7d0d 0a0d 0a20 2020 2064        }....    d
-000012c0: 6566 2073 6574 5f73 7464 6572 725f 6361  ef set_stderr_ca
-000012d0: 6c6c 6261 636b 2873 656c 662c 2063 616c  llback(self, cal
-000012e0: 6c62 6163 6b3a 2043 616c 6c61 626c 655b  lback: Callable[
-000012f0: 5b73 7472 5d2c 204e 6f6e 655d 2920 2d3e  [str], None]) ->
-00001300: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00001310: 2727 270d 0a20 2020 2020 2020 2053 6574  '''..        Set
-00001320: 2061 2063 616c 6c62 6163 6b20 6675 6e63   a callback func
-00001330: 7469 6f6e 2074 6f20 6265 2063 616c 6c65  tion to be calle
-00001340: 6420 6f6e 2073 7464 6572 7220 6f75 7470  d on stderr outp
-00001350: 7574 2e0d 0a20 2020 2020 2020 2054 6865  ut...        The
-00001360: 2063 616c 6c62 6163 6b20 6675 6e63 7469   callback functi
-00001370: 6f6e 206d 7573 7420 6163 6365 7074 2061  on must accept a
-00001380: 2073 696e 676c 6520 7374 7269 6e67 2061   single string a
-00001390: 7267 756d 656e 742e 0d0a 2020 2020 2020  rgument...      
-000013a0: 2020 4e6f 7465 2074 6861 7420 7468 6973    Note that this
-000013b0: 2069 7320 6361 6c6c 6564 206f 6e20 6576   is called on ev
-000013c0: 6572 7920 6c69 6e65 206f 6620 7374 6465  ery line of stde
-000013d0: 7272 206f 7574 7075 742c 2073 6f20 6974  rr output, so it
-000013e0: 2063 616e 2062 6520 6361 6c6c 6564 2061   can be called a
-000013f0: 206c 6f74 2e0d 0a20 2020 2020 2020 2041   lot...        A
-00001400: 6c73 6f20 6e6f 7465 2074 6861 7420 7374  lso note that st
-00001410: 646f 7574 2f73 7464 6572 7220 6172 6520  dout/stderr are 
-00001420: 6a6f 696e 6564 2069 6e74 6f20 6f6e 6520  joined into one 
-00001430: 7374 7265 616d 2c20 736f 2079 6f75 206d  stream, so you m
-00001440: 6967 6874 2067 6574 2073 7464 6f75 7420  ight get stdout 
-00001450: 6f75 7470 7574 2069 6e20 7468 6520 6361  output in the ca
-00001460: 6c6c 6261 636b 2e0d 0a0d 0a20 2020 2020  llback.....     
-00001470: 2020 2041 7267 733a 0d0a 2020 2020 2020     Args:..      
-00001480: 2020 2020 2020 6361 6c6c 6261 636b 2028        callback (
-00001490: 4361 6c6c 6162 6c65 5b5b 7374 725d 2c20  Callable[[str], 
-000014a0: 4e6f 6e65 5d29 3a20 4120 6361 6c6c 6261  None]): A callba
-000014b0: 636b 2066 756e 6374 696f 6e20 7468 6174  ck function that
-000014c0: 2061 6363 6570 7473 2061 2073 696e 676c   accepts a singl
-000014d0: 6520 7374 7269 6e67 2061 7267 756d 656e  e string argumen
-000014e0: 742e 0d0a 2020 2020 2020 2020 2727 270d  t...        '''.
-000014f0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00001500: 6361 6c6c 6162 6c65 2863 616c 6c62 6163  callable(callbac
-00001510: 6b29 206f 7220 6c65 6e28 6361 6c6c 6261  k) or len(callba
-00001520: 636b 2e5f 5f63 6f64 655f 5f2e 636f 5f76  ck.__code__.co_v
-00001530: 6172 6e61 6d65 7329 2021 3d20 313a 0d0a  arnames) != 1:..
-00001540: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00001550: 6520 5661 6c75 6545 7272 6f72 280d 0a20  e ValueError(.. 
-00001560: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001570: 4361 6c6c 6261 636b 206d 7573 7420 6265  Callback must be
-00001580: 2061 2066 756e 6374 696f 6e20 7468 6174   a function that
-00001590: 2061 6363 6570 7473 206f 6e6c 7920 6f6e   accepts only on
-000015a0: 6520 6172 6775 6d65 6e74 220d 0a20 2020  e argument"..   
-000015b0: 2020 2020 2020 2020 2029 0d0a 0d0a 2020           )....  
-000015c0: 2020 2020 2020 7365 6c66 2e73 7464 6572        self.stder
-000015d0: 725f 6361 6c6c 6261 636b 203d 2063 616c  r_callback = cal
-000015e0: 6c62 6163 6b0d 0a0d 0a20 2020 2064 6566  lback....    def
-000015f0: 2072 756e 5f63 6f6d 6d61 6e64 5f77 6974   run_command_wit
-00001600: 685f 7072 6f67 7265 7373 280d 0a20 2020  h_progress(..   
-00001610: 2020 2020 2073 656c 662c 2070 6f70 656e       self, popen
-00001620: 5f6b 7761 7267 733d 4e6f 6e65 2c20 6475  _kwargs=None, du
-00001630: 7261 7469 6f6e 5f6f 7665 7272 6964 653a  ration_override:
-00001640: 2055 6e69 6f6e 5b66 6c6f 6174 2c20 4e6f   Union[float, No
-00001650: 6e65 5d20 3d20 4e6f 6e65 0d0a 2020 2020  ne] = None..    
-00001660: 2920 2d3e 2049 7465 7261 746f 725b 696e  ) -> Iterator[in
-00001670: 745d 3a0d 0a20 2020 2020 2020 2027 2727  t]:..        '''
-00001680: 0d0a 2020 2020 2020 2020 5275 6e20 616e  ..        Run an
-00001690: 2066 666d 7065 6720 636f 6d6d 616e 642c   ffmpeg command,
-000016a0: 2074 7279 696e 6720 746f 2063 6170 7475   trying to captu
-000016b0: 7265 2074 6865 2070 726f 6365 7373 206f  re the process o
-000016c0: 7574 7075 7420 616e 6420 6361 6c63 756c  utput and calcul
-000016d0: 6174 650d 0a20 2020 2020 2020 2074 6865  ate..        the
-000016e0: 2064 7572 6174 696f 6e20 2f20 7072 6f67   duration / prog
-000016f0: 7265 7373 2e0d 0a20 2020 2020 2020 2059  ress...        Y
-00001700: 6965 6c64 7320 7468 6520 7072 6f67 7265  ields the progre
-00001710: 7373 2069 6e20 7065 7263 656e 742e 0d0a  ss in percent...
-00001720: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
-00001730: 0a20 2020 2020 2020 2020 2020 2070 6f70  .            pop
-00001740: 656e 5f6b 7761 7267 7320 2864 6963 742c  en_kwargs (dict,
-00001750: 206f 7074 696f 6e61 6c29 3a20 4120 6469   optional): A di
-00001760: 6374 2074 6f20 7370 6563 6966 7920 6578  ct to specify ex
-00001770: 7472 6120 6172 6775 6d65 6e74 7320 746f  tra arguments to
-00001780: 2074 6865 2070 6f70 656e 2063 616c 6c2c   the popen call,
-00001790: 2065 2e67 2e20 7b20 6372 6561 7469 6f6e   e.g. { creation
-000017a0: 666c 6167 733a 2043 5245 4154 455f 4e4f  flags: CREATE_NO
-000017b0: 5f57 494e 444f 5720 7d0d 0a20 2020 2020  _WINDOW }..     
-000017c0: 2020 2020 2020 2064 7572 6174 696f 6e5f         duration_
-000017d0: 6f76 6572 7269 6465 2028 666c 6f61 742c  override (float,
-000017e0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
-000017f0: 6475 7261 7469 6f6e 2069 6e20 7365 636f  duration in seco
-00001800: 6e64 732e 2049 6620 6e6f 7420 7370 6563  nds. If not spec
-00001810: 6966 6965 642c 2069 7420 7769 6c6c 2062  ified, it will b
-00001820: 6520 6361 6c63 756c 6174 6564 2066 726f  e calculated fro
-00001830: 6d20 7468 6520 6666 6d70 6567 206f 7574  m the ffmpeg out
-00001840: 7075 742e 0d0a 0d0a 2020 2020 2020 2020  put.....        
-00001850: 5261 6973 6573 3a0d 0a20 2020 2020 2020  Raises:..       
-00001860: 2020 2020 2052 756e 7469 6d65 4572 726f       RuntimeErro
-00001870: 723a 2049 6620 7468 6520 636f 6d6d 616e  r: If the comman
-00001880: 6420 6661 696c 732c 2061 6e20 6578 6365  d fails, an exce
-00001890: 7074 696f 6e20 6973 2072 6169 7365 642e  ption is raised.
-000018a0: 0d0a 0d0a 2020 2020 2020 2020 5969 656c  ....        Yiel
-000018b0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-000018c0: 2049 7465 7261 746f 725b 696e 745d 3a20   Iterator[int]: 
-000018d0: 4120 6765 6e65 7261 746f 7220 7468 6174  A generator that
-000018e0: 2079 6965 6c64 7320 7468 6520 7072 6f67   yields the prog
-000018f0: 7265 7373 2069 6e20 7065 7263 656e 742e  ress in percent.
-00001900: 0d0a 2020 2020 2020 2020 2727 270d 0a20  ..        '''.. 
-00001910: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00001920: 7279 5f72 756e 3a0d 0a20 2020 2020 2020  ry_run:..       
-00001930: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00001940: 2e63 6d64 0d0a 0d0a 2020 2020 2020 2020  .cmd....        
-00001950: 746f 7461 6c5f 6475 723a 2055 6e69 6f6e  total_dur: Union
-00001960: 5b4e 6f6e 652c 2069 6e74 5d20 3d20 4e6f  [None, int] = No
-00001970: 6e65 0d0a 2020 2020 2020 2020 6966 205f  ne..        if _
-00001980: 7573 6573 5f65 7272 6f72 5f6c 6f67 6c65  uses_error_logle
-00001990: 7665 6c28 7365 6c66 2e63 6d64 293a 0d0a  vel(self.cmd):..
-000019a0: 2020 2020 2020 2020 2020 2020 746f 7461              tota
-000019b0: 6c5f 6475 7220 3d20 5f70 726f 6265 5f64  l_dur = _probe_d
-000019c0: 7572 6174 696f 6e28 7365 6c66 2e63 6d64  uration(self.cmd
-000019d0: 290d 0a0d 0a20 2020 2020 2020 2063 6d64  )....        cmd
-000019e0: 5f77 6974 685f 7072 6f67 7265 7373 203d  _with_progress =
-000019f0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00001a00: 5b73 656c 662e 636d 645b 305d 5d20 2b20  [self.cmd[0]] + 
-00001a10: 5b22 2d70 726f 6772 6573 7322 2c20 222d  ["-progress", "-
-00001a20: 222c 2022 2d6e 6f73 7461 7473 225d 202b  ", "-nostats"] +
-00001a30: 2073 656c 662e 636d 645b 313a 5d0d 0a20   self.cmd[1:].. 
-00001a40: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
-00001a50: 2020 2020 7374 6465 7272 203d 205b 5d0d      stderr = [].
-00001a60: 0a20 2020 2020 2020 2062 6173 655f 706f  .        base_po
-00001a70: 7065 6e5f 6b77 6172 6773 203d 2073 656c  pen_kwargs = sel
-00001a80: 662e 6261 7365 5f70 6f70 656e 5f6b 7761  f.base_popen_kwa
-00001a90: 7267 732e 636f 7079 2829 0d0a 2020 2020  rgs.copy()..    
-00001aa0: 2020 2020 6966 2070 6f70 656e 5f6b 7761      if popen_kwa
-00001ab0: 7267 7320 6973 206e 6f74 204e 6f6e 653a  rgs is not None:
-00001ac0: 0d0a 2020 2020 2020 2020 2020 2020 6261  ..            ba
-00001ad0: 7365 5f70 6f70 656e 5f6b 7761 7267 732e  se_popen_kwargs.
-00001ae0: 7570 6461 7465 2870 6f70 656e 5f6b 7761  update(popen_kwa
-00001af0: 7267 7329 0d0a 0d0a 2020 2020 2020 2020  rgs)....        
-00001b00: 6966 2073 7973 2e70 6c61 7466 6f72 6d20  if sys.platform 
-00001b10: 3d3d 2022 7769 6e64 3332 223a 0d0a 2020  == "wind32":..  
-00001b20: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00001b30: 726f 6365 7373 203d 2073 7562 7072 6f63  rocess = subproc
-00001b40: 6573 732e 506f 7065 6e28 0d0a 2020 2020  ess.Popen(..    
-00001b50: 2020 2020 2020 2020 2020 2020 636d 645f              cmd_
-00001b60: 7769 7468 5f70 726f 6772 6573 732c 0d0a  with_progress,..
-00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b80: 2a2a 6261 7365 5f70 6f70 656e 5f6b 7761  **base_popen_kwa
-00001b90: 7267 732c 0d0a 2020 2020 2020 2020 2020  rgs,..          
-00001ba0: 2020 2020 2020 6372 6561 7469 6f6e 666c        creationfl
-00001bb0: 6167 733d 7375 6270 726f 6365 7373 2e43  ags=subprocess.C
-00001bc0: 5245 4154 455f 4e4f 5f57 494e 444f 572c  REATE_NO_WINDOW,
-00001bd0: 0d0a 2020 2020 2020 2020 2020 2020 2920  ..            ) 
-00001be0: 2023 2074 7970 653a 2069 676e 6f72 650d   # type: ignore.
-00001bf0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00001c00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001c10: 2e70 726f 6365 7373 203d 2073 7562 7072  .process = subpr
-00001c20: 6f63 6573 732e 506f 7065 6e28 0d0a 2020  ocess.Popen(..  
-00001c30: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-00001c40: 645f 7769 7468 5f70 726f 6772 6573 732c  d_with_progress,
-00001c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001c60: 2020 2a2a 6261 7365 5f70 6f70 656e 5f6b    **base_popen_k
-00001c70: 7761 7267 732c 0d0a 2020 2020 2020 2020  wargs,..        
-00001c80: 2020 2020 2920 2023 2074 7970 653a 2069      )  # type: i
-00001c90: 676e 6f72 650d 0a0d 0a20 2020 2020 2020  gnore....       
-00001ca0: 2079 6965 6c64 2030 0d0a 0d0a 2020 2020   yield 0....    
-00001cb0: 2020 2020 7768 696c 6520 5472 7565 3a0d      while True:.
-00001cc0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00001cd0: 7365 6c66 2e70 726f 6365 7373 2e73 7464  self.process.std
-00001ce0: 6f75 7420 6973 204e 6f6e 653a 0d0a 2020  out is None:..  
-00001cf0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00001d00: 6e74 696e 7565 0d0a 0d0a 2020 2020 2020  ntinue....      
-00001d10: 2020 2020 2020 7374 6465 7272 5f6c 696e        stderr_lin
-00001d20: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
-00001d30: 2020 2020 2020 2073 656c 662e 7072 6f63         self.proc
-00001d40: 6573 732e 7374 646f 7574 2e72 6561 646c  ess.stdout.readl
-00001d50: 696e 6528 292e 6465 636f 6465 2822 7574  ine().decode("ut
-00001d60: 662d 3822 2c20 6572 726f 7273 3d22 7265  f-8", errors="re
-00001d70: 706c 6163 6522 292e 7374 7269 7028 290d  place").strip().
-00001d80: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-00001d90: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00001da0: 2073 656c 662e 7374 6465 7272 5f63 616c   self.stderr_cal
-00001db0: 6c62 6163 6b3a 0d0a 2020 2020 2020 2020  lback:..        
-00001dc0: 2020 2020 2020 2020 7365 6c66 2e73 7464          self.std
-00001dd0: 6572 725f 6361 6c6c 6261 636b 2873 7464  err_callback(std
-00001de0: 6572 725f 6c69 6e65 290d 0a0d 0a20 2020  err_line)....   
-00001df0: 2020 2020 2020 2020 2069 6620 7374 6465           if stde
-00001e00: 7272 5f6c 696e 6520 3d3d 2027 2720 616e  rr_line == '' an
-00001e10: 6420 7365 6c66 2e70 726f 6365 7373 2e70  d self.process.p
-00001e20: 6f6c 6c28 2920 6973 206e 6f74 204e 6f6e  oll() is not Non
-00001e30: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00001e40: 2020 2020 6272 6561 6b0d 0a0d 0a20 2020      break....   
-00001e50: 2020 2020 2020 2020 2073 7464 6572 722e           stderr.
-00001e60: 6170 7065 6e64 2873 7464 6572 725f 6c69  append(stderr_li
-00001e70: 6e65 2e73 7472 6970 2829 290d 0a0d 0a20  ne.strip()).... 
-00001e80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001e90: 7374 6465 7272 203d 2022 5c6e 222e 6a6f  stderr = "\n".jo
-00001ea0: 696e 2873 7464 6572 7229 0d0a 0d0a 2020  in(stderr)....  
-00001eb0: 2020 2020 2020 2020 2020 6966 2074 6f74            if tot
-00001ec0: 616c 5f64 7572 2069 7320 4e6f 6e65 3a0d  al_dur is None:.
-00001ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ee0: 2074 6f74 616c 5f64 7572 5f6d 6174 6368   total_dur_match
-00001ef0: 203d 2073 656c 662e 4455 525f 5245 4745   = self.DUR_REGE
-00001f00: 582e 7365 6172 6368 2873 7464 6572 725f  X.search(stderr_
-00001f10: 6c69 6e65 290d 0a20 2020 2020 2020 2020  line)..         
-00001f20: 2020 2020 2020 2069 6620 746f 7461 6c5f         if total_
-00001f30: 6475 725f 6d61 7463 683a 0d0a 2020 2020  dur_match:..    
-00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f50: 746f 7461 6c5f 6475 7220 3d20 746f 5f6d  total_dur = to_m
-00001f60: 7328 2a2a 746f 7461 6c5f 6475 725f 6d61  s(**total_dur_ma
-00001f70: 7463 682e 6772 6f75 7064 6963 7428 2929  tch.groupdict())
-00001f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001f90: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
-00001fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fb0: 656c 6966 2064 7572 6174 696f 6e5f 6f76  elif duration_ov
-00001fc0: 6572 7269 6465 2069 7320 6e6f 7420 4e6f  erride is not No
-00001fd0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00001fe0: 2020 2020 2020 2020 2023 2075 7365 2074           # use t
-00001ff0: 6865 206f 7665 7272 6964 6520 2873 686f  he override (sho
-00002000: 756c 6420 6170 706c 7920 696e 2074 6865  uld apply in the
-00002010: 2066 6972 7374 206c 6f6f 7029 0d0a 2020   first loop)..  
-00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002030: 2020 746f 7461 6c5f 6475 7220 3d20 696e    total_dur = in
-00002040: 7428 6475 7261 7469 6f6e 5f6f 7665 7272  t(duration_overr
-00002050: 6964 6520 2a20 3130 3030 290d 0a20 2020  ide * 1000)..   
-00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002070: 2063 6f6e 7469 6e75 650d 0a0d 0a20 2020   continue....   
-00002080: 2020 2020 2020 2020 2069 6620 746f 7461           if tota
-00002090: 6c5f 6475 723a 0d0a 2020 2020 2020 2020  l_dur:..        
-000020a0: 2020 2020 2020 2020 7072 6f67 7265 7373          progress
-000020b0: 5f74 696d 6520 3d20 4666 6d70 6567 5072  _time = FfmpegPr
-000020c0: 6f67 7265 7373 2e54 494d 455f 5245 4745  ogress.TIME_REGE
-000020d0: 582e 7365 6172 6368 2873 7464 6572 725f  X.search(stderr_
-000020e0: 6c69 6e65 290d 0a20 2020 2020 2020 2020  line)..         
-000020f0: 2020 2020 2020 2069 6620 7072 6f67 7265         if progre
-00002100: 7373 5f74 696d 653a 0d0a 2020 2020 2020  ss_time:..      
-00002110: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00002120: 6170 7365 645f 7469 6d65 203d 2074 6f5f  apsed_time = to_
-00002130: 6d73 282a 2a70 726f 6772 6573 735f 7469  ms(**progress_ti
-00002140: 6d65 2e67 726f 7570 6469 6374 2829 290d  me.groupdict()).
-00002150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002160: 2020 2020 2079 6965 6c64 2069 6e74 2865       yield int(e
-00002170: 6c61 7073 6564 5f74 696d 6520 2a20 3130  lapsed_time * 10
-00002180: 302f 2074 6f74 616c 5f64 7572 290d 0a0d  0/ total_dur)...
-00002190: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000021a0: 2e70 726f 6365 7373 2069 7320 4e6f 6e65  .process is None
-000021b0: 206f 7220 7365 6c66 2e70 726f 6365 7373   or self.process
-000021c0: 2e72 6574 7572 6e63 6f64 6520 213d 2030  .returncode != 0
-000021d0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-000021e0: 7072 696e 7428 7365 6c66 2e70 726f 6365  print(self.proce
-000021f0: 7373 290d 0a20 2020 2020 2020 2020 2020  ss)..           
-00002200: 2023 7072 696e 7428 7365 6c66 2e70 726f   #print(self.pro
-00002210: 6365 7373 2e72 6574 7572 6e63 6f64 6529  cess.returncode)
-00002220: 0d0a 2020 2020 2020 2020 2020 2020 5f70  ..            _p
-00002230: 7265 7474 795f 7374 6465 7272 203d 2022  retty_stderr = "
-00002240: 5c6e 222e 6a6f 696e 2873 7464 6572 7229  \n".join(stderr)
-00002250: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-00002260: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
-00002270: 2866 2245 7272 6f72 2072 756e 6e69 6e67  (f"Error running
-00002280: 2063 6f6d 6d61 6e64 207b 7365 6c66 2e63   command {self.c
-00002290: 6d64 7d3a 207b 5f70 7265 7474 795f 7374  md}: {_pretty_st
-000022a0: 6465 7272 7d22 290d 0a0d 0a20 2020 2020  derr}")....     
-000022b0: 2020 2079 6965 6c64 2031 3030 0d0a 2020     yield 100..  
-000022c0: 2020 2020 2020 7365 6c66 2e70 726f 6365        self.proce
-000022d0: 7373 203d 204e 6f6e 650d 0a0d 0a20 2020  ss = None....   
-000022e0: 2064 6566 2071 7569 745f 6772 6163 6566   def quit_gracef
-000022f0: 756c 6c79 2873 656c 6629 202d 3e20 4e6f  ully(self) -> No
-00002300: 6e65 3a0d 0a20 2020 2020 2020 2027 2727  ne:..        '''
-00002310: 0d0a 2020 2020 2020 2020 5175 6974 2074  ..        Quit t
-00002320: 6865 2066 666d 7065 6720 7072 6f63 6573  he ffmpeg proces
-00002330: 7320 6279 2073 656e 6469 6e67 2027 7127  s by sending 'q'
-00002340: 0d0a 0d0a 2020 2020 2020 2020 5261 6973  ....        Rais
-00002350: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
-00002360: 2052 756e 7469 6d65 4572 726f 723a 2049   RuntimeError: I
-00002370: 6620 6e6f 2070 726f 6365 7373 2069 7320  f no process is 
-00002380: 666f 756e 642e 0d0a 2020 2020 2020 2020  found...        
-00002390: 2727 270d 0a20 2020 2020 2020 2069 6620  '''..        if 
-000023a0: 7365 6c66 2e70 726f 6365 7373 2069 7320  self.process is 
-000023b0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-000023c0: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
-000023d0: 4572 726f 7228 224e 6f20 7072 6f63 6573  Error("No proces
-000023e0: 7320 666f 756e 642e 2044 6964 2079 6f75  s found. Did you
-000023f0: 2072 756e 2074 6865 2063 6f6d 6d61 6e64   run the command
-00002400: 3f22 290d 0a0d 0a20 2020 2020 2020 2073  ?")....        s
-00002410: 656c 662e 7072 6f63 6573 732e 636f 6d6d  elf.process.comm
-00002420: 756e 6963 6174 6528 696e 7075 743d 6222  unicate(input=b"
-00002430: 7122 290d 0a20 2020 2020 2020 2073 656c  q")..        sel
-00002440: 662e 7072 6f63 6573 732e 6b69 6c6c 2829  f.process.kill()
-00002450: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-00002460: 726f 6365 7373 203d 204e 6f6e 650d 0a0d  rocess = None...
-00002470: 0a20 2020 2064 6566 2071 7569 7428 7365  .    def quit(se
-00002480: 6c66 2920 2d3e 204e 6f6e 653a 0d0a 2020  lf) -> None:..  
-00002490: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
-000024a0: 2020 2051 7569 7420 7468 6520 6666 6d70     Quit the ffmp
-000024b0: 6567 2070 726f 6365 7373 2062 7920 7365  eg process by se
-000024c0: 6e64 696e 6720 5349 474b 494c 4c2e 0d0a  nding SIGKILL...
-000024d0: 0d0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
-000024e0: 3a0d 0a20 2020 2020 2020 2020 2020 2052  :..            R
-000024f0: 756e 7469 6d65 4572 726f 723a 2049 6620  untimeError: If 
-00002500: 6e6f 2070 726f 6365 7373 2069 7320 666f  no process is fo
-00002510: 756e 642e 0d0a 2020 2020 2020 2020 2727  und...        ''
-00002520: 270d 0a20 2020 2020 2020 2069 6620 7365  '..        if se
-00002530: 6c66 2e70 726f 6365 7373 2069 7320 4e6f  lf.process is No
-00002540: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00002550: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
-00002560: 726f 7228 224e 6f20 7072 6f63 6573 7320  ror("No process 
-00002570: 666f 756e 642e 2044 6964 2079 6f75 2072  found. Did you r
-00002580: 756e 2074 6865 2063 6f6d 6d61 6e64 3f22  un the command?"
-00002590: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
-000025a0: 662e 7072 6f63 6573 732e 6b69 6c6c 2829  f.process.kill()
-000025b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-000025c0: 726f 6365 7373 203d 204e 6f6e 650d 0a0d  rocess = None...
-000025d0: 0a0d 0a23 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ...#============
-000025e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000025f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002600: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002610: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002620: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002630: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002640: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002650: 3d3d 3d3d 3d3d 3d3d 3d3d 3d23 0d0a 0d0a  ===========#....
-00002660: 0d0a 6465 6620 7374 6f70 5f66 666d 7065  ..def stop_ffmpe
-00002670: 675f 7769 6e64 6f77 7328 6572 726f 725f  g_windows(error_
-00002680: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-00002690: 6b3d 4e6f 6e65 293a 0d0a 2020 2020 7472  k=None):..    tr
-000026a0: 793a 0d0a 2020 2020 2020 2020 7461 736b  y:..        task
-000026b0: 6c69 7374 5f6f 7574 7075 7420 3d20 7375  list_output = su
-000026c0: 6270 726f 6365 7373 2e63 6865 636b 5f6f  bprocess.check_o
-000026d0: 7574 7075 7428 5b27 7461 736b 6c69 7374  utput(['tasklist
-000026e0: 275d 2c20 6372 6561 7469 6f6e 666c 6167  '], creationflag
-000026f0: 733d 7375 6270 726f 6365 7373 2e43 5245  s=subprocess.CRE
-00002700: 4154 455f 4e4f 5f57 494e 444f 5729 2e64  ATE_NO_WINDOW).d
-00002710: 6563 6f64 6528 2775 7466 2d38 2729 0d0a  ecode('utf-8')..
-00002720: 2020 2020 2020 2020 6666 6d70 6567 5f70          ffmpeg_p
-00002730: 6964 203d 204e 6f6e 650d 0a20 2020 2020  id = None..     
-00002740: 2020 2066 6f72 206c 696e 6520 696e 2074     for line in t
-00002750: 6173 6b6c 6973 745f 6f75 7470 7574 2e73  asklist_output.s
-00002760: 706c 6974 2827 5c6e 2729 3a0d 0a20 2020  plit('\n'):..   
-00002770: 2020 2020 2020 2020 2069 6620 2266 666d           if "ffm
-00002780: 7065 6722 2069 6e20 6c69 6e65 3a0d 0a20  peg" in line:.. 
-00002790: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000027a0: 666d 7065 675f 7069 6420 3d20 6c69 6e65  fmpeg_pid = line
-000027b0: 2e73 706c 6974 2829 5b31 5d0d 0a20 2020  .split()[1]..   
-000027c0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-000027d0: 616b 0d0a 2020 2020 2020 2020 6966 2066  ak..        if f
-000027e0: 666d 7065 675f 7069 643a 0d0a 2020 2020  fmpeg_pid:..    
-000027f0: 2020 2020 2020 2020 6465 766e 756c 6c20          devnull 
-00002800: 3d20 6f70 656e 286f 732e 6465 766e 756c  = open(os.devnul
-00002810: 6c2c 2027 7727 290d 0a20 2020 2020 2020  l, 'w')..       
-00002820: 2020 2020 2073 7562 7072 6f63 6573 732e       subprocess.
-00002830: 506f 7065 6e28 5b27 7461 736b 6b69 6c6c  Popen(['taskkill
-00002840: 272c 2027 2f46 272c 2027 2f54 272c 2027  ', '/F', '/T', '
-00002850: 2f50 4944 272c 2066 666d 7065 675f 7069  /PID', ffmpeg_pi
-00002860: 645d 2c20 7374 646f 7574 3d73 7562 7072  d], stdout=subpr
-00002870: 6f63 6573 732e 5049 5045 2c20 7374 6465  ocess.PIPE, stde
-00002880: 7272 3d73 7562 7072 6f63 6573 732e 5354  rr=subprocess.ST
-00002890: 444f 5554 2c20 7368 656c 6c3d 5472 7565  DOUT, shell=True
-000028a0: 2c20 6372 6561 7469 6f6e 666c 6167 733d  , creationflags=
-000028b0: 7375 6270 726f 6365 7373 2e43 5245 4154  subprocess.CREAT
-000028c0: 455f 4e4f 5f57 494e 444f 5729 0d0a 0d0a  E_NO_WINDOW)....
-000028d0: 2020 2020 6578 6365 7074 204b 6579 626f      except Keybo
-000028e0: 6172 6449 6e74 6572 7275 7074 3a0d 0a20  ardInterrupt:.. 
-000028f0: 2020 2020 2020 2069 6620 6572 726f 725f         if error_
-00002900: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-00002910: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
-00002920: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-00002930: 616c 6c62 6163 6b28 2243 616e 6365 6c6c  allback("Cancell
-00002940: 696e 6720 616c 6c20 7461 736b 7322 290d  ing all tasks").
-00002950: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00002960: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00002970: 7428 2243 616e 6365 6c6c 696e 6720 616c  t("Cancelling al
-00002980: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
-00002990: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
-000029a0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-000029b0: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
-000029c0: 2069 6620 6572 726f 725f 6d65 7373 6167   if error_messag
-000029d0: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
-000029e0: 2020 2020 2020 2020 2020 6572 726f 725f            error_
-000029f0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-00002a00: 6b28 6529 0d0a 2020 2020 2020 2020 656c  k(e)..        el
-00002a10: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00002a20: 2070 7269 6e74 2865 290d 0a20 2020 2020   print(e)..     
-00002a30: 2020 2072 6574 7572 6e0d 0a0d 0a0d 0a64     return......d
-00002a40: 6566 2073 746f 705f 6666 6d70 6567 5f6c  ef stop_ffmpeg_l
-00002a50: 696e 7578 2865 7272 6f72 5f6d 6573 7361  inux(error_messa
-00002a60: 6765 735f 6361 6c6c 6261 636b 3d4e 6f6e  ges_callback=Non
-00002a70: 6529 3a0d 0a20 2020 2070 726f 6365 7373  e):..    process
-00002a80: 5f6e 616d 6520 3d20 2766 666d 7065 6727  _name = 'ffmpeg'
-00002a90: 0d0a 2020 2020 7472 793a 0d0a 2020 2020  ..    try:..    
-00002aa0: 2020 2020 6f75 7470 7574 203d 2073 7562      output = sub
-00002ab0: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
-00002ac0: 7470 7574 285b 2770 7327 2c20 272d 6566  tput(['ps', '-ef
-00002ad0: 275d 290d 0a20 2020 2020 2020 2070 6964  '])..        pid
-00002ae0: 203d 205b 6c69 6e65 2e73 706c 6974 2829   = [line.split()
-00002af0: 5b31 5d20 666f 7220 6c69 6e65 2069 6e20  [1] for line in 
-00002b00: 6f75 7470 7574 2e64 6563 6f64 6528 2775  output.decode('u
-00002b10: 7466 2d38 2729 2e73 706c 6974 2827 5c6e  tf-8').split('\n
-00002b20: 2729 2069 6620 7072 6f63 6573 735f 6e61  ') if process_na
-00002b30: 6d65 2069 6e20 6c69 6e65 5d5b 305d 0d0a  me in line][0]..
-00002b40: 2020 2020 2020 2020 7375 6270 726f 6365          subproce
-00002b50: 7373 2e63 616c 6c28 5b27 6b69 6c6c 272c  ss.call(['kill',
-00002b60: 2027 2d39 272c 2073 7472 2870 6964 295d   '-9', str(pid)]
-00002b70: 290d 0a20 2020 2020 2020 2023 7072 696e  )..        #prin
-00002b80: 7428 6622 7b70 726f 6365 7373 5f6e 616d  t(f"{process_nam
-00002b90: 657d 2068 6173 2062 6565 6e20 6b69 6c6c  e} has been kill
-00002ba0: 6564 2229 0d0a 2020 2020 6578 6365 7074  ed")..    except
-00002bb0: 2049 6e64 6578 4572 726f 723a 0d0a 2020   IndexError:..  
-00002bc0: 2020 2020 2020 2370 7269 6e74 2866 227b        #print(f"{
-00002bd0: 7072 6f63 6573 735f 6e61 6d65 7d20 6973  process_name} is
-00002be0: 206e 6f74 2072 756e 6e69 6e67 2229 0d0a   not running")..
-00002bf0: 2020 2020 2020 2020 7061 7373 0d0a 0d0a          pass....
-00002c00: 2020 2020 6578 6365 7074 204b 6579 626f      except Keybo
-00002c10: 6172 6449 6e74 6572 7275 7074 3a0d 0a20  ardInterrupt:.. 
-00002c20: 2020 2020 2020 2069 6620 6572 726f 725f         if error_
-00002c30: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-00002c40: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
-00002c50: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-00002c60: 616c 6c62 6163 6b28 2243 616e 6365 6c6c  allback("Cancell
-00002c70: 696e 6720 616c 6c20 7461 736b 7322 290d  ing all tasks").
-00002c80: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00002c90: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00002ca0: 7428 2243 616e 6365 6c6c 696e 6720 616c  t("Cancelling al
-00002cb0: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
-00002cc0: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
-00002cd0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00002ce0: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
-00002cf0: 2069 6620 6572 726f 725f 6d65 7373 6167   if error_messag
-00002d00: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
-00002d10: 2020 2020 2020 2020 2020 6572 726f 725f            error_
-00002d20: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-00002d30: 6b28 6529 0d0a 2020 2020 2020 2020 656c  k(e)..        el
-00002d40: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00002d50: 2070 7269 6e74 2865 290d 0a20 2020 2020   print(e)..     
-00002d60: 2020 2072 6574 7572 6e0d 0a0d 0a0d 0a64     return......d
-00002d70: 6566 2072 656d 6f76 655f 7465 6d70 5f66  ef remove_temp_f
-00002d80: 696c 6573 2865 7874 656e 7369 6f6e 2c20  iles(extension, 
-00002d90: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-00002da0: 616c 6c62 6163 6b3d 4e6f 6e65 293a 0d0a  allback=None):..
-00002db0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00002dc0: 2020 7465 6d70 5f64 6972 203d 2074 656d    temp_dir = tem
-00002dd0: 7066 696c 652e 6765 7474 656d 7064 6972  pfile.gettempdir
-00002de0: 2829 0d0a 2020 2020 2020 2020 666f 7220  ()..        for 
-00002df0: 726f 6f74 2c20 6469 7273 2c20 6669 6c65  root, dirs, file
-00002e00: 7320 696e 206f 732e 7761 6c6b 2874 656d  s in os.walk(tem
-00002e10: 705f 6469 7229 3a0d 0a20 2020 2020 2020  p_dir):..       
-00002e20: 2020 2020 2066 6f72 2066 696c 6520 696e       for file in
-00002e30: 2066 696c 6573 3a0d 0a20 2020 2020 2020   files:..       
-00002e40: 2020 2020 2020 2020 2069 6620 6669 6c65           if file
-00002e50: 2e65 6e64 7377 6974 6828 222e 2220 2b20  .endswith("." + 
-00002e60: 6578 7465 6e73 696f 6e29 3a0d 0a20 2020  extension):..   
-00002e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e80: 206f 732e 7265 6d6f 7665 286f 732e 7061   os.remove(os.pa
-00002e90: 7468 2e6a 6f69 6e28 726f 6f74 2c20 6669  th.join(root, fi
-00002ea0: 6c65 2929 0d0a 2020 2020 6578 6365 7074  le))..    except
-00002eb0: 204b 6579 626f 6172 6449 6e74 6572 7275   KeyboardInterru
-00002ec0: 7074 3a0d 0a20 2020 2020 2020 2069 6620  pt:..        if 
-00002ed0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-00002ee0: 616c 6c62 6163 6b3a 0d0a 2020 2020 2020  allback:..      
-00002ef0: 2020 2020 2020 6572 726f 725f 6d65 7373        error_mess
-00002f00: 6167 6573 5f63 616c 6c62 6163 6b28 2243  ages_callback("C
-00002f10: 616e 6365 6c6c 696e 6720 616c 6c20 7461  ancelling all ta
-00002f20: 736b 7322 290d 0a20 2020 2020 2020 2065  sks")..        e
-00002f30: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00002f40: 2020 7072 696e 7428 2243 616e 6365 6c6c    print("Cancell
-00002f50: 696e 6720 616c 6c20 7461 736b 7322 290d  ing all tasks").
-00002f60: 0a20 2020 2020 2020 2072 6574 7572 6e0d  .        return.
-00002f70: 0a0d 0a20 2020 2065 7863 6570 7420 4578  ...    except Ex
-00002f80: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
-00002f90: 2020 2020 2020 2069 6620 6572 726f 725f         if error_
-00002fa0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-00002fb0: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
-00002fc0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-00002fd0: 616c 6c62 6163 6b28 6529 0d0a 2020 2020  allback(e)..    
-00002fe0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00002ff0: 2020 2020 2020 2070 7269 6e74 2865 290d         print(e).
-00003000: 0a20 2020 2020 2020 2072 6574 7572 6e0d  .        return.
-00003010: 0a0d 0a0d 0a64 6566 2069 735f 7361 6d65  .....def is_same
-00003020: 5f6c 616e 6775 6167 6528 7372 632c 2064  _language(src, d
-00003030: 7374 2c20 6572 726f 725f 6d65 7373 6167  st, error_messag
-00003040: 6573 5f63 616c 6c62 6163 6b3d 4e6f 6e65  es_callback=None
-00003050: 293a 0d0a 2020 2020 7472 793a 0d0a 2020  ):..    try:..  
-00003060: 2020 2020 2020 7265 7475 726e 2073 7263        return src
-00003070: 2e73 706c 6974 2822 2d22 295b 305d 203d  .split("-")[0] =
-00003080: 3d20 6473 742e 7370 6c69 7428 222d 2229  = dst.split("-")
-00003090: 5b30 5d0d 0a20 2020 2065 7863 6570 7420  [0]..    except 
-000030a0: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
-000030b0: 0a20 2020 2020 2020 2069 6620 6572 726f  .        if erro
-000030c0: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-000030d0: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
-000030e0: 2020 6572 726f 725f 6d65 7373 6167 6573    error_messages
-000030f0: 5f63 616c 6c62 6163 6b28 6529 0d0a 2020  _callback(e)..  
-00003100: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00003110: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
-00003120: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00003130: 6e0d 0a0d 0a0d 0a64 6566 2063 6865 636b  n......def check
-00003140: 5f66 696c 655f 7479 7065 2866 696c 655f  _file_type(file_
-00003150: 7061 7468 2c20 6572 726f 725f 6d65 7373  path, error_mess
-00003160: 6167 6573 5f63 616c 6c62 6163 6b3d 4e6f  ages_callback=No
-00003170: 6e65 293a 0d0a 2020 2020 7472 793a 0d0a  ne):..    try:..
-00003180: 2020 2020 2020 2020 6666 7072 6f62 655f          ffprobe_
-00003190: 636d 6420 3d20 5b27 6666 7072 6f62 6527  cmd = ['ffprobe'
-000031a0: 2c20 272d 7627 2c20 2765 7272 6f72 272c  , '-v', 'error',
-000031b0: 2027 2d73 686f 775f 666f 726d 6174 272c   '-show_format',
-000031c0: 2027 2d73 686f 775f 7374 7265 616d 7327   '-show_streams'
-000031d0: 2c20 272d 7072 696e 745f 666f 726d 6174  , '-print_format
-000031e0: 272c 2027 6a73 6f6e 272c 2066 696c 655f  ', 'json', file_
-000031f0: 7061 7468 5d0d 0a20 2020 2020 2020 206f  path]..        o
-00003200: 7574 7075 7420 3d20 4e6f 6e65 0d0a 2020  utput = None..  
-00003210: 2020 2020 2020 6966 2073 7973 2e70 6c61        if sys.pla
-00003220: 7466 6f72 6d20 3d3d 2022 7769 6e33 3222  tform == "win32"
-00003230: 3a0d 0a20 2020 2020 2020 2020 2020 206f  :..            o
-00003240: 7574 7075 7420 3d20 7375 6270 726f 6365  utput = subproce
-00003250: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
-00003260: 6666 7072 6f62 655f 636d 642c 2063 7265  ffprobe_cmd, cre
-00003270: 6174 696f 6e66 6c61 6773 3d73 7562 7072  ationflags=subpr
-00003280: 6f63 6573 732e 4352 4541 5445 5f4e 4f5f  ocess.CREATE_NO_
-00003290: 5749 4e44 4f57 292e 6465 636f 6465 2827  WINDOW).decode('
-000032a0: 7574 662d 3827 290d 0a20 2020 2020 2020  utf-8')..       
-000032b0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-000032c0: 2020 2020 6f75 7470 7574 203d 2073 7562      output = sub
-000032d0: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
-000032e0: 7470 7574 2866 6670 726f 6265 5f63 6d64  tput(ffprobe_cmd
-000032f0: 292e 6465 636f 6465 2827 7574 662d 3827  ).decode('utf-8'
-00003300: 290d 0a20 2020 2020 2020 2064 6174 6120  )..        data 
-00003310: 3d20 6a73 6f6e 2e6c 6f61 6473 286f 7574  = json.loads(out
-00003320: 7075 7429 0d0a 0d0a 2020 2020 2020 2020  put)....        
-00003330: 6966 2027 7374 7265 616d 7327 2069 6e20  if 'streams' in 
-00003340: 6461 7461 3a0d 0a20 2020 2020 2020 2020  data:..         
-00003350: 2020 2066 6f72 2073 7472 6561 6d20 696e     for stream in
-00003360: 2064 6174 615b 2773 7472 6561 6d73 275d   data['streams']
-00003370: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00003380: 2020 2069 6620 2763 6f64 6563 5f74 7970     if 'codec_typ
-00003390: 6527 2069 6e20 7374 7265 616d 2061 6e64  e' in stream and
-000033a0: 2073 7472 6561 6d5b 2763 6f64 6563 5f74   stream['codec_t
-000033b0: 7970 6527 5d20 3d3d 2027 6175 6469 6f27  ype'] == 'audio'
-000033c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000033d0: 2020 2020 2020 2072 6574 7572 6e20 2761         return 'a
-000033e0: 7564 696f 270d 0a20 2020 2020 2020 2020  udio'..         
-000033f0: 2020 2020 2020 2065 6c69 6620 2763 6f64         elif 'cod
-00003400: 6563 5f74 7970 6527 2069 6e20 7374 7265  ec_type' in stre
-00003410: 616d 2061 6e64 2073 7472 6561 6d5b 2763  am and stream['c
-00003420: 6f64 6563 5f74 7970 6527 5d20 3d3d 2027  odec_type'] == '
-00003430: 7669 6465 6f27 3a0d 0a20 2020 2020 2020  video':..       
-00003440: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00003450: 7572 6e20 2776 6964 656f 270d 0a20 2020  urn 'video'..   
-00003460: 2065 7863 6570 7420 2873 7562 7072 6f63   except (subproc
-00003470: 6573 732e 4361 6c6c 6564 5072 6f63 6573  ess.CalledProces
-00003480: 7345 7272 6f72 2c20 6a73 6f6e 2e4a 534f  sError, json.JSO
-00003490: 4e44 6563 6f64 6545 7272 6f72 293a 0d0a  NDecodeError):..
-000034a0: 2020 2020 2020 2020 7061 7373 0d0a 0d0a          pass....
-000034b0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-000034c0: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
-000034d0: 2020 2020 6966 2065 7272 6f72 5f6d 6573      if error_mes
-000034e0: 7361 6765 735f 6361 6c6c 6261 636b 3a0d  sages_callback:.
-000034f0: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
-00003500: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-00003510: 6261 636b 2865 290d 0a20 2020 2020 2020  back(e)..       
-00003520: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00003530: 2020 2020 7072 696e 7428 6529 0d0a 0d0a      print(e)....
-00003540: 2020 2020 7265 7475 726e 204e 6f6e 650d      return None.
-00003550: 0a0d 0a0d 0a63 6c61 7373 2057 6869 7370  .....class Whisp
-00003560: 6572 4c61 6e67 7561 6765 3a0d 0a20 2020  erLanguage:..   
-00003570: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00003580: 6c66 293a 0d0a 2020 2020 2020 2020 7365  lf):..        se
-00003590: 6c66 2e6c 6973 745f 636f 6465 7320 3d20  lf.list_codes = 
-000035a0: 5b5d 0d0a 2020 2020 2020 2020 7365 6c66  []..        self
-000035b0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-000035c0: 6e64 2822 6166 2229 0d0a 2020 2020 2020  nd("af")..      
-000035d0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-000035e0: 732e 6170 7065 6e64 2822 7371 2229 0d0a  s.append("sq")..
-000035f0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00003600: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00003610: 616d 2229 0d0a 2020 2020 2020 2020 7365  am")..        se
-00003620: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00003630: 7065 6e64 2822 6172 2229 0d0a 2020 2020  pend("ar")..    
-00003640: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00003650: 6465 732e 6170 7065 6e64 2822 6879 2229  des.append("hy")
-00003660: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00003670: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00003680: 2822 6173 2229 0d0a 2020 2020 2020 2020  ("as")..        
-00003690: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-000036a0: 6170 7065 6e64 2822 617a 2229 0d0a 2020  append("az")..  
-000036b0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000036c0: 636f 6465 732e 6170 7065 6e64 2822 6261  codes.append("ba
-000036d0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000036e0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-000036f0: 6e64 2822 6575 2229 0d0a 2020 2020 2020  nd("eu")..      
-00003700: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00003710: 732e 6170 7065 6e64 2822 6265 2229 0d0a  s.append("be")..
-00003720: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00003730: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00003740: 626e 2229 0d0a 2020 2020 2020 2020 7365  bn")..        se
-00003750: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00003760: 7065 6e64 2822 6273 2229 0d0a 2020 2020  pend("bs")..    
-00003770: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00003780: 6465 732e 6170 7065 6e64 2822 6272 2229  des.append("br")
-00003790: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000037a0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-000037b0: 2822 6267 2229 0d0a 2020 2020 2020 2020  ("bg")..        
-000037c0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-000037d0: 6170 7065 6e64 2822 6361 2229 0d0a 2020  append("ca")..  
-000037e0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000037f0: 636f 6465 732e 6170 7065 6e64 2822 7a68  codes.append("zh
-00003800: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00003810: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00003820: 6e64 2822 6872 2229 0d0a 2020 2020 2020  nd("hr")..      
-00003830: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00003840: 732e 6170 7065 6e64 2822 6373 2229 0d0a  s.append("cs")..
-00003850: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00003860: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00003870: 6461 2229 0d0a 2020 2020 2020 2020 7365  da")..        se
-00003880: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00003890: 7065 6e64 2822 6e6c 2229 0d0a 2020 2020  pend("nl")..    
-000038a0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000038b0: 6465 732e 6170 7065 6e64 2822 656e 2229  des.append("en")
-000038c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000038d0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-000038e0: 2822 6574 2229 0d0a 2020 2020 2020 2020  ("et")..        
-000038f0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00003900: 6170 7065 6e64 2822 666f 2229 0d0a 2020  append("fo")..  
-00003910: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00003920: 636f 6465 732e 6170 7065 6e64 2822 6669  codes.append("fi
-00003930: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00003940: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00003950: 6e64 2822 6672 2229 0d0a 2020 2020 2020  nd("fr")..      
-00003960: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00003970: 732e 6170 7065 6e64 2822 676c 2229 0d0a  s.append("gl")..
-00003980: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00003990: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-000039a0: 6b61 2229 0d0a 2020 2020 2020 2020 7365  ka")..        se
-000039b0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-000039c0: 7065 6e64 2822 6465 2229 0d0a 2020 2020  pend("de")..    
-000039d0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000039e0: 6465 732e 6170 7065 6e64 2822 656c 2229  des.append("el")
-000039f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00003a00: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00003a10: 2822 6775 2229 0d0a 2020 2020 2020 2020  ("gu")..        
-00003a20: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00003a30: 6170 7065 6e64 2822 6874 2229 0d0a 2020  append("ht")..  
-00003a40: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00003a50: 636f 6465 732e 6170 7065 6e64 2822 6861  codes.append("ha
-00003a60: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00003a70: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00003a80: 6e64 2822 6861 7722 290d 0a20 2020 2020  nd("haw")..     
-00003a90: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00003aa0: 6573 2e61 7070 656e 6428 2268 6522 290d  es.append("he").
-00003ab0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00003ac0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00003ad0: 2268 6922 290d 0a20 2020 2020 2020 2073  "hi")..        s
-00003ae0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00003af0: 7070 656e 6428 2268 7522 290d 0a20 2020  ppend("hu")..   
-00003b00: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00003b10: 6f64 6573 2e61 7070 656e 6428 2269 7322  odes.append("is"
-00003b20: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003b30: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00003b40: 6428 2269 6422 290d 0a20 2020 2020 2020  d("id")..       
-00003b50: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00003b60: 2e61 7070 656e 6428 2269 7422 290d 0a20  .append("it").. 
-00003b70: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00003b80: 5f63 6f64 6573 2e61 7070 656e 6428 226a  _codes.append("j
-00003b90: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
-00003ba0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00003bb0: 656e 6428 226a 7622 290d 0a20 2020 2020  end("jv")..     
-00003bc0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00003bd0: 6573 2e61 7070 656e 6428 226b 6e22 290d  es.append("kn").
-00003be0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00003bf0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00003c00: 226b 6b22 290d 0a20 2020 2020 2020 2073  "kk")..        s
-00003c10: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00003c20: 7070 656e 6428 226b 6d22 290d 0a20 2020  ppend("km")..   
-00003c30: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00003c40: 6f64 6573 2e61 7070 656e 6428 226b 6f22  odes.append("ko"
-00003c50: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003c60: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00003c70: 6428 226c 6f22 290d 0a20 2020 2020 2020  d("lo")..       
-00003c80: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00003c90: 2e61 7070 656e 6428 226c 6122 290d 0a20  .append("la").. 
-00003ca0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00003cb0: 5f63 6f64 6573 2e61 7070 656e 6428 226c  _codes.append("l
-00003cc0: 7622 290d 0a20 2020 2020 2020 2073 656c  v")..        sel
-00003cd0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00003ce0: 656e 6428 226c 6e22 290d 0a20 2020 2020  end("ln")..     
-00003cf0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00003d00: 6573 2e61 7070 656e 6428 226c 7422 290d  es.append("lt").
-00003d10: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00003d20: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00003d30: 226c 6222 290d 0a20 2020 2020 2020 2073  "lb")..        s
-00003d40: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00003d50: 7070 656e 6428 226d 6b22 290d 0a20 2020  ppend("mk")..   
-00003d60: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00003d70: 6f64 6573 2e61 7070 656e 6428 226d 6722  odes.append("mg"
-00003d80: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003d90: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00003da0: 6428 226d 7322 290d 0a20 2020 2020 2020  d("ms")..       
-00003db0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00003dc0: 2e61 7070 656e 6428 226d 6c22 290d 0a20  .append("ml").. 
-00003dd0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00003de0: 5f63 6f64 6573 2e61 7070 656e 6428 226d  _codes.append("m
-00003df0: 7422 290d 0a20 2020 2020 2020 2073 656c  t")..        sel
-00003e00: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00003e10: 656e 6428 226d 6922 290d 0a20 2020 2020  end("mi")..     
-00003e20: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00003e30: 6573 2e61 7070 656e 6428 226d 7222 290d  es.append("mr").
-00003e40: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00003e50: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00003e60: 226d 6e22 290d 0a20 2020 2020 2020 2073  "mn")..        s
-00003e70: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00003e80: 7070 656e 6428 226d 7922 290d 0a20 2020  ppend("my")..   
-00003e90: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00003ea0: 6f64 6573 2e61 7070 656e 6428 226e 6522  odes.append("ne"
-00003eb0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003ec0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00003ed0: 6428 226e 6f22 290d 0a20 2020 2020 2020  d("no")..       
-00003ee0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00003ef0: 2e61 7070 656e 6428 226e 6e22 290d 0a20  .append("nn").. 
-00003f00: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00003f10: 5f63 6f64 6573 2e61 7070 656e 6428 226f  _codes.append("o
-00003f20: 6322 290d 0a20 2020 2020 2020 2073 656c  c")..        sel
-00003f30: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00003f40: 656e 6428 2270 7322 290d 0a20 2020 2020  end("ps")..     
-00003f50: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00003f60: 6573 2e61 7070 656e 6428 2266 6122 290d  es.append("fa").
-00003f70: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00003f80: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00003f90: 2270 6c22 290d 0a20 2020 2020 2020 2073  "pl")..        s
-00003fa0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00003fb0: 7070 656e 6428 2270 7422 290d 0a20 2020  ppend("pt")..   
-00003fc0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00003fd0: 6f64 6573 2e61 7070 656e 6428 2270 6122  odes.append("pa"
-00003fe0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003ff0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00004000: 6428 2272 6f22 290d 0a20 2020 2020 2020  d("ro")..       
-00004010: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00004020: 2e61 7070 656e 6428 2272 7522 290d 0a20  .append("ru").. 
-00004030: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00004040: 5f63 6f64 6573 2e61 7070 656e 6428 2273  _codes.append("s
-00004050: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
-00004060: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00004070: 656e 6428 2273 7222 290d 0a20 2020 2020  end("sr")..     
-00004080: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00004090: 6573 2e61 7070 656e 6428 2273 6e22 290d  es.append("sn").
-000040a0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000040b0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-000040c0: 2273 6422 290d 0a20 2020 2020 2020 2073  "sd")..        s
-000040d0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-000040e0: 7070 656e 6428 2273 6922 290d 0a20 2020  ppend("si")..   
-000040f0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00004100: 6f64 6573 2e61 7070 656e 6428 2273 6b22  odes.append("sk"
-00004110: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004120: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00004130: 6428 2273 6c22 290d 0a20 2020 2020 2020  d("sl")..       
-00004140: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00004150: 2e61 7070 656e 6428 2273 6f22 290d 0a20  .append("so").. 
-00004160: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00004170: 5f63 6f64 6573 2e61 7070 656e 6428 2265  _codes.append("e
-00004180: 7322 290d 0a20 2020 2020 2020 2073 656c  s")..        sel
-00004190: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-000041a0: 656e 6428 2273 7522 290d 0a20 2020 2020  end("su")..     
-000041b0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-000041c0: 6573 2e61 7070 656e 6428 2273 7722 290d  es.append("sw").
-000041d0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000041e0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-000041f0: 2273 7622 290d 0a20 2020 2020 2020 2073  "sv")..        s
-00004200: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00004210: 7070 656e 6428 2274 6c22 290d 0a20 2020  ppend("tl")..   
-00004220: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00004230: 6f64 6573 2e61 7070 656e 6428 2274 6722  odes.append("tg"
-00004240: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004250: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00004260: 6428 2274 6122 290d 0a20 2020 2020 2020  d("ta")..       
-00004270: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00004280: 2e61 7070 656e 6428 2274 7422 290d 0a20  .append("tt").. 
-00004290: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000042a0: 5f63 6f64 6573 2e61 7070 656e 6428 2274  _codes.append("t
-000042b0: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
-000042c0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-000042d0: 656e 6428 2274 6822 290d 0a20 2020 2020  end("th")..     
-000042e0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-000042f0: 6573 2e61 7070 656e 6428 2262 6f22 290d  es.append("bo").
-00004300: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004310: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00004320: 2274 7222 290d 0a20 2020 2020 2020 2073  "tr")..        s
-00004330: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00004340: 7070 656e 6428 2274 6b22 290d 0a20 2020  ppend("tk")..   
-00004350: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00004360: 6f64 6573 2e61 7070 656e 6428 2275 6b22  odes.append("uk"
-00004370: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004380: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00004390: 6428 2275 7222 290d 0a20 2020 2020 2020  d("ur")..       
-000043a0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-000043b0: 2e61 7070 656e 6428 2275 7a22 290d 0a20  .append("uz").. 
-000043c0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000043d0: 5f63 6f64 6573 2e61 7070 656e 6428 2276  _codes.append("v
-000043e0: 6922 290d 0a20 2020 2020 2020 2073 656c  i")..        sel
-000043f0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00004400: 656e 6428 2263 7922 290d 0a20 2020 2020  end("cy")..     
-00004410: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00004420: 6573 2e61 7070 656e 6428 2279 6922 290d  es.append("yi").
-00004430: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004440: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00004450: 2279 6f22 290d 0a0d 0a20 2020 2020 2020  "yo")....       
-00004460: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004470: 203d 205b 5d0d 0a20 2020 2020 2020 2073   = []..        s
-00004480: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00004490: 7070 656e 6428 2241 6672 696b 6161 6e73  ppend("Afrikaans
-000044a0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000044b0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-000044c0: 6e64 2822 416c 6261 6e69 616e 2229 0d0a  nd("Albanian")..
-000044d0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000044e0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000044f0: 416d 6861 7269 6322 290d 0a20 2020 2020  Amharic")..     
-00004500: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00004510: 6573 2e61 7070 656e 6428 2241 7261 6269  es.append("Arabi
-00004520: 6322 290d 0a20 2020 2020 2020 2073 656c  c")..        sel
-00004530: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00004540: 656e 6428 2241 726d 656e 6961 6e22 290d  end("Armenian").
-00004550: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004560: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00004570: 2241 7373 616d 6573 6522 290d 0a20 2020  "Assamese")..   
-00004580: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004590: 616d 6573 2e61 7070 656e 6428 2241 7a65  ames.append("Aze
-000045a0: 7262 6169 6a61 6e69 2229 0d0a 2020 2020  rbaijani")..    
-000045b0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-000045c0: 6d65 732e 6170 7065 6e64 2822 4261 7368  mes.append("Bash
-000045d0: 6b69 7222 290d 0a20 2020 2020 2020 2073  kir")..        s
-000045e0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-000045f0: 7070 656e 6428 2242 6173 7175 6522 290d  ppend("Basque").
-00004600: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004610: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00004620: 2242 656c 6172 7573 6961 6e22 290d 0a20  "Belarusian").. 
-00004630: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00004640: 5f6e 616d 6573 2e61 7070 656e 6428 2242  _names.append("B
-00004650: 656e 6761 6c69 2229 0d0a 2020 2020 2020  engali")..      
-00004660: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00004670: 732e 6170 7065 6e64 2822 426f 736e 6961  s.append("Bosnia
-00004680: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-00004690: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-000046a0: 656e 6428 2242 7265 746f 6e22 290d 0a20  end("Breton").. 
-000046b0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000046c0: 5f6e 616d 6573 2e61 7070 656e 6428 2242  _names.append("B
-000046d0: 756c 6761 7269 616e 2229 0d0a 2020 2020  ulgarian")..    
-000046e0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-000046f0: 6d65 732e 6170 7065 6e64 2822 4361 7461  mes.append("Cata
-00004700: 6c61 6e22 290d 0a20 2020 2020 2020 2073  lan")..        s
-00004710: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00004720: 7070 656e 6428 2243 6869 6e65 7365 2229  ppend("Chinese")
-00004730: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00004740: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00004750: 2822 4372 6f61 7469 616e 2229 0d0a 2020  ("Croatian")..  
-00004760: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00004770: 6e61 6d65 732e 6170 7065 6e64 2822 437a  names.append("Cz
-00004780: 6563 6822 290d 0a20 2020 2020 2020 2073  ech")..        s
-00004790: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-000047a0: 7070 656e 6428 2244 616e 6973 6822 290d  ppend("Danish").
-000047b0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000047c0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-000047d0: 2244 7574 6368 2229 0d0a 2020 2020 2020  "Dutch")..      
-000047e0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-000047f0: 732e 6170 7065 6e64 2822 456e 676c 6973  s.append("Englis
-00004800: 6822 290d 0a20 2020 2020 2020 2073 656c  h")..        sel
-00004810: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00004820: 656e 6428 2245 7374 6f6e 6961 6e22 290d  end("Estonian").
-00004830: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004840: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00004850: 2246 6172 6f65 7365 2229 0d0a 2020 2020  "Faroese")..    
-00004860: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00004870: 6d65 732e 6170 7065 6e64 2822 4669 6e6e  mes.append("Finn
-00004880: 6973 6822 290d 0a20 2020 2020 2020 2073  ish")..        s
-00004890: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-000048a0: 7070 656e 6428 2246 7265 6e63 6822 290d  ppend("French").
-000048b0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000048c0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-000048d0: 2247 616c 6963 6961 6e22 290d 0a20 2020  "Galician")..   
-000048e0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-000048f0: 616d 6573 2e61 7070 656e 6428 2247 656f  ames.append("Geo
-00004900: 7267 6961 6e22 290d 0a20 2020 2020 2020  rgian")..       
-00004910: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004920: 2e61 7070 656e 6428 2247 6572 6d61 6e22  .append("German"
-00004930: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004940: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00004950: 6428 2247 7265 656b 2229 0d0a 2020 2020  d("Greek")..    
-00004960: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00004970: 6d65 732e 6170 7065 6e64 2822 4775 6a61  mes.append("Guja
-00004980: 7261 7469 2229 0d0a 2020 2020 2020 2020  rati")..        
-00004990: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-000049a0: 6170 7065 6e64 2822 4861 6974 6961 6e20  append("Haitian 
-000049b0: 4372 656f 6c65 2229 0d0a 2020 2020 2020  Creole")..      
-000049c0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-000049d0: 732e 6170 7065 6e64 2822 4861 7573 6122  s.append("Hausa"
-000049e0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000049f0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00004a00: 6428 2248 6177 6169 6961 6e22 290d 0a20  d("Hawaiian").. 
-00004a10: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00004a20: 5f6e 616d 6573 2e61 7070 656e 6428 2248  _names.append("H
-00004a30: 6562 7265 7722 290d 0a20 2020 2020 2020  ebrew")..       
-00004a40: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004a50: 2e61 7070 656e 6428 2248 696e 6469 2229  .append("Hindi")
-00004a60: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00004a70: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00004a80: 2822 4875 6e67 6172 6961 6e22 290d 0a20  ("Hungarian").. 
-00004a90: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00004aa0: 5f6e 616d 6573 2e61 7070 656e 6428 2249  _names.append("I
-00004ab0: 6365 6c61 6e64 6963 2229 0d0a 2020 2020  celandic")..    
-00004ac0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00004ad0: 6d65 732e 6170 7065 6e64 2822 496e 646f  mes.append("Indo
-00004ae0: 6e65 7369 616e 2229 0d0a 2020 2020 2020  nesian")..      
-00004af0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00004b00: 732e 6170 7065 6e64 2822 4974 616c 6961  s.append("Italia
-00004b10: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-00004b20: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00004b30: 656e 6428 224a 6170 616e 6573 6522 290d  end("Japanese").
-00004b40: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004b50: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00004b60: 224a 6176 616e 6573 6522 290d 0a20 2020  "Javanese")..   
-00004b70: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004b80: 616d 6573 2e61 7070 656e 6428 224b 616e  ames.append("Kan
-00004b90: 6e61 6461 2229 0d0a 2020 2020 2020 2020  nada")..        
-00004ba0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00004bb0: 6170 7065 6e64 2822 4b61 7a61 6b68 2229  append("Kazakh")
-00004bc0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00004bd0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00004be0: 2822 4b68 6d65 7222 290d 0a20 2020 2020  ("Khmer")..     
-00004bf0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00004c00: 6573 2e61 7070 656e 6428 224b 6f72 6561  es.append("Korea
-00004c10: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-00004c20: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00004c30: 656e 6428 224c 616f 2229 0d0a 2020 2020  end("Lao")..    
-00004c40: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00004c50: 6d65 732e 6170 7065 6e64 2822 4c61 7469  mes.append("Lati
-00004c60: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-00004c70: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00004c80: 656e 6428 224c 6174 7669 616e 2229 0d0a  end("Latvian")..
-00004c90: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00004ca0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00004cb0: 4c69 6e67 616c 6122 290d 0a20 2020 2020  Lingala")..     
-00004cc0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00004cd0: 6573 2e61 7070 656e 6428 224c 6974 6875  es.append("Lithu
-00004ce0: 616e 6961 6e22 290d 0a20 2020 2020 2020  anian")..       
-00004cf0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004d00: 2e61 7070 656e 6428 224c 7578 656d 626f  .append("Luxembo
-00004d10: 7572 6769 7368 2229 0d0a 2020 2020 2020  urgish")..      
-00004d20: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00004d30: 732e 6170 7065 6e64 2822 4d61 6365 646f  s.append("Macedo
-00004d40: 6e69 616e 2229 0d0a 2020 2020 2020 2020  nian")..        
-00004d50: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00004d60: 6170 7065 6e64 2822 4d61 6c61 6761 7379  append("Malagasy
-00004d70: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004d80: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00004d90: 6e64 2822 4d61 6c61 7922 290d 0a20 2020  nd("Malay")..   
-00004da0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004db0: 616d 6573 2e61 7070 656e 6428 224d 616c  ames.append("Mal
-00004dc0: 6179 616c 616d 2229 0d0a 2020 2020 2020  ayalam")..      
-00004dd0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00004de0: 732e 6170 7065 6e64 2822 4d61 6c74 6573  s.append("Maltes
-00004df0: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
-00004e00: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00004e10: 656e 6428 224d 616f 7269 2229 0d0a 2020  end("Maori")..  
-00004e20: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00004e30: 6e61 6d65 732e 6170 7065 6e64 2822 4d61  names.append("Ma
-00004e40: 7261 7468 6922 290d 0a20 2020 2020 2020  rathi")..       
-00004e50: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004e60: 2e61 7070 656e 6428 224d 6f6e 676f 6c69  .append("Mongoli
-00004e70: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
-00004e80: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00004e90: 7065 6e64 2822 4d79 616e 6d61 7220 2842  pend("Myanmar (B
-00004ea0: 7572 6d65 7365 2922 290d 0a20 2020 2020  urmese)")..     
-00004eb0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00004ec0: 6573 2e61 7070 656e 6428 224e 6570 616c  es.append("Nepal
-00004ed0: 6922 290d 0a20 2020 2020 2020 2073 656c  i")..        sel
-00004ee0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00004ef0: 656e 6428 224e 6f72 7765 6769 616e 2229  end("Norwegian")
-00004f00: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00004f10: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00004f20: 2822 4e79 6e6f 7273 6b22 290d 0a20 2020  ("Nynorsk")..   
-00004f30: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004f40: 616d 6573 2e61 7070 656e 6428 224f 6363  ames.append("Occ
-00004f50: 6974 616e 2229 0d0a 2020 2020 2020 2020  itan")..        
-00004f60: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00004f70: 6170 7065 6e64 2822 5061 7368 746f 2229  append("Pashto")
-00004f80: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00004f90: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00004fa0: 2822 5065 7273 6961 6e22 290d 0a20 2020  ("Persian")..   
-00004fb0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004fc0: 616d 6573 2e61 7070 656e 6428 2250 6f6c  ames.append("Pol
-00004fd0: 6973 6822 290d 0a20 2020 2020 2020 2073  ish")..        s
-00004fe0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00004ff0: 7070 656e 6428 2250 6f72 7475 6775 6573  ppend("Portugues
-00005000: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
-00005010: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00005020: 656e 6428 2250 756e 6a61 6269 2229 0d0a  end("Punjabi")..
-00005030: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00005040: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00005050: 526f 6d61 6e69 616e 2229 0d0a 2020 2020  Romanian")..    
-00005060: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00005070: 6d65 732e 6170 7065 6e64 2822 5275 7373  mes.append("Russ
-00005080: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
-00005090: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-000050a0: 7070 656e 6428 2253 616e 736b 7269 7422  ppend("Sanskrit"
-000050b0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000050c0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-000050d0: 6428 2253 6572 6269 616e 2229 0d0a 2020  d("Serbian")..  
-000050e0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000050f0: 6e61 6d65 732e 6170 7065 6e64 2822 5368  names.append("Sh
-00005100: 6f6e 6122 290d 0a20 2020 2020 2020 2073  ona")..        s
-00005110: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00005120: 7070 656e 6428 2253 696e 6468 6922 290d  ppend("Sindhi").
-00005130: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00005140: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00005150: 2253 696e 6861 6c61 2229 0d0a 2020 2020  "Sinhala")..    
-00005160: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00005170: 6d65 732e 6170 7065 6e64 2822 536c 6f76  mes.append("Slov
-00005180: 616b 2229 0d0a 2020 2020 2020 2020 7365  ak")..        se
-00005190: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-000051a0: 7065 6e64 2822 536c 6f76 656e 6961 6e22  pend("Slovenian"
-000051b0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000051c0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-000051d0: 6428 2253 6f6d 616c 6922 290d 0a20 2020  d("Somali")..   
-000051e0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-000051f0: 616d 6573 2e61 7070 656e 6428 2253 7061  ames.append("Spa
-00005200: 6e69 7368 2229 0d0a 2020 2020 2020 2020  nish")..        
-00005210: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00005220: 6170 7065 6e64 2822 5375 6e64 616e 6573  append("Sundanes
-00005230: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
-00005240: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00005250: 656e 6428 2253 7761 6869 6c69 2229 0d0a  end("Swahili")..
-00005260: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00005270: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00005280: 5377 6564 6973 6822 290d 0a20 2020 2020  Swedish")..     
-00005290: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-000052a0: 6573 2e61 7070 656e 6428 2254 6167 616c  es.append("Tagal
-000052b0: 6f67 2229 0d0a 2020 2020 2020 2020 7365  og")..        se
-000052c0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-000052d0: 7065 6e64 2822 5461 6a69 6b22 290d 0a20  pend("Tajik").. 
-000052e0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000052f0: 5f6e 616d 6573 2e61 7070 656e 6428 2254  _names.append("T
-00005300: 616d 696c 2229 0d0a 2020 2020 2020 2020  amil")..        
-00005310: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00005320: 6170 7065 6e64 2822 5461 7461 7222 290d  append("Tatar").
-00005330: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00005340: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00005350: 2254 656c 7567 7522 290d 0a20 2020 2020  "Telugu")..     
-00005360: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00005370: 6573 2e61 7070 656e 6428 2254 6861 6922  es.append("Thai"
-00005380: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00005390: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-000053a0: 6428 2254 6962 6574 616e 2229 0d0a 2020  d("Tibetan")..  
-000053b0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000053c0: 6e61 6d65 732e 6170 7065 6e64 2822 5475  names.append("Tu
-000053d0: 726b 6973 6822 290d 0a20 2020 2020 2020  rkish")..       
-000053e0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-000053f0: 2e61 7070 656e 6428 2254 7572 6b6d 656e  .append("Turkmen
-00005400: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00005410: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00005420: 6e64 2822 556b 7261 696e 6961 6e22 290d  nd("Ukrainian").
-00005430: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00005440: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00005450: 2255 7264 7522 290d 0a20 2020 2020 2020  "Urdu")..       
-00005460: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00005470: 2e61 7070 656e 6428 2255 7a62 656b 2229  .append("Uzbek")
-00005480: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00005490: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-000054a0: 2822 5669 6574 6e61 6d65 7365 2229 0d0a  ("Vietnamese")..
-000054b0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000054c0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000054d0: 5765 6c73 6822 290d 0a20 2020 2020 2020  Welsh")..       
-000054e0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-000054f0: 2e61 7070 656e 6428 2259 6964 6469 7368  .append("Yiddish
-00005500: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00005510: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00005520: 6e64 2822 596f 7275 6261 2229 0d0a 0d0a  nd("Yoruba")....
-00005530: 2020 2020 2020 2020 7365 6c66 2e63 6f64          self.cod
-00005540: 655f 6f66 5f6e 616d 6520 3d20 6469 6374  e_of_name = dict
-00005550: 287a 6970 2873 656c 662e 6c69 7374 5f6e  (zip(self.list_n
-00005560: 616d 6573 2c20 7365 6c66 2e6c 6973 745f  ames, self.list_
-00005570: 636f 6465 7329 290d 0a20 2020 2020 2020  codes))..       
-00005580: 2073 656c 662e 6e61 6d65 5f6f 665f 636f   self.name_of_co
-00005590: 6465 203d 2064 6963 7428 7a69 7028 7365  de = dict(zip(se
-000055a0: 6c66 2e6c 6973 745f 636f 6465 732c 2073  lf.list_codes, s
-000055b0: 656c 662e 6c69 7374 5f6e 616d 6573 2929  elf.list_names))
-000055c0: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
-000055d0: 2e64 6963 7420 3d20 7b0d 0a20 2020 2020  .dict = {..     
-000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055f0: 2020 2027 6166 273a 2027 4166 7269 6b61     'af': 'Afrika
-00005600: 616e 7327 2c0d 0a20 2020 2020 2020 2020  ans',..         
-00005610: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00005620: 7371 273a 2027 416c 6261 6e69 616e 272c  sq': 'Albanian',
-00005630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005640: 2020 2020 2020 2020 2020 2761 6d27 3a20            'am': 
-00005650: 2741 6d68 6172 6963 272c 0d0a 2020 2020  'Amharic',..    
-00005660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005670: 2020 2020 2761 7227 3a20 2741 7261 6269      'ar': 'Arabi
-00005680: 6327 2c0d 0a20 2020 2020 2020 2020 2020  c',..           
-00005690: 2020 2020 2020 2020 2020 2020 2027 6879               'hy
-000056a0: 273a 2027 4172 6d65 6e69 616e 272c 0d0a  ': 'Armenian',..
-000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056c0: 2020 2020 2020 2020 2761 7327 3a20 2741          'as': 'A
-000056d0: 7373 616d 6573 6527 2c0d 0a20 2020 2020  ssamese',..     
-000056e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056f0: 2020 2027 617a 273a 2027 417a 6572 6261     'az': 'Azerba
-00005700: 696a 616e 6927 2c0d 0a20 2020 2020 2020  ijani',..       
-00005710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005720: 2027 6261 273a 2027 4261 7368 6b69 7227   'ba': 'Bashkir'
-00005730: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005740: 2020 2020 2020 2020 2020 2027 6575 273a             'eu':
-00005750: 2027 4261 7371 7565 272c 0d0a 2020 2020   'Basque',..    
-00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005770: 2020 2020 2762 6527 3a20 2742 656c 6172      'be': 'Belar
-00005780: 7573 6961 6e27 2c0d 0a20 2020 2020 2020  usian',..       
-00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057a0: 2027 626e 273a 2027 4265 6e67 616c 6927   'bn': 'Bengali'
-000057b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000057c0: 2020 2020 2020 2020 2020 2027 6273 273a             'bs':
-000057d0: 2027 426f 736e 6961 6e27 2c0d 0a20 2020   'Bosnian',..   
-000057e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057f0: 2020 2020 2027 6272 273a 2027 4272 6574       'br': 'Bret
-00005800: 6f6e 272c 0d0a 2020 2020 2020 2020 2020  on',..          
-00005810: 2020 2020 2020 2020 2020 2020 2020 2762                'b
-00005820: 6727 3a20 2742 756c 6761 7269 616e 272c  g': 'Bulgarian',
-00005830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005840: 2020 2020 2020 2020 2020 2763 6127 3a20            'ca': 
-00005850: 2743 6174 616c 616e 272c 0d0a 2020 2020  'Catalan',..    
-00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005870: 2020 2020 277a 6827 3a20 2743 6869 6e65      'zh': 'Chine
-00005880: 7365 272c 0d0a 2020 2020 2020 2020 2020  se',..          
-00005890: 2020 2020 2020 2020 2020 2020 2020 2768                'h
-000058a0: 7227 3a20 2743 726f 6174 6961 6e27 2c0d  r': 'Croatian',.
-000058b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000058c0: 2020 2020 2020 2020 2027 6373 273a 2027           'cs': '
-000058d0: 437a 6563 6827 2c0d 0a20 2020 2020 2020  Czech',..       
-000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058f0: 2027 6461 273a 2027 4461 6e69 7368 272c   'da': 'Danish',
-00005900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005910: 2020 2020 2020 2020 2020 276e 6c27 3a20            'nl': 
-00005920: 2744 7574 6368 272c 0d0a 2020 2020 2020  'Dutch',..      
-00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005940: 2020 2765 6e27 3a20 2745 6e67 6c69 7368    'en': 'English
-00005950: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005960: 2020 2020 2020 2020 2020 2020 2765 7427              'et'
-00005970: 3a20 2745 7374 6f6e 6961 6e27 2c0d 0a20  : 'Estonian',.. 
-00005980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005990: 2020 2020 2020 2027 666f 273a 2027 4661         'fo': 'Fa
-000059a0: 726f 6573 6527 2c0d 0a20 2020 2020 2020  roese',..       
-000059b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059c0: 2027 6669 273a 2027 4669 6e6e 6973 6827   'fi': 'Finnish'
-000059d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000059e0: 2020 2020 2020 2020 2020 2027 6672 273a             'fr':
-000059f0: 2027 4672 656e 6368 272c 0d0a 2020 2020   'French',..    
-00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a10: 2020 2020 2767 6c27 3a20 2747 616c 6963      'gl': 'Galic
-00005a20: 6961 6e27 2c0d 0a20 2020 2020 2020 2020  ian',..         
-00005a30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00005a40: 6b61 273a 2027 4765 6f72 6769 616e 272c  ka': 'Georgian',
-00005a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005a60: 2020 2020 2020 2020 2020 2764 6527 3a20            'de': 
-00005a70: 2747 6572 6d61 6e27 2c0d 0a20 2020 2020  'German',..     
-00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a90: 2020 2027 656c 273a 2027 4772 6565 6b27     'el': 'Greek'
-00005aa0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005ab0: 2020 2020 2020 2020 2020 2027 6775 273a             'gu':
-00005ac0: 2027 4775 6a61 7261 7469 272c 0d0a 2020   'Gujarati',..  
-00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ae0: 2020 2020 2020 2768 7427 3a20 2748 6169        'ht': 'Hai
-00005af0: 7469 616e 2043 7265 6f6c 6527 2c0d 0a20  tian Creole',.. 
-00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b10: 2020 2020 2020 2027 6861 273a 2027 4861         'ha': 'Ha
-00005b20: 7573 6127 2c0d 0a20 2020 2020 2020 2020  usa',..         
-00005b30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00005b40: 6861 7727 3a20 2748 6177 6169 6961 6e27  haw': 'Hawaiian'
-00005b50: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005b60: 2020 2020 2020 2020 2020 2027 6865 273a             'he':
-00005b70: 2027 4865 6272 6577 272c 0d0a 2020 2020   'Hebrew',..    
-00005b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b90: 2020 2020 2768 6927 3a20 2748 696e 6469      'hi': 'Hindi
-00005ba0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005bb0: 2020 2020 2020 2020 2020 2020 2768 7527              'hu'
-00005bc0: 3a20 2748 756e 6761 7269 616e 272c 0d0a  : 'Hungarian',..
-00005bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005be0: 2020 2020 2020 2020 2769 7327 3a20 2749          'is': 'I
-00005bf0: 6365 6c61 6e64 6963 272c 0d0a 2020 2020  celandic',..    
-00005c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c10: 2020 2020 2769 6427 3a20 2749 6e64 6f6e      'id': 'Indon
-00005c20: 6573 6961 6e27 2c0d 0a20 2020 2020 2020  esian',..       
-00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c40: 2027 6974 273a 2027 4974 616c 6961 6e27   'it': 'Italian'
-00005c50: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005c60: 2020 2020 2020 2020 2020 2027 6a61 273a             'ja':
-00005c70: 2027 4a61 7061 6e65 7365 272c 0d0a 2020   'Japanese',..  
-00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c90: 2020 2020 2020 276a 7627 3a20 274a 6176        'jv': 'Jav
-00005ca0: 616e 6573 6527 2c0d 0a20 2020 2020 2020  anese',..       
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cc0: 2027 6b6e 273a 2027 4b61 6e6e 6164 6127   'kn': 'Kannada'
-00005cd0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005ce0: 2020 2020 2020 2020 2020 2027 6b6b 273a             'kk':
-00005cf0: 2027 4b61 7a61 6b68 272c 0d0a 2020 2020   'Kazakh',..    
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 2020 2020 276b 6d27 3a20 274b 686d 6572      'km': 'Khmer
-00005d20: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005d30: 2020 2020 2020 2020 2020 2020 276b 6f27              'ko'
-00005d40: 3a20 274b 6f72 6561 6e27 2c0d 0a20 2020  : 'Korean',..   
-00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d60: 2020 2020 2027 6c6f 273a 2027 4c61 6f27       'lo': 'Lao'
-00005d70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005d80: 2020 2020 2020 2020 2020 2027 6c61 273a             'la':
-00005d90: 2027 4c61 7469 6e27 2c0d 0a20 2020 2020   'Latin',..     
-00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005db0: 2020 2027 6c76 273a 2027 4c61 7476 6961     'lv': 'Latvia
-00005dc0: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
-00005dd0: 2020 2020 2020 2020 2020 2020 2027 6c6e               'ln
-00005de0: 273a 2027 4c69 6e67 616c 6127 2c0d 0a20  ': 'Lingala',.. 
-00005df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e00: 2020 2020 2020 2027 6c74 273a 2027 4c69         'lt': 'Li
-00005e10: 7468 7561 6e69 616e 272c 0d0a 2020 2020  thuanian',..    
-00005e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e30: 2020 2020 276c 6227 3a20 274c 7578 656d      'lb': 'Luxem
-00005e40: 626f 7572 6769 7368 272c 0d0a 2020 2020  bourgish',..    
-00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e60: 2020 2020 276d 6b27 3a20 274d 6163 6564      'mk': 'Maced
-00005e70: 6f6e 6961 6e27 2c0d 0a20 2020 2020 2020  onian',..       
+00000000: 6672 6f6d 205f 5f66 7574 7572 655f 5f20  from __future__ 
+00000010: 696d 706f 7274 2061 6273 6f6c 7574 655f  import absolute_
+00000020: 696d 706f 7274 2c20 7072 696e 745f 6675  import, print_fu
+00000030: 6e63 7469 6f6e 2c20 756e 6963 6f64 655f  nction, unicode_
+00000040: 6c69 7465 7261 6c73 0d0a 696d 706f 7274  literals..import
+00000050: 2061 7267 7061 7273 650d 0a69 6d70 6f72   argparse..impor
+00000060: 7420 6175 6469 6f6f 700d 0a69 6d70 6f72  t audioop..impor
+00000070: 7420 6d61 7468 0d0a 696d 706f 7274 206d  t math..import m
+00000080: 756c 7469 7072 6f63 6573 7369 6e67 0d0a  ultiprocessing..
+00000090: 696d 706f 7274 206f 730d 0a69 6d70 6f72  import os..impor
+000000a0: 7420 7375 6270 726f 6365 7373 0d0a 696d  t subprocess..im
+000000b0: 706f 7274 2073 7973 0d0a 696d 706f 7274  port sys..import
+000000c0: 2074 656d 7066 696c 650d 0a69 6d70 6f72   tempfile..impor
+000000d0: 7420 7761 7665 0d0a 696d 706f 7274 206a  t wave..import j
+000000e0: 736f 6e0d 0a69 6d70 6f72 7420 7265 7175  son..import requ
+000000f0: 6573 7473 0d0a 7472 793a 0d0a 2020 2020  ests..try:..    
+00000100: 6672 6f6d 206a 736f 6e2e 6465 636f 6465  from json.decode
+00000110: 7220 696d 706f 7274 204a 534f 4e44 6563  r import JSONDec
+00000120: 6f64 6545 7272 6f72 0d0a 6578 6365 7074  odeError..except
+00000130: 2049 6d70 6f72 7445 7272 6f72 3a0d 0a20   ImportError:.. 
+00000140: 2020 204a 534f 4e44 6563 6f64 6545 7272     JSONDecodeErr
+00000150: 6f72 203d 2056 616c 7565 4572 726f 720d  or = ValueError.
+00000160: 0a66 726f 6d20 7072 6f67 7265 7373 6261  .from progressba
+00000170: 7220 696d 706f 7274 2050 726f 6772 6573  r import Progres
+00000180: 7342 6172 2c20 5065 7263 656e 7461 6765  sBar, Percentage
+00000190: 2c20 4261 722c 2045 5441 0d0a 696d 706f  , Bar, ETA..impo
+000001a0: 7274 2070 7973 7274 0d0a 696d 706f 7274  rt pysrt..import
+000001b0: 2073 6978 0d0a 2320 4144 4449 5449 4f4e   six..# ADDITION
+000001c0: 414c 2049 4d50 4f52 540d 0a66 726f 6d20  AL IMPORT..from 
+000001d0: 676c 6f62 2069 6d70 6f72 7420 676c 6f62  glob import glob
+000001e0: 2c20 6573 6361 7065 0d0a 696d 706f 7274  , escape..import
+000001f0: 2074 696d 650d 0a66 726f 6d20 6461 7465   time..from date
+00000200: 7469 6d65 2069 6d70 6f72 7420 6461 7465  time import date
+00000210: 7469 6d65 2c20 7469 6d65 6465 6c74 610d  time, timedelta.
+00000220: 0a66 726f 6d20 7061 7468 6c69 6220 696d  .from pathlib im
+00000230: 706f 7274 2050 6174 680d 0a69 6d70 6f72  port Path..impor
+00000240: 7420 7761 726e 696e 6773 0d0a 7761 726e  t warnings..warn
+00000250: 696e 6773 2e66 696c 7465 7277 6172 6e69  ings.filterwarni
+00000260: 6e67 7328 2269 676e 6f72 6522 2c20 6d65  ngs("ignore", me
+00000270: 7373 6167 653d 222e 2a54 6865 2027 6e6f  ssage=".*The 'no
+00000280: 7079 7468 6f6e 2720 6b65 7977 6f72 642e  python' keyword.
+00000290: 2a22 290d 0a66 726f 6d20 6661 7374 6572  *")..from faster
+000002a0: 5f77 6869 7370 6572 2069 6d70 6f72 7420  _whisper import 
+000002b0: 5768 6973 7065 724d 6f64 656c 0d0a 0d0a  WhisperModel....
+000002c0: 0d0a 5645 5253 494f 4e20 3d20 2230 2e30  ..VERSION = "0.0
+000002d0: 2e34 220d 0a0d 0a77 6869 7370 6572 5f6d  .4"....whisper_m
+000002e0: 6f64 656c 7320 3d20 5b0d 0a20 2020 2020  odels = [..     
+000002f0: 2020 2020 2020 2020 2020 2022 7469 6e79             "tiny
+00000300: 2e65 6e22 2c0d 0a20 2020 2020 2020 2020  .en",..         
+00000310: 2020 2020 2020 2022 7469 6e79 222c 0d0a         "tiny",..
+00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000330: 2262 6173 652e 656e 222c 0d0a 2020 2020  "base.en",..    
+00000340: 2020 2020 2020 2020 2020 2020 2262 6173              "bas
+00000350: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
+00000360: 2020 2020 2022 736d 616c 6c2e 656e 222c       "small.en",
+00000370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000380: 2020 2273 6d61 6c6c 222c 0d0a 2020 2020    "small",..    
+00000390: 2020 2020 2020 2020 2020 2020 226d 6564              "med
+000003a0: 6975 6d2e 656e 222c 0d0a 2020 2020 2020  ium.en",..      
+000003b0: 2020 2020 2020 2020 2020 226d 6564 6975            "mediu
+000003c0: 6d22 2c0d 0a20 2020 2020 2020 2020 2020  m",..           
+000003d0: 2020 2020 2022 6c61 7267 652d 7631 222c       "large-v1",
+000003e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000003f0: 2020 226c 6172 6765 2d76 3222 2c0d 0a20    "large-v2",.. 
+00000400: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000410: 6c61 7267 6522 0d0a 5d0d 0a0d 0a23 3d3d  large"..]....#==
+00000420: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000430: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000440: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000450: 3d3d 3d3d 3d3d 2066 666d 7065 675f 7072  ====== ffmpeg_pr
+00000460: 6f67 7265 7373 5f79 6965 6c64 203d 3d3d  ogress_yield ===
+00000470: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000490: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000004a0: 3d3d 3d3d 3d23 0d0a 0d0a 696d 706f 7274  =====#....import
+000004b0: 2072 650d 0a23 696d 706f 7274 2073 7562   re..#import sub
+000004c0: 7072 6f63 6573 730d 0a66 726f 6d20 7479  process..from ty
+000004d0: 7069 6e67 2069 6d70 6f72 7420 416e 792c  ping import Any,
+000004e0: 2043 616c 6c61 626c 652c 2049 7465 7261   Callable, Itera
+000004f0: 746f 722c 204c 6973 742c 204f 7074 696f  tor, List, Optio
+00000500: 6e61 6c2c 2055 6e69 6f6e 0d0a 0d0a 0d0a  nal, Union......
+00000510: 6465 6620 746f 5f6d 7328 2a2a 6b77 6172  def to_ms(**kwar
+00000520: 6773 3a20 556e 696f 6e5b 666c 6f61 742c  gs: Union[float,
+00000530: 2069 6e74 2c20 7374 725d 2920 2d3e 2069   int, str]) -> i
+00000540: 6e74 3a0d 0a20 2020 2068 6f75 7220 3d20  nt:..    hour = 
+00000550: 696e 7428 6b77 6172 6773 2e67 6574 2822  int(kwargs.get("
+00000560: 686f 7572 222c 2030 2929 0d0a 2020 2020  hour", 0))..    
+00000570: 6d69 6e75 7465 203d 2069 6e74 286b 7761  minute = int(kwa
+00000580: 7267 732e 6765 7428 226d 696e 222c 2030  rgs.get("min", 0
+00000590: 2929 0d0a 2020 2020 7365 6320 3d20 696e  ))..    sec = in
+000005a0: 7428 6b77 6172 6773 2e67 6574 2822 7365  t(kwargs.get("se
+000005b0: 6322 2c20 3029 290d 0a20 2020 206d 7320  c", 0))..    ms 
+000005c0: 3d20 696e 7428 6b77 6172 6773 2e67 6574  = int(kwargs.get
+000005d0: 2822 6d73 222c 2030 2929 0d0a 0d0a 2020  ("ms", 0))....  
+000005e0: 2020 7265 7475 726e 2028 686f 7572 202a    return (hour *
+000005f0: 2036 3020 2a20 3630 202a 2031 3030 3029   60 * 60 * 1000)
+00000600: 202b 2028 6d69 6e75 7465 202a 2036 3020   + (minute * 60 
+00000610: 2a20 3130 3030 2920 2b20 2873 6563 202a  * 1000) + (sec *
+00000620: 2031 3030 3029 202b 206d 730d 0a0d 0a0d   1000) + ms.....
+00000630: 0a64 6566 205f 7072 6f62 655f 6475 7261  .def _probe_dura
+00000640: 7469 6f6e 2863 6d64 3a20 4c69 7374 5b73  tion(cmd: List[s
+00000650: 7472 5d29 202d 3e20 4f70 7469 6f6e 616c  tr]) -> Optional
+00000660: 5b69 6e74 5d3a 0d0a 2020 2020 2727 270d  [int]:..    '''.
+00000670: 0a20 2020 2047 6574 2074 6865 2064 7572  .    Get the dur
+00000680: 6174 696f 6e20 7669 6120 6666 7072 6f62  ation via ffprob
+00000690: 6520 6672 6f6d 2069 6e70 7574 206d 6564  e from input med
+000006a0: 6961 2066 696c 650d 0a20 2020 2069 6e20  ia file..    in 
+000006b0: 6361 7365 2066 666d 7065 6720 7761 7320  case ffmpeg was 
+000006c0: 7275 6e20 7769 7468 206c 6f67 6c65 7665  run with logleve
+000006d0: 6c3d 6572 726f 722e 0d0a 0d0a 2020 2020  l=error.....    
+000006e0: 4172 6773 3a0d 0a20 2020 2020 2020 2063  Args:..        c
+000006f0: 6d64 2028 4c69 7374 5b73 7472 5d29 3a20  md (List[str]): 
+00000700: 4120 6c69 7374 206f 6620 636f 6d6d 616e  A list of comman
+00000710: 6420 6c69 6e65 2065 6c65 6d65 6e74 732c  d line elements,
+00000720: 2065 2e67 2e20 5b22 6666 6d70 6567 222c   e.g. ["ffmpeg",
+00000730: 2022 2d69 222c 202e 2e2e 5d0d 0a0d 0a20   "-i", ...].... 
+00000740: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
+00000750: 2020 2020 204f 7074 696f 6e61 6c5b 696e       Optional[in
+00000760: 745d 3a20 5468 6520 6475 7261 7469 6f6e  t]: The duration
+00000770: 2069 6e20 6d69 6c6c 6973 6563 6f6e 6473   in milliseconds
+00000780: 2e0d 0a20 2020 2027 2727 0d0a 0d0a 2020  ...    '''....  
+00000790: 2020 6465 6620 5f67 6574 5f66 696c 655f    def _get_file_
+000007a0: 6e61 6d65 2863 6d64 3a20 4c69 7374 5b73  name(cmd: List[s
+000007b0: 7472 5d29 202d 3e20 4f70 7469 6f6e 616c  tr]) -> Optional
+000007c0: 5b73 7472 5d3a 0d0a 2020 2020 2020 2020  [str]:..        
+000007d0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+000007e0: 2020 6964 7820 3d20 636d 642e 696e 6465    idx = cmd.inde
+000007f0: 7828 222d 6922 290d 0a20 2020 2020 2020  x("-i")..       
+00000800: 2020 2020 2072 6574 7572 6e20 636d 645b       return cmd[
+00000810: 6964 7820 2b20 315d 0d0a 2020 2020 2020  idx + 1]..      
+00000820: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
+00000830: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
+00000840: 2020 7265 7475 726e 204e 6f6e 650d 0a0d    return None...
+00000850: 0a20 2020 2066 696c 655f 6e61 6d65 203d  .    file_name =
+00000860: 205f 6765 745f 6669 6c65 5f6e 616d 6528   _get_file_name(
+00000870: 636d 6429 0d0a 2020 2020 6966 2066 696c  cmd)..    if fil
+00000880: 655f 6e61 6d65 2069 7320 4e6f 6e65 3a0d  e_name is None:.
+00000890: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000008a0: 4e6f 6e65 0d0a 0d0a 2020 2020 7472 793a  None....    try:
+000008b0: 0d0a 2020 2020 2020 2020 6966 2073 7973  ..        if sys
+000008c0: 2e70 6c61 7466 6f72 6d20 3d3d 2022 7769  .platform == "wi
+000008d0: 6e33 3222 3a0d 0a20 2020 2020 2020 2020  n32":..         
+000008e0: 2020 206f 7574 7075 7420 3d20 7375 6270     output = subp
+000008f0: 726f 6365 7373 2e63 6865 636b 5f6f 7574  rocess.check_out
+00000900: 7075 7428 0d0a 2020 2020 2020 2020 2020  put(..          
+00000910: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
+00000920: 2020 2020 2020 2020 2020 2020 2022 6666               "ff
+00000930: 7072 6f62 6522 2c0d 0a20 2020 2020 2020  probe",..       
+00000940: 2020 2020 2020 2020 2020 2020 2022 2d6c               "-l
+00000950: 6f67 6c65 7665 6c22 2c0d 0a20 2020 2020  oglevel",..     
+00000960: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000970: 2d31 222c 0d0a 2020 2020 2020 2020 2020  -1",..          
+00000980: 2020 2020 2020 2020 2020 222d 6869 6465            "-hide
+00000990: 5f62 616e 6e65 7222 2c0d 0a20 2020 2020  _banner",..     
+000009a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000009b0: 2d73 686f 775f 656e 7472 6965 7322 2c0d  -show_entries",.
+000009c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000009d0: 2020 2020 2022 666f 726d 6174 3d64 7572       "format=dur
+000009e0: 6174 696f 6e22 2c0d 0a20 2020 2020 2020  ation",..       
+000009f0: 2020 2020 2020 2020 2020 2020 2022 2d6f               "-o
+00000a00: 6622 2c0d 0a20 2020 2020 2020 2020 2020  f",..           
+00000a10: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
+00000a20: 743d 6e6f 7072 696e 745f 7772 6170 7065  t=noprint_wrappe
+00000a30: 7273 3d31 3a6e 6f6b 6579 3d31 222c 0d0a  rs=1:nokey=1",..
+00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a50: 2020 2020 6669 6c65 5f6e 616d 652c 0d0a      file_name,..
+00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a70: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00000a80: 2020 2020 756e 6976 6572 7361 6c5f 6e65      universal_ne
+00000a90: 776c 696e 6573 3d54 7275 652c 0d0a 2020  wlines=True,..  
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
+00000ab0: 6561 7469 6f6e 666c 6167 733d 7375 6270  eationflags=subp
+00000ac0: 726f 6365 7373 2e43 5245 4154 455f 4e4f  rocess.CREATE_NO
+00000ad0: 5f57 494e 444f 572c 0d0a 2020 2020 2020  _WINDOW,..      
+00000ae0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00000af0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00000b00: 2020 2020 6f75 7470 7574 203d 2073 7562      output = sub
+00000b10: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
+00000b20: 7470 7574 280d 0a20 2020 2020 2020 2020  tput(..         
+00000b30: 2020 2020 2020 205b 0d0a 2020 2020 2020         [..      
+00000b40: 2020 2020 2020 2020 2020 2020 2020 2266                "f
+00000b50: 6670 726f 6265 222c 0d0a 2020 2020 2020  fprobe",..      
+00000b60: 2020 2020 2020 2020 2020 2020 2020 222d                "-
+00000b70: 6c6f 676c 6576 656c 222c 0d0a 2020 2020  loglevel",..    
+00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b90: 222d 3122 2c0d 0a20 2020 2020 2020 2020  "-1",..         
+00000ba0: 2020 2020 2020 2020 2020 2022 2d68 6964             "-hid
+00000bb0: 655f 6261 6e6e 6572 222c 0d0a 2020 2020  e_banner",..    
+00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bd0: 222d 7368 6f77 5f65 6e74 7269 6573 222c  "-show_entries",
+00000be0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000bf0: 2020 2020 2020 2266 6f72 6d61 743d 6475        "format=du
+00000c00: 7261 7469 6f6e 222c 0d0a 2020 2020 2020  ration",..      
+00000c10: 2020 2020 2020 2020 2020 2020 2020 222d                "-
+00000c20: 6f66 222c 0d0a 2020 2020 2020 2020 2020  of",..          
+00000c30: 2020 2020 2020 2020 2020 2264 6566 6175            "defau
+00000c40: 6c74 3d6e 6f70 7269 6e74 5f77 7261 7070  lt=noprint_wrapp
+00000c50: 6572 733d 313a 6e6f 6b65 793d 3122 2c0d  ers=1:nokey=1",.
+00000c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000c70: 2020 2020 2066 696c 655f 6e61 6d65 2c0d       file_name,.
+00000c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000c90: 205d 2c0d 0a20 2020 2020 2020 2020 2020   ],..           
+00000ca0: 2020 2020 2075 6e69 7665 7273 616c 5f6e       universal_n
+00000cb0: 6577 6c69 6e65 733d 5472 7565 2c0d 0a20  ewlines=True,.. 
+00000cc0: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
+00000cd0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+00000ce0: 6e74 2866 6c6f 6174 286f 7574 7075 742e  nt(float(output.
+00000cf0: 7374 7269 7028 2929 202a 2031 3030 3029  strip()) * 1000)
+00000d00: 0d0a 2020 2020 6578 6365 7074 2045 7863  ..    except Exc
+00000d10: 6570 7469 6f6e 3a0d 0a20 2020 2020 2020  eption:..       
+00000d20: 2023 2054 4f44 4f3a 2061 6464 206c 6f67   # TODO: add log
+00000d30: 6769 6e67 0d0a 2020 2020 2020 2020 7265  ging..        re
+00000d40: 7475 726e 204e 6f6e 650d 0a0d 0a0d 0a64  turn None......d
+00000d50: 6566 205f 7573 6573 5f65 7272 6f72 5f6c  ef _uses_error_l
+00000d60: 6f67 6c65 7665 6c28 636d 643a 204c 6973  oglevel(cmd: Lis
+00000d70: 745b 7374 725d 2920 2d3e 2062 6f6f 6c3a  t[str]) -> bool:
+00000d80: 0d0a 2020 2020 7472 793a 0d0a 2020 2020  ..    try:..    
+00000d90: 2020 2020 6964 7820 3d20 636d 642e 696e      idx = cmd.in
+00000da0: 6465 7828 222d 6c6f 676c 6576 656c 2229  dex("-loglevel")
+00000db0: 0d0a 2020 2020 2020 2020 6966 2063 6d64  ..        if cmd
+00000dc0: 5b69 6478 202b 2031 5d20 3d3d 2022 6572  [idx + 1] == "er
+00000dd0: 726f 7222 3a0d 0a20 2020 2020 2020 2020  ror":..         
+00000de0: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
+00000df0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00000e00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000e10: 6e20 4661 6c73 650d 0a20 2020 2065 7863  n False..    exc
+00000e20: 6570 7420 5661 6c75 6545 7272 6f72 3a0d  ept ValueError:.
+00000e30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000e40: 4661 6c73 650d 0a0d 0a0d 0a63 6c61 7373  False......class
+00000e50: 2046 666d 7065 6750 726f 6772 6573 733a   FfmpegProgress:
+00000e60: 0d0a 2020 2020 4455 525f 5245 4745 5820  ..    DUR_REGEX 
+00000e70: 3d20 7265 2e63 6f6d 7069 6c65 280d 0a20  = re.compile(.. 
+00000e80: 2020 2020 2020 2072 2244 7572 6174 696f         r"Duratio
+00000e90: 6e3a 2028 3f50 3c68 6f75 723e 5c64 7b32  n: (?P<hour>\d{2
+00000ea0: 7d29 3a28 3f50 3c6d 696e 3e5c 647b 327d  }):(?P<min>\d{2}
+00000eb0: 293a 283f 503c 7365 633e 5c64 7b32 7d29  ):(?P<sec>\d{2})
+00000ec0: 5c2e 283f 503c 6d73 3e5c 647b 327d 2922  \.(?P<ms>\d{2})"
+00000ed0: 0d0a 2020 2020 290d 0a20 2020 2054 494d  ..    )..    TIM
+00000ee0: 455f 5245 4745 5820 3d20 7265 2e63 6f6d  E_REGEX = re.com
+00000ef0: 7069 6c65 280d 0a20 2020 2020 2020 2072  pile(..        r
+00000f00: 226f 7574 5f74 696d 653d 283f 503c 686f  "out_time=(?P<ho
+00000f10: 7572 3e5c 647b 327d 293a 283f 503c 6d69  ur>\d{2}):(?P<mi
+00000f20: 6e3e 5c64 7b32 7d29 3a28 3f50 3c73 6563  n>\d{2}):(?P<sec
+00000f30: 3e5c 647b 327d 295c 2e28 3f50 3c6d 733e  >\d{2})\.(?P<ms>
+00000f40: 5c64 7b32 7d29 220d 0a20 2020 2029 0d0a  \d{2})"..    )..
+00000f50: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00000f60: 5f5f 2873 656c 662c 2063 6d64 3a20 4c69  __(self, cmd: Li
+00000f70: 7374 5b73 7472 5d2c 2064 7279 5f72 756e  st[str], dry_run
+00000f80: 3a20 626f 6f6c 203d 2046 616c 7365 2920  : bool = False) 
+00000f90: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
+00000fa0: 2020 2727 2749 6e69 7469 616c 697a 6520    '''Initialize 
+00000fb0: 7468 6520 4666 6d70 6567 5072 6f67 7265  the FfmpegProgre
+00000fc0: 7373 2063 6c61 7373 2e0d 0a0d 0a20 2020  ss class.....   
+00000fd0: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
+00000fe0: 2020 2020 2020 2020 636d 6420 284c 6973          cmd (Lis
+00000ff0: 745b 7374 725d 293a 2041 206c 6973 7420  t[str]): A list 
+00001000: 6f66 2063 6f6d 6d61 6e64 206c 696e 6520  of command line 
+00001010: 656c 656d 656e 7473 2c20 652e 672e 205b  elements, e.g. [
+00001020: 2266 666d 7065 6722 2c20 222d 6922 2c20  "ffmpeg", "-i", 
+00001030: 2e2e 2e5d 0d0a 2020 2020 2020 2020 2020  ...]..          
+00001040: 2020 6472 795f 7275 6e20 2862 6f6f 6c2c    dry_run (bool,
+00001050: 206f 7074 696f 6e61 6c29 3a20 4f6e 6c79   optional): Only
+00001060: 2073 686f 7720 7768 6174 2077 6f75 6c64   show what would
+00001070: 2062 6520 646f 6e65 2e20 4465 6661 756c   be done. Defaul
+00001080: 7473 2074 6f20 4661 6c73 652e 0d0a 2020  ts to False...  
+00001090: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
+000010a0: 2020 2073 656c 662e 636d 6420 3d20 636d     self.cmd = cm
+000010b0: 640d 0a20 2020 2020 2020 2073 656c 662e  d..        self.
+000010c0: 7374 6465 7272 3a20 556e 696f 6e5b 7374  stderr: Union[st
+000010d0: 722c 204e 6f6e 655d 203d 204e 6f6e 650d  r, None] = None.
+000010e0: 0a20 2020 2020 2020 2073 656c 662e 6472  .        self.dr
+000010f0: 795f 7275 6e20 3d20 6472 795f 7275 6e0d  y_run = dry_run.
+00001100: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
+00001110: 6f63 6573 733a 2041 6e79 203d 204e 6f6e  ocess: Any = Non
+00001120: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+00001130: 7374 6465 7272 5f63 616c 6c62 6163 6b3a  stderr_callback:
+00001140: 2055 6e69 6f6e 5b43 616c 6c61 626c 655b   Union[Callable[
+00001150: 5b73 7472 5d2c 204e 6f6e 655d 2c20 4e6f  [str], None], No
+00001160: 6e65 5d20 3d20 4e6f 6e65 0d0a 2020 2020  ne] = None..    
+00001170: 2020 2020 6966 2073 7973 2e70 6c61 7466      if sys.platf
+00001180: 6f72 6d20 3d3d 2022 7769 6e33 3222 3a0d  orm == "win32":.
+00001190: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000011a0: 662e 6261 7365 5f70 6f70 656e 5f6b 7761  f.base_popen_kwa
+000011b0: 7267 7320 3d20 7b0d 0a20 2020 2020 2020  rgs = {..       
+000011c0: 2020 2020 2020 2020 2022 7374 6469 6e22           "stdin"
+000011d0: 3a20 7375 6270 726f 6365 7373 2e50 4950  : subprocess.PIP
+000011e0: 452c 2020 2320 4170 706c 7920 7374 6469  E,  # Apply stdi
+000011f0: 6e20 6973 6f6c 6174 696f 6e20 6279 2063  n isolation by c
+00001200: 7265 6174 696e 6720 7365 7061 7261 7465  reating separate
+00001210: 2070 6970 652e 0d0a 2020 2020 2020 2020   pipe...        
+00001220: 2020 2020 2020 2020 2273 7464 6f75 7422          "stdout"
+00001230: 3a20 7375 6270 726f 6365 7373 2e50 4950  : subprocess.PIP
+00001240: 452c 0d0a 2020 2020 2020 2020 2020 2020  E,..            
+00001250: 2020 2020 2273 7464 6572 7222 3a20 7375      "stderr": su
+00001260: 6270 726f 6365 7373 2e53 5444 4f55 542c  bprocess.STDOUT,
+00001270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001280: 2020 2275 6e69 7665 7273 616c 5f6e 6577    "universal_new
+00001290: 6c69 6e65 7322 3a20 4661 6c73 652c 0d0a  lines": False,..
+000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012b0: 2273 6865 6c6c 223a 2054 7275 652c 0d0a  "shell": True,..
+000012c0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
+000012d0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000012e0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+000012f0: 6173 655f 706f 7065 6e5f 6b77 6172 6773  ase_popen_kwargs
+00001300: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
+00001310: 2020 2020 2020 2273 7464 696e 223a 2073        "stdin": s
+00001320: 7562 7072 6f63 6573 732e 5049 5045 2c20  ubprocess.PIPE, 
+00001330: 2023 2041 7070 6c79 2073 7464 696e 2069   # Apply stdin i
+00001340: 736f 6c61 7469 6f6e 2062 7920 6372 6561  solation by crea
+00001350: 7469 6e67 2073 6570 6172 6174 6520 7069  ting separate pi
+00001360: 7065 2e0d 0a20 2020 2020 2020 2020 2020  pe...           
+00001370: 2020 2020 2022 7374 646f 7574 223a 2073       "stdout": s
+00001380: 7562 7072 6f63 6573 732e 5049 5045 2c0d  ubprocess.PIPE,.
+00001390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000013a0: 2022 7374 6465 7272 223a 2073 7562 7072   "stderr": subpr
+000013b0: 6f63 6573 732e 5354 444f 5554 2c0d 0a20  ocess.STDOUT,.. 
+000013c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000013d0: 756e 6976 6572 7361 6c5f 6e65 776c 696e  universal_newlin
+000013e0: 6573 223a 2046 616c 7365 2c0d 0a20 2020  es": False,..   
+000013f0: 2020 2020 2020 2020 207d 0d0a 0d0a 2020           }....  
+00001400: 2020 6465 6620 7365 745f 7374 6465 7272    def set_stderr
+00001410: 5f63 616c 6c62 6163 6b28 7365 6c66 2c20  _callback(self, 
+00001420: 6361 6c6c 6261 636b 3a20 4361 6c6c 6162  callback: Callab
+00001430: 6c65 5b5b 7374 725d 2c20 4e6f 6e65 5d29  le[[str], None])
+00001440: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
+00001450: 2020 2027 2727 0d0a 2020 2020 2020 2020     '''..        
+00001460: 5365 7420 6120 6361 6c6c 6261 636b 2066  Set a callback f
+00001470: 756e 6374 696f 6e20 746f 2062 6520 6361  unction to be ca
+00001480: 6c6c 6564 206f 6e20 7374 6465 7272 206f  lled on stderr o
+00001490: 7574 7075 742e 0d0a 2020 2020 2020 2020  utput...        
+000014a0: 5468 6520 6361 6c6c 6261 636b 2066 756e  The callback fun
+000014b0: 6374 696f 6e20 6d75 7374 2061 6363 6570  ction must accep
+000014c0: 7420 6120 7369 6e67 6c65 2073 7472 696e  t a single strin
+000014d0: 6720 6172 6775 6d65 6e74 2e0d 0a20 2020  g argument...   
+000014e0: 2020 2020 204e 6f74 6520 7468 6174 2074       Note that t
+000014f0: 6869 7320 6973 2063 616c 6c65 6420 6f6e  his is called on
+00001500: 2065 7665 7279 206c 696e 6520 6f66 2073   every line of s
+00001510: 7464 6572 7220 6f75 7470 7574 2c20 736f  tderr output, so
+00001520: 2069 7420 6361 6e20 6265 2063 616c 6c65   it can be calle
+00001530: 6420 6120 6c6f 742e 0d0a 2020 2020 2020  d a lot...      
+00001540: 2020 416c 736f 206e 6f74 6520 7468 6174    Also note that
+00001550: 2073 7464 6f75 742f 7374 6465 7272 2061   stdout/stderr a
+00001560: 7265 206a 6f69 6e65 6420 696e 746f 206f  re joined into o
+00001570: 6e65 2073 7472 6561 6d2c 2073 6f20 796f  ne stream, so yo
+00001580: 7520 6d69 6768 7420 6765 7420 7374 646f  u might get stdo
+00001590: 7574 206f 7574 7075 7420 696e 2074 6865  ut output in the
+000015a0: 2063 616c 6c62 6163 6b2e 0d0a 0d0a 2020   callback.....  
+000015b0: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
+000015c0: 2020 2020 2020 2020 2063 616c 6c62 6163           callbac
+000015d0: 6b20 2843 616c 6c61 626c 655b 5b73 7472  k (Callable[[str
+000015e0: 5d2c 204e 6f6e 655d 293a 2041 2063 616c  ], None]): A cal
+000015f0: 6c62 6163 6b20 6675 6e63 7469 6f6e 2074  lback function t
+00001600: 6861 7420 6163 6365 7074 7320 6120 7369  hat accepts a si
+00001610: 6e67 6c65 2073 7472 696e 6720 6172 6775  ngle string argu
+00001620: 6d65 6e74 2e0d 0a20 2020 2020 2020 2027  ment...        '
+00001630: 2727 0d0a 2020 2020 2020 2020 6966 206e  ''..        if n
+00001640: 6f74 2063 616c 6c61 626c 6528 6361 6c6c  ot callable(call
+00001650: 6261 636b 2920 6f72 206c 656e 2863 616c  back) or len(cal
+00001660: 6c62 6163 6b2e 5f5f 636f 6465 5f5f 2e63  lback.__code__.c
+00001670: 6f5f 7661 726e 616d 6573 2920 213d 2031  o_varnames) != 1
+00001680: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00001690: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000016a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000016b0: 2020 2243 616c 6c62 6163 6b20 6d75 7374    "Callback must
+000016c0: 2062 6520 6120 6675 6e63 7469 6f6e 2074   be a function t
+000016d0: 6861 7420 6163 6365 7074 7320 6f6e 6c79  hat accepts only
+000016e0: 206f 6e65 2061 7267 756d 656e 7422 0d0a   one argument"..
+000016f0: 2020 2020 2020 2020 2020 2020 290d 0a0d              )...
+00001700: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+00001710: 6465 7272 5f63 616c 6c62 6163 6b20 3d20  derr_callback = 
+00001720: 6361 6c6c 6261 636b 0d0a 0d0a 2020 2020  callback....    
+00001730: 6465 6620 7275 6e5f 636f 6d6d 616e 645f  def run_command_
+00001740: 7769 7468 5f70 726f 6772 6573 7328 0d0a  with_progress(..
+00001750: 2020 2020 2020 2020 7365 6c66 2c20 706f          self, po
+00001760: 7065 6e5f 6b77 6172 6773 3d4e 6f6e 652c  pen_kwargs=None,
+00001770: 2064 7572 6174 696f 6e5f 6f76 6572 7269   duration_overri
+00001780: 6465 3a20 556e 696f 6e5b 666c 6f61 742c  de: Union[float,
+00001790: 204e 6f6e 655d 203d 204e 6f6e 650d 0a20   None] = None.. 
+000017a0: 2020 2029 202d 3e20 4974 6572 6174 6f72     ) -> Iterator
+000017b0: 5b69 6e74 5d3a 0d0a 2020 2020 2020 2020  [int]:..        
+000017c0: 2727 270d 0a20 2020 2020 2020 2052 756e  '''..        Run
+000017d0: 2061 6e20 6666 6d70 6567 2063 6f6d 6d61   an ffmpeg comma
+000017e0: 6e64 2c20 7472 7969 6e67 2074 6f20 6361  nd, trying to ca
+000017f0: 7074 7572 6520 7468 6520 7072 6f63 6573  pture the proces
+00001800: 7320 6f75 7470 7574 2061 6e64 2063 616c  s output and cal
+00001810: 6375 6c61 7465 0d0a 2020 2020 2020 2020  culate..        
+00001820: 7468 6520 6475 7261 7469 6f6e 202f 2070  the duration / p
+00001830: 726f 6772 6573 732e 0d0a 2020 2020 2020  rogress...      
+00001840: 2020 5969 656c 6473 2074 6865 2070 726f    Yields the pro
+00001850: 6772 6573 7320 696e 2070 6572 6365 6e74  gress in percent
+00001860: 2e0d 0a0d 0a20 2020 2020 2020 2041 7267  .....        Arg
+00001870: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00001880: 706f 7065 6e5f 6b77 6172 6773 2028 6469  popen_kwargs (di
+00001890: 6374 2c20 6f70 7469 6f6e 616c 293a 2041  ct, optional): A
+000018a0: 2064 6963 7420 746f 2073 7065 6369 6679   dict to specify
+000018b0: 2065 7874 7261 2061 7267 756d 656e 7473   extra arguments
+000018c0: 2074 6f20 7468 6520 706f 7065 6e20 6361   to the popen ca
+000018d0: 6c6c 2c20 652e 672e 207b 2063 7265 6174  ll, e.g. { creat
+000018e0: 696f 6e66 6c61 6773 3a20 4352 4541 5445  ionflags: CREATE
+000018f0: 5f4e 4f5f 5749 4e44 4f57 207d 0d0a 2020  _NO_WINDOW }..  
+00001900: 2020 2020 2020 2020 2020 6475 7261 7469            durati
+00001910: 6f6e 5f6f 7665 7272 6964 6520 2866 6c6f  on_override (flo
+00001920: 6174 2c20 6f70 7469 6f6e 616c 293a 2054  at, optional): T
+00001930: 6865 2064 7572 6174 696f 6e20 696e 2073  he duration in s
+00001940: 6563 6f6e 6473 2e20 4966 206e 6f74 2073  econds. If not s
+00001950: 7065 6369 6669 6564 2c20 6974 2077 696c  pecified, it wil
+00001960: 6c20 6265 2063 616c 6375 6c61 7465 6420  l be calculated 
+00001970: 6672 6f6d 2074 6865 2066 666d 7065 6720  from the ffmpeg 
+00001980: 6f75 7470 7574 2e0d 0a0d 0a20 2020 2020  output.....     
+00001990: 2020 2052 6169 7365 733a 0d0a 2020 2020     Raises:..    
+000019a0: 2020 2020 2020 2020 5275 6e74 696d 6545          RuntimeE
+000019b0: 7272 6f72 3a20 4966 2074 6865 2063 6f6d  rror: If the com
+000019c0: 6d61 6e64 2066 6169 6c73 2c20 616e 2065  mand fails, an e
+000019d0: 7863 6570 7469 6f6e 2069 7320 7261 6973  xception is rais
+000019e0: 6564 2e0d 0a0d 0a20 2020 2020 2020 2059  ed.....        Y
+000019f0: 6965 6c64 733a 0d0a 2020 2020 2020 2020  ields:..        
+00001a00: 2020 2020 4974 6572 6174 6f72 5b69 6e74      Iterator[int
+00001a10: 5d3a 2041 2067 656e 6572 6174 6f72 2074  ]: A generator t
+00001a20: 6861 7420 7969 656c 6473 2074 6865 2070  hat yields the p
+00001a30: 726f 6772 6573 7320 696e 2070 6572 6365  rogress in perce
+00001a40: 6e74 2e0d 0a20 2020 2020 2020 2027 2727  nt...        '''
+00001a50: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00001a60: 662e 6472 795f 7275 6e3a 0d0a 2020 2020  f.dry_run:..    
+00001a70: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00001a80: 656c 662e 636d 640d 0a0d 0a20 2020 2020  elf.cmd....     
+00001a90: 2020 2074 6f74 616c 5f64 7572 3a20 556e     total_dur: Un
+00001aa0: 696f 6e5b 4e6f 6e65 2c20 696e 745d 203d  ion[None, int] =
+00001ab0: 204e 6f6e 650d 0a20 2020 2020 2020 2069   None..        i
+00001ac0: 6620 5f75 7365 735f 6572 726f 725f 6c6f  f _uses_error_lo
+00001ad0: 676c 6576 656c 2873 656c 662e 636d 6429  glevel(self.cmd)
+00001ae0: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+00001af0: 6f74 616c 5f64 7572 203d 205f 7072 6f62  otal_dur = _prob
+00001b00: 655f 6475 7261 7469 6f6e 2873 656c 662e  e_duration(self.
+00001b10: 636d 6429 0d0a 0d0a 2020 2020 2020 2020  cmd)....        
+00001b20: 636d 645f 7769 7468 5f70 726f 6772 6573  cmd_with_progres
+00001b30: 7320 3d20 280d 0a20 2020 2020 2020 2020  s = (..         
+00001b40: 2020 205b 7365 6c66 2e63 6d64 5b30 5d5d     [self.cmd[0]]
+00001b50: 202b 205b 222d 7072 6f67 7265 7373 222c   + ["-progress",
+00001b60: 2022 2d22 2c20 222d 6e6f 7374 6174 7322   "-", "-nostats"
+00001b70: 5d20 2b20 7365 6c66 2e63 6d64 5b31 3a5d  ] + self.cmd[1:]
+00001b80: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
+00001b90: 2020 2020 2020 2073 7464 6572 7220 3d20         stderr = 
+00001ba0: 5b5d 0d0a 2020 2020 2020 2020 6261 7365  []..        base
+00001bb0: 5f70 6f70 656e 5f6b 7761 7267 7320 3d20  _popen_kwargs = 
+00001bc0: 7365 6c66 2e62 6173 655f 706f 7065 6e5f  self.base_popen_
+00001bd0: 6b77 6172 6773 2e63 6f70 7928 290d 0a20  kwargs.copy().. 
+00001be0: 2020 2020 2020 2069 6620 706f 7065 6e5f         if popen_
+00001bf0: 6b77 6172 6773 2069 7320 6e6f 7420 4e6f  kwargs is not No
+00001c00: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00001c10: 2062 6173 655f 706f 7065 6e5f 6b77 6172   base_popen_kwar
+00001c20: 6773 2e75 7064 6174 6528 706f 7065 6e5f  gs.update(popen_
+00001c30: 6b77 6172 6773 290d 0a0d 0a20 2020 2020  kwargs)....     
+00001c40: 2020 2069 6620 7379 732e 706c 6174 666f     if sys.platfo
+00001c50: 726d 203d 3d20 2277 696e 6433 3222 3a0d  rm == "wind32":.
+00001c60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00001c70: 662e 7072 6f63 6573 7320 3d20 7375 6270  f.process = subp
+00001c80: 726f 6365 7373 2e50 6f70 656e 280d 0a20  rocess.Popen(.. 
+00001c90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001ca0: 6d64 5f77 6974 685f 7072 6f67 7265 7373  md_with_progress
+00001cb0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001cc0: 2020 202a 2a62 6173 655f 706f 7065 6e5f     **base_popen_
+00001cd0: 6b77 6172 6773 2c0d 0a20 2020 2020 2020  kwargs,..       
+00001ce0: 2020 2020 2020 2020 2063 7265 6174 696f           creatio
+00001cf0: 6e66 6c61 6773 3d73 7562 7072 6f63 6573  nflags=subproces
+00001d00: 732e 4352 4541 5445 5f4e 4f5f 5749 4e44  s.CREATE_NO_WIND
+00001d10: 4f57 2c0d 0a20 2020 2020 2020 2020 2020  OW,..           
+00001d20: 2029 2020 2320 7479 7065 3a20 6967 6e6f   )  # type: igno
+00001d30: 7265 0d0a 2020 2020 2020 2020 656c 7365  re..        else
+00001d40: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00001d50: 656c 662e 7072 6f63 6573 7320 3d20 7375  elf.process = su
+00001d60: 6270 726f 6365 7373 2e50 6f70 656e 280d  bprocess.Popen(.
+00001d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d80: 2063 6d64 5f77 6974 685f 7072 6f67 7265   cmd_with_progre
+00001d90: 7373 2c0d 0a20 2020 2020 2020 2020 2020  ss,..           
+00001da0: 2020 2020 202a 2a62 6173 655f 706f 7065       **base_pope
+00001db0: 6e5f 6b77 6172 6773 2c0d 0a20 2020 2020  n_kwargs,..     
+00001dc0: 2020 2020 2020 2029 2020 2320 7479 7065         )  # type
+00001dd0: 3a20 6967 6e6f 7265 0d0a 0d0a 2020 2020  : ignore....    
+00001de0: 2020 2020 7969 656c 6420 300d 0a0d 0a20      yield 0.... 
+00001df0: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
+00001e00: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001e10: 6966 2073 656c 662e 7072 6f63 6573 732e  if self.process.
+00001e20: 7374 646f 7574 2069 7320 4e6f 6e65 3a0d  stdout is None:.
+00001e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001e40: 2063 6f6e 7469 6e75 650d 0a0d 0a20 2020   continue....   
+00001e50: 2020 2020 2020 2020 2073 7464 6572 725f           stderr_
+00001e60: 6c69 6e65 203d 2028 0d0a 2020 2020 2020  line = (..      
+00001e70: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00001e80: 726f 6365 7373 2e73 7464 6f75 742e 7265  rocess.stdout.re
+00001e90: 6164 6c69 6e65 2829 2e64 6563 6f64 6528  adline().decode(
+00001ea0: 2275 7466 2d38 222c 2065 7272 6f72 733d  "utf-8", errors=
+00001eb0: 2272 6570 6c61 6365 2229 2e73 7472 6970  "replace").strip
+00001ec0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00001ed0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00001ee0: 2069 6620 7365 6c66 2e73 7464 6572 725f   if self.stderr_
+00001ef0: 6361 6c6c 6261 636b 3a0d 0a20 2020 2020  callback:..     
+00001f00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001f10: 7374 6465 7272 5f63 616c 6c62 6163 6b28  stderr_callback(
+00001f20: 7374 6465 7272 5f6c 696e 6529 0d0a 0d0a  stderr_line)....
+00001f30: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00001f40: 7464 6572 725f 6c69 6e65 203d 3d20 2727  tderr_line == ''
+00001f50: 2061 6e64 2073 656c 662e 7072 6f63 6573   and self.proces
+00001f60: 732e 706f 6c6c 2829 2069 7320 6e6f 7420  s.poll() is not 
+00001f70: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00001f80: 2020 2020 2020 2062 7265 616b 0d0a 0d0a         break....
+00001f90: 2020 2020 2020 2020 2020 2020 7374 6465              stde
+00001fa0: 7272 2e61 7070 656e 6428 7374 6465 7272  rr.append(stderr
+00001fb0: 5f6c 696e 652e 7374 7269 7028 2929 0d0a  _line.strip())..
+00001fc0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00001fd0: 6c66 2e73 7464 6572 7220 3d20 225c 6e22  lf.stderr = "\n"
+00001fe0: 2e6a 6f69 6e28 7374 6465 7272 290d 0a0d  .join(stderr)...
+00001ff0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002000: 746f 7461 6c5f 6475 7220 6973 204e 6f6e  total_dur is Non
+00002010: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00002020: 2020 2020 746f 7461 6c5f 6475 725f 6d61      total_dur_ma
+00002030: 7463 6820 3d20 7365 6c66 2e44 5552 5f52  tch = self.DUR_R
+00002040: 4547 4558 2e73 6561 7263 6828 7374 6465  EGEX.search(stde
+00002050: 7272 5f6c 696e 6529 0d0a 2020 2020 2020  rr_line)..      
+00002060: 2020 2020 2020 2020 2020 6966 2074 6f74            if tot
+00002070: 616c 5f64 7572 5f6d 6174 6368 3a0d 0a20  al_dur_match:.. 
+00002080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002090: 2020 2074 6f74 616c 5f64 7572 203d 2074     total_dur = t
+000020a0: 6f5f 6d73 282a 2a74 6f74 616c 5f64 7572  o_ms(**total_dur
+000020b0: 5f6d 6174 6368 2e67 726f 7570 6469 6374  _match.groupdict
+000020c0: 2829 290d 0a20 2020 2020 2020 2020 2020  ())..           
+000020d0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+000020e0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+000020f0: 2020 2065 6c69 6620 6475 7261 7469 6f6e     elif duration
+00002100: 5f6f 7665 7272 6964 6520 6973 206e 6f74  _override is not
+00002110: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00002120: 2020 2020 2020 2020 2020 2020 2320 7573              # us
+00002130: 6520 7468 6520 6f76 6572 7269 6465 2028  e the override (
+00002140: 7368 6f75 6c64 2061 7070 6c79 2069 6e20  should apply in 
+00002150: 7468 6520 6669 7273 7420 6c6f 6f70 290d  the first loop).
+00002160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002170: 2020 2020 2074 6f74 616c 5f64 7572 203d       total_dur =
+00002180: 2069 6e74 2864 7572 6174 696f 6e5f 6f76   int(duration_ov
+00002190: 6572 7269 6465 202a 2031 3030 3029 0d0a  erride * 1000)..
+000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021b0: 2020 2020 636f 6e74 696e 7565 0d0a 0d0a      continue....
+000021c0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+000021d0: 6f74 616c 5f64 7572 3a0d 0a20 2020 2020  otal_dur:..     
+000021e0: 2020 2020 2020 2020 2020 2070 726f 6772             progr
+000021f0: 6573 735f 7469 6d65 203d 2046 666d 7065  ess_time = Ffmpe
+00002200: 6750 726f 6772 6573 732e 5449 4d45 5f52  gProgress.TIME_R
+00002210: 4547 4558 2e73 6561 7263 6828 7374 6465  EGEX.search(stde
+00002220: 7272 5f6c 696e 6529 0d0a 2020 2020 2020  rr_line)..      
+00002230: 2020 2020 2020 2020 2020 6966 2070 726f            if pro
+00002240: 6772 6573 735f 7469 6d65 3a0d 0a20 2020  gress_time:..   
+00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002260: 2065 6c61 7073 6564 5f74 696d 6520 3d20   elapsed_time = 
+00002270: 746f 5f6d 7328 2a2a 7072 6f67 7265 7373  to_ms(**progress
+00002280: 5f74 696d 652e 6772 6f75 7064 6963 7428  _time.groupdict(
+00002290: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000022a0: 2020 2020 2020 2020 7969 656c 6420 696e          yield in
+000022b0: 7428 656c 6170 7365 645f 7469 6d65 202a  t(elapsed_time *
+000022c0: 2031 3030 2f20 746f 7461 6c5f 6475 7229   100/ total_dur)
+000022d0: 0d0a 0d0a 2020 2020 2020 2020 6966 2073  ....        if s
+000022e0: 656c 662e 7072 6f63 6573 7320 6973 204e  elf.process is N
+000022f0: 6f6e 6520 6f72 2073 656c 662e 7072 6f63  one or self.proc
+00002300: 6573 732e 7265 7475 726e 636f 6465 2021  ess.returncode !
+00002310: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+00002320: 2020 5f70 7265 7474 795f 7374 6465 7272    _pretty_stderr
+00002330: 203d 2022 5c6e 222e 6a6f 696e 2873 7464   = "\n".join(std
+00002340: 6572 7229 0d0a 2020 2020 2020 2020 2020  err)..          
+00002350: 2020 7261 6973 6520 5275 6e74 696d 6545    raise RuntimeE
+00002360: 7272 6f72 2866 2245 7272 6f72 2072 756e  rror(f"Error run
+00002370: 6e69 6e67 2063 6f6d 6d61 6e64 207b 7365  ning command {se
+00002380: 6c66 2e63 6d64 7d3a 207b 5f70 7265 7474  lf.cmd}: {_prett
+00002390: 795f 7374 6465 7272 7d22 290d 0a0d 0a20  y_stderr}").... 
+000023a0: 2020 2020 2020 2079 6965 6c64 2031 3030         yield 100
+000023b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+000023c0: 726f 6365 7373 203d 204e 6f6e 650d 0a0d  rocess = None...
+000023d0: 0a20 2020 2064 6566 2071 7569 745f 6772  .    def quit_gr
+000023e0: 6163 6566 756c 6c79 2873 656c 6629 202d  acefully(self) -
+000023f0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
+00002400: 2027 2727 0d0a 2020 2020 2020 2020 5175   '''..        Qu
+00002410: 6974 2074 6865 2066 666d 7065 6720 7072  it the ffmpeg pr
+00002420: 6f63 6573 7320 6279 2073 656e 6469 6e67  ocess by sending
+00002430: 2027 7127 0d0a 0d0a 2020 2020 2020 2020   'q'....        
+00002440: 5261 6973 6573 3a0d 0a20 2020 2020 2020  Raises:..       
+00002450: 2020 2020 2052 756e 7469 6d65 4572 726f       RuntimeErro
+00002460: 723a 2049 6620 6e6f 2070 726f 6365 7373  r: If no process
+00002470: 2069 7320 666f 756e 642e 0d0a 2020 2020   is found...    
+00002480: 2020 2020 2727 270d 0a20 2020 2020 2020      '''..       
+00002490: 2069 6620 7365 6c66 2e70 726f 6365 7373   if self.process
+000024a0: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+000024b0: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
+000024c0: 7469 6d65 4572 726f 7228 224e 6f20 7072  timeError("No pr
+000024d0: 6f63 6573 7320 666f 756e 642e 2044 6964  ocess found. Did
+000024e0: 2079 6f75 2072 756e 2074 6865 2063 6f6d   you run the com
+000024f0: 6d61 6e64 3f22 290d 0a0d 0a20 2020 2020  mand?")....     
+00002500: 2020 2073 656c 662e 7072 6f63 6573 732e     self.process.
+00002510: 636f 6d6d 756e 6963 6174 6528 696e 7075  communicate(inpu
+00002520: 743d 6222 7122 290d 0a20 2020 2020 2020  t=b"q")..       
+00002530: 2073 656c 662e 7072 6f63 6573 732e 6b69   self.process.ki
+00002540: 6c6c 2829 0d0a 2020 2020 2020 2020 7365  ll()..        se
+00002550: 6c66 2e70 726f 6365 7373 203d 204e 6f6e  lf.process = Non
+00002560: 650d 0a0d 0a20 2020 2064 6566 2071 7569  e....    def qui
+00002570: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
+00002580: 0d0a 2020 2020 2020 2020 2727 270d 0a20  ..        '''.. 
+00002590: 2020 2020 2020 2051 7569 7420 7468 6520         Quit the 
+000025a0: 6666 6d70 6567 2070 726f 6365 7373 2062  ffmpeg process b
+000025b0: 7920 7365 6e64 696e 6720 5349 474b 494c  y sending SIGKIL
+000025c0: 4c2e 0d0a 0d0a 2020 2020 2020 2020 5261  L.....        Ra
+000025d0: 6973 6573 3a0d 0a20 2020 2020 2020 2020  ises:..         
+000025e0: 2020 2052 756e 7469 6d65 4572 726f 723a     RuntimeError:
+000025f0: 2049 6620 6e6f 2070 726f 6365 7373 2069   If no process i
+00002600: 7320 666f 756e 642e 0d0a 2020 2020 2020  s found...      
+00002610: 2020 2727 270d 0a20 2020 2020 2020 2069    '''..        i
+00002620: 6620 7365 6c66 2e70 726f 6365 7373 2069  f self.process i
+00002630: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+00002640: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
+00002650: 6d65 4572 726f 7228 224e 6f20 7072 6f63  meError("No proc
+00002660: 6573 7320 666f 756e 642e 2044 6964 2079  ess found. Did y
+00002670: 6f75 2072 756e 2074 6865 2063 6f6d 6d61  ou run the comma
+00002680: 6e64 3f22 290d 0a0d 0a20 2020 2020 2020  nd?")....       
+00002690: 2073 656c 662e 7072 6f63 6573 732e 6b69   self.process.ki
+000026a0: 6c6c 2829 0d0a 2020 2020 2020 2020 7365  ll()..        se
+000026b0: 6c66 2e70 726f 6365 7373 203d 204e 6f6e  lf.process = Non
+000026c0: 650d 0a0d 0a0d 0a23 3d3d 3d3d 3d3d 3d3d  e......#========
+000026d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000026e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000026f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002700: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002710: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002720: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002730: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002740: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d23  ===============#
+00002750: 0d0a 0d0a 0d0a 6465 6620 7374 6f70 5f66  ......def stop_f
+00002760: 666d 7065 675f 7769 6e64 6f77 7328 6572  fmpeg_windows(er
+00002770: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+00002780: 6c62 6163 6b3d 4e6f 6e65 293a 0d0a 2020  lback=None):..  
+00002790: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+000027a0: 7461 736b 6c69 7374 5f6f 7574 7075 7420  tasklist_output 
+000027b0: 3d20 7375 6270 726f 6365 7373 2e63 6865  = subprocess.che
+000027c0: 636b 5f6f 7574 7075 7428 5b27 7461 736b  ck_output(['task
+000027d0: 6c69 7374 275d 2c20 6372 6561 7469 6f6e  list'], creation
+000027e0: 666c 6167 733d 7375 6270 726f 6365 7373  flags=subprocess
+000027f0: 2e43 5245 4154 455f 4e4f 5f57 494e 444f  .CREATE_NO_WINDO
+00002800: 5729 2e64 6563 6f64 6528 2775 7466 2d38  W).decode('utf-8
+00002810: 2729 0d0a 2020 2020 2020 2020 6666 6d70  ')..        ffmp
+00002820: 6567 5f70 6964 203d 204e 6f6e 650d 0a20  eg_pid = None.. 
+00002830: 2020 2020 2020 2066 6f72 206c 696e 6520         for line 
+00002840: 696e 2074 6173 6b6c 6973 745f 6f75 7470  in tasklist_outp
+00002850: 7574 2e73 706c 6974 2827 5c6e 2729 3a0d  ut.split('\n'):.
+00002860: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002870: 2266 666d 7065 6722 2069 6e20 6c69 6e65  "ffmpeg" in line
+00002880: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002890: 2020 2066 666d 7065 675f 7069 6420 3d20     ffmpeg_pid = 
+000028a0: 6c69 6e65 2e73 706c 6974 2829 5b31 5d0d  line.split()[1].
+000028b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000028c0: 2062 7265 616b 0d0a 2020 2020 2020 2020   break..        
+000028d0: 6966 2066 666d 7065 675f 7069 643a 0d0a  if ffmpeg_pid:..
+000028e0: 2020 2020 2020 2020 2020 2020 6465 766e              devn
+000028f0: 756c 6c20 3d20 6f70 656e 286f 732e 6465  ull = open(os.de
+00002900: 766e 756c 6c2c 2027 7727 290d 0a20 2020  vnull, 'w')..   
+00002910: 2020 2020 2020 2020 2073 7562 7072 6f63           subproc
+00002920: 6573 732e 506f 7065 6e28 5b27 7461 736b  ess.Popen(['task
+00002930: 6b69 6c6c 272c 2027 2f46 272c 2027 2f54  kill', '/F', '/T
+00002940: 272c 2027 2f50 4944 272c 2066 666d 7065  ', '/PID', ffmpe
+00002950: 675f 7069 645d 2c20 7374 646f 7574 3d73  g_pid], stdout=s
+00002960: 7562 7072 6f63 6573 732e 5049 5045 2c20  ubprocess.PIPE, 
+00002970: 7374 6465 7272 3d73 7562 7072 6f63 6573  stderr=subproces
+00002980: 732e 5354 444f 5554 2c20 7368 656c 6c3d  s.STDOUT, shell=
+00002990: 5472 7565 2c20 6372 6561 7469 6f6e 666c  True, creationfl
+000029a0: 6167 733d 7375 6270 726f 6365 7373 2e43  ags=subprocess.C
+000029b0: 5245 4154 455f 4e4f 5f57 494e 444f 5729  REATE_NO_WINDOW)
+000029c0: 0d0a 0d0a 2020 2020 6578 6365 7074 204b  ....    except K
+000029d0: 6579 626f 6172 6449 6e74 6572 7275 7074  eyboardInterrupt
+000029e0: 3a0d 0a20 2020 2020 2020 2069 6620 6572  :..        if er
+000029f0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+00002a00: 6c62 6163 6b3a 0d0a 2020 2020 2020 2020  lback:..        
+00002a10: 2020 2020 6572 726f 725f 6d65 7373 6167      error_messag
+00002a20: 6573 5f63 616c 6c62 6163 6b28 2243 616e  es_callback("Can
+00002a30: 6365 6c6c 696e 6720 616c 6c20 7461 736b  celling all task
+00002a40: 7322 290d 0a20 2020 2020 2020 2065 6c73  s")..        els
+00002a50: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00002a60: 7072 696e 7428 2243 616e 6365 6c6c 696e  print("Cancellin
+00002a70: 6720 616c 6c20 7461 736b 7322 290d 0a20  g all tasks").. 
+00002a80: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
+00002a90: 0a20 2020 2065 7863 6570 7420 4578 6365  .    except Exce
+00002aa0: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
+00002ab0: 2020 2020 2069 6620 6572 726f 725f 6d65       if error_me
+00002ac0: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
+00002ad0: 0d0a 2020 2020 2020 2020 2020 2020 6572  ..            er
+00002ae0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+00002af0: 6c62 6163 6b28 6529 0d0a 2020 2020 2020  lback(e)..      
+00002b00: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00002b10: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
+00002b20: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
+00002b30: 0a0d 0a64 6566 2073 746f 705f 6666 6d70  ...def stop_ffmp
+00002b40: 6567 5f6c 696e 7578 2865 7272 6f72 5f6d  eg_linux(error_m
+00002b50: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+00002b60: 3d4e 6f6e 6529 3a0d 0a20 2020 2070 726f  =None):..    pro
+00002b70: 6365 7373 5f6e 616d 6520 3d20 2766 666d  cess_name = 'ffm
+00002b80: 7065 6727 0d0a 2020 2020 7472 793a 0d0a  peg'..    try:..
+00002b90: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
+00002ba0: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
+00002bb0: 6b5f 6f75 7470 7574 285b 2770 7327 2c20  k_output(['ps', 
+00002bc0: 272d 6566 275d 290d 0a20 2020 2020 2020  '-ef'])..       
+00002bd0: 2070 6964 203d 205b 6c69 6e65 2e73 706c   pid = [line.spl
+00002be0: 6974 2829 5b31 5d20 666f 7220 6c69 6e65  it()[1] for line
+00002bf0: 2069 6e20 6f75 7470 7574 2e64 6563 6f64   in output.decod
+00002c00: 6528 2775 7466 2d38 2729 2e73 706c 6974  e('utf-8').split
+00002c10: 2827 5c6e 2729 2069 6620 7072 6f63 6573  ('\n') if proces
+00002c20: 735f 6e61 6d65 2069 6e20 6c69 6e65 5d5b  s_name in line][
+00002c30: 305d 0d0a 2020 2020 2020 2020 7375 6270  0]..        subp
+00002c40: 726f 6365 7373 2e63 616c 6c28 5b27 6b69  rocess.call(['ki
+00002c50: 6c6c 272c 2027 2d39 272c 2073 7472 2870  ll', '-9', str(p
+00002c60: 6964 295d 290d 0a20 2020 2065 7863 6570  id)])..    excep
+00002c70: 7420 496e 6465 7845 7272 6f72 3a0d 0a20  t IndexError:.. 
+00002c80: 2020 2020 2020 2070 6173 730d 0a0d 0a20         pass.... 
+00002c90: 2020 2065 7863 6570 7420 4b65 7962 6f61     except Keyboa
+00002ca0: 7264 496e 7465 7272 7570 743a 0d0a 2020  rdInterrupt:..  
+00002cb0: 2020 2020 2020 6966 2065 7272 6f72 5f6d        if error_m
+00002cc0: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+00002cd0: 3a0d 0a20 2020 2020 2020 2020 2020 2065  :..            e
+00002ce0: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+00002cf0: 6c6c 6261 636b 2822 4361 6e63 656c 6c69  llback("Cancelli
+00002d00: 6e67 2061 6c6c 2074 6173 6b73 2229 0d0a  ng all tasks")..
+00002d10: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00002d20: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00002d30: 2822 4361 6e63 656c 6c69 6e67 2061 6c6c  ("Cancelling all
+00002d40: 2074 6173 6b73 2229 0d0a 2020 2020 2020   tasks")..      
+00002d50: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
+00002d60: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00002d70: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
+00002d80: 6966 2065 7272 6f72 5f6d 6573 7361 6765  if error_message
+00002d90: 735f 6361 6c6c 6261 636b 3a0d 0a20 2020  s_callback:..   
+00002da0: 2020 2020 2020 2020 2065 7272 6f72 5f6d           error_m
+00002db0: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+00002dc0: 2865 290d 0a20 2020 2020 2020 2065 6c73  (e)..        els
+00002dd0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00002de0: 7072 696e 7428 6529 0d0a 2020 2020 2020  print(e)..      
+00002df0: 2020 7265 7475 726e 0d0a 0d0a 0d0a 6465    return......de
+00002e00: 6620 7265 6d6f 7665 5f74 656d 705f 6669  f remove_temp_fi
+00002e10: 6c65 7328 6578 7465 6e73 696f 6e2c 2065  les(extension, e
+00002e20: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+00002e30: 6c6c 6261 636b 3d4e 6f6e 6529 3a0d 0a20  llback=None):.. 
+00002e40: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00002e50: 2074 656d 705f 6469 7220 3d20 7465 6d70   temp_dir = temp
+00002e60: 6669 6c65 2e67 6574 7465 6d70 6469 7228  file.gettempdir(
+00002e70: 290d 0a20 2020 2020 2020 2066 6f72 2072  )..        for r
+00002e80: 6f6f 742c 2064 6972 732c 2066 696c 6573  oot, dirs, files
+00002e90: 2069 6e20 6f73 2e77 616c 6b28 7465 6d70   in os.walk(temp
+00002ea0: 5f64 6972 293a 0d0a 2020 2020 2020 2020  _dir):..        
+00002eb0: 2020 2020 666f 7220 6669 6c65 2069 6e20      for file in 
+00002ec0: 6669 6c65 733a 0d0a 2020 2020 2020 2020  files:..        
+00002ed0: 2020 2020 2020 2020 6966 2066 696c 652e          if file.
+00002ee0: 656e 6473 7769 7468 2822 2e22 202b 2065  endswith("." + e
+00002ef0: 7874 656e 7369 6f6e 293a 0d0a 2020 2020  xtension):..    
+00002f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f10: 6f73 2e72 656d 6f76 6528 6f73 2e70 6174  os.remove(os.pat
+00002f20: 682e 6a6f 696e 2872 6f6f 742c 2066 696c  h.join(root, fil
+00002f30: 6529 290d 0a20 2020 2065 7863 6570 7420  e))..    except 
+00002f40: 4b65 7962 6f61 7264 496e 7465 7272 7570  KeyboardInterrup
+00002f50: 743a 0d0a 2020 2020 2020 2020 6966 2065  t:..        if e
+00002f60: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+00002f70: 6c6c 6261 636b 3a0d 0a20 2020 2020 2020  llback:..       
+00002f80: 2020 2020 2065 7272 6f72 5f6d 6573 7361       error_messa
+00002f90: 6765 735f 6361 6c6c 6261 636b 2822 4361  ges_callback("Ca
+00002fa0: 6e63 656c 6c69 6e67 2061 6c6c 2074 6173  ncelling all tas
+00002fb0: 6b73 2229 0d0a 2020 2020 2020 2020 656c  ks")..        el
+00002fc0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00002fd0: 2070 7269 6e74 2822 4361 6e63 656c 6c69   print("Cancelli
+00002fe0: 6e67 2061 6c6c 2074 6173 6b73 2229 0d0a  ng all tasks")..
+00002ff0: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+00003000: 0d0a 2020 2020 6578 6365 7074 2045 7863  ..    except Exc
+00003010: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
+00003020: 2020 2020 2020 6966 2065 7272 6f72 5f6d        if error_m
+00003030: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+00003040: 3a0d 0a20 2020 2020 2020 2020 2020 2065  :..            e
+00003050: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+00003060: 6c6c 6261 636b 2865 290d 0a20 2020 2020  llback(e)..     
+00003070: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00003080: 2020 2020 2020 7072 696e 7428 6529 0d0a        print(e)..
+00003090: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+000030a0: 0d0a 0d0a 6465 6620 6973 5f73 616d 655f  ....def is_same_
+000030b0: 6c61 6e67 7561 6765 2873 7263 2c20 6473  language(src, ds
+000030c0: 742c 2065 7272 6f72 5f6d 6573 7361 6765  t, error_message
+000030d0: 735f 6361 6c6c 6261 636b 3d4e 6f6e 6529  s_callback=None)
+000030e0: 3a0d 0a20 2020 2074 7279 3a0d 0a20 2020  :..    try:..   
+000030f0: 2020 2020 2072 6574 7572 6e20 7372 632e       return src.
+00003100: 7370 6c69 7428 222d 2229 5b30 5d20 3d3d  split("-")[0] ==
+00003110: 2064 7374 2e73 706c 6974 2822 2d22 295b   dst.split("-")[
+00003120: 305d 0d0a 2020 2020 6578 6365 7074 2045  0]..    except E
+00003130: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
+00003140: 2020 2020 2020 2020 6966 2065 7272 6f72          if error
+00003150: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+00003160: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
+00003170: 2065 7272 6f72 5f6d 6573 7361 6765 735f   error_messages_
+00003180: 6361 6c6c 6261 636b 2865 290d 0a20 2020  callback(e)..   
+00003190: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+000031a0: 2020 2020 2020 2020 7072 696e 7428 6529          print(e)
+000031b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000031c0: 0d0a 0d0a 0d0a 6465 6620 6368 6563 6b5f  ......def check_
+000031d0: 6669 6c65 5f74 7970 6528 6669 6c65 5f70  file_type(file_p
+000031e0: 6174 682c 2065 7272 6f72 5f6d 6573 7361  ath, error_messa
+000031f0: 6765 735f 6361 6c6c 6261 636b 3d4e 6f6e  ges_callback=Non
+00003200: 6529 3a0d 0a20 2020 2074 7279 3a0d 0a20  e):..    try:.. 
+00003210: 2020 2020 2020 2066 6670 726f 6265 5f63         ffprobe_c
+00003220: 6d64 203d 205b 2766 6670 726f 6265 272c  md = ['ffprobe',
+00003230: 2027 2d76 272c 2027 6572 726f 7227 2c20   '-v', 'error', 
+00003240: 272d 7368 6f77 5f66 6f72 6d61 7427 2c20  '-show_format', 
+00003250: 272d 7368 6f77 5f73 7472 6561 6d73 272c  '-show_streams',
+00003260: 2027 2d70 7269 6e74 5f66 6f72 6d61 7427   '-print_format'
+00003270: 2c20 276a 736f 6e27 2c20 6669 6c65 5f70  , 'json', file_p
+00003280: 6174 685d 0d0a 2020 2020 2020 2020 6f75  ath]..        ou
+00003290: 7470 7574 203d 204e 6f6e 650d 0a20 2020  tput = None..   
+000032a0: 2020 2020 2069 6620 7379 732e 706c 6174       if sys.plat
+000032b0: 666f 726d 203d 3d20 2277 696e 3332 223a  form == "win32":
+000032c0: 0d0a 2020 2020 2020 2020 2020 2020 6f75  ..            ou
+000032d0: 7470 7574 203d 2073 7562 7072 6f63 6573  tput = subproces
+000032e0: 732e 6368 6563 6b5f 6f75 7470 7574 2866  s.check_output(f
+000032f0: 6670 726f 6265 5f63 6d64 2c20 6372 6561  fprobe_cmd, crea
+00003300: 7469 6f6e 666c 6167 733d 7375 6270 726f  tionflags=subpro
+00003310: 6365 7373 2e43 5245 4154 455f 4e4f 5f57  cess.CREATE_NO_W
+00003320: 494e 444f 5729 2e64 6563 6f64 6528 2775  INDOW).decode('u
+00003330: 7466 2d38 2729 0d0a 2020 2020 2020 2020  tf-8')..        
+00003340: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00003350: 2020 206f 7574 7075 7420 3d20 7375 6270     output = subp
+00003360: 726f 6365 7373 2e63 6865 636b 5f6f 7574  rocess.check_out
+00003370: 7075 7428 6666 7072 6f62 655f 636d 6429  put(ffprobe_cmd)
+00003380: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
+00003390: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+000033a0: 206a 736f 6e2e 6c6f 6164 7328 6f75 7470   json.loads(outp
+000033b0: 7574 290d 0a0d 0a20 2020 2020 2020 2069  ut)....        i
+000033c0: 6620 2773 7472 6561 6d73 2720 696e 2064  f 'streams' in d
+000033d0: 6174 613a 0d0a 2020 2020 2020 2020 2020  ata:..          
+000033e0: 2020 666f 7220 7374 7265 616d 2069 6e20    for stream in 
+000033f0: 6461 7461 5b27 7374 7265 616d 7327 5d3a  data['streams']:
+00003400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003410: 2020 6966 2027 636f 6465 635f 7479 7065    if 'codec_type
+00003420: 2720 696e 2073 7472 6561 6d20 616e 6420  ' in stream and 
+00003430: 7374 7265 616d 5b27 636f 6465 635f 7479  stream['codec_ty
+00003440: 7065 275d 203d 3d20 2761 7564 696f 273a  pe'] == 'audio':
+00003450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003460: 2020 2020 2020 7265 7475 726e 2027 6175        return 'au
+00003470: 6469 6f27 0d0a 2020 2020 2020 2020 2020  dio'..          
+00003480: 2020 2020 2020 656c 6966 2027 636f 6465        elif 'code
+00003490: 635f 7479 7065 2720 696e 2073 7472 6561  c_type' in strea
+000034a0: 6d20 616e 6420 7374 7265 616d 5b27 636f  m and stream['co
+000034b0: 6465 635f 7479 7065 275d 203d 3d20 2776  dec_type'] == 'v
+000034c0: 6964 656f 273a 0d0a 2020 2020 2020 2020  ideo':..        
+000034d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000034e0: 726e 2027 7669 6465 6f27 0d0a 2020 2020  rn 'video'..    
+000034f0: 6578 6365 7074 2028 7375 6270 726f 6365  except (subproce
+00003500: 7373 2e43 616c 6c65 6450 726f 6365 7373  ss.CalledProcess
+00003510: 4572 726f 722c 206a 736f 6e2e 4a53 4f4e  Error, json.JSON
+00003520: 4465 636f 6465 4572 726f 7229 3a0d 0a20  DecodeError):.. 
+00003530: 2020 2020 2020 2070 6173 730d 0a0d 0a20         pass.... 
+00003540: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00003550: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
+00003560: 2020 2069 6620 6572 726f 725f 6d65 7373     if error_mess
+00003570: 6167 6573 5f63 616c 6c62 6163 6b3a 0d0a  ages_callback:..
+00003580: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+00003590: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+000035a0: 6163 6b28 6529 0d0a 2020 2020 2020 2020  ack(e)..        
+000035b0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000035c0: 2020 2070 7269 6e74 2865 290d 0a0d 0a20     print(e).... 
+000035d0: 2020 2072 6574 7572 6e20 4e6f 6e65 0d0a     return None..
+000035e0: 0d0a 0d0a 636c 6173 7320 5768 6973 7065  ....class Whispe
+000035f0: 724c 616e 6775 6167 653a 0d0a 2020 2020  rLanguage:..    
+00003600: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00003610: 6629 3a0d 0a20 2020 2020 2020 2073 656c  f):..        sel
+00003620: 662e 6c69 7374 5f63 6f64 6573 203d 205b  f.list_codes = [
+00003630: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
+00003640: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00003650: 6428 2261 6622 290d 0a20 2020 2020 2020  d("af")..       
+00003660: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00003670: 2e61 7070 656e 6428 2273 7122 290d 0a20  .append("sq").. 
+00003680: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00003690: 5f63 6f64 6573 2e61 7070 656e 6428 2261  _codes.append("a
+000036a0: 6d22 290d 0a20 2020 2020 2020 2073 656c  m")..        sel
+000036b0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+000036c0: 656e 6428 2261 7222 290d 0a20 2020 2020  end("ar")..     
+000036d0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+000036e0: 6573 2e61 7070 656e 6428 2268 7922 290d  es.append("hy").
+000036f0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00003700: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00003710: 2261 7322 290d 0a20 2020 2020 2020 2073  "as")..        s
+00003720: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00003730: 7070 656e 6428 2261 7a22 290d 0a20 2020  ppend("az")..   
+00003740: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00003750: 6f64 6573 2e61 7070 656e 6428 2262 6122  odes.append("ba"
+00003760: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003770: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00003780: 6428 2265 7522 290d 0a20 2020 2020 2020  d("eu")..       
+00003790: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+000037a0: 2e61 7070 656e 6428 2262 6522 290d 0a20  .append("be").. 
+000037b0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000037c0: 5f63 6f64 6573 2e61 7070 656e 6428 2262  _codes.append("b
+000037d0: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+000037e0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+000037f0: 656e 6428 2262 7322 290d 0a20 2020 2020  end("bs")..     
+00003800: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00003810: 6573 2e61 7070 656e 6428 2262 7222 290d  es.append("br").
+00003820: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00003830: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00003840: 2262 6722 290d 0a20 2020 2020 2020 2073  "bg")..        s
+00003850: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00003860: 7070 656e 6428 2263 6122 290d 0a20 2020  ppend("ca")..   
+00003870: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00003880: 6f64 6573 2e61 7070 656e 6428 227a 6822  odes.append("zh"
+00003890: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000038a0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+000038b0: 6428 2268 7222 290d 0a20 2020 2020 2020  d("hr")..       
+000038c0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+000038d0: 2e61 7070 656e 6428 2263 7322 290d 0a20  .append("cs").. 
+000038e0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000038f0: 5f63 6f64 6573 2e61 7070 656e 6428 2264  _codes.append("d
+00003900: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
+00003910: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00003920: 656e 6428 226e 6c22 290d 0a20 2020 2020  end("nl")..     
+00003930: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00003940: 6573 2e61 7070 656e 6428 2265 6e22 290d  es.append("en").
+00003950: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00003960: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00003970: 2265 7422 290d 0a20 2020 2020 2020 2073  "et")..        s
+00003980: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00003990: 7070 656e 6428 2266 6f22 290d 0a20 2020  ppend("fo")..   
+000039a0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+000039b0: 6f64 6573 2e61 7070 656e 6428 2266 6922  odes.append("fi"
+000039c0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000039d0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+000039e0: 6428 2266 7222 290d 0a20 2020 2020 2020  d("fr")..       
+000039f0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00003a00: 2e61 7070 656e 6428 2267 6c22 290d 0a20  .append("gl").. 
+00003a10: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00003a20: 5f63 6f64 6573 2e61 7070 656e 6428 226b  _codes.append("k
+00003a30: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
+00003a40: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00003a50: 656e 6428 2264 6522 290d 0a20 2020 2020  end("de")..     
+00003a60: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00003a70: 6573 2e61 7070 656e 6428 2265 6c22 290d  es.append("el").
+00003a80: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00003a90: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00003aa0: 2267 7522 290d 0a20 2020 2020 2020 2073  "gu")..        s
+00003ab0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00003ac0: 7070 656e 6428 2268 7422 290d 0a20 2020  ppend("ht")..   
+00003ad0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00003ae0: 6f64 6573 2e61 7070 656e 6428 2268 6122  odes.append("ha"
+00003af0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003b00: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00003b10: 6428 2268 6177 2229 0d0a 2020 2020 2020  d("haw")..      
+00003b20: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00003b30: 732e 6170 7065 6e64 2822 6865 2229 0d0a  s.append("he")..
+00003b40: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00003b50: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00003b60: 6869 2229 0d0a 2020 2020 2020 2020 7365  hi")..        se
+00003b70: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00003b80: 7065 6e64 2822 6875 2229 0d0a 2020 2020  pend("hu")..    
+00003b90: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00003ba0: 6465 732e 6170 7065 6e64 2822 6973 2229  des.append("is")
+00003bb0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00003bc0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00003bd0: 2822 6964 2229 0d0a 2020 2020 2020 2020  ("id")..        
+00003be0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00003bf0: 6170 7065 6e64 2822 6974 2229 0d0a 2020  append("it")..  
+00003c00: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00003c10: 636f 6465 732e 6170 7065 6e64 2822 6a61  codes.append("ja
+00003c20: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00003c30: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00003c40: 6e64 2822 6a76 2229 0d0a 2020 2020 2020  nd("jv")..      
+00003c50: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00003c60: 732e 6170 7065 6e64 2822 6b6e 2229 0d0a  s.append("kn")..
+00003c70: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00003c80: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00003c90: 6b6b 2229 0d0a 2020 2020 2020 2020 7365  kk")..        se
+00003ca0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00003cb0: 7065 6e64 2822 6b6d 2229 0d0a 2020 2020  pend("km")..    
+00003cc0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00003cd0: 6465 732e 6170 7065 6e64 2822 6b6f 2229  des.append("ko")
+00003ce0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00003cf0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00003d00: 2822 6c6f 2229 0d0a 2020 2020 2020 2020  ("lo")..        
+00003d10: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00003d20: 6170 7065 6e64 2822 6c61 2229 0d0a 2020  append("la")..  
+00003d30: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00003d40: 636f 6465 732e 6170 7065 6e64 2822 6c76  codes.append("lv
+00003d50: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00003d60: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00003d70: 6e64 2822 6c6e 2229 0d0a 2020 2020 2020  nd("ln")..      
+00003d80: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00003d90: 732e 6170 7065 6e64 2822 6c74 2229 0d0a  s.append("lt")..
+00003da0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00003db0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00003dc0: 6c62 2229 0d0a 2020 2020 2020 2020 7365  lb")..        se
+00003dd0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00003de0: 7065 6e64 2822 6d6b 2229 0d0a 2020 2020  pend("mk")..    
+00003df0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00003e00: 6465 732e 6170 7065 6e64 2822 6d67 2229  des.append("mg")
+00003e10: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00003e20: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00003e30: 2822 6d73 2229 0d0a 2020 2020 2020 2020  ("ms")..        
+00003e40: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00003e50: 6170 7065 6e64 2822 6d6c 2229 0d0a 2020  append("ml")..  
+00003e60: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00003e70: 636f 6465 732e 6170 7065 6e64 2822 6d74  codes.append("mt
+00003e80: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00003e90: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00003ea0: 6e64 2822 6d69 2229 0d0a 2020 2020 2020  nd("mi")..      
+00003eb0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00003ec0: 732e 6170 7065 6e64 2822 6d72 2229 0d0a  s.append("mr")..
+00003ed0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00003ee0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00003ef0: 6d6e 2229 0d0a 2020 2020 2020 2020 7365  mn")..        se
+00003f00: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00003f10: 7065 6e64 2822 6d79 2229 0d0a 2020 2020  pend("my")..    
+00003f20: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00003f30: 6465 732e 6170 7065 6e64 2822 6e65 2229  des.append("ne")
+00003f40: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00003f50: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00003f60: 2822 6e6f 2229 0d0a 2020 2020 2020 2020  ("no")..        
+00003f70: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00003f80: 6170 7065 6e64 2822 6e6e 2229 0d0a 2020  append("nn")..  
+00003f90: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00003fa0: 636f 6465 732e 6170 7065 6e64 2822 6f63  codes.append("oc
+00003fb0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00003fc0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00003fd0: 6e64 2822 7073 2229 0d0a 2020 2020 2020  nd("ps")..      
+00003fe0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00003ff0: 732e 6170 7065 6e64 2822 6661 2229 0d0a  s.append("fa")..
+00004000: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004010: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00004020: 706c 2229 0d0a 2020 2020 2020 2020 7365  pl")..        se
+00004030: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00004040: 7065 6e64 2822 7074 2229 0d0a 2020 2020  pend("pt")..    
+00004050: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00004060: 6465 732e 6170 7065 6e64 2822 7061 2229  des.append("pa")
+00004070: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00004080: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00004090: 2822 726f 2229 0d0a 2020 2020 2020 2020  ("ro")..        
+000040a0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+000040b0: 6170 7065 6e64 2822 7275 2229 0d0a 2020  append("ru")..  
+000040c0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000040d0: 636f 6465 732e 6170 7065 6e64 2822 7361  codes.append("sa
+000040e0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000040f0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00004100: 6e64 2822 7372 2229 0d0a 2020 2020 2020  nd("sr")..      
+00004110: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00004120: 732e 6170 7065 6e64 2822 736e 2229 0d0a  s.append("sn")..
+00004130: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004140: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00004150: 7364 2229 0d0a 2020 2020 2020 2020 7365  sd")..        se
+00004160: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00004170: 7065 6e64 2822 7369 2229 0d0a 2020 2020  pend("si")..    
+00004180: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00004190: 6465 732e 6170 7065 6e64 2822 736b 2229  des.append("sk")
+000041a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000041b0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+000041c0: 2822 736c 2229 0d0a 2020 2020 2020 2020  ("sl")..        
+000041d0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+000041e0: 6170 7065 6e64 2822 736f 2229 0d0a 2020  append("so")..  
+000041f0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004200: 636f 6465 732e 6170 7065 6e64 2822 6573  codes.append("es
+00004210: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004220: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00004230: 6e64 2822 7375 2229 0d0a 2020 2020 2020  nd("su")..      
+00004240: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00004250: 732e 6170 7065 6e64 2822 7377 2229 0d0a  s.append("sw")..
+00004260: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004270: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00004280: 7376 2229 0d0a 2020 2020 2020 2020 7365  sv")..        se
+00004290: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+000042a0: 7065 6e64 2822 746c 2229 0d0a 2020 2020  pend("tl")..    
+000042b0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+000042c0: 6465 732e 6170 7065 6e64 2822 7467 2229  des.append("tg")
+000042d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000042e0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+000042f0: 2822 7461 2229 0d0a 2020 2020 2020 2020  ("ta")..        
+00004300: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00004310: 6170 7065 6e64 2822 7474 2229 0d0a 2020  append("tt")..  
+00004320: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004330: 636f 6465 732e 6170 7065 6e64 2822 7465  codes.append("te
+00004340: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004350: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00004360: 6e64 2822 7468 2229 0d0a 2020 2020 2020  nd("th")..      
+00004370: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00004380: 732e 6170 7065 6e64 2822 626f 2229 0d0a  s.append("bo")..
+00004390: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000043a0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+000043b0: 7472 2229 0d0a 2020 2020 2020 2020 7365  tr")..        se
+000043c0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+000043d0: 7065 6e64 2822 746b 2229 0d0a 2020 2020  pend("tk")..    
+000043e0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+000043f0: 6465 732e 6170 7065 6e64 2822 756b 2229  des.append("uk")
+00004400: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00004410: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00004420: 2822 7572 2229 0d0a 2020 2020 2020 2020  ("ur")..        
+00004430: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00004440: 6170 7065 6e64 2822 757a 2229 0d0a 2020  append("uz")..  
+00004450: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004460: 636f 6465 732e 6170 7065 6e64 2822 7669  codes.append("vi
+00004470: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004480: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00004490: 6e64 2822 6379 2229 0d0a 2020 2020 2020  nd("cy")..      
+000044a0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+000044b0: 732e 6170 7065 6e64 2822 7969 2229 0d0a  s.append("yi")..
+000044c0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000044d0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+000044e0: 796f 2229 0d0a 0d0a 2020 2020 2020 2020  yo")....        
+000044f0: 7365 6c66 2e6c 6973 745f 6e61 6d65 7320  self.list_names 
+00004500: 3d20 5b5d 0d0a 2020 2020 2020 2020 7365  = []..        se
+00004510: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00004520: 7065 6e64 2822 4166 7269 6b61 616e 7322  pend("Afrikaans"
+00004530: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004540: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00004550: 6428 2241 6c62 616e 6961 6e22 290d 0a20  d("Albanian").. 
+00004560: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00004570: 5f6e 616d 6573 2e61 7070 656e 6428 2241  _names.append("A
+00004580: 6d68 6172 6963 2229 0d0a 2020 2020 2020  mharic")..      
+00004590: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+000045a0: 732e 6170 7065 6e64 2822 4172 6162 6963  s.append("Arabic
+000045b0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000045c0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+000045d0: 6e64 2822 4172 6d65 6e69 616e 2229 0d0a  nd("Armenian")..
+000045e0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000045f0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00004600: 4173 7361 6d65 7365 2229 0d0a 2020 2020  Assamese")..    
+00004610: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00004620: 6d65 732e 6170 7065 6e64 2822 417a 6572  mes.append("Azer
+00004630: 6261 696a 616e 6922 290d 0a20 2020 2020  baijani")..     
+00004640: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004650: 6573 2e61 7070 656e 6428 2242 6173 686b  es.append("Bashk
+00004660: 6972 2229 0d0a 2020 2020 2020 2020 7365  ir")..        se
+00004670: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00004680: 7065 6e64 2822 4261 7371 7565 2229 0d0a  pend("Basque")..
+00004690: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000046a0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000046b0: 4265 6c61 7275 7369 616e 2229 0d0a 2020  Belarusian")..  
+000046c0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000046d0: 6e61 6d65 732e 6170 7065 6e64 2822 4265  names.append("Be
+000046e0: 6e67 616c 6922 290d 0a20 2020 2020 2020  ngali")..       
+000046f0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004700: 2e61 7070 656e 6428 2242 6f73 6e69 616e  .append("Bosnian
+00004710: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004720: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00004730: 6e64 2822 4272 6574 6f6e 2229 0d0a 2020  nd("Breton")..  
+00004740: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004750: 6e61 6d65 732e 6170 7065 6e64 2822 4275  names.append("Bu
+00004760: 6c67 6172 6961 6e22 290d 0a20 2020 2020  lgarian")..     
+00004770: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004780: 6573 2e61 7070 656e 6428 2243 6174 616c  es.append("Catal
+00004790: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
+000047a0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+000047b0: 7065 6e64 2822 4368 696e 6573 6522 290d  pend("Chinese").
+000047c0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000047d0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+000047e0: 2243 726f 6174 6961 6e22 290d 0a20 2020  "Croatian")..   
+000047f0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00004800: 616d 6573 2e61 7070 656e 6428 2243 7a65  ames.append("Cze
+00004810: 6368 2229 0d0a 2020 2020 2020 2020 7365  ch")..        se
+00004820: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00004830: 7065 6e64 2822 4461 6e69 7368 2229 0d0a  pend("Danish")..
+00004840: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004850: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00004860: 4475 7463 6822 290d 0a20 2020 2020 2020  Dutch")..       
+00004870: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004880: 2e61 7070 656e 6428 2245 6e67 6c69 7368  .append("English
+00004890: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000048a0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+000048b0: 6e64 2822 4573 746f 6e69 616e 2229 0d0a  nd("Estonian")..
+000048c0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000048d0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000048e0: 4661 726f 6573 6522 290d 0a20 2020 2020  Faroese")..     
+000048f0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004900: 6573 2e61 7070 656e 6428 2246 696e 6e69  es.append("Finni
+00004910: 7368 2229 0d0a 2020 2020 2020 2020 7365  sh")..        se
+00004920: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00004930: 7065 6e64 2822 4672 656e 6368 2229 0d0a  pend("French")..
+00004940: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004950: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00004960: 4761 6c69 6369 616e 2229 0d0a 2020 2020  Galician")..    
+00004970: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00004980: 6d65 732e 6170 7065 6e64 2822 4765 6f72  mes.append("Geor
+00004990: 6769 616e 2229 0d0a 2020 2020 2020 2020  gian")..        
+000049a0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+000049b0: 6170 7065 6e64 2822 4765 726d 616e 2229  append("German")
+000049c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000049d0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+000049e0: 2822 4772 6565 6b22 290d 0a20 2020 2020  ("Greek")..     
+000049f0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004a00: 6573 2e61 7070 656e 6428 2247 756a 6172  es.append("Gujar
+00004a10: 6174 6922 290d 0a20 2020 2020 2020 2073  ati")..        s
+00004a20: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00004a30: 7070 656e 6428 2248 6169 7469 616e 2043  ppend("Haitian C
+00004a40: 7265 6f6c 6522 290d 0a20 2020 2020 2020  reole")..       
+00004a50: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004a60: 2e61 7070 656e 6428 2248 6175 7361 2229  .append("Hausa")
+00004a70: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00004a80: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00004a90: 2822 4861 7761 6969 616e 2229 0d0a 2020  ("Hawaiian")..  
+00004aa0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004ab0: 6e61 6d65 732e 6170 7065 6e64 2822 4865  names.append("He
+00004ac0: 6272 6577 2229 0d0a 2020 2020 2020 2020  brew")..        
+00004ad0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00004ae0: 6170 7065 6e64 2822 4869 6e64 6922 290d  append("Hindi").
+00004af0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004b00: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00004b10: 2248 756e 6761 7269 616e 2229 0d0a 2020  "Hungarian")..  
+00004b20: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004b30: 6e61 6d65 732e 6170 7065 6e64 2822 4963  names.append("Ic
+00004b40: 656c 616e 6469 6322 290d 0a20 2020 2020  elandic")..     
+00004b50: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004b60: 6573 2e61 7070 656e 6428 2249 6e64 6f6e  es.append("Indon
+00004b70: 6573 6961 6e22 290d 0a20 2020 2020 2020  esian")..       
+00004b80: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004b90: 2e61 7070 656e 6428 2249 7461 6c69 616e  .append("Italian
+00004ba0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004bb0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00004bc0: 6e64 2822 4a61 7061 6e65 7365 2229 0d0a  nd("Japanese")..
+00004bd0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004be0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00004bf0: 4a61 7661 6e65 7365 2229 0d0a 2020 2020  Javanese")..    
+00004c00: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00004c10: 6d65 732e 6170 7065 6e64 2822 4b61 6e6e  mes.append("Kann
+00004c20: 6164 6122 290d 0a20 2020 2020 2020 2073  ada")..        s
+00004c30: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00004c40: 7070 656e 6428 224b 617a 616b 6822 290d  ppend("Kazakh").
+00004c50: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004c60: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00004c70: 224b 686d 6572 2229 0d0a 2020 2020 2020  "Khmer")..      
+00004c80: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00004c90: 732e 6170 7065 6e64 2822 4b6f 7265 616e  s.append("Korean
+00004ca0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004cb0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00004cc0: 6e64 2822 4c61 6f22 290d 0a20 2020 2020  nd("Lao")..     
+00004cd0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004ce0: 6573 2e61 7070 656e 6428 224c 6174 696e  es.append("Latin
+00004cf0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004d00: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00004d10: 6e64 2822 4c61 7476 6961 6e22 290d 0a20  nd("Latvian").. 
+00004d20: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00004d30: 5f6e 616d 6573 2e61 7070 656e 6428 224c  _names.append("L
+00004d40: 696e 6761 6c61 2229 0d0a 2020 2020 2020  ingala")..      
+00004d50: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00004d60: 732e 6170 7065 6e64 2822 4c69 7468 7561  s.append("Lithua
+00004d70: 6e69 616e 2229 0d0a 2020 2020 2020 2020  nian")..        
+00004d80: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00004d90: 6170 7065 6e64 2822 4c75 7865 6d62 6f75  append("Luxembou
+00004da0: 7267 6973 6822 290d 0a20 2020 2020 2020  rgish")..       
+00004db0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004dc0: 2e61 7070 656e 6428 224d 6163 6564 6f6e  .append("Macedon
+00004dd0: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
+00004de0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00004df0: 7070 656e 6428 224d 616c 6167 6173 7922  ppend("Malagasy"
+00004e00: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004e10: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00004e20: 6428 224d 616c 6179 2229 0d0a 2020 2020  d("Malay")..    
+00004e30: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00004e40: 6d65 732e 6170 7065 6e64 2822 4d61 6c61  mes.append("Mala
+00004e50: 7961 6c61 6d22 290d 0a20 2020 2020 2020  yalam")..       
+00004e60: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004e70: 2e61 7070 656e 6428 224d 616c 7465 7365  .append("Maltese
+00004e80: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004e90: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00004ea0: 6e64 2822 4d61 6f72 6922 290d 0a20 2020  nd("Maori")..   
+00004eb0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00004ec0: 616d 6573 2e61 7070 656e 6428 224d 6172  ames.append("Mar
+00004ed0: 6174 6869 2229 0d0a 2020 2020 2020 2020  athi")..        
+00004ee0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00004ef0: 6170 7065 6e64 2822 4d6f 6e67 6f6c 6961  append("Mongolia
+00004f00: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00004f10: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00004f20: 656e 6428 224d 7961 6e6d 6172 2028 4275  end("Myanmar (Bu
+00004f30: 726d 6573 6529 2229 0d0a 2020 2020 2020  rmese)")..      
+00004f40: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00004f50: 732e 6170 7065 6e64 2822 4e65 7061 6c69  s.append("Nepali
+00004f60: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004f70: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00004f80: 6e64 2822 4e6f 7277 6567 6961 6e22 290d  nd("Norwegian").
+00004f90: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004fa0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00004fb0: 224e 796e 6f72 736b 2229 0d0a 2020 2020  "Nynorsk")..    
+00004fc0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00004fd0: 6d65 732e 6170 7065 6e64 2822 4f63 6369  mes.append("Occi
+00004fe0: 7461 6e22 290d 0a20 2020 2020 2020 2073  tan")..        s
+00004ff0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00005000: 7070 656e 6428 2250 6173 6874 6f22 290d  ppend("Pashto").
+00005010: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00005020: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00005030: 2250 6572 7369 616e 2229 0d0a 2020 2020  "Persian")..    
+00005040: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00005050: 6d65 732e 6170 7065 6e64 2822 506f 6c69  mes.append("Poli
+00005060: 7368 2229 0d0a 2020 2020 2020 2020 7365  sh")..        se
+00005070: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00005080: 7065 6e64 2822 506f 7274 7567 7565 7365  pend("Portuguese
+00005090: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000050a0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+000050b0: 6e64 2822 5075 6e6a 6162 6922 290d 0a20  nd("Punjabi").. 
+000050c0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000050d0: 5f6e 616d 6573 2e61 7070 656e 6428 2252  _names.append("R
+000050e0: 6f6d 616e 6961 6e22 290d 0a20 2020 2020  omanian")..     
+000050f0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00005100: 6573 2e61 7070 656e 6428 2252 7573 7369  es.append("Russi
+00005110: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
+00005120: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00005130: 7065 6e64 2822 5361 6e73 6b72 6974 2229  pend("Sanskrit")
+00005140: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00005150: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00005160: 2822 5365 7262 6961 6e22 290d 0a20 2020  ("Serbian")..   
+00005170: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00005180: 616d 6573 2e61 7070 656e 6428 2253 686f  ames.append("Sho
+00005190: 6e61 2229 0d0a 2020 2020 2020 2020 7365  na")..        se
+000051a0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+000051b0: 7065 6e64 2822 5369 6e64 6869 2229 0d0a  pend("Sindhi")..
+000051c0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000051d0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000051e0: 5369 6e68 616c 6122 290d 0a20 2020 2020  Sinhala")..     
+000051f0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00005200: 6573 2e61 7070 656e 6428 2253 6c6f 7661  es.append("Slova
+00005210: 6b22 290d 0a20 2020 2020 2020 2073 656c  k")..        sel
+00005220: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00005230: 656e 6428 2253 6c6f 7665 6e69 616e 2229  end("Slovenian")
+00005240: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00005250: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00005260: 2822 536f 6d61 6c69 2229 0d0a 2020 2020  ("Somali")..    
+00005270: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00005280: 6d65 732e 6170 7065 6e64 2822 5370 616e  mes.append("Span
+00005290: 6973 6822 290d 0a20 2020 2020 2020 2073  ish")..        s
+000052a0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+000052b0: 7070 656e 6428 2253 756e 6461 6e65 7365  ppend("Sundanese
+000052c0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000052d0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+000052e0: 6e64 2822 5377 6168 696c 6922 290d 0a20  nd("Swahili").. 
+000052f0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00005300: 5f6e 616d 6573 2e61 7070 656e 6428 2253  _names.append("S
+00005310: 7765 6469 7368 2229 0d0a 2020 2020 2020  wedish")..      
+00005320: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00005330: 732e 6170 7065 6e64 2822 5461 6761 6c6f  s.append("Tagalo
+00005340: 6722 290d 0a20 2020 2020 2020 2073 656c  g")..        sel
+00005350: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00005360: 656e 6428 2254 616a 696b 2229 0d0a 2020  end("Tajik")..  
+00005370: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00005380: 6e61 6d65 732e 6170 7065 6e64 2822 5461  names.append("Ta
+00005390: 6d69 6c22 290d 0a20 2020 2020 2020 2073  mil")..        s
+000053a0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+000053b0: 7070 656e 6428 2254 6174 6172 2229 0d0a  ppend("Tatar")..
+000053c0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000053d0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000053e0: 5465 6c75 6775 2229 0d0a 2020 2020 2020  Telugu")..      
+000053f0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00005400: 732e 6170 7065 6e64 2822 5468 6169 2229  s.append("Thai")
+00005410: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00005420: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00005430: 2822 5469 6265 7461 6e22 290d 0a20 2020  ("Tibetan")..   
+00005440: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00005450: 616d 6573 2e61 7070 656e 6428 2254 7572  ames.append("Tur
+00005460: 6b69 7368 2229 0d0a 2020 2020 2020 2020  kish")..        
+00005470: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00005480: 6170 7065 6e64 2822 5475 726b 6d65 6e22  append("Turkmen"
+00005490: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000054a0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+000054b0: 6428 2255 6b72 6169 6e69 616e 2229 0d0a  d("Ukrainian")..
+000054c0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000054d0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000054e0: 5572 6475 2229 0d0a 2020 2020 2020 2020  Urdu")..        
+000054f0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00005500: 6170 7065 6e64 2822 557a 6265 6b22 290d  append("Uzbek").
+00005510: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00005520: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00005530: 2256 6965 746e 616d 6573 6522 290d 0a20  "Vietnamese").. 
+00005540: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00005550: 5f6e 616d 6573 2e61 7070 656e 6428 2257  _names.append("W
+00005560: 656c 7368 2229 0d0a 2020 2020 2020 2020  elsh")..        
+00005570: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00005580: 6170 7065 6e64 2822 5969 6464 6973 6822  append("Yiddish"
+00005590: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000055a0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+000055b0: 6428 2259 6f72 7562 6122 290d 0a0d 0a20  d("Yoruba").... 
+000055c0: 2020 2020 2020 2073 656c 662e 636f 6465         self.code
+000055d0: 5f6f 665f 6e61 6d65 203d 2064 6963 7428  _of_name = dict(
+000055e0: 7a69 7028 7365 6c66 2e6c 6973 745f 6e61  zip(self.list_na
+000055f0: 6d65 732c 2073 656c 662e 6c69 7374 5f63  mes, self.list_c
+00005600: 6f64 6573 2929 0d0a 2020 2020 2020 2020  odes))..        
+00005610: 7365 6c66 2e6e 616d 655f 6f66 5f63 6f64  self.name_of_cod
+00005620: 6520 3d20 6469 6374 287a 6970 2873 656c  e = dict(zip(sel
+00005630: 662e 6c69 7374 5f63 6f64 6573 2c20 7365  f.list_codes, se
+00005640: 6c66 2e6c 6973 745f 6e61 6d65 7329 290d  lf.list_names)).
+00005650: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+00005660: 6469 6374 203d 207b 0d0a 2020 2020 2020  dict = {..      
+00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005680: 2020 2761 6627 3a20 2741 6672 696b 6161    'af': 'Afrikaa
+00005690: 6e73 272c 0d0a 2020 2020 2020 2020 2020  ns',..          
+000056a0: 2020 2020 2020 2020 2020 2020 2020 2773                's
+000056b0: 7127 3a20 2741 6c62 616e 6961 6e27 2c0d  q': 'Albanian',.
+000056c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000056d0: 2020 2020 2020 2020 2027 616d 273a 2027           'am': '
+000056e0: 416d 6861 7269 6327 2c0d 0a20 2020 2020  Amharic',..     
+000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005700: 2020 2027 6172 273a 2027 4172 6162 6963     'ar': 'Arabic
+00005710: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00005720: 2020 2020 2020 2020 2020 2020 2768 7927              'hy'
+00005730: 3a20 2741 726d 656e 6961 6e27 2c0d 0a20  : 'Armenian',.. 
+00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005750: 2020 2020 2020 2027 6173 273a 2027 4173         'as': 'As
+00005760: 7361 6d65 7365 272c 0d0a 2020 2020 2020  samese',..      
+00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005780: 2020 2761 7a27 3a20 2741 7a65 7262 6169    'az': 'Azerbai
+00005790: 6a61 6e69 272c 0d0a 2020 2020 2020 2020  jani',..        
+000057a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057b0: 2762 6127 3a20 2742 6173 686b 6972 272c  'ba': 'Bashkir',
+000057c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000057d0: 2020 2020 2020 2020 2020 2765 7527 3a20            'eu': 
+000057e0: 2742 6173 7175 6527 2c0d 0a20 2020 2020  'Basque',..     
+000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005800: 2020 2027 6265 273a 2027 4265 6c61 7275     'be': 'Belaru
+00005810: 7369 616e 272c 0d0a 2020 2020 2020 2020  sian',..        
+00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005830: 2762 6e27 3a20 2742 656e 6761 6c69 272c  'bn': 'Bengali',
+00005840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005850: 2020 2020 2020 2020 2020 2762 7327 3a20            'bs': 
+00005860: 2742 6f73 6e69 616e 272c 0d0a 2020 2020  'Bosnian',..    
+00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005880: 2020 2020 2762 7227 3a20 2742 7265 746f      'br': 'Breto
+00005890: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+000058a0: 2020 2020 2020 2020 2020 2020 2027 6267               'bg
+000058b0: 273a 2027 4275 6c67 6172 6961 6e27 2c0d  ': 'Bulgarian',.
+000058c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000058d0: 2020 2020 2020 2020 2027 6361 273a 2027           'ca': '
+000058e0: 4361 7461 6c61 6e27 2c0d 0a20 2020 2020  Catalan',..     
+000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005900: 2020 2027 7a68 273a 2027 4368 696e 6573     'zh': 'Chines
+00005910: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
+00005920: 2020 2020 2020 2020 2020 2020 2027 6872               'hr
+00005930: 273a 2027 4372 6f61 7469 616e 272c 0d0a  ': 'Croatian',..
+00005940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005950: 2020 2020 2020 2020 2763 7327 3a20 2743          'cs': 'C
+00005960: 7a65 6368 272c 0d0a 2020 2020 2020 2020  zech',..        
+00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005980: 2764 6127 3a20 2744 616e 6973 6827 2c0d  'da': 'Danish',.
+00005990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000059a0: 2020 2020 2020 2020 2027 6e6c 273a 2027           'nl': '
+000059b0: 4475 7463 6827 2c0d 0a20 2020 2020 2020  Dutch',..       
+000059c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059d0: 2027 656e 273a 2027 456e 676c 6973 6827   'en': 'English'
+000059e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000059f0: 2020 2020 2020 2020 2020 2027 6574 273a             'et':
+00005a00: 2027 4573 746f 6e69 616e 272c 0d0a 2020   'Estonian',..  
+00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a20: 2020 2020 2020 2766 6f27 3a20 2746 6172        'fo': 'Far
+00005a30: 6f65 7365 272c 0d0a 2020 2020 2020 2020  oese',..        
+00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a50: 2766 6927 3a20 2746 696e 6e69 7368 272c  'fi': 'Finnish',
+00005a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005a70: 2020 2020 2020 2020 2020 2766 7227 3a20            'fr': 
+00005a80: 2746 7265 6e63 6827 2c0d 0a20 2020 2020  'French',..     
+00005a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005aa0: 2020 2027 676c 273a 2027 4761 6c69 6369     'gl': 'Galici
+00005ab0: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
+00005ac0: 2020 2020 2020 2020 2020 2020 2020 276b                'k
+00005ad0: 6127 3a20 2747 656f 7267 6961 6e27 2c0d  a': 'Georgian',.
+00005ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005af0: 2020 2020 2020 2020 2027 6465 273a 2027           'de': '
+00005b00: 4765 726d 616e 272c 0d0a 2020 2020 2020  German',..      
+00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b20: 2020 2765 6c27 3a20 2747 7265 656b 272c    'el': 'Greek',
+00005b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005b40: 2020 2020 2020 2020 2020 2767 7527 3a20            'gu': 
+00005b50: 2747 756a 6172 6174 6927 2c0d 0a20 2020  'Gujarati',..   
+00005b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b70: 2020 2020 2027 6874 273a 2027 4861 6974       'ht': 'Hait
+00005b80: 6961 6e20 4372 656f 6c65 272c 0d0a 2020  ian Creole',..  
+00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ba0: 2020 2020 2020 2768 6127 3a20 2748 6175        'ha': 'Hau
+00005bb0: 7361 272c 0d0a 2020 2020 2020 2020 2020  sa',..          
+00005bc0: 2020 2020 2020 2020 2020 2020 2020 2768                'h
+00005bd0: 6177 273a 2027 4861 7761 6969 616e 272c  aw': 'Hawaiian',
+00005be0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005bf0: 2020 2020 2020 2020 2020 2768 6527 3a20            'he': 
+00005c00: 2748 6562 7265 7727 2c0d 0a20 2020 2020  'Hebrew',..     
+00005c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c20: 2020 2027 6869 273a 2027 4869 6e64 6927     'hi': 'Hindi'
+00005c30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005c40: 2020 2020 2020 2020 2020 2027 6875 273a             'hu':
+00005c50: 2027 4875 6e67 6172 6961 6e27 2c0d 0a20   'Hungarian',.. 
+00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c70: 2020 2020 2020 2027 6973 273a 2027 4963         'is': 'Ic
+00005c80: 656c 616e 6469 6327 2c0d 0a20 2020 2020  elandic',..     
+00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ca0: 2020 2027 6964 273a 2027 496e 646f 6e65     'id': 'Indone
+00005cb0: 7369 616e 272c 0d0a 2020 2020 2020 2020  sian',..        
+00005cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cd0: 2769 7427 3a20 2749 7461 6c69 616e 272c  'it': 'Italian',
+00005ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005cf0: 2020 2020 2020 2020 2020 276a 6127 3a20            'ja': 
+00005d00: 274a 6170 616e 6573 6527 2c0d 0a20 2020  'Japanese',..   
+00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d20: 2020 2020 2027 6a76 273a 2027 4a61 7661       'jv': 'Java
+00005d30: 6e65 7365 272c 0d0a 2020 2020 2020 2020  nese',..        
+00005d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d50: 276b 6e27 3a20 274b 616e 6e61 6461 272c  'kn': 'Kannada',
+00005d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005d70: 2020 2020 2020 2020 2020 276b 6b27 3a20            'kk': 
+00005d80: 274b 617a 616b 6827 2c0d 0a20 2020 2020  'Kazakh',..     
+00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005da0: 2020 2027 6b6d 273a 2027 4b68 6d65 7227     'km': 'Khmer'
+00005db0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005dc0: 2020 2020 2020 2020 2020 2027 6b6f 273a             'ko':
+00005dd0: 2027 4b6f 7265 616e 272c 0d0a 2020 2020   'Korean',..    
+00005de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005df0: 2020 2020 276c 6f27 3a20 274c 616f 272c      'lo': 'Lao',
+00005e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005e10: 2020 2020 2020 2020 2020 276c 6127 3a20            'la': 
+00005e20: 274c 6174 696e 272c 0d0a 2020 2020 2020  'Latin',..      
+00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e40: 2020 276c 7627 3a20 274c 6174 7669 616e    'lv': 'Latvian
+00005e50: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00005e60: 2020 2020 2020 2020 2020 2020 276c 6e27              'ln'
+00005e70: 3a20 274c 696e 6761 6c61 272c 0d0a 2020  : 'Lingala',..  
 00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e90: 2027 6d67 273a 2027 4d61 6c61 6761 7379   'mg': 'Malagasy
-00005ea0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005eb0: 2020 2020 2020 2020 2020 2020 276d 7327              'ms'
-00005ec0: 3a20 274d 616c 6179 272c 0d0a 2020 2020  : 'Malay',..    
-00005ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ee0: 2020 2020 276d 6c27 3a20 274d 616c 6179      'ml': 'Malay
-00005ef0: 616c 616d 272c 0d0a 2020 2020 2020 2020  alam',..        
-00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f10: 276d 7427 3a20 274d 616c 7465 7365 272c  'mt': 'Maltese',
-00005f20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005f30: 2020 2020 2020 2020 2020 276d 6927 3a20            'mi': 
-00005f40: 274d 616f 7269 272c 0d0a 2020 2020 2020  'Maori',..      
-00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f60: 2020 276d 7227 3a20 274d 6172 6174 6869    'mr': 'Marathi
-00005f70: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005f80: 2020 2020 2020 2020 2020 2020 276d 6e27              'mn'
-00005f90: 3a20 274d 6f6e 676f 6c69 616e 272c 0d0a  : 'Mongolian',..
-00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fb0: 2020 2020 2020 2020 276d 7927 3a20 274d          'my': 'M
-00005fc0: 7961 6e6d 6172 2028 4275 726d 6573 6529  yanmar (Burmese)
-00005fd0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005fe0: 2020 2020 2020 2020 2020 2020 276e 6527              'ne'
-00005ff0: 3a20 274e 6570 616c 6927 2c0d 0a20 2020  : 'Nepali',..   
-00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006010: 2020 2020 2027 6e6f 273a 2027 4e6f 7277       'no': 'Norw
-00006020: 6567 6961 6e27 2c0d 0a20 2020 2020 2020  egian',..       
+00005e90: 2020 2020 2020 276c 7427 3a20 274c 6974        'lt': 'Lit
+00005ea0: 6875 616e 6961 6e27 2c0d 0a20 2020 2020  huanian',..     
+00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ec0: 2020 2027 6c62 273a 2027 4c75 7865 6d62     'lb': 'Luxemb
+00005ed0: 6f75 7267 6973 6827 2c0d 0a20 2020 2020  ourgish',..     
+00005ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ef0: 2020 2027 6d6b 273a 2027 4d61 6365 646f     'mk': 'Macedo
+00005f00: 6e69 616e 272c 0d0a 2020 2020 2020 2020  nian',..        
+00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f20: 276d 6727 3a20 274d 616c 6167 6173 7927  'mg': 'Malagasy'
+00005f30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005f40: 2020 2020 2020 2020 2020 2027 6d73 273a             'ms':
+00005f50: 2027 4d61 6c61 7927 2c0d 0a20 2020 2020   'Malay',..     
+00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f70: 2020 2027 6d6c 273a 2027 4d61 6c61 7961     'ml': 'Malaya
+00005f80: 6c61 6d27 2c0d 0a20 2020 2020 2020 2020  lam',..         
+00005f90: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00005fa0: 6d74 273a 2027 4d61 6c74 6573 6527 2c0d  mt': 'Maltese',.
+00005fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005fc0: 2020 2020 2020 2020 2027 6d69 273a 2027           'mi': '
+00005fd0: 4d61 6f72 6927 2c0d 0a20 2020 2020 2020  Maori',..       
+00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ff0: 2027 6d72 273a 2027 4d61 7261 7468 6927   'mr': 'Marathi'
+00006000: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00006010: 2020 2020 2020 2020 2020 2027 6d6e 273a             'mn':
+00006020: 2027 4d6f 6e67 6f6c 6961 6e27 2c0d 0a20   'Mongolian',.. 
 00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006040: 2027 6e6e 273a 2027 4e79 6e6f 7273 6b27   'nn': 'Nynorsk'
-00006050: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00006060: 2020 2020 2020 2020 2020 2027 6f63 273a             'oc':
-00006070: 2027 4f63 6369 7461 6e27 2c0d 0a20 2020   'Occitan',..   
-00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006090: 2020 2020 2027 7073 273a 2027 5061 7368       'ps': 'Pash
-000060a0: 746f 272c 0d0a 2020 2020 2020 2020 2020  to',..          
-000060b0: 2020 2020 2020 2020 2020 2020 2020 2766                'f
-000060c0: 6127 3a20 2750 6572 7369 616e 272c 0d0a  a': 'Persian',..
-000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060e0: 2020 2020 2020 2020 2770 6c27 3a20 2750          'pl': 'P
-000060f0: 6f6c 6973 6827 2c0d 0a20 2020 2020 2020  olish',..       
-00006100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006110: 2027 7074 273a 2027 506f 7274 7567 7565   'pt': 'Portugue
-00006120: 7365 272c 0d0a 2020 2020 2020 2020 2020  se',..          
-00006130: 2020 2020 2020 2020 2020 2020 2020 2770                'p
-00006140: 6127 3a20 2750 756e 6a61 6269 272c 0d0a  a': 'Punjabi',..
-00006150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006160: 2020 2020 2020 2020 2772 6f27 3a20 2752          'ro': 'R
-00006170: 6f6d 616e 6961 6e27 2c0d 0a20 2020 2020  omanian',..     
-00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006190: 2020 2027 7275 273a 2027 5275 7373 6961     'ru': 'Russia
-000061a0: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
-000061b0: 2020 2020 2020 2020 2020 2020 2027 7361               'sa
-000061c0: 273a 2027 5361 6e73 6b72 6974 272c 0d0a  ': 'Sanskrit',..
-000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061e0: 2020 2020 2020 2020 2773 7227 3a20 2753          'sr': 'S
-000061f0: 6572 6269 616e 272c 0d0a 2020 2020 2020  erbian',..      
-00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006210: 2020 2773 6e27 3a20 2753 686f 6e61 272c    'sn': 'Shona',
-00006220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006230: 2020 2020 2020 2020 2020 2773 6427 3a20            'sd': 
-00006240: 2753 696e 6468 6927 2c0d 0a20 2020 2020  'Sindhi',..     
-00006250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006260: 2020 2027 7369 273a 2027 5369 6e68 616c     'si': 'Sinhal
-00006270: 6127 2c0d 0a20 2020 2020 2020 2020 2020  a',..           
-00006280: 2020 2020 2020 2020 2020 2020 2027 736b               'sk
-00006290: 273a 2027 536c 6f76 616b 272c 0d0a 2020  ': 'Slovak',..  
-000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062b0: 2020 2020 2020 2773 6c27 3a20 2753 6c6f        'sl': 'Slo
-000062c0: 7665 6e69 616e 272c 0d0a 2020 2020 2020  venian',..      
-000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062e0: 2020 2773 6f27 3a20 2753 6f6d 616c 6927    'so': 'Somali'
-000062f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00006300: 2020 2020 2020 2020 2020 2027 6573 273a             'es':
-00006310: 2027 5370 616e 6973 6827 2c0d 0a20 2020   'Spanish',..   
-00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006330: 2020 2020 2027 7375 273a 2027 5375 6e64       'su': 'Sund
-00006340: 616e 6573 6527 2c0d 0a20 2020 2020 2020  anese',..       
-00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006360: 2027 7377 273a 2027 5377 6168 696c 6927   'sw': 'Swahili'
-00006370: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00006380: 2020 2020 2020 2020 2020 2027 7376 273a             'sv':
-00006390: 2027 5377 6564 6973 6827 2c0d 0a20 2020   'Swedish',..   
-000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063b0: 2020 2020 2027 746c 273a 2027 5461 6761       'tl': 'Taga
-000063c0: 6c6f 6727 2c0d 0a20 2020 2020 2020 2020  log',..         
-000063d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000063e0: 7467 273a 2027 5461 6a69 6b27 2c0d 0a20  tg': 'Tajik',.. 
-000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006400: 2020 2020 2020 2027 7461 273a 2027 5461         'ta': 'Ta
-00006410: 6d69 6c27 2c0d 0a20 2020 2020 2020 2020  mil',..         
-00006420: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00006430: 7474 273a 2027 5461 7461 7227 2c0d 0a20  tt': 'Tatar',.. 
-00006440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006450: 2020 2020 2020 2027 7465 273a 2027 5465         'te': 'Te
-00006460: 6c75 6775 272c 0d0a 2020 2020 2020 2020  lugu',..        
-00006470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006480: 2774 6827 3a20 2754 6861 6927 2c0d 0a20  'th': 'Thai',.. 
-00006490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064a0: 2020 2020 2020 2027 626f 273a 2027 5469         'bo': 'Ti
-000064b0: 6265 7461 6e27 2c0d 0a20 2020 2020 2020  betan',..       
-000064c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064d0: 2027 7472 273a 2027 5475 726b 6973 6827   'tr': 'Turkish'
-000064e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000064f0: 2020 2020 2020 2020 2020 2027 746b 273a             'tk':
-00006500: 2027 5475 726b 6d65 6e27 2c0d 0a20 2020   'Turkmen',..   
-00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006520: 2020 2020 2027 756b 273a 2027 556b 7261       'uk': 'Ukra
-00006530: 696e 6961 6e27 2c0d 0a20 2020 2020 2020  inian',..       
-00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006550: 2027 7572 273a 2027 5572 6475 272c 0d0a   'ur': 'Urdu',..
-00006560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006570: 2020 2020 2020 2020 2775 7a27 3a20 2755          'uz': 'U
-00006580: 7a62 656b 272c 0d0a 2020 2020 2020 2020  zbek',..        
-00006590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065a0: 2776 6927 3a20 2756 6965 746e 616d 6573  'vi': 'Vietnames
-000065b0: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
-000065c0: 2020 2020 2020 2020 2020 2020 2027 6379               'cy
-000065d0: 273a 2027 5765 6c73 6827 2c0d 0a20 2020  ': 'Welsh',..   
-000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065f0: 2020 2020 2027 7969 273a 2027 5969 6464       'yi': 'Yidd
-00006600: 6973 6827 2c0d 0a20 2020 2020 2020 2020  ish',..         
-00006610: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00006620: 796f 273a 2027 596f 7275 6261 272c 0d0a  yo': 'Yoruba',..
-00006630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006640: 2020 2020 7d0d 0a0d 0a20 2020 2064 6566      }....    def
-00006650: 2067 6574 5f6e 616d 6528 7365 6c66 2c20   get_name(self, 
-00006660: 6765 745f 636f 6465 293a 0d0a 2020 2020  get_code):..    
-00006670: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00006680: 6469 6374 2e67 6574 2867 6574 5f63 6f64  dict.get(get_cod
-00006690: 652e 6c6f 7765 7228 292c 2022 2229 0d0a  e.lower(), "")..
-000066a0: 0d0a 2020 2020 6465 6620 6765 745f 636f  ..    def get_co
-000066b0: 6465 2873 656c 662c 206c 616e 6775 6167  de(self, languag
-000066c0: 6529 3a0d 0a20 2020 2020 2020 2066 6f72  e):..        for
-000066d0: 2067 6574 5f63 6f64 652c 206c 616e 6720   get_code, lang 
-000066e0: 696e 2073 656c 662e 6469 6374 2e69 7465  in self.dict.ite
-000066f0: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-00006700: 2020 2069 6620 6c61 6e67 2e6c 6f77 6572     if lang.lower
-00006710: 2829 203d 3d20 6c61 6e67 7561 6765 2e6c  () == language.l
-00006720: 6f77 6572 2829 3a0d 0a20 2020 2020 2020  ower():..       
-00006730: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00006740: 6765 745f 636f 6465 0d0a 2020 2020 2020  get_code..      
-00006750: 2020 7265 7475 726e 2022 220d 0a0d 0a0d    return "".....
-00006760: 0a63 6c61 7373 2047 6f6f 676c 654c 616e  .class GoogleLan
-00006770: 6775 6167 653a 0d0a 2020 2020 6465 6620  guage:..    def 
-00006780: 5f5f 696e 6974 5f5f 2873 656c 6629 3a0d  __init__(self):.
-00006790: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000067a0: 7374 5f63 6f64 6573 203d 205b 5d0d 0a20  st_codes = [].. 
-000067b0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000067c0: 5f63 6f64 6573 2e61 7070 656e 6428 2261  _codes.append("a
-000067d0: 6622 290d 0a20 2020 2020 2020 2073 656c  f")..        sel
-000067e0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-000067f0: 656e 6428 2273 7122 290d 0a20 2020 2020  end("sq")..     
-00006800: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00006810: 6573 2e61 7070 656e 6428 2261 6d22 290d  es.append("am").
-00006820: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00006830: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00006840: 2261 7222 290d 0a20 2020 2020 2020 2073  "ar")..        s
-00006850: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00006860: 7070 656e 6428 2268 7922 290d 0a20 2020  ppend("hy")..   
-00006870: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00006880: 6f64 6573 2e61 7070 656e 6428 2261 7322  odes.append("as"
-00006890: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000068a0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-000068b0: 6428 2261 7922 290d 0a20 2020 2020 2020  d("ay")..       
-000068c0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-000068d0: 2e61 7070 656e 6428 2261 7a22 290d 0a20  .append("az").. 
-000068e0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000068f0: 5f63 6f64 6573 2e61 7070 656e 6428 2262  _codes.append("b
-00006900: 6d22 290d 0a20 2020 2020 2020 2073 656c  m")..        sel
-00006910: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00006920: 656e 6428 2265 7522 290d 0a20 2020 2020  end("eu")..     
-00006930: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00006940: 6573 2e61 7070 656e 6428 2262 6522 290d  es.append("be").
-00006950: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00006960: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00006970: 2262 6e22 290d 0a20 2020 2020 2020 2073  "bn")..        s
-00006980: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00006990: 7070 656e 6428 2262 686f 2229 0d0a 2020  ppend("bho")..  
-000069a0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000069b0: 636f 6465 732e 6170 7065 6e64 2822 6273  codes.append("bs
-000069c0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000069d0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-000069e0: 6e64 2822 6267 2229 0d0a 2020 2020 2020  nd("bg")..      
-000069f0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00006a00: 732e 6170 7065 6e64 2822 6361 2229 0d0a  s.append("ca")..
-00006a10: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00006a20: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00006a30: 6365 6222 290d 0a20 2020 2020 2020 2073  ceb")..        s
-00006a40: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00006a50: 7070 656e 6428 226e 7922 290d 0a20 2020  ppend("ny")..   
-00006a60: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00006a70: 6f64 6573 2e61 7070 656e 6428 227a 682d  odes.append("zh-
-00006a80: 434e 2229 0d0a 2020 2020 2020 2020 7365  CN")..        se
-00006a90: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00006aa0: 7065 6e64 2822 7a68 2d54 5722 290d 0a20  pend("zh-TW").. 
-00006ab0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00006ac0: 5f63 6f64 6573 2e61 7070 656e 6428 2263  _codes.append("c
-00006ad0: 6f22 290d 0a20 2020 2020 2020 2073 656c  o")..        sel
-00006ae0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00006af0: 656e 6428 2268 7222 290d 0a20 2020 2020  end("hr")..     
-00006b00: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00006b10: 6573 2e61 7070 656e 6428 2263 7322 290d  es.append("cs").
-00006b20: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00006b30: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00006b40: 2264 6122 290d 0a20 2020 2020 2020 2073  "da")..        s
-00006b50: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00006b60: 7070 656e 6428 2264 7622 290d 0a20 2020  ppend("dv")..   
-00006b70: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00006b80: 6f64 6573 2e61 7070 656e 6428 2264 6f69  odes.append("doi
-00006b90: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00006ba0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00006bb0: 6e64 2822 6e6c 2229 0d0a 2020 2020 2020  nd("nl")..      
-00006bc0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00006bd0: 732e 6170 7065 6e64 2822 656e 2229 0d0a  s.append("en")..
-00006be0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00006bf0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00006c00: 656f 2229 0d0a 2020 2020 2020 2020 7365  eo")..        se
-00006c10: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00006c20: 7065 6e64 2822 6574 2229 0d0a 2020 2020  pend("et")..    
-00006c30: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00006c40: 6465 732e 6170 7065 6e64 2822 6565 2229  des.append("ee")
-00006c50: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00006c60: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00006c70: 2822 6669 6c22 290d 0a20 2020 2020 2020  ("fil")..       
-00006c80: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00006c90: 2e61 7070 656e 6428 2266 6922 290d 0a20  .append("fi").. 
-00006ca0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00006cb0: 5f63 6f64 6573 2e61 7070 656e 6428 2266  _codes.append("f
-00006cc0: 7222 290d 0a20 2020 2020 2020 2073 656c  r")..        sel
-00006cd0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00006ce0: 656e 6428 2266 7922 290d 0a20 2020 2020  end("fy")..     
-00006cf0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00006d00: 6573 2e61 7070 656e 6428 2267 6c22 290d  es.append("gl").
-00006d10: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00006d20: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00006d30: 226b 6122 290d 0a20 2020 2020 2020 2073  "ka")..        s
-00006d40: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00006d50: 7070 656e 6428 2264 6522 290d 0a20 2020  ppend("de")..   
-00006d60: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00006d70: 6f64 6573 2e61 7070 656e 6428 2265 6c22  odes.append("el"
-00006d80: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00006d90: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00006da0: 6428 2267 6e22 290d 0a20 2020 2020 2020  d("gn")..       
-00006db0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00006dc0: 2e61 7070 656e 6428 2267 7522 290d 0a20  .append("gu").. 
-00006dd0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00006de0: 5f63 6f64 6573 2e61 7070 656e 6428 2268  _codes.append("h
-00006df0: 7422 290d 0a20 2020 2020 2020 2073 656c  t")..        sel
-00006e00: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00006e10: 656e 6428 2268 6122 290d 0a20 2020 2020  end("ha")..     
-00006e20: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00006e30: 6573 2e61 7070 656e 6428 2268 6177 2229  es.append("haw")
-00006e40: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00006e50: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00006e60: 2822 6865 2229 0d0a 2020 2020 2020 2020  ("he")..        
-00006e70: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00006e80: 6170 7065 6e64 2822 6869 2229 0d0a 2020  append("hi")..  
-00006e90: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00006ea0: 636f 6465 732e 6170 7065 6e64 2822 686d  codes.append("hm
-00006eb0: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-00006ec0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00006ed0: 656e 6428 2268 7522 290d 0a20 2020 2020  end("hu")..     
-00006ee0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00006ef0: 6573 2e61 7070 656e 6428 2269 7322 290d  es.append("is").
-00006f00: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00006f10: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00006f20: 2269 6722 290d 0a20 2020 2020 2020 2073  "ig")..        s
-00006f30: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00006f40: 7070 656e 6428 2269 6c6f 2229 0d0a 2020  ppend("ilo")..  
-00006f50: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00006f60: 636f 6465 732e 6170 7065 6e64 2822 6964  codes.append("id
-00006f70: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00006f80: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00006f90: 6e64 2822 6761 2229 0d0a 2020 2020 2020  nd("ga")..      
-00006fa0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00006fb0: 732e 6170 7065 6e64 2822 6974 2229 0d0a  s.append("it")..
-00006fc0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00006fd0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00006fe0: 6a61 2229 0d0a 2020 2020 2020 2020 7365  ja")..        se
-00006ff0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00007000: 7065 6e64 2822 6a76 2229 0d0a 2020 2020  pend("jv")..    
-00007010: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00007020: 6465 732e 6170 7065 6e64 2822 6b6e 2229  des.append("kn")
-00007030: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007040: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00007050: 2822 6b6b 2229 0d0a 2020 2020 2020 2020  ("kk")..        
-00007060: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00007070: 6170 7065 6e64 2822 6b6d 2229 0d0a 2020  append("km")..  
-00007080: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007090: 636f 6465 732e 6170 7065 6e64 2822 7277  codes.append("rw
-000070a0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000070b0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-000070c0: 6e64 2822 676f 6d22 290d 0a20 2020 2020  nd("gom")..     
-000070d0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-000070e0: 6573 2e61 7070 656e 6428 226b 6f22 290d  es.append("ko").
-000070f0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00007100: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00007110: 226b 7269 2229 0d0a 2020 2020 2020 2020  "kri")..        
-00007120: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00007130: 6170 7065 6e64 2822 6b6d 7222 290d 0a20  append("kmr").. 
-00007140: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007150: 5f63 6f64 6573 2e61 7070 656e 6428 2263  _codes.append("c
-00007160: 6b62 2229 0d0a 2020 2020 2020 2020 7365  kb")..        se
-00007170: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00007180: 7065 6e64 2822 6b79 2229 0d0a 2020 2020  pend("ky")..    
-00007190: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000071a0: 6465 732e 6170 7065 6e64 2822 6c6f 2229  des.append("lo")
-000071b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000071c0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-000071d0: 2822 6c61 2229 0d0a 2020 2020 2020 2020  ("la")..        
-000071e0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-000071f0: 6170 7065 6e64 2822 6c76 2229 0d0a 2020  append("lv")..  
-00007200: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007210: 636f 6465 732e 6170 7065 6e64 2822 6c6e  codes.append("ln
-00007220: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007230: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00007240: 6e64 2822 6c74 2229 0d0a 2020 2020 2020  nd("lt")..      
-00007250: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00007260: 732e 6170 7065 6e64 2822 6c67 2229 0d0a  s.append("lg")..
-00007270: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007280: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00007290: 6c62 2229 0d0a 2020 2020 2020 2020 7365  lb")..        se
-000072a0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-000072b0: 7065 6e64 2822 6d6b 2229 0d0a 2020 2020  pend("mk")..    
-000072c0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000072d0: 6465 732e 6170 7065 6e64 2822 6d67 2229  des.append("mg")
-000072e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000072f0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00007300: 2822 6d73 2229 0d0a 2020 2020 2020 2020  ("ms")..        
-00007310: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00007320: 6170 7065 6e64 2822 6d6c 2229 0d0a 2020  append("ml")..  
-00007330: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007340: 636f 6465 732e 6170 7065 6e64 2822 6d74  codes.append("mt
-00007350: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007360: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00007370: 6e64 2822 6d69 2229 0d0a 2020 2020 2020  nd("mi")..      
-00007380: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00007390: 732e 6170 7065 6e64 2822 6d72 2229 0d0a  s.append("mr")..
-000073a0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000073b0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-000073c0: 6d6e 692d 4d74 6569 2229 0d0a 2020 2020  mni-Mtei")..    
-000073d0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000073e0: 6465 732e 6170 7065 6e64 2822 6c75 7322  des.append("lus"
-000073f0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007400: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00007410: 6428 226d 6e22 290d 0a20 2020 2020 2020  d("mn")..       
-00007420: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00007430: 2e61 7070 656e 6428 226d 7922 290d 0a20  .append("my").. 
-00007440: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007450: 5f63 6f64 6573 2e61 7070 656e 6428 226e  _codes.append("n
-00007460: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
-00007470: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00007480: 656e 6428 226e 6f22 290d 0a20 2020 2020  end("no")..     
-00007490: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-000074a0: 6573 2e61 7070 656e 6428 226f 7222 290d  es.append("or").
-000074b0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000074c0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-000074d0: 226f 6d22 290d 0a20 2020 2020 2020 2073  "om")..        s
-000074e0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-000074f0: 7070 656e 6428 2270 7322 290d 0a20 2020  ppend("ps")..   
-00007500: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00007510: 6f64 6573 2e61 7070 656e 6428 2266 6122  odes.append("fa"
-00007520: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007530: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00007540: 6428 2270 6c22 290d 0a20 2020 2020 2020  d("pl")..       
-00007550: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00007560: 2e61 7070 656e 6428 2270 7422 290d 0a20  .append("pt").. 
-00007570: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007580: 5f63 6f64 6573 2e61 7070 656e 6428 2270  _codes.append("p
-00007590: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
-000075a0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-000075b0: 656e 6428 2271 7522 290d 0a20 2020 2020  end("qu")..     
-000075c0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-000075d0: 6573 2e61 7070 656e 6428 2272 6f22 290d  es.append("ro").
-000075e0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000075f0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00007600: 2272 7522 290d 0a20 2020 2020 2020 2073  "ru")..        s
-00007610: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00007620: 7070 656e 6428 2273 6d22 290d 0a20 2020  ppend("sm")..   
-00007630: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00007640: 6f64 6573 2e61 7070 656e 6428 2273 6122  odes.append("sa"
-00007650: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007660: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00007670: 6428 2267 6422 290d 0a20 2020 2020 2020  d("gd")..       
-00007680: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00007690: 2e61 7070 656e 6428 226e 736f 2229 0d0a  .append("nso")..
-000076a0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000076b0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-000076c0: 7372 2229 0d0a 2020 2020 2020 2020 7365  sr")..        se
-000076d0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-000076e0: 7065 6e64 2822 7374 2229 0d0a 2020 2020  pend("st")..    
-000076f0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00007700: 6465 732e 6170 7065 6e64 2822 736e 2229  des.append("sn")
-00007710: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007720: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00007730: 2822 7364 2229 0d0a 2020 2020 2020 2020  ("sd")..        
-00007740: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00007750: 6170 7065 6e64 2822 7369 2229 0d0a 2020  append("si")..  
-00007760: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007770: 636f 6465 732e 6170 7065 6e64 2822 736b  codes.append("sk
-00007780: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007790: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-000077a0: 6e64 2822 736c 2229 0d0a 2020 2020 2020  nd("sl")..      
-000077b0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-000077c0: 732e 6170 7065 6e64 2822 736f 2229 0d0a  s.append("so")..
-000077d0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000077e0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-000077f0: 6573 2229 0d0a 2020 2020 2020 2020 7365  es")..        se
-00007800: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00007810: 7065 6e64 2822 7375 2229 0d0a 2020 2020  pend("su")..    
-00007820: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00007830: 6465 732e 6170 7065 6e64 2822 7377 2229  des.append("sw")
-00007840: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007850: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00007860: 2822 7376 2229 0d0a 2020 2020 2020 2020  ("sv")..        
-00007870: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00007880: 6170 7065 6e64 2822 7467 2229 0d0a 2020  append("tg")..  
-00007890: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000078a0: 636f 6465 732e 6170 7065 6e64 2822 7461  codes.append("ta
-000078b0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000078c0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-000078d0: 6e64 2822 7474 2229 0d0a 2020 2020 2020  nd("tt")..      
-000078e0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-000078f0: 732e 6170 7065 6e64 2822 7465 2229 0d0a  s.append("te")..
-00007900: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007910: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00007920: 7468 2229 0d0a 2020 2020 2020 2020 7365  th")..        se
-00007930: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00007940: 7065 6e64 2822 7469 2229 0d0a 2020 2020  pend("ti")..    
-00007950: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00007960: 6465 732e 6170 7065 6e64 2822 7473 2229  des.append("ts")
-00007970: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007980: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00007990: 2822 7472 2229 0d0a 2020 2020 2020 2020  ("tr")..        
-000079a0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-000079b0: 6170 7065 6e64 2822 746b 2229 0d0a 2020  append("tk")..  
-000079c0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000079d0: 636f 6465 732e 6170 7065 6e64 2822 7477  codes.append("tw
-000079e0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000079f0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00007a00: 6e64 2822 756b 2229 0d0a 2020 2020 2020  nd("uk")..      
-00007a10: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00007a20: 732e 6170 7065 6e64 2822 7572 2229 0d0a  s.append("ur")..
-00007a30: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007a40: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00007a50: 7567 2229 0d0a 2020 2020 2020 2020 7365  ug")..        se
-00007a60: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00007a70: 7065 6e64 2822 757a 2229 0d0a 2020 2020  pend("uz")..    
-00007a80: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00007a90: 6465 732e 6170 7065 6e64 2822 7669 2229  des.append("vi")
-00007aa0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007ab0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00007ac0: 2822 6379 2229 0d0a 2020 2020 2020 2020  ("cy")..        
-00007ad0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00007ae0: 6170 7065 6e64 2822 7868 2229 0d0a 2020  append("xh")..  
-00007af0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007b00: 636f 6465 732e 6170 7065 6e64 2822 7969  codes.append("yi
-00007b10: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007b20: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00007b30: 6e64 2822 796f 2229 0d0a 2020 2020 2020  nd("yo")..      
-00007b40: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00007b50: 732e 6170 7065 6e64 2822 7a75 2229 0d0a  s.append("zu")..
-00007b60: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007b70: 6973 745f 6e61 6d65 7320 3d20 5b5d 0d0a  ist_names = []..
-00007b80: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007b90: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00007ba0: 4166 7269 6b61 616e 7322 290d 0a20 2020  Afrikaans")..   
-00007bb0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00007bc0: 616d 6573 2e61 7070 656e 6428 2241 6c62  ames.append("Alb
-00007bd0: 616e 6961 6e22 290d 0a20 2020 2020 2020  anian")..       
-00007be0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00007bf0: 2e61 7070 656e 6428 2241 6d68 6172 6963  .append("Amharic
-00007c00: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007c10: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00007c20: 6e64 2822 4172 6162 6963 2229 0d0a 2020  nd("Arabic")..  
-00007c30: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007c40: 6e61 6d65 732e 6170 7065 6e64 2822 4172  names.append("Ar
-00007c50: 6d65 6e69 616e 2229 0d0a 2020 2020 2020  menian")..      
-00007c60: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00007c70: 732e 6170 7065 6e64 2822 4173 7361 6d65  s.append("Assame
-00007c80: 7365 2229 0d0a 2020 2020 2020 2020 7365  se")..        se
-00007c90: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00007ca0: 7065 6e64 2822 4179 6d61 7261 2229 0d0a  pend("Aymara")..
-00007cb0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007cc0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00007cd0: 417a 6572 6261 696a 616e 6922 290d 0a20  Azerbaijani").. 
-00007ce0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007cf0: 5f6e 616d 6573 2e61 7070 656e 6428 2242  _names.append("B
-00007d00: 616d 6261 7261 2229 0d0a 2020 2020 2020  ambara")..      
-00007d10: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00007d20: 732e 6170 7065 6e64 2822 4261 7371 7565  s.append("Basque
-00007d30: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007d40: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00007d50: 6e64 2822 4265 6c61 7275 7369 616e 2229  nd("Belarusian")
-00007d60: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007d70: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00007d80: 2822 4265 6e67 616c 6922 290d 0a20 2020  ("Bengali")..   
-00007d90: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00007da0: 616d 6573 2e61 7070 656e 6428 2242 686f  ames.append("Bho
-00007db0: 6a70 7572 6922 290d 0a20 2020 2020 2020  jpuri")..       
-00007dc0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00007dd0: 2e61 7070 656e 6428 2242 6f73 6e69 616e  .append("Bosnian
-00007de0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007df0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00007e00: 6e64 2822 4275 6c67 6172 6961 6e22 290d  nd("Bulgarian").
-00007e10: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00007e20: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00007e30: 2243 6174 616c 616e 2229 0d0a 2020 2020  "Catalan")..    
-00007e40: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00007e50: 6d65 732e 6170 7065 6e64 2822 4365 6275  mes.append("Cebu
-00007e60: 616e 6f22 290d 0a20 2020 2020 2020 2073  ano")..        s
-00007e70: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00007e80: 7070 656e 6428 2243 6869 6368 6577 6122  ppend("Chichewa"
-00007e90: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007ea0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00007eb0: 6428 2243 6869 6e65 7365 2028 5369 6d70  d("Chinese (Simp
-00007ec0: 6c69 6669 6564 2922 290d 0a20 2020 2020  lified)")..     
+00006040: 2020 2020 2020 2027 6d79 273a 2027 4d79         'my': 'My
+00006050: 616e 6d61 7220 2842 7572 6d65 7365 2927  anmar (Burmese)'
+00006060: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00006070: 2020 2020 2020 2020 2020 2027 6e65 273a             'ne':
+00006080: 2027 4e65 7061 6c69 272c 0d0a 2020 2020   'Nepali',..    
+00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060a0: 2020 2020 276e 6f27 3a20 274e 6f72 7765      'no': 'Norwe
+000060b0: 6769 616e 272c 0d0a 2020 2020 2020 2020  gian',..        
+000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060d0: 276e 6e27 3a20 274e 796e 6f72 736b 272c  'nn': 'Nynorsk',
+000060e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000060f0: 2020 2020 2020 2020 2020 276f 6327 3a20            'oc': 
+00006100: 274f 6363 6974 616e 272c 0d0a 2020 2020  'Occitan',..    
+00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006120: 2020 2020 2770 7327 3a20 2750 6173 6874      'ps': 'Pasht
+00006130: 6f27 2c0d 0a20 2020 2020 2020 2020 2020  o',..           
+00006140: 2020 2020 2020 2020 2020 2020 2027 6661               'fa
+00006150: 273a 2027 5065 7273 6961 6e27 2c0d 0a20  ': 'Persian',.. 
+00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006170: 2020 2020 2020 2027 706c 273a 2027 506f         'pl': 'Po
+00006180: 6c69 7368 272c 0d0a 2020 2020 2020 2020  lish',..        
+00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061a0: 2770 7427 3a20 2750 6f72 7475 6775 6573  'pt': 'Portugues
+000061b0: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
+000061c0: 2020 2020 2020 2020 2020 2020 2027 7061               'pa
+000061d0: 273a 2027 5075 6e6a 6162 6927 2c0d 0a20  ': 'Punjabi',.. 
+000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061f0: 2020 2020 2020 2027 726f 273a 2027 526f         'ro': 'Ro
+00006200: 6d61 6e69 616e 272c 0d0a 2020 2020 2020  manian',..      
+00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006220: 2020 2772 7527 3a20 2752 7573 7369 616e    'ru': 'Russian
+00006230: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00006240: 2020 2020 2020 2020 2020 2020 2773 6127              'sa'
+00006250: 3a20 2753 616e 736b 7269 7427 2c0d 0a20  : 'Sanskrit',.. 
+00006260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006270: 2020 2020 2020 2027 7372 273a 2027 5365         'sr': 'Se
+00006280: 7262 6961 6e27 2c0d 0a20 2020 2020 2020  rbian',..       
+00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062a0: 2027 736e 273a 2027 5368 6f6e 6127 2c0d   'sn': 'Shona',.
+000062b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000062c0: 2020 2020 2020 2020 2027 7364 273a 2027           'sd': '
+000062d0: 5369 6e64 6869 272c 0d0a 2020 2020 2020  Sindhi',..      
+000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062f0: 2020 2773 6927 3a20 2753 696e 6861 6c61    'si': 'Sinhala
+00006300: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00006310: 2020 2020 2020 2020 2020 2020 2773 6b27              'sk'
+00006320: 3a20 2753 6c6f 7661 6b27 2c0d 0a20 2020  : 'Slovak',..   
+00006330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006340: 2020 2020 2027 736c 273a 2027 536c 6f76       'sl': 'Slov
+00006350: 656e 6961 6e27 2c0d 0a20 2020 2020 2020  enian',..       
+00006360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006370: 2027 736f 273a 2027 536f 6d61 6c69 272c   'so': 'Somali',
+00006380: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006390: 2020 2020 2020 2020 2020 2765 7327 3a20            'es': 
+000063a0: 2753 7061 6e69 7368 272c 0d0a 2020 2020  'Spanish',..    
+000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063c0: 2020 2020 2773 7527 3a20 2753 756e 6461      'su': 'Sunda
+000063d0: 6e65 7365 272c 0d0a 2020 2020 2020 2020  nese',..        
+000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063f0: 2773 7727 3a20 2753 7761 6869 6c69 272c  'sw': 'Swahili',
+00006400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006410: 2020 2020 2020 2020 2020 2773 7627 3a20            'sv': 
+00006420: 2753 7765 6469 7368 272c 0d0a 2020 2020  'Swedish',..    
+00006430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006440: 2020 2020 2774 6c27 3a20 2754 6167 616c      'tl': 'Tagal
+00006450: 6f67 272c 0d0a 2020 2020 2020 2020 2020  og',..          
+00006460: 2020 2020 2020 2020 2020 2020 2020 2774                't
+00006470: 6727 3a20 2754 616a 696b 272c 0d0a 2020  g': 'Tajik',..  
+00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006490: 2020 2020 2020 2774 6127 3a20 2754 616d        'ta': 'Tam
+000064a0: 696c 272c 0d0a 2020 2020 2020 2020 2020  il',..          
+000064b0: 2020 2020 2020 2020 2020 2020 2020 2774                't
+000064c0: 7427 3a20 2754 6174 6172 272c 0d0a 2020  t': 'Tatar',..  
+000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064e0: 2020 2020 2020 2774 6527 3a20 2754 656c        'te': 'Tel
+000064f0: 7567 7527 2c0d 0a20 2020 2020 2020 2020  ugu',..         
+00006500: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00006510: 7468 273a 2027 5468 6169 272c 0d0a 2020  th': 'Thai',..  
+00006520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006530: 2020 2020 2020 2762 6f27 3a20 2754 6962        'bo': 'Tib
+00006540: 6574 616e 272c 0d0a 2020 2020 2020 2020  etan',..        
+00006550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006560: 2774 7227 3a20 2754 7572 6b69 7368 272c  'tr': 'Turkish',
+00006570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006580: 2020 2020 2020 2020 2020 2774 6b27 3a20            'tk': 
+00006590: 2754 7572 6b6d 656e 272c 0d0a 2020 2020  'Turkmen',..    
+000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065b0: 2020 2020 2775 6b27 3a20 2755 6b72 6169      'uk': 'Ukrai
+000065c0: 6e69 616e 272c 0d0a 2020 2020 2020 2020  nian',..        
+000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065e0: 2775 7227 3a20 2755 7264 7527 2c0d 0a20  'ur': 'Urdu',.. 
+000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006600: 2020 2020 2020 2027 757a 273a 2027 557a         'uz': 'Uz
+00006610: 6265 6b27 2c0d 0a20 2020 2020 2020 2020  bek',..         
+00006620: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00006630: 7669 273a 2027 5669 6574 6e61 6d65 7365  vi': 'Vietnamese
+00006640: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00006650: 2020 2020 2020 2020 2020 2020 2763 7927              'cy'
+00006660: 3a20 2757 656c 7368 272c 0d0a 2020 2020  : 'Welsh',..    
+00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006680: 2020 2020 2779 6927 3a20 2759 6964 6469      'yi': 'Yiddi
+00006690: 7368 272c 0d0a 2020 2020 2020 2020 2020  sh',..          
+000066a0: 2020 2020 2020 2020 2020 2020 2020 2779                'y
+000066b0: 6f27 3a20 2759 6f72 7562 6127 2c0d 0a20  o': 'Yoruba',.. 
+000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066d0: 2020 207d 0d0a 0d0a 2020 2020 6465 6620     }....    def 
+000066e0: 6765 745f 6e61 6d65 2873 656c 662c 2067  get_name(self, g
+000066f0: 6574 5f63 6f64 6529 3a0d 0a20 2020 2020  et_code):..     
+00006700: 2020 2072 6574 7572 6e20 7365 6c66 2e64     return self.d
+00006710: 6963 742e 6765 7428 6765 745f 636f 6465  ict.get(get_code
+00006720: 2e6c 6f77 6572 2829 2c20 2222 290d 0a0d  .lower(), "")...
+00006730: 0a20 2020 2064 6566 2067 6574 5f63 6f64  .    def get_cod
+00006740: 6528 7365 6c66 2c20 6c61 6e67 7561 6765  e(self, language
+00006750: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
+00006760: 6765 745f 636f 6465 2c20 6c61 6e67 2069  get_code, lang i
+00006770: 6e20 7365 6c66 2e64 6963 742e 6974 656d  n self.dict.item
+00006780: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+00006790: 2020 6966 206c 616e 672e 6c6f 7765 7228    if lang.lower(
+000067a0: 2920 3d3d 206c 616e 6775 6167 652e 6c6f  ) == language.lo
+000067b0: 7765 7228 293a 0d0a 2020 2020 2020 2020  wer():..        
+000067c0: 2020 2020 2020 2020 7265 7475 726e 2067          return g
+000067d0: 6574 5f63 6f64 650d 0a20 2020 2020 2020  et_code..       
+000067e0: 2072 6574 7572 6e20 2222 0d0a 0d0a 0d0a   return ""......
+000067f0: 636c 6173 7320 476f 6f67 6c65 4c61 6e67  class GoogleLang
+00006800: 7561 6765 3a0d 0a20 2020 2064 6566 205f  uage:..    def _
+00006810: 5f69 6e69 745f 5f28 7365 6c66 293a 0d0a  _init__(self):..
+00006820: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00006830: 745f 636f 6465 7320 3d20 5b5d 0d0a 2020  t_codes = []..  
+00006840: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00006850: 636f 6465 732e 6170 7065 6e64 2822 6166  codes.append("af
+00006860: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00006870: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00006880: 6e64 2822 7371 2229 0d0a 2020 2020 2020  nd("sq")..      
+00006890: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+000068a0: 732e 6170 7065 6e64 2822 616d 2229 0d0a  s.append("am")..
+000068b0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000068c0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+000068d0: 6172 2229 0d0a 2020 2020 2020 2020 7365  ar")..        se
+000068e0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+000068f0: 7065 6e64 2822 6879 2229 0d0a 2020 2020  pend("hy")..    
+00006900: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00006910: 6465 732e 6170 7065 6e64 2822 6173 2229  des.append("as")
+00006920: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00006930: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00006940: 2822 6179 2229 0d0a 2020 2020 2020 2020  ("ay")..        
+00006950: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00006960: 6170 7065 6e64 2822 617a 2229 0d0a 2020  append("az")..  
+00006970: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00006980: 636f 6465 732e 6170 7065 6e64 2822 626d  codes.append("bm
+00006990: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000069a0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+000069b0: 6e64 2822 6575 2229 0d0a 2020 2020 2020  nd("eu")..      
+000069c0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+000069d0: 732e 6170 7065 6e64 2822 6265 2229 0d0a  s.append("be")..
+000069e0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000069f0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00006a00: 626e 2229 0d0a 2020 2020 2020 2020 7365  bn")..        se
+00006a10: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00006a20: 7065 6e64 2822 6268 6f22 290d 0a20 2020  pend("bho")..   
+00006a30: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00006a40: 6f64 6573 2e61 7070 656e 6428 2262 7322  odes.append("bs"
+00006a50: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00006a60: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00006a70: 6428 2262 6722 290d 0a20 2020 2020 2020  d("bg")..       
+00006a80: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00006a90: 2e61 7070 656e 6428 2263 6122 290d 0a20  .append("ca").. 
+00006aa0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00006ab0: 5f63 6f64 6573 2e61 7070 656e 6428 2263  _codes.append("c
+00006ac0: 6562 2229 0d0a 2020 2020 2020 2020 7365  eb")..        se
+00006ad0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00006ae0: 7065 6e64 2822 6e79 2229 0d0a 2020 2020  pend("ny")..    
+00006af0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00006b00: 6465 732e 6170 7065 6e64 2822 7a68 2d43  des.append("zh-C
+00006b10: 4e22 290d 0a20 2020 2020 2020 2073 656c  N")..        sel
+00006b20: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00006b30: 656e 6428 227a 682d 5457 2229 0d0a 2020  end("zh-TW")..  
+00006b40: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00006b50: 636f 6465 732e 6170 7065 6e64 2822 636f  codes.append("co
+00006b60: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00006b70: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00006b80: 6e64 2822 6872 2229 0d0a 2020 2020 2020  nd("hr")..      
+00006b90: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00006ba0: 732e 6170 7065 6e64 2822 6373 2229 0d0a  s.append("cs")..
+00006bb0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00006bc0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00006bd0: 6461 2229 0d0a 2020 2020 2020 2020 7365  da")..        se
+00006be0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00006bf0: 7065 6e64 2822 6476 2229 0d0a 2020 2020  pend("dv")..    
+00006c00: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00006c10: 6465 732e 6170 7065 6e64 2822 646f 6922  des.append("doi"
+00006c20: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00006c30: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00006c40: 6428 226e 6c22 290d 0a20 2020 2020 2020  d("nl")..       
+00006c50: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00006c60: 2e61 7070 656e 6428 2265 6e22 290d 0a20  .append("en").. 
+00006c70: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00006c80: 5f63 6f64 6573 2e61 7070 656e 6428 2265  _codes.append("e
+00006c90: 6f22 290d 0a20 2020 2020 2020 2073 656c  o")..        sel
+00006ca0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00006cb0: 656e 6428 2265 7422 290d 0a20 2020 2020  end("et")..     
+00006cc0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00006cd0: 6573 2e61 7070 656e 6428 2265 6522 290d  es.append("ee").
+00006ce0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00006cf0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00006d00: 2266 696c 2229 0d0a 2020 2020 2020 2020  "fil")..        
+00006d10: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00006d20: 6170 7065 6e64 2822 6669 2229 0d0a 2020  append("fi")..  
+00006d30: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00006d40: 636f 6465 732e 6170 7065 6e64 2822 6672  codes.append("fr
+00006d50: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00006d60: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00006d70: 6e64 2822 6679 2229 0d0a 2020 2020 2020  nd("fy")..      
+00006d80: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00006d90: 732e 6170 7065 6e64 2822 676c 2229 0d0a  s.append("gl")..
+00006da0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00006db0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00006dc0: 6b61 2229 0d0a 2020 2020 2020 2020 7365  ka")..        se
+00006dd0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00006de0: 7065 6e64 2822 6465 2229 0d0a 2020 2020  pend("de")..    
+00006df0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00006e00: 6465 732e 6170 7065 6e64 2822 656c 2229  des.append("el")
+00006e10: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00006e20: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00006e30: 2822 676e 2229 0d0a 2020 2020 2020 2020  ("gn")..        
+00006e40: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00006e50: 6170 7065 6e64 2822 6775 2229 0d0a 2020  append("gu")..  
+00006e60: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00006e70: 636f 6465 732e 6170 7065 6e64 2822 6874  codes.append("ht
+00006e80: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00006e90: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00006ea0: 6e64 2822 6861 2229 0d0a 2020 2020 2020  nd("ha")..      
+00006eb0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00006ec0: 732e 6170 7065 6e64 2822 6861 7722 290d  s.append("haw").
+00006ed0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00006ee0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00006ef0: 2268 6522 290d 0a20 2020 2020 2020 2073  "he")..        s
+00006f00: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00006f10: 7070 656e 6428 2268 6922 290d 0a20 2020  ppend("hi")..   
+00006f20: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00006f30: 6f64 6573 2e61 7070 656e 6428 2268 6d6e  odes.append("hmn
+00006f40: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00006f50: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00006f60: 6e64 2822 6875 2229 0d0a 2020 2020 2020  nd("hu")..      
+00006f70: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00006f80: 732e 6170 7065 6e64 2822 6973 2229 0d0a  s.append("is")..
+00006f90: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00006fa0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00006fb0: 6967 2229 0d0a 2020 2020 2020 2020 7365  ig")..        se
+00006fc0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00006fd0: 7065 6e64 2822 696c 6f22 290d 0a20 2020  pend("ilo")..   
+00006fe0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00006ff0: 6f64 6573 2e61 7070 656e 6428 2269 6422  odes.append("id"
+00007000: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007010: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007020: 6428 2267 6122 290d 0a20 2020 2020 2020  d("ga")..       
+00007030: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007040: 2e61 7070 656e 6428 2269 7422 290d 0a20  .append("it").. 
+00007050: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007060: 5f63 6f64 6573 2e61 7070 656e 6428 226a  _codes.append("j
+00007070: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
+00007080: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00007090: 656e 6428 226a 7622 290d 0a20 2020 2020  end("jv")..     
+000070a0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+000070b0: 6573 2e61 7070 656e 6428 226b 6e22 290d  es.append("kn").
+000070c0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000070d0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+000070e0: 226b 6b22 290d 0a20 2020 2020 2020 2073  "kk")..        s
+000070f0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00007100: 7070 656e 6428 226b 6d22 290d 0a20 2020  ppend("km")..   
+00007110: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00007120: 6f64 6573 2e61 7070 656e 6428 2272 7722  odes.append("rw"
+00007130: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007140: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007150: 6428 2267 6f6d 2229 0d0a 2020 2020 2020  d("gom")..      
+00007160: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00007170: 732e 6170 7065 6e64 2822 6b6f 2229 0d0a  s.append("ko")..
+00007180: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007190: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+000071a0: 6b72 6922 290d 0a20 2020 2020 2020 2073  kri")..        s
+000071b0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+000071c0: 7070 656e 6428 226b 6d72 2229 0d0a 2020  ppend("kmr")..  
+000071d0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000071e0: 636f 6465 732e 6170 7065 6e64 2822 636b  codes.append("ck
+000071f0: 6222 290d 0a20 2020 2020 2020 2073 656c  b")..        sel
+00007200: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00007210: 656e 6428 226b 7922 290d 0a20 2020 2020  end("ky")..     
+00007220: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00007230: 6573 2e61 7070 656e 6428 226c 6f22 290d  es.append("lo").
+00007240: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007250: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00007260: 226c 6122 290d 0a20 2020 2020 2020 2073  "la")..        s
+00007270: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00007280: 7070 656e 6428 226c 7622 290d 0a20 2020  ppend("lv")..   
+00007290: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+000072a0: 6f64 6573 2e61 7070 656e 6428 226c 6e22  odes.append("ln"
+000072b0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000072c0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+000072d0: 6428 226c 7422 290d 0a20 2020 2020 2020  d("lt")..       
+000072e0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+000072f0: 2e61 7070 656e 6428 226c 6722 290d 0a20  .append("lg").. 
+00007300: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007310: 5f63 6f64 6573 2e61 7070 656e 6428 226c  _codes.append("l
+00007320: 6222 290d 0a20 2020 2020 2020 2073 656c  b")..        sel
+00007330: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00007340: 656e 6428 226d 6b22 290d 0a20 2020 2020  end("mk")..     
+00007350: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00007360: 6573 2e61 7070 656e 6428 226d 6722 290d  es.append("mg").
+00007370: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007380: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00007390: 226d 7322 290d 0a20 2020 2020 2020 2073  "ms")..        s
+000073a0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+000073b0: 7070 656e 6428 226d 6c22 290d 0a20 2020  ppend("ml")..   
+000073c0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+000073d0: 6f64 6573 2e61 7070 656e 6428 226d 7422  odes.append("mt"
+000073e0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000073f0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007400: 6428 226d 6922 290d 0a20 2020 2020 2020  d("mi")..       
+00007410: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007420: 2e61 7070 656e 6428 226d 7222 290d 0a20  .append("mr").. 
+00007430: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007440: 5f63 6f64 6573 2e61 7070 656e 6428 226d  _codes.append("m
+00007450: 6e69 2d4d 7465 6922 290d 0a20 2020 2020  ni-Mtei")..     
+00007460: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00007470: 6573 2e61 7070 656e 6428 226c 7573 2229  es.append("lus")
+00007480: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00007490: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+000074a0: 2822 6d6e 2229 0d0a 2020 2020 2020 2020  ("mn")..        
+000074b0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+000074c0: 6170 7065 6e64 2822 6d79 2229 0d0a 2020  append("my")..  
+000074d0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000074e0: 636f 6465 732e 6170 7065 6e64 2822 6e65  codes.append("ne
+000074f0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00007500: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00007510: 6e64 2822 6e6f 2229 0d0a 2020 2020 2020  nd("no")..      
+00007520: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00007530: 732e 6170 7065 6e64 2822 6f72 2229 0d0a  s.append("or")..
+00007540: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007550: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00007560: 6f6d 2229 0d0a 2020 2020 2020 2020 7365  om")..        se
+00007570: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00007580: 7065 6e64 2822 7073 2229 0d0a 2020 2020  pend("ps")..    
+00007590: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+000075a0: 6465 732e 6170 7065 6e64 2822 6661 2229  des.append("fa")
+000075b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000075c0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+000075d0: 2822 706c 2229 0d0a 2020 2020 2020 2020  ("pl")..        
+000075e0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+000075f0: 6170 7065 6e64 2822 7074 2229 0d0a 2020  append("pt")..  
+00007600: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00007610: 636f 6465 732e 6170 7065 6e64 2822 7061  codes.append("pa
+00007620: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00007630: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00007640: 6e64 2822 7175 2229 0d0a 2020 2020 2020  nd("qu")..      
+00007650: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00007660: 732e 6170 7065 6e64 2822 726f 2229 0d0a  s.append("ro")..
+00007670: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007680: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00007690: 7275 2229 0d0a 2020 2020 2020 2020 7365  ru")..        se
+000076a0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+000076b0: 7065 6e64 2822 736d 2229 0d0a 2020 2020  pend("sm")..    
+000076c0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+000076d0: 6465 732e 6170 7065 6e64 2822 7361 2229  des.append("sa")
+000076e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000076f0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00007700: 2822 6764 2229 0d0a 2020 2020 2020 2020  ("gd")..        
+00007710: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00007720: 6170 7065 6e64 2822 6e73 6f22 290d 0a20  append("nso").. 
+00007730: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007740: 5f63 6f64 6573 2e61 7070 656e 6428 2273  _codes.append("s
+00007750: 7222 290d 0a20 2020 2020 2020 2073 656c  r")..        sel
+00007760: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00007770: 656e 6428 2273 7422 290d 0a20 2020 2020  end("st")..     
+00007780: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00007790: 6573 2e61 7070 656e 6428 2273 6e22 290d  es.append("sn").
+000077a0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000077b0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+000077c0: 2273 6422 290d 0a20 2020 2020 2020 2073  "sd")..        s
+000077d0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+000077e0: 7070 656e 6428 2273 6922 290d 0a20 2020  ppend("si")..   
+000077f0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00007800: 6f64 6573 2e61 7070 656e 6428 2273 6b22  odes.append("sk"
+00007810: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007820: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007830: 6428 2273 6c22 290d 0a20 2020 2020 2020  d("sl")..       
+00007840: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007850: 2e61 7070 656e 6428 2273 6f22 290d 0a20  .append("so").. 
+00007860: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007870: 5f63 6f64 6573 2e61 7070 656e 6428 2265  _codes.append("e
+00007880: 7322 290d 0a20 2020 2020 2020 2073 656c  s")..        sel
+00007890: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+000078a0: 656e 6428 2273 7522 290d 0a20 2020 2020  end("su")..     
+000078b0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+000078c0: 6573 2e61 7070 656e 6428 2273 7722 290d  es.append("sw").
+000078d0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000078e0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+000078f0: 2273 7622 290d 0a20 2020 2020 2020 2073  "sv")..        s
+00007900: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00007910: 7070 656e 6428 2274 6722 290d 0a20 2020  ppend("tg")..   
+00007920: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00007930: 6f64 6573 2e61 7070 656e 6428 2274 6122  odes.append("ta"
+00007940: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007950: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007960: 6428 2274 7422 290d 0a20 2020 2020 2020  d("tt")..       
+00007970: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007980: 2e61 7070 656e 6428 2274 6522 290d 0a20  .append("te").. 
+00007990: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000079a0: 5f63 6f64 6573 2e61 7070 656e 6428 2274  _codes.append("t
+000079b0: 6822 290d 0a20 2020 2020 2020 2073 656c  h")..        sel
+000079c0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+000079d0: 656e 6428 2274 6922 290d 0a20 2020 2020  end("ti")..     
+000079e0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+000079f0: 6573 2e61 7070 656e 6428 2274 7322 290d  es.append("ts").
+00007a00: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007a10: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00007a20: 2274 7222 290d 0a20 2020 2020 2020 2073  "tr")..        s
+00007a30: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00007a40: 7070 656e 6428 2274 6b22 290d 0a20 2020  ppend("tk")..   
+00007a50: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00007a60: 6f64 6573 2e61 7070 656e 6428 2274 7722  odes.append("tw"
+00007a70: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007a80: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007a90: 6428 2275 6b22 290d 0a20 2020 2020 2020  d("uk")..       
+00007aa0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007ab0: 2e61 7070 656e 6428 2275 7222 290d 0a20  .append("ur").. 
+00007ac0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007ad0: 5f63 6f64 6573 2e61 7070 656e 6428 2275  _codes.append("u
+00007ae0: 6722 290d 0a20 2020 2020 2020 2073 656c  g")..        sel
+00007af0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00007b00: 656e 6428 2275 7a22 290d 0a20 2020 2020  end("uz")..     
+00007b10: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00007b20: 6573 2e61 7070 656e 6428 2276 6922 290d  es.append("vi").
+00007b30: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007b40: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00007b50: 2263 7922 290d 0a20 2020 2020 2020 2073  "cy")..        s
+00007b60: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00007b70: 7070 656e 6428 2278 6822 290d 0a20 2020  ppend("xh")..   
+00007b80: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00007b90: 6f64 6573 2e61 7070 656e 6428 2279 6922  odes.append("yi"
+00007ba0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007bb0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007bc0: 6428 2279 6f22 290d 0a20 2020 2020 2020  d("yo")..       
+00007bd0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007be0: 2e61 7070 656e 6428 227a 7522 290d 0a0d  .append("zu")...
+00007bf0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007c00: 7374 5f6e 616d 6573 203d 205b 5d0d 0a20  st_names = [].. 
+00007c10: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007c20: 5f6e 616d 6573 2e61 7070 656e 6428 2241  _names.append("A
+00007c30: 6672 696b 6161 6e73 2229 0d0a 2020 2020  frikaans")..    
+00007c40: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00007c50: 6d65 732e 6170 7065 6e64 2822 416c 6261  mes.append("Alba
+00007c60: 6e69 616e 2229 0d0a 2020 2020 2020 2020  nian")..        
+00007c70: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00007c80: 6170 7065 6e64 2822 416d 6861 7269 6322  append("Amharic"
+00007c90: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007ca0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00007cb0: 6428 2241 7261 6269 6322 290d 0a20 2020  d("Arabic")..   
+00007cc0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00007cd0: 616d 6573 2e61 7070 656e 6428 2241 726d  ames.append("Arm
+00007ce0: 656e 6961 6e22 290d 0a20 2020 2020 2020  enian")..       
+00007cf0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00007d00: 2e61 7070 656e 6428 2241 7373 616d 6573  .append("Assames
+00007d10: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
+00007d20: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00007d30: 656e 6428 2241 796d 6172 6122 290d 0a20  end("Aymara").. 
+00007d40: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007d50: 5f6e 616d 6573 2e61 7070 656e 6428 2241  _names.append("A
+00007d60: 7a65 7262 6169 6a61 6e69 2229 0d0a 2020  zerbaijani")..  
+00007d70: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00007d80: 6e61 6d65 732e 6170 7065 6e64 2822 4261  names.append("Ba
+00007d90: 6d62 6172 6122 290d 0a20 2020 2020 2020  mbara")..       
+00007da0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00007db0: 2e61 7070 656e 6428 2242 6173 7175 6522  .append("Basque"
+00007dc0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007dd0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00007de0: 6428 2242 656c 6172 7573 6961 6e22 290d  d("Belarusian").
+00007df0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007e00: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00007e10: 2242 656e 6761 6c69 2229 0d0a 2020 2020  "Bengali")..    
+00007e20: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00007e30: 6d65 732e 6170 7065 6e64 2822 4268 6f6a  mes.append("Bhoj
+00007e40: 7075 7269 2229 0d0a 2020 2020 2020 2020  puri")..        
+00007e50: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00007e60: 6170 7065 6e64 2822 426f 736e 6961 6e22  append("Bosnian"
+00007e70: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007e80: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00007e90: 6428 2242 756c 6761 7269 616e 2229 0d0a  d("Bulgarian")..
+00007ea0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007eb0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00007ec0: 4361 7461 6c61 6e22 290d 0a20 2020 2020  Catalan")..     
 00007ed0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00007ee0: 6573 2e61 7070 656e 6428 2243 6869 6e65  es.append("Chine
-00007ef0: 7365 2028 5472 6164 6974 696f 6e61 6c29  se (Traditional)
-00007f00: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007f10: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00007f20: 6e64 2822 436f 7273 6963 616e 2229 0d0a  nd("Corsican")..
-00007f30: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007f40: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00007f50: 4372 6f61 7469 616e 2229 0d0a 2020 2020  Croatian")..    
-00007f60: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00007f70: 6d65 732e 6170 7065 6e64 2822 437a 6563  mes.append("Czec
-00007f80: 6822 290d 0a20 2020 2020 2020 2073 656c  h")..        sel
-00007f90: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00007fa0: 656e 6428 2244 616e 6973 6822 290d 0a20  end("Danish").. 
-00007fb0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007fc0: 5f6e 616d 6573 2e61 7070 656e 6428 2244  _names.append("D
-00007fd0: 6869 7665 6869 2229 0d0a 2020 2020 2020  hivehi")..      
-00007fe0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00007ff0: 732e 6170 7065 6e64 2822 446f 6772 6922  s.append("Dogri"
-00008000: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008010: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008020: 6428 2244 7574 6368 2229 0d0a 2020 2020  d("Dutch")..    
-00008030: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008040: 6d65 732e 6170 7065 6e64 2822 456e 676c  mes.append("Engl
-00008050: 6973 6822 290d 0a20 2020 2020 2020 2073  ish")..        s
-00008060: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008070: 7070 656e 6428 2245 7370 6572 616e 746f  ppend("Esperanto
-00008080: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008090: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-000080a0: 6e64 2822 4573 746f 6e69 616e 2229 0d0a  nd("Estonian")..
-000080b0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000080c0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000080d0: 4577 6522 290d 0a20 2020 2020 2020 2073  Ewe")..        s
-000080e0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-000080f0: 7070 656e 6428 2246 696c 6970 696e 6f22  ppend("Filipino"
-00008100: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008110: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008120: 6428 2246 696e 6e69 7368 2229 0d0a 2020  d("Finnish")..  
-00008130: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008140: 6e61 6d65 732e 6170 7065 6e64 2822 4672  names.append("Fr
-00008150: 656e 6368 2229 0d0a 2020 2020 2020 2020  ench")..        
-00008160: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00008170: 6170 7065 6e64 2822 4672 6973 6961 6e22  append("Frisian"
-00008180: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008190: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-000081a0: 6428 2247 616c 6963 6961 6e22 290d 0a20  d("Galician").. 
-000081b0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000081c0: 5f6e 616d 6573 2e61 7070 656e 6428 2247  _names.append("G
-000081d0: 656f 7267 6961 6e22 290d 0a20 2020 2020  eorgian")..     
-000081e0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-000081f0: 6573 2e61 7070 656e 6428 2247 6572 6d61  es.append("Germa
-00008200: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-00008210: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00008220: 656e 6428 2247 7265 656b 2229 0d0a 2020  end("Greek")..  
-00008230: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008240: 6e61 6d65 732e 6170 7065 6e64 2822 4775  names.append("Gu
-00008250: 6172 616e 6922 290d 0a20 2020 2020 2020  arani")..       
-00008260: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00008270: 2e61 7070 656e 6428 2247 756a 6172 6174  .append("Gujarat
-00008280: 6922 290d 0a20 2020 2020 2020 2073 656c  i")..        sel
-00008290: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-000082a0: 656e 6428 2248 6169 7469 616e 2043 7265  end("Haitian Cre
-000082b0: 6f6c 6522 290d 0a20 2020 2020 2020 2073  ole")..        s
-000082c0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-000082d0: 7070 656e 6428 2248 6175 7361 2229 0d0a  ppend("Hausa")..
-000082e0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000082f0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00008300: 4861 7761 6969 616e 2229 0d0a 2020 2020  Hawaiian")..    
-00008310: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008320: 6d65 732e 6170 7065 6e64 2822 4865 6272  mes.append("Hebr
-00008330: 6577 2229 0d0a 2020 2020 2020 2020 7365  ew")..        se
-00008340: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008350: 7065 6e64 2822 4869 6e64 6922 290d 0a20  pend("Hindi").. 
-00008360: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008370: 5f6e 616d 6573 2e61 7070 656e 6428 2248  _names.append("H
-00008380: 6d6f 6e67 2229 0d0a 2020 2020 2020 2020  mong")..        
-00008390: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-000083a0: 6170 7065 6e64 2822 4875 6e67 6172 6961  append("Hungaria
-000083b0: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-000083c0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-000083d0: 656e 6428 2249 6365 6c61 6e64 6963 2229  end("Icelandic")
-000083e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000083f0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00008400: 2822 4967 626f 2229 0d0a 2020 2020 2020  ("Igbo")..      
-00008410: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00008420: 732e 6170 7065 6e64 2822 496c 6f63 616e  s.append("Ilocan
-00008430: 6f22 290d 0a20 2020 2020 2020 2073 656c  o")..        sel
-00008440: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00008450: 656e 6428 2249 6e64 6f6e 6573 6961 6e22  end("Indonesian"
-00008460: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008470: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008480: 6428 2249 7269 7368 2229 0d0a 2020 2020  d("Irish")..    
-00008490: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-000084a0: 6d65 732e 6170 7065 6e64 2822 4974 616c  mes.append("Ital
-000084b0: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
-000084c0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-000084d0: 7070 656e 6428 224a 6170 616e 6573 6522  ppend("Japanese"
-000084e0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000084f0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008500: 6428 224a 6176 616e 6573 6522 290d 0a20  d("Javanese").. 
-00008510: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008520: 5f6e 616d 6573 2e61 7070 656e 6428 224b  _names.append("K
-00008530: 616e 6e61 6461 2229 0d0a 2020 2020 2020  annada")..      
-00008540: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00008550: 732e 6170 7065 6e64 2822 4b61 7a61 6b68  s.append("Kazakh
-00008560: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008570: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008580: 6e64 2822 4b68 6d65 7222 290d 0a20 2020  nd("Khmer")..   
-00008590: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-000085a0: 616d 6573 2e61 7070 656e 6428 224b 696e  ames.append("Kin
-000085b0: 7961 7277 616e 6461 2229 0d0a 2020 2020  yarwanda")..    
-000085c0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-000085d0: 6d65 732e 6170 7065 6e64 2822 4b6f 6e6b  mes.append("Konk
-000085e0: 616e 6922 290d 0a20 2020 2020 2020 2073  ani")..        s
-000085f0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008600: 7070 656e 6428 224b 6f72 6561 6e22 290d  ppend("Korean").
-00008610: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008620: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008630: 224b 7269 6f22 290d 0a20 2020 2020 2020  "Krio")..       
-00008640: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00008650: 2e61 7070 656e 6428 224b 7572 6469 7368  .append("Kurdish
-00008660: 2028 4b75 726d 616e 6a69 2922 290d 0a20   (Kurmanji)").. 
-00008670: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008680: 5f6e 616d 6573 2e61 7070 656e 6428 224b  _names.append("K
-00008690: 7572 6469 7368 2028 536f 7261 6e69 2922  urdish (Sorani)"
-000086a0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000086b0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-000086c0: 6428 224b 7972 6779 7a22 290d 0a20 2020  d("Kyrgyz")..   
-000086d0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-000086e0: 616d 6573 2e61 7070 656e 6428 224c 616f  ames.append("Lao
-000086f0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008700: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008710: 6e64 2822 4c61 7469 6e22 290d 0a20 2020  nd("Latin")..   
-00008720: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00008730: 616d 6573 2e61 7070 656e 6428 224c 6174  ames.append("Lat
-00008740: 7669 616e 2229 0d0a 2020 2020 2020 2020  vian")..        
-00008750: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00008760: 6170 7065 6e64 2822 4c69 6e67 616c 6122  append("Lingala"
-00008770: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008780: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008790: 6428 224c 6974 6875 616e 6961 6e22 290d  d("Lithuanian").
-000087a0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000087b0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-000087c0: 224c 7567 616e 6461 2229 0d0a 2020 2020  "Luganda")..    
-000087d0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-000087e0: 6d65 732e 6170 7065 6e64 2822 4c75 7865  mes.append("Luxe
-000087f0: 6d62 6f75 7267 6973 6822 290d 0a20 2020  mbourgish")..   
-00008800: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00008810: 616d 6573 2e61 7070 656e 6428 224d 6163  ames.append("Mac
-00008820: 6564 6f6e 6961 6e22 290d 0a20 2020 2020  edonian")..     
-00008830: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00008840: 6573 2e61 7070 656e 6428 224d 616c 6167  es.append("Malag
-00008850: 6173 7922 290d 0a20 2020 2020 2020 2073  asy")..        s
-00008860: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008870: 7070 656e 6428 224d 616c 6179 2229 0d0a  ppend("Malay")..
-00008880: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00008890: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000088a0: 4d61 6c61 7961 6c61 6d22 290d 0a20 2020  Malayalam")..   
-000088b0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-000088c0: 616d 6573 2e61 7070 656e 6428 224d 616c  ames.append("Mal
-000088d0: 7465 7365 2229 0d0a 2020 2020 2020 2020  tese")..        
-000088e0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-000088f0: 6170 7065 6e64 2822 4d61 6f72 6922 290d  append("Maori").
-00008900: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008910: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008920: 224d 6172 6174 6869 2229 0d0a 2020 2020  "Marathi")..    
-00008930: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008940: 6d65 732e 6170 7065 6e64 2822 4d65 6974  mes.append("Meit
-00008950: 6569 6c6f 6e20 284d 616e 6970 7572 6929  eilon (Manipuri)
-00008960: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008970: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008980: 6e64 2822 4d69 7a6f 2229 0d0a 2020 2020  nd("Mizo")..    
-00008990: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-000089a0: 6d65 732e 6170 7065 6e64 2822 4d6f 6e67  mes.append("Mong
-000089b0: 6f6c 6961 6e22 290d 0a20 2020 2020 2020  olian")..       
-000089c0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-000089d0: 2e61 7070 656e 6428 224d 7961 6e6d 6172  .append("Myanmar
-000089e0: 2028 4275 726d 6573 6529 2229 0d0a 2020   (Burmese)")..  
-000089f0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008a00: 6e61 6d65 732e 6170 7065 6e64 2822 4e65  names.append("Ne
-00008a10: 7061 6c69 2229 0d0a 2020 2020 2020 2020  pali")..        
-00008a20: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00008a30: 6170 7065 6e64 2822 4e6f 7277 6567 6961  append("Norwegia
-00008a40: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-00008a50: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00008a60: 656e 6428 224f 6469 7961 2028 4f72 6979  end("Odiya (Oriy
-00008a70: 6129 2229 0d0a 2020 2020 2020 2020 7365  a)")..        se
-00008a80: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008a90: 7065 6e64 2822 4f72 6f6d 6f22 290d 0a20  pend("Oromo").. 
-00008aa0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008ab0: 5f6e 616d 6573 2e61 7070 656e 6428 2250  _names.append("P
-00008ac0: 6173 6874 6f22 290d 0a20 2020 2020 2020  ashto")..       
-00008ad0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00008ae0: 2e61 7070 656e 6428 2250 6572 7369 616e  .append("Persian
-00008af0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008b00: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008b10: 6e64 2822 506f 6c69 7368 2229 0d0a 2020  nd("Polish")..  
-00008b20: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008b30: 6e61 6d65 732e 6170 7065 6e64 2822 506f  names.append("Po
-00008b40: 7274 7567 7565 7365 2229 0d0a 2020 2020  rtuguese")..    
-00008b50: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008b60: 6d65 732e 6170 7065 6e64 2822 5075 6e6a  mes.append("Punj
-00008b70: 6162 6922 290d 0a20 2020 2020 2020 2073  abi")..        s
-00008b80: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008b90: 7070 656e 6428 2251 7565 6368 7561 2229  ppend("Quechua")
-00008ba0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00008bb0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00008bc0: 2822 526f 6d61 6e69 616e 2229 0d0a 2020  ("Romanian")..  
-00008bd0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008be0: 6e61 6d65 732e 6170 7065 6e64 2822 5275  names.append("Ru
-00008bf0: 7373 6961 6e22 290d 0a20 2020 2020 2020  ssian")..       
-00008c00: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00008c10: 2e61 7070 656e 6428 2253 616d 6f61 6e22  .append("Samoan"
-00008c20: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008c30: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008c40: 6428 2253 616e 736b 7269 7422 290d 0a20  d("Sanskrit").. 
-00008c50: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008c60: 5f6e 616d 6573 2e61 7070 656e 6428 2253  _names.append("S
-00008c70: 636f 7473 2047 6165 6c69 6322 290d 0a20  cots Gaelic").. 
-00008c80: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008c90: 5f6e 616d 6573 2e61 7070 656e 6428 2253  _names.append("S
-00008ca0: 6570 6564 6922 290d 0a20 2020 2020 2020  epedi")..       
-00008cb0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00008cc0: 2e61 7070 656e 6428 2253 6572 6269 616e  .append("Serbian
-00008cd0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008ce0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008cf0: 6e64 2822 5365 736f 7468 6f22 290d 0a20  nd("Sesotho").. 
-00008d00: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008d10: 5f6e 616d 6573 2e61 7070 656e 6428 2253  _names.append("S
-00008d20: 686f 6e61 2229 0d0a 2020 2020 2020 2020  hona")..        
-00008d30: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00008d40: 6170 7065 6e64 2822 5369 6e64 6869 2229  append("Sindhi")
-00008d50: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00008d60: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00008d70: 2822 5369 6e68 616c 6122 290d 0a20 2020  ("Sinhala")..   
-00008d80: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00008d90: 616d 6573 2e61 7070 656e 6428 2253 6c6f  ames.append("Slo
-00008da0: 7661 6b22 290d 0a20 2020 2020 2020 2073  vak")..        s
-00008db0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008dc0: 7070 656e 6428 2253 6c6f 7665 6e69 616e  ppend("Slovenian
-00008dd0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008de0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008df0: 6e64 2822 536f 6d61 6c69 2229 0d0a 2020  nd("Somali")..  
-00008e00: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008e10: 6e61 6d65 732e 6170 7065 6e64 2822 5370  names.append("Sp
-00008e20: 616e 6973 6822 290d 0a20 2020 2020 2020  anish")..       
-00008e30: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00008e40: 2e61 7070 656e 6428 2253 756e 6461 6e65  .append("Sundane
-00008e50: 7365 2229 0d0a 2020 2020 2020 2020 7365  se")..        se
-00008e60: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008e70: 7065 6e64 2822 5377 6168 696c 6922 290d  pend("Swahili").
-00008e80: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008e90: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008ea0: 2253 7765 6469 7368 2229 0d0a 2020 2020  "Swedish")..    
-00008eb0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008ec0: 6d65 732e 6170 7065 6e64 2822 5461 6a69  mes.append("Taji
-00008ed0: 6b22 290d 0a20 2020 2020 2020 2073 656c  k")..        sel
-00008ee0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00008ef0: 656e 6428 2254 616d 696c 2229 0d0a 2020  end("Tamil")..  
-00008f00: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008f10: 6e61 6d65 732e 6170 7065 6e64 2822 5461  names.append("Ta
-00008f20: 7461 7222 290d 0a20 2020 2020 2020 2073  tar")..        s
-00008f30: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008f40: 7070 656e 6428 2254 656c 7567 7522 290d  ppend("Telugu").
-00008f50: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008f60: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008f70: 2254 6861 6922 290d 0a20 2020 2020 2020  "Thai")..       
-00008f80: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00008f90: 2e61 7070 656e 6428 2254 6967 7269 6e79  .append("Tigriny
-00008fa0: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
-00008fb0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00008fc0: 656e 6428 2254 736f 6e67 6122 290d 0a20  end("Tsonga").. 
-00008fd0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008fe0: 5f6e 616d 6573 2e61 7070 656e 6428 2254  _names.append("T
-00008ff0: 7572 6b69 7368 2229 0d0a 2020 2020 2020  urkish")..      
-00009000: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00009010: 732e 6170 7065 6e64 2822 5475 726b 6d65  s.append("Turkme
-00009020: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-00009030: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00009040: 656e 6428 2254 7769 2028 416b 616e 2922  end("Twi (Akan)"
-00009050: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00009060: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00009070: 6428 2255 6b72 6169 6e69 616e 2229 0d0a  d("Ukrainian")..
-00009080: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00009090: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000090a0: 5572 6475 2229 0d0a 2020 2020 2020 2020  Urdu")..        
-000090b0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-000090c0: 6170 7065 6e64 2822 5579 6768 7572 2229  append("Uyghur")
-000090d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000090e0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-000090f0: 2822 557a 6265 6b22 290d 0a20 2020 2020  ("Uzbek")..     
-00009100: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00009110: 6573 2e61 7070 656e 6428 2256 6965 746e  es.append("Vietn
-00009120: 616d 6573 6522 290d 0a20 2020 2020 2020  amese")..       
-00009130: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00009140: 2e61 7070 656e 6428 2257 656c 7368 2229  .append("Welsh")
-00009150: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00009160: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00009170: 2822 5868 6f73 6122 290d 0a20 2020 2020  ("Xhosa")..     
-00009180: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00009190: 6573 2e61 7070 656e 6428 2259 6964 6469  es.append("Yiddi
-000091a0: 7368 2229 0d0a 2020 2020 2020 2020 7365  sh")..        se
-000091b0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-000091c0: 7065 6e64 2822 596f 7275 6261 2229 0d0a  pend("Yoruba")..
-000091d0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000091e0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000091f0: 5a75 6c75 2229 0d0a 0d0a 2020 2020 2020  Zulu")....      
-00009200: 2020 7365 6c66 2e63 6f64 655f 6f66 5f6e    self.code_of_n
-00009210: 616d 6520 3d20 6469 6374 287a 6970 2873  ame = dict(zip(s
-00009220: 656c 662e 6c69 7374 5f6e 616d 6573 2c20  elf.list_names, 
-00009230: 7365 6c66 2e6c 6973 745f 636f 6465 7329  self.list_codes)
-00009240: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00009250: 6e61 6d65 5f6f 665f 636f 6465 203d 2064  name_of_code = d
-00009260: 6963 7428 7a69 7028 7365 6c66 2e6c 6973  ict(zip(self.lis
-00009270: 745f 636f 6465 732c 2073 656c 662e 6c69  t_codes, self.li
-00009280: 7374 5f6e 616d 6573 2929 0d0a 0d0a 2020  st_names))....  
-00009290: 2020 2020 2020 7365 6c66 2e64 6963 7420        self.dict 
-000092a0: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
-000092b0: 2020 2020 2020 2020 2020 2020 2027 6166               'af
-000092c0: 273a 2027 4166 7269 6b61 616e 7327 2c0d  ': 'Afrikaans',.
-000092d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000092e0: 2020 2020 2020 2020 2027 7371 273a 2027           'sq': '
-000092f0: 416c 6261 6e69 616e 272c 0d0a 2020 2020  Albanian',..    
-00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009310: 2020 2020 2761 6d27 3a20 2741 6d68 6172      'am': 'Amhar
-00009320: 6963 272c 0d0a 2020 2020 2020 2020 2020  ic',..          
-00009330: 2020 2020 2020 2020 2020 2020 2020 2761                'a
-00009340: 7227 3a20 2741 7261 6269 6327 2c0d 0a20  r': 'Arabic',.. 
-00009350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009360: 2020 2020 2020 2027 6879 273a 2027 4172         'hy': 'Ar
-00009370: 6d65 6e69 616e 272c 0d0a 2020 2020 2020  menian',..      
-00009380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009390: 2020 2761 7327 3a20 2741 7373 616d 6573    'as': 'Assames
-000093a0: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
-000093b0: 2020 2020 2020 2020 2020 2020 2027 6179               'ay
-000093c0: 273a 2027 4179 6d61 7261 272c 0d0a 2020  ': 'Aymara',..  
-000093d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093e0: 2020 2020 2020 2761 7a27 3a20 2741 7a65        'az': 'Aze
-000093f0: 7262 6169 6a61 6e69 272c 0d0a 2020 2020  rbaijani',..    
-00009400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009410: 2020 2020 2762 6d27 3a20 2742 616d 6261      'bm': 'Bamba
-00009420: 7261 272c 0d0a 2020 2020 2020 2020 2020  ra',..          
-00009430: 2020 2020 2020 2020 2020 2020 2020 2765                'e
-00009440: 7527 3a20 2742 6173 7175 6527 2c0d 0a20  u': 'Basque',.. 
-00009450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009460: 2020 2020 2020 2027 6265 273a 2027 4265         'be': 'Be
-00009470: 6c61 7275 7369 616e 272c 0d0a 2020 2020  larusian',..    
-00009480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009490: 2020 2020 2762 6e27 3a20 2742 656e 6761      'bn': 'Benga
-000094a0: 6c69 272c 0d0a 2020 2020 2020 2020 2020  li',..          
-000094b0: 2020 2020 2020 2020 2020 2020 2020 2762                'b
-000094c0: 686f 273a 2027 4268 6f6a 7075 7269 272c  ho': 'Bhojpuri',
-000094d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000094e0: 2020 2020 2020 2020 2020 2762 7327 3a20            'bs': 
-000094f0: 2742 6f73 6e69 616e 272c 0d0a 2020 2020  'Bosnian',..    
-00009500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009510: 2020 2020 2762 6727 3a20 2742 756c 6761      'bg': 'Bulga
-00009520: 7269 616e 272c 0d0a 2020 2020 2020 2020  rian',..        
-00009530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009540: 2763 6127 3a20 2743 6174 616c 616e 272c  'ca': 'Catalan',
-00009550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009560: 2020 2020 2020 2020 2020 2763 6562 273a            'ceb':
-00009570: 2027 4365 6275 616e 6f27 2c0d 0a20 2020   'Cebuano',..   
-00009580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009590: 2020 2020 2027 6e79 273a 2027 4368 6963       'ny': 'Chic
-000095a0: 6865 7761 272c 0d0a 2020 2020 2020 2020  hewa',..        
-000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095c0: 277a 682d 434e 273a 2027 4368 696e 6573  'zh-CN': 'Chines
-000095d0: 6520 2853 696d 706c 6966 6965 6429 272c  e (Simplified)',
-000095e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000095f0: 2020 2020 2020 2020 2020 277a 682d 5457            'zh-TW
-00009600: 273a 2027 4368 696e 6573 6520 2854 7261  ': 'Chinese (Tra
-00009610: 6469 7469 6f6e 616c 2927 2c0d 0a20 2020  ditional)',..   
-00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009630: 2020 2020 2027 636f 273a 2027 436f 7273       'co': 'Cors
-00009640: 6963 616e 272c 0d0a 2020 2020 2020 2020  ican',..        
-00009650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009660: 2768 7227 3a20 2743 726f 6174 6961 6e27  'hr': 'Croatian'
-00009670: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00009680: 2020 2020 2020 2020 2020 2027 6373 273a             'cs':
-00009690: 2027 437a 6563 6827 2c0d 0a20 2020 2020   'Czech',..     
-000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096b0: 2020 2027 6461 273a 2027 4461 6e69 7368     'da': 'Danish
-000096c0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-000096d0: 2020 2020 2020 2020 2020 2020 2764 7627              'dv'
-000096e0: 3a20 2744 6869 7665 6869 272c 0d0a 2020  : 'Dhivehi',..  
-000096f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009700: 2020 2020 2020 2764 6f69 273a 2027 446f        'doi': 'Do
-00009710: 6772 6927 2c0d 0a20 2020 2020 2020 2020  gri',..         
-00009720: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00009730: 6e6c 273a 2027 4475 7463 6827 2c0d 0a20  nl': 'Dutch',.. 
-00009740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009750: 2020 2020 2020 2027 656e 273a 2027 456e         'en': 'En
-00009760: 676c 6973 6827 2c0d 0a20 2020 2020 2020  glish',..       
-00009770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009780: 2027 656f 273a 2027 4573 7065 7261 6e74   'eo': 'Esperant
-00009790: 6f27 2c0d 0a20 2020 2020 2020 2020 2020  o',..           
-000097a0: 2020 2020 2020 2020 2020 2020 2027 6574               'et
-000097b0: 273a 2027 4573 746f 6e69 616e 272c 0d0a  ': 'Estonian',..
-000097c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097d0: 2020 2020 2020 2020 2765 6527 3a20 2745          'ee': 'E
-000097e0: 7765 272c 0d0a 2020 2020 2020 2020 2020  we',..          
-000097f0: 2020 2020 2020 2020 2020 2020 2020 2766                'f
-00009800: 696c 273a 2027 4669 6c69 7069 6e6f 272c  il': 'Filipino',
-00009810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009820: 2020 2020 2020 2020 2020 2766 6927 3a20            'fi': 
-00009830: 2746 696e 6e69 7368 272c 0d0a 2020 2020  'Finnish',..    
-00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009850: 2020 2020 2766 7227 3a20 2746 7265 6e63      'fr': 'Frenc
-00009860: 6827 2c0d 0a20 2020 2020 2020 2020 2020  h',..           
-00009870: 2020 2020 2020 2020 2020 2020 2027 6679               'fy
-00009880: 273a 2027 4672 6973 6961 6e27 2c0d 0a20  ': 'Frisian',.. 
-00009890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098a0: 2020 2020 2020 2027 676c 273a 2027 4761         'gl': 'Ga
-000098b0: 6c69 6369 616e 272c 0d0a 2020 2020 2020  lician',..      
-000098c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098d0: 2020 276b 6127 3a20 2747 656f 7267 6961    'ka': 'Georgia
-000098e0: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
-000098f0: 2020 2020 2020 2020 2020 2020 2027 6465               'de
-00009900: 273a 2027 4765 726d 616e 272c 0d0a 2020  ': 'German',..  
-00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009920: 2020 2020 2020 2765 6c27 3a20 2747 7265        'el': 'Gre
-00009930: 656b 272c 0d0a 2020 2020 2020 2020 2020  ek',..          
-00009940: 2020 2020 2020 2020 2020 2020 2020 2767                'g
-00009950: 6e27 3a20 2747 7561 7261 6e69 272c 0d0a  n': 'Guarani',..
-00009960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009970: 2020 2020 2020 2020 2767 7527 3a20 2747          'gu': 'G
-00009980: 756a 6172 6174 6927 2c0d 0a20 2020 2020  ujarati',..     
-00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099a0: 2020 2027 6874 273a 2027 4861 6974 6961     'ht': 'Haitia
-000099b0: 6e20 4372 656f 6c65 272c 0d0a 2020 2020  n Creole',..    
-000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099d0: 2020 2020 2768 6127 3a20 2748 6175 7361      'ha': 'Hausa
-000099e0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-000099f0: 2020 2020 2020 2020 2020 2020 2768 6177              'haw
-00009a00: 273a 2027 4861 7761 6969 616e 272c 0d0a  ': 'Hawaiian',..
-00009a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a20: 2020 2020 2020 2020 2768 6527 3a20 2748          'he': 'H
-00009a30: 6562 7265 7727 2c0d 0a20 2020 2020 2020  ebrew',..       
-00009a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a50: 2027 6869 273a 2027 4869 6e64 6927 2c0d   'hi': 'Hindi',.
-00009a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009a70: 2020 2020 2020 2020 2027 686d 6e27 3a20           'hmn': 
-00009a80: 2748 6d6f 6e67 272c 0d0a 2020 2020 2020  'Hmong',..      
-00009a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009aa0: 2020 2768 7527 3a20 2748 756e 6761 7269    'hu': 'Hungari
-00009ab0: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
-00009ac0: 2020 2020 2020 2020 2020 2020 2020 2769                'i
-00009ad0: 7327 3a20 2749 6365 6c61 6e64 6963 272c  s': 'Icelandic',
-00009ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009af0: 2020 2020 2020 2020 2020 2769 6727 3a20            'ig': 
-00009b00: 2749 6762 6f27 2c0d 0a20 2020 2020 2020  'Igbo',..       
-00009b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b20: 2027 696c 6f27 3a20 2749 6c6f 6361 6e6f   'ilo': 'Ilocano
-00009b30: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00009b40: 2020 2020 2020 2020 2020 2020 2769 6427              'id'
-00009b50: 3a20 2749 6e64 6f6e 6573 6961 6e27 2c0d  : 'Indonesian',.
-00009b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009b70: 2020 2020 2020 2020 2027 6761 273a 2027           'ga': '
-00009b80: 4972 6973 6827 2c0d 0a20 2020 2020 2020  Irish',..       
-00009b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ba0: 2027 6974 273a 2027 4974 616c 6961 6e27   'it': 'Italian'
-00009bb0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00009bc0: 2020 2020 2020 2020 2020 2027 6a61 273a             'ja':
-00009bd0: 2027 4a61 7061 6e65 7365 272c 0d0a 2020   'Japanese',..  
-00009be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bf0: 2020 2020 2020 276a 7627 3a20 274a 6176        'jv': 'Jav
-00009c00: 616e 6573 6527 2c0d 0a20 2020 2020 2020  anese',..       
-00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c20: 2027 6b6e 273a 2027 4b61 6e6e 6164 6127   'kn': 'Kannada'
-00009c30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00009c40: 2020 2020 2020 2020 2020 2027 6b6b 273a             'kk':
-00009c50: 2027 4b61 7a61 6b68 272c 0d0a 2020 2020   'Kazakh',..    
-00009c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c70: 2020 2020 276b 6d27 3a20 274b 686d 6572      'km': 'Khmer
-00009c80: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00009c90: 2020 2020 2020 2020 2020 2020 2772 7727              'rw'
-00009ca0: 3a20 274b 696e 7961 7277 616e 6461 272c  : 'Kinyarwanda',
-00009cb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009cc0: 2020 2020 2020 2020 2020 2767 6f6d 273a            'gom':
-00009cd0: 2027 4b6f 6e6b 616e 6927 2c0d 0a20 2020   'Konkani',..   
-00009ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cf0: 2020 2020 2027 6b6f 273a 2027 4b6f 7265       'ko': 'Kore
-00009d00: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
-00009d10: 2020 2020 2020 2020 2020 2020 2020 276b                'k
-00009d20: 7269 273a 2027 4b72 696f 272c 0d0a 2020  ri': 'Krio',..  
-00009d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d40: 2020 2020 2020 276b 6d72 273a 2027 4b75        'kmr': 'Ku
-00009d50: 7264 6973 6820 284b 7572 6d61 6e6a 6929  rdish (Kurmanji)
-00009d60: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00009d70: 2020 2020 2020 2020 2020 2020 2763 6b62              'ckb
-00009d80: 273a 2027 4b75 7264 6973 6820 2853 6f72  ': 'Kurdish (Sor
-00009d90: 616e 6929 272c 0d0a 2020 2020 2020 2020  ani)',..        
-00009da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009db0: 276b 7927 3a20 274b 7972 6779 7a27 2c0d  'ky': 'Kyrgyz',.
-00009dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009dd0: 2020 2020 2020 2020 2027 6c6f 273a 2027           'lo': '
-00009de0: 4c61 6f27 2c0d 0a20 2020 2020 2020 2020  Lao',..         
-00009df0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00009e00: 6c61 273a 2027 4c61 7469 6e27 2c0d 0a20  la': 'Latin',.. 
-00009e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e20: 2020 2020 2020 2027 6c76 273a 2027 4c61         'lv': 'La
-00009e30: 7476 6961 6e27 2c0d 0a20 2020 2020 2020  tvian',..       
-00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e50: 2027 6c6e 273a 2027 4c69 6e67 616c 6127   'ln': 'Lingala'
-00009e60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00009e70: 2020 2020 2020 2020 2020 2027 6c74 273a             'lt':
-00009e80: 2027 4c69 7468 7561 6e69 616e 272c 0d0a   'Lithuanian',..
-00009e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ea0: 2020 2020 2020 2020 276c 6727 3a20 274c          'lg': 'L
-00009eb0: 7567 616e 6461 272c 0d0a 2020 2020 2020  uganda',..      
-00009ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ed0: 2020 276c 6227 3a20 274c 7578 656d 626f    'lb': 'Luxembo
-00009ee0: 7572 6769 7368 272c 0d0a 2020 2020 2020  urgish',..      
-00009ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f00: 2020 276d 6b27 3a20 274d 6163 6564 6f6e    'mk': 'Macedon
-00009f10: 6961 6e27 2c0d 0a20 2020 2020 2020 2020  ian',..         
-00009f20: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00009f30: 6d67 273a 2027 4d61 6c61 6761 7379 272c  mg': 'Malagasy',
-00009f40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009f50: 2020 2020 2020 2020 2020 276d 7327 3a20            'ms': 
-00009f60: 274d 616c 6179 272c 0d0a 2020 2020 2020  'Malay',..      
-00009f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f80: 2020 276d 6c27 3a20 274d 616c 6179 616c    'ml': 'Malayal
-00009f90: 616d 272c 0d0a 2020 2020 2020 2020 2020  am',..          
-00009fa0: 2020 2020 2020 2020 2020 2020 2020 276d                'm
-00009fb0: 7427 3a20 274d 616c 7465 7365 272c 0d0a  t': 'Maltese',..
-00009fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fd0: 2020 2020 2020 2020 276d 6927 3a20 274d          'mi': 'M
-00009fe0: 616f 7269 272c 0d0a 2020 2020 2020 2020  aori',..        
-00009ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a000: 276d 7227 3a20 274d 6172 6174 6869 272c  'mr': 'Marathi',
-0000a010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a020: 2020 2020 2020 2020 2020 276d 6e69 2d4d            'mni-M
-0000a030: 7465 6927 3a20 274d 6569 7465 696c 6f6e  tei': 'Meiteilon
-0000a040: 2028 4d61 6e69 7075 7269 2927 2c0d 0a20   (Manipuri)',.. 
+00007ee0: 6573 2e61 7070 656e 6428 2243 6562 7561  es.append("Cebua
+00007ef0: 6e6f 2229 0d0a 2020 2020 2020 2020 7365  no")..        se
+00007f00: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00007f10: 7065 6e64 2822 4368 6963 6865 7761 2229  pend("Chichewa")
+00007f20: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00007f30: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00007f40: 2822 4368 696e 6573 6520 2853 696d 706c  ("Chinese (Simpl
+00007f50: 6966 6965 6429 2229 0d0a 2020 2020 2020  ified)")..      
+00007f60: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00007f70: 732e 6170 7065 6e64 2822 4368 696e 6573  s.append("Chines
+00007f80: 6520 2854 7261 6469 7469 6f6e 616c 2922  e (Traditional)"
+00007f90: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007fa0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00007fb0: 6428 2243 6f72 7369 6361 6e22 290d 0a20  d("Corsican").. 
+00007fc0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007fd0: 5f6e 616d 6573 2e61 7070 656e 6428 2243  _names.append("C
+00007fe0: 726f 6174 6961 6e22 290d 0a20 2020 2020  roatian")..     
+00007ff0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00008000: 6573 2e61 7070 656e 6428 2243 7a65 6368  es.append("Czech
+00008010: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008020: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00008030: 6e64 2822 4461 6e69 7368 2229 0d0a 2020  nd("Danish")..  
+00008040: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008050: 6e61 6d65 732e 6170 7065 6e64 2822 4468  names.append("Dh
+00008060: 6976 6568 6922 290d 0a20 2020 2020 2020  ivehi")..       
+00008070: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00008080: 2e61 7070 656e 6428 2244 6f67 7269 2229  .append("Dogri")
+00008090: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000080a0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+000080b0: 2822 4475 7463 6822 290d 0a20 2020 2020  ("Dutch")..     
+000080c0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+000080d0: 6573 2e61 7070 656e 6428 2245 6e67 6c69  es.append("Engli
+000080e0: 7368 2229 0d0a 2020 2020 2020 2020 7365  sh")..        se
+000080f0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008100: 7065 6e64 2822 4573 7065 7261 6e74 6f22  pend("Esperanto"
+00008110: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008120: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008130: 6428 2245 7374 6f6e 6961 6e22 290d 0a20  d("Estonian").. 
+00008140: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00008150: 5f6e 616d 6573 2e61 7070 656e 6428 2245  _names.append("E
+00008160: 7765 2229 0d0a 2020 2020 2020 2020 7365  we")..        se
+00008170: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008180: 7065 6e64 2822 4669 6c69 7069 6e6f 2229  pend("Filipino")
+00008190: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000081a0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+000081b0: 2822 4669 6e6e 6973 6822 290d 0a20 2020  ("Finnish")..   
+000081c0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+000081d0: 616d 6573 2e61 7070 656e 6428 2246 7265  ames.append("Fre
+000081e0: 6e63 6822 290d 0a20 2020 2020 2020 2073  nch")..        s
+000081f0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008200: 7070 656e 6428 2246 7269 7369 616e 2229  ppend("Frisian")
+00008210: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008220: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008230: 2822 4761 6c69 6369 616e 2229 0d0a 2020  ("Galician")..  
+00008240: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008250: 6e61 6d65 732e 6170 7065 6e64 2822 4765  names.append("Ge
+00008260: 6f72 6769 616e 2229 0d0a 2020 2020 2020  orgian")..      
+00008270: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00008280: 732e 6170 7065 6e64 2822 4765 726d 616e  s.append("German
+00008290: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000082a0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+000082b0: 6e64 2822 4772 6565 6b22 290d 0a20 2020  nd("Greek")..   
+000082c0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+000082d0: 616d 6573 2e61 7070 656e 6428 2247 7561  ames.append("Gua
+000082e0: 7261 6e69 2229 0d0a 2020 2020 2020 2020  rani")..        
+000082f0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008300: 6170 7065 6e64 2822 4775 6a61 7261 7469  append("Gujarati
+00008310: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008320: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00008330: 6e64 2822 4861 6974 6961 6e20 4372 656f  nd("Haitian Creo
+00008340: 6c65 2229 0d0a 2020 2020 2020 2020 7365  le")..        se
+00008350: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008360: 7065 6e64 2822 4861 7573 6122 290d 0a20  pend("Hausa").. 
+00008370: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00008380: 5f6e 616d 6573 2e61 7070 656e 6428 2248  _names.append("H
+00008390: 6177 6169 6961 6e22 290d 0a20 2020 2020  awaiian")..     
+000083a0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+000083b0: 6573 2e61 7070 656e 6428 2248 6562 7265  es.append("Hebre
+000083c0: 7722 290d 0a20 2020 2020 2020 2073 656c  w")..        sel
+000083d0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+000083e0: 656e 6428 2248 696e 6469 2229 0d0a 2020  end("Hindi")..  
+000083f0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008400: 6e61 6d65 732e 6170 7065 6e64 2822 486d  names.append("Hm
+00008410: 6f6e 6722 290d 0a20 2020 2020 2020 2073  ong")..        s
+00008420: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008430: 7070 656e 6428 2248 756e 6761 7269 616e  ppend("Hungarian
+00008440: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008450: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00008460: 6e64 2822 4963 656c 616e 6469 6322 290d  nd("Icelandic").
+00008470: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00008480: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00008490: 2249 6762 6f22 290d 0a20 2020 2020 2020  "Igbo")..       
+000084a0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+000084b0: 2e61 7070 656e 6428 2249 6c6f 6361 6e6f  .append("Ilocano
+000084c0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000084d0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+000084e0: 6e64 2822 496e 646f 6e65 7369 616e 2229  nd("Indonesian")
+000084f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008500: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008510: 2822 4972 6973 6822 290d 0a20 2020 2020  ("Irish")..     
+00008520: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00008530: 6573 2e61 7070 656e 6428 2249 7461 6c69  es.append("Itali
+00008540: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
+00008550: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008560: 7065 6e64 2822 4a61 7061 6e65 7365 2229  pend("Japanese")
+00008570: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008580: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008590: 2822 4a61 7661 6e65 7365 2229 0d0a 2020  ("Javanese")..  
+000085a0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000085b0: 6e61 6d65 732e 6170 7065 6e64 2822 4b61  names.append("Ka
+000085c0: 6e6e 6164 6122 290d 0a20 2020 2020 2020  nnada")..       
+000085d0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+000085e0: 2e61 7070 656e 6428 224b 617a 616b 6822  .append("Kazakh"
+000085f0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008600: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008610: 6428 224b 686d 6572 2229 0d0a 2020 2020  d("Khmer")..    
+00008620: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008630: 6d65 732e 6170 7065 6e64 2822 4b69 6e79  mes.append("Kiny
+00008640: 6172 7761 6e64 6122 290d 0a20 2020 2020  arwanda")..     
+00008650: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00008660: 6573 2e61 7070 656e 6428 224b 6f6e 6b61  es.append("Konka
+00008670: 6e69 2229 0d0a 2020 2020 2020 2020 7365  ni")..        se
+00008680: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008690: 7065 6e64 2822 4b6f 7265 616e 2229 0d0a  pend("Korean")..
+000086a0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000086b0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000086c0: 4b72 696f 2229 0d0a 2020 2020 2020 2020  Krio")..        
+000086d0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+000086e0: 6170 7065 6e64 2822 4b75 7264 6973 6820  append("Kurdish 
+000086f0: 284b 7572 6d61 6e6a 6929 2229 0d0a 2020  (Kurmanji)")..  
+00008700: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008710: 6e61 6d65 732e 6170 7065 6e64 2822 4b75  names.append("Ku
+00008720: 7264 6973 6820 2853 6f72 616e 6929 2229  rdish (Sorani)")
+00008730: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008740: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008750: 2822 4b79 7267 797a 2229 0d0a 2020 2020  ("Kyrgyz")..    
+00008760: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008770: 6d65 732e 6170 7065 6e64 2822 4c61 6f22  mes.append("Lao"
+00008780: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008790: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+000087a0: 6428 224c 6174 696e 2229 0d0a 2020 2020  d("Latin")..    
+000087b0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+000087c0: 6d65 732e 6170 7065 6e64 2822 4c61 7476  mes.append("Latv
+000087d0: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
+000087e0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+000087f0: 7070 656e 6428 224c 696e 6761 6c61 2229  ppend("Lingala")
+00008800: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008810: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008820: 2822 4c69 7468 7561 6e69 616e 2229 0d0a  ("Lithuanian")..
+00008830: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00008840: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00008850: 4c75 6761 6e64 6122 290d 0a20 2020 2020  Luganda")..     
+00008860: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00008870: 6573 2e61 7070 656e 6428 224c 7578 656d  es.append("Luxem
+00008880: 626f 7572 6769 7368 2229 0d0a 2020 2020  bourgish")..    
+00008890: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+000088a0: 6d65 732e 6170 7065 6e64 2822 4d61 6365  mes.append("Mace
+000088b0: 646f 6e69 616e 2229 0d0a 2020 2020 2020  donian")..      
+000088c0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+000088d0: 732e 6170 7065 6e64 2822 4d61 6c61 6761  s.append("Malaga
+000088e0: 7379 2229 0d0a 2020 2020 2020 2020 7365  sy")..        se
+000088f0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008900: 7065 6e64 2822 4d61 6c61 7922 290d 0a20  pend("Malay").. 
+00008910: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00008920: 5f6e 616d 6573 2e61 7070 656e 6428 224d  _names.append("M
+00008930: 616c 6179 616c 616d 2229 0d0a 2020 2020  alayalam")..    
+00008940: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008950: 6d65 732e 6170 7065 6e64 2822 4d61 6c74  mes.append("Malt
+00008960: 6573 6522 290d 0a20 2020 2020 2020 2073  ese")..        s
+00008970: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008980: 7070 656e 6428 224d 616f 7269 2229 0d0a  ppend("Maori")..
+00008990: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000089a0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000089b0: 4d61 7261 7468 6922 290d 0a20 2020 2020  Marathi")..     
+000089c0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+000089d0: 6573 2e61 7070 656e 6428 224d 6569 7465  es.append("Meite
+000089e0: 696c 6f6e 2028 4d61 6e69 7075 7269 2922  ilon (Manipuri)"
+000089f0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008a00: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008a10: 6428 224d 697a 6f22 290d 0a20 2020 2020  d("Mizo")..     
+00008a20: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00008a30: 6573 2e61 7070 656e 6428 224d 6f6e 676f  es.append("Mongo
+00008a40: 6c69 616e 2229 0d0a 2020 2020 2020 2020  lian")..        
+00008a50: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008a60: 6170 7065 6e64 2822 4d79 616e 6d61 7220  append("Myanmar 
+00008a70: 2842 7572 6d65 7365 2922 290d 0a20 2020  (Burmese)")..   
+00008a80: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00008a90: 616d 6573 2e61 7070 656e 6428 224e 6570  ames.append("Nep
+00008aa0: 616c 6922 290d 0a20 2020 2020 2020 2073  ali")..        s
+00008ab0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008ac0: 7070 656e 6428 224e 6f72 7765 6769 616e  ppend("Norwegian
+00008ad0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008ae0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00008af0: 6e64 2822 4f64 6979 6120 284f 7269 7961  nd("Odiya (Oriya
+00008b00: 2922 290d 0a20 2020 2020 2020 2073 656c  )")..        sel
+00008b10: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00008b20: 656e 6428 224f 726f 6d6f 2229 0d0a 2020  end("Oromo")..  
+00008b30: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008b40: 6e61 6d65 732e 6170 7065 6e64 2822 5061  names.append("Pa
+00008b50: 7368 746f 2229 0d0a 2020 2020 2020 2020  shto")..        
+00008b60: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008b70: 6170 7065 6e64 2822 5065 7273 6961 6e22  append("Persian"
+00008b80: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008b90: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008ba0: 6428 2250 6f6c 6973 6822 290d 0a20 2020  d("Polish")..   
+00008bb0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00008bc0: 616d 6573 2e61 7070 656e 6428 2250 6f72  ames.append("Por
+00008bd0: 7475 6775 6573 6522 290d 0a20 2020 2020  tuguese")..     
+00008be0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00008bf0: 6573 2e61 7070 656e 6428 2250 756e 6a61  es.append("Punja
+00008c00: 6269 2229 0d0a 2020 2020 2020 2020 7365  bi")..        se
+00008c10: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008c20: 7065 6e64 2822 5175 6563 6875 6122 290d  pend("Quechua").
+00008c30: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00008c40: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00008c50: 2252 6f6d 616e 6961 6e22 290d 0a20 2020  "Romanian")..   
+00008c60: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00008c70: 616d 6573 2e61 7070 656e 6428 2252 7573  ames.append("Rus
+00008c80: 7369 616e 2229 0d0a 2020 2020 2020 2020  sian")..        
+00008c90: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008ca0: 6170 7065 6e64 2822 5361 6d6f 616e 2229  append("Samoan")
+00008cb0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008cc0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008cd0: 2822 5361 6e73 6b72 6974 2229 0d0a 2020  ("Sanskrit")..  
+00008ce0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008cf0: 6e61 6d65 732e 6170 7065 6e64 2822 5363  names.append("Sc
+00008d00: 6f74 7320 4761 656c 6963 2229 0d0a 2020  ots Gaelic")..  
+00008d10: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008d20: 6e61 6d65 732e 6170 7065 6e64 2822 5365  names.append("Se
+00008d30: 7065 6469 2229 0d0a 2020 2020 2020 2020  pedi")..        
+00008d40: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008d50: 6170 7065 6e64 2822 5365 7262 6961 6e22  append("Serbian"
+00008d60: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008d70: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008d80: 6428 2253 6573 6f74 686f 2229 0d0a 2020  d("Sesotho")..  
+00008d90: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008da0: 6e61 6d65 732e 6170 7065 6e64 2822 5368  names.append("Sh
+00008db0: 6f6e 6122 290d 0a20 2020 2020 2020 2073  ona")..        s
+00008dc0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008dd0: 7070 656e 6428 2253 696e 6468 6922 290d  ppend("Sindhi").
+00008de0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00008df0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00008e00: 2253 696e 6861 6c61 2229 0d0a 2020 2020  "Sinhala")..    
+00008e10: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008e20: 6d65 732e 6170 7065 6e64 2822 536c 6f76  mes.append("Slov
+00008e30: 616b 2229 0d0a 2020 2020 2020 2020 7365  ak")..        se
+00008e40: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008e50: 7065 6e64 2822 536c 6f76 656e 6961 6e22  pend("Slovenian"
+00008e60: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008e70: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008e80: 6428 2253 6f6d 616c 6922 290d 0a20 2020  d("Somali")..   
+00008e90: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00008ea0: 616d 6573 2e61 7070 656e 6428 2253 7061  ames.append("Spa
+00008eb0: 6e69 7368 2229 0d0a 2020 2020 2020 2020  nish")..        
+00008ec0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008ed0: 6170 7065 6e64 2822 5375 6e64 616e 6573  append("Sundanes
+00008ee0: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
+00008ef0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00008f00: 656e 6428 2253 7761 6869 6c69 2229 0d0a  end("Swahili")..
+00008f10: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00008f20: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00008f30: 5377 6564 6973 6822 290d 0a20 2020 2020  Swedish")..     
+00008f40: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00008f50: 6573 2e61 7070 656e 6428 2254 616a 696b  es.append("Tajik
+00008f60: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008f70: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00008f80: 6e64 2822 5461 6d69 6c22 290d 0a20 2020  nd("Tamil")..   
+00008f90: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00008fa0: 616d 6573 2e61 7070 656e 6428 2254 6174  ames.append("Tat
+00008fb0: 6172 2229 0d0a 2020 2020 2020 2020 7365  ar")..        se
+00008fc0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008fd0: 7065 6e64 2822 5465 6c75 6775 2229 0d0a  pend("Telugu")..
+00008fe0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00008ff0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00009000: 5468 6169 2229 0d0a 2020 2020 2020 2020  Thai")..        
+00009010: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00009020: 6170 7065 6e64 2822 5469 6772 696e 7961  append("Tigrinya
+00009030: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00009040: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00009050: 6e64 2822 5473 6f6e 6761 2229 0d0a 2020  nd("Tsonga")..  
+00009060: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00009070: 6e61 6d65 732e 6170 7065 6e64 2822 5475  names.append("Tu
+00009080: 726b 6973 6822 290d 0a20 2020 2020 2020  rkish")..       
+00009090: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+000090a0: 2e61 7070 656e 6428 2254 7572 6b6d 656e  .append("Turkmen
+000090b0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000090c0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+000090d0: 6e64 2822 5477 6920 2841 6b61 6e29 2229  nd("Twi (Akan)")
+000090e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000090f0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00009100: 2822 556b 7261 696e 6961 6e22 290d 0a20  ("Ukrainian").. 
+00009110: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00009120: 5f6e 616d 6573 2e61 7070 656e 6428 2255  _names.append("U
+00009130: 7264 7522 290d 0a20 2020 2020 2020 2073  rdu")..        s
+00009140: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00009150: 7070 656e 6428 2255 7967 6875 7222 290d  ppend("Uyghur").
+00009160: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00009170: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00009180: 2255 7a62 656b 2229 0d0a 2020 2020 2020  "Uzbek")..      
+00009190: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+000091a0: 732e 6170 7065 6e64 2822 5669 6574 6e61  s.append("Vietna
+000091b0: 6d65 7365 2229 0d0a 2020 2020 2020 2020  mese")..        
+000091c0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+000091d0: 6170 7065 6e64 2822 5765 6c73 6822 290d  append("Welsh").
+000091e0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000091f0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00009200: 2258 686f 7361 2229 0d0a 2020 2020 2020  "Xhosa")..      
+00009210: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00009220: 732e 6170 7065 6e64 2822 5969 6464 6973  s.append("Yiddis
+00009230: 6822 290d 0a20 2020 2020 2020 2073 656c  h")..        sel
+00009240: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00009250: 656e 6428 2259 6f72 7562 6122 290d 0a20  end("Yoruba").. 
+00009260: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00009270: 5f6e 616d 6573 2e61 7070 656e 6428 225a  _names.append("Z
+00009280: 756c 7522 290d 0a0d 0a20 2020 2020 2020  ulu")....       
+00009290: 2073 656c 662e 636f 6465 5f6f 665f 6e61   self.code_of_na
+000092a0: 6d65 203d 2064 6963 7428 7a69 7028 7365  me = dict(zip(se
+000092b0: 6c66 2e6c 6973 745f 6e61 6d65 732c 2073  lf.list_names, s
+000092c0: 656c 662e 6c69 7374 5f63 6f64 6573 2929  elf.list_codes))
+000092d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
+000092e0: 616d 655f 6f66 5f63 6f64 6520 3d20 6469  ame_of_code = di
+000092f0: 6374 287a 6970 2873 656c 662e 6c69 7374  ct(zip(self.list
+00009300: 5f63 6f64 6573 2c20 7365 6c66 2e6c 6973  _codes, self.lis
+00009310: 745f 6e61 6d65 7329 290d 0a0d 0a20 2020  t_names))....   
+00009320: 2020 2020 2073 656c 662e 6469 6374 203d       self.dict =
+00009330: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00009340: 2020 2020 2020 2020 2020 2020 2761 6627              'af'
+00009350: 3a20 2741 6672 696b 6161 6e73 272c 0d0a  : 'Afrikaans',..
+00009360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009370: 2020 2020 2020 2020 2773 7127 3a20 2741          'sq': 'A
+00009380: 6c62 616e 6961 6e27 2c0d 0a20 2020 2020  lbanian',..     
+00009390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093a0: 2020 2027 616d 273a 2027 416d 6861 7269     'am': 'Amhari
+000093b0: 6327 2c0d 0a20 2020 2020 2020 2020 2020  c',..           
+000093c0: 2020 2020 2020 2020 2020 2020 2027 6172               'ar
+000093d0: 273a 2027 4172 6162 6963 272c 0d0a 2020  ': 'Arabic',..  
+000093e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093f0: 2020 2020 2020 2768 7927 3a20 2741 726d        'hy': 'Arm
+00009400: 656e 6961 6e27 2c0d 0a20 2020 2020 2020  enian',..       
+00009410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009420: 2027 6173 273a 2027 4173 7361 6d65 7365   'as': 'Assamese
+00009430: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00009440: 2020 2020 2020 2020 2020 2020 2761 7927              'ay'
+00009450: 3a20 2741 796d 6172 6127 2c0d 0a20 2020  : 'Aymara',..   
+00009460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009470: 2020 2020 2027 617a 273a 2027 417a 6572       'az': 'Azer
+00009480: 6261 696a 616e 6927 2c0d 0a20 2020 2020  baijani',..     
+00009490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094a0: 2020 2027 626d 273a 2027 4261 6d62 6172     'bm': 'Bambar
+000094b0: 6127 2c0d 0a20 2020 2020 2020 2020 2020  a',..           
+000094c0: 2020 2020 2020 2020 2020 2020 2027 6575               'eu
+000094d0: 273a 2027 4261 7371 7565 272c 0d0a 2020  ': 'Basque',..  
+000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094f0: 2020 2020 2020 2762 6527 3a20 2742 656c        'be': 'Bel
+00009500: 6172 7573 6961 6e27 2c0d 0a20 2020 2020  arusian',..     
+00009510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009520: 2020 2027 626e 273a 2027 4265 6e67 616c     'bn': 'Bengal
+00009530: 6927 2c0d 0a20 2020 2020 2020 2020 2020  i',..           
+00009540: 2020 2020 2020 2020 2020 2020 2027 6268               'bh
+00009550: 6f27 3a20 2742 686f 6a70 7572 6927 2c0d  o': 'Bhojpuri',.
+00009560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009570: 2020 2020 2020 2020 2027 6273 273a 2027           'bs': '
+00009580: 426f 736e 6961 6e27 2c0d 0a20 2020 2020  Bosnian',..     
+00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095a0: 2020 2027 6267 273a 2027 4275 6c67 6172     'bg': 'Bulgar
+000095b0: 6961 6e27 2c0d 0a20 2020 2020 2020 2020  ian',..         
+000095c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000095d0: 6361 273a 2027 4361 7461 6c61 6e27 2c0d  ca': 'Catalan',.
+000095e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000095f0: 2020 2020 2020 2020 2027 6365 6227 3a20           'ceb': 
+00009600: 2743 6562 7561 6e6f 272c 0d0a 2020 2020  'Cebuano',..    
+00009610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009620: 2020 2020 276e 7927 3a20 2743 6869 6368      'ny': 'Chich
+00009630: 6577 6127 2c0d 0a20 2020 2020 2020 2020  ewa',..         
+00009640: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009650: 7a68 2d43 4e27 3a20 2743 6869 6e65 7365  zh-CN': 'Chinese
+00009660: 2028 5369 6d70 6c69 6669 6564 2927 2c0d   (Simplified)',.
+00009670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009680: 2020 2020 2020 2020 2027 7a68 2d54 5727           'zh-TW'
+00009690: 3a20 2743 6869 6e65 7365 2028 5472 6164  : 'Chinese (Trad
+000096a0: 6974 696f 6e61 6c29 272c 0d0a 2020 2020  itional)',..    
+000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096c0: 2020 2020 2763 6f27 3a20 2743 6f72 7369      'co': 'Corsi
+000096d0: 6361 6e27 2c0d 0a20 2020 2020 2020 2020  can',..         
+000096e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000096f0: 6872 273a 2027 4372 6f61 7469 616e 272c  hr': 'Croatian',
+00009700: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009710: 2020 2020 2020 2020 2020 2763 7327 3a20            'cs': 
+00009720: 2743 7a65 6368 272c 0d0a 2020 2020 2020  'Czech',..      
+00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009740: 2020 2764 6127 3a20 2744 616e 6973 6827    'da': 'Danish'
+00009750: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009760: 2020 2020 2020 2020 2020 2027 6476 273a             'dv':
+00009770: 2027 4468 6976 6568 6927 2c0d 0a20 2020   'Dhivehi',..   
+00009780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009790: 2020 2020 2027 646f 6927 3a20 2744 6f67       'doi': 'Dog
+000097a0: 7269 272c 0d0a 2020 2020 2020 2020 2020  ri',..          
+000097b0: 2020 2020 2020 2020 2020 2020 2020 276e                'n
+000097c0: 6c27 3a20 2744 7574 6368 272c 0d0a 2020  l': 'Dutch',..  
+000097d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097e0: 2020 2020 2020 2765 6e27 3a20 2745 6e67        'en': 'Eng
+000097f0: 6c69 7368 272c 0d0a 2020 2020 2020 2020  lish',..        
+00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009810: 2765 6f27 3a20 2745 7370 6572 616e 746f  'eo': 'Esperanto
+00009820: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00009830: 2020 2020 2020 2020 2020 2020 2765 7427              'et'
+00009840: 3a20 2745 7374 6f6e 6961 6e27 2c0d 0a20  : 'Estonian',.. 
+00009850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009860: 2020 2020 2020 2027 6565 273a 2027 4577         'ee': 'Ew
+00009870: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
+00009880: 2020 2020 2020 2020 2020 2020 2027 6669               'fi
+00009890: 6c27 3a20 2746 696c 6970 696e 6f27 2c0d  l': 'Filipino',.
+000098a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000098b0: 2020 2020 2020 2020 2027 6669 273a 2027           'fi': '
+000098c0: 4669 6e6e 6973 6827 2c0d 0a20 2020 2020  Finnish',..     
+000098d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098e0: 2020 2027 6672 273a 2027 4672 656e 6368     'fr': 'French
+000098f0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00009900: 2020 2020 2020 2020 2020 2020 2766 7927              'fy'
+00009910: 3a20 2746 7269 7369 616e 272c 0d0a 2020  : 'Frisian',..  
+00009920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009930: 2020 2020 2020 2767 6c27 3a20 2747 616c        'gl': 'Gal
+00009940: 6963 6961 6e27 2c0d 0a20 2020 2020 2020  ician',..       
+00009950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009960: 2027 6b61 273a 2027 4765 6f72 6769 616e   'ka': 'Georgian
+00009970: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00009980: 2020 2020 2020 2020 2020 2020 2764 6527              'de'
+00009990: 3a20 2747 6572 6d61 6e27 2c0d 0a20 2020  : 'German',..   
+000099a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099b0: 2020 2020 2027 656c 273a 2027 4772 6565       'el': 'Gree
+000099c0: 6b27 2c0d 0a20 2020 2020 2020 2020 2020  k',..           
+000099d0: 2020 2020 2020 2020 2020 2020 2027 676e               'gn
+000099e0: 273a 2027 4775 6172 616e 6927 2c0d 0a20  ': 'Guarani',.. 
+000099f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a00: 2020 2020 2020 2027 6775 273a 2027 4775         'gu': 'Gu
+00009a10: 6a61 7261 7469 272c 0d0a 2020 2020 2020  jarati',..      
+00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a30: 2020 2768 7427 3a20 2748 6169 7469 616e    'ht': 'Haitian
+00009a40: 2043 7265 6f6c 6527 2c0d 0a20 2020 2020   Creole',..     
+00009a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a60: 2020 2027 6861 273a 2027 4861 7573 6127     'ha': 'Hausa'
+00009a70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009a80: 2020 2020 2020 2020 2020 2027 6861 7727             'haw'
+00009a90: 3a20 2748 6177 6169 6961 6e27 2c0d 0a20  : 'Hawaiian',.. 
+00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ab0: 2020 2020 2020 2027 6865 273a 2027 4865         'he': 'He
+00009ac0: 6272 6577 272c 0d0a 2020 2020 2020 2020  brew',..        
+00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ae0: 2768 6927 3a20 2748 696e 6469 272c 0d0a  'hi': 'Hindi',..
+00009af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b00: 2020 2020 2020 2020 2768 6d6e 273a 2027          'hmn': '
+00009b10: 486d 6f6e 6727 2c0d 0a20 2020 2020 2020  Hmong',..       
+00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b30: 2027 6875 273a 2027 4875 6e67 6172 6961   'hu': 'Hungaria
+00009b40: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+00009b50: 2020 2020 2020 2020 2020 2020 2027 6973               'is
+00009b60: 273a 2027 4963 656c 616e 6469 6327 2c0d  ': 'Icelandic',.
+00009b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009b80: 2020 2020 2020 2020 2027 6967 273a 2027           'ig': '
+00009b90: 4967 626f 272c 0d0a 2020 2020 2020 2020  Igbo',..        
+00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bb0: 2769 6c6f 273a 2027 496c 6f63 616e 6f27  'ilo': 'Ilocano'
+00009bc0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009bd0: 2020 2020 2020 2020 2020 2027 6964 273a             'id':
+00009be0: 2027 496e 646f 6e65 7369 616e 272c 0d0a   'Indonesian',..
+00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c00: 2020 2020 2020 2020 2767 6127 3a20 2749          'ga': 'I
+00009c10: 7269 7368 272c 0d0a 2020 2020 2020 2020  rish',..        
+00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c30: 2769 7427 3a20 2749 7461 6c69 616e 272c  'it': 'Italian',
+00009c40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009c50: 2020 2020 2020 2020 2020 276a 6127 3a20            'ja': 
+00009c60: 274a 6170 616e 6573 6527 2c0d 0a20 2020  'Japanese',..   
+00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c80: 2020 2020 2027 6a76 273a 2027 4a61 7661       'jv': 'Java
+00009c90: 6e65 7365 272c 0d0a 2020 2020 2020 2020  nese',..        
+00009ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cb0: 276b 6e27 3a20 274b 616e 6e61 6461 272c  'kn': 'Kannada',
+00009cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009cd0: 2020 2020 2020 2020 2020 276b 6b27 3a20            'kk': 
+00009ce0: 274b 617a 616b 6827 2c0d 0a20 2020 2020  'Kazakh',..     
+00009cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d00: 2020 2027 6b6d 273a 2027 4b68 6d65 7227     'km': 'Khmer'
+00009d10: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009d20: 2020 2020 2020 2020 2020 2027 7277 273a             'rw':
+00009d30: 2027 4b69 6e79 6172 7761 6e64 6127 2c0d   'Kinyarwanda',.
+00009d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009d50: 2020 2020 2020 2020 2027 676f 6d27 3a20           'gom': 
+00009d60: 274b 6f6e 6b61 6e69 272c 0d0a 2020 2020  'Konkani',..    
+00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d80: 2020 2020 276b 6f27 3a20 274b 6f72 6561      'ko': 'Korea
+00009d90: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+00009da0: 2020 2020 2020 2020 2020 2020 2027 6b72               'kr
+00009db0: 6927 3a20 274b 7269 6f27 2c0d 0a20 2020  i': 'Krio',..   
+00009dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009dd0: 2020 2020 2027 6b6d 7227 3a20 274b 7572       'kmr': 'Kur
+00009de0: 6469 7368 2028 4b75 726d 616e 6a69 2927  dish (Kurmanji)'
+00009df0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009e00: 2020 2020 2020 2020 2020 2027 636b 6227             'ckb'
+00009e10: 3a20 274b 7572 6469 7368 2028 536f 7261  : 'Kurdish (Sora
+00009e20: 6e69 2927 2c0d 0a20 2020 2020 2020 2020  ni)',..         
+00009e30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009e40: 6b79 273a 2027 4b79 7267 797a 272c 0d0a  ky': 'Kyrgyz',..
+00009e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e60: 2020 2020 2020 2020 276c 6f27 3a20 274c          'lo': 'L
+00009e70: 616f 272c 0d0a 2020 2020 2020 2020 2020  ao',..          
+00009e80: 2020 2020 2020 2020 2020 2020 2020 276c                'l
+00009e90: 6127 3a20 274c 6174 696e 272c 0d0a 2020  a': 'Latin',..  
+00009ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009eb0: 2020 2020 2020 276c 7627 3a20 274c 6174        'lv': 'Lat
+00009ec0: 7669 616e 272c 0d0a 2020 2020 2020 2020  vian',..        
+00009ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ee0: 276c 6e27 3a20 274c 696e 6761 6c61 272c  'ln': 'Lingala',
+00009ef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009f00: 2020 2020 2020 2020 2020 276c 7427 3a20            'lt': 
+00009f10: 274c 6974 6875 616e 6961 6e27 2c0d 0a20  'Lithuanian',.. 
+00009f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f30: 2020 2020 2020 2027 6c67 273a 2027 4c75         'lg': 'Lu
+00009f40: 6761 6e64 6127 2c0d 0a20 2020 2020 2020  ganda',..       
+00009f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f60: 2027 6c62 273a 2027 4c75 7865 6d62 6f75   'lb': 'Luxembou
+00009f70: 7267 6973 6827 2c0d 0a20 2020 2020 2020  rgish',..       
+00009f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f90: 2027 6d6b 273a 2027 4d61 6365 646f 6e69   'mk': 'Macedoni
+00009fa0: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
+00009fb0: 2020 2020 2020 2020 2020 2020 2020 276d                'm
+00009fc0: 6727 3a20 274d 616c 6167 6173 7927 2c0d  g': 'Malagasy',.
+00009fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009fe0: 2020 2020 2020 2020 2027 6d73 273a 2027           'ms': '
+00009ff0: 4d61 6c61 7927 2c0d 0a20 2020 2020 2020  Malay',..       
+0000a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a010: 2027 6d6c 273a 2027 4d61 6c61 7961 6c61   'ml': 'Malayala
+0000a020: 6d27 2c0d 0a20 2020 2020 2020 2020 2020  m',..           
+0000a030: 2020 2020 2020 2020 2020 2020 2027 6d74               'mt
+0000a040: 273a 2027 4d61 6c74 6573 6527 2c0d 0a20  ': 'Maltese',.. 
 0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a060: 2020 2020 2020 2027 6c75 7327 3a20 274d         'lus': 'M
-0000a070: 697a 6f27 2c0d 0a20 2020 2020 2020 2020  izo',..         
+0000a060: 2020 2020 2020 2027 6d69 273a 2027 4d61         'mi': 'Ma
+0000a070: 6f72 6927 2c0d 0a20 2020 2020 2020 2020  ori',..         
 0000a080: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a090: 6d6e 273a 2027 4d6f 6e67 6f6c 6961 6e27  mn': 'Mongolian'
-0000a0a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a0b0: 2020 2020 2020 2020 2020 2027 6d79 273a             'my':
-0000a0c0: 2027 4d79 616e 6d61 7220 2842 7572 6d65   'Myanmar (Burme
-0000a0d0: 7365 2927 2c0d 0a20 2020 2020 2020 2020  se)',..         
-0000a0e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a0f0: 6e65 273a 2027 4e65 7061 6c69 272c 0d0a  ne': 'Nepali',..
-0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a110: 2020 2020 2020 2020 276e 6f27 3a20 274e          'no': 'N
-0000a120: 6f72 7765 6769 616e 272c 0d0a 2020 2020  orwegian',..    
-0000a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a140: 2020 2020 276f 7227 3a20 274f 6469 7961      'or': 'Odiya
-0000a150: 2028 4f72 6979 6129 272c 0d0a 2020 2020   (Oriya)',..    
-0000a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a170: 2020 2020 276f 6d27 3a20 274f 726f 6d6f      'om': 'Oromo
-0000a180: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-0000a190: 2020 2020 2020 2020 2020 2020 2770 7327              'ps'
-0000a1a0: 3a20 2750 6173 6874 6f27 2c0d 0a20 2020  : 'Pashto',..   
-0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1c0: 2020 2020 2027 6661 273a 2027 5065 7273       'fa': 'Pers
-0000a1d0: 6961 6e27 2c0d 0a20 2020 2020 2020 2020  ian',..         
-0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a1f0: 706c 273a 2027 506f 6c69 7368 272c 0d0a  pl': 'Polish',..
-0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a210: 2020 2020 2020 2020 2770 7427 3a20 2750          'pt': 'P
-0000a220: 6f72 7475 6775 6573 6527 2c0d 0a20 2020  ortuguese',..   
-0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a240: 2020 2020 2027 7061 273a 2027 5075 6e6a       'pa': 'Punj
-0000a250: 6162 6927 2c0d 0a20 2020 2020 2020 2020  abi',..         
-0000a260: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a270: 7175 273a 2027 5175 6563 6875 6127 2c0d  qu': 'Quechua',.
-0000a280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a290: 2020 2020 2020 2020 2027 726f 273a 2027           'ro': '
-0000a2a0: 526f 6d61 6e69 616e 272c 0d0a 2020 2020  Romanian',..    
-0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2c0: 2020 2020 2772 7527 3a20 2752 7573 7369      'ru': 'Russi
-0000a2d0: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
-0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-0000a2f0: 6d27 3a20 2753 616d 6f61 6e27 2c0d 0a20  m': 'Samoan',.. 
-0000a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a310: 2020 2020 2020 2027 7361 273a 2027 5361         'sa': 'Sa
-0000a320: 6e73 6b72 6974 272c 0d0a 2020 2020 2020  nskrit',..      
-0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a340: 2020 2767 6427 3a20 2753 636f 7473 2047    'gd': 'Scots G
-0000a350: 6165 6c69 6327 2c0d 0a20 2020 2020 2020  aelic',..       
-0000a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a370: 2027 6e73 6f27 3a20 2753 6570 6564 6927   'nso': 'Sepedi'
-0000a380: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a390: 2020 2020 2020 2020 2020 2027 7372 273a             'sr':
-0000a3a0: 2027 5365 7262 6961 6e27 2c0d 0a20 2020   'Serbian',..   
-0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3c0: 2020 2020 2027 7374 273a 2027 5365 736f       'st': 'Seso
-0000a3d0: 7468 6f27 2c0d 0a20 2020 2020 2020 2020  tho',..         
-0000a3e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a3f0: 736e 273a 2027 5368 6f6e 6127 2c0d 0a20  sn': 'Shona',.. 
-0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a410: 2020 2020 2020 2027 7364 273a 2027 5369         'sd': 'Si
-0000a420: 6e64 6869 272c 0d0a 2020 2020 2020 2020  ndhi',..        
-0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a440: 2773 6927 3a20 2753 696e 6861 6c61 272c  'si': 'Sinhala',
-0000a450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a460: 2020 2020 2020 2020 2020 2773 6b27 3a20            'sk': 
-0000a470: 2753 6c6f 7661 6b27 2c0d 0a20 2020 2020  'Slovak',..     
-0000a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a490: 2020 2027 736c 273a 2027 536c 6f76 656e     'sl': 'Sloven
-0000a4a0: 6961 6e27 2c0d 0a20 2020 2020 2020 2020  ian',..         
-0000a4b0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a4c0: 736f 273a 2027 536f 6d61 6c69 272c 0d0a  so': 'Somali',..
-0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4e0: 2020 2020 2020 2020 2765 7327 3a20 2753          'es': 'S
-0000a4f0: 7061 6e69 7368 272c 0d0a 2020 2020 2020  panish',..      
-0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a510: 2020 2773 7527 3a20 2753 756e 6461 6e65    'su': 'Sundane
-0000a520: 7365 272c 0d0a 2020 2020 2020 2020 2020  se',..          
-0000a530: 2020 2020 2020 2020 2020 2020 2020 2773                's
-0000a540: 7727 3a20 2753 7761 6869 6c69 272c 0d0a  w': 'Swahili',..
-0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a560: 2020 2020 2020 2020 2773 7627 3a20 2753          'sv': 'S
-0000a570: 7765 6469 7368 272c 0d0a 2020 2020 2020  wedish',..      
-0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a590: 2020 2774 6727 3a20 2754 616a 696b 272c    'tg': 'Tajik',
-0000a5a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a5b0: 2020 2020 2020 2020 2020 2774 6127 3a20            'ta': 
-0000a5c0: 2754 616d 696c 272c 0d0a 2020 2020 2020  'Tamil',..      
-0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5e0: 2020 2774 7427 3a20 2754 6174 6172 272c    'tt': 'Tatar',
-0000a5f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a600: 2020 2020 2020 2020 2020 2774 6527 3a20            'te': 
-0000a610: 2754 656c 7567 7527 2c0d 0a20 2020 2020  'Telugu',..     
-0000a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a630: 2020 2027 7468 273a 2027 5468 6169 272c     'th': 'Thai',
-0000a640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a650: 2020 2020 2020 2020 2020 2774 6927 3a20            'ti': 
-0000a660: 2754 6967 7269 6e79 6127 2c0d 0a20 2020  'Tigrinya',..   
-0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a680: 2020 2020 2027 7473 273a 2027 5473 6f6e       'ts': 'Tson
-0000a690: 6761 272c 0d0a 2020 2020 2020 2020 2020  ga',..          
-0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2774                't
-0000a6b0: 7227 3a20 2754 7572 6b69 7368 272c 0d0a  r': 'Turkish',..
-0000a6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6d0: 2020 2020 2020 2020 2774 6b27 3a20 2754          'tk': 'T
-0000a6e0: 7572 6b6d 656e 272c 0d0a 2020 2020 2020  urkmen',..      
-0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a700: 2020 2774 7727 3a20 2754 7769 2028 416b    'tw': 'Twi (Ak
-0000a710: 616e 2927 2c0d 0a20 2020 2020 2020 2020  an)',..         
-0000a720: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a730: 756b 273a 2027 556b 7261 696e 6961 6e27  uk': 'Ukrainian'
-0000a740: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a750: 2020 2020 2020 2020 2020 2027 7572 273a             'ur':
-0000a760: 2027 5572 6475 272c 0d0a 2020 2020 2020   'Urdu',..      
-0000a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a780: 2020 2775 6727 3a20 2755 7967 6875 7227    'ug': 'Uyghur'
-0000a790: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a7a0: 2020 2020 2020 2020 2020 2027 757a 273a             'uz':
-0000a7b0: 2027 557a 6265 6b27 2c0d 0a20 2020 2020   'Uzbek',..     
-0000a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7d0: 2020 2027 7669 273a 2027 5669 6574 6e61     'vi': 'Vietna
-0000a7e0: 6d65 7365 272c 0d0a 2020 2020 2020 2020  mese',..        
-0000a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a800: 2763 7927 3a20 2757 656c 7368 272c 0d0a  'cy': 'Welsh',..
-0000a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a820: 2020 2020 2020 2020 2778 6827 3a20 2758          'xh': 'X
-0000a830: 686f 7361 272c 0d0a 2020 2020 2020 2020  hosa',..        
-0000a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a850: 2779 6927 3a20 2759 6964 6469 7368 272c  'yi': 'Yiddish',
-0000a860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a870: 2020 2020 2020 2020 2020 2779 6f27 3a20            'yo': 
-0000a880: 2759 6f72 7562 6127 2c0d 0a20 2020 2020  'Yoruba',..     
-0000a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8a0: 2020 2027 7a75 273a 2027 5a75 6c75 272c     'zu': 'Zulu',
-0000a8b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a8c0: 2020 2020 2020 7d0d 0a0d 0a20 2020 2064        }....    d
-0000a8d0: 6566 2067 6574 5f6e 616d 6528 7365 6c66  ef get_name(self
-0000a8e0: 2c20 6765 745f 636f 6465 293a 0d0a 2020  , get_code):..  
-0000a8f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000a900: 662e 6469 6374 2e67 6574 2867 6574 5f63  f.dict.get(get_c
-0000a910: 6f64 652e 6c6f 7765 7228 292c 2022 2229  ode.lower(), "")
-0000a920: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
-0000a930: 636f 6465 2873 656c 662c 206c 616e 6775  code(self, langu
-0000a940: 6167 6529 3a0d 0a20 2020 2020 2020 2066  age):..        f
-0000a950: 6f72 2067 6574 5f63 6f64 652c 206c 616e  or get_code, lan
-0000a960: 6720 696e 2073 656c 662e 6469 6374 2e69  g in self.dict.i
-0000a970: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-0000a980: 2020 2020 2069 6620 6c61 6e67 2e6c 6f77       if lang.low
-0000a990: 6572 2829 203d 3d20 6c61 6e67 7561 6765  er() == language
-0000a9a0: 2e6c 6f77 6572 2829 3a0d 0a20 2020 2020  .lower():..     
-0000a9b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000a9c0: 6e20 6765 745f 636f 6465 0d0a 2020 2020  n get_code..    
-0000a9d0: 2020 2020 7265 7475 726e 2022 220d 0a0d      return ""...
-0000a9e0: 0a0d 0a63 6c61 7373 2057 6176 436f 6e76  ...class WavConv
-0000a9f0: 6572 7465 723a 0d0a 2020 2020 4073 7461  erter:..    @sta
-0000aa00: 7469 636d 6574 686f 640d 0a20 2020 2064  ticmethod..    d
-0000aa10: 6566 2077 6869 6368 2870 726f 6772 616d  ef which(program
-0000aa20: 293a 0d0a 2020 2020 2020 2020 6465 6620  ):..        def 
-0000aa30: 6973 5f65 7865 2866 696c 655f 7061 7468  is_exe(file_path
-0000aa40: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000aa50: 7265 7475 726e 206f 732e 7061 7468 2e69  return os.path.i
-0000aa60: 7366 696c 6528 6669 6c65 5f70 6174 6829  sfile(file_path)
-0000aa70: 2061 6e64 206f 732e 6163 6365 7373 2866   and os.access(f
-0000aa80: 696c 655f 7061 7468 2c20 6f73 2e58 5f4f  ile_path, os.X_O
-0000aa90: 4b29 0d0a 2020 2020 2020 2020 6670 6174  K)..        fpat
-0000aaa0: 682c 205f 203d 206f 732e 7061 7468 2e73  h, _ = os.path.s
-0000aab0: 706c 6974 2870 726f 6772 616d 290d 0a20  plit(program).. 
-0000aac0: 2020 2020 2020 2069 6620 6670 6174 683a         if fpath:
-0000aad0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000aae0: 2069 735f 6578 6528 7072 6f67 7261 6d29   is_exe(program)
-0000aaf0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000ab00: 2020 2072 6574 7572 6e20 7072 6f67 7261     return progra
-0000ab10: 6d0d 0a20 2020 2020 2020 2065 6c73 653a  m..        else:
-0000ab20: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-0000ab30: 7220 7061 7468 2069 6e20 6f73 2e65 6e76  r path in os.env
-0000ab40: 6972 6f6e 5b22 5041 5448 225d 2e73 706c  iron["PATH"].spl
-0000ab50: 6974 286f 732e 7061 7468 7365 7029 3a0d  it(os.pathsep):.
-0000ab60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ab70: 2070 6174 6820 3d20 7061 7468 2e73 7472   path = path.str
-0000ab80: 6970 2827 2227 290d 0a20 2020 2020 2020  ip('"')..       
-0000ab90: 2020 2020 2020 2020 2065 7865 5f66 696c           exe_fil
-0000aba0: 6520 3d20 6f73 2e70 6174 682e 6a6f 696e  e = os.path.join
-0000abb0: 2870 6174 682c 2070 726f 6772 616d 290d  (path, program).
-0000abc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000abd0: 2069 6620 6973 5f65 7865 2865 7865 5f66   if is_exe(exe_f
-0000abe0: 696c 6529 3a0d 0a20 2020 2020 2020 2020  ile):..         
-0000abf0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000ac00: 6e20 6578 655f 6669 6c65 0d0a 2020 2020  n exe_file..    
-0000ac10: 2020 2020 7265 7475 726e 204e 6f6e 650d      return None.
-0000ac20: 0a0d 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
-0000ac30: 7468 6f64 0d0a 2020 2020 6465 6620 6666  thod..    def ff
-0000ac40: 6d70 6567 5f63 6865 636b 2829 3a0d 0a20  mpeg_check():.. 
-0000ac50: 2020 2020 2020 2069 6620 5761 7643 6f6e         if WavCon
-0000ac60: 7665 7274 6572 2e77 6869 6368 2822 6666  verter.which("ff
-0000ac70: 6d70 6567 2229 3a0d 0a20 2020 2020 2020  mpeg"):..       
-0000ac80: 2020 2020 2072 6574 7572 6e20 2266 666d       return "ffm
-0000ac90: 7065 6722 0d0a 2020 2020 2020 2020 6966  peg"..        if
-0000aca0: 2057 6176 436f 6e76 6572 7465 722e 7768   WavConverter.wh
-0000acb0: 6963 6828 2266 666d 7065 672e 6578 6522  ich("ffmpeg.exe"
-0000acc0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000acd0: 7265 7475 726e 2022 6666 6d70 6567 2e65  return "ffmpeg.e
-0000ace0: 7865 220d 0a20 2020 2020 2020 2072 6574  xe"..        ret
-0000acf0: 7572 6e20 4e6f 6e65 0d0a 0d0a 2020 2020  urn None....    
-0000ad00: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0000ad10: 662c 2063 6861 6e6e 656c 733d 312c 2072  f, channels=1, r
-0000ad20: 6174 653d 3438 3030 302c 2070 726f 6772  ate=48000, progr
-0000ad30: 6573 735f 6361 6c6c 6261 636b 3d4e 6f6e  ess_callback=Non
-0000ad40: 652c 2065 7272 6f72 5f6d 6573 7361 6765  e, error_message
-0000ad50: 735f 6361 6c6c 6261 636b 3d4e 6f6e 6529  s_callback=None)
-0000ad60: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-0000ad70: 6368 616e 6e65 6c73 203d 2063 6861 6e6e  channels = chann
-0000ad80: 656c 730d 0a20 2020 2020 2020 2073 656c  els..        sel
-0000ad90: 662e 7261 7465 203d 2072 6174 650d 0a20  f.rate = rate.. 
-0000ada0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000adb0: 7265 7373 5f63 616c 6c62 6163 6b20 3d20  ress_callback = 
-0000adc0: 7072 6f67 7265 7373 5f63 616c 6c62 6163  progress_callbac
-0000add0: 6b0d 0a20 2020 2020 2020 2073 656c 662e  k..        self.
-0000ade0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-0000adf0: 616c 6c62 6163 6b20 3d20 6572 726f 725f  allback = error_
-0000ae00: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000ae10: 6b0d 0a0d 0a20 2020 2064 6566 205f 5f63  k....    def __c
-0000ae20: 616c 6c5f 5f28 7365 6c66 2c20 6d65 6469  all__(self, medi
-0000ae30: 615f 6669 6c65 7061 7468 293a 0d0a 2020  a_filepath):..  
-0000ae40: 2020 2020 2020 7465 6d70 203d 2074 656d        temp = tem
-0000ae50: 7066 696c 652e 4e61 6d65 6454 656d 706f  pfile.NamedTempo
-0000ae60: 7261 7279 4669 6c65 2873 7566 6669 783d  raryFile(suffix=
-0000ae70: 272e 7761 7627 2c20 6465 6c65 7465 3d46  '.wav', delete=F
-0000ae80: 616c 7365 290d 0a20 2020 2020 2020 2069  alse)..        i
-0000ae90: 6620 6e6f 7420 6f73 2e70 6174 682e 6973  f not os.path.is
-0000aea0: 6669 6c65 286d 6564 6961 5f66 696c 6570  file(media_filep
-0000aeb0: 6174 6829 3a0d 0a20 2020 2020 2020 2020  ath):..         
-0000aec0: 2020 2069 6620 7365 6c66 2e65 7272 6f72     if self.error
-0000aed0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000aee0: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
-0000aef0: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
-0000af00: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000af10: 6b28 2254 6865 2067 6976 656e 2066 696c  k("The given fil
-0000af20: 6520 646f 6573 206e 6f74 2065 7869 7374  e does not exist
-0000af30: 3a20 7b30 7d22 2e66 6f72 6d61 7428 6d65  : {0}".format(me
-0000af40: 6469 615f 6669 6c65 7061 7468 2929 0d0a  dia_filepath))..
-0000af50: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000af60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000af70: 2020 2070 7269 6e74 2822 5468 6520 6769     print("The gi
-0000af80: 7665 6e20 6669 6c65 2064 6f65 7320 6e6f  ven file does no
-0000af90: 7420 6578 6973 743a 207b 307d 222e 666f  t exist: {0}".fo
-0000afa0: 726d 6174 286d 6564 6961 5f66 696c 6570  rmat(media_filep
-0000afb0: 6174 6829 290d 0a20 2020 2020 2020 2020  ath))..         
-0000afc0: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
-0000afd0: 6570 7469 6f6e 2822 496e 7661 6c69 6420  eption("Invalid 
-0000afe0: 6669 6c65 3a20 7b30 7d22 2e66 6f72 6d61  file: {0}".forma
-0000aff0: 7428 6d65 6469 615f 6669 6c65 7061 7468  t(media_filepath
-0000b000: 2929 0d0a 2020 2020 2020 2020 6966 206e  ))..        if n
-0000b010: 6f74 2073 656c 662e 6666 6d70 6567 5f63  ot self.ffmpeg_c
-0000b020: 6865 636b 2829 3a0d 0a20 2020 2020 2020  heck():..       
-0000b030: 2020 2020 2069 6620 7365 6c66 2e65 7272       if self.err
-0000b040: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-0000b050: 6261 636b 3a0d 0a20 2020 2020 2020 2020  back:..         
-0000b060: 2020 2020 2020 2073 656c 662e 6572 726f         self.erro
-0000b070: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000b080: 6163 6b28 2266 666d 7065 673a 2045 7865  ack("ffmpeg: Exe
-0000b090: 6375 7461 626c 6520 6e6f 7420 666f 756e  cutable not foun
-0000b0a0: 6420 6f6e 206d 6163 6869 6e65 2e22 290d  d on machine.").
-0000b0b0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000b0c0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000b0d0: 2020 2020 7072 696e 7428 2266 666d 7065      print("ffmpe
-0000b0e0: 673a 2045 7865 6375 7461 626c 6520 6e6f  g: Executable no
-0000b0f0: 7420 666f 756e 6420 6f6e 206d 6163 6869  t found on machi
-0000b100: 6e65 2e22 290d 0a20 2020 2020 2020 2020  ne.")..         
-0000b110: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
-0000b120: 6570 7469 6f6e 2822 4465 7065 6e64 656e  eption("Dependen
-0000b130: 6379 206e 6f74 2066 6f75 6e64 3a20 6666  cy not found: ff
-0000b140: 6d70 6567 2229 0d0a 0d0a 2020 2020 2020  mpeg")....      
-0000b150: 2020 636f 6d6d 616e 6420 3d20 5b0d 0a20    command = [.. 
-0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b170: 2020 2022 6666 6d70 6567 222c 0d0a 2020     "ffmpeg",..  
-0000b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b190: 2020 222d 7922 2c0d 0a20 2020 2020 2020    "-y",..       
-0000b1a0: 2020 2020 2020 2020 2020 2020 2022 2d69               "-i
-0000b1b0: 222c 206d 6564 6961 5f66 696c 6570 6174  ", media_filepat
-0000b1c0: 682c 0d0a 2020 2020 2020 2020 2020 2020  h,..            
-0000b1d0: 2020 2020 2020 2020 222d 6163 222c 2073          "-ac", s
-0000b1e0: 7472 2873 656c 662e 6368 616e 6e65 6c73  tr(self.channels
-0000b1f0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000b200: 2020 2020 2020 2020 222d 6172 222c 2073          "-ar", s
-0000b210: 7472 2873 656c 662e 7261 7465 292c 0d0a  tr(self.rate),..
-0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b230: 2020 2020 222d 6c6f 676c 6576 656c 222c      "-loglevel",
-0000b240: 2022 6572 726f 7222 2c0d 0a20 2020 2020   "error",..     
-0000b250: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000b260: 2d68 6964 655f 6261 6e6e 6572 222c 0d0a  -hide_banner",..
-0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b280: 2020 2020 7465 6d70 2e6e 616d 650d 0a20      temp.name.. 
-0000b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2a0: 205d 0d0a 0d0a 2020 2020 2020 2020 7472   ]....        tr
-0000b2b0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-0000b2c0: 2320 5255 4e4e 494e 4720 6666 6d70 6567  # RUNNING ffmpeg
-0000b2d0: 2057 4954 484f 5554 2053 484f 5749 4e47   WITHOUT SHOWING
-0000b2e0: 2050 524f 4752 4553 5353 0d0a 2020 2020   PROGRESSS..    
-0000b2f0: 2020 2020 2020 2020 2375 7365 5f73 6865          #use_she
-0000b300: 6c6c 203d 2054 7275 6520 6966 206f 732e  ll = True if os.
-0000b310: 6e61 6d65 203d 3d20 226e 7422 2065 6c73  name == "nt" els
-0000b320: 6520 4661 6c73 650d 0a20 2020 2020 2020  e False..       
-0000b330: 2020 2020 2023 7375 6270 726f 6365 7373       #subprocess
-0000b340: 2e63 6865 636b 5f6f 7574 7075 7428 636f  .check_output(co
-0000b350: 6d6d 616e 642c 2073 7464 696e 3d6f 7065  mmand, stdin=ope
-0000b360: 6e28 6f73 2e64 6576 6e75 6c6c 292c 2073  n(os.devnull), s
-0000b370: 6865 6c6c 3d75 7365 5f73 6865 6c6c 290d  hell=use_shell).
-0000b380: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
-0000b390: 2052 554e 4e49 4e47 2066 666d 7065 6720   RUNNING ffmpeg 
-0000b3a0: 5749 5448 2050 524f 4752 4553 5353 0d0a  WITH PROGRESSS..
-0000b3b0: 2020 2020 2020 2020 2020 2020 6666 203d              ff =
-0000b3c0: 2046 666d 7065 6750 726f 6772 6573 7328   FfmpegProgress(
-0000b3d0: 636f 6d6d 616e 6429 0d0a 2020 2020 2020  command)..      
-0000b3e0: 2020 2020 2020 7065 7263 656e 7461 6765        percentage
-0000b3f0: 203d 2030 0d0a 2020 2020 2020 2020 2020   = 0..          
-0000b400: 2020 666f 7220 7072 6f67 7265 7373 2069    for progress i
-0000b410: 6e20 6666 2e72 756e 5f63 6f6d 6d61 6e64  n ff.run_command
-0000b420: 5f77 6974 685f 7072 6f67 7265 7373 2829  _with_progress()
-0000b430: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000b440: 2020 2070 6572 6365 6e74 6167 6520 3d20     percentage = 
-0000b450: 7072 6f67 7265 7373 0d0a 2020 2020 2020  progress..      
-0000b460: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000b470: 662e 7072 6f67 7265 7373 5f63 616c 6c62  f.progress_callb
-0000b480: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
-0000b490: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000b4a0: 726f 6772 6573 735f 6361 6c6c 6261 636b  rogress_callback
-0000b4b0: 286d 6564 6961 5f66 696c 6570 6174 682c  (media_filepath,
-0000b4c0: 2070 6572 6365 6e74 6167 6529 0d0a 2020   percentage)..  
-0000b4d0: 2020 2020 2020 2020 2020 7465 6d70 2e63            temp.c
-0000b4e0: 6c6f 7365 2829 0d0a 0d0a 2020 2020 2020  lose()....      
-0000b4f0: 2020 2020 2020 7265 7475 726e 2074 656d        return tem
-0000b500: 702e 6e61 6d65 2c20 7365 6c66 2e72 6174  p.name, self.rat
-0000b510: 650d 0a0d 0a20 2020 2020 2020 2065 7863  e....        exc
-0000b520: 6570 7420 4b65 7962 6f61 7264 496e 7465  ept KeyboardInte
-0000b530: 7272 7570 743a 0d0a 2020 2020 2020 2020  rrupt:..        
-0000b540: 2020 2020 6966 2073 656c 662e 6572 726f      if self.erro
-0000b550: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000b560: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
-0000b570: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
-0000b580: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000b590: 636b 2822 4361 6e63 656c 6c69 6e67 2061  ck("Cancelling a
-0000b5a0: 6c6c 2074 6173 6b73 2229 0d0a 2020 2020  ll tasks")..    
-0000b5b0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0000b5c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000b5d0: 7269 6e74 2822 4361 6e63 656c 6c69 6e67  rint("Cancelling
-0000b5e0: 2061 6c6c 2074 6173 6b73 2229 0d0a 2020   all tasks")..  
-0000b5f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000b600: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
-0000b610: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-0000b620: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000b630: 6966 2073 656c 662e 6572 726f 725f 6d65  if self.error_me
-0000b640: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
-0000b650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b660: 2020 7365 6c66 2e65 7272 6f72 5f6d 6573    self.error_mes
-0000b670: 7361 6765 735f 6361 6c6c 6261 636b 2865  sages_callback(e
-0000b680: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-0000b690: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0000b6a0: 2020 2020 2020 7072 696e 7428 6529 0d0a        print(e)..
-0000b6b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000b6c0: 726e 0d0a 0d0a 0d0a 636c 6173 7320 5370  rn......class Sp
-0000b6d0: 6565 6368 5265 6769 6f6e 4669 6e64 6572  eechRegionFinder
-0000b6e0: 3a0d 0a20 2020 2040 7374 6174 6963 6d65  :..    @staticme
-0000b6f0: 7468 6f64 0d0a 2020 2020 6465 6620 7065  thod..    def pe
-0000b700: 7263 656e 7469 6c65 2861 7272 2c20 7065  rcentile(arr, pe
-0000b710: 7263 656e 7429 3a0d 0a20 2020 2020 2020  rcent):..       
-0000b720: 2061 7272 203d 2073 6f72 7465 6428 6172   arr = sorted(ar
-0000b730: 7229 0d0a 2020 2020 2020 2020 6b20 3d20  r)..        k = 
-0000b740: 286c 656e 2861 7272 2920 2d20 3129 202a  (len(arr) - 1) *
-0000b750: 2070 6572 6365 6e74 0d0a 2020 2020 2020   percent..      
-0000b760: 2020 6620 3d20 6d61 7468 2e66 6c6f 6f72    f = math.floor
-0000b770: 286b 290d 0a20 2020 2020 2020 2063 203d  (k)..        c =
-0000b780: 206d 6174 682e 6365 696c 286b 290d 0a20   math.ceil(k).. 
-0000b790: 2020 2020 2020 2069 6620 6620 3d3d 2063         if f == c
-0000b7a0: 3a20 7265 7475 726e 2061 7272 5b69 6e74  : return arr[int
-0000b7b0: 286b 295d 0d0a 2020 2020 2020 2020 6430  (k)]..        d0
-0000b7c0: 203d 2061 7272 5b69 6e74 2866 295d 202a   = arr[int(f)] *
-0000b7d0: 2028 6320 2d20 6b29 0d0a 2020 2020 2020   (c - k)..      
-0000b7e0: 2020 6431 203d 2061 7272 5b69 6e74 2863    d1 = arr[int(c
-0000b7f0: 295d 202a 2028 6b20 2d20 6629 0d0a 2020  )] * (k - f)..  
-0000b800: 2020 2020 2020 7265 7475 726e 2064 3020        return d0 
-0000b810: 2b20 6431 0d0a 0d0a 2020 2020 2364 6566  + d1....    #def
-0000b820: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-0000b830: 6672 616d 655f 7769 6474 683d 3430 3936  frame_width=4096
-0000b840: 2c20 6d69 6e5f 7265 6769 6f6e 5f73 697a  , min_region_siz
-0000b850: 653d 302e 352c 206d 6178 5f72 6567 696f  e=0.5, max_regio
-0000b860: 6e5f 7369 7a65 3d36 293a 0d0a 2020 2020  n_size=6):..    
-0000b870: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0000b880: 662c 2066 7261 6d65 5f77 6964 7468 3d34  f, frame_width=4
-0000b890: 3039 362c 206d 696e 5f72 6567 696f 6e5f  096, min_region_
-0000b8a0: 7369 7a65 3d30 2e35 2c20 6d61 785f 7265  size=0.5, max_re
-0000b8b0: 6769 6f6e 5f73 697a 653d 362c 2065 7272  gion_size=6, err
-0000b8c0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-0000b8d0: 6261 636b 3d4e 6f6e 6529 3a0d 0a20 2020  back=None):..   
-0000b8e0: 2020 2020 2073 656c 662e 6672 616d 655f       self.frame_
-0000b8f0: 7769 6474 6820 3d20 6672 616d 655f 7769  width = frame_wi
-0000b900: 6474 680d 0a20 2020 2020 2020 2073 656c  dth..        sel
-0000b910: 662e 6d69 6e5f 7265 6769 6f6e 5f73 697a  f.min_region_siz
-0000b920: 6520 3d20 6d69 6e5f 7265 6769 6f6e 5f73  e = min_region_s
-0000b930: 697a 650d 0a20 2020 2020 2020 2073 656c  ize..        sel
-0000b940: 662e 6d61 785f 7265 6769 6f6e 5f73 697a  f.max_region_siz
-0000b950: 6520 3d20 6d61 785f 7265 6769 6f6e 5f73  e = max_region_s
-0000b960: 697a 650d 0a20 2020 2020 2020 2073 656c  ize..        sel
-0000b970: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
-0000b980: 5f63 616c 6c62 6163 6b20 3d20 6572 726f  _callback = erro
-0000b990: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000b9a0: 6163 6b0d 0a0d 0a20 2020 2023 6465 6620  ack....    #def 
-0000b9b0: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2077  __call__(self, w
-0000b9c0: 6176 5f66 696c 6570 6174 682c 2065 7272  av_filepath, err
-0000b9d0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-0000b9e0: 6261 636b 3d4e 6f6e 6529 3a0d 0a20 2020  back=None):..   
-0000b9f0: 2064 6566 205f 5f63 616c 6c5f 5f28 7365   def __call__(se
-0000ba00: 6c66 2c20 7761 765f 6669 6c65 7061 7468  lf, wav_filepath
-0000ba10: 293a 0d0a 2020 2020 2020 2020 7472 793a  ):..        try:
-0000ba20: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0000ba30: 6164 6572 203d 2077 6176 652e 6f70 656e  ader = wave.open
-0000ba40: 2877 6176 5f66 696c 6570 6174 6829 0d0a  (wav_filepath)..
-0000ba50: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
-0000ba60: 6c65 5f77 6964 7468 203d 2072 6561 6465  le_width = reade
-0000ba70: 722e 6765 7473 616d 7077 6964 7468 2829  r.getsampwidth()
-0000ba80: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-0000ba90: 7465 203d 2072 6561 6465 722e 6765 7466  te = reader.getf
-0000baa0: 7261 6d65 7261 7465 2829 0d0a 2020 2020  ramerate()..    
-0000bab0: 2020 2020 2020 2020 6e5f 6368 616e 6e65          n_channe
-0000bac0: 6c73 203d 2072 6561 6465 722e 6765 746e  ls = reader.getn
-0000bad0: 6368 616e 6e65 6c73 2829 0d0a 2020 2020  channels()..    
-0000bae0: 2020 2020 2020 2020 746f 7461 6c5f 6475          total_du
-0000baf0: 7261 7469 6f6e 203d 2072 6561 6465 722e  ration = reader.
-0000bb00: 6765 746e 6672 616d 6573 2829 202f 2072  getnframes() / r
-0000bb10: 6174 650d 0a20 2020 2020 2020 2020 2020  ate..           
-0000bb20: 2063 6875 6e6b 5f64 7572 6174 696f 6e20   chunk_duration 
-0000bb30: 3d20 666c 6f61 7428 7365 6c66 2e66 7261  = float(self.fra
-0000bb40: 6d65 5f77 6964 7468 2920 2f20 7261 7465  me_width) / rate
-0000bb50: 0d0a 2020 2020 2020 2020 2020 2020 6e5f  ..            n_
-0000bb60: 6368 756e 6b73 203d 2069 6e74 2874 6f74  chunks = int(tot
-0000bb70: 616c 5f64 7572 6174 696f 6e20 2f20 6368  al_duration / ch
-0000bb80: 756e 6b5f 6475 7261 7469 6f6e 290d 0a20  unk_duration).. 
-0000bb90: 2020 2020 2020 2020 2020 2065 6e65 7267             energ
-0000bba0: 6965 7320 3d20 5b5d 0d0a 2020 2020 2020  ies = []..      
-0000bbb0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-0000bbc0: 616e 6765 286e 5f63 6875 6e6b 7329 3a0d  ange(n_chunks):.
-0000bbd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bbe0: 2063 6875 6e6b 203d 2072 6561 6465 722e   chunk = reader.
-0000bbf0: 7265 6164 6672 616d 6573 2873 656c 662e  readframes(self.
-0000bc00: 6672 616d 655f 7769 6474 6829 0d0a 2020  frame_width)..  
-0000bc10: 2020 2020 2020 2020 2020 2020 2020 656e                en
-0000bc20: 6572 6769 6573 2e61 7070 656e 6428 6175  ergies.append(au
-0000bc30: 6469 6f6f 702e 726d 7328 6368 756e 6b2c  dioop.rms(chunk,
-0000bc40: 2073 616d 706c 655f 7769 6474 6820 2a20   sample_width * 
-0000bc50: 6e5f 6368 616e 6e65 6c73 2929 0d0a 2020  n_channels))..  
-0000bc60: 2020 2020 2020 2020 2020 7468 7265 7368            thresh
-0000bc70: 6f6c 6420 3d20 5370 6565 6368 5265 6769  old = SpeechRegi
-0000bc80: 6f6e 4669 6e64 6572 2e70 6572 6365 6e74  onFinder.percent
-0000bc90: 696c 6528 656e 6572 6769 6573 2c20 302e  ile(energies, 0.
-0000bca0: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-0000bcb0: 656c 6170 7365 645f 7469 6d65 203d 2030  elapsed_time = 0
-0000bcc0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0000bcd0: 6769 6f6e 7320 3d20 5b5d 0d0a 2020 2020  gions = []..    
-0000bce0: 2020 2020 2020 2020 7265 6769 6f6e 5f73          region_s
-0000bcf0: 7461 7274 203d 204e 6f6e 650d 0a20 2020  tart = None..   
-0000bd00: 2020 2020 2020 2020 2066 6f72 2065 6e65           for ene
-0000bd10: 7267 7920 696e 2065 6e65 7267 6965 733a  rgy in energies:
-0000bd20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bd30: 2020 6973 5f73 696c 656e 6365 203d 2065    is_silence = e
-0000bd40: 6e65 7267 7920 3c3d 2074 6872 6573 686f  nergy <= thresho
-0000bd50: 6c64 0d0a 2020 2020 2020 2020 2020 2020  ld..            
-0000bd60: 2020 2020 6d61 785f 6578 6365 6564 6564      max_exceeded
-0000bd70: 203d 2072 6567 696f 6e5f 7374 6172 7420   = region_start 
-0000bd80: 616e 6420 656c 6170 7365 645f 7469 6d65  and elapsed_time
-0000bd90: 202d 2072 6567 696f 6e5f 7374 6172 7420   - region_start 
-0000bda0: 3e3d 2073 656c 662e 6d61 785f 7265 6769  >= self.max_regi
-0000bdb0: 6f6e 5f73 697a 650d 0a20 2020 2020 2020  on_size..       
-0000bdc0: 2020 2020 2020 2020 2069 6620 286d 6178           if (max
-0000bdd0: 5f65 7863 6565 6465 6420 6f72 2069 735f  _exceeded or is_
-0000bde0: 7369 6c65 6e63 6529 2061 6e64 2072 6567  silence) and reg
-0000bdf0: 696f 6e5f 7374 6172 743a 0d0a 2020 2020  ion_start:..    
-0000be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be10: 6966 2065 6c61 7073 6564 5f74 696d 6520  if elapsed_time 
-0000be20: 2d20 7265 6769 6f6e 5f73 7461 7274 203e  - region_start >
-0000be30: 3d20 7365 6c66 2e6d 696e 5f72 6567 696f  = self.min_regio
-0000be40: 6e5f 7369 7a65 3a0d 0a20 2020 2020 2020  n_size:..       
-0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be60: 2072 6567 696f 6e73 2e61 7070 656e 6428   regions.append(
-0000be70: 2872 6567 696f 6e5f 7374 6172 742c 2065  (region_start, e
-0000be80: 6c61 7073 6564 5f74 696d 6529 290d 0a20  lapsed_time)).. 
-0000be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bea0: 2020 2020 2020 2072 6567 696f 6e5f 7374         region_st
-0000beb0: 6172 7420 3d20 4e6f 6e65 0d0a 2020 2020  art = None..    
-0000bec0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0000bed0: 2028 6e6f 7420 7265 6769 6f6e 5f73 7461   (not region_sta
-0000bee0: 7274 2920 616e 6420 286e 6f74 2069 735f  rt) and (not is_
-0000bef0: 7369 6c65 6e63 6529 3a0d 0a20 2020 2020  silence):..     
-0000bf00: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000bf10: 6567 696f 6e5f 7374 6172 7420 3d20 656c  egion_start = el
-0000bf20: 6170 7365 645f 7469 6d65 0d0a 2020 2020  apsed_time..    
-0000bf30: 2020 2020 2020 2020 2020 2020 656c 6170              elap
-0000bf40: 7365 645f 7469 6d65 202b 3d20 6368 756e  sed_time += chun
-0000bf50: 6b5f 6475 7261 7469 6f6e 0d0a 2020 2020  k_duration..    
-0000bf60: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0000bf70: 6567 696f 6e73 0d0a 0d0a 2020 2020 2020  egions....      
-0000bf80: 2020 6578 6365 7074 204b 6579 626f 6172    except Keyboar
-0000bf90: 6449 6e74 6572 7275 7074 3a0d 0a20 2020  dInterrupt:..   
-0000bfa0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000bfb0: 2e65 7272 6f72 5f6d 6573 7361 6765 735f  .error_messages_
-0000bfc0: 6361 6c6c 6261 636b 3a0d 0a20 2020 2020  callback:..     
-0000bfd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000bfe0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-0000bff0: 616c 6c62 6163 6b28 2243 616e 6365 6c6c  allback("Cancell
-0000c000: 696e 6720 616c 6c20 7461 736b 7322 290d  ing all tasks").
-0000c010: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000c020: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000c030: 2020 2020 7072 696e 7428 2243 616e 6365      print("Cance
-0000c040: 6c6c 696e 6720 616c 6c20 7461 736b 7322  lling all tasks"
-0000c050: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-0000c060: 6574 7572 6e0d 0a0d 0a20 2020 2020 2020  eturn....       
-0000c070: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0000c080: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
-0000c090: 2020 2020 2069 6620 7365 6c66 2e65 7272       if self.err
-0000c0a0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-0000c0b0: 6261 636b 3a0d 0a20 2020 2020 2020 2020  back:..         
-0000c0c0: 2020 2020 2020 2073 656c 662e 6572 726f         self.erro
-0000c0d0: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000c0e0: 6163 6b28 6529 0d0a 2020 2020 2020 2020  ack(e)..        
-0000c0f0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0000c100: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000c110: 2865 290d 0a20 2020 2020 2020 2020 2020  (e)..           
-0000c120: 2072 6574 7572 6e0d 0a0d 0a0d 0a63 6c61   return......cla
-0000c130: 7373 2046 4c41 4343 6f6e 7665 7274 6572  ss FLACConverter
-0000c140: 286f 626a 6563 7429 3a0d 0a20 2020 2023  (object):..    #
-0000c150: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0000c160: 662c 2077 6176 5f66 696c 6570 6174 682c  f, wav_filepath,
-0000c170: 2069 6e63 6c75 6465 5f62 6566 6f72 653d   include_before=
-0000c180: 302e 3235 2c20 696e 636c 7564 655f 6166  0.25, include_af
-0000c190: 7465 723d 302e 3235 293a 0d0a 2020 2020  ter=0.25):..    
-0000c1a0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0000c1b0: 662c 2077 6176 5f66 696c 6570 6174 682c  f, wav_filepath,
-0000c1c0: 2069 6e63 6c75 6465 5f62 6566 6f72 653d   include_before=
-0000c1d0: 302e 3235 2c20 696e 636c 7564 655f 6166  0.25, include_af
-0000c1e0: 7465 723d 302e 3235 2c20 6572 726f 725f  ter=0.25, error_
-0000c1f0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000c200: 6b3d 4e6f 6e65 293a 0d0a 2020 2020 2020  k=None):..      
-0000c210: 2020 7365 6c66 2e77 6176 5f66 696c 6570    self.wav_filep
-0000c220: 6174 6820 3d20 7761 765f 6669 6c65 7061  ath = wav_filepa
-0000c230: 7468 0d0a 2020 2020 2020 2020 7365 6c66  th..        self
-0000c240: 2e69 6e63 6c75 6465 5f62 6566 6f72 6520  .include_before 
-0000c250: 3d20 696e 636c 7564 655f 6265 666f 7265  = include_before
-0000c260: 0d0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
-0000c270: 6e63 6c75 6465 5f61 6674 6572 203d 2069  nclude_after = i
-0000c280: 6e63 6c75 6465 5f61 6674 6572 0d0a 2020  nclude_after..  
-0000c290: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
-0000c2a0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000c2b0: 636b 203d 2065 7272 6f72 5f6d 6573 7361  ck = error_messa
-0000c2c0: 6765 735f 6361 6c6c 6261 636b 0d0a 0d0a  ges_callback....
-0000c2d0: 2020 2020 2364 6566 205f 5f63 616c 6c5f      #def __call_
-0000c2e0: 5f28 7365 6c66 2c20 7265 6769 6f6e 2c20  _(self, region, 
-0000c2f0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-0000c300: 616c 6c62 6163 6b3d 4e6f 6e65 293a 0d0a  allback=None):..
-0000c310: 2020 2020 6465 6620 5f5f 6361 6c6c 5f5f      def __call__
-0000c320: 2873 656c 662c 2072 6567 696f 6e29 3a0d  (self, region):.
-0000c330: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-0000c340: 2020 2020 2020 2020 2020 2073 7461 7274             start
-0000c350: 2c20 656e 6420 3d20 7265 6769 6f6e 0d0a  , end = region..
-0000c360: 2020 2020 2020 2020 2020 2020 7374 6172              star
-0000c370: 7420 3d20 6d61 7828 302c 2073 7461 7274  t = max(0, start
-0000c380: 202d 2073 656c 662e 696e 636c 7564 655f   - self.include_
-0000c390: 6265 666f 7265 290d 0a20 2020 2020 2020  before)..       
-0000c3a0: 2020 2020 2065 6e64 202b 3d20 7365 6c66       end += self
-0000c3b0: 2e69 6e63 6c75 6465 5f61 6674 6572 0d0a  .include_after..
-0000c3c0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000c3d0: 203d 2074 656d 7066 696c 652e 4e61 6d65   = tempfile.Name
-0000c3e0: 6454 656d 706f 7261 7279 4669 6c65 2873  dTemporaryFile(s
-0000c3f0: 7566 6669 783d 272e 666c 6163 272c 2064  uffix='.flac', d
-0000c400: 656c 6574 653d 4661 6c73 6529 0d0a 2020  elete=False)..  
-0000c410: 2020 2020 2020 2020 2020 636f 6d6d 616e            comman
-0000c420: 6420 3d20 5b0d 0a20 2020 2020 2020 2020  d = [..         
-0000c430: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000c440: 6666 6d70 6567 222c 0d0a 2020 2020 2020  ffmpeg",..      
-0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c460: 2020 222d 7373 222c 2073 7472 2873 7461    "-ss", str(sta
-0000c470: 7274 292c 0d0a 2020 2020 2020 2020 2020  rt),..          
-0000c480: 2020 2020 2020 2020 2020 2020 2020 222d                "-
-0000c490: 7422 2c20 7374 7228 656e 6420 2d20 7374  t", str(end - st
-0000c4a0: 6172 7429 2c0d 0a20 2020 2020 2020 2020  art),..         
-0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000c4c0: 2d79 222c 0d0a 2020 2020 2020 2020 2020  -y",..          
-0000c4d0: 2020 2020 2020 2020 2020 2020 2020 222d                "-
-0000c4e0: 6922 2c20 7365 6c66 2e77 6176 5f66 696c  i", self.wav_fil
-0000c4f0: 6570 6174 682c 0d0a 2020 2020 2020 2020  epath,..        
-0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c510: 222d 6c6f 676c 6576 656c 222c 2022 6572  "-loglevel", "er
-0000c520: 726f 7222 2c0d 0a20 2020 2020 2020 2020  ror",..         
-0000c530: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000c540: 656d 702e 6e61 6d65 0d0a 2020 2020 2020  emp.name..      
-0000c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c560: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
-0000c570: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
-0000c580: 6f75 7470 7574 2863 6f6d 6d61 6e64 2c20  output(command, 
-0000c590: 7374 6469 6e3d 6f70 656e 286f 732e 6465  stdin=open(os.de
-0000c5a0: 766e 756c 6c29 290d 0a20 2020 2020 2020  vnull))..       
-0000c5b0: 2020 2020 2063 6f6e 7465 6e74 203d 2074       content = t
-0000c5c0: 656d 702e 7265 6164 2829 0d0a 2020 2020  emp.read()..    
-0000c5d0: 2020 2020 2020 2020 7465 6d70 2e63 6c6f          temp.clo
-0000c5e0: 7365 2829 0d0a 2020 2020 2020 2020 2020  se()..          
-0000c5f0: 2020 7265 7475 726e 2063 6f6e 7465 6e74    return content
-0000c600: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
-0000c610: 7074 204b 6579 626f 6172 6449 6e74 6572  pt KeyboardInter
-0000c620: 7275 7074 3a0d 0a20 2020 2020 2020 2020  rupt:..         
-0000c630: 2020 2069 6620 7365 6c66 2e65 7272 6f72     if self.error
-0000c640: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000c650: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
-0000c660: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
-0000c670: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000c680: 6b28 2243 616e 6365 6c6c 696e 6720 616c  k("Cancelling al
-0000c690: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
-0000c6a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0000c6b0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000c6c0: 696e 7428 2243 616e 6365 6c6c 696e 6720  int("Cancelling 
-0000c6d0: 616c 6c20 7461 736b 7322 290d 0a20 2020  all tasks")..   
-0000c6e0: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
-0000c6f0: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
-0000c700: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-0000c710: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-0000c720: 6620 7365 6c66 2e65 7272 6f72 5f6d 6573  f self.error_mes
-0000c730: 7361 6765 735f 6361 6c6c 6261 636b 3a0d  sages_callback:.
-0000c740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c750: 2073 656c 662e 6572 726f 725f 6d65 7373   self.error_mess
-0000c760: 6167 6573 5f63 616c 6c62 6163 6b28 6529  ages_callback(e)
-0000c770: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0000c780: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000c790: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
-0000c7a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000c7b0: 6e0d 0a0d 0a0d 0a63 6c61 7373 2053 7065  n......class Spe
-0000c7c0: 6563 6852 6563 6f67 6e69 7a65 7228 6f62  echRecognizer(ob
-0000c7d0: 6a65 6374 293a 0d0a 2020 2020 6465 6620  ject):..    def 
-0000c7e0: 5f5f 696e 6974 5f5f 2873 656c 662c 206c  __init__(self, l
-0000c7f0: 616e 6775 6167 653d 2265 6e22 2c20 7261  anguage="en", ra
-0000c800: 7465 3d34 3431 3030 2c20 7265 7472 6965  te=44100, retrie
-0000c810: 733d 332c 2061 7069 5f6b 6579 3d22 4149  s=3, api_key="AI
-0000c820: 7a61 5379 424f 7469 346d 4d2d 3678 3957  zaSyBOti4mM-6x9W
-0000c830: 446e 5a49 6a49 6579 4555 3231 4f70 4258  DnZIjIeyEU21OpBX
-0000c840: 7157 4267 7722 2c20 7469 6d65 6f75 743d  qWBgw", timeout=
-0000c850: 3330 2c20 6572 726f 725f 6d65 7373 6167  30, error_messag
-0000c860: 6573 5f63 616c 6c62 6163 6b3d 4e6f 6e65  es_callback=None
-0000c870: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
-0000c880: 2e6c 616e 6775 6167 6520 3d20 6c61 6e67  .language = lang
-0000c890: 7561 6765 0d0a 2020 2020 2020 2020 7365  uage..        se
-0000c8a0: 6c66 2e72 6174 6520 3d20 7261 7465 0d0a  lf.rate = rate..
-0000c8b0: 2020 2020 2020 2020 7365 6c66 2e61 7069          self.api
-0000c8c0: 5f6b 6579 203d 2061 7069 5f6b 6579 0d0a  _key = api_key..
-0000c8d0: 2020 2020 2020 2020 7365 6c66 2e72 6574          self.ret
-0000c8e0: 7269 6573 203d 2072 6574 7269 6573 0d0a  ries = retries..
-0000c8f0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
-0000c900: 656f 7574 203d 2074 696d 656f 7574 0d0a  eout = timeout..
-0000c910: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
-0000c920: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-0000c930: 6261 636b 203d 2065 7272 6f72 5f6d 6573  back = error_mes
-0000c940: 7361 6765 735f 6361 6c6c 6261 636b 0d0a  sages_callback..
-0000c950: 0d0a 2020 2020 6465 6620 5f5f 6361 6c6c  ..    def __call
-0000c960: 5f5f 2873 656c 662c 2064 6174 6129 3a0d  __(self, data):.
-0000c970: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-0000c980: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0000c990: 2069 6e20 7261 6e67 6528 7365 6c66 2e72   in range(self.r
-0000c9a0: 6574 7269 6573 293a 0d0a 2020 2020 2020  etries):..      
-0000c9b0: 2020 2020 2020 2020 2020 7572 6c20 3d20            url = 
-0000c9c0: 2268 7474 703a 2f2f 7777 772e 676f 6f67  "http://www.goog
-0000c9d0: 6c65 2e63 6f6d 2f73 7065 6563 682d 6170  le.com/speech-ap
-0000c9e0: 692f 7632 2f72 6563 6f67 6e69 7a65 3f63  i/v2/recognize?c
-0000c9f0: 6c69 656e 743d 6368 726f 6d69 756d 266c  lient=chromium&l
-0000ca00: 616e 673d 7b6c 616e 677d 266b 6579 3d7b  ang={lang}&key={
-0000ca10: 6b65 797d 222e 666f 726d 6174 286c 616e  key}".format(lan
-0000ca20: 673d 7365 6c66 2e6c 616e 6775 6167 652c  g=self.language,
-0000ca30: 206b 6579 3d73 656c 662e 6170 695f 6b65   key=self.api_ke
-0000ca40: 7929 0d0a 2020 2020 2020 2020 2020 2020  y)..            
-0000ca50: 2020 2020 6865 6164 6572 7320 3d20 7b22      headers = {"
-0000ca60: 436f 6e74 656e 742d 5479 7065 223a 2022  Content-Type": "
-0000ca70: 6175 6469 6f2f 782d 666c 6163 2072 6174  audio/x-flac rat
-0000ca80: 653d 2564 2220 2520 7365 6c66 2e72 6174  e=%d" % self.rat
-0000ca90: 657d 0d0a 0d0a 2020 2020 2020 2020 2020  e}....          
-0000caa0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-0000cab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cac0: 7265 7370 203d 2072 6571 7565 7374 732e  resp = requests.
-0000cad0: 706f 7374 2875 726c 2c20 6461 7461 3d64  post(url, data=d
-0000cae0: 6174 612c 2068 6561 6465 7273 3d68 6561  ata, headers=hea
-0000caf0: 6465 7273 2c20 7469 6d65 6f75 743d 7365  ders, timeout=se
-0000cb00: 6c66 2e74 696d 656f 7574 290d 0a20 2020  lf.timeout)..   
-0000cb10: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-0000cb20: 6570 7420 7265 7175 6573 7473 2e65 7863  ept requests.exc
-0000cb30: 6570 7469 6f6e 732e 436f 6e6e 6563 7469  eptions.Connecti
-0000cb40: 6f6e 4572 726f 723a 0d0a 2020 2020 2020  onError:..      
-0000cb50: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0000cb60: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-0000cb70: 2020 2020 2020 2020 2020 2020 7265 7370              resp
-0000cb80: 203d 2068 7474 7078 2e70 6f73 7428 7572   = httpx.post(ur
-0000cb90: 6c2c 2064 6174 613d 6461 7461 2c20 6865  l, data=data, he
-0000cba0: 6164 6572 733d 6865 6164 6572 732c 2074  aders=headers, t
-0000cbb0: 696d 656f 7574 3d73 656c 662e 7469 6d65  imeout=self.time
-0000cbc0: 6f75 7429 0d0a 2020 2020 2020 2020 2020  out)..          
-0000cbd0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-0000cbe0: 2068 7474 7078 2e65 7863 6570 7469 6f6e   httpx.exception
-0000cbf0: 732e 4e65 7477 6f72 6b45 7272 6f72 3a0d  s.NetworkError:.
-0000cc00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cc10: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-0000cc20: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-0000cc30: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
-0000cc40: 2072 6573 702e 636f 6e74 656e 742e 6465   resp.content.de
-0000cc50: 636f 6465 2827 7574 662d 3827 292e 7370  code('utf-8').sp
-0000cc60: 6c69 7428 225c 6e22 293a 0d0a 2020 2020  lit("\n"):..    
-0000cc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc80: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-0000cc90: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000cca0: 6e65 203d 206a 736f 6e2e 6c6f 6164 7328  ne = json.loads(
-0000ccb0: 6c69 6e65 290d 0a20 2020 2020 2020 2020  line)..         
-0000ccc0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000ccd0: 696e 6520 3d20 6c69 6e65 5b27 7265 7375  ine = line['resu
-0000cce0: 6c74 275d 5b30 5d5b 2761 6c74 6572 6e61  lt'][0]['alterna
-0000ccf0: 7469 7665 275d 5b30 5d5b 2774 7261 6e73  tive'][0]['trans
-0000cd00: 6372 6970 7427 5d0d 0a20 2020 2020 2020  cript']..       
-0000cd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd20: 2072 6574 7572 6e20 6c69 6e65 5b3a 315d   return line[:1]
-0000cd30: 2e75 7070 6572 2829 202b 206c 696e 655b  .upper() + line[
-0000cd40: 313a 5d0d 0a20 2020 2020 2020 2020 2020  1:]..           
-0000cd50: 2020 2020 2020 2020 2065 7863 6570 743a           except:
-0000cd60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cd70: 2020 2020 2020 2020 2020 2320 6e6f 2072            # no r
-0000cd80: 6573 756c 740d 0a20 2020 2020 2020 2020  esult..         
-0000cd90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000cda0: 6f6e 7469 6e75 650d 0a0d 0a20 2020 2020  ontinue....     
-0000cdb0: 2020 2065 7863 6570 7420 4b65 7962 6f61     except Keyboa
-0000cdc0: 7264 496e 7465 7272 7570 743a 0d0a 2020  rdInterrupt:..  
-0000cdd0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000cde0: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
-0000cdf0: 5f63 616c 6c62 6163 6b3a 0d0a 2020 2020  _callback:..    
-0000ce00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ce10: 2e65 7272 6f72 5f6d 6573 7361 6765 735f  .error_messages_
-0000ce20: 6361 6c6c 6261 636b 2822 4361 6e63 656c  callback("Cancel
-0000ce30: 6c69 6e67 2061 6c6c 2074 6173 6b73 2229  ling all tasks")
-0000ce40: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0000ce50: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000ce60: 2020 2020 2070 7269 6e74 2822 4361 6e63       print("Canc
-0000ce70: 656c 6c69 6e67 2061 6c6c 2074 6173 6b73  elling all tasks
-0000ce80: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000ce90: 7265 7475 726e 0d0a 0d0a 2020 2020 2020  return....      
-0000cea0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-0000ceb0: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
-0000cec0: 2020 2020 2020 6966 2073 656c 662e 6572        if self.er
-0000ced0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-0000cee0: 6c62 6163 6b3a 0d0a 2020 2020 2020 2020  lback:..        
-0000cef0: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
-0000cf00: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-0000cf10: 6261 636b 2865 290d 0a20 2020 2020 2020  back(e)..       
-0000cf20: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-0000cf30: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000cf40: 7428 6529 0d0a 2020 2020 2020 2020 2020  t(e)..          
-0000cf50: 2020 7265 7475 726e 0d0a 0d0a 0d0a 636c    return......cl
-0000cf60: 6173 7320 5768 6973 7065 7252 6563 6f67  ass WhisperRecog
-0000cf70: 6e69 7a65 7228 6f62 6a65 6374 293a 0d0a  nizer(object):..
-0000cf80: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0000cf90: 2873 656c 662c 206d 6f64 656c 3d22 736d  (self, model="sm
-0000cfa0: 616c 6c22 2c20 6c61 6e67 7561 6765 3d22  all", language="
-0000cfb0: 656e 222c 2066 7031 363d 4661 6c73 652c  en", fp16=False,
-0000cfc0: 2074 6173 6b3d 2274 7261 6e73 6372 6962   task="transcrib
-0000cfd0: 6522 2c20 7665 7262 6f73 653d 4661 6c73  e", verbose=Fals
-0000cfe0: 652c 2065 7272 6f72 5f6d 6573 7361 6765  e, error_message
-0000cff0: 735f 6361 6c6c 6261 636b 3d4e 6f6e 6529  s_callback=None)
-0000d000: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-0000d010: 6d6f 6465 6c20 3d20 6d6f 6465 6c0d 0a20  model = model.. 
-0000d020: 2020 2020 2020 2073 656c 662e 6c61 6e67         self.lang
-0000d030: 7561 6765 203d 206c 616e 6775 6167 650d  uage = language.
-0000d040: 0a20 2020 2020 2020 2073 656c 662e 6670  .        self.fp
-0000d050: 3136 203d 2066 7031 360d 0a20 2020 2020  16 = fp16..     
-0000d060: 2020 2073 656c 662e 7461 736b 203d 2074     self.task = t
-0000d070: 6173 6b0d 0a20 2020 2020 2020 2073 656c  ask..        sel
-0000d080: 662e 7665 7262 6f73 6520 3d20 7665 7262  f.verbose = verb
-0000d090: 6f73 650d 0a20 2020 2020 2020 2073 656c  ose..        sel
-0000d0a0: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
-0000d0b0: 5f63 616c 6c62 6163 6b20 3d20 6572 726f  _callback = erro
-0000d0c0: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000d0d0: 6163 6b0d 0a0d 0a20 2020 2064 6566 205f  ack....    def _
-0000d0e0: 5f63 616c 6c5f 5f28 7365 6c66 2c20 6175  _call__(self, au
-0000d0f0: 6469 6f5f 7061 7468 293a 0d0a 2020 2020  dio_path):..    
-0000d100: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-0000d110: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
-0000d120: 656c 662e 6d6f 6465 6c2e 7472 616e 7363  elf.model.transc
-0000d130: 7269 6265 2861 7564 696f 5f70 6174 682c  ribe(audio_path,
-0000d140: 206c 616e 6775 6167 653d 7365 6c66 2e6c   language=self.l
-0000d150: 616e 6775 6167 652c 2066 7031 363d 7365  anguage, fp16=se
-0000d160: 6c66 2e66 7031 362c 2074 6173 6b3d 7365  lf.fp16, task=se
-0000d170: 6c66 2e74 6173 6b2c 2076 6572 626f 7365  lf.task, verbose
-0000d180: 3d73 656c 662e 7665 7262 6f73 6529 0d0a  =self.verbose)..
-0000d190: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d1a0: 726e 2072 6573 756c 740d 0a0d 0a20 2020  rn result....   
-0000d1b0: 2020 2020 2065 7863 6570 7420 4b65 7962       except Keyb
-0000d1c0: 6f61 7264 496e 7465 7272 7570 743a 0d0a  oardInterrupt:..
-0000d1d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000d1e0: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
-0000d1f0: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
-0000d200: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d210: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
-0000d220: 735f 6361 6c6c 6261 636b 2822 4361 6e63  s_callback("Canc
-0000d230: 656c 6c69 6e67 2061 6c6c 2074 6173 6b73  elling all tasks
-0000d240: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000d250: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0000d260: 2020 2020 2020 2070 7269 6e74 2822 4361         print("Ca
-0000d270: 6e63 656c 6c69 6e67 2061 6c6c 2074 6173  ncelling all tas
-0000d280: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
-0000d290: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
-0000d2a0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-0000d2b0: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
-0000d2c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d2d0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-0000d2e0: 616c 6c62 6163 6b3a 0d0a 2020 2020 2020  allback:..      
-0000d2f0: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-0000d300: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000d310: 6c6c 6261 636b 2865 290d 0a20 2020 2020  llback(e)..     
-0000d320: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0000d330: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000d340: 696e 7428 6529 0d0a 2020 2020 2020 2020  int(e)..        
-0000d350: 2020 2020 7265 7475 726e 0d0a 0d0a 0d0a      return......
-0000d360: 636c 6173 7320 5365 6e74 656e 6365 5472  class SentenceTr
-0000d370: 616e 736c 6174 6f72 286f 626a 6563 7429  anslator(object)
-0000d380: 3a0d 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
-0000d390: 745f 5f28 7365 6c66 2c20 7372 632c 2064  t__(self, src, d
-0000d3a0: 7374 2c20 7061 7469 656e 6365 3d2d 312c  st, patience=-1,
-0000d3b0: 2074 696d 656f 7574 3d33 302c 2065 7272   timeout=30, err
-0000d3c0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-0000d3d0: 6261 636b 3d4e 6f6e 6529 3a0d 0a20 2020  back=None):..   
-0000d3e0: 2020 2020 2073 656c 662e 7372 6320 3d20       self.src = 
-0000d3f0: 7372 630d 0a20 2020 2020 2020 2073 656c  src..        sel
-0000d400: 662e 6473 7420 3d20 6473 740d 0a20 2020  f.dst = dst..   
-0000d410: 2020 2020 2073 656c 662e 7061 7469 656e       self.patien
-0000d420: 6365 203d 2070 6174 6965 6e63 650d 0a20  ce = patience.. 
-0000d430: 2020 2020 2020 2073 656c 662e 7469 6d65         self.time
-0000d440: 6f75 7420 3d20 7469 6d65 6f75 740d 0a20  out = timeout.. 
-0000d450: 2020 2020 2020 2073 656c 662e 6572 726f         self.erro
-0000d460: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000d470: 6163 6b20 3d20 6572 726f 725f 6d65 7373  ack = error_mess
-0000d480: 6167 6573 5f63 616c 6c62 6163 6b0d 0a0d  ages_callback...
-0000d490: 0a20 2020 2064 6566 205f 5f63 616c 6c5f  .    def __call_
-0000d4a0: 5f28 7365 6c66 2c20 7365 6e74 656e 6365  _(self, sentence
-0000d4b0: 293a 0d0a 2020 2020 2020 2020 7472 793a  ):..        try:
-0000d4c0: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
-0000d4d0: 616e 736c 6174 6564 5f73 656e 7465 6e63  anslated_sentenc
-0000d4e0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-0000d4f0: 2020 2020 2320 6861 6e64 6c65 2074 6865      # handle the
-0000d500: 2073 7065 6369 616c 2063 6173 653a 2065   special case: e
-0000d510: 6d70 7479 2073 7472 696e 672e 0d0a 2020  mpty string...  
-0000d520: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000d530: 2073 656e 7465 6e63 653a 0d0a 2020 2020   sentence:..    
-0000d540: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d550: 726e 204e 6f6e 650d 0a20 2020 2020 2020  rn None..       
-0000d560: 2020 2020 2074 7261 6e73 6c61 7465 645f       translated_
-0000d570: 7365 6e74 656e 6365 203d 2073 656c 662e  sentence = self.
-0000d580: 476f 6f67 6c65 5472 616e 736c 6174 6528  GoogleTranslate(
-0000d590: 7365 6e74 656e 6365 2c20 7372 633d 7365  sentence, src=se
-0000d5a0: 6c66 2e73 7263 2c20 6473 743d 7365 6c66  lf.src, dst=self
-0000d5b0: 2e64 7374 2c20 7469 6d65 6f75 743d 7365  .dst, timeout=se
-0000d5c0: 6c66 2e74 696d 656f 7574 290d 0a20 2020  lf.timeout)..   
-0000d5d0: 2020 2020 2020 2020 2066 6169 6c5f 746f           fail_to
-0000d5e0: 5f74 7261 6e73 6c61 7465 203d 2074 7261  _translate = tra
-0000d5f0: 6e73 6c61 7465 645f 7365 6e74 656e 6365  nslated_sentence
-0000d600: 5b2d 315d 203d 3d20 275c 6e27 0d0a 2020  [-1] == '\n'..  
-0000d610: 2020 2020 2020 2020 2020 7768 696c 6520            while 
-0000d620: 6661 696c 5f74 6f5f 7472 616e 736c 6174  fail_to_translat
-0000d630: 6520 616e 6420 7061 7469 656e 6365 3a0d  e and patience:.
-0000d640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d650: 2074 7261 6e73 6c61 7465 645f 7365 6e74   translated_sent
-0000d660: 656e 6365 203d 2073 656c 662e 476f 6f67  ence = self.Goog
-0000d670: 6c65 5472 616e 736c 6174 6528 7472 616e  leTranslate(tran
-0000d680: 736c 6174 6564 5f73 656e 7465 6e63 652c  slated_sentence,
-0000d690: 2073 7263 3d73 656c 662e 7372 632c 2064   src=self.src, d
-0000d6a0: 7374 3d73 656c 662e 6473 742c 2074 696d  st=self.dst, tim
-0000d6b0: 656f 7574 3d73 656c 662e 7469 6d65 6f75  eout=self.timeou
-0000d6c0: 7429 2e74 6578 740d 0a20 2020 2020 2020  t).text..       
-0000d6d0: 2020 2020 2020 2020 2069 6620 7472 616e           if tran
-0000d6e0: 736c 6174 6564 5f73 656e 7465 6e63 655b  slated_sentence[
-0000d6f0: 2d31 5d20 3d3d 2027 5c6e 273a 0d0a 2020  -1] == '\n':..  
-0000d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d710: 2020 6966 2070 6174 6965 6e63 6520 3d3d    if patience ==
-0000d720: 202d 313a 0d0a 2020 2020 2020 2020 2020   -1:..          
-0000d730: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000d740: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
-0000d750: 2020 2020 2020 2020 2020 2020 7061 7469              pati
-0000d760: 656e 6365 202d 3d20 310d 0a20 2020 2020  ence -= 1..     
-0000d770: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000d780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d790: 2020 2020 2020 6661 696c 5f74 6f5f 7472        fail_to_tr
-0000d7a0: 616e 736c 6174 6520 3d20 4661 6c73 650d  anslate = False.
-0000d7b0: 0a0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
-0000d7c0: 6574 7572 6e20 7472 616e 736c 6174 6564  eturn translated
-0000d7d0: 5f73 656e 7465 6e63 650d 0a0d 0a20 2020  _sentence....   
-0000d7e0: 2020 2020 2065 7863 6570 7420 4b65 7962       except Keyb
-0000d7f0: 6f61 7264 496e 7465 7272 7570 743a 0d0a  oardInterrupt:..
-0000d800: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000d810: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
-0000d820: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
-0000d830: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d840: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
-0000d850: 735f 6361 6c6c 6261 636b 2822 4361 6e63  s_callback("Canc
-0000d860: 656c 6c69 6e67 2061 6c6c 2074 6173 6b73  elling all tasks
-0000d870: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000d880: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0000d890: 2020 2020 2020 2070 7269 6e74 2822 4361         print("Ca
-0000d8a0: 6e63 656c 6c69 6e67 2061 6c6c 2074 6173  ncelling all tas
-0000d8b0: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
-0000d8c0: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
-0000d8d0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-0000d8e0: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
-0000d8f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d900: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-0000d910: 616c 6c62 6163 6b3a 0d0a 2020 2020 2020  allback:..      
-0000d920: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-0000d930: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000d940: 6c6c 6261 636b 2865 290d 0a20 2020 2020  llback(e)..     
-0000d950: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0000d960: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000d970: 696e 7428 6529 0d0a 2020 2020 2020 2020  int(e)..        
-0000d980: 2020 2020 7265 7475 726e 0d0a 0d0a 2020      return....  
-0000d990: 2020 6465 6620 476f 6f67 6c65 5472 616e    def GoogleTran
-0000d9a0: 736c 6174 6528 7365 6c66 2c20 7465 7874  slate(self, text
-0000d9b0: 2c20 7372 632c 2064 7374 2c20 7469 6d65  , src, dst, time
-0000d9c0: 6f75 743d 3330 293a 0d0a 2020 2020 2020  out=30):..      
-0000d9d0: 2020 7572 6c20 3d20 2768 7474 7073 3a2f    url = 'https:/
-0000d9e0: 2f74 7261 6e73 6c61 7465 2e67 6f6f 676c  /translate.googl
-0000d9f0: 6561 7069 732e 636f 6d2f 7472 616e 736c  eapis.com/transl
-0000da00: 6174 655f 612f 270d 0a20 2020 2020 2020  ate_a/'..       
-0000da10: 2070 6172 616d 7320 3d20 2773 696e 676c   params = 'singl
-0000da20: 653f 636c 6965 6e74 3d67 7478 2673 6c3d  e?client=gtx&sl=
-0000da30: 272b 7372 632b 2726 746c 3d27 2b64 7374  '+src+'&tl='+dst
-0000da40: 2b27 2664 743d 7426 713d 272b 7465 7874  +'&dt=t&q='+text
-0000da50: 3b0d 0a20 2020 2020 2020 2068 6561 6465  ;..        heade
-0000da60: 7273 203d 207b 2755 7365 722d 4167 656e  rs = {'User-Agen
-0000da70: 7427 3a20 274d 6f7a 696c 6c61 2f35 2e30  t': 'Mozilla/5.0
-0000da80: 2028 5769 6e64 6f77 7320 4e54 2031 302e   (Windows NT 10.
-0000da90: 303b 2057 696e 3634 3b20 7836 3429 272c  0; Win64; x64)',
-0000daa0: 2027 5265 6665 7265 7227 3a20 2768 7474   'Referer': 'htt
-0000dab0: 7073 3a2f 2f74 7261 6e73 6c61 7465 2e67  ps://translate.g
-0000dac0: 6f6f 676c 652e 636f 6d27 2c7d 0d0a 0d0a  oogle.com',}....
-0000dad0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-0000dae0: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
-0000daf0: 7365 203d 2072 6571 7565 7374 732e 6765  se = requests.ge
-0000db00: 7428 7572 6c2b 7061 7261 6d73 2c20 6865  t(url+params, he
-0000db10: 6164 6572 733d 6865 6164 6572 732c 2074  aders=headers, t
-0000db20: 696d 656f 7574 3d73 656c 662e 7469 6d65  imeout=self.time
-0000db30: 6f75 7429 0d0a 2020 2020 2020 2020 2020  out)..          
-0000db40: 2020 6966 2072 6573 706f 6e73 652e 7374    if response.st
-0000db50: 6174 7573 5f63 6f64 6520 3d3d 2032 3030  atus_code == 200
-0000db60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000db70: 2020 2072 6573 706f 6e73 655f 6a73 6f6e     response_json
-0000db80: 203d 2072 6573 706f 6e73 652e 6a73 6f6e   = response.json
-0000db90: 2829 5b30 5d0d 0a20 2020 2020 2020 2020  ()[0]..         
-0000dba0: 2020 2020 2020 206c 656e 6774 6820 3d20         length = 
-0000dbb0: 6c65 6e28 7265 7370 6f6e 7365 5f6a 736f  len(response_jso
-0000dbc0: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
-0000dbd0: 2020 2020 7472 616e 736c 6174 696f 6e20      translation 
-0000dbe0: 3d20 2222 0d0a 2020 2020 2020 2020 2020  = ""..          
-0000dbf0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-0000dc00: 616e 6765 286c 656e 6774 6829 3a0d 0a20  ange(length):.. 
-0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc20: 2020 2074 7261 6e73 6c61 7469 6f6e 203d     translation =
-0000dc30: 2074 7261 6e73 6c61 7469 6f6e 202b 2072   translation + r
-0000dc40: 6573 706f 6e73 655f 6a73 6f6e 5b69 5d5b  esponse_json[i][
-0000dc50: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-0000dc60: 2020 2020 7265 7475 726e 2074 7261 6e73      return trans
-0000dc70: 6c61 7469 6f6e 0d0a 2020 2020 2020 2020  lation..        
-0000dc80: 2020 2020 7265 7475 726e 0d0a 0d0a 2020      return....  
-0000dc90: 2020 2020 2020 6578 6365 7074 2072 6571        except req
-0000dca0: 7565 7374 732e 6578 6365 7074 696f 6e73  uests.exceptions
-0000dcb0: 2e43 6f6e 6e65 6374 696f 6e45 7272 6f72  .ConnectionError
-0000dcc0: 3a0d 0a20 2020 2020 2020 2020 2020 2077  :..            w
-0000dcd0: 6974 6820 6874 7470 782e 436c 6965 6e74  ith httpx.Client
-0000dce0: 2829 2061 7320 636c 6965 6e74 3a0d 0a20  () as client:.. 
-0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000dd00: 6573 706f 6e73 6520 3d20 636c 6965 6e74  esponse = client
-0000dd10: 2e67 6574 2875 726c 2b70 6172 616d 732c  .get(url+params,
-0000dd20: 2068 6561 6465 7273 3d68 6561 6465 7273   headers=headers
-0000dd30: 2c20 7469 6d65 6f75 743d 7365 6c66 2e74  , timeout=self.t
-0000dd40: 696d 656f 7574 290d 0a20 2020 2020 2020  imeout)..       
-0000dd50: 2020 2020 2020 2020 2069 6620 7265 7370           if resp
-0000dd60: 6f6e 7365 2e73 7461 7475 735f 636f 6465  onse.status_code
-0000dd70: 203d 3d20 3230 303a 0d0a 2020 2020 2020   == 200:..      
-0000dd80: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000dd90: 7370 6f6e 7365 5f6a 736f 6e20 3d20 7265  sponse_json = re
-0000dda0: 7370 6f6e 7365 2e6a 736f 6e28 295b 305d  sponse.json()[0]
-0000ddb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ddc0: 2020 2020 2020 6c65 6e67 7468 203d 206c        length = l
-0000ddd0: 656e 2872 6573 706f 6e73 655f 6a73 6f6e  en(response_json
-0000dde0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000ddf0: 2020 2020 2020 2074 7261 6e73 6c61 7469         translati
-0000de00: 6f6e 203d 2022 220d 0a20 2020 2020 2020  on = ""..       
-0000de10: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000de20: 2069 2069 6e20 7261 6e67 6528 6c65 6e67   i in range(leng
-0000de30: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
-0000de40: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0000de50: 616e 736c 6174 696f 6e20 3d20 7472 616e  anslation = tran
-0000de60: 736c 6174 696f 6e20 2b20 7265 7370 6f6e  slation + respon
-0000de70: 7365 5f6a 736f 6e5b 695d 5b30 5d0d 0a20  se_json[i][0].. 
-0000de80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de90: 2020 2072 6574 7572 6e20 7472 616e 736c     return transl
-0000dea0: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
-0000deb0: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
-0000dec0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-0000ded0: 4b65 7962 6f61 7264 496e 7465 7272 7570  KeyboardInterrup
-0000dee0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-0000def0: 6966 2073 656c 662e 6572 726f 725f 6d65  if self.error_me
-0000df00: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
-0000df10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000df20: 2020 7365 6c66 2e65 7272 6f72 5f6d 6573    self.error_mes
-0000df30: 7361 6765 735f 6361 6c6c 6261 636b 2822  sages_callback("
-0000df40: 4361 6e63 656c 6c69 6e67 2061 6c6c 2074  Cancelling all t
-0000df50: 6173 6b73 2229 0d0a 2020 2020 2020 2020  asks")..        
-0000df60: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0000df70: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000df80: 2822 4361 6e63 656c 6c69 6e67 2061 6c6c  ("Cancelling all
-0000df90: 2074 6173 6b73 2229 0d0a 2020 2020 2020   tasks")..      
-0000dfa0: 2020 2020 2020 7265 7475 726e 0d0a 0d0a        return....
-0000dfb0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-0000dfc0: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
-0000dfd0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000dfe0: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
-0000dff0: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
-0000e000: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e010: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
-0000e020: 735f 6361 6c6c 6261 636b 2865 290d 0a20  s_callback(e).. 
-0000e030: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000e040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e050: 2020 7072 696e 7428 6529 0d0a 2020 2020    print(e)..    
-0000e060: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
-0000e070: 0d0a 0d0a 636c 6173 7320 5375 6274 6974  ....class Subtit
-0000e080: 6c65 466f 726d 6174 7465 723a 0d0a 2020  leFormatter:..  
-0000e090: 2020 7375 7070 6f72 7465 645f 666f 726d    supported_form
-0000e0a0: 6174 7320 3d20 5b27 7372 7427 2c20 2776  ats = ['srt', 'v
-0000e0b0: 7474 272c 2027 6a73 6f6e 272c 2027 7261  tt', 'json', 'ra
-0000e0c0: 7727 5d0d 0a0d 0a20 2020 2064 6566 205f  w']....    def _
-0000e0d0: 5f69 6e69 745f 5f28 7365 6c66 2c20 666f  _init__(self, fo
-0000e0e0: 726d 6174 5f74 7970 652c 2065 7272 6f72  rmat_type, error
-0000e0f0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000e100: 636b 3d4e 6f6e 6529 3a0d 0a20 2020 2020  ck=None):..     
-0000e110: 2020 2073 656c 662e 666f 726d 6174 5f74     self.format_t
-0000e120: 7970 6520 3d20 666f 726d 6174 5f74 7970  ype = format_typ
-0000e130: 652e 6c6f 7765 7228 290d 0a20 2020 2020  e.lower()..     
-0000e140: 2020 2073 656c 662e 6572 726f 725f 6d65     self.error_me
-0000e150: 7373 6167 6573 5f63 616c 6c62 6163 6b20  ssages_callback 
-0000e160: 3d20 6572 726f 725f 6d65 7373 6167 6573  = error_messages
-0000e170: 5f63 616c 6c62 6163 6b0d 0a20 2020 2020  _callback..     
-0000e180: 2020 200d 0a20 2020 2064 6566 205f 5f63     ..    def __c
-0000e190: 616c 6c5f 5f28 7365 6c66 2c20 7375 6274  all__(self, subt
-0000e1a0: 6974 6c65 732c 2070 6164 6469 6e67 5f62  itles, padding_b
-0000e1b0: 6566 6f72 653d 302c 2070 6164 6469 6e67  efore=0, padding
-0000e1c0: 5f61 6674 6572 3d30 293a 0d0a 2020 2020  _after=0):..    
-0000e1d0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-0000e1e0: 2020 2020 2020 6966 2073 656c 662e 666f        if self.fo
-0000e1f0: 726d 6174 5f74 7970 6520 3d3d 2027 7372  rmat_type == 'sr
-0000e200: 7427 3a0d 0a20 2020 2020 2020 2020 2020  t':..           
-0000e210: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000e220: 2e73 7274 5f66 6f72 6d61 7474 6572 2873  .srt_formatter(s
-0000e230: 7562 7469 746c 6573 2c20 7061 6464 696e  ubtitles, paddin
-0000e240: 675f 6265 666f 7265 2c20 7061 6464 696e  g_before, paddin
-0000e250: 675f 6166 7465 7229 0d0a 2020 2020 2020  g_after)..      
-0000e260: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-0000e270: 666f 726d 6174 5f74 7970 6520 3d3d 2027  format_type == '
-0000e280: 7674 7427 3a0d 0a20 2020 2020 2020 2020  vtt':..         
-0000e290: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000e2a0: 6c66 2e76 7474 5f66 6f72 6d61 7474 6572  lf.vtt_formatter
-0000e2b0: 2873 7562 7469 746c 6573 2c20 7061 6464  (subtitles, padd
-0000e2c0: 696e 675f 6265 666f 7265 2c20 7061 6464  ing_before, padd
-0000e2d0: 696e 675f 6166 7465 7229 0d0a 2020 2020  ing_after)..    
-0000e2e0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
-0000e2f0: 662e 666f 726d 6174 5f74 7970 6520 3d3d  f.format_type ==
-0000e300: 2027 6a73 6f6e 273a 0d0a 2020 2020 2020   'json':..      
-0000e310: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000e320: 2073 656c 662e 6a73 6f6e 5f66 6f72 6d61   self.json_forma
-0000e330: 7474 6572 2873 7562 7469 746c 6573 290d  tter(subtitles).
-0000e340: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-0000e350: 6620 7365 6c66 2e66 6f72 6d61 745f 7479  f self.format_ty
-0000e360: 7065 203d 3d20 2772 6177 273a 0d0a 2020  pe == 'raw':..  
-0000e370: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000e380: 7475 726e 2073 656c 662e 7261 775f 666f  turn self.raw_fo
-0000e390: 726d 6174 7465 7228 7375 6274 6974 6c65  rmatter(subtitle
-0000e3a0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-0000e3b0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0000e3c0: 2020 2020 2020 2069 6620 6572 726f 725f         if error_
-0000e3d0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000e3e0: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
-0000e3f0: 2020 2020 2020 2020 6572 726f 725f 6d65          error_me
-0000e400: 7373 6167 6573 5f63 616c 6c62 6163 6b28  ssages_callback(
-0000e410: 6627 556e 7375 7070 6f72 7465 6420 666f  f'Unsupported fo
-0000e420: 726d 6174 2074 7970 653a 207b 7365 6c66  rmat type: {self
-0000e430: 2e66 6f72 6d61 745f 7479 7065 7d27 290d  .format_type}').
-0000e440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e450: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0000e460: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000e470: 6520 5661 6c75 6545 7272 6f72 2866 2755  e ValueError(f'U
-0000e480: 6e73 7570 706f 7274 6564 2066 6f72 6d61  nsupported forma
-0000e490: 7420 7479 7065 3a20 7b73 656c 662e 666f  t type: {self.fo
-0000e4a0: 726d 6174 5f74 7970 657d 2729 0d0a 0d0a  rmat_type}')....
-0000e4b0: 2020 2020 2020 2020 6578 6365 7074 204b          except K
-0000e4c0: 6579 626f 6172 6449 6e74 6572 7275 7074  eyboardInterrupt
-0000e4d0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-0000e4e0: 6620 7365 6c66 2e65 7272 6f72 5f6d 6573  f self.error_mes
-0000e4f0: 7361 6765 735f 6361 6c6c 6261 636b 3a0d  sages_callback:.
-0000e500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e510: 2073 656c 662e 6572 726f 725f 6d65 7373   self.error_mess
-0000e520: 6167 6573 5f63 616c 6c62 6163 6b28 2243  ages_callback("C
-0000e530: 616e 6365 6c6c 696e 6720 616c 6c20 7461  ancelling all ta
-0000e540: 736b 7322 290d 0a20 2020 2020 2020 2020  sks")..         
-0000e550: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0000e560: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000e570: 2243 616e 6365 6c6c 696e 6720 616c 6c20  "Cancelling all 
-0000e580: 7461 736b 7322 290d 0a20 2020 2020 2020  tasks")..       
-0000e590: 2020 2020 2072 6574 7572 6e0d 0a0d 0a20       return.... 
-0000e5a0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-0000e5b0: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
-0000e5c0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000e5d0: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
-0000e5e0: 735f 6361 6c6c 6261 636b 3a0d 0a20 2020  s_callback:..   
-0000e5f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e600: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
-0000e610: 5f63 616c 6c62 6163 6b28 6529 0d0a 2020  _callback(e)..  
-0000e620: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-0000e630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e640: 2070 7269 6e74 2865 290d 0a20 2020 2020   print(e)..     
-0000e650: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
-0000e660: 0a20 2020 2064 6566 2073 7274 5f66 6f72  .    def srt_for
-0000e670: 6d61 7474 6572 2873 656c 662c 2073 7562  matter(self, sub
-0000e680: 7469 746c 6573 2c20 7061 6464 696e 675f  titles, padding_
-0000e690: 6265 666f 7265 3d30 2c20 7061 6464 696e  before=0, paddin
-0000e6a0: 675f 6166 7465 723d 3029 3a0d 0a20 2020  g_after=0):..   
-0000e6b0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000e6c0: 2020 5365 7269 616c 697a 6520 6120 6c69    Serialize a li
-0000e6d0: 7374 206f 6620 7375 6274 6974 6c65 7320  st of subtitles 
-0000e6e0: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
-0000e6f0: 2053 5254 2066 6f72 6d61 742c 2077 6974   SRT format, wit
-0000e700: 6820 6f70 7469 6f6e 616c 2074 696d 6520  h optional time 
-0000e710: 7061 6464 696e 672e 0d0a 2020 2020 2020  padding...      
-0000e720: 2020 2222 220d 0a20 2020 2020 2020 2073    """..        s
-0000e730: 7562 5f72 6970 5f66 696c 6520 3d20 7079  ub_rip_file = py
-0000e740: 7372 742e 5375 6252 6970 4669 6c65 2829  srt.SubRipFile()
-0000e750: 0d0a 2020 2020 2020 2020 666f 7220 692c  ..        for i,
-0000e760: 2028 2873 7461 7274 2c20 656e 6429 2c20   ((start, end), 
-0000e770: 7465 7874 2920 696e 2065 6e75 6d65 7261  text) in enumera
-0000e780: 7465 2873 7562 7469 746c 6573 2c20 7374  te(subtitles, st
-0000e790: 6172 743d 3129 3a0d 0a20 2020 2020 2020  art=1):..       
-0000e7a0: 2020 2020 2069 7465 6d20 3d20 7079 7372       item = pysr
-0000e7b0: 742e 5375 6252 6970 4974 656d 2829 0d0a  t.SubRipItem()..
-0000e7c0: 2020 2020 2020 2020 2020 2020 6974 656d              item
-0000e7d0: 2e69 6e64 6578 203d 2069 0d0a 2020 2020  .index = i..    
-0000e7e0: 2020 2020 2020 2020 6974 656d 2e74 6578          item.tex
-0000e7f0: 7420 3d20 7369 782e 7465 7874 5f74 7970  t = six.text_typ
-0000e800: 6528 7465 7874 290d 0a20 2020 2020 2020  e(text)..       
-0000e810: 2020 2020 2069 7465 6d2e 7374 6172 742e       item.start.
-0000e820: 7365 636f 6e64 7320 3d20 6d61 7828 302c  seconds = max(0,
-0000e830: 2073 7461 7274 202d 2070 6164 6469 6e67   start - padding
-0000e840: 5f62 6566 6f72 6529 0d0a 2020 2020 2020  _before)..      
-0000e850: 2020 2020 2020 6974 656d 2e65 6e64 2e73        item.end.s
-0000e860: 6563 6f6e 6473 203d 2065 6e64 202b 2070  econds = end + p
-0000e870: 6164 6469 6e67 5f61 6674 6572 0d0a 2020  adding_after..  
-0000e880: 2020 2020 2020 2020 2020 7375 625f 7269            sub_ri
-0000e890: 705f 6669 6c65 2e61 7070 656e 6428 6974  p_file.append(it
-0000e8a0: 656d 290d 0a20 2020 2020 2020 2072 6574  em)..        ret
-0000e8b0: 7572 6e20 275c 6e27 2e6a 6f69 6e28 7369  urn '\n'.join(si
-0000e8c0: 782e 7465 7874 5f74 7970 6528 6974 656d  x.text_type(item
-0000e8d0: 2920 666f 7220 6974 656d 2069 6e20 7375  ) for item in su
-0000e8e0: 625f 7269 705f 6669 6c65 290d 0a0d 0a20  b_rip_file).... 
-0000e8f0: 2020 2064 6566 2076 7474 5f66 6f72 6d61     def vtt_forma
-0000e900: 7474 6572 2873 656c 662c 2073 7562 7469  tter(self, subti
-0000e910: 746c 6573 2c20 7061 6464 696e 675f 6265  tles, padding_be
-0000e920: 666f 7265 3d30 2c20 7061 6464 696e 675f  fore=0, padding_
-0000e930: 6166 7465 723d 3029 3a0d 0a20 2020 2020  after=0):..     
-0000e940: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-0000e950: 5365 7269 616c 697a 6520 6120 6c69 7374  Serialize a list
-0000e960: 206f 6620 7375 6274 6974 6c65 7320 6163   of subtitles ac
-0000e970: 636f 7264 696e 6720 746f 2074 6865 2056  cording to the V
-0000e980: 5454 2066 6f72 6d61 742c 2077 6974 6820  TT format, with 
-0000e990: 6f70 7469 6f6e 616c 2074 696d 6520 7061  optional time pa
-0000e9a0: 6464 696e 672e 0d0a 2020 2020 2020 2020  dding...        
-0000e9b0: 2222 220d 0a20 2020 2020 2020 2074 6578  """..        tex
-0000e9c0: 7420 3d20 7365 6c66 2e73 7274 5f66 6f72  t = self.srt_for
-0000e9d0: 6d61 7474 6572 2873 7562 7469 746c 6573  matter(subtitles
-0000e9e0: 2c20 7061 6464 696e 675f 6265 666f 7265  , padding_before
-0000e9f0: 2c20 7061 6464 696e 675f 6166 7465 7229  , padding_after)
-0000ea00: 0d0a 2020 2020 2020 2020 7465 7874 203d  ..        text =
-0000ea10: 2027 5745 4256 5454 5c6e 5c6e 2720 2b20   'WEBVTT\n\n' + 
-0000ea20: 7465 7874 2e72 6570 6c61 6365 2827 2c27  text.replace(','
-0000ea30: 2c20 272e 2729 0d0a 2020 2020 2020 2020  , '.')..        
-0000ea40: 7265 7475 726e 2074 6578 740d 0a0d 0a20  return text.... 
-0000ea50: 2020 2064 6566 206a 736f 6e5f 666f 726d     def json_form
-0000ea60: 6174 7465 7228 7365 6c66 2c20 7375 6274  atter(self, subt
-0000ea70: 6974 6c65 7329 3a0d 0a20 2020 2020 2020  itles):..       
-0000ea80: 2022 2222 0d0a 2020 2020 2020 2020 5365   """..        Se
-0000ea90: 7269 616c 697a 6520 6120 6c69 7374 206f  rialize a list o
-0000eaa0: 6620 7375 6274 6974 6c65 7320 6173 2061  f subtitles as a
-0000eab0: 204a 534f 4e20 626c 6f62 2e0d 0a20 2020   JSON blob...   
-0000eac0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000ead0: 2020 7375 6274 6974 6c65 5f64 6963 7473    subtitle_dicts
-0000eae0: 203d 205b 0d0a 2020 2020 2020 2020 2020   = [..          
-0000eaf0: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-0000eb00: 2020 2020 2027 7374 6172 7427 3a20 7374       'start': st
-0000eb10: 6172 742c 0d0a 2020 2020 2020 2020 2020  art,..          
-0000eb20: 2020 2020 2020 2765 6e64 273a 2065 6e64        'end': end
-0000eb30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000eb40: 2020 2027 636f 6e74 656e 7427 3a20 7465     'content': te
-0000eb50: 7874 2c0d 0a20 2020 2020 2020 2020 2020  xt,..           
-0000eb60: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
-0000eb70: 666f 7220 2828 7374 6172 742c 2065 6e64  for ((start, end
-0000eb80: 292c 2074 6578 7429 0d0a 2020 2020 2020  ), text)..      
-0000eb90: 2020 2020 2020 696e 2073 7562 7469 746c        in subtitl
-0000eba0: 6573 0d0a 2020 2020 2020 2020 5d0d 0a20  es..        ].. 
-0000ebb0: 2020 2020 2020 2072 6574 7572 6e20 6a73         return js
-0000ebc0: 6f6e 2e64 756d 7073 2873 7562 7469 746c  on.dumps(subtitl
-0000ebd0: 655f 6469 6374 7329 0d0a 0d0a 2020 2020  e_dicts)....    
-0000ebe0: 6465 6620 7261 775f 666f 726d 6174 7465  def raw_formatte
-0000ebf0: 7228 7365 6c66 2c20 7375 6274 6974 6c65  r(self, subtitle
-0000ec00: 7329 3a0d 0a20 2020 2020 2020 2022 2222  s):..        """
-0000ec10: 0d0a 2020 2020 2020 2020 5365 7269 616c  ..        Serial
-0000ec20: 697a 6520 6120 6c69 7374 206f 6620 7375  ize a list of su
-0000ec30: 6274 6974 6c65 7320 6173 2061 206e 6577  btitles as a new
-0000ec40: 6c69 6e65 2d64 656c 696d 6974 6564 2073  line-delimited s
-0000ec50: 7472 696e 672e 0d0a 2020 2020 2020 2020  tring...        
-0000ec60: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
-0000ec70: 7572 6e20 2720 272e 6a6f 696e 2874 6578  urn ' '.join(tex
-0000ec80: 7420 666f 7220 285f 726e 672c 2074 6578  t for (_rng, tex
-0000ec90: 7429 2069 6e20 7375 6274 6974 6c65 7329  t) in subtitles)
-0000eca0: 0d0a 0d0a 0d0a 636c 6173 7320 5375 6274  ......class Subt
-0000ecb0: 6974 6c65 5772 6974 6572 3a0d 0a20 2020  itleWriter:..   
-0000ecc0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-0000ecd0: 6c66 2c20 7265 6769 6f6e 732c 2074 7261  lf, regions, tra
-0000ece0: 6e73 6372 6970 7473 2c20 666f 726d 6174  nscripts, format
-0000ecf0: 2c20 6572 726f 725f 6d65 7373 6167 6573  , error_messages
-0000ed00: 5f63 616c 6c62 6163 6b3d 4e6f 6e65 293a  _callback=None):
-0000ed10: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-0000ed20: 6567 696f 6e73 203d 2072 6567 696f 6e73  egions = regions
-0000ed30: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
-0000ed40: 7261 6e73 6372 6970 7473 203d 2074 7261  ranscripts = tra
-0000ed50: 6e73 6372 6970 7473 0d0a 2020 2020 2020  nscripts..      
-0000ed60: 2020 7365 6c66 2e66 6f72 6d61 7420 3d20    self.format = 
-0000ed70: 666f 726d 6174 0d0a 2020 2020 2020 2020  format..        
-0000ed80: 7365 6c66 2e74 696d 6564 5f73 7562 7469  self.timed_subti
-0000ed90: 746c 6573 203d 205b 2872 2c20 7429 2066  tles = [(r, t) f
-0000eda0: 6f72 2072 2c20 7420 696e 207a 6970 2873  or r, t in zip(s
-0000edb0: 656c 662e 7265 6769 6f6e 732c 2073 656c  elf.regions, sel
-0000edc0: 662e 7472 616e 7363 7269 7074 7329 2069  f.transcripts) i
-0000edd0: 6620 745d 0d0a 2020 2020 2020 2020 7365  f t]..        se
-0000ede0: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
-0000edf0: 735f 6361 6c6c 6261 636b 203d 2065 7272  s_callback = err
-0000ee00: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-0000ee10: 6261 636b 0d0a 0d0a 2020 2020 6465 6620  back....    def 
-0000ee20: 6765 745f 7469 6d65 645f 7375 6274 6974  get_timed_subtit
-0000ee30: 6c65 7328 7365 6c66 293a 0d0a 2020 2020  les(self):..    
-0000ee40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000ee50: 7469 6d65 645f 7375 6274 6974 6c65 730d  timed_subtitles.
-0000ee60: 0a0d 0a20 2020 2064 6566 2077 7269 7465  ...    def write
-0000ee70: 2873 656c 662c 2064 6563 6c61 7265 645f  (self, declared_
-0000ee80: 7375 6274 6974 6c65 5f66 696c 6570 6174  subtitle_filepat
-0000ee90: 6829 3a0d 0a20 2020 2020 2020 2074 7279  h):..        try
-0000eea0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-0000eeb0: 6f72 6d61 7474 6572 203d 2053 7562 7469  ormatter = Subti
-0000eec0: 746c 6546 6f72 6d61 7474 6572 2873 656c  tleFormatter(sel
-0000eed0: 662e 666f 726d 6174 290d 0a20 2020 2020  f.format)..     
-0000eee0: 2020 2020 2020 2066 6f72 6d61 7474 6564         formatted
-0000eef0: 5f73 7562 7469 746c 6573 203d 2066 6f72  _subtitles = for
-0000ef00: 6d61 7474 6572 2873 656c 662e 7469 6d65  matter(self.time
-0000ef10: 645f 7375 6274 6974 6c65 7329 0d0a 2020  d_subtitles)..  
-0000ef20: 2020 2020 2020 2020 2020 7361 7665 645f            saved_
-0000ef30: 7375 6274 6974 6c65 5f66 696c 6570 6174  subtitle_filepat
-0000ef40: 6820 3d20 6465 636c 6172 6564 5f73 7562  h = declared_sub
-0000ef50: 7469 746c 655f 6669 6c65 7061 7468 0d0a  title_filepath..
-0000ef60: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000ef70: 6176 6564 5f73 7562 7469 746c 655f 6669  aved_subtitle_fi
-0000ef80: 6c65 7061 7468 3a0d 0a20 2020 2020 2020  lepath:..       
-0000ef90: 2020 2020 2020 2020 2073 7562 7469 746c           subtitl
-0000efa0: 655f 6669 6c65 5f62 6173 652c 2073 7562  e_file_base, sub
-0000efb0: 7469 746c 655f 6669 6c65 5f65 7874 203d  title_file_ext =
-0000efc0: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
-0000efd0: 7428 7361 7665 645f 7375 6274 6974 6c65  t(saved_subtitle
-0000efe0: 5f66 696c 6570 6174 6829 0d0a 2020 2020  _filepath)..    
-0000eff0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000f000: 6f74 2073 7562 7469 746c 655f 6669 6c65  ot subtitle_file
-0000f010: 5f65 7874 3a0d 0a20 2020 2020 2020 2020  _ext:..         
-0000f020: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-0000f030: 5f73 7562 7469 746c 655f 6669 6c65 7061  _subtitle_filepa
-0000f040: 7468 203d 2022 7b62 6173 657d 2e7b 666f  th = "{base}.{fo
-0000f050: 726d 6174 7d22 2e66 6f72 6d61 7428 6261  rmat}".format(ba
-0000f060: 7365 3d73 7562 7469 746c 655f 6669 6c65  se=subtitle_file
-0000f070: 5f62 6173 652c 2066 6f72 6d61 743d 7365  _base, format=se
-0000f080: 6c66 2e66 6f72 6d61 7429 0d0a 2020 2020  lf.format)..    
-0000f090: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000f0a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000f0b0: 2020 2020 2020 2073 6176 6564 5f73 7562         saved_sub
-0000f0c0: 7469 746c 655f 6669 6c65 7061 7468 203d  title_filepath =
-0000f0d0: 2064 6563 6c61 7265 645f 7375 6274 6974   declared_subtit
-0000f0e0: 6c65 5f66 696c 6570 6174 680d 0a20 2020  le_filepath..   
-0000f0f0: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-0000f100: 656e 2873 6176 6564 5f73 7562 7469 746c  en(saved_subtitl
-0000f110: 655f 6669 6c65 7061 7468 2c20 2777 6227  e_filepath, 'wb'
-0000f120: 2920 6173 2066 3a0d 0a20 2020 2020 2020  ) as f:..       
-0000f130: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-0000f140: 2866 6f72 6d61 7474 6564 5f73 7562 7469  (formatted_subti
-0000f150: 746c 6573 2e65 6e63 6f64 6528 2275 7466  tles.encode("utf
-0000f160: 2d38 2229 290d 0a20 2020 2020 2020 2020  -8"))..         
-0000f170: 2020 2023 7769 7468 206f 7065 6e28 7361     #with open(sa
-0000f180: 7665 645f 7375 6274 6974 6c65 5f66 696c  ved_subtitle_fil
-0000f190: 6570 6174 682c 2027 6127 2920 6173 2066  epath, 'a') as f
-0000f1a0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-0000f1b0: 2020 2020 662e 7772 6974 6528 225c 6e22      f.write("\n"
-0000f1c0: 290d 0a0d 0a20 2020 2020 2020 2065 7863  )....        exc
-0000f1d0: 6570 7420 4b65 7962 6f61 7264 496e 7465  ept KeyboardInte
-0000f1e0: 7272 7570 743a 0d0a 2020 2020 2020 2020  rrupt:..        
-0000f1f0: 2020 2020 6966 2073 656c 662e 6572 726f      if self.erro
-0000f200: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000f210: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
-0000f220: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
-0000f230: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000f240: 636b 2822 4361 6e63 656c 6c69 6e67 2061  ck("Cancelling a
-0000f250: 6c6c 2074 6173 6b73 2229 0d0a 2020 2020  ll tasks")..    
-0000f260: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0000f270: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000f280: 7269 6e74 2822 4361 6e63 656c 6c69 6e67  rint("Cancelling
-0000f290: 2061 6c6c 2074 6173 6b73 2229 0d0a 2020   all tasks")..  
-0000f2a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000f2b0: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
-0000f2c0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-0000f2d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000f2e0: 6966 2073 656c 662e 6572 726f 725f 6d65  if self.error_me
-0000f2f0: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
-0000f300: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f310: 2020 7365 6c66 2e65 7272 6f72 5f6d 6573    self.error_mes
-0000f320: 7361 6765 735f 6361 6c6c 6261 636b 2865  sages_callback(e
-0000f330: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-0000f340: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0000f350: 2020 2020 2020 7072 696e 7428 6529 0d0a        print(e)..
-0000f360: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000f370: 726e 0d0a 0d0a 0d0a 636c 6173 7320 5352  rn......class SR
-0000f380: 5446 696c 6552 6561 6465 723a 0d0a 2020  TFileReader:..  
-0000f390: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0000f3a0: 656c 662c 2073 7274 5f66 696c 655f 7061  elf, srt_file_pa
-0000f3b0: 7468 2c20 6572 726f 725f 6d65 7373 6167  th, error_messag
-0000f3c0: 6573 5f63 616c 6c62 6163 6b3d 4e6f 6e65  es_callback=None
-0000f3d0: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
-0000f3e0: 2e74 696d 6564 5f73 7562 7469 746c 6573  .timed_subtitles
-0000f3f0: 203d 2073 656c 6628 7372 745f 6669 6c65   = self(srt_file
-0000f400: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
-0000f410: 7365 6c66 2e65 7272 6f72 5f6d 6573 7361  self.error_messa
-0000f420: 6765 735f 6361 6c6c 6261 636b 203d 2065  ges_callback = e
-0000f430: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000f440: 6c6c 6261 636b 0d0a 0d0a 2020 2020 4073  llback....    @s
-0000f450: 7461 7469 636d 6574 686f 640d 0a20 2020  taticmethod..   
-0000f460: 2064 6566 205f 5f63 616c 6c5f 5f28 7372   def __call__(sr
-0000f470: 745f 6669 6c65 5f70 6174 6829 3a0d 0a20  t_file_path):.. 
-0000f480: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-0000f490: 2020 2020 2020 2020 2022 2222 0d0a 2020           """..  
-0000f4a0: 2020 2020 2020 2020 2020 5265 6164 2053            Read S
-0000f4b0: 5254 2066 6f72 6d61 7474 6564 2073 7562  RT formatted sub
-0000f4c0: 7469 746c 6520 6669 6c65 2061 6e64 2072  title file and r
-0000f4d0: 6574 7572 6e20 7375 6274 6974 6c65 7320  eturn subtitles 
-0000f4e0: 6173 206c 6973 7420 6f66 2074 7570 6c65  as list of tuple
-0000f4f0: 730d 0a20 2020 2020 2020 2020 2020 2022  s..            "
-0000f500: 2222 0d0a 2020 2020 2020 2020 2020 2020  ""..            
-0000f510: 7469 6d65 645f 7375 6274 6974 6c65 7320  timed_subtitles 
-0000f520: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-0000f530: 2020 7769 7468 206f 7065 6e28 7372 745f    with open(srt_
-0000f540: 6669 6c65 5f70 6174 682c 2027 7227 2920  file_path, 'r') 
-0000f550: 6173 2073 7274 5f66 696c 653a 0d0a 2020  as srt_file:..  
-0000f560: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000f570: 6e65 7320 3d20 7372 745f 6669 6c65 2e72  nes = srt_file.r
-0000f580: 6561 646c 696e 6573 2829 0d0a 2020 2020  eadlines()..    
-0000f590: 2020 2020 2020 2020 2020 2020 2320 5370              # Sp
-0000f5a0: 6c69 7420 7468 6520 7375 6274 6974 6c65  lit the subtitle
-0000f5b0: 2066 696c 6520 696e 746f 2073 7562 7469   file into subti
-0000f5c0: 746c 6520 626c 6f63 6b73 0d0a 2020 2020  tle blocks..    
-0000f5d0: 2020 2020 2020 2020 2020 2020 7375 6274              subt
-0000f5e0: 6974 6c65 5f62 6c6f 636b 7320 3d20 5b5d  itle_blocks = []
-0000f5f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f600: 2020 626c 6f63 6b20 3d20 5b5d 0d0a 2020    block = []..  
-0000f610: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000f620: 7220 6c69 6e65 2069 6e20 6c69 6e65 733a  r line in lines:
-0000f630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f640: 2020 2020 2020 6966 206c 696e 652e 7374        if line.st
-0000f650: 7269 7028 2920 3d3d 2027 273a 0d0a 2020  rip() == '':..  
-0000f660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f670: 2020 2020 2020 7375 6274 6974 6c65 5f62        subtitle_b
-0000f680: 6c6f 636b 732e 6170 7065 6e64 2862 6c6f  locks.append(blo
-0000f690: 636b 290d 0a20 2020 2020 2020 2020 2020  ck)..           
-0000f6a0: 2020 2020 2020 2020 2020 2020 2062 6c6f               blo
-0000f6b0: 636b 203d 205b 5d0d 0a20 2020 2020 2020  ck = []..       
-0000f6c0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000f6d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000f6e0: 2020 2020 2020 2020 2020 2020 626c 6f63              bloc
-0000f6f0: 6b2e 6170 7065 6e64 286c 696e 652e 7374  k.append(line.st
-0000f700: 7269 7028 2929 0d0a 2020 2020 2020 2020  rip())..        
-0000f710: 2020 2020 2020 2020 7375 6274 6974 6c65          subtitle
-0000f720: 5f62 6c6f 636b 732e 6170 7065 6e64 2862  _blocks.append(b
-0000f730: 6c6f 636b 290d 0a0d 0a20 2020 2020 2020  lock)....       
-0000f740: 2020 2020 2020 2020 2023 2050 6172 7365           # Parse
-0000f750: 2065 6163 6820 7375 6274 6974 6c65 2062   each subtitle b
-0000f760: 6c6f 636b 2061 6e64 2073 746f 7265 2061  lock and store a
-0000f770: 7320 7475 706c 6520 696e 2074 696d 6564  s tuple in timed
-0000f780: 5f73 7562 7469 746c 6573 206c 6973 740d  _subtitles list.
-0000f790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f7a0: 2066 6f72 2062 6c6f 636b 2069 6e20 7375   for block in su
-0000f7b0: 6274 6974 6c65 5f62 6c6f 636b 733a 0d0a  btitle_blocks:..
-0000f7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7d0: 2020 2020 6966 2062 6c6f 636b 3a0d 0a20      if block:.. 
-0000f7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7f0: 2020 2020 2020 2023 2045 7874 7261 6374         # Extract
-0000f800: 2073 7461 7274 2061 6e64 2065 6e64 2074   start and end t
-0000f810: 696d 6573 2066 726f 6d20 7375 6274 6974  imes from subtit
-0000f820: 6c65 2062 6c6f 636b 0d0a 2020 2020 2020  le block..      
-0000f830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f840: 2020 7374 6172 745f 7469 6d65 5f73 7472    start_time_str
-0000f850: 2c20 656e 645f 7469 6d65 5f73 7472 203d  , end_time_str =
-0000f860: 2062 6c6f 636b 5b31 5d2e 7370 6c69 7428   block[1].split(
-0000f870: 2720 2d2d 3e20 2729 0d0a 2020 2020 2020  ' --> ')..      
-0000f880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f890: 2020 7469 6d65 5f66 6f72 6d61 7420 3d20    time_format = 
-0000f8a0: 2725 483a 254d 3a25 532c 2566 270d 0a20  '%H:%M:%S,%f'.. 
-0000f8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8c0: 2020 2020 2020 2073 7461 7274 5f74 696d         start_tim
-0000f8d0: 655f 7469 6d65 5f64 656c 7461 203d 2064  e_time_delta = d
-0000f8e0: 6174 6574 696d 652e 7374 7270 7469 6d65  atetime.strptime
-0000f8f0: 2873 7461 7274 5f74 696d 655f 7374 722c  (start_time_str,
-0000f900: 2074 696d 655f 666f 726d 6174 2920 2d20   time_format) - 
-0000f910: 6461 7465 7469 6d65 2e73 7472 7074 696d  datetime.strptim
-0000f920: 6528 2730 303a 3030 3a30 302c 3030 3027  e('00:00:00,000'
-0000f930: 2c20 7469 6d65 5f66 6f72 6d61 7429 0d0a  , time_format)..
-0000f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f950: 2020 2020 2020 2020 7374 6172 745f 7469          start_ti
-0000f960: 6d65 5f74 6f74 616c 5f73 6563 6f6e 6473  me_total_seconds
-0000f970: 203d 2073 7461 7274 5f74 696d 655f 7469   = start_time_ti
-0000f980: 6d65 5f64 656c 7461 2e74 6f74 616c 5f73  me_delta.total_s
-0000f990: 6563 6f6e 6473 2829 0d0a 2020 2020 2020  econds()..      
-0000f9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9b0: 2020 656e 645f 7469 6d65 5f74 696d 655f    end_time_time_
-0000f9c0: 6465 6c74 6120 3d20 6461 7465 7469 6d65  delta = datetime
-0000f9d0: 2e73 7472 7074 696d 6528 656e 645f 7469  .strptime(end_ti
-0000f9e0: 6d65 5f73 7472 2c20 7469 6d65 5f66 6f72  me_str, time_for
-0000f9f0: 6d61 7429 202d 2064 6174 6574 696d 652e  mat) - datetime.
-0000fa00: 7374 7270 7469 6d65 2827 3030 3a30 303a  strptime('00:00:
-0000fa10: 3030 2c30 3030 272c 2074 696d 655f 666f  00,000', time_fo
-0000fa20: 726d 6174 290d 0a20 2020 2020 2020 2020  rmat)..         
-0000fa30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000fa40: 6e64 5f74 696d 655f 746f 7461 6c5f 7365  nd_time_total_se
-0000fa50: 636f 6e64 7320 3d20 656e 645f 7469 6d65  conds = end_time
-0000fa60: 5f74 696d 655f 6465 6c74 612e 746f 7461  _time_delta.tota
-0000fa70: 6c5f 7365 636f 6e64 7328 290d 0a20 2020  l_seconds()..   
-0000fa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa90: 2020 2020 2023 2045 7874 7261 6374 2073       # Extract s
-0000faa0: 7562 7469 746c 6520 7465 7874 2066 726f  ubtitle text fro
-0000fab0: 6d20 7375 6274 6974 6c65 2062 6c6f 636b  m subtitle block
-0000fac0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fad0: 2020 2020 2020 2020 2020 7375 6274 6974            subtit
-0000fae0: 6c65 203d 2027 2027 2e6a 6f69 6e28 626c  le = ' '.join(bl
-0000faf0: 6f63 6b5b 323a 5d29 0d0a 2020 2020 2020  ock[2:])..      
-0000fb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb10: 2020 7469 6d65 645f 7375 6274 6974 6c65    timed_subtitle
-0000fb20: 732e 6170 7065 6e64 2828 2873 7461 7274  s.append(((start
-0000fb30: 5f74 696d 655f 746f 7461 6c5f 7365 636f  _time_total_seco
-0000fb40: 6e64 732c 2065 6e64 5f74 696d 655f 746f  nds, end_time_to
-0000fb50: 7461 6c5f 7365 636f 6e64 7329 2c20 7375  tal_seconds), su
-0000fb60: 6274 6974 6c65 2929 0d0a 2020 2020 2020  btitle))..      
-0000fb70: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000fb80: 2074 696d 6564 5f73 7562 7469 746c 6573   timed_subtitles
-0000fb90: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
-0000fba0: 7074 204b 6579 626f 6172 6449 6e74 6572  pt KeyboardInter
-0000fbb0: 7275 7074 3a0d 0a20 2020 2020 2020 2020  rupt:..         
-0000fbc0: 2020 2069 6620 7365 6c66 2e65 7272 6f72     if self.error
-0000fbd0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000fbe0: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
-0000fbf0: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
-0000fc00: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000fc10: 6b28 2243 616e 6365 6c6c 696e 6720 616c  k("Cancelling al
-0000fc20: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
-0000fc30: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0000fc40: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000fc50: 696e 7428 2243 616e 6365 6c6c 696e 6720  int("Cancelling 
-0000fc60: 616c 6c20 7461 736b 7322 290d 0a20 2020  all tasks")..   
-0000fc70: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
-0000fc80: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
-0000fc90: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-0000fca0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-0000fcb0: 6620 7365 6c66 2e65 7272 6f72 5f6d 6573  f self.error_mes
-0000fcc0: 7361 6765 735f 6361 6c6c 6261 636b 3a0d  sages_callback:.
-0000fcd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fce0: 2073 656c 662e 6572 726f 725f 6d65 7373   self.error_mess
-0000fcf0: 6167 6573 5f63 616c 6c62 6163 6b28 6529  ages_callback(e)
-0000fd00: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0000fd10: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000fd20: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
-0000fd30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000fd40: 6e0d 0a0d 0a0d 0a64 6566 2073 686f 775f  n......def show_
-0000fd50: 7072 6f67 7265 7373 286d 6564 6961 5f66  progress(media_f
-0000fd60: 696c 6570 6174 682c 2070 726f 6772 6573  ilepath, progres
-0000fd70: 7329 3a0d 0a20 2020 2067 6c6f 6261 6c20  s):..    global 
-0000fd80: 7062 6172 0d0a 2020 2020 7062 6172 2e75  pbar..    pbar.u
-0000fd90: 7064 6174 6528 7072 6f67 7265 7373 290d  pdate(progress).
-0000fda0: 0a0d 0a0d 0a64 6566 2073 686f 775f 6572  .....def show_er
-0000fdb0: 726f 725f 6d65 7373 6167 6573 286d 6573  ror_messages(mes
-0000fdc0: 7361 6765 7329 3a0d 0a20 2020 2070 7269  sages):..    pri
-0000fdd0: 6e74 286d 6573 7361 6765 7329 0d0a 0d0a  nt(messages)....
-0000fde0: 0d0a 6465 6620 6d61 696e 2829 3a0d 0a20  ..def main():.. 
-0000fdf0: 2020 2067 6c6f 6261 6c20 7062 6172 0d0a     global pbar..
-0000fe00: 0d0a 2020 2020 6966 2073 7973 2e70 6c61  ..    if sys.pla
-0000fe10: 7466 6f72 6d20 3d3d 2022 7769 6e33 3222  tform == "win32"
-0000fe20: 3a0d 0a20 2020 2020 2020 2073 746f 705f  :..        stop_
-0000fe30: 6666 6d70 6567 5f77 696e 646f 7773 2865  ffmpeg_windows(e
-0000fe40: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000fe50: 6c6c 6261 636b 3d73 686f 775f 6572 726f  llback=show_erro
-0000fe60: 725f 6d65 7373 6167 6573 290d 0a20 2020  r_messages)..   
-0000fe70: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0000fe80: 7374 6f70 5f66 666d 7065 675f 6c69 6e75  stop_ffmpeg_linu
-0000fe90: 7828 6572 726f 725f 6d65 7373 6167 6573  x(error_messages
-0000fea0: 5f63 616c 6c62 6163 6b3d 7368 6f77 5f65  _callback=show_e
-0000feb0: 7272 6f72 5f6d 6573 7361 6765 7329 0d0a  rror_messages)..
-0000fec0: 0d0a 2020 2020 7265 6d6f 7665 5f74 656d  ..    remove_tem
-0000fed0: 705f 6669 6c65 7328 2266 6c61 6322 2c20  p_files("flac", 
-0000fee0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-0000fef0: 616c 6c62 6163 6b3d 7368 6f77 5f65 7272  allback=show_err
-0000ff00: 6f72 5f6d 6573 7361 6765 7329 0d0a 2020  or_messages)..  
-0000ff10: 2020 7265 6d6f 7665 5f74 656d 705f 6669    remove_temp_fi
-0000ff20: 6c65 7328 2277 6176 222c 2065 7272 6f72  les("wav", error
-0000ff30: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000ff40: 636b 3d73 686f 775f 6572 726f 725f 6d65  ck=show_error_me
-0000ff50: 7373 6167 6573 290d 0a0d 0a20 2020 2070  ssages)....    p
-0000ff60: 6172 7365 7220 3d20 6172 6770 6172 7365  arser = argparse
-0000ff70: 2e41 7267 756d 656e 7450 6172 7365 7228  .ArgumentParser(
-0000ff80: 290d 0a20 2020 2070 6172 7365 722e 6164  )..    parser.ad
-0000ff90: 645f 6172 6775 6d65 6e74 2827 736f 7572  d_argument('sour
-0000ffa0: 6365 5f70 6174 6827 2c20 6865 6c70 3d22  ce_path', help="
-0000ffb0: 5061 7468 2074 6f20 7468 6520 7669 6465  Path to the vide
-0000ffc0: 6f20 6f72 2061 7564 696f 2066 696c 6573  o or audio files
-0000ffd0: 2074 6f20 6765 6e65 7261 7465 2073 7562   to generate sub
-0000ffe0: 7469 746c 6573 2066 696c 6573 2028 7573  titles files (us
-0000fff0: 6520 7769 6c64 6361 7264 2066 6f72 206d  e wildcard for m
-00010000: 756c 7469 706c 6520 6669 6c65 7320 6f72  ultiple files or
-00010010: 2073 6570 6172 6174 6520 7468 656d 2077   separate them w
-00010020: 6974 6820 6120 7370 6163 6520 6368 6172  ith a space char
-00010030: 6163 7465 7220 652e 672e 205c 2266 696c  acter e.g. \"fil
-00010040: 6520 312e 6d70 345c 2220 5c22 6669 6c65  e 1.mp4\" \"file
-00010050: 2032 2e6d 7034 5c22 2922 2c20 6e61 7267   2.mp4\")", narg
-00010060: 733d 272a 2729 0d0a 2020 2020 7061 7273  s='*')..    pars
-00010070: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-00010080: 272d 6d27 2c20 272d 2d6d 6f64 656c 2d6e  '-m', '--model-n
-00010090: 616d 6527 2c20 6465 6661 756c 743d 2273  ame', default="s
-000100a0: 6d61 6c6c 222c 2068 656c 703d 226e 616d  mall", help="nam
-000100b0: 6520 6f66 2074 6865 2057 6869 7370 6572  e of the Whisper
-000100c0: 206d 6f64 656c 2074 6f20 7573 6522 290d   model to use").
-000100d0: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
-000100e0: 6172 6775 6d65 6e74 2827 2d6c 6d27 2c20  argument('-lm', 
-000100f0: 272d 2d6c 6973 742d 6d6f 6465 6c73 272c  '--list-models',
-00010100: 2068 656c 703d 224c 6973 7420 6f66 2057   help="List of W
-00010110: 6869 7370 6572 206d 6f64 656c 7320 6e61  hisper models na
-00010120: 6d65 222c 2061 6374 696f 6e3d 2773 746f  me", action='sto
-00010130: 7265 5f74 7275 6527 290d 0a20 2020 2070  re_true')..    p
-00010140: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-00010150: 6e74 2827 2d53 272c 2027 2d2d 7372 632d  nt('-S', '--src-
-00010160: 6c61 6e67 7561 6765 272c 2068 656c 703d  language', help=
-00010170: 224c 616e 6775 6167 6520 636f 6465 206f  "Language code o
-00010180: 6620 7468 6520 6175 6469 6f20 6c61 6e67  f the audio lang
-00010190: 7561 6765 2073 706f 6b65 6e20 696e 2076  uage spoken in v
-000101a0: 6964 656f 2f61 7564 696f 2073 6f75 7263  ideo/audio sourc
-000101b0: 655f 7061 7468 222c 2064 6566 6175 6c74  e_path", default
-000101c0: 3d22 656e 2229 0d0a 2020 2020 7061 7273  ="en")..    pars
-000101d0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-000101e0: 272d 4427 2c20 272d 2d64 7374 2d6c 616e  '-D', '--dst-lan
-000101f0: 6775 6167 6527 2c20 6865 6c70 3d22 4465  guage', help="De
-00010200: 7369 7265 6420 7472 616e 736c 6174 696f  sired translatio
-00010210: 6e20 6c61 6e67 7561 6765 2063 6f64 6520  n language code 
-00010220: 666f 7220 7468 6520 7375 6274 6974 6c65  for the subtitle
-00010230: 7322 2c20 6465 6661 756c 743d 4e6f 6e65  s", default=None
-00010240: 290d 0a20 2020 2070 6172 7365 722e 6164  )..    parser.ad
-00010250: 645f 6172 6775 6d65 6e74 2827 2d6c 776c  d_argument('-lwl
-00010260: 272c 2027 2d2d 6c69 7374 2d77 6869 7370  ', '--list-whisp
-00010270: 6572 2d6c 616e 6775 6167 6573 272c 2068  er-languages', h
-00010280: 656c 703d 224c 6973 7420 616c 6c20 7768  elp="List all wh
-00010290: 6973 7065 7220 7375 7070 6f72 7465 6420  isper supported 
-000102a0: 6c61 6e67 7561 6765 7322 2c20 6163 7469  languages", acti
-000102b0: 6f6e 3d27 7374 6f72 655f 7472 7565 2729  on='store_true')
-000102c0: 0d0a 2020 2020 7061 7273 6572 2e61 6464  ..    parser.add
-000102d0: 5f61 7267 756d 656e 7428 272d 6c67 6c27  _argument('-lgl'
-000102e0: 2c20 272d 2d6c 6973 742d 676f 6f67 6c65  , '--list-google
-000102f0: 2d6c 616e 6775 6167 6573 272c 2068 656c  -languages', hel
-00010300: 703d 224c 6973 7420 616c 6c20 676f 6f67  p="List all goog
-00010310: 6c65 2074 7261 6e73 6c61 7465 2073 7570  le translate sup
-00010320: 706f 7274 6564 206c 616e 6775 6167 6573  ported languages
-00010330: 222c 2061 6374 696f 6e3d 2773 746f 7265  ", action='store
-00010340: 5f74 7275 6527 290d 0a20 2020 2070 6172  _true')..    par
-00010350: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
-00010360: 2827 2d46 272c 2027 2d2d 666f 726d 6174  ('-F', '--format
-00010370: 272c 2068 656c 703d 2244 6573 6972 6564  ', help="Desired
-00010380: 2073 7562 7469 746c 6520 666f 726d 6174   subtitle format
-00010390: 222c 2064 6566 6175 6c74 3d22 7372 7422  ", default="srt"
-000103a0: 290d 0a20 2020 2070 6172 7365 722e 6164  )..    parser.ad
-000103b0: 645f 6172 6775 6d65 6e74 2827 2d6c 6627  d_argument('-lf'
-000103c0: 2c20 272d 2d6c 6973 742d 666f 726d 6174  , '--list-format
-000103d0: 7327 2c20 6865 6c70 3d22 4c69 7374 2061  s', help="List a
-000103e0: 6c6c 2073 7570 706f 7274 6564 2073 7562  ll supported sub
-000103f0: 7469 746c 6520 666f 726d 6174 7322 2c20  title formats", 
-00010400: 6163 7469 6f6e 3d27 7374 6f72 655f 7472  action='store_tr
-00010410: 7565 2729 0d0a 2020 2020 7061 7273 6572  ue')..    parser
-00010420: 2e61 6464 5f61 7267 756d 656e 7428 272d  .add_argument('-
-00010430: 4327 2c20 272d 2d63 6f6e 6375 7272 656e  C', '--concurren
-00010440: 6379 272c 2068 656c 703d 224e 756d 6265  cy', help="Numbe
-00010450: 7220 6f66 2063 6f6e 6375 7272 656e 7420  r of concurrent 
-00010460: 4150 4920 7265 7175 6573 7473 2074 6f20  API requests to 
-00010470: 6d61 6b65 222c 2074 7970 653d 696e 742c  make", type=int,
-00010480: 2064 6566 6175 6c74 3d31 3029 0d0a 2020   default=10)..  
-00010490: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-000104a0: 756d 656e 7428 272d 7627 2c20 272d 2d76  ument('-v', '--v
-000104b0: 6572 7369 6f6e 272c 2061 6374 696f 6e3d  ersion', action=
-000104c0: 2776 6572 7369 6f6e 272c 2076 6572 7369  'version', versi
-000104d0: 6f6e 3d56 4552 5349 4f4e 290d 0a0d 0a20  on=VERSION).... 
-000104e0: 2020 2061 7267 7320 3d20 7061 7273 6572     args = parser
-000104f0: 2e70 6172 7365 5f61 7267 7328 290d 0a0d  .parse_args()...
-00010500: 0a20 2020 2073 7263 5f6c 616e 6775 6167  .    src_languag
-00010510: 6520 3d20 6172 6773 2e73 7263 5f6c 616e  e = args.src_lan
-00010520: 6775 6167 650d 0a20 2020 2064 7374 5f6c  guage..    dst_l
-00010530: 616e 6775 6167 6520 3d20 6172 6773 2e64  anguage = args.d
-00010540: 7374 5f6c 616e 6775 6167 650d 0a0d 0a20  st_language.... 
-00010550: 2020 206d 6f64 656c 5f6e 616d 6520 3d20     model_name = 
-00010560: 6172 6773 2e6d 6f64 656c 5f6e 616d 650d  args.model_name.
-00010570: 0a20 2020 2069 6620 6d6f 6465 6c5f 6e61  .    if model_na
-00010580: 6d65 2e65 6e64 7377 6974 6828 222e 656e  me.endswith(".en
-00010590: 2229 3a0d 0a20 2020 2020 2020 2070 7269  "):..        pri
-000105a0: 6e74 2866 227b 6d6f 6465 6c5f 6e61 6d65  nt(f"{model_name
-000105b0: 7d20 6973 2061 6e20 456e 676c 6973 682d  } is an English-
-000105c0: 6f6e 6c79 206d 6f64 656c 2c20 666f 7263  only model, forc
-000105d0: 696e 6720 456e 676c 6973 6820 6465 7465  ing English dete
-000105e0: 6374 696f 6e2e 2229 0d0a 2020 2020 2020  ction.")..      
-000105f0: 2020 6172 6773 2e73 7263 5f6c 616e 6775    args.src_langu
-00010600: 6167 6520 3d20 2265 6e22 0d0a 2020 2020  age = "en"..    
-00010610: 656c 6966 2061 7267 732e 7372 635f 6c61  elif args.src_la
-00010620: 6e67 7561 6765 2021 3d20 2261 7574 6f22  nguage != "auto"
-00010630: 3a0d 0a20 2020 2020 2020 2061 7267 732e  :..        args.
-00010640: 7372 635f 6c61 6e67 7561 6765 203d 2073  src_language = s
-00010650: 7263 5f6c 616e 6775 6167 650d 0a0d 0a20  rc_language.... 
-00010660: 2020 206d 6f64 656c 203d 2077 6869 7370     model = whisp
-00010670: 6572 2e6c 6f61 645f 6d6f 6465 6c28 6d6f  er.load_model(mo
-00010680: 6465 6c5f 6e61 6d65 290d 0a0d 0a20 2020  del_name)....   
-00010690: 2069 6620 6172 6773 2e6c 6973 745f 6d6f   if args.list_mo
-000106a0: 6465 6c73 3a0d 0a20 2020 2020 2020 2070  dels:..        p
-000106b0: 7269 6e74 2822 4c69 7374 206f 6620 7768  rint("List of wh
-000106c0: 6973 7065 7220 6d6f 6465 6c73 3a22 290d  isper models:").
-000106d0: 0a20 2020 2020 2020 2066 6f72 206d 6f64  .        for mod
-000106e0: 656c 5f6e 616d 6520 696e 2077 6869 7370  el_name in whisp
-000106f0: 6572 2e61 7661 696c 6162 6c65 5f6d 6f64  er.available_mod
-00010700: 656c 7328 293a 0d0a 2020 2020 2020 2020  els():..        
-00010710: 2020 2020 7072 696e 7428 6d6f 6465 6c5f      print(model_
-00010720: 6e61 6d65 290d 0a20 2020 2020 2020 2072  name)..        r
-00010730: 6574 7572 6e20 300d 0a0d 0a20 2020 2077  eturn 0....    w
-00010740: 6869 7370 6572 5f6c 616e 6775 6167 6520  hisper_language 
-00010750: 3d20 5768 6973 7065 724c 616e 6775 6167  = WhisperLanguag
-00010760: 6528 290d 0a20 2020 2067 6f6f 676c 655f  e()..    google_
-00010770: 6c61 6e67 7561 6765 203d 2047 6f6f 676c  language = Googl
-00010780: 654c 616e 6775 6167 6528 290d 0a0d 0a20  eLanguage().... 
-00010790: 2020 2069 6620 6172 6773 2e6c 6973 745f     if args.list_
-000107a0: 7768 6973 7065 725f 6c61 6e67 7561 6765  whisper_language
-000107b0: 733a 0d0a 2020 2020 2020 2020 7072 696e  s:..        prin
-000107c0: 7428 224c 6973 7420 6f66 2077 6869 7370  t("List of whisp
-000107d0: 6572 2073 7570 706f 7274 6564 206c 616e  er supported lan
-000107e0: 6775 6167 6573 3a22 290d 0a20 2020 2020  guages:")..     
-000107f0: 2020 2066 6f72 2077 6869 7370 6572 5f63     for whisper_c
-00010800: 6f64 652c 2077 6869 7370 6572 5f6c 616e  ode, whisper_lan
-00010810: 6775 6167 6520 696e 2073 6f72 7465 6428  guage in sorted(
-00010820: 7768 6973 7065 725f 6c61 6e67 7561 6765  whisper_language
-00010830: 2e6e 616d 655f 6f66 5f63 6f64 652e 6974  .name_of_code.it
-00010840: 656d 7328 2929 3a0d 0a20 2020 2020 2020  ems()):..       
-00010850: 2020 2020 2070 7269 6e74 2822 252d 3873       print("%-8s
-00010860: 203a 2025 7322 2025 2877 6869 7370 6572   : %s" %(whisper
-00010870: 5f63 6f64 652c 2077 6869 7370 6572 5f6c  _code, whisper_l
-00010880: 616e 6775 6167 6529 290d 0a20 2020 2020  anguage))..     
-00010890: 2020 2072 6574 7572 6e20 300d 0a0d 0a20     return 0.... 
-000108a0: 2020 2069 6620 6172 6773 2e6c 6973 745f     if args.list_
-000108b0: 676f 6f67 6c65 5f6c 616e 6775 6167 6573  google_languages
-000108c0: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
-000108d0: 2822 4c69 7374 206f 6620 676f 6f67 6c65  ("List of google
-000108e0: 2074 7261 6e73 6c61 7465 2073 7570 706f   translate suppo
-000108f0: 7274 6564 206c 616e 6775 6167 6573 3a22  rted languages:"
-00010900: 290d 0a20 2020 2020 2020 2066 6f72 2067  )..        for g
-00010910: 6f6f 676c 655f 636f 6465 2c20 676f 6f67  oogle_code, goog
-00010920: 6c65 5f6c 616e 6775 6167 6520 696e 2073  le_language in s
-00010930: 6f72 7465 6428 676f 6f67 6c65 5f6c 616e  orted(google_lan
-00010940: 6775 6167 652e 6e61 6d65 5f6f 665f 636f  guage.name_of_co
-00010950: 6465 2e69 7465 6d73 2829 293a 0d0a 2020  de.items()):..  
-00010960: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00010970: 2225 2d38 7320 3a20 2573 2220 2528 676f  "%-8s : %s" %(go
-00010980: 6f67 6c65 5f63 6f64 652c 2067 6f6f 676c  ogle_code, googl
-00010990: 655f 6c61 6e67 7561 6765 2929 0d0a 2020  e_language))..  
-000109a0: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
-000109b0: 0d0a 2020 2020 6966 2061 7267 732e 7372  ..    if args.sr
-000109c0: 635f 6c61 6e67 7561 6765 206e 6f74 2069  c_language not i
-000109d0: 6e20 7768 6973 7065 725f 6c61 6e67 7561  n whisper_langua
-000109e0: 6765 2e6e 616d 655f 6f66 5f63 6f64 652e  ge.name_of_code.
-000109f0: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
-00010a00: 2070 7269 6e74 2822 536f 7572 6365 206c   print("Source l
-00010a10: 616e 6775 6167 6520 6973 206e 6f74 2073  anguage is not s
-00010a20: 7570 706f 7274 6564 2e20 5275 6e20 7769  upported. Run wi
-00010a30: 7468 202d 2d6c 6973 742d 7768 6973 7065  th --list-whispe
-00010a40: 722d 6c61 6e67 7561 6765 7320 746f 2073  r-languages to s
-00010a50: 6565 2061 6c6c 2077 6869 7370 6572 2073  ee all whisper s
-00010a60: 7570 706f 7274 6564 206c 616e 6775 6167  upported languag
-00010a70: 6573 2e22 290d 0a20 2020 2020 2020 2072  es.")..        r
-00010a80: 6574 7572 6e20 310d 0a0d 0a20 2020 2069  eturn 1....    i
-00010a90: 6620 6172 6773 2e64 7374 5f6c 616e 6775  f args.dst_langu
-00010aa0: 6167 653a 0d0a 2020 2020 2020 2020 6966  age:..        if
-00010ab0: 206e 6f74 2061 7267 732e 6473 745f 6c61   not args.dst_la
-00010ac0: 6e67 7561 6765 2069 6e20 676f 6f67 6c65  nguage in google
-00010ad0: 5f6c 616e 6775 6167 652e 6e61 6d65 5f6f  _language.name_o
-00010ae0: 665f 636f 6465 2e6b 6579 7328 293a 0d0a  f_code.keys():..
-00010af0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00010b00: 7428 2244 6573 7469 6e61 7469 6f6e 206c  t("Destination l
-00010b10: 616e 6775 6167 6520 6973 206e 6f74 2073  anguage is not s
-00010b20: 7570 706f 7274 6564 2e20 5275 6e20 7769  upported. Run wi
-00010b30: 7468 202d 2d6c 6973 742d 676f 6f67 6c65  th --list-google
-00010b40: 2d6c 616e 6775 6167 6573 2074 6f20 7365  -languages to se
-00010b50: 6520 616c 6c20 676f 6f67 6c65 2074 7261  e all google tra
-00010b60: 6e73 6c61 7465 2073 7570 706f 7274 6564  nslate supported
-00010b70: 206c 616e 6775 6167 6573 2e22 290d 0a20   languages.").. 
-00010b80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00010b90: 6e20 310d 0a20 2020 2020 2020 2069 6620  n 1..        if 
-00010ba0: 6e6f 7420 6973 5f73 616d 655f 6c61 6e67  not is_same_lang
-00010bb0: 7561 6765 2861 7267 732e 7372 635f 6c61  uage(args.src_la
-00010bc0: 6e67 7561 6765 2c20 6172 6773 2e64 7374  nguage, args.dst
-00010bd0: 5f6c 616e 6775 6167 652c 2065 7272 6f72  _language, error
-00010be0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-00010bf0: 636b 3d73 686f 775f 6572 726f 725f 6d65  ck=show_error_me
-00010c00: 7373 6167 6573 293a 0d0a 2020 2020 2020  ssages):..      
-00010c10: 2020 2020 2020 646f 5f74 7261 6e73 6c61        do_transla
-00010c20: 7465 203d 2054 7275 650d 0a20 2020 2020  te = True..     
-00010c30: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00010c40: 2020 2020 2020 646f 5f74 7261 6e73 6c61        do_transla
-00010c50: 7465 203d 2046 616c 7365 0d0a 2020 2020  te = False..    
-00010c60: 656c 7365 3a0d 0a20 2020 2020 2020 2064  else:..        d
-00010c70: 6f5f 7472 616e 736c 6174 6520 3d20 4661  o_translate = Fa
-00010c80: 6c73 650d 0a0d 0a20 2020 2069 6620 6172  lse....    if ar
-00010c90: 6773 2e6c 6973 745f 666f 726d 6174 733a  gs.list_formats:
-00010ca0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00010cb0: 224c 6973 7420 6f66 2073 7570 706f 7274  "List of support
-00010cc0: 6564 2073 7562 7469 746c 6520 666f 726d  ed subtitle form
-00010cd0: 6174 733a 2229 0d0a 2020 2020 2020 2020  ats:")..        
-00010ce0: 666f 7220 7375 6274 6974 6c65 5f66 6f72  for subtitle_for
-00010cf0: 6d61 7420 696e 2053 7562 7469 746c 6546  mat in SubtitleF
-00010d00: 6f72 6d61 7474 6572 2e73 7570 706f 7274  ormatter.support
-00010d10: 6564 5f66 6f72 6d61 7473 3a0d 0a20 2020  ed_formats:..   
-00010d20: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-00010d30: 7b66 6f72 6d61 747d 222e 666f 726d 6174  {format}".format
-00010d40: 2866 6f72 6d61 743d 7375 6274 6974 6c65  (format=subtitle
-00010d50: 5f66 6f72 6d61 7429 290d 0a20 2020 2020  _format))..     
-00010d60: 2020 2072 6574 7572 6e20 300d 0a0d 0a20     return 0.... 
-00010d70: 2020 2069 6620 6172 6773 2e66 6f72 6d61     if args.forma
-00010d80: 7420 6e6f 7420 696e 2053 7562 7469 746c  t not in Subtitl
-00010d90: 6546 6f72 6d61 7474 6572 2e73 7570 706f  eFormatter.suppo
-00010da0: 7274 6564 5f66 6f72 6d61 7473 3a0d 0a20  rted_formats:.. 
-00010db0: 2020 2020 2020 2070 7269 6e74 2822 5375         print("Su
-00010dc0: 6274 6974 6c65 2066 6f72 6d61 7420 6973  btitle format is
-00010dd0: 206e 6f74 2073 7570 706f 7274 6564 2e20   not supported. 
-00010de0: 5275 6e20 7769 7468 202d 2d6c 6973 742d  Run with --list-
-00010df0: 666f 726d 6174 7320 746f 2073 6565 2061  formats to see a
-00010e00: 6c6c 2073 7570 706f 7274 6564 2066 6f72  ll supported for
-00010e10: 6d61 7473 2e22 290d 0a20 2020 2020 2020  mats.")..       
-00010e20: 2072 6574 7572 6e20 310d 0a0d 0a20 2020   return 1....   
-00010e30: 2069 6620 6e6f 7420 6172 6773 2e73 6f75   if not args.sou
-00010e40: 7263 655f 7061 7468 3a0d 0a20 2020 2020  rce_path:..     
-00010e50: 2020 2070 6172 7365 722e 7072 696e 745f     parser.print_
-00010e60: 6865 6c70 2873 7973 2e73 7464 6572 7229  help(sys.stderr)
-00010e70: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00010e80: 2031 0d0a 0d0a 2020 2020 636f 6d70 6c65   1....    comple
-00010e90: 7465 645f 7461 736b 7320 3d20 300d 0a20  ted_tasks = 0.. 
-00010ea0: 2020 206d 6564 6961 5f66 696c 6570 6174     media_filepat
-00010eb0: 6873 203d 205b 5d0d 0a20 2020 2061 7267  hs = []..    arg
-00010ec0: 5f66 696c 6570 6174 6873 203d 205b 5d0d  _filepaths = [].
-00010ed0: 0a20 2020 2069 6e76 616c 6964 5f6d 6564  .    invalid_med
-00010ee0: 6961 5f66 696c 6570 6174 6873 203d 205b  ia_filepaths = [
-00010ef0: 5d0d 0a20 2020 206e 6f74 5f65 7869 7374  ]..    not_exist
-00010f00: 5f66 696c 6570 6174 6873 203d 205b 5d0d  _filepaths = [].
-00010f10: 0a20 2020 2061 7267 7061 7468 203d 204e  .    argpath = N
-00010f20: 6f6e 650d 0a0d 0a20 2020 2061 7267 735f  one....    args_
-00010f30: 736f 7572 6365 5f70 6174 6820 3d20 6172  source_path = ar
-00010f40: 6773 2e73 6f75 7263 655f 7061 7468 0d0a  gs.source_path..
-00010f50: 0d0a 2020 2020 6966 2028 6e6f 7420 2822  ..    if (not ("
-00010f60: 2a22 2061 6e64 2022 3f22 2920 696e 2073  *" and "?") in s
-00010f70: 7472 2861 7267 735f 736f 7572 6365 5f70  tr(args_source_p
-00010f80: 6174 6829 293a 0d0a 2020 2020 2020 2020  ath)):..        
-00010f90: 666f 7220 6669 6c65 7061 7468 2069 6e20  for filepath in 
-00010fa0: 6172 6773 5f73 6f75 7263 655f 7061 7468  args_source_path
-00010fb0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-00010fc0: 7061 7468 203d 2050 6174 6828 6669 6c65  path = Path(file
-00010fd0: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
-00010fe0: 2020 2023 7072 696e 7428 2266 7061 7468     #print("fpath
-00010ff0: 203d 2025 7322 2025 6670 6174 6829 0d0a   = %s" %fpath)..
-00011000: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00011010: 6f74 206f 732e 7061 7468 2e69 7366 696c  ot os.path.isfil
-00011020: 6528 6670 6174 6829 3a0d 0a20 2020 2020  e(fpath):..     
-00011030: 2020 2020 2020 2020 2020 206e 6f74 5f65             not_e
-00011040: 7869 7374 5f66 696c 6570 6174 6873 2e61  xist_filepaths.a
-00011050: 7070 656e 6428 6669 6c65 7061 7468 290d  ppend(filepath).
-00011060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011070: 2023 7072 696e 7428 7374 7228 6670 6174   #print(str(fpat
-00011080: 6829 202b 2022 2069 7320 6e6f 7420 6578  h) + " is not ex
-00011090: 6973 7422 290d 0a0d 0a20 2020 2069 6620  ist")....    if 
-000110a0: 7379 732e 706c 6174 666f 726d 203d 3d20  sys.platform == 
-000110b0: 2277 696e 3332 223a 0d0a 2020 2020 2020  "win32":..      
-000110c0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-000110d0: 286c 656e 2861 7267 732e 736f 7572 6365  (len(args.source
-000110e0: 5f70 6174 6829 293a 0d0a 2020 2020 2020  _path)):..      
-000110f0: 2020 2020 2020 6966 2028 225b 2220 6f72        if ("[" or
-00011100: 2022 5d22 2920 696e 2061 7267 732e 736f   "]") in args.so
-00011110: 7572 6365 5f70 6174 685b 695d 3a0d 0a20  urce_path[i]:.. 
-00011120: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00011130: 6c61 6365 686f 6c64 6572 203d 2022 2354  laceholder = "#T
-00011140: 454d 5023 220d 0a20 2020 2020 2020 2020  EMP#"..         
-00011150: 2020 2020 2020 2061 7267 735f 736f 7572         args_sour
-00011160: 6365 5f70 6174 685b 695d 203d 2061 7267  ce_path[i] = arg
-00011170: 732e 736f 7572 6365 5f70 6174 685b 695d  s.source_path[i]
-00011180: 2e72 6570 6c61 6365 2822 5b22 2c20 706c  .replace("[", pl
-00011190: 6163 6568 6f6c 6465 7229 0d0a 2020 2020  aceholder)..    
-000111a0: 2020 2020 2020 2020 2020 2020 6172 6773              args
-000111b0: 5f73 6f75 7263 655f 7061 7468 5b69 5d20  _source_path[i] 
-000111c0: 3d20 6172 6773 5f73 6f75 7263 655f 7061  = args_source_pa
-000111d0: 7468 5b69 5d2e 7265 706c 6163 6528 225d  th[i].replace("]
-000111e0: 222c 2022 5b5d 5d22 290d 0a20 2020 2020  ", "[]]")..     
-000111f0: 2020 2020 2020 2020 2020 2061 7267 735f             args_
-00011200: 736f 7572 6365 5f70 6174 685b 695d 203d  source_path[i] =
-00011210: 2061 7267 735f 736f 7572 6365 5f70 6174   args_source_pat
-00011220: 685b 695d 2e72 6570 6c61 6365 2870 6c61  h[i].replace(pla
-00011230: 6365 686f 6c64 6572 2c20 225b 5b5d 2229  ceholder, "[[]")
-00011240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011250: 2020 2370 7269 6e74 2822 6172 6773 5f73    #print("args_s
-00011260: 6f75 7263 655f 7061 7468 203d 2025 7322  ource_path = %s"
-00011270: 2025 2861 7267 735f 736f 7572 6365 5f70   %(args_source_p
-00011280: 6174 6829 290d 0a0d 0a20 2020 2066 6f72  ath))....    for
-00011290: 2061 7267 2069 6e20 6172 6773 5f73 6f75   arg in args_sou
-000112a0: 7263 655f 7061 7468 3a0d 0a20 2020 2020  rce_path:..     
-000112b0: 2020 2069 6620 6e6f 7420 7379 732e 706c     if not sys.pl
-000112c0: 6174 666f 726d 203d 3d20 2277 696e 3332  atform == "win32
-000112d0: 2220 3a0d 0a20 2020 2020 2020 2020 2020  " :..           
-000112e0: 2061 7267 203d 2065 7363 6170 6528 6172   arg = escape(ar
-000112f0: 6729 0d0a 0d0a 2020 2020 2020 2020 2370  g)....        #p
-00011300: 7269 6e74 2822 676c 6f62 2861 7267 2920  rint("glob(arg) 
-00011310: 3d20 2573 2220 2528 676c 6f62 2861 7267  = %s" %(glob(arg
-00011320: 2929 290d 0a0d 0a20 2020 2020 2020 2061  )))....        a
-00011330: 7267 5f66 696c 6570 6174 6873 202b 3d20  rg_filepaths += 
-00011340: 676c 6f62 2861 7267 290d 0a0d 0a20 2020  glob(arg)....   
-00011350: 2069 6620 6172 675f 6669 6c65 7061 7468   if arg_filepath
-00011360: 733a 0d0a 2020 2020 2020 2020 666f 7220  s:..        for 
-00011370: 6172 6770 6174 6820 696e 2061 7267 5f66  argpath in arg_f
-00011380: 696c 6570 6174 6873 3a0d 0a20 2020 2020  ilepaths:..     
-00011390: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
-000113a0: 682e 6973 6669 6c65 2861 7267 7061 7468  h.isfile(argpath
-000113b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000113c0: 2020 2020 6966 2063 6865 636b 5f66 696c      if check_fil
-000113d0: 655f 7479 7065 2861 7267 7061 7468 2c20  e_type(argpath, 
-000113e0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-000113f0: 616c 6c62 6163 6b3d 7368 6f77 5f65 7272  allback=show_err
-00011400: 6f72 5f6d 6573 7361 6765 7329 203d 3d20  or_messages) == 
-00011410: 2776 6964 656f 2720 6f72 2063 6865 636b  'video' or check
-00011420: 5f66 696c 655f 7479 7065 2861 7267 7061  _file_type(argpa
-00011430: 7468 2c20 6572 726f 725f 6d65 7373 6167  th, error_messag
-00011440: 6573 5f63 616c 6c62 6163 6b3d 7368 6f77  es_callback=show
-00011450: 5f65 7272 6f72 5f6d 6573 7361 6765 7329  _error_messages)
-00011460: 203d 3d20 2761 7564 696f 273a 0d0a 2020   == 'audio':..  
-00011470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011480: 2020 6d65 6469 615f 6669 6c65 7061 7468    media_filepath
-00011490: 732e 6170 7065 6e64 2861 7267 7061 7468  s.append(argpath
-000114a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000114b0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000114c0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-000114d0: 7661 6c69 645f 6d65 6469 615f 6669 6c65  valid_media_file
-000114e0: 7061 7468 732e 6170 7065 6e64 2861 7267  paths.append(arg
-000114f0: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
-00011500: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00011510: 2020 2020 2020 2020 2020 6e6f 745f 6578            not_ex
-00011520: 6973 745f 6669 6c65 7061 7468 732e 6170  ist_filepaths.ap
-00011530: 7065 6e64 2861 7267 7061 7468 290d 0a0d  pend(argpath)...
-00011540: 0a20 2020 2020 2020 2069 6620 696e 7661  .        if inva
-00011550: 6c69 645f 6d65 6469 615f 6669 6c65 7061  lid_media_filepa
-00011560: 7468 733a 0d0a 2020 2020 2020 2020 2020  ths:..          
-00011570: 2020 666f 7220 696e 7661 6c69 645f 6d65    for invalid_me
-00011580: 6469 615f 6669 6c65 7061 7468 2069 6e20  dia_filepath in 
-00011590: 696e 7661 6c69 645f 6d65 6469 615f 6669  invalid_media_fi
-000115a0: 6c65 7061 7468 733a 0d0a 2020 2020 2020  lepaths:..      
-000115b0: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
-000115c0: 227b 7d20 6973 206e 6f74 2076 616c 6964  "{} is not valid
-000115d0: 2076 6964 656f 206f 7220 6175 6469 6f20   video or audio 
-000115e0: 6669 6c65 7322 2e66 6f72 6d61 7428 696e  files".format(in
-000115f0: 7661 6c69 645f 6d65 6469 615f 6669 6c65  valid_media_file
-00011600: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
-00011610: 2020 2020 2020 2070 7269 6e74 286d 7367         print(msg
-00011620: 290d 0a0d 0a20 2020 2023 7072 696e 7428  )....    #print(
-00011630: 226e 6f74 5f65 7869 7374 5f66 696c 6570  "not_exist_filep
-00011640: 6174 6873 203d 2025 7322 2025 286e 6f74  aths = %s" %(not
-00011650: 5f65 7869 7374 5f66 696c 6570 6174 6873  _exist_filepaths
-00011660: 2929 0d0a 0d0a 2020 2020 6966 206e 6f74  ))....    if not
-00011670: 5f65 7869 7374 5f66 696c 6570 6174 6873  _exist_filepaths
-00011680: 3a0d 0a20 2020 2020 2020 2066 6f72 206e  :..        for n
-00011690: 6f74 5f65 7869 7374 5f66 696c 6570 6174  ot_exist_filepat
-000116a0: 6820 696e 206e 6f74 5f65 7869 7374 5f66  h in not_exist_f
-000116b0: 696c 6570 6174 6873 3a0d 0a20 2020 2020  ilepaths:..     
-000116c0: 2020 2020 2020 206d 7367 203d 2022 7b7d         msg = "{}
-000116d0: 2069 7320 6e6f 7420 6578 6973 7422 2e66   is not exist".f
-000116e0: 6f72 6d61 7428 6e6f 745f 6578 6973 745f  ormat(not_exist_
-000116f0: 6669 6c65 7061 7468 290d 0a20 2020 2020  filepath)..     
-00011700: 2020 2020 2020 2070 7269 6e74 286d 7367         print(msg
-00011710: 290d 0a20 2020 2020 2020 2069 6620 286e  )..        if (n
-00011720: 6f74 2028 222a 2220 616e 6420 223f 2229  ot ("*" and "?")
-00011730: 2069 6e20 7374 7228 6172 6773 5f73 6f75   in str(args_sou
-00011740: 7263 655f 7061 7468 2929 3a0d 0a20 2020  rce_path)):..   
-00011750: 2020 2020 2020 2020 2073 7973 2e65 7869           sys.exi
-00011760: 7428 3029 0d0a 0d0a 2020 2020 6966 206e  t(0)....    if n
-00011770: 6f74 2061 7267 5f66 696c 6570 6174 6873  ot arg_filepaths
-00011780: 2061 6e64 206e 6f74 206e 6f74 5f65 7869   and not not_exi
-00011790: 7374 5f66 696c 6570 6174 6873 3a0d 0a20  st_filepaths:.. 
-000117a0: 2020 2020 2020 2070 7269 6e74 2822 4e6f         print("No
-000117b0: 2061 6e79 2066 696c 6573 206d 6174 6368   any files match
-000117c0: 696e 6720 6669 6c65 6e61 6d65 7320 796f  ing filenames yo
-000117d0: 7520 7479 7065 6422 290d 0a20 2020 2020  u typed")..     
-000117e0: 2020 2073 7973 2e65 7869 7428 3029 0d0a     sys.exit(0)..
-000117f0: 0d0a 2020 2020 706f 6f6c 203d 206d 756c  ..    pool = mul
-00011800: 7469 7072 6f63 6573 7369 6e67 2e50 6f6f  tiprocessing.Poo
-00011810: 6c28 6172 6773 2e63 6f6e 6375 7272 656e  l(args.concurren
-00011820: 6379 290d 0a0d 0a20 2020 2074 7261 6e73  cy)....    trans
-00011830: 6372 6962 655f 656e 645f 7469 6d65 203d  cribe_end_time =
-00011840: 204e 6f6e 650d 0a20 2020 2074 7261 6e73   None..    trans
-00011850: 6372 6962 655f 656c 6170 7365 645f 7469  cribe_elapsed_ti
-00011860: 6d65 203d 204e 6f6e 650d 0a20 2020 2074  me = None..    t
-00011870: 7261 6e73 6372 6962 655f 7374 6172 745f  ranscribe_start_
-00011880: 7469 6d65 203d 2074 696d 652e 7469 6d65  time = time.time
-00011890: 2829 0d0a 2020 2020 7461 736b 203d 2022  ()..    task = "
-000118a0: 7472 616e 7363 7269 6265 220d 0a0d 0a20  transcribe".... 
-000118b0: 2020 2069 6620 6172 6773 2e73 7263 5f6c     if args.src_l
-000118c0: 616e 6775 6167 6520 3d3d 2028 2262 6122  anguage == ("ba"
-000118d0: 206f 7220 2262 7222 206f 7220 2266 6f22   or "br" or "fo"
-000118e0: 206f 7220 226e 6e22 206f 7220 226f 6322   or "nn" or "oc"
-000118f0: 206f 7220 2274 6c22 206f 7220 2262 6f22   or "tl" or "bo"
-00011900: 2920 616e 6420 646f 5f74 7261 6e73 6c61  ) and do_transla
-00011910: 7465 3a0d 0a20 2020 2020 2020 2074 6173  te:..        tas
-00011920: 6b20 3d20 2274 7261 6e73 6c61 7465 220d  k = "translate".
-00011930: 0a20 2020 2020 2020 2073 7263 5f6c 616e  .        src_lan
-00011940: 6775 6167 6520 3d20 2265 6e22 0d0a 0d0a  guage = "en"....
-00011950: 2020 2020 666f 7220 6d65 6469 615f 6669      for media_fi
-00011960: 6c65 7061 7468 2069 6e20 6d65 6469 615f  lepath in media_
-00011970: 6669 6c65 7061 7468 733a 0d0a 2020 2020  filepaths:..    
-00011980: 2020 2020 7072 696e 7428 2250 726f 6365      print("Proce
-00011990: 7373 696e 6720 7b7d 203a 222e 666f 726d  ssing {} :".form
-000119a0: 6174 286d 6564 6961 5f66 696c 6570 6174  at(media_filepat
-000119b0: 6829 290d 0a0d 0a20 2020 2020 2020 2074  h))....        t
-000119c0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-000119d0: 2070 7269 6e74 2822 436f 6e76 6572 7469   print("Converti
-000119e0: 6e67 2074 6f20 6120 7465 6d70 6f72 6172  ng to a temporar
-000119f0: 7920 5741 5620 6669 6c65 2020 2020 2020  y WAV file      
-00011a00: 3a20 2229 0d0a 2020 2020 2020 2020 2020  : ")..          
-00011a10: 2020 7769 6467 6574 7320 3d20 5b22 222c    widgets = ["",
-00011a20: 2050 6572 6365 6e74 6167 6528 292c 2027   Percentage(), '
-00011a30: 2027 2c20 4261 7228 6d61 726b 6572 3d27   ', Bar(marker='
-00011a40: e296 8827 292c 2027 2027 2c20 4554 4128  ...'), ' ', ETA(
-00011a50: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
-00011a60: 7062 6172 203d 2050 726f 6772 6573 7342  pbar = ProgressB
-00011a70: 6172 2877 6964 6765 7473 3d77 6964 6765  ar(widgets=widge
-00011a80: 7473 2c20 6d61 7876 616c 3d31 3030 292e  ts, maxval=100).
-00011a90: 7374 6172 7428 290d 0a20 2020 2020 2020  start()..       
-00011aa0: 2020 2020 2077 6176 5f63 6f6e 7665 7274       wav_convert
-00011ab0: 6572 203d 2057 6176 436f 6e76 6572 7465  er = WavConverte
-00011ac0: 7228 7072 6f67 7265 7373 5f63 616c 6c62  r(progress_callb
-00011ad0: 6163 6b3d 7368 6f77 5f70 726f 6772 6573  ack=show_progres
-00011ae0: 732c 2065 7272 6f72 5f6d 6573 7361 6765  s, error_message
-00011af0: 735f 6361 6c6c 6261 636b 3d73 686f 775f  s_callback=show_
-00011b00: 6572 726f 725f 6d65 7373 6167 6573 290d  error_messages).
-00011b10: 0a20 2020 2020 2020 2020 2020 2077 6176  .            wav
-00011b20: 5f66 696c 6570 6174 682c 2073 616d 706c  _filepath, sampl
-00011b30: 655f 7261 7465 203d 2077 6176 5f63 6f6e  e_rate = wav_con
-00011b40: 7665 7274 6572 286d 6564 6961 5f66 696c  verter(media_fil
-00011b50: 6570 6174 6829 0d0a 2020 2020 2020 2020  epath)..        
-00011b60: 2020 2020 7062 6172 2e66 696e 6973 6828      pbar.finish(
-00011b70: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00011b80: 2070 7269 6e74 2822 5065 7266 6f72 6d69   print("Performi
-00011b90: 6e67 2073 7065 6563 6820 7265 636f 676e  ng speech recogn
-00011ba0: 6974 696f 6e20 2020 2020 2020 2020 2020  ition           
-00011bb0: 3a20 2229 0d0a 2020 2020 2020 2020 2020  : ")..          
-00011bc0: 2020 7768 6973 7065 725f 7265 636f 676e    whisper_recogn
-00011bd0: 697a 6572 203d 2057 6869 7370 6572 5265  izer = WhisperRe
-00011be0: 636f 676e 697a 6572 286c 616e 6775 6167  cognizer(languag
-00011bf0: 653d 6172 6773 2e73 7263 5f6c 616e 6775  e=args.src_langu
-00011c00: 6167 652c 206d 6f64 656c 3d6d 6f64 656c  age, model=model
-00011c10: 2c20 6670 3136 3d46 616c 7365 2c20 7461  , fp16=False, ta
-00011c20: 736b 3d74 6173 6b2c 2076 6572 626f 7365  sk=task, verbose
-00011c30: 3d46 616c 7365 2c20 6572 726f 725f 6d65  =False, error_me
-00011c40: 7373 6167 6573 5f63 616c 6c62 6163 6b3d  ssages_callback=
-00011c50: 7368 6f77 5f65 7272 6f72 5f6d 6573 7361  show_error_messa
-00011c60: 6765 7329 0d0a 2020 2020 2020 2020 2020  ges)..          
-00011c70: 2020 7265 7375 6c74 203d 2077 6869 7370    result = whisp
-00011c80: 6572 5f72 6563 6f67 6e69 7a65 7228 7761  er_recognizer(wa
-00011c90: 765f 6669 6c65 7061 7468 290d 0a0d 0a20  v_filepath).... 
-00011ca0: 2020 2020 2020 2020 2020 2074 696d 6564             timed
-00011cb0: 5f73 7562 7469 746c 6573 203d 205b 5d0d  _subtitles = [].
-00011cc0: 0a20 2020 2020 2020 2020 2020 2072 6567  .            reg
-00011cd0: 696f 6e73 203d 205b 5d0d 0a20 2020 2020  ions = []..     
-00011ce0: 2020 2020 2020 2074 7261 6e73 6372 6970         transcrip
-00011cf0: 7473 203d 205b 5d0d 0a20 2020 2020 2020  ts = []..       
-00011d00: 2020 2020 2066 6f72 2073 6567 6d65 6e74       for segment
-00011d10: 2069 6e20 7265 7375 6c74 5b27 7365 676d   in result['segm
-00011d20: 656e 7473 275d 3a0d 0a20 2020 2020 2020  ents']:..       
-00011d30: 2020 2020 2020 2020 2073 7461 7274 203d           start =
-00011d40: 2073 6567 6d65 6e74 5b27 7374 6172 7427   segment['start'
-00011d50: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00011d60: 2020 2065 6e64 203d 2073 6567 6d65 6e74     end = segment
-00011d70: 5b27 656e 6427 5d0d 0a20 2020 2020 2020  ['end']..       
-00011d80: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
-00011d90: 7365 676d 656e 745b 2774 6578 7427 5d0d  segment['text'].
-00011da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011db0: 2072 6567 696f 6e73 2e61 7070 656e 6428   regions.append(
-00011dc0: 2873 7461 7274 2c20 656e 6429 290d 0a20  (start, end)).. 
-00011dd0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00011de0: 7261 6e73 6372 6970 7473 2e61 7070 656e  ranscripts.appen
-00011df0: 6428 7465 7874 290d 0a20 2020 2020 2020  d(text)..       
-00011e00: 2020 2020 2074 696d 6564 5f73 7562 7469       timed_subti
-00011e10: 746c 6573 203d 205b 2872 2c20 7429 2066  tles = [(r, t) f
-00011e20: 6f72 2072 2c20 7420 696e 207a 6970 2872  or r, t in zip(r
-00011e30: 6567 696f 6e73 2c20 7472 616e 7363 7269  egions, transcri
-00011e40: 7074 7329 2069 6620 745d 0d0a 0d0a 2020  pts) if t]....  
-00011e50: 2020 2020 2020 2020 2020 7375 6274 6974            subtit
-00011e60: 6c65 5f66 6f72 6d61 7420 3d20 6172 6773  le_format = args
-00011e70: 2e66 6f72 6d61 740d 0a20 2020 2020 2020  .format..       
-00011e80: 2020 2020 2062 6173 652c 2065 7874 203d       base, ext =
-00011e90: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
-00011ea0: 7428 6d65 6469 615f 6669 6c65 7061 7468  t(media_filepath
-00011eb0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00011ec0: 7562 7469 746c 655f 6669 6c65 7061 7468  ubtitle_filepath
-00011ed0: 203d 2022 7b62 6173 657d 2e7b 666f 726d   = "{base}.{form
-00011ee0: 6174 7d22 2e66 6f72 6d61 7428 6261 7365  at}".format(base
-00011ef0: 3d62 6173 652c 2066 6f72 6d61 743d 7375  =base, format=su
-00011f00: 6274 6974 6c65 5f66 6f72 6d61 7429 0d0a  btitle_format)..
-00011f10: 0d0a 2020 2020 2020 2020 2020 2020 7772  ..            wr
-00011f20: 6974 6572 203d 2053 7562 7469 746c 6557  iter = SubtitleW
-00011f30: 7269 7465 7228 7265 6769 6f6e 732c 2074  riter(regions, t
-00011f40: 7261 6e73 6372 6970 7473 2c20 7375 6274  ranscripts, subt
-00011f50: 6974 6c65 5f66 6f72 6d61 742c 2065 7272  itle_format, err
-00011f60: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-00011f70: 6261 636b 3d73 686f 775f 6572 726f 725f  back=show_error_
-00011f80: 6d65 7373 6167 6573 290d 0a20 2020 2020  messages)..     
-00011f90: 2020 2020 2020 2077 7269 7465 722e 7772         writer.wr
-00011fa0: 6974 6528 7375 6274 6974 6c65 5f66 696c  ite(subtitle_fil
-00011fb0: 6570 6174 6829 0d0a 0d0a 2020 2020 2020  epath)....      
-00011fc0: 2020 2020 2020 6966 2064 6f5f 7472 616e        if do_tran
-00011fd0: 736c 6174 653a 0d0a 2020 2020 2020 2020  slate:..        
-00011fe0: 2020 2020 2020 2020 2320 434f 4e43 5552          # CONCUR
-00011ff0: 5245 4e54 2054 5241 4e53 4c41 5449 4f4e  RENT TRANSLATION
-00012000: 2055 5349 4e47 2063 6c61 7373 2053 656e   USING class Sen
-00012010: 7465 6e63 6554 7261 6e73 6c61 746f 7228  tenceTranslator(
-00012020: 6f62 6a65 6374 290d 0a20 2020 2020 2020  object)..       
-00012030: 2020 2020 2020 2020 2023 204e 4f20 4e45           # NO NE
-00012040: 4544 2054 4f20 5452 414e 534c 4154 4520  ED TO TRANSLATE 
-00012050: 414c 4c20 7472 616e 7363 7269 7074 2049  ALL transcript I
-00012060: 4e20 7472 616e 7363 7269 7074 730d 0a20  N transcripts.. 
-00012070: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00012080: 2042 4543 4155 5345 2053 4f4d 4520 7265   BECAUSE SOME re
-00012090: 6769 6f6e 2049 4e20 7265 6769 6f6e 7320  gion IN regions 
-000120a0: 4d41 5920 4a55 5354 2048 4156 4520 7472  MAY JUST HAVE tr
-000120b0: 616e 7363 7269 7074 2057 4954 4820 454d  anscript WITH EM
-000120c0: 5054 5920 5354 5249 4e47 0d0a 2020 2020  PTY STRING..    
-000120d0: 2020 2020 2020 2020 2020 2020 2320 4a55              # JU
-000120e0: 5354 2054 5241 4e53 4c41 5445 2041 4c52  ST TRANSLATE ALR
-000120f0: 4541 4459 2043 5245 4154 4544 2073 7562  EADY CREATED sub
-00012100: 7469 746c 6573 2045 4e54 5249 4553 2046  titles ENTRIES F
-00012110: 524f 4d20 7469 6d65 645f 7375 6274 6974  ROM timed_subtit
-00012120: 6c65 730d 0a20 2020 2020 2020 2020 2020  les..           
-00012130: 2020 2020 2074 696d 6564 5f73 7562 7469       timed_subti
-00012140: 746c 6573 203d 2077 7269 7465 722e 7469  tles = writer.ti
-00012150: 6d65 645f 7375 6274 6974 6c65 730d 0a20  med_subtitles.. 
-00012160: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012170: 7265 6174 6564 5f72 6567 696f 6e73 203d  reated_regions =
-00012180: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012190: 2020 2020 2063 7265 6174 6564 5f73 7562       created_sub
-000121a0: 7469 746c 6573 203d 205b 5d0d 0a20 2020  titles = []..   
-000121b0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000121c0: 2065 6e74 7279 2069 6e20 7469 6d65 645f   entry in timed_
-000121d0: 7375 6274 6974 6c65 733a 0d0a 2020 2020  subtitles:..    
-000121e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121f0: 6372 6561 7465 645f 7265 6769 6f6e 732e  created_regions.
-00012200: 6170 7065 6e64 2865 6e74 7279 5b30 5d29  append(entry[0])
-00012210: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012220: 2020 2020 2020 6372 6561 7465 645f 7375        created_su
-00012230: 6274 6974 6c65 732e 6170 7065 6e64 2865  btitles.append(e
-00012240: 6e74 7279 5b31 5d29 0d0a 0d0a 2020 2020  ntry[1])....    
-00012250: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00012260: 7428 2254 7261 6e73 6c61 7469 6e67 2066  t("Translating f
-00012270: 726f 6d20 2573 2074 6f20 2573 2020 203a  rom %s to %s   :
-00012280: 2022 2025 2873 7263 5f6c 616e 6775 6167   " %(src_languag
-00012290: 652e 6365 6e74 6572 2838 292c 2064 7374  e.center(8), dst
-000122a0: 5f6c 616e 6775 6167 652e 6365 6e74 6572  _language.center
-000122b0: 2838 2929 290d 0a20 2020 2020 2020 2020  (8)))..         
-000122c0: 2020 2020 2020 2077 6964 6765 7473 203d         widgets =
-000122d0: 205b 2222 2c20 5065 7263 656e 7461 6765   ["", Percentage
-000122e0: 2829 2c20 2720 272c 2042 6172 286d 6172  (), ' ', Bar(mar
-000122f0: 6b65 723d 27e2 9688 2729 2c20 2720 272c  ker='...'), ' ',
-00012300: 2045 5441 2829 5d0d 0a20 2020 2020 2020   ETA()]..       
-00012310: 2020 2020 2020 2020 2070 6261 7220 3d20           pbar = 
-00012320: 5072 6f67 7265 7373 4261 7228 7769 6467  ProgressBar(widg
-00012330: 6574 733d 7769 6467 6574 732c 206d 6178  ets=widgets, max
-00012340: 7661 6c3d 6c65 6e28 7469 6d65 645f 7375  val=len(timed_su
-00012350: 6274 6974 6c65 7329 292e 7374 6172 7428  btitles)).start(
-00012360: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00012370: 2020 2020 2074 7261 6e73 6372 6970 745f       transcript_
-00012380: 7472 616e 736c 6174 6f72 203d 2053 656e  translator = Sen
-00012390: 7465 6e63 6554 7261 6e73 6c61 746f 7228  tenceTranslator(
-000123a0: 7372 633d 6172 6773 2e73 7263 5f6c 616e  src=args.src_lan
-000123b0: 6775 6167 652c 2064 7374 3d61 7267 732e  guage, dst=args.
-000123c0: 6473 745f 6c61 6e67 7561 6765 2c20 6572  dst_language, er
-000123d0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-000123e0: 6c62 6163 6b3d 7368 6f77 5f65 7272 6f72  lback=show_error
-000123f0: 5f6d 6573 7361 6765 7329 0d0a 0d0a 2020  _messages)....  
-00012400: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00012410: 616e 736c 6174 6564 5f73 7562 7469 746c  anslated_subtitl
-00012420: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
-00012430: 2020 2020 2020 2020 2066 6f72 2069 2c20           for i, 
-00012440: 7472 616e 736c 6174 6564 5f73 7562 7469  translated_subti
-00012450: 746c 6520 696e 2065 6e75 6d65 7261 7465  tle in enumerate
-00012460: 2870 6f6f 6c2e 696d 6170 2874 7261 6e73  (pool.imap(trans
-00012470: 6372 6970 745f 7472 616e 736c 6174 6f72  cript_translator
-00012480: 2c20 6372 6561 7465 645f 7375 6274 6974  , created_subtit
-00012490: 6c65 7329 293a 0d0a 2020 2020 2020 2020  les)):..        
-000124a0: 2020 2020 2020 2020 2020 2020 7472 616e              tran
-000124b0: 736c 6174 6564 5f73 7562 7469 746c 6573  slated_subtitles
-000124c0: 2e61 7070 656e 6428 7472 616e 736c 6174  .append(translat
-000124d0: 6564 5f73 7562 7469 746c 6529 0d0a 2020  ed_subtitle)..  
-000124e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124f0: 2020 7062 6172 2e75 7064 6174 6528 6929    pbar.update(i)
-00012500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012510: 2020 7062 6172 2e66 696e 6973 6828 290d    pbar.finish().
-00012520: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00012530: 2020 2074 7261 6e73 6c61 7465 645f 7375     translated_su
-00012540: 6274 6974 6c65 5f66 696c 6570 6174 6820  btitle_filepath 
-00012550: 3d20 7375 6274 6974 6c65 5f66 696c 6570  = subtitle_filep
-00012560: 6174 685b 203a 2d34 5d20 2b20 272e 7472  ath[ :-4] + '.tr
-00012570: 616e 736c 6174 6564 2e27 202b 2073 7562  anslated.' + sub
-00012580: 7469 746c 655f 666f 726d 6174 0d0a 2020  title_format..  
-00012590: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000125a0: 616e 736c 6174 696f 6e5f 7772 6974 6572  anslation_writer
-000125b0: 203d 2053 7562 7469 746c 6557 7269 7465   = SubtitleWrite
-000125c0: 7228 6372 6561 7465 645f 7265 6769 6f6e  r(created_region
-000125d0: 732c 2074 7261 6e73 6c61 7465 645f 7375  s, translated_su
-000125e0: 6274 6974 6c65 732c 2073 7562 7469 746c  btitles, subtitl
-000125f0: 655f 666f 726d 6174 2c20 6572 726f 725f  e_format, error_
-00012600: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-00012610: 6b3d 7368 6f77 5f65 7272 6f72 5f6d 6573  k=show_error_mes
-00012620: 7361 6765 7329 0d0a 2020 2020 2020 2020  sages)..        
-00012630: 2020 2020 2020 2020 7472 616e 736c 6174          translat
-00012640: 696f 6e5f 7772 6974 6572 2e77 7269 7465  ion_writer.write
-00012650: 2874 7261 6e73 6c61 7465 645f 7375 6274  (translated_subt
-00012660: 6974 6c65 5f66 696c 6570 6174 6829 0d0a  itle_filepath)..
-00012670: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00012680: 696e 7428 2744 6f6e 652e 2729 0d0a 2020  int('Done.')..  
-00012690: 2020 2020 2020 2020 2020 6966 2064 6f5f            if do_
-000126a0: 7472 616e 736c 6174 653a 0d0a 2020 2020  translate:..    
-000126b0: 2020 2020 2020 2020 2020 2020 2370 7269              #pri
-000126c0: 6e74 2822 4f72 6967 696e 616c 2073 7562  nt("Original sub
-000126d0: 7469 746c 6573 2066 696c 6520 6372 6561  titles file crea
-000126e0: 7465 6420 6174 2020 2020 2020 3a20 7b7d  ted at      : {}
-000126f0: 222e 666f 726d 6174 2873 7562 7469 746c  ".format(subtitl
-00012700: 655f 6669 6c65 7061 7468 2929 0d0a 2020  e_filepath))..  
-00012710: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00012720: 2e72 656d 6f76 6528 7375 6274 6974 6c65  .remove(subtitle
-00012730: 5f66 696c 6570 6174 6829 0d0a 2020 2020  _filepath)..    
-00012740: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00012750: 7428 2754 7261 6e73 6c61 7465 6420 7375  t('Translated su
-00012760: 6274 6974 6c65 7320 6669 6c65 2063 7265  btitles file cre
-00012770: 6174 6564 2061 7420 2020 203a 207b 7d27  ated at    : {}'
-00012780: 202e 666f 726d 6174 2874 7261 6e73 6c61   .format(transla
-00012790: 7465 645f 7375 6274 6974 6c65 5f66 696c  ted_subtitle_fil
-000127a0: 6570 6174 6829 290d 0a20 2020 2020 2020  epath))..       
-000127b0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-000127c0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000127d0: 7428 2253 7562 7469 746c 6573 2066 696c  t("Subtitles fil
-000127e0: 6520 6372 6561 7465 6420 6174 2020 2020  e created at    
-000127f0: 2020 2020 2020 2020 2020 203a 207b 7d22             : {}"
-00012800: 2e66 6f72 6d61 7428 7375 6274 6974 6c65  .format(subtitle
-00012810: 5f66 696c 6570 6174 6829 290d 0a20 2020  _filepath))..   
-00012820: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00012830: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00012840: 636f 6d70 6c65 7465 645f 7461 736b 7320  completed_tasks 
-00012850: 2b3d 2031 0d0a 0d0a 2020 2020 2020 2020  += 1....        
-00012860: 2020 2020 6966 206c 656e 286d 6564 6961      if len(media
-00012870: 5f66 696c 6570 6174 6873 293e 3020 616e  _filepaths)>0 an
-00012880: 6420 636f 6d70 6c65 7465 645f 7461 736b  d completed_task
-00012890: 7320 3d3d 206c 656e 286d 6564 6961 5f66  s == len(media_f
-000128a0: 696c 6570 6174 6873 293a 0d0a 2020 2020  ilepaths):..    
-000128b0: 2020 2020 2020 2020 2020 2020 7472 616e              tran
-000128c0: 7363 7269 6265 5f65 6e64 5f74 696d 6520  scribe_end_time 
-000128d0: 3d20 7469 6d65 2e74 696d 6528 290d 0a20  = time.time().. 
-000128e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000128f0: 7261 6e73 6372 6962 655f 656c 6170 7365  ranscribe_elapse
-00012900: 645f 7469 6d65 203d 2074 7261 6e73 6372  d_time = transcr
-00012910: 6962 655f 656e 645f 7469 6d65 202d 2074  ibe_end_time - t
-00012920: 7261 6e73 6372 6962 655f 7374 6172 745f  ranscribe_start_
-00012930: 7469 6d65 0d0a 2020 2020 2020 2020 2020  time..          
-00012940: 2020 2020 2020 7472 616e 7363 7269 6265        transcribe
-00012950: 5f65 6c61 7073 6564 5f74 696d 655f 7365  _elapsed_time_se
-00012960: 636f 6e64 7320 3d20 7469 6d65 6465 6c74  conds = timedelt
-00012970: 6128 7365 636f 6e64 733d 696e 7428 7472  a(seconds=int(tr
-00012980: 616e 7363 7269 6265 5f65 6c61 7073 6564  anscribe_elapsed
-00012990: 5f74 696d 6529 290d 0a20 2020 2020 2020  _time))..       
-000129a0: 2020 2020 2020 2020 2074 7261 6e73 6372           transcr
-000129b0: 6962 655f 656c 6170 7365 645f 7469 6d65  ibe_elapsed_time
-000129c0: 5f73 7472 203d 2073 7472 2874 7261 6e73  _str = str(trans
-000129d0: 6372 6962 655f 656c 6170 7365 645f 7469  cribe_elapsed_ti
-000129e0: 6d65 5f73 6563 6f6e 6473 290d 0a20 2020  me_seconds)..   
-000129f0: 2020 2020 2020 2020 2020 2020 2068 6f75               hou
-00012a00: 722c 206d 696e 7574 652c 2073 6563 6f6e  r, minute, secon
-00012a10: 6420 3d20 7472 616e 7363 7269 6265 5f65  d = transcribe_e
-00012a20: 6c61 7073 6564 5f74 696d 655f 7374 722e  lapsed_time_str.
-00012a30: 7370 6c69 7428 223a 2229 0d0a 2020 2020  split(":")..    
-00012a40: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
-00012a50: 3d20 2254 6f74 616c 2074 7261 6e73 6372  = "Total transcr
-00012a60: 6962 6520 7469 6d65 2020 2020 2020 2020  ibe time        
-00012a70: 2020 2020 2020 2020 2020 203a 2025 733a             : %s:
-00012a80: 2573 3a25 7322 2025 2868 6f75 722e 7a66  %s:%s" %(hour.zf
-00012a90: 696c 6c28 3229 2c20 6d69 6e75 7465 2c20  ill(2), minute, 
-00012aa0: 7365 636f 6e64 290d 0a20 2020 2020 2020  second)..       
-00012ab0: 2020 2020 2020 2020 2070 7269 6e74 286d           print(m
-00012ac0: 7367 290d 0a0d 0a20 2020 2020 2020 2065  sg)....        e
-00012ad0: 7863 6570 7420 4b65 7962 6f61 7264 496e  xcept KeyboardIn
-00012ae0: 7465 7272 7570 743a 0d0a 2020 2020 2020  terrupt:..      
-00012af0: 2020 2020 2020 7062 6172 2e66 696e 6973        pbar.finis
-00012b00: 6828 290d 0a20 2020 2020 2020 2020 2020  h()..           
-00012b10: 2070 6f6f 6c2e 7465 726d 696e 6174 6528   pool.terminate(
-00012b20: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
-00012b30: 6f6f 6c2e 636c 6f73 6528 290d 0a20 2020  ool.close()..   
-00012b40: 2020 2020 2020 2020 2070 6f6f 6c2e 6a6f           pool.jo
-00012b50: 696e 2829 0d0a 2020 2020 2020 2020 2020  in()..          
-00012b60: 2020 7072 696e 7428 2243 616e 6365 6c6c    print("Cancell
-00012b70: 696e 6720 616c 6c20 7461 736b 7322 290d  ing all tasks").
-00012b80: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-00012b90: 6620 7379 732e 706c 6174 666f 726d 203d  f sys.platform =
-00012ba0: 3d20 2277 696e 3332 223a 0d0a 2020 2020  = "win32":..    
-00012bb0: 2020 2020 2020 2020 2020 2020 7374 6f70              stop
-00012bc0: 5f66 666d 7065 675f 7769 6e64 6f77 7328  _ffmpeg_windows(
-00012bd0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-00012be0: 616c 6c62 6163 6b3d 7368 6f77 5f65 7272  allback=show_err
-00012bf0: 6f72 5f6d 6573 7361 6765 7329 0d0a 2020  or_messages)..  
-00012c00: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00012c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012c20: 2073 746f 705f 6666 6d70 6567 5f6c 696e   stop_ffmpeg_lin
-00012c30: 7578 2865 7272 6f72 5f6d 6573 7361 6765  ux(error_message
-00012c40: 735f 6361 6c6c 6261 636b 3d73 686f 775f  s_callback=show_
-00012c50: 6572 726f 725f 6d65 7373 6167 6573 290d  error_messages).
-00012c60: 0a0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
-00012c70: 656d 6f76 655f 7465 6d70 5f66 696c 6573  emove_temp_files
-00012c80: 2822 666c 6163 2229 0d0a 2020 2020 2020  ("flac")..      
-00012c90: 2020 2020 2020 7265 6d6f 7665 5f74 656d        remove_tem
-00012ca0: 705f 6669 6c65 7328 2277 6176 2229 0d0a  p_files("wav")..
-00012cb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00012cc0: 726e 2031 0d0a 0d0a 2020 2020 2020 2020  rn 1....        
-00012cd0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00012ce0: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
-00012cf0: 2020 2020 6966 206e 6f74 204b 6579 626f      if not Keybo
-00012d00: 6172 6449 6e74 6572 7275 7074 2069 6e20  ardInterrupt in 
-00012d10: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00012d20: 2020 2020 7062 6172 2e66 696e 6973 6828      pbar.finish(
-00012d30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012d40: 2020 2070 6f6f 6c2e 7465 726d 696e 6174     pool.terminat
-00012d50: 6528 290d 0a20 2020 2020 2020 2020 2020  e()..           
-00012d60: 2020 2020 2070 6f6f 6c2e 636c 6f73 6528       pool.close(
-00012d70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012d80: 2020 2070 6f6f 6c2e 6a6f 696e 2829 0d0a     pool.join()..
-00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012da0: 7072 696e 7428 6529 0d0a 0d0a 2020 2020  print(e)....    
-00012db0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00012dc0: 7973 2e70 6c61 7466 6f72 6d20 3d3d 2022  ys.platform == "
-00012dd0: 7769 6e33 3222 3a0d 0a20 2020 2020 2020  win32":..       
-00012de0: 2020 2020 2020 2020 2020 2020 2073 746f               sto
-00012df0: 705f 6666 6d70 6567 5f77 696e 646f 7773  p_ffmpeg_windows
-00012e00: 2865 7272 6f72 5f6d 6573 7361 6765 735f  (error_messages_
-00012e10: 6361 6c6c 6261 636b 3d73 686f 775f 6572  callback=show_er
-00012e20: 726f 725f 6d65 7373 6167 6573 290d 0a20  ror_messages).. 
-00012e30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00012e40: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00012e50: 2020 2020 2020 2020 2020 7374 6f70 5f66            stop_f
-00012e60: 666d 7065 675f 6c69 6e75 7828 6572 726f  fmpeg_linux(erro
-00012e70: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-00012e80: 6163 6b3d 7368 6f77 5f65 7272 6f72 5f6d  ack=show_error_m
-00012e90: 6573 7361 6765 7329 0d0a 0d0a 2020 2020  essages)....    
-00012ea0: 2020 2020 2020 2020 2020 2020 7265 6d6f              remo
-00012eb0: 7665 5f74 656d 705f 6669 6c65 7328 2266  ve_temp_files("f
-00012ec0: 6c61 6322 290d 0a20 2020 2020 2020 2020  lac")..         
-00012ed0: 2020 2020 2020 2072 656d 6f76 655f 7465         remove_te
-00012ee0: 6d70 5f66 696c 6573 2822 7761 7622 290d  mp_files("wav").
-00012ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012f00: 2072 6574 7572 6e20 310d 0a0d 0a20 2020   return 1....   
-00012f10: 2069 6620 706f 6f6c 3a0d 0a20 2020 2020   if pool:..     
-00012f20: 2020 2070 6f6f 6c2e 636c 6f73 6528 290d     pool.close().
-00012f30: 0a20 2020 2020 2020 2070 6f6f 6c2e 6a6f  .        pool.jo
-00012f40: 696e 2829 0d0a 2020 2020 2020 2020 706f  in()..        po
-00012f50: 6f6c 203d 204e 6f6e 650d 0a0d 0a20 2020  ol = None....   
-00012f60: 2069 6620 7379 732e 706c 6174 666f 726d   if sys.platform
-00012f70: 203d 3d20 2277 696e 3332 223a 0d0a 2020   == "win32":..  
-00012f80: 2020 2020 2020 7374 6f70 5f66 666d 7065        stop_ffmpe
-00012f90: 675f 7769 6e64 6f77 7328 6572 726f 725f  g_windows(error_
-00012fa0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-00012fb0: 6b3d 7368 6f77 5f65 7272 6f72 5f6d 6573  k=show_error_mes
-00012fc0: 7361 6765 7329 0d0a 2020 2020 656c 7365  sages)..    else
-00012fd0: 3a0d 0a20 2020 2020 2020 2073 746f 705f  :..        stop_
-00012fe0: 6666 6d70 6567 5f6c 696e 7578 2865 7272  ffmpeg_linux(err
-00012ff0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-00013000: 6261 636b 3d73 686f 775f 6572 726f 725f  back=show_error_
-00013010: 6d65 7373 6167 6573 290d 0a0d 0a20 2020  messages)....   
-00013020: 2072 656d 6f76 655f 7465 6d70 5f66 696c   remove_temp_fil
-00013030: 6573 2822 666c 6163 2229 0d0a 2020 2020  es("flac")..    
-00013040: 7265 6d6f 7665 5f74 656d 705f 6669 6c65  remove_temp_file
-00013050: 7328 2277 6176 2229 0d0a 0d0a 6966 205f  s("wav")....if _
-00013060: 5f6e 616d 655f 5f20 3d3d 2027 5f5f 6d61  _name__ == '__ma
-00013070: 696e 5f5f 273a 0d0a 2020 2020 6d75 6c74  in__':..    mult
-00013080: 6970 726f 6365 7373 696e 672e 6672 6565  iprocessing.free
-00013090: 7a65 5f73 7570 706f 7274 2829 0d0a 2020  ze_support()..  
-000130a0: 2020 7379 732e 6578 6974 286d 6169 6e28    sys.exit(main(
-000130b0: 2929 0d0a                                ))..
+0000a090: 6d72 273a 2027 4d61 7261 7468 6927 2c0d  mr': 'Marathi',.
+0000a0a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a0b0: 2020 2020 2020 2020 2027 6d6e 692d 4d74           'mni-Mt
+0000a0c0: 6569 273a 2027 4d65 6974 6569 6c6f 6e20  ei': 'Meiteilon 
+0000a0d0: 284d 616e 6970 7572 6929 272c 0d0a 2020  (Manipuri)',..  
+0000a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0f0: 2020 2020 2020 276c 7573 273a 2027 4d69        'lus': 'Mi
+0000a100: 7a6f 272c 0d0a 2020 2020 2020 2020 2020  zo',..          
+0000a110: 2020 2020 2020 2020 2020 2020 2020 276d                'm
+0000a120: 6e27 3a20 274d 6f6e 676f 6c69 616e 272c  n': 'Mongolian',
+0000a130: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a140: 2020 2020 2020 2020 2020 276d 7927 3a20            'my': 
+0000a150: 274d 7961 6e6d 6172 2028 4275 726d 6573  'Myanmar (Burmes
+0000a160: 6529 272c 0d0a 2020 2020 2020 2020 2020  e)',..          
+0000a170: 2020 2020 2020 2020 2020 2020 2020 276e                'n
+0000a180: 6527 3a20 274e 6570 616c 6927 2c0d 0a20  e': 'Nepali',.. 
+0000a190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1a0: 2020 2020 2020 2027 6e6f 273a 2027 4e6f         'no': 'No
+0000a1b0: 7277 6567 6961 6e27 2c0d 0a20 2020 2020  rwegian',..     
+0000a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1d0: 2020 2027 6f72 273a 2027 4f64 6979 6120     'or': 'Odiya 
+0000a1e0: 284f 7269 7961 2927 2c0d 0a20 2020 2020  (Oriya)',..     
+0000a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a200: 2020 2027 6f6d 273a 2027 4f72 6f6d 6f27     'om': 'Oromo'
+0000a210: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a220: 2020 2020 2020 2020 2020 2027 7073 273a             'ps':
+0000a230: 2027 5061 7368 746f 272c 0d0a 2020 2020   'Pashto',..    
+0000a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a250: 2020 2020 2766 6127 3a20 2750 6572 7369      'fa': 'Persi
+0000a260: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
+0000a270: 2020 2020 2020 2020 2020 2020 2020 2770                'p
+0000a280: 6c27 3a20 2750 6f6c 6973 6827 2c0d 0a20  l': 'Polish',.. 
+0000a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2a0: 2020 2020 2020 2027 7074 273a 2027 506f         'pt': 'Po
+0000a2b0: 7274 7567 7565 7365 272c 0d0a 2020 2020  rtuguese',..    
+0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2d0: 2020 2020 2770 6127 3a20 2750 756e 6a61      'pa': 'Punja
+0000a2e0: 6269 272c 0d0a 2020 2020 2020 2020 2020  bi',..          
+0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2771                'q
+0000a300: 7527 3a20 2751 7565 6368 7561 272c 0d0a  u': 'Quechua',..
+0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a320: 2020 2020 2020 2020 2772 6f27 3a20 2752          'ro': 'R
+0000a330: 6f6d 616e 6961 6e27 2c0d 0a20 2020 2020  omanian',..     
+0000a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a350: 2020 2027 7275 273a 2027 5275 7373 6961     'ru': 'Russia
+0000a360: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+0000a370: 2020 2020 2020 2020 2020 2020 2027 736d               'sm
+0000a380: 273a 2027 5361 6d6f 616e 272c 0d0a 2020  ': 'Samoan',..  
+0000a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3a0: 2020 2020 2020 2773 6127 3a20 2753 616e        'sa': 'San
+0000a3b0: 736b 7269 7427 2c0d 0a20 2020 2020 2020  skrit',..       
+0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3d0: 2027 6764 273a 2027 5363 6f74 7320 4761   'gd': 'Scots Ga
+0000a3e0: 656c 6963 272c 0d0a 2020 2020 2020 2020  elic',..        
+0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a400: 276e 736f 273a 2027 5365 7065 6469 272c  'nso': 'Sepedi',
+0000a410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a420: 2020 2020 2020 2020 2020 2773 7227 3a20            'sr': 
+0000a430: 2753 6572 6269 616e 272c 0d0a 2020 2020  'Serbian',..    
+0000a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a450: 2020 2020 2773 7427 3a20 2753 6573 6f74      'st': 'Sesot
+0000a460: 686f 272c 0d0a 2020 2020 2020 2020 2020  ho',..          
+0000a470: 2020 2020 2020 2020 2020 2020 2020 2773                's
+0000a480: 6e27 3a20 2753 686f 6e61 272c 0d0a 2020  n': 'Shona',..  
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 2020 2020 2020 2773 6427 3a20 2753 696e        'sd': 'Sin
+0000a4b0: 6468 6927 2c0d 0a20 2020 2020 2020 2020  dhi',..         
+0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000a4d0: 7369 273a 2027 5369 6e68 616c 6127 2c0d  si': 'Sinhala',.
+0000a4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a4f0: 2020 2020 2020 2020 2027 736b 273a 2027           'sk': '
+0000a500: 536c 6f76 616b 272c 0d0a 2020 2020 2020  Slovak',..      
+0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a520: 2020 2773 6c27 3a20 2753 6c6f 7665 6e69    'sl': 'Sloveni
+0000a530: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
+0000a540: 2020 2020 2020 2020 2020 2020 2020 2773                's
+0000a550: 6f27 3a20 2753 6f6d 616c 6927 2c0d 0a20  o': 'Somali',.. 
+0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a570: 2020 2020 2020 2027 6573 273a 2027 5370         'es': 'Sp
+0000a580: 616e 6973 6827 2c0d 0a20 2020 2020 2020  anish',..       
+0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5a0: 2027 7375 273a 2027 5375 6e64 616e 6573   'su': 'Sundanes
+0000a5b0: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
+0000a5c0: 2020 2020 2020 2020 2020 2020 2027 7377               'sw
+0000a5d0: 273a 2027 5377 6168 696c 6927 2c0d 0a20  ': 'Swahili',.. 
+0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5f0: 2020 2020 2020 2027 7376 273a 2027 5377         'sv': 'Sw
+0000a600: 6564 6973 6827 2c0d 0a20 2020 2020 2020  edish',..       
+0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a620: 2027 7467 273a 2027 5461 6a69 6b27 2c0d   'tg': 'Tajik',.
+0000a630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a640: 2020 2020 2020 2020 2027 7461 273a 2027           'ta': '
+0000a650: 5461 6d69 6c27 2c0d 0a20 2020 2020 2020  Tamil',..       
+0000a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a670: 2027 7474 273a 2027 5461 7461 7227 2c0d   'tt': 'Tatar',.
+0000a680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a690: 2020 2020 2020 2020 2027 7465 273a 2027           'te': '
+0000a6a0: 5465 6c75 6775 272c 0d0a 2020 2020 2020  Telugu',..      
+0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6c0: 2020 2774 6827 3a20 2754 6861 6927 2c0d    'th': 'Thai',.
+0000a6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a6e0: 2020 2020 2020 2020 2027 7469 273a 2027           'ti': '
+0000a6f0: 5469 6772 696e 7961 272c 0d0a 2020 2020  Tigrinya',..    
+0000a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a710: 2020 2020 2774 7327 3a20 2754 736f 6e67      'ts': 'Tsong
+0000a720: 6127 2c0d 0a20 2020 2020 2020 2020 2020  a',..           
+0000a730: 2020 2020 2020 2020 2020 2020 2027 7472               'tr
+0000a740: 273a 2027 5475 726b 6973 6827 2c0d 0a20  ': 'Turkish',.. 
+0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a760: 2020 2020 2020 2027 746b 273a 2027 5475         'tk': 'Tu
+0000a770: 726b 6d65 6e27 2c0d 0a20 2020 2020 2020  rkmen',..       
+0000a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a790: 2027 7477 273a 2027 5477 6920 2841 6b61   'tw': 'Twi (Aka
+0000a7a0: 6e29 272c 0d0a 2020 2020 2020 2020 2020  n)',..          
+0000a7b0: 2020 2020 2020 2020 2020 2020 2020 2775                'u
+0000a7c0: 6b27 3a20 2755 6b72 6169 6e69 616e 272c  k': 'Ukrainian',
+0000a7d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a7e0: 2020 2020 2020 2020 2020 2775 7227 3a20            'ur': 
+0000a7f0: 2755 7264 7527 2c0d 0a20 2020 2020 2020  'Urdu',..       
+0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a810: 2027 7567 273a 2027 5579 6768 7572 272c   'ug': 'Uyghur',
+0000a820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a830: 2020 2020 2020 2020 2020 2775 7a27 3a20            'uz': 
+0000a840: 2755 7a62 656b 272c 0d0a 2020 2020 2020  'Uzbek',..      
+0000a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a860: 2020 2776 6927 3a20 2756 6965 746e 616d    'vi': 'Vietnam
+0000a870: 6573 6527 2c0d 0a20 2020 2020 2020 2020  ese',..         
+0000a880: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000a890: 6379 273a 2027 5765 6c73 6827 2c0d 0a20  cy': 'Welsh',.. 
+0000a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8b0: 2020 2020 2020 2027 7868 273a 2027 5868         'xh': 'Xh
+0000a8c0: 6f73 6127 2c0d 0a20 2020 2020 2020 2020  osa',..         
+0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000a8e0: 7969 273a 2027 5969 6464 6973 6827 2c0d  yi': 'Yiddish',.
+0000a8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a900: 2020 2020 2020 2020 2027 796f 273a 2027           'yo': '
+0000a910: 596f 7275 6261 272c 0d0a 2020 2020 2020  Yoruba',..      
+0000a920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a930: 2020 277a 7527 3a20 275a 756c 7527 2c0d    'zu': 'Zulu',.
+0000a940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a950: 2020 2020 207d 0d0a 0d0a 2020 2020 6465       }....    de
+0000a960: 6620 6765 745f 6e61 6d65 2873 656c 662c  f get_name(self,
+0000a970: 2067 6574 5f63 6f64 6529 3a0d 0a20 2020   get_code):..   
+0000a980: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000a990: 2e64 6963 742e 6765 7428 6765 745f 636f  .dict.get(get_co
+0000a9a0: 6465 2e6c 6f77 6572 2829 2c20 2222 290d  de.lower(), "").
+0000a9b0: 0a0d 0a20 2020 2064 6566 2067 6574 5f63  ...    def get_c
+0000a9c0: 6f64 6528 7365 6c66 2c20 6c61 6e67 7561  ode(self, langua
+0000a9d0: 6765 293a 0d0a 2020 2020 2020 2020 666f  ge):..        fo
+0000a9e0: 7220 6765 745f 636f 6465 2c20 6c61 6e67  r get_code, lang
+0000a9f0: 2069 6e20 7365 6c66 2e64 6963 742e 6974   in self.dict.it
+0000aa00: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
+0000aa10: 2020 2020 6966 206c 616e 672e 6c6f 7765      if lang.lowe
+0000aa20: 7228 2920 3d3d 206c 616e 6775 6167 652e  r() == language.
+0000aa30: 6c6f 7765 7228 293a 0d0a 2020 2020 2020  lower():..      
+0000aa40: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000aa50: 2067 6574 5f63 6f64 650d 0a20 2020 2020   get_code..     
+0000aa60: 2020 2072 6574 7572 6e20 2222 0d0a 0d0a     return ""....
+0000aa70: 0d0a 636c 6173 7320 5761 7643 6f6e 7665  ..class WavConve
+0000aa80: 7274 6572 3a0d 0a20 2020 2040 7374 6174  rter:..    @stat
+0000aa90: 6963 6d65 7468 6f64 0d0a 2020 2020 6465  icmethod..    de
+0000aaa0: 6620 7768 6963 6828 7072 6f67 7261 6d29  f which(program)
+0000aab0: 3a0d 0a20 2020 2020 2020 2064 6566 2069  :..        def i
+0000aac0: 735f 6578 6528 6669 6c65 5f70 6174 6829  s_exe(file_path)
+0000aad0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+0000aae0: 6574 7572 6e20 6f73 2e70 6174 682e 6973  eturn os.path.is
+0000aaf0: 6669 6c65 2866 696c 655f 7061 7468 2920  file(file_path) 
+0000ab00: 616e 6420 6f73 2e61 6363 6573 7328 6669  and os.access(fi
+0000ab10: 6c65 5f70 6174 682c 206f 732e 585f 4f4b  le_path, os.X_OK
+0000ab20: 290d 0a20 2020 2020 2020 2066 7061 7468  )..        fpath
+0000ab30: 2c20 5f20 3d20 6f73 2e70 6174 682e 7370  , _ = os.path.sp
+0000ab40: 6c69 7428 7072 6f67 7261 6d29 0d0a 2020  lit(program)..  
+0000ab50: 2020 2020 2020 6966 2066 7061 7468 3a0d        if fpath:.
+0000ab60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000ab70: 6973 5f65 7865 2870 726f 6772 616d 293a  is_exe(program):
+0000ab80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ab90: 2020 7265 7475 726e 2070 726f 6772 616d    return program
+0000aba0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+0000abb0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000abc0: 2070 6174 6820 696e 206f 732e 656e 7669   path in os.envi
+0000abd0: 726f 6e5b 2250 4154 4822 5d2e 7370 6c69  ron["PATH"].spli
+0000abe0: 7428 6f73 2e70 6174 6873 6570 293a 0d0a  t(os.pathsep):..
+0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac00: 7061 7468 203d 2070 6174 682e 7374 7269  path = path.stri
+0000ac10: 7028 2722 2729 0d0a 2020 2020 2020 2020  p('"')..        
+0000ac20: 2020 2020 2020 2020 6578 655f 6669 6c65          exe_file
+0000ac30: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+0000ac40: 7061 7468 2c20 7072 6f67 7261 6d29 0d0a  path, program)..
+0000ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac60: 6966 2069 735f 6578 6528 6578 655f 6669  if is_exe(exe_fi
+0000ac70: 6c65 293a 0d0a 2020 2020 2020 2020 2020  le):..          
+0000ac80: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000ac90: 2065 7865 5f66 696c 650d 0a20 2020 2020   exe_file..     
+0000aca0: 2020 2072 6574 7572 6e20 4e6f 6e65 0d0a     return None..
+0000acb0: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+0000acc0: 686f 640d 0a20 2020 2064 6566 2066 666d  hod..    def ffm
+0000acd0: 7065 675f 6368 6563 6b28 293a 0d0a 2020  peg_check():..  
+0000ace0: 2020 2020 2020 6966 2057 6176 436f 6e76        if WavConv
+0000acf0: 6572 7465 722e 7768 6963 6828 2266 666d  erter.which("ffm
+0000ad00: 7065 6722 293a 0d0a 2020 2020 2020 2020  peg"):..        
+0000ad10: 2020 2020 7265 7475 726e 2022 6666 6d70      return "ffmp
+0000ad20: 6567 220d 0a20 2020 2020 2020 2069 6620  eg"..        if 
+0000ad30: 5761 7643 6f6e 7665 7274 6572 2e77 6869  WavConverter.whi
+0000ad40: 6368 2822 6666 6d70 6567 2e65 7865 2229  ch("ffmpeg.exe")
+0000ad50: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+0000ad60: 6574 7572 6e20 2266 666d 7065 672e 6578  eturn "ffmpeg.ex
+0000ad70: 6522 0d0a 2020 2020 2020 2020 7265 7475  e"..        retu
+0000ad80: 726e 204e 6f6e 650d 0a0d 0a20 2020 2064  rn None....    d
+0000ad90: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+0000ada0: 2c20 6368 616e 6e65 6c73 3d31 2c20 7261  , channels=1, ra
+0000adb0: 7465 3d34 3830 3030 2c20 7072 6f67 7265  te=48000, progre
+0000adc0: 7373 5f63 616c 6c62 6163 6b3d 4e6f 6e65  ss_callback=None
+0000add0: 2c20 6572 726f 725f 6d65 7373 6167 6573  , error_messages
+0000ade0: 5f63 616c 6c62 6163 6b3d 4e6f 6e65 293a  _callback=None):
+0000adf0: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+0000ae00: 6861 6e6e 656c 7320 3d20 6368 616e 6e65  hannels = channe
+0000ae10: 6c73 0d0a 2020 2020 2020 2020 7365 6c66  ls..        self
+0000ae20: 2e72 6174 6520 3d20 7261 7465 0d0a 2020  .rate = rate..  
+0000ae30: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+0000ae40: 6573 735f 6361 6c6c 6261 636b 203d 2070  ess_callback = p
+0000ae50: 726f 6772 6573 735f 6361 6c6c 6261 636b  rogress_callback
+0000ae60: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
+0000ae70: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+0000ae80: 6c6c 6261 636b 203d 2065 7272 6f72 5f6d  llback = error_m
+0000ae90: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+0000aea0: 0d0a 0d0a 2020 2020 6465 6620 5f5f 6361  ....    def __ca
+0000aeb0: 6c6c 5f5f 2873 656c 662c 206d 6564 6961  ll__(self, media
+0000aec0: 5f66 696c 6570 6174 6829 3a0d 0a20 2020  _filepath):..   
+0000aed0: 2020 2020 2074 656d 7020 3d20 7465 6d70       temp = temp
+0000aee0: 6669 6c65 2e4e 616d 6564 5465 6d70 6f72  file.NamedTempor
+0000aef0: 6172 7946 696c 6528 7375 6666 6978 3d27  aryFile(suffix='
+0000af00: 2e77 6176 272c 2064 656c 6574 653d 4661  .wav', delete=Fa
+0000af10: 6c73 6529 0d0a 2020 2020 2020 2020 6966  lse)..        if
+0000af20: 206e 6f74 206f 732e 7061 7468 2e69 7366   not os.path.isf
+0000af30: 696c 6528 6d65 6469 615f 6669 6c65 7061  ile(media_filepa
+0000af40: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
+0000af50: 2020 6966 2073 656c 662e 6572 726f 725f    if self.error_
+0000af60: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+0000af70: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
+0000af80: 2020 2020 7365 6c66 2e65 7272 6f72 5f6d      self.error_m
+0000af90: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+0000afa0: 2822 5468 6520 6769 7665 6e20 6669 6c65  ("The given file
+0000afb0: 2064 6f65 7320 6e6f 7420 6578 6973 743a   does not exist:
+0000afc0: 207b 307d 222e 666f 726d 6174 286d 6564   {0}".format(med
+0000afd0: 6961 5f66 696c 6570 6174 6829 290d 0a20  ia_filepath)).. 
+0000afe0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000aff0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b000: 2020 7072 696e 7428 2254 6865 2067 6976    print("The giv
+0000b010: 656e 2066 696c 6520 646f 6573 206e 6f74  en file does not
+0000b020: 2065 7869 7374 3a20 7b30 7d22 2e66 6f72   exist: {0}".for
+0000b030: 6d61 7428 6d65 6469 615f 6669 6c65 7061  mat(media_filepa
+0000b040: 7468 2929 0d0a 2020 2020 2020 2020 2020  th))..          
+0000b050: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
+0000b060: 7074 696f 6e28 2249 6e76 616c 6964 2066  ption("Invalid f
+0000b070: 696c 653a 207b 307d 222e 666f 726d 6174  ile: {0}".format
+0000b080: 286d 6564 6961 5f66 696c 6570 6174 6829  (media_filepath)
+0000b090: 290d 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+0000b0a0: 7420 7365 6c66 2e66 666d 7065 675f 6368  t self.ffmpeg_ch
+0000b0b0: 6563 6b28 293a 0d0a 2020 2020 2020 2020  eck():..        
+0000b0c0: 2020 2020 6966 2073 656c 662e 6572 726f      if self.erro
+0000b0d0: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000b0e0: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
+0000b0f0: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
+0000b100: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000b110: 636b 2822 6666 6d70 6567 3a20 4578 6563  ck("ffmpeg: Exec
+0000b120: 7574 6162 6c65 206e 6f74 2066 6f75 6e64  utable not found
+0000b130: 206f 6e20 6d61 6368 696e 652e 2229 0d0a   on machine.")..
+0000b140: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000b150: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000b160: 2020 2070 7269 6e74 2822 6666 6d70 6567     print("ffmpeg
+0000b170: 3a20 4578 6563 7574 6162 6c65 206e 6f74  : Executable not
+0000b180: 2066 6f75 6e64 206f 6e20 6d61 6368 696e   found on machin
+0000b190: 652e 2229 0d0a 2020 2020 2020 2020 2020  e.")..          
+0000b1a0: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
+0000b1b0: 7074 696f 6e28 2244 6570 656e 6465 6e63  ption("Dependenc
+0000b1c0: 7920 6e6f 7420 666f 756e 643a 2066 666d  y not found: ffm
+0000b1d0: 7065 6722 290d 0a0d 0a20 2020 2020 2020  peg")....       
+0000b1e0: 2063 6f6d 6d61 6e64 203d 205b 0d0a 2020   command = [..  
+0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b200: 2020 2266 666d 7065 6722 2c0d 0a20 2020    "ffmpeg",..   
+0000b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b220: 2022 2d79 222c 0d0a 2020 2020 2020 2020   "-y",..        
+0000b230: 2020 2020 2020 2020 2020 2020 222d 6922              "-i"
+0000b240: 2c20 6d65 6469 615f 6669 6c65 7061 7468  , media_filepath
+0000b250: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000b260: 2020 2020 2020 2022 2d61 6322 2c20 7374         "-ac", st
+0000b270: 7228 7365 6c66 2e63 6861 6e6e 656c 7329  r(self.channels)
+0000b280: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000b290: 2020 2020 2020 2022 2d61 7222 2c20 7374         "-ar", st
+0000b2a0: 7228 7365 6c66 2e72 6174 6529 2c0d 0a20  r(self.rate),.. 
+0000b2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2c0: 2020 2022 2d6c 6f67 6c65 7665 6c22 2c20     "-loglevel", 
+0000b2d0: 2265 7272 6f72 222c 0d0a 2020 2020 2020  "error",..      
+0000b2e0: 2020 2020 2020 2020 2020 2020 2020 222d                "-
+0000b2f0: 6869 6465 5f62 616e 6e65 7222 2c0d 0a20  hide_banner",.. 
+0000b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b310: 2020 2074 656d 702e 6e61 6d65 0d0a 2020     temp.name..  
+0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b330: 5d0d 0a0d 0a20 2020 2020 2020 2074 7279  ]....        try
+0000b340: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+0000b350: 2052 554e 4e49 4e47 2066 666d 7065 6720   RUNNING ffmpeg 
+0000b360: 5749 5448 4f55 5420 5348 4f57 494e 4720  WITHOUT SHOWING 
+0000b370: 5052 4f47 5245 5353 530d 0a20 2020 2020  PROGRESSS..     
+0000b380: 2020 2020 2020 2023 7573 655f 7368 656c         #use_shel
+0000b390: 6c20 3d20 5472 7565 2069 6620 6f73 2e6e  l = True if os.n
+0000b3a0: 616d 6520 3d3d 2022 6e74 2220 656c 7365  ame == "nt" else
+0000b3b0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+0000b3c0: 2020 2020 2373 7562 7072 6f63 6573 732e      #subprocess.
+0000b3d0: 6368 6563 6b5f 6f75 7470 7574 2863 6f6d  check_output(com
+0000b3e0: 6d61 6e64 2c20 7374 6469 6e3d 6f70 656e  mand, stdin=open
+0000b3f0: 286f 732e 6465 766e 756c 6c29 2c20 7368  (os.devnull), sh
+0000b400: 656c 6c3d 7573 655f 7368 656c 6c29 0d0a  ell=use_shell)..
+0000b410: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000b420: 5255 4e4e 494e 4720 6666 6d70 6567 2057  RUNNING ffmpeg W
+0000b430: 4954 4820 5052 4f47 5245 5353 530d 0a20  ITH PROGRESSS.. 
+0000b440: 2020 2020 2020 2020 2020 2066 6620 3d20             ff = 
+0000b450: 4666 6d70 6567 5072 6f67 7265 7373 2863  FfmpegProgress(c
+0000b460: 6f6d 6d61 6e64 290d 0a20 2020 2020 2020  ommand)..       
+0000b470: 2020 2020 2070 6572 6365 6e74 6167 6520       percentage 
+0000b480: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
+0000b490: 2066 6f72 2070 726f 6772 6573 7320 696e   for progress in
+0000b4a0: 2066 662e 7275 6e5f 636f 6d6d 616e 645f   ff.run_command_
+0000b4b0: 7769 7468 5f70 726f 6772 6573 7328 293a  with_progress():
+0000b4c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b4d0: 2020 7065 7263 656e 7461 6765 203d 2070    percentage = p
+0000b4e0: 726f 6772 6573 730d 0a20 2020 2020 2020  rogress..       
+0000b4f0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000b500: 2e70 726f 6772 6573 735f 6361 6c6c 6261  .progress_callba
+0000b510: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
+0000b520: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000b530: 6f67 7265 7373 5f63 616c 6c62 6163 6b28  ogress_callback(
+0000b540: 6d65 6469 615f 6669 6c65 7061 7468 2c20  media_filepath, 
+0000b550: 7065 7263 656e 7461 6765 290d 0a20 2020  percentage)..   
+0000b560: 2020 2020 2020 2020 2074 656d 702e 636c           temp.cl
+0000b570: 6f73 6528 290d 0a0d 0a20 2020 2020 2020  ose()....       
+0000b580: 2020 2020 2072 6574 7572 6e20 7465 6d70       return temp
+0000b590: 2e6e 616d 652c 2073 656c 662e 7261 7465  .name, self.rate
+0000b5a0: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
+0000b5b0: 7074 204b 6579 626f 6172 6449 6e74 6572  pt KeyboardInter
+0000b5c0: 7275 7074 3a0d 0a20 2020 2020 2020 2020  rupt:..         
+0000b5d0: 2020 2069 6620 7365 6c66 2e65 7272 6f72     if self.error
+0000b5e0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000b5f0: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
+0000b600: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
+0000b610: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+0000b620: 6b28 2243 616e 6365 6c6c 696e 6720 616c  k("Cancelling al
+0000b630: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
+0000b640: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0000b650: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000b660: 696e 7428 2243 616e 6365 6c6c 696e 6720  int("Cancelling 
+0000b670: 616c 6c20 7461 736b 7322 290d 0a20 2020  all tasks")..   
+0000b680: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
+0000b690: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
+0000b6a0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+0000b6b0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+0000b6c0: 6620 7365 6c66 2e65 7272 6f72 5f6d 6573  f self.error_mes
+0000b6d0: 7361 6765 735f 6361 6c6c 6261 636b 3a0d  sages_callback:.
+0000b6e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b6f0: 2073 656c 662e 6572 726f 725f 6d65 7373   self.error_mess
+0000b700: 6167 6573 5f63 616c 6c62 6163 6b28 6529  ages_callback(e)
+0000b710: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+0000b720: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000b730: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
+0000b740: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000b750: 6e0d 0a0d 0a0d 0a63 6c61 7373 2053 656e  n......class Sen
+0000b760: 7465 6e63 6554 7261 6e73 6c61 746f 7228  tenceTranslator(
+0000b770: 6f62 6a65 6374 293a 0d0a 2020 2020 6465  object):..    de
+0000b780: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+0000b790: 2073 7263 2c20 6473 742c 2070 6174 6965   src, dst, patie
+0000b7a0: 6e63 653d 2d31 2c20 7469 6d65 6f75 743d  nce=-1, timeout=
+0000b7b0: 3330 2c20 6572 726f 725f 6d65 7373 6167  30, error_messag
+0000b7c0: 6573 5f63 616c 6c62 6163 6b3d 4e6f 6e65  es_callback=None
+0000b7d0: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+0000b7e0: 2e73 7263 203d 2073 7263 0d0a 2020 2020  .src = src..    
+0000b7f0: 2020 2020 7365 6c66 2e64 7374 203d 2064      self.dst = d
+0000b800: 7374 0d0a 2020 2020 2020 2020 7365 6c66  st..        self
+0000b810: 2e70 6174 6965 6e63 6520 3d20 7061 7469  .patience = pati
+0000b820: 656e 6365 0d0a 2020 2020 2020 2020 7365  ence..        se
+0000b830: 6c66 2e74 696d 656f 7574 203d 2074 696d  lf.timeout = tim
+0000b840: 656f 7574 0d0a 2020 2020 2020 2020 7365  eout..        se
+0000b850: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
+0000b860: 735f 6361 6c6c 6261 636b 203d 2065 7272  s_callback = err
+0000b870: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000b880: 6261 636b 0d0a 0d0a 2020 2020 6465 6620  back....    def 
+0000b890: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2073  __call__(self, s
+0000b8a0: 656e 7465 6e63 6529 3a0d 0a20 2020 2020  entence):..     
+0000b8b0: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+0000b8c0: 2020 2020 2074 7261 6e73 6c61 7465 645f       translated_
+0000b8d0: 7365 6e74 656e 6365 203d 205b 5d0d 0a20  sentence = [].. 
+0000b8e0: 2020 2020 2020 2020 2020 2023 2068 616e             # han
+0000b8f0: 646c 6520 7468 6520 7370 6563 6961 6c20  dle the special 
+0000b900: 6361 7365 3a20 656d 7074 7920 7374 7269  case: empty stri
+0000b910: 6e67 2e0d 0a20 2020 2020 2020 2020 2020  ng...           
+0000b920: 2069 6620 6e6f 7420 7365 6e74 656e 6365   if not sentence
+0000b930: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000b940: 2020 2072 6574 7572 6e20 4e6f 6e65 0d0a     return None..
+0000b950: 2020 2020 2020 2020 2020 2020 7472 616e              tran
+0000b960: 736c 6174 6564 5f73 656e 7465 6e63 6520  slated_sentence 
+0000b970: 3d20 7365 6c66 2e47 6f6f 676c 6554 7261  = self.GoogleTra
+0000b980: 6e73 6c61 7465 2873 656e 7465 6e63 652c  nslate(sentence,
+0000b990: 2073 7263 3d73 656c 662e 7372 632c 2064   src=self.src, d
+0000b9a0: 7374 3d73 656c 662e 6473 742c 2074 696d  st=self.dst, tim
+0000b9b0: 656f 7574 3d73 656c 662e 7469 6d65 6f75  eout=self.timeou
+0000b9c0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+0000b9d0: 6661 696c 5f74 6f5f 7472 616e 736c 6174  fail_to_translat
+0000b9e0: 6520 3d20 7472 616e 736c 6174 6564 5f73  e = translated_s
+0000b9f0: 656e 7465 6e63 655b 2d31 5d20 3d3d 2027  entence[-1] == '
+0000ba00: 5c6e 270d 0a20 2020 2020 2020 2020 2020  \n'..           
+0000ba10: 2077 6869 6c65 2066 6169 6c5f 746f 5f74   while fail_to_t
+0000ba20: 7261 6e73 6c61 7465 2061 6e64 2070 6174  ranslate and pat
+0000ba30: 6965 6e63 653a 0d0a 2020 2020 2020 2020  ience:..        
+0000ba40: 2020 2020 2020 2020 7472 616e 736c 6174          translat
+0000ba50: 6564 5f73 656e 7465 6e63 6520 3d20 7365  ed_sentence = se
+0000ba60: 6c66 2e47 6f6f 676c 6554 7261 6e73 6c61  lf.GoogleTransla
+0000ba70: 7465 2874 7261 6e73 6c61 7465 645f 7365  te(translated_se
+0000ba80: 6e74 656e 6365 2c20 7372 633d 7365 6c66  ntence, src=self
+0000ba90: 2e73 7263 2c20 6473 743d 7365 6c66 2e64  .src, dst=self.d
+0000baa0: 7374 2c20 7469 6d65 6f75 743d 7365 6c66  st, timeout=self
+0000bab0: 2e74 696d 656f 7574 292e 7465 7874 0d0a  .timeout).text..
+0000bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bad0: 6966 2074 7261 6e73 6c61 7465 645f 7365  if translated_se
+0000bae0: 6e74 656e 6365 5b2d 315d 203d 3d20 275c  ntence[-1] == '\
+0000baf0: 6e27 3a0d 0a20 2020 2020 2020 2020 2020  n':..           
+0000bb00: 2020 2020 2020 2020 2069 6620 7061 7469           if pati
+0000bb10: 656e 6365 203d 3d20 2d31 3a0d 0a20 2020  ence == -1:..   
+0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb30: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
+0000bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb50: 2020 2070 6174 6965 6e63 6520 2d3d 2031     patience -= 1
+0000bb60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bb70: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0000bb80: 2020 2020 2020 2020 2020 2020 2066 6169               fai
+0000bb90: 6c5f 746f 5f74 7261 6e73 6c61 7465 203d  l_to_translate =
+0000bba0: 2046 616c 7365 0d0a 0d0a 2020 2020 2020   False....      
+0000bbb0: 2020 2020 2020 7265 7475 726e 2074 7261        return tra
+0000bbc0: 6e73 6c61 7465 645f 7365 6e74 656e 6365  nslated_sentence
+0000bbd0: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
+0000bbe0: 7074 204b 6579 626f 6172 6449 6e74 6572  pt KeyboardInter
+0000bbf0: 7275 7074 3a0d 0a20 2020 2020 2020 2020  rupt:..         
+0000bc00: 2020 2069 6620 7365 6c66 2e65 7272 6f72     if self.error
+0000bc10: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000bc20: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
+0000bc30: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
+0000bc40: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+0000bc50: 6b28 2243 616e 6365 6c6c 696e 6720 616c  k("Cancelling al
+0000bc60: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
+0000bc70: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0000bc80: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000bc90: 696e 7428 2243 616e 6365 6c6c 696e 6720  int("Cancelling 
+0000bca0: 616c 6c20 7461 736b 7322 290d 0a20 2020  all tasks")..   
+0000bcb0: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
+0000bcc0: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
+0000bcd0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+0000bce0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+0000bcf0: 6620 7365 6c66 2e65 7272 6f72 5f6d 6573  f self.error_mes
+0000bd00: 7361 6765 735f 6361 6c6c 6261 636b 3a0d  sages_callback:.
+0000bd10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bd20: 2073 656c 662e 6572 726f 725f 6d65 7373   self.error_mess
+0000bd30: 6167 6573 5f63 616c 6c62 6163 6b28 6529  ages_callback(e)
+0000bd40: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+0000bd50: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000bd60: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
+0000bd70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000bd80: 6e0d 0a0d 0a20 2020 2064 6566 2047 6f6f  n....    def Goo
+0000bd90: 676c 6554 7261 6e73 6c61 7465 2873 656c  gleTranslate(sel
+0000bda0: 662c 2074 6578 742c 2073 7263 2c20 6473  f, text, src, ds
+0000bdb0: 742c 2074 696d 656f 7574 3d33 3029 3a0d  t, timeout=30):.
+0000bdc0: 0a20 2020 2020 2020 2075 726c 203d 2027  .        url = '
+0000bdd0: 6874 7470 733a 2f2f 7472 616e 736c 6174  https://translat
+0000bde0: 652e 676f 6f67 6c65 6170 6973 2e63 6f6d  e.googleapis.com
+0000bdf0: 2f74 7261 6e73 6c61 7465 5f61 2f27 0d0a  /translate_a/'..
+0000be00: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
+0000be10: 2027 7369 6e67 6c65 3f63 6c69 656e 743d   'single?client=
+0000be20: 6774 7826 736c 3d27 2b73 7263 2b27 2674  gtx&sl='+src+'&t
+0000be30: 6c3d 272b 6473 742b 2726 6474 3d74 2671  l='+dst+'&dt=t&q
+0000be40: 3d27 2b74 6578 743b 0d0a 2020 2020 2020  ='+text;..      
+0000be50: 2020 6865 6164 6572 7320 3d20 7b27 5573    headers = {'Us
+0000be60: 6572 2d41 6765 6e74 273a 2027 4d6f 7a69  er-Agent': 'Mozi
+0000be70: 6c6c 612f 352e 3020 2857 696e 646f 7773  lla/5.0 (Windows
+0000be80: 204e 5420 3130 2e30 3b20 5769 6e36 343b   NT 10.0; Win64;
+0000be90: 2078 3634 2927 2c20 2752 6566 6572 6572   x64)', 'Referer
+0000bea0: 273a 2027 6874 7470 733a 2f2f 7472 616e  ': 'https://tran
+0000beb0: 736c 6174 652e 676f 6f67 6c65 2e63 6f6d  slate.google.com
+0000bec0: 272c 7d0d 0a0d 0a20 2020 2020 2020 2074  ',}....        t
+0000bed0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+0000bee0: 2072 6573 706f 6e73 6520 3d20 7265 7175   response = requ
+0000bef0: 6573 7473 2e67 6574 2875 726c 2b70 6172  ests.get(url+par
+0000bf00: 616d 732c 2068 6561 6465 7273 3d68 6561  ams, headers=hea
+0000bf10: 6465 7273 2c20 7469 6d65 6f75 743d 7365  ders, timeout=se
+0000bf20: 6c66 2e74 696d 656f 7574 290d 0a20 2020  lf.timeout)..   
+0000bf30: 2020 2020 2020 2020 2069 6620 7265 7370           if resp
+0000bf40: 6f6e 7365 2e73 7461 7475 735f 636f 6465  onse.status_code
+0000bf50: 203d 3d20 3230 303a 0d0a 2020 2020 2020   == 200:..      
+0000bf60: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+0000bf70: 7365 5f6a 736f 6e20 3d20 7265 7370 6f6e  se_json = respon
+0000bf80: 7365 2e6a 736f 6e28 295b 305d 0d0a 2020  se.json()[0]..  
+0000bf90: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+0000bfa0: 6e67 7468 203d 206c 656e 2872 6573 706f  ngth = len(respo
+0000bfb0: 6e73 655f 6a73 6f6e 290d 0a20 2020 2020  nse_json)..     
+0000bfc0: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
+0000bfd0: 6c61 7469 6f6e 203d 2022 220d 0a20 2020  lation = ""..   
+0000bfe0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000bff0: 2069 2069 6e20 7261 6e67 6528 6c65 6e67   i in range(leng
+0000c000: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
+0000c010: 2020 2020 2020 2020 2020 7472 616e 736c            transl
+0000c020: 6174 696f 6e20 3d20 7472 616e 736c 6174  ation = translat
+0000c030: 696f 6e20 2b20 7265 7370 6f6e 7365 5f6a  ion + response_j
+0000c040: 736f 6e5b 695d 5b30 5d0d 0a20 2020 2020  son[i][0]..     
+0000c050: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000c060: 6e20 7472 616e 736c 6174 696f 6e0d 0a20  n translation.. 
+0000c070: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000c080: 6e0d 0a0d 0a20 2020 2020 2020 2065 7863  n....        exc
+0000c090: 6570 7420 7265 7175 6573 7473 2e65 7863  ept requests.exc
+0000c0a0: 6570 7469 6f6e 732e 436f 6e6e 6563 7469  eptions.Connecti
+0000c0b0: 6f6e 4572 726f 723a 0d0a 2020 2020 2020  onError:..      
+0000c0c0: 2020 2020 2020 7769 7468 2068 7474 7078        with httpx
+0000c0d0: 2e43 6c69 656e 7428 2920 6173 2063 6c69  .Client() as cli
+0000c0e0: 656e 743a 0d0a 2020 2020 2020 2020 2020  ent:..          
+0000c0f0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+0000c100: 2063 6c69 656e 742e 6765 7428 7572 6c2b   client.get(url+
+0000c110: 7061 7261 6d73 2c20 6865 6164 6572 733d  params, headers=
+0000c120: 6865 6164 6572 732c 2074 696d 656f 7574  headers, timeout
+0000c130: 3d73 656c 662e 7469 6d65 6f75 7429 0d0a  =self.timeout)..
+0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c150: 6966 2072 6573 706f 6e73 652e 7374 6174  if response.stat
+0000c160: 7573 5f63 6f64 6520 3d3d 2032 3030 3a0d  us_code == 200:.
+0000c170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c180: 2020 2020 2072 6573 706f 6e73 655f 6a73       response_js
+0000c190: 6f6e 203d 2072 6573 706f 6e73 652e 6a73  on = response.js
+0000c1a0: 6f6e 2829 5b30 5d0d 0a20 2020 2020 2020  on()[0]..       
+0000c1b0: 2020 2020 2020 2020 2020 2020 206c 656e               len
+0000c1c0: 6774 6820 3d20 6c65 6e28 7265 7370 6f6e  gth = len(respon
+0000c1d0: 7365 5f6a 736f 6e29 0d0a 2020 2020 2020  se_json)..      
+0000c1e0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+0000c1f0: 616e 736c 6174 696f 6e20 3d20 2222 0d0a  anslation = ""..
+0000c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c210: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+0000c220: 6765 286c 656e 6774 6829 3a0d 0a20 2020  ge(length):..   
+0000c230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c240: 2020 2020 2074 7261 6e73 6c61 7469 6f6e       translation
+0000c250: 203d 2074 7261 6e73 6c61 7469 6f6e 202b   = translation +
+0000c260: 2072 6573 706f 6e73 655f 6a73 6f6e 5b69   response_json[i
+0000c270: 5d5b 305d 0d0a 2020 2020 2020 2020 2020  ][0]..          
+0000c280: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000c290: 2074 7261 6e73 6c61 7469 6f6e 0d0a 2020   translation..  
+0000c2a0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000c2b0: 7475 726e 0d0a 0d0a 2020 2020 2020 2020  turn....        
+0000c2c0: 6578 6365 7074 204b 6579 626f 6172 6449  except KeyboardI
+0000c2d0: 6e74 6572 7275 7074 3a0d 0a20 2020 2020  nterrupt:..     
+0000c2e0: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
+0000c2f0: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+0000c300: 6c6c 6261 636b 3a0d 0a20 2020 2020 2020  llback:..       
+0000c310: 2020 2020 2020 2020 2073 656c 662e 6572           self.er
+0000c320: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+0000c330: 6c62 6163 6b28 2243 616e 6365 6c6c 696e  lback("Cancellin
+0000c340: 6720 616c 6c20 7461 736b 7322 290d 0a20  g all tasks").. 
+0000c350: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000c360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c370: 2020 7072 696e 7428 2243 616e 6365 6c6c    print("Cancell
+0000c380: 696e 6720 616c 6c20 7461 736b 7322 290d  ing all tasks").
+0000c390: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000c3a0: 7572 6e0d 0a0d 0a20 2020 2020 2020 2065  urn....        e
+0000c3b0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+0000c3c0: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
+0000c3d0: 2020 2069 6620 7365 6c66 2e65 7272 6f72     if self.error
+0000c3e0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000c3f0: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
+0000c400: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
+0000c410: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+0000c420: 6b28 6529 0d0a 2020 2020 2020 2020 2020  k(e)..          
+0000c430: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0000c440: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
+0000c450: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+0000c460: 6574 7572 6e0d 0a0d 0a0d 0a63 6c61 7373  eturn......class
+0000c470: 2053 7562 7469 746c 6546 6f72 6d61 7474   SubtitleFormatt
+0000c480: 6572 3a0d 0a20 2020 2073 7570 706f 7274  er:..    support
+0000c490: 6564 5f66 6f72 6d61 7473 203d 205b 2773  ed_formats = ['s
+0000c4a0: 7274 272c 2027 7674 7427 2c20 276a 736f  rt', 'vtt', 'jso
+0000c4b0: 6e27 2c20 2772 6177 275d 0d0a 0d0a 2020  n', 'raw']....  
+0000c4c0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000c4d0: 656c 662c 2066 6f72 6d61 745f 7479 7065  elf, format_type
+0000c4e0: 2c20 6572 726f 725f 6d65 7373 6167 6573  , error_messages
+0000c4f0: 5f63 616c 6c62 6163 6b3d 4e6f 6e65 293a  _callback=None):
+0000c500: 0d0a 2020 2020 2020 2020 7365 6c66 2e66  ..        self.f
+0000c510: 6f72 6d61 745f 7479 7065 203d 2066 6f72  ormat_type = for
+0000c520: 6d61 745f 7479 7065 2e6c 6f77 6572 2829  mat_type.lower()
+0000c530: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
+0000c540: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+0000c550: 6c6c 6261 636b 203d 2065 7272 6f72 5f6d  llback = error_m
+0000c560: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+0000c570: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0000c580: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
+0000c590: 662c 2073 7562 7469 746c 6573 2c20 7061  f, subtitles, pa
+0000c5a0: 6464 696e 675f 6265 666f 7265 3d30 2c20  dding_before=0, 
+0000c5b0: 7061 6464 696e 675f 6166 7465 723d 3029  padding_after=0)
+0000c5c0: 3a0d 0a20 2020 2020 2020 2074 7279 3a0d  :..        try:.
+0000c5d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000c5e0: 7365 6c66 2e66 6f72 6d61 745f 7479 7065  self.format_type
+0000c5f0: 203d 3d20 2773 7274 273a 0d0a 2020 2020   == 'srt':..    
+0000c600: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c610: 726e 2073 656c 662e 7372 745f 666f 726d  rn self.srt_form
+0000c620: 6174 7465 7228 7375 6274 6974 6c65 732c  atter(subtitles,
+0000c630: 2070 6164 6469 6e67 5f62 6566 6f72 652c   padding_before,
+0000c640: 2070 6164 6469 6e67 5f61 6674 6572 290d   padding_after).
+0000c650: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000c660: 6620 7365 6c66 2e66 6f72 6d61 745f 7479  f self.format_ty
+0000c670: 7065 203d 3d20 2776 7474 273a 0d0a 2020  pe == 'vtt':..  
+0000c680: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000c690: 7475 726e 2073 656c 662e 7674 745f 666f  turn self.vtt_fo
+0000c6a0: 726d 6174 7465 7228 7375 6274 6974 6c65  rmatter(subtitle
+0000c6b0: 732c 2070 6164 6469 6e67 5f62 6566 6f72  s, padding_befor
+0000c6c0: 652c 2070 6164 6469 6e67 5f61 6674 6572  e, padding_after
+0000c6d0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+0000c6e0: 6c69 6620 7365 6c66 2e66 6f72 6d61 745f  lif self.format_
+0000c6f0: 7479 7065 203d 3d20 276a 736f 6e27 3a0d  type == 'json':.
+0000c700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c710: 2072 6574 7572 6e20 7365 6c66 2e6a 736f   return self.jso
+0000c720: 6e5f 666f 726d 6174 7465 7228 7375 6274  n_formatter(subt
+0000c730: 6974 6c65 7329 0d0a 2020 2020 2020 2020  itles)..        
+0000c740: 2020 2020 656c 6966 2073 656c 662e 666f      elif self.fo
+0000c750: 726d 6174 5f74 7970 6520 3d3d 2027 7261  rmat_type == 'ra
+0000c760: 7727 3a0d 0a20 2020 2020 2020 2020 2020  w':..           
+0000c770: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000c780: 2e72 6177 5f66 6f72 6d61 7474 6572 2873  .raw_formatter(s
+0000c790: 7562 7469 746c 6573 290d 0a20 2020 2020  ubtitles)..     
+0000c7a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0000c7b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000c7c0: 2065 7272 6f72 5f6d 6573 7361 6765 735f   error_messages_
+0000c7d0: 6361 6c6c 6261 636b 3a0d 0a20 2020 2020  callback:..     
+0000c7e0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000c7f0: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+0000c800: 6c6c 6261 636b 2866 2755 6e73 7570 706f  llback(f'Unsuppo
+0000c810: 7274 6564 2066 6f72 6d61 7420 7479 7065  rted format type
+0000c820: 3a20 7b73 656c 662e 666f 726d 6174 5f74  : {self.format_t
+0000c830: 7970 657d 2729 0d0a 2020 2020 2020 2020  ype}')..        
+0000c840: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c860: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0000c870: 726f 7228 6627 556e 7375 7070 6f72 7465  ror(f'Unsupporte
+0000c880: 6420 666f 726d 6174 2074 7970 653a 207b  d format type: {
+0000c890: 7365 6c66 2e66 6f72 6d61 745f 7479 7065  self.format_type
+0000c8a0: 7d27 290d 0a0d 0a20 2020 2020 2020 2065  }')....        e
+0000c8b0: 7863 6570 7420 4b65 7962 6f61 7264 496e  xcept KeyboardIn
+0000c8c0: 7465 7272 7570 743a 0d0a 2020 2020 2020  terrupt:..      
+0000c8d0: 2020 2020 2020 6966 2073 656c 662e 6572        if self.er
+0000c8e0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+0000c8f0: 6c62 6163 6b3a 0d0a 2020 2020 2020 2020  lback:..        
+0000c900: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
+0000c910: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000c920: 6261 636b 2822 4361 6e63 656c 6c69 6e67  back("Cancelling
+0000c930: 2061 6c6c 2074 6173 6b73 2229 0d0a 2020   all tasks")..  
+0000c940: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+0000c950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c960: 2070 7269 6e74 2822 4361 6e63 656c 6c69   print("Cancelli
+0000c970: 6e67 2061 6c6c 2074 6173 6b73 2229 0d0a  ng all tasks")..
+0000c980: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c990: 726e 0d0a 0d0a 2020 2020 2020 2020 6578  rn....        ex
+0000c9a0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+0000c9b0: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
+0000c9c0: 2020 6966 2073 656c 662e 6572 726f 725f    if self.error_
+0000c9d0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+0000c9e0: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
+0000c9f0: 2020 2020 7365 6c66 2e65 7272 6f72 5f6d      self.error_m
+0000ca00: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+0000ca10: 2865 290d 0a20 2020 2020 2020 2020 2020  (e)..           
+0000ca20: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0000ca30: 2020 2020 2020 2020 7072 696e 7428 6529          print(e)
+0000ca40: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000ca50: 7475 726e 0d0a 0d0a 2020 2020 6465 6620  turn....    def 
+0000ca60: 7372 745f 666f 726d 6174 7465 7228 7365  srt_formatter(se
+0000ca70: 6c66 2c20 7375 6274 6974 6c65 732c 2070  lf, subtitles, p
+0000ca80: 6164 6469 6e67 5f62 6566 6f72 653d 302c  adding_before=0,
+0000ca90: 2070 6164 6469 6e67 5f61 6674 6572 3d30   padding_after=0
+0000caa0: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
+0000cab0: 0a20 2020 2020 2020 2053 6572 6961 6c69  .        Seriali
+0000cac0: 7a65 2061 206c 6973 7420 6f66 2073 7562  ze a list of sub
+0000cad0: 7469 746c 6573 2061 6363 6f72 6469 6e67  titles according
+0000cae0: 2074 6f20 7468 6520 5352 5420 666f 726d   to the SRT form
+0000caf0: 6174 2c20 7769 7468 206f 7074 696f 6e61  at, with optiona
+0000cb00: 6c20 7469 6d65 2070 6164 6469 6e67 2e0d  l time padding..
+0000cb10: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0000cb20: 2020 2020 2020 7375 625f 7269 705f 6669        sub_rip_fi
+0000cb30: 6c65 203d 2070 7973 7274 2e53 7562 5269  le = pysrt.SubRi
+0000cb40: 7046 696c 6528 290d 0a20 2020 2020 2020  pFile()..       
+0000cb50: 2066 6f72 2069 2c20 2828 7374 6172 742c   for i, ((start,
+0000cb60: 2065 6e64 292c 2074 6578 7429 2069 6e20   end), text) in 
+0000cb70: 656e 756d 6572 6174 6528 7375 6274 6974  enumerate(subtit
+0000cb80: 6c65 732c 2073 7461 7274 3d31 293a 0d0a  les, start=1):..
+0000cb90: 2020 2020 2020 2020 2020 2020 6974 656d              item
+0000cba0: 203d 2070 7973 7274 2e53 7562 5269 7049   = pysrt.SubRipI
+0000cbb0: 7465 6d28 290d 0a20 2020 2020 2020 2020  tem()..         
+0000cbc0: 2020 2069 7465 6d2e 696e 6465 7820 3d20     item.index = 
+0000cbd0: 690d 0a20 2020 2020 2020 2020 2020 2069  i..            i
+0000cbe0: 7465 6d2e 7465 7874 203d 2073 6978 2e74  tem.text = six.t
+0000cbf0: 6578 745f 7479 7065 2874 6578 7429 0d0a  ext_type(text)..
+0000cc00: 2020 2020 2020 2020 2020 2020 6974 656d              item
+0000cc10: 2e73 7461 7274 2e73 6563 6f6e 6473 203d  .start.seconds =
+0000cc20: 206d 6178 2830 2c20 7374 6172 7420 2d20   max(0, start - 
+0000cc30: 7061 6464 696e 675f 6265 666f 7265 290d  padding_before).
+0000cc40: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
+0000cc50: 6d2e 656e 642e 7365 636f 6e64 7320 3d20  m.end.seconds = 
+0000cc60: 656e 6420 2b20 7061 6464 696e 675f 6166  end + padding_af
+0000cc70: 7465 720d 0a20 2020 2020 2020 2020 2020  ter..           
+0000cc80: 2073 7562 5f72 6970 5f66 696c 652e 6170   sub_rip_file.ap
+0000cc90: 7065 6e64 2869 7465 6d29 0d0a 2020 2020  pend(item)..    
+0000cca0: 2020 2020 7265 7475 726e 2027 5c6e 272e      return '\n'.
+0000ccb0: 6a6f 696e 2873 6978 2e74 6578 745f 7479  join(six.text_ty
+0000ccc0: 7065 2869 7465 6d29 2066 6f72 2069 7465  pe(item) for ite
+0000ccd0: 6d20 696e 2073 7562 5f72 6970 5f66 696c  m in sub_rip_fil
+0000cce0: 6529 0d0a 0d0a 2020 2020 6465 6620 7674  e)....    def vt
+0000ccf0: 745f 666f 726d 6174 7465 7228 7365 6c66  t_formatter(self
+0000cd00: 2c20 7375 6274 6974 6c65 732c 2070 6164  , subtitles, pad
+0000cd10: 6469 6e67 5f62 6566 6f72 653d 302c 2070  ding_before=0, p
+0000cd20: 6164 6469 6e67 5f61 6674 6572 3d30 293a  adding_after=0):
+0000cd30: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0000cd40: 2020 2020 2020 2053 6572 6961 6c69 7a65         Serialize
+0000cd50: 2061 206c 6973 7420 6f66 2073 7562 7469   a list of subti
+0000cd60: 746c 6573 2061 6363 6f72 6469 6e67 2074  tles according t
+0000cd70: 6f20 7468 6520 5654 5420 666f 726d 6174  o the VTT format
+0000cd80: 2c20 7769 7468 206f 7074 696f 6e61 6c20  , with optional 
+0000cd90: 7469 6d65 2070 6164 6469 6e67 2e0d 0a20  time padding... 
+0000cda0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+0000cdb0: 2020 2020 7465 7874 203d 2073 656c 662e      text = self.
+0000cdc0: 7372 745f 666f 726d 6174 7465 7228 7375  srt_formatter(su
+0000cdd0: 6274 6974 6c65 732c 2070 6164 6469 6e67  btitles, padding
+0000cde0: 5f62 6566 6f72 652c 2070 6164 6469 6e67  _before, padding
+0000cdf0: 5f61 6674 6572 290d 0a20 2020 2020 2020  _after)..       
+0000ce00: 2074 6578 7420 3d20 2757 4542 5654 545c   text = 'WEBVTT\
+0000ce10: 6e5c 6e27 202b 2074 6578 742e 7265 706c  n\n' + text.repl
+0000ce20: 6163 6528 272c 272c 2027 2e27 290d 0a20  ace(',', '.').. 
+0000ce30: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
+0000ce40: 7874 0d0a 0d0a 2020 2020 6465 6620 6a73  xt....    def js
+0000ce50: 6f6e 5f66 6f72 6d61 7474 6572 2873 656c  on_formatter(sel
+0000ce60: 662c 2073 7562 7469 746c 6573 293a 0d0a  f, subtitles):..
+0000ce70: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+0000ce80: 2020 2020 2053 6572 6961 6c69 7a65 2061       Serialize a
+0000ce90: 206c 6973 7420 6f66 2073 7562 7469 746c   list of subtitl
+0000cea0: 6573 2061 7320 6120 4a53 4f4e 2062 6c6f  es as a JSON blo
+0000ceb0: 622e 0d0a 2020 2020 2020 2020 2222 220d  b...        """.
+0000cec0: 0a20 2020 2020 2020 2073 7562 7469 746c  .        subtitl
+0000ced0: 655f 6469 6374 7320 3d20 5b0d 0a20 2020  e_dicts = [..   
+0000cee0: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
+0000cef0: 2020 2020 2020 2020 2020 2020 2773 7461              'sta
+0000cf00: 7274 273a 2073 7461 7274 2c0d 0a20 2020  rt': start,..   
+0000cf10: 2020 2020 2020 2020 2020 2020 2027 656e               'en
+0000cf20: 6427 3a20 656e 642c 0d0a 2020 2020 2020  d': end,..      
+0000cf30: 2020 2020 2020 2020 2020 2763 6f6e 7465            'conte
+0000cf40: 6e74 273a 2074 6578 742c 0d0a 2020 2020  nt': text,..    
+0000cf50: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
+0000cf60: 2020 2020 2020 2066 6f72 2028 2873 7461         for ((sta
+0000cf70: 7274 2c20 656e 6429 2c20 7465 7874 290d  rt, end), text).
+0000cf80: 0a20 2020 2020 2020 2020 2020 2069 6e20  .            in 
+0000cf90: 7375 6274 6974 6c65 730d 0a20 2020 2020  subtitles..     
+0000cfa0: 2020 205d 0d0a 2020 2020 2020 2020 7265     ]..        re
+0000cfb0: 7475 726e 206a 736f 6e2e 6475 6d70 7328  turn json.dumps(
+0000cfc0: 7375 6274 6974 6c65 5f64 6963 7473 290d  subtitle_dicts).
+0000cfd0: 0a0d 0a20 2020 2064 6566 2072 6177 5f66  ...    def raw_f
+0000cfe0: 6f72 6d61 7474 6572 2873 656c 662c 2073  ormatter(self, s
+0000cff0: 7562 7469 746c 6573 293a 0d0a 2020 2020  ubtitles):..    
+0000d000: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0000d010: 2053 6572 6961 6c69 7a65 2061 206c 6973   Serialize a lis
+0000d020: 7420 6f66 2073 7562 7469 746c 6573 2061  t of subtitles a
+0000d030: 7320 6120 6e65 776c 696e 652d 6465 6c69  s a newline-deli
+0000d040: 6d69 7465 6420 7374 7269 6e67 2e0d 0a20  mited string... 
+0000d050: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+0000d060: 2020 2020 7265 7475 726e 2027 2027 2e6a      return ' '.j
+0000d070: 6f69 6e28 7465 7874 2066 6f72 2028 5f72  oin(text for (_r
+0000d080: 6e67 2c20 7465 7874 2920 696e 2073 7562  ng, text) in sub
+0000d090: 7469 746c 6573 290d 0a0d 0a0d 0a63 6c61  titles)......cla
+0000d0a0: 7373 2053 7562 7469 746c 6557 7269 7465  ss SubtitleWrite
+0000d0b0: 723a 0d0a 2020 2020 6465 6620 5f5f 696e  r:..    def __in
+0000d0c0: 6974 5f5f 2873 656c 662c 2072 6567 696f  it__(self, regio
+0000d0d0: 6e73 2c20 7472 616e 7363 7269 7074 732c  ns, transcripts,
+0000d0e0: 2066 6f72 6d61 742c 2065 7272 6f72 5f6d   format, error_m
+0000d0f0: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+0000d100: 3d4e 6f6e 6529 3a0d 0a20 2020 2020 2020  =None):..       
+0000d110: 2073 656c 662e 7265 6769 6f6e 7320 3d20   self.regions = 
+0000d120: 7265 6769 6f6e 730d 0a20 2020 2020 2020  regions..       
+0000d130: 2073 656c 662e 7472 616e 7363 7269 7074   self.transcript
+0000d140: 7320 3d20 7472 616e 7363 7269 7074 730d  s = transcripts.
+0000d150: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
+0000d160: 726d 6174 203d 2066 6f72 6d61 740d 0a20  rmat = format.. 
+0000d170: 2020 2020 2020 2073 656c 662e 7469 6d65         self.time
+0000d180: 645f 7375 6274 6974 6c65 7320 3d20 5b28  d_subtitles = [(
+0000d190: 722c 2074 2920 666f 7220 722c 2074 2069  r, t) for r, t i
+0000d1a0: 6e20 7a69 7028 7365 6c66 2e72 6567 696f  n zip(self.regio
+0000d1b0: 6e73 2c20 7365 6c66 2e74 7261 6e73 6372  ns, self.transcr
+0000d1c0: 6970 7473 2920 6966 2074 5d0d 0a20 2020  ipts) if t]..   
+0000d1d0: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
+0000d1e0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+0000d1f0: 6b20 3d20 6572 726f 725f 6d65 7373 6167  k = error_messag
+0000d200: 6573 5f63 616c 6c62 6163 6b0d 0a0d 0a20  es_callback.... 
+0000d210: 2020 2064 6566 2067 6574 5f74 696d 6564     def get_timed
+0000d220: 5f73 7562 7469 746c 6573 2873 656c 6629  _subtitles(self)
+0000d230: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+0000d240: 6e20 7365 6c66 2e74 696d 6564 5f73 7562  n self.timed_sub
+0000d250: 7469 746c 6573 0d0a 0d0a 2020 2020 6465  titles....    de
+0000d260: 6620 7772 6974 6528 7365 6c66 2c20 6465  f write(self, de
+0000d270: 636c 6172 6564 5f73 7562 7469 746c 655f  clared_subtitle_
+0000d280: 6669 6c65 7061 7468 293a 0d0a 2020 2020  filepath):..    
+0000d290: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+0000d2a0: 2020 2020 2020 666f 726d 6174 7465 7220        formatter 
+0000d2b0: 3d20 5375 6274 6974 6c65 466f 726d 6174  = SubtitleFormat
+0000d2c0: 7465 7228 7365 6c66 2e66 6f72 6d61 7429  ter(self.format)
+0000d2d0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+0000d2e0: 726d 6174 7465 645f 7375 6274 6974 6c65  rmatted_subtitle
+0000d2f0: 7320 3d20 666f 726d 6174 7465 7228 7365  s = formatter(se
+0000d300: 6c66 2e74 696d 6564 5f73 7562 7469 746c  lf.timed_subtitl
+0000d310: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
+0000d320: 2073 6176 6564 5f73 7562 7469 746c 655f   saved_subtitle_
+0000d330: 6669 6c65 7061 7468 203d 2064 6563 6c61  filepath = decla
+0000d340: 7265 645f 7375 6274 6974 6c65 5f66 696c  red_subtitle_fil
+0000d350: 6570 6174 680d 0a20 2020 2020 2020 2020  epath..         
+0000d360: 2020 2069 6620 7361 7665 645f 7375 6274     if saved_subt
+0000d370: 6974 6c65 5f66 696c 6570 6174 683a 0d0a  itle_filepath:..
+0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d390: 7375 6274 6974 6c65 5f66 696c 655f 6261  subtitle_file_ba
+0000d3a0: 7365 2c20 7375 6274 6974 6c65 5f66 696c  se, subtitle_fil
+0000d3b0: 655f 6578 7420 3d20 6f73 2e70 6174 682e  e_ext = os.path.
+0000d3c0: 7370 6c69 7465 7874 2873 6176 6564 5f73  splitext(saved_s
+0000d3d0: 7562 7469 746c 655f 6669 6c65 7061 7468  ubtitle_filepath
+0000d3e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000d3f0: 2020 2069 6620 6e6f 7420 7375 6274 6974     if not subtit
+0000d400: 6c65 5f66 696c 655f 6578 743a 0d0a 2020  le_file_ext:..  
+0000d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d420: 2020 7361 7665 645f 7375 6274 6974 6c65    saved_subtitle
+0000d430: 5f66 696c 6570 6174 6820 3d20 227b 6261  _filepath = "{ba
+0000d440: 7365 7d2e 7b66 6f72 6d61 747d 222e 666f  se}.{format}".fo
+0000d450: 726d 6174 2862 6173 653d 7375 6274 6974  rmat(base=subtit
+0000d460: 6c65 5f66 696c 655f 6261 7365 2c20 666f  le_file_base, fo
+0000d470: 726d 6174 3d73 656c 662e 666f 726d 6174  rmat=self.format
+0000d480: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000d490: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0000d4a0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+0000d4b0: 7665 645f 7375 6274 6974 6c65 5f66 696c  ved_subtitle_fil
+0000d4c0: 6570 6174 6820 3d20 6465 636c 6172 6564  epath = declared
+0000d4d0: 5f73 7562 7469 746c 655f 6669 6c65 7061  _subtitle_filepa
+0000d4e0: 7468 0d0a 2020 2020 2020 2020 2020 2020  th..            
+0000d4f0: 7769 7468 206f 7065 6e28 7361 7665 645f  with open(saved_
+0000d500: 7375 6274 6974 6c65 5f66 696c 6570 6174  subtitle_filepat
+0000d510: 682c 2027 7762 2729 2061 7320 663a 0d0a  h, 'wb') as f:..
+0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d530: 662e 7772 6974 6528 666f 726d 6174 7465  f.write(formatte
+0000d540: 645f 7375 6274 6974 6c65 732e 656e 636f  d_subtitles.enco
+0000d550: 6465 2822 7574 662d 3822 2929 0d0a 2020  de("utf-8"))..  
+0000d560: 2020 2020 2020 2020 2020 2377 6974 6820            #with 
+0000d570: 6f70 656e 2873 6176 6564 5f73 7562 7469  open(saved_subti
+0000d580: 746c 655f 6669 6c65 7061 7468 2c20 2761  tle_filepath, 'a
+0000d590: 2729 2061 7320 663a 0d0a 2020 2020 2020  ') as f:..      
+0000d5a0: 2020 2020 2020 2320 2020 2066 2e77 7269        #    f.wri
+0000d5b0: 7465 2822 5c6e 2229 0d0a 0d0a 2020 2020  te("\n")....    
+0000d5c0: 2020 2020 6578 6365 7074 204b 6579 626f      except Keybo
+0000d5d0: 6172 6449 6e74 6572 7275 7074 3a0d 0a20  ardInterrupt:.. 
+0000d5e0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000d5f0: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
+0000d600: 735f 6361 6c6c 6261 636b 3a0d 0a20 2020  s_callback:..   
+0000d610: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000d620: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
+0000d630: 5f63 616c 6c62 6163 6b28 2243 616e 6365  _callback("Cance
+0000d640: 6c6c 696e 6720 616c 6c20 7461 736b 7322  lling all tasks"
+0000d650: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+0000d660: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0000d670: 2020 2020 2020 7072 696e 7428 2243 616e        print("Can
+0000d680: 6365 6c6c 696e 6720 616c 6c20 7461 736b  celling all task
+0000d690: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
+0000d6a0: 2072 6574 7572 6e0d 0a0d 0a20 2020 2020   return....     
+0000d6b0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+0000d6c0: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
+0000d6d0: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
+0000d6e0: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+0000d6f0: 6c6c 6261 636b 3a0d 0a20 2020 2020 2020  llback:..       
+0000d700: 2020 2020 2020 2020 2073 656c 662e 6572           self.er
+0000d710: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+0000d720: 6c62 6163 6b28 6529 0d0a 2020 2020 2020  lback(e)..      
+0000d730: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0000d740: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+0000d750: 6e74 2865 290d 0a20 2020 2020 2020 2020  nt(e)..         
+0000d760: 2020 2072 6574 7572 6e0d 0a0d 0a0d 0a63     return......c
+0000d770: 6c61 7373 2053 5254 4669 6c65 5265 6164  lass SRTFileRead
+0000d780: 6572 3a0d 0a20 2020 2064 6566 205f 5f69  er:..    def __i
+0000d790: 6e69 745f 5f28 7365 6c66 2c20 7372 745f  nit__(self, srt_
+0000d7a0: 6669 6c65 5f70 6174 682c 2065 7272 6f72  file_path, error
+0000d7b0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000d7c0: 636b 3d4e 6f6e 6529 3a0d 0a20 2020 2020  ck=None):..     
+0000d7d0: 2020 2073 656c 662e 7469 6d65 645f 7375     self.timed_su
+0000d7e0: 6274 6974 6c65 7320 3d20 7365 6c66 2873  btitles = self(s
+0000d7f0: 7274 5f66 696c 655f 7061 7468 290d 0a20  rt_file_path).. 
+0000d800: 2020 2020 2020 2073 656c 662e 6572 726f         self.erro
+0000d810: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000d820: 6163 6b20 3d20 6572 726f 725f 6d65 7373  ack = error_mess
+0000d830: 6167 6573 5f63 616c 6c62 6163 6b0d 0a0d  ages_callback...
+0000d840: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+0000d850: 6f64 0d0a 2020 2020 6465 6620 5f5f 6361  od..    def __ca
+0000d860: 6c6c 5f5f 2873 7274 5f66 696c 655f 7061  ll__(srt_file_pa
+0000d870: 7468 293a 0d0a 2020 2020 2020 2020 7472  th):..        tr
+0000d880: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+0000d890: 2222 220d 0a20 2020 2020 2020 2020 2020  """..           
+0000d8a0: 2052 6561 6420 5352 5420 666f 726d 6174   Read SRT format
+0000d8b0: 7465 6420 7375 6274 6974 6c65 2066 696c  ted subtitle fil
+0000d8c0: 6520 616e 6420 7265 7475 726e 2073 7562  e and return sub
+0000d8d0: 7469 746c 6573 2061 7320 6c69 7374 206f  titles as list o
+0000d8e0: 6620 7475 706c 6573 0d0a 2020 2020 2020  f tuples..      
+0000d8f0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0000d900: 2020 2020 2020 2074 696d 6564 5f73 7562         timed_sub
+0000d910: 7469 746c 6573 203d 205b 5d0d 0a20 2020  titles = []..   
+0000d920: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
+0000d930: 656e 2873 7274 5f66 696c 655f 7061 7468  en(srt_file_path
+0000d940: 2c20 2772 2729 2061 7320 7372 745f 6669  , 'r') as srt_fi
+0000d950: 6c65 3a0d 0a20 2020 2020 2020 2020 2020  le:..           
+0000d960: 2020 2020 206c 696e 6573 203d 2073 7274       lines = srt
+0000d970: 5f66 696c 652e 7265 6164 6c69 6e65 7328  _file.readlines(
+0000d980: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000d990: 2020 2023 2053 706c 6974 2074 6865 2073     # Split the s
+0000d9a0: 7562 7469 746c 6520 6669 6c65 2069 6e74  ubtitle file int
+0000d9b0: 6f20 7375 6274 6974 6c65 2062 6c6f 636b  o subtitle block
+0000d9c0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+0000d9d0: 2020 2073 7562 7469 746c 655f 626c 6f63     subtitle_bloc
+0000d9e0: 6b73 203d 205b 5d0d 0a20 2020 2020 2020  ks = []..       
+0000d9f0: 2020 2020 2020 2020 2062 6c6f 636b 203d           block =
+0000da00: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+0000da10: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
+0000da20: 206c 696e 6573 3a0d 0a20 2020 2020 2020   lines:..       
+0000da30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000da40: 6c69 6e65 2e73 7472 6970 2829 203d 3d20  line.strip() == 
+0000da50: 2727 3a0d 0a20 2020 2020 2020 2020 2020  '':..           
+0000da60: 2020 2020 2020 2020 2020 2020 2073 7562               sub
+0000da70: 7469 746c 655f 626c 6f63 6b73 2e61 7070  title_blocks.app
+0000da80: 656e 6428 626c 6f63 6b29 0d0a 2020 2020  end(block)..    
+0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000daa0: 2020 2020 626c 6f63 6b20 3d20 5b5d 0d0a      block = []..
+0000dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dac0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dae0: 2020 2062 6c6f 636b 2e61 7070 656e 6428     block.append(
+0000daf0: 6c69 6e65 2e73 7472 6970 2829 290d 0a20  line.strip()).. 
+0000db00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000db10: 7562 7469 746c 655f 626c 6f63 6b73 2e61  ubtitle_blocks.a
+0000db20: 7070 656e 6428 626c 6f63 6b29 0d0a 0d0a  ppend(block)....
+0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db40: 2320 5061 7273 6520 6561 6368 2073 7562  # Parse each sub
+0000db50: 7469 746c 6520 626c 6f63 6b20 616e 6420  title block and 
+0000db60: 7374 6f72 6520 6173 2074 7570 6c65 2069  store as tuple i
+0000db70: 6e20 7469 6d65 645f 7375 6274 6974 6c65  n timed_subtitle
+0000db80: 7320 6c69 7374 0d0a 2020 2020 2020 2020  s list..        
+0000db90: 2020 2020 2020 2020 666f 7220 626c 6f63          for bloc
+0000dba0: 6b20 696e 2073 7562 7469 746c 655f 626c  k in subtitle_bl
+0000dbb0: 6f63 6b73 3a0d 0a20 2020 2020 2020 2020  ocks:..         
+0000dbc0: 2020 2020 2020 2020 2020 2069 6620 626c             if bl
+0000dbd0: 6f63 6b3a 0d0a 2020 2020 2020 2020 2020  ock:..          
+0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000dbf0: 4578 7472 6163 7420 7374 6172 7420 616e  Extract start an
+0000dc00: 6420 656e 6420 7469 6d65 7320 6672 6f6d  d end times from
+0000dc10: 2073 7562 7469 746c 6520 626c 6f63 6b0d   subtitle block.
+0000dc20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dc30: 2020 2020 2020 2020 2073 7461 7274 5f74           start_t
+0000dc40: 696d 655f 7374 722c 2065 6e64 5f74 696d  ime_str, end_tim
+0000dc50: 655f 7374 7220 3d20 626c 6f63 6b5b 315d  e_str = block[1]
+0000dc60: 2e73 706c 6974 2827 202d 2d3e 2027 290d  .split(' --> ').
+0000dc70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dc80: 2020 2020 2020 2020 2074 696d 655f 666f           time_fo
+0000dc90: 726d 6174 203d 2027 2548 3a25 4d3a 2553  rmat = '%H:%M:%S
+0000dca0: 2c25 6627 0d0a 2020 2020 2020 2020 2020  ,%f'..          
+0000dcb0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000dcc0: 6172 745f 7469 6d65 5f74 696d 655f 6465  art_time_time_de
+0000dcd0: 6c74 6120 3d20 6461 7465 7469 6d65 2e73  lta = datetime.s
+0000dce0: 7472 7074 696d 6528 7374 6172 745f 7469  trptime(start_ti
+0000dcf0: 6d65 5f73 7472 2c20 7469 6d65 5f66 6f72  me_str, time_for
+0000dd00: 6d61 7429 202d 2064 6174 6574 696d 652e  mat) - datetime.
+0000dd10: 7374 7270 7469 6d65 2827 3030 3a30 303a  strptime('00:00:
+0000dd20: 3030 2c30 3030 272c 2074 696d 655f 666f  00,000', time_fo
+0000dd30: 726d 6174 290d 0a20 2020 2020 2020 2020  rmat)..         
+0000dd40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000dd50: 7461 7274 5f74 696d 655f 746f 7461 6c5f  tart_time_total_
+0000dd60: 7365 636f 6e64 7320 3d20 7374 6172 745f  seconds = start_
+0000dd70: 7469 6d65 5f74 696d 655f 6465 6c74 612e  time_time_delta.
+0000dd80: 746f 7461 6c5f 7365 636f 6e64 7328 290d  total_seconds().
+0000dd90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dda0: 2020 2020 2020 2020 2065 6e64 5f74 696d           end_tim
+0000ddb0: 655f 7469 6d65 5f64 656c 7461 203d 2064  e_time_delta = d
+0000ddc0: 6174 6574 696d 652e 7374 7270 7469 6d65  atetime.strptime
+0000ddd0: 2865 6e64 5f74 696d 655f 7374 722c 2074  (end_time_str, t
+0000dde0: 696d 655f 666f 726d 6174 2920 2d20 6461  ime_format) - da
+0000ddf0: 7465 7469 6d65 2e73 7472 7074 696d 6528  tetime.strptime(
+0000de00: 2730 303a 3030 3a30 302c 3030 3027 2c20  '00:00:00,000', 
+0000de10: 7469 6d65 5f66 6f72 6d61 7429 0d0a 2020  time_format)..  
+0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de30: 2020 2020 2020 656e 645f 7469 6d65 5f74        end_time_t
+0000de40: 6f74 616c 5f73 6563 6f6e 6473 203d 2065  otal_seconds = e
+0000de50: 6e64 5f74 696d 655f 7469 6d65 5f64 656c  nd_time_time_del
+0000de60: 7461 2e74 6f74 616c 5f73 6563 6f6e 6473  ta.total_seconds
+0000de70: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+0000de80: 2020 2020 2020 2020 2020 2020 2320 4578              # Ex
+0000de90: 7472 6163 7420 7375 6274 6974 6c65 2074  tract subtitle t
+0000dea0: 6578 7420 6672 6f6d 2073 7562 7469 746c  ext from subtitl
+0000deb0: 6520 626c 6f63 6b0d 0a20 2020 2020 2020  e block..       
+0000dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ded0: 2073 7562 7469 746c 6520 3d20 2720 272e   subtitle = ' '.
+0000dee0: 6a6f 696e 2862 6c6f 636b 5b32 3a5d 290d  join(block[2:]).
+0000def0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000df00: 2020 2020 2020 2020 2074 696d 6564 5f73           timed_s
+0000df10: 7562 7469 746c 6573 2e61 7070 656e 6428  ubtitles.append(
+0000df20: 2828 7374 6172 745f 7469 6d65 5f74 6f74  ((start_time_tot
+0000df30: 616c 5f73 6563 6f6e 6473 2c20 656e 645f  al_seconds, end_
+0000df40: 7469 6d65 5f74 6f74 616c 5f73 6563 6f6e  time_total_secon
+0000df50: 6473 292c 2073 7562 7469 746c 6529 290d  ds), subtitle)).
+0000df60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000df70: 2072 6574 7572 6e20 7469 6d65 645f 7375   return timed_su
+0000df80: 6274 6974 6c65 730d 0a0d 0a20 2020 2020  btitles....     
+0000df90: 2020 2065 7863 6570 7420 4b65 7962 6f61     except Keyboa
+0000dfa0: 7264 496e 7465 7272 7570 743a 0d0a 2020  rdInterrupt:..  
+0000dfb0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000dfc0: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
+0000dfd0: 5f63 616c 6c62 6163 6b3a 0d0a 2020 2020  _callback:..    
+0000dfe0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000dff0: 2e65 7272 6f72 5f6d 6573 7361 6765 735f  .error_messages_
+0000e000: 6361 6c6c 6261 636b 2822 4361 6e63 656c  callback("Cancel
+0000e010: 6c69 6e67 2061 6c6c 2074 6173 6b73 2229  ling all tasks")
+0000e020: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+0000e030: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000e040: 2020 2020 2070 7269 6e74 2822 4361 6e63       print("Canc
+0000e050: 656c 6c69 6e67 2061 6c6c 2074 6173 6b73  elling all tasks
+0000e060: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000e070: 7265 7475 726e 0d0a 0d0a 2020 2020 2020  return....      
+0000e080: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+0000e090: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
+0000e0a0: 2020 2020 2020 6966 2073 656c 662e 6572        if self.er
+0000e0b0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+0000e0c0: 6c62 6163 6b3a 0d0a 2020 2020 2020 2020  lback:..        
+0000e0d0: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
+0000e0e0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000e0f0: 6261 636b 2865 290d 0a20 2020 2020 2020  back(e)..       
+0000e100: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000e110: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000e120: 7428 6529 0d0a 2020 2020 2020 2020 2020  t(e)..          
+0000e130: 2020 7265 7475 726e 0d0a 0d0a 0d0a 6465    return......de
+0000e140: 6620 7368 6f77 5f70 726f 6772 6573 7328  f show_progress(
+0000e150: 6d65 6469 615f 6669 6c65 7061 7468 2c20  media_filepath, 
+0000e160: 7072 6f67 7265 7373 293a 0d0a 2020 2020  progress):..    
+0000e170: 676c 6f62 616c 2070 6261 720d 0a20 2020  global pbar..   
+0000e180: 2070 6261 722e 7570 6461 7465 2870 726f   pbar.update(pro
+0000e190: 6772 6573 7329 0d0a 0d0a 0d0a 6465 6620  gress)......def 
+0000e1a0: 7368 6f77 5f65 7272 6f72 5f6d 6573 7361  show_error_messa
+0000e1b0: 6765 7328 6d65 7373 6167 6573 293a 0d0a  ges(messages):..
+0000e1c0: 2020 2020 7072 696e 7428 6d65 7373 6167      print(messag
+0000e1d0: 6573 290d 0a0d 0a0d 0a64 6566 206d 6169  es)......def mai
+0000e1e0: 6e28 293a 0d0a 2020 2020 676c 6f62 616c  n():..    global
+0000e1f0: 2070 6261 720d 0a0d 0a20 2020 2069 6620   pbar....    if 
+0000e200: 7379 732e 706c 6174 666f 726d 203d 3d20  sys.platform == 
+0000e210: 2277 696e 3332 223a 0d0a 2020 2020 2020  "win32":..      
+0000e220: 2020 7374 6f70 5f66 666d 7065 675f 7769    stop_ffmpeg_wi
+0000e230: 6e64 6f77 7328 6572 726f 725f 6d65 7373  ndows(error_mess
+0000e240: 6167 6573 5f63 616c 6c62 6163 6b3d 7368  ages_callback=sh
+0000e250: 6f77 5f65 7272 6f72 5f6d 6573 7361 6765  ow_error_message
+0000e260: 7329 0d0a 2020 2020 656c 7365 3a0d 0a20  s)..    else:.. 
+0000e270: 2020 2020 2020 2073 746f 705f 6666 6d70         stop_ffmp
+0000e280: 6567 5f6c 696e 7578 2865 7272 6f72 5f6d  eg_linux(error_m
+0000e290: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+0000e2a0: 3d73 686f 775f 6572 726f 725f 6d65 7373  =show_error_mess
+0000e2b0: 6167 6573 290d 0a0d 0a20 2020 2072 656d  ages)....    rem
+0000e2c0: 6f76 655f 7465 6d70 5f66 696c 6573 2822  ove_temp_files("
+0000e2d0: 666c 6163 222c 2065 7272 6f72 5f6d 6573  flac", error_mes
+0000e2e0: 7361 6765 735f 6361 6c6c 6261 636b 3d73  sages_callback=s
+0000e2f0: 686f 775f 6572 726f 725f 6d65 7373 6167  how_error_messag
+0000e300: 6573 290d 0a20 2020 2072 656d 6f76 655f  es)..    remove_
+0000e310: 7465 6d70 5f66 696c 6573 2822 7761 7622  temp_files("wav"
+0000e320: 2c20 6572 726f 725f 6d65 7373 6167 6573  , error_messages
+0000e330: 5f63 616c 6c62 6163 6b3d 7368 6f77 5f65  _callback=show_e
+0000e340: 7272 6f72 5f6d 6573 7361 6765 7329 0d0a  rror_messages)..
+0000e350: 0d0a 2020 2020 7061 7273 6572 203d 2061  ..    parser = a
+0000e360: 7267 7061 7273 652e 4172 6775 6d65 6e74  rgparse.Argument
+0000e370: 5061 7273 6572 2829 0d0a 2020 2020 7061  Parser()..    pa
+0000e380: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+0000e390: 7428 2773 6f75 7263 655f 7061 7468 272c  t('source_path',
+0000e3a0: 2068 656c 703d 2250 6174 6820 746f 2074   help="Path to t
+0000e3b0: 6865 2076 6964 656f 206f 7220 6175 6469  he video or audi
+0000e3c0: 6f20 6669 6c65 7320 746f 2067 656e 6572  o files to gener
+0000e3d0: 6174 6520 7375 6274 6974 6c65 7320 6669  ate subtitles fi
+0000e3e0: 6c65 7320 2875 7365 2077 696c 6463 6172  les (use wildcar
+0000e3f0: 6420 666f 7220 6d75 6c74 6970 6c65 2066  d for multiple f
+0000e400: 696c 6573 206f 7220 7365 7061 7261 7465  iles or separate
+0000e410: 2074 6865 6d20 7769 7468 2061 2073 7061   them with a spa
+0000e420: 6365 2063 6861 7261 6374 6572 2065 2e67  ce character e.g
+0000e430: 2e20 5c22 6669 6c65 2031 2e6d 7034 5c22  . \"file 1.mp4\"
+0000e440: 205c 2266 696c 6520 322e 6d70 345c 2229   \"file 2.mp4\")
+0000e450: 222c 206e 6172 6773 3d27 2a27 290d 0a20  ", nargs='*').. 
+0000e460: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
+0000e470: 6775 6d65 6e74 2827 2d6d 272c 2027 2d2d  gument('-m', '--
+0000e480: 6d6f 6465 6c2d 6e61 6d65 272c 2064 6566  model-name', def
+0000e490: 6175 6c74 3d22 736d 616c 6c22 2c20 6865  ault="small", he
+0000e4a0: 6c70 3d22 6e61 6d65 206f 6620 7468 6520  lp="name of the 
+0000e4b0: 5768 6973 7065 7220 6d6f 6465 6c20 746f  Whisper model to
+0000e4c0: 2075 7365 2229 0d0a 2020 2020 7061 7273   use")..    pars
+0000e4d0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
+0000e4e0: 272d 6c6d 272c 2027 2d2d 6c69 7374 2d6d  '-lm', '--list-m
+0000e4f0: 6f64 656c 7327 2c20 6865 6c70 3d22 4c69  odels', help="Li
+0000e500: 7374 206f 6620 5768 6973 7065 7220 6d6f  st of Whisper mo
+0000e510: 6465 6c73 206e 616d 6522 2c20 6163 7469  dels name", acti
+0000e520: 6f6e 3d27 7374 6f72 655f 7472 7565 2729  on='store_true')
+0000e530: 0d0a 2020 2020 7061 7273 6572 2e61 6464  ..    parser.add
+0000e540: 5f61 7267 756d 656e 7428 272d 5327 2c20  _argument('-S', 
+0000e550: 272d 2d73 7263 2d6c 616e 6775 6167 6527  '--src-language'
+0000e560: 2c20 6865 6c70 3d22 4c61 6e67 7561 6765  , help="Language
+0000e570: 2063 6f64 6520 6f66 2074 6865 2061 7564   code of the aud
+0000e580: 696f 206c 616e 6775 6167 6520 7370 6f6b  io language spok
+0000e590: 656e 2069 6e20 7669 6465 6f2f 6175 6469  en in video/audi
+0000e5a0: 6f20 736f 7572 6365 5f70 6174 6822 2c20  o source_path", 
+0000e5b0: 6465 6661 756c 743d 2265 6e22 290d 0a20  default="en").. 
+0000e5c0: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
+0000e5d0: 6775 6d65 6e74 2827 2d44 272c 2027 2d2d  gument('-D', '--
+0000e5e0: 6473 742d 6c61 6e67 7561 6765 272c 2068  dst-language', h
+0000e5f0: 656c 703d 2244 6573 6972 6564 2074 7261  elp="Desired tra
+0000e600: 6e73 6c61 7469 6f6e 206c 616e 6775 6167  nslation languag
+0000e610: 6520 636f 6465 2066 6f72 2074 6865 2073  e code for the s
+0000e620: 7562 7469 746c 6573 222c 2064 6566 6175  ubtitles", defau
+0000e630: 6c74 3d4e 6f6e 6529 0d0a 2020 2020 7061  lt=None)..    pa
+0000e640: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+0000e650: 7428 272d 6c77 6c27 2c20 272d 2d6c 6973  t('-lwl', '--lis
+0000e660: 742d 7768 6973 7065 722d 6c61 6e67 7561  t-whisper-langua
+0000e670: 6765 7327 2c20 6865 6c70 3d22 4c69 7374  ges', help="List
+0000e680: 2061 6c6c 2077 6869 7370 6572 2073 7570   all whisper sup
+0000e690: 706f 7274 6564 206c 616e 6775 6167 6573  ported languages
+0000e6a0: 222c 2061 6374 696f 6e3d 2773 746f 7265  ", action='store
+0000e6b0: 5f74 7275 6527 290d 0a20 2020 2070 6172  _true')..    par
+0000e6c0: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
+0000e6d0: 2827 2d6c 676c 272c 2027 2d2d 6c69 7374  ('-lgl', '--list
+0000e6e0: 2d67 6f6f 676c 652d 6c61 6e67 7561 6765  -google-language
+0000e6f0: 7327 2c20 6865 6c70 3d22 4c69 7374 2061  s', help="List a
+0000e700: 6c6c 2067 6f6f 676c 6520 7472 616e 736c  ll google transl
+0000e710: 6174 6520 7375 7070 6f72 7465 6420 6c61  ate supported la
+0000e720: 6e67 7561 6765 7322 2c20 6163 7469 6f6e  nguages", action
+0000e730: 3d27 7374 6f72 655f 7472 7565 2729 0d0a  ='store_true')..
+0000e740: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
+0000e750: 7267 756d 656e 7428 272d 4627 2c20 272d  rgument('-F', '-
+0000e760: 2d66 6f72 6d61 7427 2c20 6865 6c70 3d22  -format', help="
+0000e770: 4465 7369 7265 6420 7375 6274 6974 6c65  Desired subtitle
+0000e780: 2066 6f72 6d61 7422 2c20 6465 6661 756c   format", defaul
+0000e790: 743d 2273 7274 2229 0d0a 2020 2020 7061  t="srt")..    pa
+0000e7a0: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+0000e7b0: 7428 272d 6c66 272c 2027 2d2d 6c69 7374  t('-lf', '--list
+0000e7c0: 2d66 6f72 6d61 7473 272c 2068 656c 703d  -formats', help=
+0000e7d0: 224c 6973 7420 616c 6c20 7375 7070 6f72  "List all suppor
+0000e7e0: 7465 6420 7375 6274 6974 6c65 2066 6f72  ted subtitle for
+0000e7f0: 6d61 7473 222c 2061 6374 696f 6e3d 2773  mats", action='s
+0000e800: 746f 7265 5f74 7275 6527 290d 0a20 2020  tore_true')..   
+0000e810: 2070 6172 7365 722e 6164 645f 6172 6775   parser.add_argu
+0000e820: 6d65 6e74 2827 2d43 272c 2027 2d2d 636f  ment('-C', '--co
+0000e830: 6e63 7572 7265 6e63 7927 2c20 6865 6c70  ncurrency', help
+0000e840: 3d22 4e75 6d62 6572 206f 6620 636f 6e63  ="Number of conc
+0000e850: 7572 7265 6e74 2041 5049 2072 6571 7565  urrent API reque
+0000e860: 7374 7320 746f 206d 616b 6522 2c20 7479  sts to make", ty
+0000e870: 7065 3d69 6e74 2c20 6465 6661 756c 743d  pe=int, default=
+0000e880: 3130 290d 0a20 2020 2070 6172 7365 722e  10)..    parser.
+0000e890: 6164 645f 6172 6775 6d65 6e74 2827 2d76  add_argument('-v
+0000e8a0: 272c 2027 2d2d 7665 7273 696f 6e27 2c20  ', '--version', 
+0000e8b0: 6163 7469 6f6e 3d27 7665 7273 696f 6e27  action='version'
+0000e8c0: 2c20 7665 7273 696f 6e3d 5645 5253 494f  , version=VERSIO
+0000e8d0: 4e29 0d0a 0d0a 2020 2020 6172 6773 203d  N)....    args =
+0000e8e0: 2070 6172 7365 722e 7061 7273 655f 6172   parser.parse_ar
+0000e8f0: 6773 2829 0d0a 0d0a 2020 2020 7372 635f  gs()....    src_
+0000e900: 6c61 6e67 7561 6765 203d 2061 7267 732e  language = args.
+0000e910: 7372 635f 6c61 6e67 7561 6765 0d0a 2020  src_language..  
+0000e920: 2020 6473 745f 6c61 6e67 7561 6765 203d    dst_language =
+0000e930: 2061 7267 732e 6473 745f 6c61 6e67 7561   args.dst_langua
+0000e940: 6765 0d0a 0d0a 2020 2020 6d6f 6465 6c5f  ge....    model_
+0000e950: 6e61 6d65 203d 2061 7267 732e 6d6f 6465  name = args.mode
+0000e960: 6c5f 6e61 6d65 0d0a 2020 2020 6966 206d  l_name..    if m
+0000e970: 6f64 656c 5f6e 616d 652e 656e 6473 7769  odel_name.endswi
+0000e980: 7468 2822 2e65 6e22 293a 0d0a 2020 2020  th(".en"):..    
+0000e990: 2020 2020 7072 696e 7428 6622 7b6d 6f64      print(f"{mod
+0000e9a0: 656c 5f6e 616d 657d 2069 7320 616e 2045  el_name} is an E
+0000e9b0: 6e67 6c69 7368 2d6f 6e6c 7920 6d6f 6465  nglish-only mode
+0000e9c0: 6c2c 2066 6f72 6369 6e67 2045 6e67 6c69  l, forcing Engli
+0000e9d0: 7368 2064 6574 6563 7469 6f6e 2e22 290d  sh detection.").
+0000e9e0: 0a20 2020 2020 2020 2061 7267 732e 7372  .        args.sr
+0000e9f0: 635f 6c61 6e67 7561 6765 203d 2022 656e  c_language = "en
+0000ea00: 220d 0a20 2020 2065 6c69 6620 6172 6773  "..    elif args
+0000ea10: 2e73 7263 5f6c 616e 6775 6167 6520 213d  .src_language !=
+0000ea20: 2022 6175 746f 223a 0d0a 2020 2020 2020   "auto":..      
+0000ea30: 2020 6172 6773 2e73 7263 5f6c 616e 6775    args.src_langu
+0000ea40: 6167 6520 3d20 7372 635f 6c61 6e67 7561  age = src_langua
+0000ea50: 6765 0d0a 0d0a 2020 2020 236d 6f64 656c  ge....    #model
+0000ea60: 203d 2057 6869 7370 6572 4d6f 6465 6c28   = WhisperModel(
+0000ea70: 6d6f 6465 6c5f 6e61 6d65 2c20 636f 6d70  model_name, comp
+0000ea80: 7574 655f 7479 7065 3d22 666c 6f61 7433  ute_type="float3
+0000ea90: 3222 2c20 6370 755f 7468 7265 6164 733d  2", cpu_threads=
+0000eaa0: 342c 206e 756d 5f77 6f72 6b65 7273 3d31  4, num_workers=1
+0000eab0: 3629 0d0a 2020 2020 6d6f 6465 6c20 3d20  6)..    model = 
+0000eac0: 5768 6973 7065 724d 6f64 656c 286d 6f64  WhisperModel(mod
+0000ead0: 656c 5f6e 616d 652c 2063 6f6d 7075 7465  el_name, compute
+0000eae0: 5f74 7970 653d 2266 6c6f 6174 3332 2229  _type="float32")
+0000eaf0: 0d0a 0d0a 2020 2020 6966 2061 7267 732e  ....    if args.
+0000eb00: 6c69 7374 5f6d 6f64 656c 733a 0d0a 2020  list_models:..  
+0000eb10: 2020 2020 2020 7072 696e 7428 224c 6973        print("Lis
+0000eb20: 7420 6f66 2077 6869 7370 6572 206d 6f64  t of whisper mod
+0000eb30: 656c 733a 2229 0d0a 2020 2020 2020 2020  els:")..        
+0000eb40: 2366 6f72 206d 6f64 656c 5f6e 616d 6520  #for model_name 
+0000eb50: 696e 2077 6869 7370 6572 2e61 7661 696c  in whisper.avail
+0000eb60: 6162 6c65 5f6d 6f64 656c 7328 293a 0d0a  able_models():..
+0000eb70: 2020 2020 2020 2020 666f 7220 6d6f 6465          for mode
+0000eb80: 6c5f 6e61 6d65 2069 6e20 7768 6973 7065  l_name in whispe
+0000eb90: 725f 6d6f 6465 6c73 3a0d 0a20 2020 2020  r_models:..     
+0000eba0: 2020 2020 2020 2070 7269 6e74 286d 6f64         print(mod
+0000ebb0: 656c 5f6e 616d 6529 0d0a 2020 2020 2020  el_name)..      
+0000ebc0: 2020 7265 7475 726e 2030 0d0a 0d0a 2020    return 0....  
+0000ebd0: 2020 7768 6973 7065 725f 6c61 6e67 7561    whisper_langua
+0000ebe0: 6765 203d 2057 6869 7370 6572 4c61 6e67  ge = WhisperLang
+0000ebf0: 7561 6765 2829 0d0a 2020 2020 676f 6f67  uage()..    goog
+0000ec00: 6c65 5f6c 616e 6775 6167 6520 3d20 476f  le_language = Go
+0000ec10: 6f67 6c65 4c61 6e67 7561 6765 2829 0d0a  ogleLanguage()..
+0000ec20: 0d0a 2020 2020 6966 2061 7267 732e 6c69  ..    if args.li
+0000ec30: 7374 5f77 6869 7370 6572 5f6c 616e 6775  st_whisper_langu
+0000ec40: 6167 6573 3a0d 0a20 2020 2020 2020 2070  ages:..        p
+0000ec50: 7269 6e74 2822 4c69 7374 206f 6620 7768  rint("List of wh
+0000ec60: 6973 7065 7220 7375 7070 6f72 7465 6420  isper supported 
+0000ec70: 6c61 6e67 7561 6765 733a 2229 0d0a 2020  languages:")..  
+0000ec80: 2020 2020 2020 666f 7220 7768 6973 7065        for whispe
+0000ec90: 725f 636f 6465 2c20 7768 6973 7065 725f  r_code, whisper_
+0000eca0: 6c61 6e67 7561 6765 2069 6e20 736f 7274  language in sort
+0000ecb0: 6564 2877 6869 7370 6572 5f6c 616e 6775  ed(whisper_langu
+0000ecc0: 6167 652e 6e61 6d65 5f6f 665f 636f 6465  age.name_of_code
+0000ecd0: 2e69 7465 6d73 2829 293a 0d0a 2020 2020  .items()):..    
+0000ece0: 2020 2020 2020 2020 7072 696e 7428 2225          print("%
+0000ecf0: 2d38 7320 3a20 2573 2220 2528 7768 6973  -8s : %s" %(whis
+0000ed00: 7065 725f 636f 6465 2c20 7768 6973 7065  per_code, whispe
+0000ed10: 725f 6c61 6e67 7561 6765 2929 0d0a 2020  r_language))..  
+0000ed20: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
+0000ed30: 0d0a 2020 2020 6966 2061 7267 732e 6c69  ..    if args.li
+0000ed40: 7374 5f67 6f6f 676c 655f 6c61 6e67 7561  st_google_langua
+0000ed50: 6765 733a 0d0a 2020 2020 2020 2020 7072  ges:..        pr
+0000ed60: 696e 7428 224c 6973 7420 6f66 2067 6f6f  int("List of goo
+0000ed70: 676c 6520 7472 616e 736c 6174 6520 7375  gle translate su
+0000ed80: 7070 6f72 7465 6420 6c61 6e67 7561 6765  pported language
+0000ed90: 733a 2229 0d0a 2020 2020 2020 2020 666f  s:")..        fo
+0000eda0: 7220 676f 6f67 6c65 5f63 6f64 652c 2067  r google_code, g
+0000edb0: 6f6f 676c 655f 6c61 6e67 7561 6765 2069  oogle_language i
+0000edc0: 6e20 736f 7274 6564 2867 6f6f 676c 655f  n sorted(google_
+0000edd0: 6c61 6e67 7561 6765 2e6e 616d 655f 6f66  language.name_of
+0000ede0: 5f63 6f64 652e 6974 656d 7328 2929 3a0d  _code.items()):.
+0000edf0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0000ee00: 6e74 2822 252d 3873 203a 2025 7322 2025  nt("%-8s : %s" %
+0000ee10: 2867 6f6f 676c 655f 636f 6465 2c20 676f  (google_code, go
+0000ee20: 6f67 6c65 5f6c 616e 6775 6167 6529 290d  ogle_language)).
+0000ee30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000ee40: 300d 0a0d 0a20 2020 2069 6620 6172 6773  0....    if args
+0000ee50: 2e73 7263 5f6c 616e 6775 6167 6520 6e6f  .src_language no
+0000ee60: 7420 696e 2077 6869 7370 6572 5f6c 616e  t in whisper_lan
+0000ee70: 6775 6167 652e 6e61 6d65 5f6f 665f 636f  guage.name_of_co
+0000ee80: 6465 2e6b 6579 7328 293a 0d0a 2020 2020  de.keys():..    
+0000ee90: 2020 2020 7072 696e 7428 2253 6f75 7263      print("Sourc
+0000eea0: 6520 6c61 6e67 7561 6765 2069 7320 6e6f  e language is no
+0000eeb0: 7420 7375 7070 6f72 7465 642e 2052 756e  t supported. Run
+0000eec0: 2077 6974 6820 2d2d 6c69 7374 2d77 6869   with --list-whi
+0000eed0: 7370 6572 2d6c 616e 6775 6167 6573 2074  sper-languages t
+0000eee0: 6f20 7365 6520 616c 6c20 7768 6973 7065  o see all whispe
+0000eef0: 7220 7375 7070 6f72 7465 6420 6c61 6e67  r supported lang
+0000ef00: 7561 6765 732e 2229 0d0a 2020 2020 2020  uages.")..      
+0000ef10: 2020 7265 7475 726e 2031 0d0a 0d0a 2020    return 1....  
+0000ef20: 2020 6966 2061 7267 732e 6473 745f 6c61    if args.dst_la
+0000ef30: 6e67 7561 6765 3a0d 0a20 2020 2020 2020  nguage:..       
+0000ef40: 2069 6620 6e6f 7420 6172 6773 2e64 7374   if not args.dst
+0000ef50: 5f6c 616e 6775 6167 6520 696e 2067 6f6f  _language in goo
+0000ef60: 676c 655f 6c61 6e67 7561 6765 2e6e 616d  gle_language.nam
+0000ef70: 655f 6f66 5f63 6f64 652e 6b65 7973 2829  e_of_code.keys()
+0000ef80: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+0000ef90: 7269 6e74 2822 4465 7374 696e 6174 696f  rint("Destinatio
+0000efa0: 6e20 6c61 6e67 7561 6765 2069 7320 6e6f  n language is no
+0000efb0: 7420 7375 7070 6f72 7465 642e 2052 756e  t supported. Run
+0000efc0: 2077 6974 6820 2d2d 6c69 7374 2d67 6f6f   with --list-goo
+0000efd0: 676c 652d 6c61 6e67 7561 6765 7320 746f  gle-languages to
+0000efe0: 2073 6565 2061 6c6c 2067 6f6f 676c 6520   see all google 
+0000eff0: 7472 616e 736c 6174 6520 7375 7070 6f72  translate suppor
+0000f000: 7465 6420 6c61 6e67 7561 6765 732e 2229  ted languages.")
+0000f010: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000f020: 7475 726e 2031 0d0a 2020 2020 2020 2020  turn 1..        
+0000f030: 6966 206e 6f74 2069 735f 7361 6d65 5f6c  if not is_same_l
+0000f040: 616e 6775 6167 6528 6172 6773 2e73 7263  anguage(args.src
+0000f050: 5f6c 616e 6775 6167 652c 2061 7267 732e  _language, args.
+0000f060: 6473 745f 6c61 6e67 7561 6765 2c20 6572  dst_language, er
+0000f070: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+0000f080: 6c62 6163 6b3d 7368 6f77 5f65 7272 6f72  lback=show_error
+0000f090: 5f6d 6573 7361 6765 7329 3a0d 0a20 2020  _messages):..   
+0000f0a0: 2020 2020 2020 2020 2064 6f5f 7472 616e           do_tran
+0000f0b0: 736c 6174 6520 3d20 5472 7565 0d0a 2020  slate = True..  
+0000f0c0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0000f0d0: 2020 2020 2020 2020 2064 6f5f 7472 616e           do_tran
+0000f0e0: 736c 6174 6520 3d20 4661 6c73 650d 0a20  slate = False.. 
+0000f0f0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0000f100: 2020 646f 5f74 7261 6e73 6c61 7465 203d    do_translate =
+0000f110: 2046 616c 7365 0d0a 0d0a 2020 2020 6966   False....    if
+0000f120: 2061 7267 732e 6c69 7374 5f66 6f72 6d61   args.list_forma
+0000f130: 7473 3a0d 0a20 2020 2020 2020 2070 7269  ts:..        pri
+0000f140: 6e74 2822 4c69 7374 206f 6620 7375 7070  nt("List of supp
+0000f150: 6f72 7465 6420 7375 6274 6974 6c65 2066  orted subtitle f
+0000f160: 6f72 6d61 7473 3a22 290d 0a20 2020 2020  ormats:")..     
+0000f170: 2020 2066 6f72 2073 7562 7469 746c 655f     for subtitle_
+0000f180: 666f 726d 6174 2069 6e20 5375 6274 6974  format in Subtit
+0000f190: 6c65 466f 726d 6174 7465 722e 7375 7070  leFormatter.supp
+0000f1a0: 6f72 7465 645f 666f 726d 6174 733a 0d0a  orted_formats:..
+0000f1b0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000f1c0: 7428 227b 666f 726d 6174 7d22 2e66 6f72  t("{format}".for
+0000f1d0: 6d61 7428 666f 726d 6174 3d73 7562 7469  mat(format=subti
+0000f1e0: 746c 655f 666f 726d 6174 2929 0d0a 2020  tle_format))..  
+0000f1f0: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
+0000f200: 0d0a 2020 2020 6966 2061 7267 732e 666f  ..    if args.fo
+0000f210: 726d 6174 206e 6f74 2069 6e20 5375 6274  rmat not in Subt
+0000f220: 6974 6c65 466f 726d 6174 7465 722e 7375  itleFormatter.su
+0000f230: 7070 6f72 7465 645f 666f 726d 6174 733a  pported_formats:
+0000f240: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+0000f250: 2253 7562 7469 746c 6520 666f 726d 6174  "Subtitle format
+0000f260: 2069 7320 6e6f 7420 7375 7070 6f72 7465   is not supporte
+0000f270: 642e 2052 756e 2077 6974 6820 2d2d 6c69  d. Run with --li
+0000f280: 7374 2d66 6f72 6d61 7473 2074 6f20 7365  st-formats to se
+0000f290: 6520 616c 6c20 7375 7070 6f72 7465 6420  e all supported 
+0000f2a0: 666f 726d 6174 732e 2229 0d0a 2020 2020  formats.")..    
+0000f2b0: 2020 2020 7265 7475 726e 2031 0d0a 0d0a      return 1....
+0000f2c0: 2020 2020 6966 206e 6f74 2061 7267 732e      if not args.
+0000f2d0: 736f 7572 6365 5f70 6174 683a 0d0a 2020  source_path:..  
+0000f2e0: 2020 2020 2020 7061 7273 6572 2e70 7269        parser.pri
+0000f2f0: 6e74 5f68 656c 7028 7379 732e 7374 6465  nt_help(sys.stde
+0000f300: 7272 290d 0a20 2020 2020 2020 2072 6574  rr)..        ret
+0000f310: 7572 6e20 310d 0a0d 0a20 2020 2063 6f6d  urn 1....    com
+0000f320: 706c 6574 6564 5f74 6173 6b73 203d 2030  pleted_tasks = 0
+0000f330: 0d0a 2020 2020 6d65 6469 615f 6669 6c65  ..    media_file
+0000f340: 7061 7468 7320 3d20 5b5d 0d0a 2020 2020  paths = []..    
+0000f350: 6172 675f 6669 6c65 7061 7468 7320 3d20  arg_filepaths = 
+0000f360: 5b5d 0d0a 2020 2020 696e 7661 6c69 645f  []..    invalid_
+0000f370: 6d65 6469 615f 6669 6c65 7061 7468 7320  media_filepaths 
+0000f380: 3d20 5b5d 0d0a 2020 2020 6e6f 745f 6578  = []..    not_ex
+0000f390: 6973 745f 6669 6c65 7061 7468 7320 3d20  ist_filepaths = 
+0000f3a0: 5b5d 0d0a 2020 2020 6172 6770 6174 6820  []..    argpath 
+0000f3b0: 3d20 4e6f 6e65 0d0a 0d0a 2020 2020 6172  = None....    ar
+0000f3c0: 6773 5f73 6f75 7263 655f 7061 7468 203d  gs_source_path =
+0000f3d0: 2061 7267 732e 736f 7572 6365 5f70 6174   args.source_pat
+0000f3e0: 680d 0a0d 0a20 2020 2069 6620 286e 6f74  h....    if (not
+0000f3f0: 2022 2a22 2069 6e20 7374 7228 6172 6773   "*" in str(args
+0000f400: 5f73 6f75 7263 655f 7061 7468 2929 2061  _source_path)) a
+0000f410: 6e64 2028 6e6f 7420 223f 2220 696e 2073  nd (not "?" in s
+0000f420: 7472 2861 7267 735f 736f 7572 6365 5f70  tr(args_source_p
+0000f430: 6174 6829 293a 0d0a 2020 2020 2020 2020  ath)):..        
+0000f440: 666f 7220 6669 6c65 7061 7468 2069 6e20  for filepath in 
+0000f450: 6172 6773 5f73 6f75 7263 655f 7061 7468  args_source_path
+0000f460: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+0000f470: 7061 7468 203d 2050 6174 6828 6669 6c65  path = Path(file
+0000f480: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
+0000f490: 2020 2069 6620 6e6f 7420 6f73 2e70 6174     if not os.pat
+0000f4a0: 682e 6973 6669 6c65 2866 7061 7468 293a  h.isfile(fpath):
+0000f4b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f4c0: 2020 6e6f 745f 6578 6973 745f 6669 6c65    not_exist_file
+0000f4d0: 7061 7468 732e 6170 7065 6e64 2866 696c  paths.append(fil
+0000f4e0: 6570 6174 6829 0d0a 0d0a 2020 2020 6966  epath)....    if
+0000f4f0: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
+0000f500: 2022 7769 6e33 3222 3a0d 0a20 2020 2020   "win32":..     
+0000f510: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+0000f520: 6528 6c65 6e28 6172 6773 2e73 6f75 7263  e(len(args.sourc
+0000f530: 655f 7061 7468 2929 3a0d 0a20 2020 2020  e_path)):..     
+0000f540: 2020 2020 2020 2069 6620 2822 5b22 206f         if ("[" o
+0000f550: 7220 225d 2229 2069 6e20 6172 6773 2e73  r "]") in args.s
+0000f560: 6f75 7263 655f 7061 7468 5b69 5d3a 0d0a  ource_path[i]:..
+0000f570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f580: 706c 6163 6568 6f6c 6465 7220 3d20 2223  placeholder = "#
+0000f590: 5445 4d50 2322 0d0a 2020 2020 2020 2020  TEMP#"..        
+0000f5a0: 2020 2020 2020 2020 6172 6773 5f73 6f75          args_sou
+0000f5b0: 7263 655f 7061 7468 5b69 5d20 3d20 6172  rce_path[i] = ar
+0000f5c0: 6773 2e73 6f75 7263 655f 7061 7468 5b69  gs.source_path[i
+0000f5d0: 5d2e 7265 706c 6163 6528 225b 222c 2070  ].replace("[", p
+0000f5e0: 6c61 6365 686f 6c64 6572 290d 0a20 2020  laceholder)..   
+0000f5f0: 2020 2020 2020 2020 2020 2020 2061 7267               arg
+0000f600: 735f 736f 7572 6365 5f70 6174 685b 695d  s_source_path[i]
+0000f610: 203d 2061 7267 735f 736f 7572 6365 5f70   = args_source_p
+0000f620: 6174 685b 695d 2e72 6570 6c61 6365 2822  ath[i].replace("
+0000f630: 5d22 2c20 225b 5d5d 2229 0d0a 2020 2020  ]", "[]]")..    
+0000f640: 2020 2020 2020 2020 2020 2020 6172 6773              args
+0000f650: 5f73 6f75 7263 655f 7061 7468 5b69 5d20  _source_path[i] 
+0000f660: 3d20 6172 6773 5f73 6f75 7263 655f 7061  = args_source_pa
+0000f670: 7468 5b69 5d2e 7265 706c 6163 6528 706c  th[i].replace(pl
+0000f680: 6163 6568 6f6c 6465 722c 2022 5b5b 5d22  aceholder, "[[]"
+0000f690: 290d 0a0d 0a20 2020 2066 6f72 2061 7267  )....    for arg
+0000f6a0: 2069 6e20 6172 6773 5f73 6f75 7263 655f   in args_source_
+0000f6b0: 7061 7468 3a0d 0a20 2020 2020 2020 2069  path:..        i
+0000f6c0: 6620 6e6f 7420 7379 732e 706c 6174 666f  f not sys.platfo
+0000f6d0: 726d 203d 3d20 2277 696e 3332 2220 3a0d  rm == "win32" :.
+0000f6e0: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
+0000f6f0: 203d 2065 7363 6170 6528 6172 6729 0d0a   = escape(arg)..
+0000f700: 0d0a 2020 2020 2020 2020 6172 675f 6669  ..        arg_fi
+0000f710: 6c65 7061 7468 7320 2b3d 2067 6c6f 6228  lepaths += glob(
+0000f720: 6172 6729 0d0a 0d0a 2020 2020 6966 2061  arg)....    if a
+0000f730: 7267 5f66 696c 6570 6174 6873 3a0d 0a20  rg_filepaths:.. 
+0000f740: 2020 2020 2020 2066 6f72 2061 7267 7061         for argpa
+0000f750: 7468 2069 6e20 6172 675f 6669 6c65 7061  th in arg_filepa
+0000f760: 7468 733a 0d0a 2020 2020 2020 2020 2020  ths:..          
+0000f770: 2020 6966 206f 732e 7061 7468 2e69 7366    if os.path.isf
+0000f780: 696c 6528 6172 6770 6174 6829 3a0d 0a20  ile(argpath):.. 
+0000f790: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000f7a0: 6620 6368 6563 6b5f 6669 6c65 5f74 7970  f check_file_typ
+0000f7b0: 6528 6172 6770 6174 682c 2065 7272 6f72  e(argpath, error
+0000f7c0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000f7d0: 636b 3d73 686f 775f 6572 726f 725f 6d65  ck=show_error_me
+0000f7e0: 7373 6167 6573 2920 3d3d 2027 7669 6465  ssages) == 'vide
+0000f7f0: 6f27 206f 7220 6368 6563 6b5f 6669 6c65  o' or check_file
+0000f800: 5f74 7970 6528 6172 6770 6174 682c 2065  _type(argpath, e
+0000f810: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+0000f820: 6c6c 6261 636b 3d73 686f 775f 6572 726f  llback=show_erro
+0000f830: 725f 6d65 7373 6167 6573 2920 3d3d 2027  r_messages) == '
+0000f840: 6175 6469 6f27 3a0d 0a20 2020 2020 2020  audio':..       
+0000f850: 2020 2020 2020 2020 2020 2020 206d 6564               med
+0000f860: 6961 5f66 696c 6570 6174 6873 2e61 7070  ia_filepaths.app
+0000f870: 656e 6428 6172 6770 6174 6829 0d0a 2020  end(argpath)..  
+0000f880: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000f890: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000f8a0: 2020 2020 2020 2020 2069 6e76 616c 6964           invalid
+0000f8b0: 5f6d 6564 6961 5f66 696c 6570 6174 6873  _media_filepaths
+0000f8c0: 2e61 7070 656e 6428 6172 6770 6174 6829  .append(argpath)
+0000f8d0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+0000f8e0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000f8f0: 2020 2020 206e 6f74 5f65 7869 7374 5f66       not_exist_f
+0000f900: 696c 6570 6174 6873 2e61 7070 656e 6428  ilepaths.append(
+0000f910: 6172 6770 6174 6829 0d0a 0d0a 2020 2020  argpath)....    
+0000f920: 2020 2020 6966 2069 6e76 616c 6964 5f6d      if invalid_m
+0000f930: 6564 6961 5f66 696c 6570 6174 6873 3a0d  edia_filepaths:.
+0000f940: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000f950: 2069 6e76 616c 6964 5f6d 6564 6961 5f66   invalid_media_f
+0000f960: 696c 6570 6174 6820 696e 2069 6e76 616c  ilepath in inval
+0000f970: 6964 5f6d 6564 6961 5f66 696c 6570 6174  id_media_filepat
+0000f980: 6873 3a0d 0a20 2020 2020 2020 2020 2020  hs:..           
+0000f990: 2020 2020 206d 7367 203d 2022 7b7d 2069       msg = "{} i
+0000f9a0: 7320 6e6f 7420 7661 6c69 6420 7669 6465  s not valid vide
+0000f9b0: 6f20 6f72 2061 7564 696f 2066 696c 6573  o or audio files
+0000f9c0: 222e 666f 726d 6174 2869 6e76 616c 6964  ".format(invalid
+0000f9d0: 5f6d 6564 6961 5f66 696c 6570 6174 6829  _media_filepath)
+0000f9e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f9f0: 2020 7072 696e 7428 6d73 6729 0d0a 0d0a    print(msg)....
+0000fa00: 2020 2020 6966 206e 6f74 5f65 7869 7374      if not_exist
+0000fa10: 5f66 696c 6570 6174 6873 3a0d 0a20 2020  _filepaths:..   
+0000fa20: 2020 2020 2066 6f72 206e 6f74 5f65 7869       for not_exi
+0000fa30: 7374 5f66 696c 6570 6174 6820 696e 206e  st_filepath in n
+0000fa40: 6f74 5f65 7869 7374 5f66 696c 6570 6174  ot_exist_filepat
+0000fa50: 6873 3a0d 0a20 2020 2020 2020 2020 2020  hs:..           
+0000fa60: 206d 7367 203d 2022 7b7d 2069 7320 6e6f   msg = "{} is no
+0000fa70: 7420 6578 6973 7422 2e66 6f72 6d61 7428  t exist".format(
+0000fa80: 6e6f 745f 6578 6973 745f 6669 6c65 7061  not_exist_filepa
+0000fa90: 7468 290d 0a20 2020 2020 2020 2020 2020  th)..           
+0000faa0: 2070 7269 6e74 286d 7367 290d 0a20 2020   print(msg)..   
+0000fab0: 2020 2020 2069 6620 286e 6f74 2028 222a       if (not ("*
+0000fac0: 2220 616e 6420 223f 2229 2069 6e20 7374  " and "?") in st
+0000fad0: 7228 6172 6773 5f73 6f75 7263 655f 7061  r(args_source_pa
+0000fae0: 7468 2929 3a0d 0a20 2020 2020 2020 2020  th)):..         
+0000faf0: 2020 2073 7973 2e65 7869 7428 3029 0d0a     sys.exit(0)..
+0000fb00: 0d0a 2020 2020 6966 206e 6f74 2061 7267  ..    if not arg
+0000fb10: 5f66 696c 6570 6174 6873 2061 6e64 206e  _filepaths and n
+0000fb20: 6f74 206e 6f74 5f65 7869 7374 5f66 696c  ot not_exist_fil
+0000fb30: 6570 6174 6873 3a0d 0a20 2020 2020 2020  epaths:..       
+0000fb40: 2070 7269 6e74 2822 4e6f 2061 6e79 2066   print("No any f
+0000fb50: 696c 6573 206d 6174 6368 696e 6720 6669  iles matching fi
+0000fb60: 6c65 6e61 6d65 7320 796f 7520 7479 7065  lenames you type
+0000fb70: 6422 290d 0a20 2020 2020 2020 2073 7973  d")..        sys
+0000fb80: 2e65 7869 7428 3029 0d0a 0d0a 2020 2020  .exit(0)....    
+0000fb90: 706f 6f6c 203d 206d 756c 7469 7072 6f63  pool = multiproc
+0000fba0: 6573 7369 6e67 2e50 6f6f 6c28 6172 6773  essing.Pool(args
+0000fbb0: 2e63 6f6e 6375 7272 656e 6379 290d 0a0d  .concurrency)...
+0000fbc0: 0a20 2020 2074 7261 6e73 6372 6962 655f  .    transcribe_
+0000fbd0: 656e 645f 7469 6d65 203d 204e 6f6e 650d  end_time = None.
+0000fbe0: 0a20 2020 2074 7261 6e73 6372 6962 655f  .    transcribe_
+0000fbf0: 656c 6170 7365 645f 7469 6d65 203d 204e  elapsed_time = N
+0000fc00: 6f6e 650d 0a20 2020 2074 7261 6e73 6372  one..    transcr
+0000fc10: 6962 655f 7374 6172 745f 7469 6d65 203d  ibe_start_time =
+0000fc20: 2074 696d 652e 7469 6d65 2829 0d0a 2020   time.time()..  
+0000fc30: 2020 7461 736b 203d 2022 7472 616e 7363    task = "transc
+0000fc40: 7269 6265 220d 0a0d 0a20 2020 2069 6620  ribe"....    if 
+0000fc50: 6172 6773 2e73 7263 5f6c 616e 6775 6167  args.src_languag
+0000fc60: 6520 3d3d 2028 2262 6122 206f 7220 2262  e == ("ba" or "b
+0000fc70: 7222 206f 7220 2266 6f22 206f 7220 226e  r" or "fo" or "n
+0000fc80: 6e22 206f 7220 226f 6322 206f 7220 2274  n" or "oc" or "t
+0000fc90: 6c22 206f 7220 2262 6f22 2920 616e 6420  l" or "bo") and 
+0000fca0: 646f 5f74 7261 6e73 6c61 7465 3a0d 0a20  do_translate:.. 
+0000fcb0: 2020 2020 2020 2074 6173 6b20 3d20 2274         task = "t
+0000fcc0: 7261 6e73 6c61 7465 220d 0a20 2020 2020  ranslate"..     
+0000fcd0: 2020 2073 7263 5f6c 616e 6775 6167 6520     src_language 
+0000fce0: 3d20 2265 6e22 0d0a 0d0a 2020 2020 666f  = "en"....    fo
+0000fcf0: 7220 6d65 6469 615f 6669 6c65 7061 7468  r media_filepath
+0000fd00: 2069 6e20 6d65 6469 615f 6669 6c65 7061   in media_filepa
+0000fd10: 7468 733a 0d0a 2020 2020 2020 2020 7072  ths:..        pr
+0000fd20: 696e 7428 2250 726f 6365 7373 696e 6720  int("Processing 
+0000fd30: 7b7d 203a 222e 666f 726d 6174 286d 6564  {} :".format(med
+0000fd40: 6961 5f66 696c 6570 6174 6829 290d 0a0d  ia_filepath))...
+0000fd50: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+0000fd60: 2020 2020 2020 2020 2020 2023 6d61 726b             #mark
+0000fd70: 6572 3d27 e296 8827 0d0a 2020 2020 2020  er='...'..      
+0000fd80: 2020 2020 2020 7769 6467 6574 7320 3d20        widgets = 
+0000fd90: 5b22 436f 6e76 6572 7469 6e67 2074 6f20  ["Converting to 
+0000fda0: 6120 7465 6d70 6f72 6172 7920 5741 5620  a temporary WAV 
+0000fdb0: 6669 6c65 2020 2020 2020 3a20 222c 2050  file      : ", P
+0000fdc0: 6572 6365 6e74 6167 6528 292c 2027 2027  ercentage(), ' '
+0000fdd0: 2c20 4261 7228 6d61 726b 6572 3d27 2327  , Bar(marker='#'
+0000fde0: 292c 2027 2027 2c20 4554 4128 295d 0d0a  ), ' ', ETA()]..
+0000fdf0: 2020 2020 2020 2020 2020 2020 7062 6172              pbar
+0000fe00: 203d 2050 726f 6772 6573 7342 6172 2877   = ProgressBar(w
+0000fe10: 6964 6765 7473 3d77 6964 6765 7473 2c20  idgets=widgets, 
+0000fe20: 6d61 7876 616c 3d31 3030 292e 7374 6172  maxval=100).star
+0000fe30: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+0000fe40: 2077 6176 5f63 6f6e 7665 7274 6572 203d   wav_converter =
+0000fe50: 2057 6176 436f 6e76 6572 7465 7228 7072   WavConverter(pr
+0000fe60: 6f67 7265 7373 5f63 616c 6c62 6163 6b3d  ogress_callback=
+0000fe70: 7368 6f77 5f70 726f 6772 6573 732c 2065  show_progress, e
+0000fe80: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+0000fe90: 6c6c 6261 636b 3d73 686f 775f 6572 726f  llback=show_erro
+0000fea0: 725f 6d65 7373 6167 6573 290d 0a20 2020  r_messages)..   
+0000feb0: 2020 2020 2020 2020 2077 6176 5f66 696c           wav_fil
+0000fec0: 6570 6174 682c 2073 616d 706c 655f 7261  epath, sample_ra
+0000fed0: 7465 203d 2077 6176 5f63 6f6e 7665 7274  te = wav_convert
+0000fee0: 6572 286d 6564 6961 5f66 696c 6570 6174  er(media_filepat
+0000fef0: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
+0000ff00: 7062 6172 2e66 696e 6973 6828 290d 0a0d  pbar.finish()...
+0000ff10: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
+0000ff20: 6465 7220 3d20 7761 7665 2e6f 7065 6e28  der = wave.open(
+0000ff30: 7761 765f 6669 6c65 7061 7468 290d 0a20  wav_filepath).. 
+0000ff40: 2020 2020 2020 2020 2020 2072 6174 6520             rate 
+0000ff50: 3d20 7265 6164 6572 2e67 6574 6672 616d  = reader.getfram
+0000ff60: 6572 6174 6528 290d 0a20 2020 2020 2020  erate()..       
+0000ff70: 2020 2020 2074 6f74 616c 5f64 7572 6174       total_durat
+0000ff80: 696f 6e20 3d20 7265 6164 6572 2e67 6574  ion = reader.get
+0000ff90: 6e66 7261 6d65 7328 2920 2f20 7261 7465  nframes() / rate
+0000ffa0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000ffb0: 6164 6572 2e63 6c6f 7365 2829 0d0a 0d0a  ader.close()....
+0000ffc0: 2020 2020 2020 2020 2020 2020 7365 676d              segm
+0000ffd0: 656e 7473 2c20 696e 666f 203d 206d 6f64  ents, info = mod
+0000ffe0: 656c 2e74 7261 6e73 6372 6962 6528 7761  el.transcribe(wa
+0000fff0: 765f 6669 6c65 7061 7468 2c20 6265 616d  v_filepath, beam
+00010000: 5f73 697a 653d 352c 206c 616e 6775 6167  _size=5, languag
+00010010: 653d 7372 635f 6c61 6e67 7561 6765 290d  e=src_language).
+00010020: 0a0d 0a20 2020 2020 2020 2020 2020 2077  ...            w
+00010030: 6964 6765 7473 203d 205b 2250 6572 666f  idgets = ["Perfo
+00010040: 726d 696e 6720 7370 6565 6368 2072 6563  rming speech rec
+00010050: 6f67 6e69 7469 6f6e 2020 2020 2020 2020  ognition        
+00010060: 2020 203a 2022 2c20 5065 7263 656e 7461     : ", Percenta
+00010070: 6765 2829 2c20 2720 272c 2042 6172 286d  ge(), ' ', Bar(m
+00010080: 6172 6b65 723d 2723 2729 2c20 2720 272c  arker='#'), ' ',
+00010090: 2045 5441 2829 5d0d 0a20 2020 2020 2020   ETA()]..       
+000100a0: 2020 2020 2070 6261 7220 3d20 5072 6f67       pbar = Prog
+000100b0: 7265 7373 4261 7228 7769 6467 6574 733d  ressBar(widgets=
+000100c0: 7769 6467 6574 732c 206d 6178 7661 6c3d  widgets, maxval=
+000100d0: 3130 3029 2e73 7461 7274 2829 0d0a 0d0a  100).start()....
+000100e0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+000100f0: 645f 7375 6274 6974 6c65 7320 3d20 5b5d  d_subtitles = []
+00010100: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00010110: 6769 6f6e 7320 3d20 5b5d 0d0a 2020 2020  gions = []..    
+00010120: 2020 2020 2020 2020 7472 616e 7363 7269          transcri
+00010130: 7074 7320 3d20 5b5d 0d0a 2020 2020 2020  pts = []..      
+00010140: 2020 2020 2020 666f 7220 7365 676d 656e        for segmen
+00010150: 7420 696e 2073 6567 6d65 6e74 733a 0d0a  t in segments:..
+00010160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010170: 7374 6172 7420 3d20 7365 676d 656e 742e  start = segment.
+00010180: 7374 6172 740d 0a20 2020 2020 2020 2020  start..         
+00010190: 2020 2020 2020 2065 6e64 203d 2073 6567         end = seg
+000101a0: 6d65 6e74 2e65 6e64 0d0a 2020 2020 2020  ment.end..      
+000101b0: 2020 2020 2020 2020 2020 7465 7874 203d            text =
+000101c0: 2073 6567 6d65 6e74 2e74 6578 740d 0a20   segment.text.. 
+000101d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000101e0: 6567 696f 6e73 2e61 7070 656e 6428 2873  egions.append((s
+000101f0: 7461 7274 2c20 656e 6429 290d 0a20 2020  tart, end))..   
+00010200: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00010210: 6e73 6372 6970 7473 2e61 7070 656e 6428  nscripts.append(
+00010220: 7465 7874 290d 0a20 2020 2020 2020 2020  text)..         
+00010230: 2020 2020 2020 2070 726f 6772 6573 7320         progress 
+00010240: 3d20 696e 7428 656e 6429 2a31 3030 2f74  = int(end)*100/t
+00010250: 6f74 616c 5f64 7572 6174 696f 6e0d 0a20  otal_duration.. 
+00010260: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00010270: 6261 722e 7570 6461 7465 2870 726f 6772  bar.update(progr
+00010280: 6573 7329 0d0a 2020 2020 2020 2020 2020  ess)..          
+00010290: 2020 7062 6172 2e66 696e 6973 6828 290d    pbar.finish().
+000102a0: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+000102b0: 6564 5f73 7562 7469 746c 6573 203d 205b  ed_subtitles = [
+000102c0: 2872 2c20 7429 2066 6f72 2072 2c20 7420  (r, t) for r, t 
+000102d0: 696e 207a 6970 2872 6567 696f 6e73 2c20  in zip(regions, 
+000102e0: 7472 616e 7363 7269 7074 7329 2069 6620  transcripts) if 
+000102f0: 745d 0d0a 0d0a 2020 2020 2020 2020 2020  t]....          
+00010300: 2020 7375 6274 6974 6c65 5f66 6f72 6d61    subtitle_forma
+00010310: 7420 3d20 6172 6773 2e66 6f72 6d61 740d  t = args.format.
+00010320: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
+00010330: 652c 2065 7874 203d 206f 732e 7061 7468  e, ext = os.path
+00010340: 2e73 706c 6974 6578 7428 6d65 6469 615f  .splitext(media_
+00010350: 6669 6c65 7061 7468 290d 0a20 2020 2020  filepath)..     
+00010360: 2020 2020 2020 2073 7562 7469 746c 655f         subtitle_
+00010370: 6669 6c65 7061 7468 203d 2022 7b62 6173  filepath = "{bas
+00010380: 657d 2e7b 666f 726d 6174 7d22 2e66 6f72  e}.{format}".for
+00010390: 6d61 7428 6261 7365 3d62 6173 652c 2066  mat(base=base, f
+000103a0: 6f72 6d61 743d 7375 6274 6974 6c65 5f66  ormat=subtitle_f
+000103b0: 6f72 6d61 7429 0d0a 0d0a 2020 2020 2020  ormat)....      
+000103c0: 2020 2020 2020 7772 6974 6572 203d 2053        writer = S
+000103d0: 7562 7469 746c 6557 7269 7465 7228 7265  ubtitleWriter(re
+000103e0: 6769 6f6e 732c 2074 7261 6e73 6372 6970  gions, transcrip
+000103f0: 7473 2c20 7375 6274 6974 6c65 5f66 6f72  ts, subtitle_for
+00010400: 6d61 742c 2065 7272 6f72 5f6d 6573 7361  mat, error_messa
+00010410: 6765 735f 6361 6c6c 6261 636b 3d73 686f  ges_callback=sho
+00010420: 775f 6572 726f 725f 6d65 7373 6167 6573  w_error_messages
+00010430: 290d 0a20 2020 2020 2020 2020 2020 2077  )..            w
+00010440: 7269 7465 722e 7772 6974 6528 7375 6274  riter.write(subt
+00010450: 6974 6c65 5f66 696c 6570 6174 6829 0d0a  itle_filepath)..
+00010460: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00010470: 2064 6f5f 7472 616e 736c 6174 653a 0d0a   do_translate:..
+00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010490: 2320 434f 4e43 5552 5245 4e54 2054 5241  # CONCURRENT TRA
+000104a0: 4e53 4c41 5449 4f4e 2055 5349 4e47 2063  NSLATION USING c
+000104b0: 6c61 7373 2053 656e 7465 6e63 6554 7261  lass SentenceTra
+000104c0: 6e73 6c61 746f 7228 6f62 6a65 6374 290d  nslator(object).
+000104d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000104e0: 2023 204e 4f20 4e45 4544 2054 4f20 5452   # NO NEED TO TR
+000104f0: 414e 534c 4154 4520 414c 4c20 7472 616e  ANSLATE ALL tran
+00010500: 7363 7269 7074 2049 4e20 7472 616e 7363  script IN transc
+00010510: 7269 7074 730d 0a20 2020 2020 2020 2020  ripts..         
+00010520: 2020 2020 2020 2023 2042 4543 4155 5345         # BECAUSE
+00010530: 2053 4f4d 4520 7265 6769 6f6e 2049 4e20   SOME region IN 
+00010540: 7265 6769 6f6e 7320 4d41 5920 4a55 5354  regions MAY JUST
+00010550: 2048 4156 4520 7472 616e 7363 7269 7074   HAVE transcript
+00010560: 2057 4954 4820 454d 5054 5920 5354 5249   WITH EMPTY STRI
+00010570: 4e47 0d0a 2020 2020 2020 2020 2020 2020  NG..            
+00010580: 2020 2020 2320 4a55 5354 2054 5241 4e53      # JUST TRANS
+00010590: 4c41 5445 2041 4c52 4541 4459 2043 5245  LATE ALREADY CRE
+000105a0: 4154 4544 2073 7562 7469 746c 6573 2045  ATED subtitles E
+000105b0: 4e54 5249 4553 2046 524f 4d20 7469 6d65  NTRIES FROM time
+000105c0: 645f 7375 6274 6974 6c65 730d 0a20 2020  d_subtitles..   
+000105d0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+000105e0: 6564 5f73 7562 7469 746c 6573 203d 2077  ed_subtitles = w
+000105f0: 7269 7465 722e 7469 6d65 645f 7375 6274  riter.timed_subt
+00010600: 6974 6c65 730d 0a20 2020 2020 2020 2020  itles..         
+00010610: 2020 2020 2020 2063 7265 6174 6564 5f72         created_r
+00010620: 6567 696f 6e73 203d 205b 5d0d 0a20 2020  egions = []..   
+00010630: 2020 2020 2020 2020 2020 2020 2063 7265               cre
+00010640: 6174 6564 5f73 7562 7469 746c 6573 203d  ated_subtitles =
+00010650: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00010660: 2020 2020 2066 6f72 2065 6e74 7279 2069       for entry i
+00010670: 6e20 7469 6d65 645f 7375 6274 6974 6c65  n timed_subtitle
+00010680: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00010690: 2020 2020 2020 2020 6372 6561 7465 645f          created_
+000106a0: 7265 6769 6f6e 732e 6170 7065 6e64 2865  regions.append(e
+000106b0: 6e74 7279 5b30 5d29 0d0a 2020 2020 2020  ntry[0])..      
+000106c0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
+000106d0: 6561 7465 645f 7375 6274 6974 6c65 732e  eated_subtitles.
+000106e0: 6170 7065 6e64 2865 6e74 7279 5b31 5d29  append(entry[1])
+000106f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00010700: 2020 2020 7072 6f6d 7074 203d 2022 5472      prompt = "Tr
+00010710: 616e 736c 6174 696e 6720 6672 6f6d 2025  anslating from %
+00010720: 7320 746f 2025 7320 2020 3a20 2220 2528  s to %s   : " %(
+00010730: 7372 635f 6c61 6e67 7561 6765 2e63 656e  src_language.cen
+00010740: 7465 7228 3829 2c20 6473 745f 6c61 6e67  ter(8), dst_lang
+00010750: 7561 6765 2e63 656e 7465 7228 3829 290d  uage.center(8)).
+00010760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010770: 2077 6964 6765 7473 203d 205b 7072 6f6d   widgets = [prom
+00010780: 7074 2c20 5065 7263 656e 7461 6765 2829  pt, Percentage()
+00010790: 2c20 2720 272c 2042 6172 286d 6172 6b65  , ' ', Bar(marke
+000107a0: 723d 2723 2729 2c20 2720 272c 2045 5441  r='#'), ' ', ETA
+000107b0: 2829 5d0d 0a20 2020 2020 2020 2020 2020  ()]..           
+000107c0: 2020 2020 2070 6261 7220 3d20 5072 6f67       pbar = Prog
+000107d0: 7265 7373 4261 7228 7769 6467 6574 733d  ressBar(widgets=
+000107e0: 7769 6467 6574 732c 206d 6178 7661 6c3d  widgets, maxval=
+000107f0: 6c65 6e28 7469 6d65 645f 7375 6274 6974  len(timed_subtit
+00010800: 6c65 7329 292e 7374 6172 7428 290d 0a0d  les)).start()...
+00010810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010820: 2074 7261 6e73 6372 6970 745f 7472 616e   transcript_tran
+00010830: 736c 6174 6f72 203d 2053 656e 7465 6e63  slator = Sentenc
+00010840: 6554 7261 6e73 6c61 746f 7228 7372 633d  eTranslator(src=
+00010850: 6172 6773 2e73 7263 5f6c 616e 6775 6167  args.src_languag
+00010860: 652c 2064 7374 3d61 7267 732e 6473 745f  e, dst=args.dst_
+00010870: 6c61 6e67 7561 6765 2c20 6572 726f 725f  language, error_
+00010880: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+00010890: 6b3d 7368 6f77 5f65 7272 6f72 5f6d 6573  k=show_error_mes
+000108a0: 7361 6765 7329 0d0a 0d0a 2020 2020 2020  sages)....      
+000108b0: 2020 2020 2020 2020 2020 7472 616e 736c            transl
+000108c0: 6174 6564 5f73 7562 7469 746c 6573 203d  ated_subtitles =
+000108d0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000108e0: 2020 2020 2066 6f72 2069 2c20 7472 616e       for i, tran
+000108f0: 736c 6174 6564 5f73 7562 7469 746c 6520  slated_subtitle 
+00010900: 696e 2065 6e75 6d65 7261 7465 2870 6f6f  in enumerate(poo
+00010910: 6c2e 696d 6170 2874 7261 6e73 6372 6970  l.imap(transcrip
+00010920: 745f 7472 616e 736c 6174 6f72 2c20 6372  t_translator, cr
+00010930: 6561 7465 645f 7375 6274 6974 6c65 7329  eated_subtitles)
+00010940: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00010950: 2020 2020 2020 2020 7472 616e 736c 6174          translat
+00010960: 6564 5f73 7562 7469 746c 6573 2e61 7070  ed_subtitles.app
+00010970: 656e 6428 7472 616e 736c 6174 6564 5f73  end(translated_s
+00010980: 7562 7469 746c 6529 0d0a 2020 2020 2020  ubtitle)..      
+00010990: 2020 2020 2020 2020 2020 2020 2020 7062                pb
+000109a0: 6172 2e75 7064 6174 6528 6929 0d0a 2020  ar.update(i)..  
+000109b0: 2020 2020 2020 2020 2020 2020 2020 7062                pb
+000109c0: 6172 2e66 696e 6973 6828 290d 0a0d 0a20  ar.finish().... 
+000109d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000109e0: 7261 6e73 6c61 7465 645f 7375 6274 6974  ranslated_subtit
+000109f0: 6c65 5f66 696c 6570 6174 6820 3d20 7375  le_filepath = su
+00010a00: 6274 6974 6c65 5f66 696c 6570 6174 685b  btitle_filepath[
+00010a10: 203a 2d34 5d20 2b20 272e 7472 616e 736c   :-4] + '.transl
+00010a20: 6174 6564 2e27 202b 2073 7562 7469 746c  ated.' + subtitl
+00010a30: 655f 666f 726d 6174 0d0a 2020 2020 2020  e_format..      
+00010a40: 2020 2020 2020 2020 2020 7472 616e 736c            transl
+00010a50: 6174 696f 6e5f 7772 6974 6572 203d 2053  ation_writer = S
+00010a60: 7562 7469 746c 6557 7269 7465 7228 6372  ubtitleWriter(cr
+00010a70: 6561 7465 645f 7265 6769 6f6e 732c 2074  eated_regions, t
+00010a80: 7261 6e73 6c61 7465 645f 7375 6274 6974  ranslated_subtit
+00010a90: 6c65 732c 2073 7562 7469 746c 655f 666f  les, subtitle_fo
+00010aa0: 726d 6174 2c20 6572 726f 725f 6d65 7373  rmat, error_mess
+00010ab0: 6167 6573 5f63 616c 6c62 6163 6b3d 7368  ages_callback=sh
+00010ac0: 6f77 5f65 7272 6f72 5f6d 6573 7361 6765  ow_error_message
+00010ad0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+00010ae0: 2020 2020 7472 616e 736c 6174 696f 6e5f      translation_
+00010af0: 7772 6974 6572 2e77 7269 7465 2874 7261  writer.write(tra
+00010b00: 6e73 6c61 7465 645f 7375 6274 6974 6c65  nslated_subtitle
+00010b10: 5f66 696c 6570 6174 6829 0d0a 0d0a 2020  _filepath)....  
+00010b20: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00010b30: 2744 6f6e 652e 2729 0d0a 2020 2020 2020  'Done.')..      
+00010b40: 2020 2020 2020 6966 2064 6f5f 7472 616e        if do_tran
+00010b50: 736c 6174 653a 0d0a 2020 2020 2020 2020  slate:..        
+00010b60: 2020 2020 2020 2020 6f73 2e72 656d 6f76          os.remov
+00010b70: 6528 7375 6274 6974 6c65 5f66 696c 6570  e(subtitle_filep
+00010b80: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
+00010b90: 2020 2020 2020 7072 696e 7428 2754 7261        print('Tra
+00010ba0: 6e73 6c61 7465 6420 7375 6274 6974 6c65  nslated subtitle
+00010bb0: 7320 6669 6c65 2063 7265 6174 6564 2061  s file created a
+00010bc0: 7420 2020 203a 207b 7d27 202e 666f 726d  t    : {}' .form
+00010bd0: 6174 2874 7261 6e73 6c61 7465 645f 7375  at(translated_su
+00010be0: 6274 6974 6c65 5f66 696c 6570 6174 6829  btitle_filepath)
+00010bf0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00010c00: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00010c10: 2020 2020 2020 7072 696e 7428 2253 7562        print("Sub
+00010c20: 7469 746c 6573 2066 696c 6520 6372 6561  titles file crea
+00010c30: 7465 6420 6174 2020 2020 2020 2020 2020  ted at          
+00010c40: 2020 2020 203a 207b 7d22 2e66 6f72 6d61       : {}".forma
+00010c50: 7428 7375 6274 6974 6c65 5f66 696c 6570  t(subtitle_filep
+00010c60: 6174 6829 290d 0a20 2020 2020 2020 2020  ath))..         
+00010c70: 2020 2070 7269 6e74 2827 2729 0d0a 2020     print('')..  
+00010c80: 2020 2020 2020 2020 2020 636f 6d70 6c65            comple
+00010c90: 7465 645f 7461 736b 7320 2b3d 2031 0d0a  ted_tasks += 1..
+00010ca0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00010cb0: 206c 656e 286d 6564 6961 5f66 696c 6570   len(media_filep
+00010cc0: 6174 6873 293e 3020 616e 6420 636f 6d70  aths)>0 and comp
+00010cd0: 6c65 7465 645f 7461 736b 7320 3d3d 206c  leted_tasks == l
+00010ce0: 656e 286d 6564 6961 5f66 696c 6570 6174  en(media_filepat
+00010cf0: 6873 293a 0d0a 2020 2020 2020 2020 2020  hs):..          
+00010d00: 2020 2020 2020 7472 616e 7363 7269 6265        transcribe
+00010d10: 5f65 6e64 5f74 696d 6520 3d20 7469 6d65  _end_time = time
+00010d20: 2e74 696d 6528 290d 0a20 2020 2020 2020  .time()..       
+00010d30: 2020 2020 2020 2020 2074 7261 6e73 6372           transcr
+00010d40: 6962 655f 656c 6170 7365 645f 7469 6d65  ibe_elapsed_time
+00010d50: 203d 2074 7261 6e73 6372 6962 655f 656e   = transcribe_en
+00010d60: 645f 7469 6d65 202d 2074 7261 6e73 6372  d_time - transcr
+00010d70: 6962 655f 7374 6172 745f 7469 6d65 0d0a  ibe_start_time..
+00010d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d90: 7472 616e 7363 7269 6265 5f65 6c61 7073  transcribe_elaps
+00010da0: 6564 5f74 696d 655f 7365 636f 6e64 7320  ed_time_seconds 
+00010db0: 3d20 7469 6d65 6465 6c74 6128 7365 636f  = timedelta(seco
+00010dc0: 6e64 733d 696e 7428 7472 616e 7363 7269  nds=int(transcri
+00010dd0: 6265 5f65 6c61 7073 6564 5f74 696d 6529  be_elapsed_time)
+00010de0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00010df0: 2020 2074 7261 6e73 6372 6962 655f 656c     transcribe_el
+00010e00: 6170 7365 645f 7469 6d65 5f73 7472 203d  apsed_time_str =
+00010e10: 2073 7472 2874 7261 6e73 6372 6962 655f   str(transcribe_
+00010e20: 656c 6170 7365 645f 7469 6d65 5f73 6563  elapsed_time_sec
+00010e30: 6f6e 6473 290d 0a20 2020 2020 2020 2020  onds)..         
+00010e40: 2020 2020 2020 2068 6f75 722c 206d 696e         hour, min
+00010e50: 7574 652c 2073 6563 6f6e 6420 3d20 7472  ute, second = tr
+00010e60: 616e 7363 7269 6265 5f65 6c61 7073 6564  anscribe_elapsed
+00010e70: 5f74 696d 655f 7374 722e 7370 6c69 7428  _time_str.split(
+00010e80: 223a 2229 0d0a 2020 2020 2020 2020 2020  ":")..          
+00010e90: 2020 2020 2020 6d73 6720 3d20 2254 6f74        msg = "Tot
+00010ea0: 616c 2074 7261 6e73 6372 6962 6520 7469  al transcribe ti
+00010eb0: 6d65 2020 2020 2020 2020 2020 2020 2020  me              
+00010ec0: 2020 2020 203a 2025 733a 2573 3a25 7322       : %s:%s:%s"
+00010ed0: 2025 2868 6f75 722e 7a66 696c 6c28 3229   %(hour.zfill(2)
+00010ee0: 2c20 6d69 6e75 7465 2c20 7365 636f 6e64  , minute, second
+00010ef0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00010f00: 2020 2070 7269 6e74 286d 7367 290d 0a0d     print(msg)...
+00010f10: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+00010f20: 4b65 7962 6f61 7264 496e 7465 7272 7570  KeyboardInterrup
+00010f30: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+00010f40: 7062 6172 2e66 696e 6973 6828 290d 0a20  pbar.finish().. 
+00010f50: 2020 2020 2020 2020 2020 2070 6f6f 6c2e             pool.
+00010f60: 7465 726d 696e 6174 6528 290d 0a20 2020  terminate()..   
+00010f70: 2020 2020 2020 2020 2070 6f6f 6c2e 636c           pool.cl
+00010f80: 6f73 6528 290d 0a20 2020 2020 2020 2020  ose()..         
+00010f90: 2020 2070 6f6f 6c2e 6a6f 696e 2829 0d0a     pool.join()..
+00010fa0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00010fb0: 7428 2243 616e 6365 6c6c 696e 6720 616c  t("Cancelling al
+00010fc0: 6c20 7461 736b 7322 290d 0a0d 0a20 2020  l tasks")....   
+00010fd0: 2020 2020 2020 2020 2069 6620 7379 732e           if sys.
+00010fe0: 706c 6174 666f 726d 203d 3d20 2277 696e  platform == "win
+00010ff0: 3332 223a 0d0a 2020 2020 2020 2020 2020  32":..          
+00011000: 2020 2020 2020 7374 6f70 5f66 666d 7065        stop_ffmpe
+00011010: 675f 7769 6e64 6f77 7328 6572 726f 725f  g_windows(error_
+00011020: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+00011030: 6b3d 7368 6f77 5f65 7272 6f72 5f6d 6573  k=show_error_mes
+00011040: 7361 6765 7329 0d0a 2020 2020 2020 2020  sages)..        
+00011050: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00011060: 2020 2020 2020 2020 2020 2073 746f 705f             stop_
+00011070: 6666 6d70 6567 5f6c 696e 7578 2865 7272  ffmpeg_linux(err
+00011080: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+00011090: 6261 636b 3d73 686f 775f 6572 726f 725f  back=show_error_
+000110a0: 6d65 7373 6167 6573 290d 0a0d 0a20 2020  messages)....   
+000110b0: 2020 2020 2020 2020 2072 656d 6f76 655f           remove_
+000110c0: 7465 6d70 5f66 696c 6573 2822 7761 7622  temp_files("wav"
+000110d0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+000110e0: 6574 7572 6e20 310d 0a0d 0a20 2020 2020  eturn 1....     
+000110f0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00011100: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
+00011110: 2020 2020 2020 2069 6620 6e6f 7420 4b65         if not Ke
+00011120: 7962 6f61 7264 496e 7465 7272 7570 7420  yboardInterrupt 
+00011130: 696e 2065 3a0d 0a20 2020 2020 2020 2020  in e:..         
+00011140: 2020 2020 2020 2070 6261 722e 6669 6e69         pbar.fini
+00011150: 7368 2829 0d0a 2020 2020 2020 2020 2020  sh()..          
+00011160: 2020 2020 2020 706f 6f6c 2e74 6572 6d69        pool.termi
+00011170: 6e61 7465 2829 0d0a 2020 2020 2020 2020  nate()..        
+00011180: 2020 2020 2020 2020 706f 6f6c 2e63 6c6f          pool.clo
+00011190: 7365 2829 0d0a 2020 2020 2020 2020 2020  se()..          
+000111a0: 2020 2020 2020 706f 6f6c 2e6a 6f69 6e28        pool.join(
+000111b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000111c0: 2020 2070 7269 6e74 2865 290d 0a0d 0a20     print(e).... 
+000111d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000111e0: 6620 7379 732e 706c 6174 666f 726d 203d  f sys.platform =
+000111f0: 3d20 2277 696e 3332 223a 0d0a 2020 2020  = "win32":..    
+00011200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011210: 7374 6f70 5f66 666d 7065 675f 7769 6e64  stop_ffmpeg_wind
+00011220: 6f77 7328 6572 726f 725f 6d65 7373 6167  ows(error_messag
+00011230: 6573 5f63 616c 6c62 6163 6b3d 7368 6f77  es_callback=show
+00011240: 5f65 7272 6f72 5f6d 6573 7361 6765 7329  _error_messages)
+00011250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011260: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00011270: 2020 2020 2020 2020 2020 2020 2073 746f               sto
+00011280: 705f 6666 6d70 6567 5f6c 696e 7578 2865  p_ffmpeg_linux(e
+00011290: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+000112a0: 6c6c 6261 636b 3d73 686f 775f 6572 726f  llback=show_erro
+000112b0: 725f 6d65 7373 6167 6573 290d 0a0d 0a20  r_messages).... 
+000112c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000112d0: 656d 6f76 655f 7465 6d70 5f66 696c 6573  emove_temp_files
+000112e0: 2822 7761 7622 290d 0a20 2020 2020 2020  ("wav")..       
+000112f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00011300: 310d 0a0d 0a20 2020 2069 6620 706f 6f6c  1....    if pool
+00011310: 3a0d 0a20 2020 2020 2020 2070 6f6f 6c2e  :..        pool.
+00011320: 636c 6f73 6528 290d 0a20 2020 2020 2020  close()..       
+00011330: 2070 6f6f 6c2e 6a6f 696e 2829 0d0a 2020   pool.join()..  
+00011340: 2020 2020 2020 706f 6f6c 203d 204e 6f6e        pool = Non
+00011350: 650d 0a0d 0a20 2020 2069 6620 7379 732e  e....    if sys.
+00011360: 706c 6174 666f 726d 203d 3d20 2277 696e  platform == "win
+00011370: 3332 223a 0d0a 2020 2020 2020 2020 7374  32":..        st
+00011380: 6f70 5f66 666d 7065 675f 7769 6e64 6f77  op_ffmpeg_window
+00011390: 7328 6572 726f 725f 6d65 7373 6167 6573  s(error_messages
+000113a0: 5f63 616c 6c62 6163 6b3d 7368 6f77 5f65  _callback=show_e
+000113b0: 7272 6f72 5f6d 6573 7361 6765 7329 0d0a  rror_messages)..
+000113c0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000113d0: 2020 2073 746f 705f 6666 6d70 6567 5f6c     stop_ffmpeg_l
+000113e0: 696e 7578 2865 7272 6f72 5f6d 6573 7361  inux(error_messa
+000113f0: 6765 735f 6361 6c6c 6261 636b 3d73 686f  ges_callback=sho
+00011400: 775f 6572 726f 725f 6d65 7373 6167 6573  w_error_messages
+00011410: 290d 0a0d 0a20 2020 2072 656d 6f76 655f  )....    remove_
+00011420: 7465 6d70 5f66 696c 6573 2822 7761 7622  temp_files("wav"
+00011430: 290d 0a0d 0a69 6620 5f5f 6e61 6d65 5f5f  )....if __name__
+00011440: 203d 3d20 275f 5f6d 6169 6e5f 5f27 3a0d   == '__main__':.
+00011450: 0a20 2020 206d 756c 7469 7072 6f63 6573  .    multiproces
+00011460: 7369 6e67 2e66 7265 657a 655f 7375 7070  sing.freeze_supp
+00011470: 6f72 7428 290d 0a20 2020 2073 7973 2e65  ort()..    sys.e
+00011480: 7869 7428 6d61 696e 2829 290d 0a         xit(main())..
```

### Comparing `whisper_autosrt-0.0.2/whisper_autosrt.egg-info/PKG-INFO` & `whisper_autosrt-0.0.4/whisper_autosrt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: whisper-autosrt
-Version: 0.0.2
-Summary: a command line utility for automatic speech recognition and subtitle generation
-Home-page: https://github.com/botbahlul/whisper_autosrt
-Author: Bot Bahlul
-Author-email: bot.bahlul@gmail.com
-License: MIT License
-        
-        Copyright (c) 2022 botbahlul
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-
-whisper_autosrt is a utility for automatic speech recognition and subtitle generation.  It takes video or audio files as input, convert it to a temporary wav file then generatetranscriptions for that wav file, and optionally translates them to a different languageand finally saves the resulting subtitles file to disk.                                 It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+Metadata-Version: 2.1
+Name: whisper-autosrt
+Version: 0.0.4
+Summary: a command line utility for automatic speech recognition and subtitle generation
+Home-page: https://github.com/botbahlul/whisper_autosrt
+Author: Bot Bahlul
+Author-email: bot.bahlul@gmail.com
+License: MIT License
+        
+        Copyright (c) 2022 botbahlul
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+
+whisper_autosrt is a utility for automatic speech recognition and subtitle generation.  It takes video or audio files as input, convert it to a temporary wav file then generatetranscriptions for that wav file, and optionally translates them to a different languageand finally saves the resulting subtitles file to disk.                                 It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
```

