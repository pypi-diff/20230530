# Comparing `tmp/whisper_autosrt-0.0.5.tar.gz` & `tmp/whisper_autosrt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_autosrt-0.0.5.tar", last modified: Tue May 30 05:54:13 2023, max compression
+gzip compressed data, was "whisper_autosrt-0.0.6.tar", last modified: Tue May 30 14:18:41 2023, max compression
```

## Comparing `whisper_autosrt-0.0.5.tar` & `whisper_autosrt-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 05:54:13.452858 whisper_autosrt-0.0.5/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2009 2023-05-30 05:54:13.452858 whisper_autosrt-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.0.5/README.md
--rw-rw-rw-   0        0        0      147 2023-05-30 05:54:13.455853 whisper_autosrt-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1463 2023-05-29 23:39:40.000000 whisper_autosrt-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:54:13.395403 whisper_autosrt-0.0.5/whisper_autosrt/
--rw-rw-rw-   0        0        0    70808 2023-05-30 05:53:15.000000 whisper_autosrt-0.0.5/whisper_autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 05:54:13.450610 whisper_autosrt-0.0.5/whisper_autosrt.egg-info/
--rw-rw-rw-   0        0        0     2009 2023-05-30 05:54:13.000000 whisper_autosrt-0.0.5/whisper_autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-05-30 05:54:13.000000 whisper_autosrt-0.0.5/whisper_autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 05:54:13.000000 whisper_autosrt-0.0.5/whisper_autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-30 05:54:13.000000 whisper_autosrt-0.0.5/whisper_autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2023-05-30 05:54:13.000000 whisper_autosrt-0.0.5/whisper_autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-30 05:54:13.000000 whisper_autosrt-0.0.5/whisper_autosrt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 14:18:41.129151 whisper_autosrt-0.0.6/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1956 2023-05-30 14:18:41.129899 whisper_autosrt-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.0.6/README.md
+-rw-rw-rw-   0        0        0      147 2023-05-30 14:18:41.132146 whisper_autosrt-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2023-05-30 14:11:58.000000 whisper_autosrt-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:18:41.083910 whisper_autosrt-0.0.6/whisper_autosrt/
+-rw-rw-rw-   0        0        0    71925 2023-05-30 14:12:34.000000 whisper_autosrt-0.0.6/whisper_autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:18:41.127652 whisper_autosrt-0.0.6/whisper_autosrt.egg-info/
+-rw-rw-rw-   0        0        0     1956 2023-05-30 14:18:40.000000 whisper_autosrt-0.0.6/whisper_autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-05-30 14:18:40.000000 whisper_autosrt-0.0.6/whisper_autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 14:18:40.000000 whisper_autosrt-0.0.6/whisper_autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-30 14:18:40.000000 whisper_autosrt-0.0.6/whisper_autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2023-05-30 14:18:40.000000 whisper_autosrt-0.0.6/whisper_autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-30 14:18:40.000000 whisper_autosrt-0.0.6/whisper_autosrt.egg-info/top_level.txt
```

### Comparing `whisper_autosrt-0.0.5/LICENSE` & `whisper_autosrt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.0.5/PKG-INFO` & `whisper_autosrt-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper_autosrt
-Version: 0.0.5
+Version: 0.0.6
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
@@ -24,8 +24,8 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 
-whisper_autosrt is a utility for automatic speech recognition and subtitle generation.  It takes video or audio files as input, convert it to a temporary wav file then generatetranscriptions for that wav file, and optionally translates them to a different languageand finally saves the resulting subtitles file to disk.                                 It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+whisper_autosrt is a command line utility for automatic speech recognition and subtitle generation. It takes video or audio files as input, generate transcriptions for them and optionally translates  them to a different language, and finally saves the resulting subtitles file to disk.               It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT,JSON, and RAW format.
```

### Comparing `whisper_autosrt-0.0.5/README.md` & `whisper_autosrt-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.0.5/setup.py` & `whisper_autosrt-0.0.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 from whisper_autosrt import VERSION
 
 long_description = (
-    'whisper_autosrt is a utility for automatic speech recognition and subtitle generation.  '
-    'It takes video or audio files as input, convert it to a temporary wav file then generate'
-    'transcriptions for that wav file, and optionally translates them to a different language'
-    'and finally saves the resulting subtitles file to disk.                                 '
-    'It supports a variety of input and output languages and can currently produce subtitles '
-    'in SRT, VTT, JSON, and RAW format.'
+    'whisper_autosrt is a command line utility for automatic speech recognition and subtitle generation. '
+    'It takes video or audio files as input, generate transcriptions for them and optionally translates  '
+    'them to a different language, and finally saves the resulting subtitles file to disk.               '
+    'It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT,'
+    'JSON, and RAW format.'
 )
 
 install_requires=[
     "requests>=2.3.0",
     "httpx>=0.24.0",
     "urllib3 >=1.26.0,<3.0",
     "pysrt>=1.0.1",
```

### Comparing `whisper_autosrt-0.0.5/whisper_autosrt/__init__.py` & `whisper_autosrt-0.0.6/whisper_autosrt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,4388 +39,4458 @@
 00000260: 6e67 7328 2269 676e 6f72 6522 2c20 6d65  ngs("ignore", me
 00000270: 7373 6167 653d 222e 2a54 6865 2027 6e6f  ssage=".*The 'no
 00000280: 7079 7468 6f6e 2720 6b65 7977 6f72 642e  python' keyword.
 00000290: 2a22 290d 0a66 726f 6d20 6661 7374 6572  *")..from faster
 000002a0: 5f77 6869 7370 6572 2069 6d70 6f72 7420  _whisper import 
 000002b0: 5768 6973 7065 724d 6f64 656c 0d0a 0d0a  WhisperModel....
 000002c0: 0d0a 5645 5253 494f 4e20 3d20 2230 2e30  ..VERSION = "0.0
-000002d0: 2e35 220d 0a0d 0a77 6869 7370 6572 5f6d  .5"....whisper_m
-000002e0: 6f64 656c 7320 3d20 5b0d 0a20 2020 2020  odels = [..     
-000002f0: 2020 2020 2020 2020 2020 2022 7469 6e79             "tiny
-00000300: 2e65 6e22 2c0d 0a20 2020 2020 2020 2020  .en",..         
-00000310: 2020 2020 2020 2022 7469 6e79 222c 0d0a         "tiny",..
-00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000330: 2262 6173 652e 656e 222c 0d0a 2020 2020  "base.en",..    
-00000340: 2020 2020 2020 2020 2020 2020 2262 6173              "bas
-00000350: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-00000360: 2020 2020 2022 736d 616c 6c2e 656e 222c       "small.en",
-00000370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000380: 2020 2273 6d61 6c6c 222c 0d0a 2020 2020    "small",..    
-00000390: 2020 2020 2020 2020 2020 2020 226d 6564              "med
-000003a0: 6975 6d2e 656e 222c 0d0a 2020 2020 2020  ium.en",..      
-000003b0: 2020 2020 2020 2020 2020 226d 6564 6975            "mediu
-000003c0: 6d22 2c0d 0a20 2020 2020 2020 2020 2020  m",..           
-000003d0: 2020 2020 2022 6c61 7267 652d 7631 222c       "large-v1",
-000003e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000003f0: 2020 226c 6172 6765 2d76 3222 2c0d 0a20    "large-v2",.. 
-00000400: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000410: 6c61 7267 6522 0d0a 5d0d 0a0d 0a23 3d3d  large"..]....#==
-00000420: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000430: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000440: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000450: 3d3d 3d3d 3d3d 2066 666d 7065 675f 7072  ====== ffmpeg_pr
-00000460: 6f67 7265 7373 5f79 6965 6c64 203d 3d3d  ogress_yield ===
-00000470: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000490: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000004a0: 3d3d 3d3d 3d23 0d0a 0d0a 696d 706f 7274  =====#....import
-000004b0: 2072 650d 0a23 696d 706f 7274 2073 7562   re..#import sub
-000004c0: 7072 6f63 6573 730d 0a66 726f 6d20 7479  process..from ty
-000004d0: 7069 6e67 2069 6d70 6f72 7420 416e 792c  ping import Any,
-000004e0: 2043 616c 6c61 626c 652c 2049 7465 7261   Callable, Itera
-000004f0: 746f 722c 204c 6973 742c 204f 7074 696f  tor, List, Optio
-00000500: 6e61 6c2c 2055 6e69 6f6e 0d0a 0d0a 0d0a  nal, Union......
-00000510: 6465 6620 746f 5f6d 7328 2a2a 6b77 6172  def to_ms(**kwar
-00000520: 6773 3a20 556e 696f 6e5b 666c 6f61 742c  gs: Union[float,
-00000530: 2069 6e74 2c20 7374 725d 2920 2d3e 2069   int, str]) -> i
-00000540: 6e74 3a0d 0a20 2020 2068 6f75 7220 3d20  nt:..    hour = 
-00000550: 696e 7428 6b77 6172 6773 2e67 6574 2822  int(kwargs.get("
-00000560: 686f 7572 222c 2030 2929 0d0a 2020 2020  hour", 0))..    
-00000570: 6d69 6e75 7465 203d 2069 6e74 286b 7761  minute = int(kwa
-00000580: 7267 732e 6765 7428 226d 696e 222c 2030  rgs.get("min", 0
-00000590: 2929 0d0a 2020 2020 7365 6320 3d20 696e  ))..    sec = in
-000005a0: 7428 6b77 6172 6773 2e67 6574 2822 7365  t(kwargs.get("se
-000005b0: 6322 2c20 3029 290d 0a20 2020 206d 7320  c", 0))..    ms 
-000005c0: 3d20 696e 7428 6b77 6172 6773 2e67 6574  = int(kwargs.get
-000005d0: 2822 6d73 222c 2030 2929 0d0a 0d0a 2020  ("ms", 0))....  
-000005e0: 2020 7265 7475 726e 2028 686f 7572 202a    return (hour *
-000005f0: 2036 3020 2a20 3630 202a 2031 3030 3029   60 * 60 * 1000)
-00000600: 202b 2028 6d69 6e75 7465 202a 2036 3020   + (minute * 60 
-00000610: 2a20 3130 3030 2920 2b20 2873 6563 202a  * 1000) + (sec *
-00000620: 2031 3030 3029 202b 206d 730d 0a0d 0a0d   1000) + ms.....
-00000630: 0a64 6566 205f 7072 6f62 655f 6475 7261  .def _probe_dura
-00000640: 7469 6f6e 2863 6d64 3a20 4c69 7374 5b73  tion(cmd: List[s
-00000650: 7472 5d29 202d 3e20 4f70 7469 6f6e 616c  tr]) -> Optional
-00000660: 5b69 6e74 5d3a 0d0a 2020 2020 2727 270d  [int]:..    '''.
-00000670: 0a20 2020 2047 6574 2074 6865 2064 7572  .    Get the dur
-00000680: 6174 696f 6e20 7669 6120 6666 7072 6f62  ation via ffprob
-00000690: 6520 6672 6f6d 2069 6e70 7574 206d 6564  e from input med
-000006a0: 6961 2066 696c 650d 0a20 2020 2069 6e20  ia file..    in 
-000006b0: 6361 7365 2066 666d 7065 6720 7761 7320  case ffmpeg was 
-000006c0: 7275 6e20 7769 7468 206c 6f67 6c65 7665  run with logleve
-000006d0: 6c3d 6572 726f 722e 0d0a 0d0a 2020 2020  l=error.....    
-000006e0: 4172 6773 3a0d 0a20 2020 2020 2020 2063  Args:..        c
-000006f0: 6d64 2028 4c69 7374 5b73 7472 5d29 3a20  md (List[str]): 
-00000700: 4120 6c69 7374 206f 6620 636f 6d6d 616e  A list of comman
-00000710: 6420 6c69 6e65 2065 6c65 6d65 6e74 732c  d line elements,
-00000720: 2065 2e67 2e20 5b22 6666 6d70 6567 222c   e.g. ["ffmpeg",
-00000730: 2022 2d69 222c 202e 2e2e 5d0d 0a0d 0a20   "-i", ...].... 
-00000740: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-00000750: 2020 2020 204f 7074 696f 6e61 6c5b 696e       Optional[in
-00000760: 745d 3a20 5468 6520 6475 7261 7469 6f6e  t]: The duration
-00000770: 2069 6e20 6d69 6c6c 6973 6563 6f6e 6473   in milliseconds
-00000780: 2e0d 0a20 2020 2027 2727 0d0a 0d0a 2020  ...    '''....  
-00000790: 2020 6465 6620 5f67 6574 5f66 696c 655f    def _get_file_
-000007a0: 6e61 6d65 2863 6d64 3a20 4c69 7374 5b73  name(cmd: List[s
-000007b0: 7472 5d29 202d 3e20 4f70 7469 6f6e 616c  tr]) -> Optional
-000007c0: 5b73 7472 5d3a 0d0a 2020 2020 2020 2020  [str]:..        
-000007d0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-000007e0: 2020 6964 7820 3d20 636d 642e 696e 6465    idx = cmd.inde
-000007f0: 7828 222d 6922 290d 0a20 2020 2020 2020  x("-i")..       
-00000800: 2020 2020 2072 6574 7572 6e20 636d 645b       return cmd[
-00000810: 6964 7820 2b20 315d 0d0a 2020 2020 2020  idx + 1]..      
-00000820: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
-00000830: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
-00000840: 2020 7265 7475 726e 204e 6f6e 650d 0a0d    return None...
-00000850: 0a20 2020 2066 696c 655f 6e61 6d65 203d  .    file_name =
-00000860: 205f 6765 745f 6669 6c65 5f6e 616d 6528   _get_file_name(
-00000870: 636d 6429 0d0a 2020 2020 6966 2066 696c  cmd)..    if fil
-00000880: 655f 6e61 6d65 2069 7320 4e6f 6e65 3a0d  e_name is None:.
-00000890: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000008a0: 4e6f 6e65 0d0a 0d0a 2020 2020 7472 793a  None....    try:
-000008b0: 0d0a 2020 2020 2020 2020 6966 2073 7973  ..        if sys
-000008c0: 2e70 6c61 7466 6f72 6d20 3d3d 2022 7769  .platform == "wi
-000008d0: 6e33 3222 3a0d 0a20 2020 2020 2020 2020  n32":..         
-000008e0: 2020 206f 7574 7075 7420 3d20 7375 6270     output = subp
-000008f0: 726f 6365 7373 2e63 6865 636b 5f6f 7574  rocess.check_out
-00000900: 7075 7428 0d0a 2020 2020 2020 2020 2020  put(..          
-00000910: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
-00000920: 2020 2020 2020 2020 2020 2020 2022 6666               "ff
-00000930: 7072 6f62 6522 2c0d 0a20 2020 2020 2020  probe",..       
-00000940: 2020 2020 2020 2020 2020 2020 2022 2d6c               "-l
-00000950: 6f67 6c65 7665 6c22 2c0d 0a20 2020 2020  oglevel",..     
-00000960: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000970: 2d31 222c 0d0a 2020 2020 2020 2020 2020  -1",..          
-00000980: 2020 2020 2020 2020 2020 222d 6869 6465            "-hide
-00000990: 5f62 616e 6e65 7222 2c0d 0a20 2020 2020  _banner",..     
-000009a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000009b0: 2d73 686f 775f 656e 7472 6965 7322 2c0d  -show_entries",.
-000009c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000009d0: 2020 2020 2022 666f 726d 6174 3d64 7572       "format=dur
-000009e0: 6174 696f 6e22 2c0d 0a20 2020 2020 2020  ation",..       
-000009f0: 2020 2020 2020 2020 2020 2020 2022 2d6f               "-o
-00000a00: 6622 2c0d 0a20 2020 2020 2020 2020 2020  f",..           
-00000a10: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
-00000a20: 743d 6e6f 7072 696e 745f 7772 6170 7065  t=noprint_wrappe
-00000a30: 7273 3d31 3a6e 6f6b 6579 3d31 222c 0d0a  rs=1:nokey=1",..
-00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a50: 2020 2020 6669 6c65 5f6e 616d 652c 0d0a      file_name,..
-00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a70: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00000a80: 2020 2020 756e 6976 6572 7361 6c5f 6e65      universal_ne
-00000a90: 776c 696e 6573 3d54 7275 652c 0d0a 2020  wlines=True,..  
-00000aa0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
-00000ab0: 6561 7469 6f6e 666c 6167 733d 7375 6270  eationflags=subp
-00000ac0: 726f 6365 7373 2e43 5245 4154 455f 4e4f  rocess.CREATE_NO
-00000ad0: 5f57 494e 444f 572c 0d0a 2020 2020 2020  _WINDOW,..      
-00000ae0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00000af0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00000b00: 2020 2020 6f75 7470 7574 203d 2073 7562      output = sub
-00000b10: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
-00000b20: 7470 7574 280d 0a20 2020 2020 2020 2020  tput(..         
-00000b30: 2020 2020 2020 205b 0d0a 2020 2020 2020         [..      
-00000b40: 2020 2020 2020 2020 2020 2020 2020 2266                "f
-00000b50: 6670 726f 6265 222c 0d0a 2020 2020 2020  fprobe",..      
-00000b60: 2020 2020 2020 2020 2020 2020 2020 222d                "-
-00000b70: 6c6f 676c 6576 656c 222c 0d0a 2020 2020  loglevel",..    
-00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b90: 222d 3122 2c0d 0a20 2020 2020 2020 2020  "-1",..         
-00000ba0: 2020 2020 2020 2020 2020 2022 2d68 6964             "-hid
-00000bb0: 655f 6261 6e6e 6572 222c 0d0a 2020 2020  e_banner",..    
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 222d 7368 6f77 5f65 6e74 7269 6573 222c  "-show_entries",
-00000be0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000bf0: 2020 2020 2020 2266 6f72 6d61 743d 6475        "format=du
-00000c00: 7261 7469 6f6e 222c 0d0a 2020 2020 2020  ration",..      
-00000c10: 2020 2020 2020 2020 2020 2020 2020 222d                "-
-00000c20: 6f66 222c 0d0a 2020 2020 2020 2020 2020  of",..          
-00000c30: 2020 2020 2020 2020 2020 2264 6566 6175            "defau
-00000c40: 6c74 3d6e 6f70 7269 6e74 5f77 7261 7070  lt=noprint_wrapp
-00000c50: 6572 733d 313a 6e6f 6b65 793d 3122 2c0d  ers=1:nokey=1",.
-00000c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c70: 2020 2020 2066 696c 655f 6e61 6d65 2c0d       file_name,.
-00000c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c90: 205d 2c0d 0a20 2020 2020 2020 2020 2020   ],..           
-00000ca0: 2020 2020 2075 6e69 7665 7273 616c 5f6e       universal_n
-00000cb0: 6577 6c69 6e65 733d 5472 7565 2c0d 0a20  ewlines=True,.. 
-00000cc0: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
-00000cd0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-00000ce0: 6e74 2866 6c6f 6174 286f 7574 7075 742e  nt(float(output.
-00000cf0: 7374 7269 7028 2929 202a 2031 3030 3029  strip()) * 1000)
-00000d00: 0d0a 2020 2020 6578 6365 7074 2045 7863  ..    except Exc
-00000d10: 6570 7469 6f6e 3a0d 0a20 2020 2020 2020  eption:..       
-00000d20: 2023 2054 4f44 4f3a 2061 6464 206c 6f67   # TODO: add log
-00000d30: 6769 6e67 0d0a 2020 2020 2020 2020 7265  ging..        re
-00000d40: 7475 726e 204e 6f6e 650d 0a0d 0a0d 0a64  turn None......d
-00000d50: 6566 205f 7573 6573 5f65 7272 6f72 5f6c  ef _uses_error_l
-00000d60: 6f67 6c65 7665 6c28 636d 643a 204c 6973  oglevel(cmd: Lis
-00000d70: 745b 7374 725d 2920 2d3e 2062 6f6f 6c3a  t[str]) -> bool:
-00000d80: 0d0a 2020 2020 7472 793a 0d0a 2020 2020  ..    try:..    
-00000d90: 2020 2020 6964 7820 3d20 636d 642e 696e      idx = cmd.in
-00000da0: 6465 7828 222d 6c6f 676c 6576 656c 2229  dex("-loglevel")
-00000db0: 0d0a 2020 2020 2020 2020 6966 2063 6d64  ..        if cmd
-00000dc0: 5b69 6478 202b 2031 5d20 3d3d 2022 6572  [idx + 1] == "er
-00000dd0: 726f 7222 3a0d 0a20 2020 2020 2020 2020  ror":..         
-00000de0: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
-00000df0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00000e00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000e10: 6e20 4661 6c73 650d 0a20 2020 2065 7863  n False..    exc
-00000e20: 6570 7420 5661 6c75 6545 7272 6f72 3a0d  ept ValueError:.
-00000e30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000e40: 4661 6c73 650d 0a0d 0a0d 0a63 6c61 7373  False......class
-00000e50: 2046 666d 7065 6750 726f 6772 6573 733a   FfmpegProgress:
-00000e60: 0d0a 2020 2020 4455 525f 5245 4745 5820  ..    DUR_REGEX 
-00000e70: 3d20 7265 2e63 6f6d 7069 6c65 280d 0a20  = re.compile(.. 
-00000e80: 2020 2020 2020 2072 2244 7572 6174 696f         r"Duratio
-00000e90: 6e3a 2028 3f50 3c68 6f75 723e 5c64 7b32  n: (?P<hour>\d{2
-00000ea0: 7d29 3a28 3f50 3c6d 696e 3e5c 647b 327d  }):(?P<min>\d{2}
-00000eb0: 293a 283f 503c 7365 633e 5c64 7b32 7d29  ):(?P<sec>\d{2})
-00000ec0: 5c2e 283f 503c 6d73 3e5c 647b 327d 2922  \.(?P<ms>\d{2})"
-00000ed0: 0d0a 2020 2020 290d 0a20 2020 2054 494d  ..    )..    TIM
-00000ee0: 455f 5245 4745 5820 3d20 7265 2e63 6f6d  E_REGEX = re.com
-00000ef0: 7069 6c65 280d 0a20 2020 2020 2020 2072  pile(..        r
-00000f00: 226f 7574 5f74 696d 653d 283f 503c 686f  "out_time=(?P<ho
-00000f10: 7572 3e5c 647b 327d 293a 283f 503c 6d69  ur>\d{2}):(?P<mi
-00000f20: 6e3e 5c64 7b32 7d29 3a28 3f50 3c73 6563  n>\d{2}):(?P<sec
-00000f30: 3e5c 647b 327d 295c 2e28 3f50 3c6d 733e  >\d{2})\.(?P<ms>
-00000f40: 5c64 7b32 7d29 220d 0a20 2020 2029 0d0a  \d{2})"..    )..
-00000f50: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-00000f60: 5f5f 2873 656c 662c 2063 6d64 3a20 4c69  __(self, cmd: Li
-00000f70: 7374 5b73 7472 5d2c 2064 7279 5f72 756e  st[str], dry_run
-00000f80: 3a20 626f 6f6c 203d 2046 616c 7365 2920  : bool = False) 
-00000f90: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
-00000fa0: 2020 2727 2749 6e69 7469 616c 697a 6520    '''Initialize 
-00000fb0: 7468 6520 4666 6d70 6567 5072 6f67 7265  the FfmpegProgre
-00000fc0: 7373 2063 6c61 7373 2e0d 0a0d 0a20 2020  ss class.....   
-00000fd0: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
-00000fe0: 2020 2020 2020 2020 636d 6420 284c 6973          cmd (Lis
-00000ff0: 745b 7374 725d 293a 2041 206c 6973 7420  t[str]): A list 
-00001000: 6f66 2063 6f6d 6d61 6e64 206c 696e 6520  of command line 
-00001010: 656c 656d 656e 7473 2c20 652e 672e 205b  elements, e.g. [
-00001020: 2266 666d 7065 6722 2c20 222d 6922 2c20  "ffmpeg", "-i", 
-00001030: 2e2e 2e5d 0d0a 2020 2020 2020 2020 2020  ...]..          
-00001040: 2020 6472 795f 7275 6e20 2862 6f6f 6c2c    dry_run (bool,
-00001050: 206f 7074 696f 6e61 6c29 3a20 4f6e 6c79   optional): Only
-00001060: 2073 686f 7720 7768 6174 2077 6f75 6c64   show what would
-00001070: 2062 6520 646f 6e65 2e20 4465 6661 756c   be done. Defaul
-00001080: 7473 2074 6f20 4661 6c73 652e 0d0a 2020  ts to False...  
-00001090: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
-000010a0: 2020 2073 656c 662e 636d 6420 3d20 636d     self.cmd = cm
-000010b0: 640d 0a20 2020 2020 2020 2073 656c 662e  d..        self.
-000010c0: 7374 6465 7272 3a20 556e 696f 6e5b 7374  stderr: Union[st
-000010d0: 722c 204e 6f6e 655d 203d 204e 6f6e 650d  r, None] = None.
-000010e0: 0a20 2020 2020 2020 2073 656c 662e 6472  .        self.dr
-000010f0: 795f 7275 6e20 3d20 6472 795f 7275 6e0d  y_run = dry_run.
-00001100: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
-00001110: 6f63 6573 733a 2041 6e79 203d 204e 6f6e  ocess: Any = Non
-00001120: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00001130: 7374 6465 7272 5f63 616c 6c62 6163 6b3a  stderr_callback:
-00001140: 2055 6e69 6f6e 5b43 616c 6c61 626c 655b   Union[Callable[
-00001150: 5b73 7472 5d2c 204e 6f6e 655d 2c20 4e6f  [str], None], No
-00001160: 6e65 5d20 3d20 4e6f 6e65 0d0a 2020 2020  ne] = None..    
-00001170: 2020 2020 6966 2073 7973 2e70 6c61 7466      if sys.platf
-00001180: 6f72 6d20 3d3d 2022 7769 6e33 3222 3a0d  orm == "win32":.
-00001190: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000011a0: 662e 6261 7365 5f70 6f70 656e 5f6b 7761  f.base_popen_kwa
-000011b0: 7267 7320 3d20 7b0d 0a20 2020 2020 2020  rgs = {..       
-000011c0: 2020 2020 2020 2020 2022 7374 6469 6e22           "stdin"
-000011d0: 3a20 7375 6270 726f 6365 7373 2e50 4950  : subprocess.PIP
-000011e0: 452c 2020 2320 4170 706c 7920 7374 6469  E,  # Apply stdi
-000011f0: 6e20 6973 6f6c 6174 696f 6e20 6279 2063  n isolation by c
-00001200: 7265 6174 696e 6720 7365 7061 7261 7465  reating separate
-00001210: 2070 6970 652e 0d0a 2020 2020 2020 2020   pipe...        
-00001220: 2020 2020 2020 2020 2273 7464 6f75 7422          "stdout"
-00001230: 3a20 7375 6270 726f 6365 7373 2e50 4950  : subprocess.PIP
-00001240: 452c 0d0a 2020 2020 2020 2020 2020 2020  E,..            
-00001250: 2020 2020 2273 7464 6572 7222 3a20 7375      "stderr": su
-00001260: 6270 726f 6365 7373 2e53 5444 4f55 542c  bprocess.STDOUT,
-00001270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001280: 2020 2275 6e69 7665 7273 616c 5f6e 6577    "universal_new
-00001290: 6c69 6e65 7322 3a20 4661 6c73 652c 0d0a  lines": False,..
-000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012b0: 2273 6865 6c6c 223a 2054 7275 652c 0d0a  "shell": True,..
-000012c0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-000012d0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000012e0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-000012f0: 6173 655f 706f 7065 6e5f 6b77 6172 6773  ase_popen_kwargs
-00001300: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
-00001310: 2020 2020 2020 2273 7464 696e 223a 2073        "stdin": s
-00001320: 7562 7072 6f63 6573 732e 5049 5045 2c20  ubprocess.PIPE, 
-00001330: 2023 2041 7070 6c79 2073 7464 696e 2069   # Apply stdin i
-00001340: 736f 6c61 7469 6f6e 2062 7920 6372 6561  solation by crea
-00001350: 7469 6e67 2073 6570 6172 6174 6520 7069  ting separate pi
-00001360: 7065 2e0d 0a20 2020 2020 2020 2020 2020  pe...           
-00001370: 2020 2020 2022 7374 646f 7574 223a 2073       "stdout": s
-00001380: 7562 7072 6f63 6573 732e 5049 5045 2c0d  ubprocess.PIPE,.
-00001390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000013a0: 2022 7374 6465 7272 223a 2073 7562 7072   "stderr": subpr
-000013b0: 6f63 6573 732e 5354 444f 5554 2c0d 0a20  ocess.STDOUT,.. 
-000013c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000013d0: 756e 6976 6572 7361 6c5f 6e65 776c 696e  universal_newlin
-000013e0: 6573 223a 2046 616c 7365 2c0d 0a20 2020  es": False,..   
-000013f0: 2020 2020 2020 2020 207d 0d0a 0d0a 2020           }....  
-00001400: 2020 6465 6620 7365 745f 7374 6465 7272    def set_stderr
-00001410: 5f63 616c 6c62 6163 6b28 7365 6c66 2c20  _callback(self, 
-00001420: 6361 6c6c 6261 636b 3a20 4361 6c6c 6162  callback: Callab
-00001430: 6c65 5b5b 7374 725d 2c20 4e6f 6e65 5d29  le[[str], None])
-00001440: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
-00001450: 2020 2027 2727 0d0a 2020 2020 2020 2020     '''..        
-00001460: 5365 7420 6120 6361 6c6c 6261 636b 2066  Set a callback f
-00001470: 756e 6374 696f 6e20 746f 2062 6520 6361  unction to be ca
-00001480: 6c6c 6564 206f 6e20 7374 6465 7272 206f  lled on stderr o
-00001490: 7574 7075 742e 0d0a 2020 2020 2020 2020  utput...        
-000014a0: 5468 6520 6361 6c6c 6261 636b 2066 756e  The callback fun
-000014b0: 6374 696f 6e20 6d75 7374 2061 6363 6570  ction must accep
-000014c0: 7420 6120 7369 6e67 6c65 2073 7472 696e  t a single strin
-000014d0: 6720 6172 6775 6d65 6e74 2e0d 0a20 2020  g argument...   
-000014e0: 2020 2020 204e 6f74 6520 7468 6174 2074       Note that t
-000014f0: 6869 7320 6973 2063 616c 6c65 6420 6f6e  his is called on
-00001500: 2065 7665 7279 206c 696e 6520 6f66 2073   every line of s
-00001510: 7464 6572 7220 6f75 7470 7574 2c20 736f  tderr output, so
-00001520: 2069 7420 6361 6e20 6265 2063 616c 6c65   it can be calle
-00001530: 6420 6120 6c6f 742e 0d0a 2020 2020 2020  d a lot...      
-00001540: 2020 416c 736f 206e 6f74 6520 7468 6174    Also note that
-00001550: 2073 7464 6f75 742f 7374 6465 7272 2061   stdout/stderr a
-00001560: 7265 206a 6f69 6e65 6420 696e 746f 206f  re joined into o
-00001570: 6e65 2073 7472 6561 6d2c 2073 6f20 796f  ne stream, so yo
-00001580: 7520 6d69 6768 7420 6765 7420 7374 646f  u might get stdo
-00001590: 7574 206f 7574 7075 7420 696e 2074 6865  ut output in the
-000015a0: 2063 616c 6c62 6163 6b2e 0d0a 0d0a 2020   callback.....  
-000015b0: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
-000015c0: 2020 2020 2020 2020 2063 616c 6c62 6163           callbac
-000015d0: 6b20 2843 616c 6c61 626c 655b 5b73 7472  k (Callable[[str
-000015e0: 5d2c 204e 6f6e 655d 293a 2041 2063 616c  ], None]): A cal
-000015f0: 6c62 6163 6b20 6675 6e63 7469 6f6e 2074  lback function t
-00001600: 6861 7420 6163 6365 7074 7320 6120 7369  hat accepts a si
-00001610: 6e67 6c65 2073 7472 696e 6720 6172 6775  ngle string argu
-00001620: 6d65 6e74 2e0d 0a20 2020 2020 2020 2027  ment...        '
-00001630: 2727 0d0a 2020 2020 2020 2020 6966 206e  ''..        if n
-00001640: 6f74 2063 616c 6c61 626c 6528 6361 6c6c  ot callable(call
-00001650: 6261 636b 2920 6f72 206c 656e 2863 616c  back) or len(cal
-00001660: 6c62 6163 6b2e 5f5f 636f 6465 5f5f 2e63  lback.__code__.c
-00001670: 6f5f 7661 726e 616d 6573 2920 213d 2031  o_varnames) != 1
-00001680: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00001690: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-000016a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000016b0: 2020 2243 616c 6c62 6163 6b20 6d75 7374    "Callback must
-000016c0: 2062 6520 6120 6675 6e63 7469 6f6e 2074   be a function t
-000016d0: 6861 7420 6163 6365 7074 7320 6f6e 6c79  hat accepts only
-000016e0: 206f 6e65 2061 7267 756d 656e 7422 0d0a   one argument"..
-000016f0: 2020 2020 2020 2020 2020 2020 290d 0a0d              )...
-00001700: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-00001710: 6465 7272 5f63 616c 6c62 6163 6b20 3d20  derr_callback = 
-00001720: 6361 6c6c 6261 636b 0d0a 0d0a 2020 2020  callback....    
-00001730: 6465 6620 7275 6e5f 636f 6d6d 616e 645f  def run_command_
-00001740: 7769 7468 5f70 726f 6772 6573 7328 0d0a  with_progress(..
-00001750: 2020 2020 2020 2020 7365 6c66 2c20 706f          self, po
-00001760: 7065 6e5f 6b77 6172 6773 3d4e 6f6e 652c  pen_kwargs=None,
-00001770: 2064 7572 6174 696f 6e5f 6f76 6572 7269   duration_overri
-00001780: 6465 3a20 556e 696f 6e5b 666c 6f61 742c  de: Union[float,
-00001790: 204e 6f6e 655d 203d 204e 6f6e 650d 0a20   None] = None.. 
-000017a0: 2020 2029 202d 3e20 4974 6572 6174 6f72     ) -> Iterator
-000017b0: 5b69 6e74 5d3a 0d0a 2020 2020 2020 2020  [int]:..        
-000017c0: 2727 270d 0a20 2020 2020 2020 2052 756e  '''..        Run
-000017d0: 2061 6e20 6666 6d70 6567 2063 6f6d 6d61   an ffmpeg comma
-000017e0: 6e64 2c20 7472 7969 6e67 2074 6f20 6361  nd, trying to ca
-000017f0: 7074 7572 6520 7468 6520 7072 6f63 6573  pture the proces
-00001800: 7320 6f75 7470 7574 2061 6e64 2063 616c  s output and cal
-00001810: 6375 6c61 7465 0d0a 2020 2020 2020 2020  culate..        
-00001820: 7468 6520 6475 7261 7469 6f6e 202f 2070  the duration / p
-00001830: 726f 6772 6573 732e 0d0a 2020 2020 2020  rogress...      
-00001840: 2020 5969 656c 6473 2074 6865 2070 726f    Yields the pro
-00001850: 6772 6573 7320 696e 2070 6572 6365 6e74  gress in percent
-00001860: 2e0d 0a0d 0a20 2020 2020 2020 2041 7267  .....        Arg
-00001870: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00001880: 706f 7065 6e5f 6b77 6172 6773 2028 6469  popen_kwargs (di
-00001890: 6374 2c20 6f70 7469 6f6e 616c 293a 2041  ct, optional): A
-000018a0: 2064 6963 7420 746f 2073 7065 6369 6679   dict to specify
-000018b0: 2065 7874 7261 2061 7267 756d 656e 7473   extra arguments
-000018c0: 2074 6f20 7468 6520 706f 7065 6e20 6361   to the popen ca
-000018d0: 6c6c 2c20 652e 672e 207b 2063 7265 6174  ll, e.g. { creat
-000018e0: 696f 6e66 6c61 6773 3a20 4352 4541 5445  ionflags: CREATE
-000018f0: 5f4e 4f5f 5749 4e44 4f57 207d 0d0a 2020  _NO_WINDOW }..  
-00001900: 2020 2020 2020 2020 2020 6475 7261 7469            durati
-00001910: 6f6e 5f6f 7665 7272 6964 6520 2866 6c6f  on_override (flo
-00001920: 6174 2c20 6f70 7469 6f6e 616c 293a 2054  at, optional): T
-00001930: 6865 2064 7572 6174 696f 6e20 696e 2073  he duration in s
-00001940: 6563 6f6e 6473 2e20 4966 206e 6f74 2073  econds. If not s
-00001950: 7065 6369 6669 6564 2c20 6974 2077 696c  pecified, it wil
-00001960: 6c20 6265 2063 616c 6375 6c61 7465 6420  l be calculated 
-00001970: 6672 6f6d 2074 6865 2066 666d 7065 6720  from the ffmpeg 
-00001980: 6f75 7470 7574 2e0d 0a0d 0a20 2020 2020  output.....     
-00001990: 2020 2052 6169 7365 733a 0d0a 2020 2020     Raises:..    
-000019a0: 2020 2020 2020 2020 5275 6e74 696d 6545          RuntimeE
-000019b0: 7272 6f72 3a20 4966 2074 6865 2063 6f6d  rror: If the com
-000019c0: 6d61 6e64 2066 6169 6c73 2c20 616e 2065  mand fails, an e
-000019d0: 7863 6570 7469 6f6e 2069 7320 7261 6973  xception is rais
-000019e0: 6564 2e0d 0a0d 0a20 2020 2020 2020 2059  ed.....        Y
-000019f0: 6965 6c64 733a 0d0a 2020 2020 2020 2020  ields:..        
-00001a00: 2020 2020 4974 6572 6174 6f72 5b69 6e74      Iterator[int
-00001a10: 5d3a 2041 2067 656e 6572 6174 6f72 2074  ]: A generator t
-00001a20: 6861 7420 7969 656c 6473 2074 6865 2070  hat yields the p
-00001a30: 726f 6772 6573 7320 696e 2070 6572 6365  rogress in perce
-00001a40: 6e74 2e0d 0a20 2020 2020 2020 2027 2727  nt...        '''
-00001a50: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00001a60: 662e 6472 795f 7275 6e3a 0d0a 2020 2020  f.dry_run:..    
-00001a70: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00001a80: 656c 662e 636d 640d 0a0d 0a20 2020 2020  elf.cmd....     
-00001a90: 2020 2074 6f74 616c 5f64 7572 3a20 556e     total_dur: Un
-00001aa0: 696f 6e5b 4e6f 6e65 2c20 696e 745d 203d  ion[None, int] =
-00001ab0: 204e 6f6e 650d 0a20 2020 2020 2020 2069   None..        i
-00001ac0: 6620 5f75 7365 735f 6572 726f 725f 6c6f  f _uses_error_lo
-00001ad0: 676c 6576 656c 2873 656c 662e 636d 6429  glevel(self.cmd)
-00001ae0: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
-00001af0: 6f74 616c 5f64 7572 203d 205f 7072 6f62  otal_dur = _prob
-00001b00: 655f 6475 7261 7469 6f6e 2873 656c 662e  e_duration(self.
-00001b10: 636d 6429 0d0a 0d0a 2020 2020 2020 2020  cmd)....        
-00001b20: 636d 645f 7769 7468 5f70 726f 6772 6573  cmd_with_progres
-00001b30: 7320 3d20 280d 0a20 2020 2020 2020 2020  s = (..         
-00001b40: 2020 205b 7365 6c66 2e63 6d64 5b30 5d5d     [self.cmd[0]]
-00001b50: 202b 205b 222d 7072 6f67 7265 7373 222c   + ["-progress",
-00001b60: 2022 2d22 2c20 222d 6e6f 7374 6174 7322   "-", "-nostats"
-00001b70: 5d20 2b20 7365 6c66 2e63 6d64 5b31 3a5d  ] + self.cmd[1:]
-00001b80: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
-00001b90: 2020 2020 2020 2073 7464 6572 7220 3d20         stderr = 
-00001ba0: 5b5d 0d0a 2020 2020 2020 2020 6261 7365  []..        base
-00001bb0: 5f70 6f70 656e 5f6b 7761 7267 7320 3d20  _popen_kwargs = 
-00001bc0: 7365 6c66 2e62 6173 655f 706f 7065 6e5f  self.base_popen_
-00001bd0: 6b77 6172 6773 2e63 6f70 7928 290d 0a20  kwargs.copy().. 
-00001be0: 2020 2020 2020 2069 6620 706f 7065 6e5f         if popen_
-00001bf0: 6b77 6172 6773 2069 7320 6e6f 7420 4e6f  kwargs is not No
-00001c00: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00001c10: 2062 6173 655f 706f 7065 6e5f 6b77 6172   base_popen_kwar
-00001c20: 6773 2e75 7064 6174 6528 706f 7065 6e5f  gs.update(popen_
-00001c30: 6b77 6172 6773 290d 0a0d 0a20 2020 2020  kwargs)....     
-00001c40: 2020 2069 6620 7379 732e 706c 6174 666f     if sys.platfo
-00001c50: 726d 203d 3d20 2277 696e 6433 3222 3a0d  rm == "wind32":.
-00001c60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00001c70: 662e 7072 6f63 6573 7320 3d20 7375 6270  f.process = subp
-00001c80: 726f 6365 7373 2e50 6f70 656e 280d 0a20  rocess.Popen(.. 
-00001c90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001ca0: 6d64 5f77 6974 685f 7072 6f67 7265 7373  md_with_progress
-00001cb0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001cc0: 2020 202a 2a62 6173 655f 706f 7065 6e5f     **base_popen_
-00001cd0: 6b77 6172 6773 2c0d 0a20 2020 2020 2020  kwargs,..       
-00001ce0: 2020 2020 2020 2020 2063 7265 6174 696f           creatio
-00001cf0: 6e66 6c61 6773 3d73 7562 7072 6f63 6573  nflags=subproces
-00001d00: 732e 4352 4541 5445 5f4e 4f5f 5749 4e44  s.CREATE_NO_WIND
-00001d10: 4f57 2c0d 0a20 2020 2020 2020 2020 2020  OW,..           
-00001d20: 2029 2020 2320 7479 7065 3a20 6967 6e6f   )  # type: igno
-00001d30: 7265 0d0a 2020 2020 2020 2020 656c 7365  re..        else
-00001d40: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00001d50: 656c 662e 7072 6f63 6573 7320 3d20 7375  elf.process = su
-00001d60: 6270 726f 6365 7373 2e50 6f70 656e 280d  bprocess.Popen(.
-00001d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001d80: 2063 6d64 5f77 6974 685f 7072 6f67 7265   cmd_with_progre
-00001d90: 7373 2c0d 0a20 2020 2020 2020 2020 2020  ss,..           
-00001da0: 2020 2020 202a 2a62 6173 655f 706f 7065       **base_pope
-00001db0: 6e5f 6b77 6172 6773 2c0d 0a20 2020 2020  n_kwargs,..     
-00001dc0: 2020 2020 2020 2029 2020 2320 7479 7065         )  # type
-00001dd0: 3a20 6967 6e6f 7265 0d0a 0d0a 2020 2020  : ignore....    
-00001de0: 2020 2020 7969 656c 6420 300d 0a0d 0a20      yield 0.... 
-00001df0: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
-00001e00: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00001e10: 6966 2073 656c 662e 7072 6f63 6573 732e  if self.process.
-00001e20: 7374 646f 7574 2069 7320 4e6f 6e65 3a0d  stdout is None:.
+000002d0: 2e36 220d 0a0d 0a23 3d3d 3d3d 3d3d 3d3d  .6"....#========
+000002e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000002f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000300: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000310: 2066 666d 7065 675f 7072 6f67 7265 7373   ffmpeg_progress
+00000320: 5f79 6965 6c64 203d 3d3d 3d3d 3d3d 3d3d  _yield =========
+00000330: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000340: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d23  ===============#
+00000360: 0d0a 0d0a 696d 706f 7274 2072 650d 0a23  ....import re..#
+00000370: 696d 706f 7274 2073 7562 7072 6f63 6573  import subproces
+00000380: 730d 0a66 726f 6d20 7479 7069 6e67 2069  s..from typing i
+00000390: 6d70 6f72 7420 416e 792c 2043 616c 6c61  mport Any, Calla
+000003a0: 626c 652c 2049 7465 7261 746f 722c 204c  ble, Iterator, L
+000003b0: 6973 742c 204f 7074 696f 6e61 6c2c 2055  ist, Optional, U
+000003c0: 6e69 6f6e 0d0a 0d0a 0d0a 6465 6620 746f  nion......def to
+000003d0: 5f6d 7328 2a2a 6b77 6172 6773 3a20 556e  _ms(**kwargs: Un
+000003e0: 696f 6e5b 666c 6f61 742c 2069 6e74 2c20  ion[float, int, 
+000003f0: 7374 725d 2920 2d3e 2069 6e74 3a0d 0a20  str]) -> int:.. 
+00000400: 2020 2068 6f75 7220 3d20 696e 7428 6b77     hour = int(kw
+00000410: 6172 6773 2e67 6574 2822 686f 7572 222c  args.get("hour",
+00000420: 2030 2929 0d0a 2020 2020 6d69 6e75 7465   0))..    minute
+00000430: 203d 2069 6e74 286b 7761 7267 732e 6765   = int(kwargs.ge
+00000440: 7428 226d 696e 222c 2030 2929 0d0a 2020  t("min", 0))..  
+00000450: 2020 7365 6320 3d20 696e 7428 6b77 6172    sec = int(kwar
+00000460: 6773 2e67 6574 2822 7365 6322 2c20 3029  gs.get("sec", 0)
+00000470: 290d 0a20 2020 206d 7320 3d20 696e 7428  )..    ms = int(
+00000480: 6b77 6172 6773 2e67 6574 2822 6d73 222c  kwargs.get("ms",
+00000490: 2030 2929 0d0a 0d0a 2020 2020 7265 7475   0))....    retu
+000004a0: 726e 2028 686f 7572 202a 2036 3020 2a20  rn (hour * 60 * 
+000004b0: 3630 202a 2031 3030 3029 202b 2028 6d69  60 * 1000) + (mi
+000004c0: 6e75 7465 202a 2036 3020 2a20 3130 3030  nute * 60 * 1000
+000004d0: 2920 2b20 2873 6563 202a 2031 3030 3029  ) + (sec * 1000)
+000004e0: 202b 206d 730d 0a0d 0a0d 0a64 6566 205f   + ms......def _
+000004f0: 7072 6f62 655f 6475 7261 7469 6f6e 2863  probe_duration(c
+00000500: 6d64 3a20 4c69 7374 5b73 7472 5d29 202d  md: List[str]) -
+00000510: 3e20 4f70 7469 6f6e 616c 5b69 6e74 5d3a  > Optional[int]:
+00000520: 0d0a 2020 2020 2727 270d 0a20 2020 2047  ..    '''..    G
+00000530: 6574 2074 6865 2064 7572 6174 696f 6e20  et the duration 
+00000540: 7669 6120 6666 7072 6f62 6520 6672 6f6d  via ffprobe from
+00000550: 2069 6e70 7574 206d 6564 6961 2066 696c   input media fil
+00000560: 650d 0a20 2020 2069 6e20 6361 7365 2066  e..    in case f
+00000570: 666d 7065 6720 7761 7320 7275 6e20 7769  fmpeg was run wi
+00000580: 7468 206c 6f67 6c65 7665 6c3d 6572 726f  th loglevel=erro
+00000590: 722e 0d0a 0d0a 2020 2020 4172 6773 3a0d  r.....    Args:.
+000005a0: 0a20 2020 2020 2020 2063 6d64 2028 4c69  .        cmd (Li
+000005b0: 7374 5b73 7472 5d29 3a20 4120 6c69 7374  st[str]): A list
+000005c0: 206f 6620 636f 6d6d 616e 6420 6c69 6e65   of command line
+000005d0: 2065 6c65 6d65 6e74 732c 2065 2e67 2e20   elements, e.g. 
+000005e0: 5b22 6666 6d70 6567 222c 2022 2d69 222c  ["ffmpeg", "-i",
+000005f0: 202e 2e2e 5d0d 0a0d 0a20 2020 2052 6574   ...]....    Ret
+00000600: 7572 6e73 3a0d 0a20 2020 2020 2020 204f  urns:..        O
+00000610: 7074 696f 6e61 6c5b 696e 745d 3a20 5468  ptional[int]: Th
+00000620: 6520 6475 7261 7469 6f6e 2069 6e20 6d69  e duration in mi
+00000630: 6c6c 6973 6563 6f6e 6473 2e0d 0a20 2020  lliseconds...   
+00000640: 2027 2727 0d0a 0d0a 2020 2020 6465 6620   '''....    def 
+00000650: 5f67 6574 5f66 696c 655f 6e61 6d65 2863  _get_file_name(c
+00000660: 6d64 3a20 4c69 7374 5b73 7472 5d29 202d  md: List[str]) -
+00000670: 3e20 4f70 7469 6f6e 616c 5b73 7472 5d3a  > Optional[str]:
+00000680: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
+00000690: 2020 2020 2020 2020 2020 2020 6964 7820              idx 
+000006a0: 3d20 636d 642e 696e 6465 7828 222d 6922  = cmd.index("-i"
+000006b0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+000006c0: 6574 7572 6e20 636d 645b 6964 7820 2b20  eturn cmd[idx + 
+000006d0: 315d 0d0a 2020 2020 2020 2020 6578 6365  1]..        exce
+000006e0: 7074 2056 616c 7565 4572 726f 723a 0d0a  pt ValueError:..
+000006f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000700: 726e 204e 6f6e 650d 0a0d 0a20 2020 2066  rn None....    f
+00000710: 696c 655f 6e61 6d65 203d 205f 6765 745f  ile_name = _get_
+00000720: 6669 6c65 5f6e 616d 6528 636d 6429 0d0a  file_name(cmd)..
+00000730: 2020 2020 6966 2066 696c 655f 6e61 6d65      if file_name
+00000740: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00000750: 2020 2072 6574 7572 6e20 4e6f 6e65 0d0a     return None..
+00000760: 0d0a 2020 2020 7472 793a 0d0a 2020 2020  ..    try:..    
+00000770: 2020 2020 6966 2073 7973 2e70 6c61 7466      if sys.platf
+00000780: 6f72 6d20 3d3d 2022 7769 6e33 3222 3a0d  orm == "win32":.
+00000790: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+000007a0: 7075 7420 3d20 7375 6270 726f 6365 7373  put = subprocess
+000007b0: 2e63 6865 636b 5f6f 7574 7075 7428 0d0a  .check_output(..
+000007c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007d0: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+000007e0: 2020 2020 2020 2022 6666 7072 6f62 6522         "ffprobe"
+000007f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000800: 2020 2020 2020 2022 2d6c 6f67 6c65 7665         "-logleve
+00000810: 6c22 2c0d 0a20 2020 2020 2020 2020 2020  l",..           
+00000820: 2020 2020 2020 2020 2022 2d31 222c 0d0a           "-1",..
+00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000840: 2020 2020 222d 6869 6465 5f62 616e 6e65      "-hide_banne
+00000850: 7222 2c0d 0a20 2020 2020 2020 2020 2020  r",..           
+00000860: 2020 2020 2020 2020 2022 2d73 686f 775f           "-show_
+00000870: 656e 7472 6965 7322 2c0d 0a20 2020 2020  entries",..     
+00000880: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000890: 666f 726d 6174 3d64 7572 6174 696f 6e22  format=duration"
+000008a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000008b0: 2020 2020 2020 2022 2d6f 6622 2c0d 0a20         "-of",.. 
+000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008d0: 2020 2022 6465 6661 756c 743d 6e6f 7072     "default=nopr
+000008e0: 696e 745f 7772 6170 7065 7273 3d31 3a6e  int_wrappers=1:n
+000008f0: 6f6b 6579 3d31 222c 0d0a 2020 2020 2020  okey=1",..      
+00000900: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00000910: 6c65 5f6e 616d 652c 0d0a 2020 2020 2020  le_name,..      
+00000920: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
+00000930: 2020 2020 2020 2020 2020 2020 2020 756e                un
+00000940: 6976 6572 7361 6c5f 6e65 776c 696e 6573  iversal_newlines
+00000950: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00000960: 2020 2020 2020 2020 6372 6561 7469 6f6e          creation
+00000970: 666c 6167 733d 7375 6270 726f 6365 7373  flags=subprocess
+00000980: 2e43 5245 4154 455f 4e4f 5f57 494e 444f  .CREATE_NO_WINDO
+00000990: 572c 0d0a 2020 2020 2020 2020 2020 2020  W,..            
+000009a0: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
+000009b0: 0d0a 2020 2020 2020 2020 2020 2020 6f75  ..            ou
+000009c0: 7470 7574 203d 2073 7562 7072 6f63 6573  tput = subproces
+000009d0: 732e 6368 6563 6b5f 6f75 7470 7574 280d  s.check_output(.
+000009e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000009f0: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+00000a00: 2020 2020 2020 2020 2266 6670 726f 6265          "ffprobe
+00000a10: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000a20: 2020 2020 2020 2020 222d 6c6f 676c 6576          "-loglev
+00000a30: 656c 222c 0d0a 2020 2020 2020 2020 2020  el",..          
+00000a40: 2020 2020 2020 2020 2020 222d 3122 2c0d            "-1",.
+00000a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a60: 2020 2020 2022 2d68 6964 655f 6261 6e6e       "-hide_bann
+00000a70: 6572 222c 0d0a 2020 2020 2020 2020 2020  er",..          
+00000a80: 2020 2020 2020 2020 2020 222d 7368 6f77            "-show
+00000a90: 5f65 6e74 7269 6573 222c 0d0a 2020 2020  _entries",..    
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ab0: 2266 6f72 6d61 743d 6475 7261 7469 6f6e  "format=duration
+00000ac0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000ad0: 2020 2020 2020 2020 222d 6f66 222c 0d0a          "-of",..
+00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000af0: 2020 2020 2264 6566 6175 6c74 3d6e 6f70      "default=nop
+00000b00: 7269 6e74 5f77 7261 7070 6572 733d 313a  rint_wrappers=1:
+00000b10: 6e6f 6b65 793d 3122 2c0d 0a20 2020 2020  nokey=1",..     
+00000b20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00000b30: 696c 655f 6e61 6d65 2c0d 0a20 2020 2020  ile_name,..     
+00000b40: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
+00000b50: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00000b60: 6e69 7665 7273 616c 5f6e 6577 6c69 6e65  niversal_newline
+00000b70: 733d 5472 7565 2c0d 0a20 2020 2020 2020  s=True,..       
+00000b80: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
+00000b90: 2020 7265 7475 726e 2069 6e74 2866 6c6f    return int(flo
+00000ba0: 6174 286f 7574 7075 742e 7374 7269 7028  at(output.strip(
+00000bb0: 2929 202a 2031 3030 3029 0d0a 2020 2020  )) * 1000)..    
+00000bc0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00000bd0: 3a0d 0a20 2020 2020 2020 2023 2054 4f44  :..        # TOD
+00000be0: 4f3a 2061 6464 206c 6f67 6769 6e67 0d0a  O: add logging..
+00000bf0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00000c00: 6f6e 650d 0a0d 0a0d 0a64 6566 205f 7573  one......def _us
+00000c10: 6573 5f65 7272 6f72 5f6c 6f67 6c65 7665  es_error_logleve
+00000c20: 6c28 636d 643a 204c 6973 745b 7374 725d  l(cmd: List[str]
+00000c30: 2920 2d3e 2062 6f6f 6c3a 0d0a 2020 2020  ) -> bool:..    
+00000c40: 7472 793a 0d0a 2020 2020 2020 2020 6964  try:..        id
+00000c50: 7820 3d20 636d 642e 696e 6465 7828 222d  x = cmd.index("-
+00000c60: 6c6f 676c 6576 656c 2229 0d0a 2020 2020  loglevel")..    
+00000c70: 2020 2020 6966 2063 6d64 5b69 6478 202b      if cmd[idx +
+00000c80: 2031 5d20 3d3d 2022 6572 726f 7222 3a0d   1] == "error":.
+00000c90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00000ca0: 7572 6e20 5472 7565 0d0a 2020 2020 2020  urn True..      
+00000cb0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00000cc0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00000cd0: 650d 0a20 2020 2065 7863 6570 7420 5661  e..    except Va
+00000ce0: 6c75 6545 7272 6f72 3a0d 0a20 2020 2020  lueError:..     
+00000cf0: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
+00000d00: 0a0d 0a0d 0a63 6c61 7373 2046 666d 7065  .....class Ffmpe
+00000d10: 6750 726f 6772 6573 733a 0d0a 2020 2020  gProgress:..    
+00000d20: 4455 525f 5245 4745 5820 3d20 7265 2e63  DUR_REGEX = re.c
+00000d30: 6f6d 7069 6c65 280d 0a20 2020 2020 2020  ompile(..       
+00000d40: 2072 2244 7572 6174 696f 6e3a 2028 3f50   r"Duration: (?P
+00000d50: 3c68 6f75 723e 5c64 7b32 7d29 3a28 3f50  <hour>\d{2}):(?P
+00000d60: 3c6d 696e 3e5c 647b 327d 293a 283f 503c  <min>\d{2}):(?P<
+00000d70: 7365 633e 5c64 7b32 7d29 5c2e 283f 503c  sec>\d{2})\.(?P<
+00000d80: 6d73 3e5c 647b 327d 2922 0d0a 2020 2020  ms>\d{2})"..    
+00000d90: 290d 0a20 2020 2054 494d 455f 5245 4745  )..    TIME_REGE
+00000da0: 5820 3d20 7265 2e63 6f6d 7069 6c65 280d  X = re.compile(.
+00000db0: 0a20 2020 2020 2020 2072 226f 7574 5f74  .        r"out_t
+00000dc0: 696d 653d 283f 503c 686f 7572 3e5c 647b  ime=(?P<hour>\d{
+00000dd0: 327d 293a 283f 503c 6d69 6e3e 5c64 7b32  2}):(?P<min>\d{2
+00000de0: 7d29 3a28 3f50 3c73 6563 3e5c 647b 327d  }):(?P<sec>\d{2}
+00000df0: 295c 2e28 3f50 3c6d 733e 5c64 7b32 7d29  )\.(?P<ms>\d{2})
+00000e00: 220d 0a20 2020 2029 0d0a 0d0a 2020 2020  "..    )....    
+00000e10: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00000e20: 662c 2063 6d64 3a20 4c69 7374 5b73 7472  f, cmd: List[str
+00000e30: 5d2c 2064 7279 5f72 756e 3a20 626f 6f6c  ], dry_run: bool
+00000e40: 203d 2046 616c 7365 2920 2d3e 204e 6f6e   = False) -> Non
+00000e50: 653a 0d0a 2020 2020 2020 2020 2727 2749  e:..        '''I
+00000e60: 6e69 7469 616c 697a 6520 7468 6520 4666  nitialize the Ff
+00000e70: 6d70 6567 5072 6f67 7265 7373 2063 6c61  mpegProgress cla
+00000e80: 7373 2e0d 0a0d 0a20 2020 2020 2020 2041  ss.....        A
+00000e90: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
+00000ea0: 2020 636d 6420 284c 6973 745b 7374 725d    cmd (List[str]
+00000eb0: 293a 2041 206c 6973 7420 6f66 2063 6f6d  ): A list of com
+00000ec0: 6d61 6e64 206c 696e 6520 656c 656d 656e  mand line elemen
+00000ed0: 7473 2c20 652e 672e 205b 2266 666d 7065  ts, e.g. ["ffmpe
+00000ee0: 6722 2c20 222d 6922 2c20 2e2e 2e5d 0d0a  g", "-i", ...]..
+00000ef0: 2020 2020 2020 2020 2020 2020 6472 795f              dry_
+00000f00: 7275 6e20 2862 6f6f 6c2c 206f 7074 696f  run (bool, optio
+00000f10: 6e61 6c29 3a20 4f6e 6c79 2073 686f 7720  nal): Only show 
+00000f20: 7768 6174 2077 6f75 6c64 2062 6520 646f  what would be do
+00000f30: 6e65 2e20 4465 6661 756c 7473 2074 6f20  ne. Defaults to 
+00000f40: 4661 6c73 652e 0d0a 2020 2020 2020 2020  False...        
+00000f50: 2727 270d 0a20 2020 2020 2020 2073 656c  '''..        sel
+00000f60: 662e 636d 6420 3d20 636d 640d 0a20 2020  f.cmd = cmd..   
+00000f70: 2020 2020 2073 656c 662e 7374 6465 7272       self.stderr
+00000f80: 3a20 556e 696f 6e5b 7374 722c 204e 6f6e  : Union[str, Non
+00000f90: 655d 203d 204e 6f6e 650d 0a20 2020 2020  e] = None..     
+00000fa0: 2020 2073 656c 662e 6472 795f 7275 6e20     self.dry_run 
+00000fb0: 3d20 6472 795f 7275 6e0d 0a20 2020 2020  = dry_run..     
+00000fc0: 2020 2073 656c 662e 7072 6f63 6573 733a     self.process:
+00000fd0: 2041 6e79 203d 204e 6f6e 650d 0a20 2020   Any = None..   
+00000fe0: 2020 2020 2073 656c 662e 7374 6465 7272       self.stderr
+00000ff0: 5f63 616c 6c62 6163 6b3a 2055 6e69 6f6e  _callback: Union
+00001000: 5b43 616c 6c61 626c 655b 5b73 7472 5d2c  [Callable[[str],
+00001010: 204e 6f6e 655d 2c20 4e6f 6e65 5d20 3d20   None], None] = 
+00001020: 4e6f 6e65 0d0a 2020 2020 2020 2020 6966  None..        if
+00001030: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
+00001040: 2022 7769 6e33 3222 3a0d 0a20 2020 2020   "win32":..     
+00001050: 2020 2020 2020 2073 656c 662e 6261 7365         self.base
+00001060: 5f70 6f70 656e 5f6b 7761 7267 7320 3d20  _popen_kwargs = 
+00001070: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+00001080: 2020 2022 7374 6469 6e22 3a20 7375 6270     "stdin": subp
+00001090: 726f 6365 7373 2e50 4950 452c 2020 2320  rocess.PIPE,  # 
+000010a0: 4170 706c 7920 7374 6469 6e20 6973 6f6c  Apply stdin isol
+000010b0: 6174 696f 6e20 6279 2063 7265 6174 696e  ation by creatin
+000010c0: 6720 7365 7061 7261 7465 2070 6970 652e  g separate pipe.
+000010d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000010e0: 2020 2273 7464 6f75 7422 3a20 7375 6270    "stdout": subp
+000010f0: 726f 6365 7373 2e50 4950 452c 0d0a 2020  rocess.PIPE,..  
+00001100: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00001110: 7464 6572 7222 3a20 7375 6270 726f 6365  tderr": subproce
+00001120: 7373 2e53 5444 4f55 542c 0d0a 2020 2020  ss.STDOUT,..    
+00001130: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
+00001140: 7665 7273 616c 5f6e 6577 6c69 6e65 7322  versal_newlines"
+00001150: 3a20 4661 6c73 652c 0d0a 2020 2020 2020  : False,..      
+00001160: 2020 2020 2020 2020 2020 2273 6865 6c6c            "shell
+00001170: 223a 2054 7275 652c 0d0a 2020 2020 2020  ": True,..      
+00001180: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
+00001190: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+000011a0: 2020 2020 7365 6c66 2e62 6173 655f 706f      self.base_po
+000011b0: 7065 6e5f 6b77 6172 6773 203d 207b 0d0a  pen_kwargs = {..
+000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011d0: 2273 7464 696e 223a 2073 7562 7072 6f63  "stdin": subproc
+000011e0: 6573 732e 5049 5045 2c20 2023 2041 7070  ess.PIPE,  # App
+000011f0: 6c79 2073 7464 696e 2069 736f 6c61 7469  ly stdin isolati
+00001200: 6f6e 2062 7920 6372 6561 7469 6e67 2073  on by creating s
+00001210: 6570 6172 6174 6520 7069 7065 2e0d 0a20  eparate pipe... 
+00001220: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001230: 7374 646f 7574 223a 2073 7562 7072 6f63  stdout": subproc
+00001240: 6573 732e 5049 5045 2c0d 0a20 2020 2020  ess.PIPE,..     
+00001250: 2020 2020 2020 2020 2020 2022 7374 6465             "stde
+00001260: 7272 223a 2073 7562 7072 6f63 6573 732e  rr": subprocess.
+00001270: 5354 444f 5554 2c0d 0a20 2020 2020 2020  STDOUT,..       
+00001280: 2020 2020 2020 2020 2022 756e 6976 6572           "univer
+00001290: 7361 6c5f 6e65 776c 696e 6573 223a 2046  sal_newlines": F
+000012a0: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+000012b0: 2020 207d 0d0a 0d0a 2020 2020 6465 6620     }....    def 
+000012c0: 7365 745f 7374 6465 7272 5f63 616c 6c62  set_stderr_callb
+000012d0: 6163 6b28 7365 6c66 2c20 6361 6c6c 6261  ack(self, callba
+000012e0: 636b 3a20 4361 6c6c 6162 6c65 5b5b 7374  ck: Callable[[st
+000012f0: 725d 2c20 4e6f 6e65 5d29 202d 3e20 4e6f  r], None]) -> No
+00001300: 6e65 3a0d 0a20 2020 2020 2020 2027 2727  ne:..        '''
+00001310: 0d0a 2020 2020 2020 2020 5365 7420 6120  ..        Set a 
+00001320: 6361 6c6c 6261 636b 2066 756e 6374 696f  callback functio
+00001330: 6e20 746f 2062 6520 6361 6c6c 6564 206f  n to be called o
+00001340: 6e20 7374 6465 7272 206f 7574 7075 742e  n stderr output.
+00001350: 0d0a 2020 2020 2020 2020 5468 6520 6361  ..        The ca
+00001360: 6c6c 6261 636b 2066 756e 6374 696f 6e20  llback function 
+00001370: 6d75 7374 2061 6363 6570 7420 6120 7369  must accept a si
+00001380: 6e67 6c65 2073 7472 696e 6720 6172 6775  ngle string argu
+00001390: 6d65 6e74 2e0d 0a20 2020 2020 2020 204e  ment...        N
+000013a0: 6f74 6520 7468 6174 2074 6869 7320 6973  ote that this is
+000013b0: 2063 616c 6c65 6420 6f6e 2065 7665 7279   called on every
+000013c0: 206c 696e 6520 6f66 2073 7464 6572 7220   line of stderr 
+000013d0: 6f75 7470 7574 2c20 736f 2069 7420 6361  output, so it ca
+000013e0: 6e20 6265 2063 616c 6c65 6420 6120 6c6f  n be called a lo
+000013f0: 742e 0d0a 2020 2020 2020 2020 416c 736f  t...        Also
+00001400: 206e 6f74 6520 7468 6174 2073 7464 6f75   note that stdou
+00001410: 742f 7374 6465 7272 2061 7265 206a 6f69  t/stderr are joi
+00001420: 6e65 6420 696e 746f 206f 6e65 2073 7472  ned into one str
+00001430: 6561 6d2c 2073 6f20 796f 7520 6d69 6768  eam, so you migh
+00001440: 7420 6765 7420 7374 646f 7574 206f 7574  t get stdout out
+00001450: 7075 7420 696e 2074 6865 2063 616c 6c62  put in the callb
+00001460: 6163 6b2e 0d0a 0d0a 2020 2020 2020 2020  ack.....        
+00001470: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
+00001480: 2020 2063 616c 6c62 6163 6b20 2843 616c     callback (Cal
+00001490: 6c61 626c 655b 5b73 7472 5d2c 204e 6f6e  lable[[str], Non
+000014a0: 655d 293a 2041 2063 616c 6c62 6163 6b20  e]): A callback 
+000014b0: 6675 6e63 7469 6f6e 2074 6861 7420 6163  function that ac
+000014c0: 6365 7074 7320 6120 7369 6e67 6c65 2073  cepts a single s
+000014d0: 7472 696e 6720 6172 6775 6d65 6e74 2e0d  tring argument..
+000014e0: 0a20 2020 2020 2020 2027 2727 0d0a 2020  .        '''..  
+000014f0: 2020 2020 2020 6966 206e 6f74 2063 616c        if not cal
+00001500: 6c61 626c 6528 6361 6c6c 6261 636b 2920  lable(callback) 
+00001510: 6f72 206c 656e 2863 616c 6c62 6163 6b2e  or len(callback.
+00001520: 5f5f 636f 6465 5f5f 2e63 6f5f 7661 726e  __code__.co_varn
+00001530: 616d 6573 2920 213d 2031 3a0d 0a20 2020  ames) != 1:..   
+00001540: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00001550: 616c 7565 4572 726f 7228 0d0a 2020 2020  alueError(..    
+00001560: 2020 2020 2020 2020 2020 2020 2243 616c              "Cal
+00001570: 6c62 6163 6b20 6d75 7374 2062 6520 6120  lback must be a 
+00001580: 6675 6e63 7469 6f6e 2074 6861 7420 6163  function that ac
+00001590: 6365 7074 7320 6f6e 6c79 206f 6e65 2061  cepts only one a
+000015a0: 7267 756d 656e 7422 0d0a 2020 2020 2020  rgument"..      
+000015b0: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
+000015c0: 2020 2073 656c 662e 7374 6465 7272 5f63     self.stderr_c
+000015d0: 616c 6c62 6163 6b20 3d20 6361 6c6c 6261  allback = callba
+000015e0: 636b 0d0a 0d0a 2020 2020 6465 6620 7275  ck....    def ru
+000015f0: 6e5f 636f 6d6d 616e 645f 7769 7468 5f70  n_command_with_p
+00001600: 726f 6772 6573 7328 0d0a 2020 2020 2020  rogress(..      
+00001610: 2020 7365 6c66 2c20 706f 7065 6e5f 6b77    self, popen_kw
+00001620: 6172 6773 3d4e 6f6e 652c 2064 7572 6174  args=None, durat
+00001630: 696f 6e5f 6f76 6572 7269 6465 3a20 556e  ion_override: Un
+00001640: 696f 6e5b 666c 6f61 742c 204e 6f6e 655d  ion[float, None]
+00001650: 203d 204e 6f6e 650d 0a20 2020 2029 202d   = None..    ) -
+00001660: 3e20 4974 6572 6174 6f72 5b69 6e74 5d3a  > Iterator[int]:
+00001670: 0d0a 2020 2020 2020 2020 2727 270d 0a20  ..        '''.. 
+00001680: 2020 2020 2020 2052 756e 2061 6e20 6666         Run an ff
+00001690: 6d70 6567 2063 6f6d 6d61 6e64 2c20 7472  mpeg command, tr
+000016a0: 7969 6e67 2074 6f20 6361 7074 7572 6520  ying to capture 
+000016b0: 7468 6520 7072 6f63 6573 7320 6f75 7470  the process outp
+000016c0: 7574 2061 6e64 2063 616c 6375 6c61 7465  ut and calculate
+000016d0: 0d0a 2020 2020 2020 2020 7468 6520 6475  ..        the du
+000016e0: 7261 7469 6f6e 202f 2070 726f 6772 6573  ration / progres
+000016f0: 732e 0d0a 2020 2020 2020 2020 5969 656c  s...        Yiel
+00001700: 6473 2074 6865 2070 726f 6772 6573 7320  ds the progress 
+00001710: 696e 2070 6572 6365 6e74 2e0d 0a0d 0a20  in percent..... 
+00001720: 2020 2020 2020 2041 7267 733a 0d0a 2020         Args:..  
+00001730: 2020 2020 2020 2020 2020 706f 7065 6e5f            popen_
+00001740: 6b77 6172 6773 2028 6469 6374 2c20 6f70  kwargs (dict, op
+00001750: 7469 6f6e 616c 293a 2041 2064 6963 7420  tional): A dict 
+00001760: 746f 2073 7065 6369 6679 2065 7874 7261  to specify extra
+00001770: 2061 7267 756d 656e 7473 2074 6f20 7468   arguments to th
+00001780: 6520 706f 7065 6e20 6361 6c6c 2c20 652e  e popen call, e.
+00001790: 672e 207b 2063 7265 6174 696f 6e66 6c61  g. { creationfla
+000017a0: 6773 3a20 4352 4541 5445 5f4e 4f5f 5749  gs: CREATE_NO_WI
+000017b0: 4e44 4f57 207d 0d0a 2020 2020 2020 2020  NDOW }..        
+000017c0: 2020 2020 6475 7261 7469 6f6e 5f6f 7665      duration_ove
+000017d0: 7272 6964 6520 2866 6c6f 6174 2c20 6f70  rride (float, op
+000017e0: 7469 6f6e 616c 293a 2054 6865 2064 7572  tional): The dur
+000017f0: 6174 696f 6e20 696e 2073 6563 6f6e 6473  ation in seconds
+00001800: 2e20 4966 206e 6f74 2073 7065 6369 6669  . If not specifi
+00001810: 6564 2c20 6974 2077 696c 6c20 6265 2063  ed, it will be c
+00001820: 616c 6375 6c61 7465 6420 6672 6f6d 2074  alculated from t
+00001830: 6865 2066 666d 7065 6720 6f75 7470 7574  he ffmpeg output
+00001840: 2e0d 0a0d 0a20 2020 2020 2020 2052 6169  .....        Rai
+00001850: 7365 733a 0d0a 2020 2020 2020 2020 2020  ses:..          
+00001860: 2020 5275 6e74 696d 6545 7272 6f72 3a20    RuntimeError: 
+00001870: 4966 2074 6865 2063 6f6d 6d61 6e64 2066  If the command f
+00001880: 6169 6c73 2c20 616e 2065 7863 6570 7469  ails, an excepti
+00001890: 6f6e 2069 7320 7261 6973 6564 2e0d 0a0d  on is raised....
+000018a0: 0a20 2020 2020 2020 2059 6965 6c64 733a  .        Yields:
+000018b0: 0d0a 2020 2020 2020 2020 2020 2020 4974  ..            It
+000018c0: 6572 6174 6f72 5b69 6e74 5d3a 2041 2067  erator[int]: A g
+000018d0: 656e 6572 6174 6f72 2074 6861 7420 7969  enerator that yi
+000018e0: 656c 6473 2074 6865 2070 726f 6772 6573  elds the progres
+000018f0: 7320 696e 2070 6572 6365 6e74 2e0d 0a20  s in percent... 
+00001900: 2020 2020 2020 2027 2727 0d0a 2020 2020         '''..    
+00001910: 2020 2020 6966 2073 656c 662e 6472 795f      if self.dry_
+00001920: 7275 6e3a 0d0a 2020 2020 2020 2020 2020  run:..          
+00001930: 2020 7265 7475 726e 2073 656c 662e 636d    return self.cm
+00001940: 640d 0a0d 0a20 2020 2020 2020 2074 6f74  d....        tot
+00001950: 616c 5f64 7572 3a20 556e 696f 6e5b 4e6f  al_dur: Union[No
+00001960: 6e65 2c20 696e 745d 203d 204e 6f6e 650d  ne, int] = None.
+00001970: 0a20 2020 2020 2020 2069 6620 5f75 7365  .        if _use
+00001980: 735f 6572 726f 725f 6c6f 676c 6576 656c  s_error_loglevel
+00001990: 2873 656c 662e 636d 6429 3a0d 0a20 2020  (self.cmd):..   
+000019a0: 2020 2020 2020 2020 2074 6f74 616c 5f64           total_d
+000019b0: 7572 203d 205f 7072 6f62 655f 6475 7261  ur = _probe_dura
+000019c0: 7469 6f6e 2873 656c 662e 636d 6429 0d0a  tion(self.cmd)..
+000019d0: 0d0a 2020 2020 2020 2020 636d 645f 7769  ..        cmd_wi
+000019e0: 7468 5f70 726f 6772 6573 7320 3d20 280d  th_progress = (.
+000019f0: 0a20 2020 2020 2020 2020 2020 205b 7365  .            [se
+00001a00: 6c66 2e63 6d64 5b30 5d5d 202b 205b 222d  lf.cmd[0]] + ["-
+00001a10: 7072 6f67 7265 7373 222c 2022 2d22 2c20  progress", "-", 
+00001a20: 222d 6e6f 7374 6174 7322 5d20 2b20 7365  "-nostats"] + se
+00001a30: 6c66 2e63 6d64 5b31 3a5d 0d0a 2020 2020  lf.cmd[1:]..    
+00001a40: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
+00001a50: 2073 7464 6572 7220 3d20 5b5d 0d0a 2020   stderr = []..  
+00001a60: 2020 2020 2020 6261 7365 5f70 6f70 656e        base_popen
+00001a70: 5f6b 7761 7267 7320 3d20 7365 6c66 2e62  _kwargs = self.b
+00001a80: 6173 655f 706f 7065 6e5f 6b77 6172 6773  ase_popen_kwargs
+00001a90: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
+00001aa0: 2069 6620 706f 7065 6e5f 6b77 6172 6773   if popen_kwargs
+00001ab0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00001ac0: 2020 2020 2020 2020 2020 2062 6173 655f             base_
+00001ad0: 706f 7065 6e5f 6b77 6172 6773 2e75 7064  popen_kwargs.upd
+00001ae0: 6174 6528 706f 7065 6e5f 6b77 6172 6773  ate(popen_kwargs
+00001af0: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
+00001b00: 7379 732e 706c 6174 666f 726d 203d 3d20  sys.platform == 
+00001b10: 2277 696e 6433 3222 3a0d 0a20 2020 2020  "wind32":..     
+00001b20: 2020 2020 2020 2073 656c 662e 7072 6f63         self.proc
+00001b30: 6573 7320 3d20 7375 6270 726f 6365 7373  ess = subprocess
+00001b40: 2e50 6f70 656e 280d 0a20 2020 2020 2020  .Popen(..       
+00001b50: 2020 2020 2020 2020 2063 6d64 5f77 6974           cmd_wit
+00001b60: 685f 7072 6f67 7265 7373 2c0d 0a20 2020  h_progress,..   
+00001b70: 2020 2020 2020 2020 2020 2020 202a 2a62               **b
+00001b80: 6173 655f 706f 7065 6e5f 6b77 6172 6773  ase_popen_kwargs
+00001b90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001ba0: 2020 2063 7265 6174 696f 6e66 6c61 6773     creationflags
+00001bb0: 3d73 7562 7072 6f63 6573 732e 4352 4541  =subprocess.CREA
+00001bc0: 5445 5f4e 4f5f 5749 4e44 4f57 2c0d 0a20  TE_NO_WINDOW,.. 
+00001bd0: 2020 2020 2020 2020 2020 2029 2020 2320             )  # 
+00001be0: 7479 7065 3a20 6967 6e6f 7265 0d0a 2020  type: ignore..  
+00001bf0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00001c00: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00001c10: 6f63 6573 7320 3d20 7375 6270 726f 6365  ocess = subproce
+00001c20: 7373 2e50 6f70 656e 280d 0a20 2020 2020  ss.Popen(..     
+00001c30: 2020 2020 2020 2020 2020 2063 6d64 5f77             cmd_w
+00001c40: 6974 685f 7072 6f67 7265 7373 2c0d 0a20  ith_progress,.. 
+00001c50: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+00001c60: 2a62 6173 655f 706f 7065 6e5f 6b77 6172  *base_popen_kwar
+00001c70: 6773 2c0d 0a20 2020 2020 2020 2020 2020  gs,..           
+00001c80: 2029 2020 2320 7479 7065 3a20 6967 6e6f   )  # type: igno
+00001c90: 7265 0d0a 0d0a 2020 2020 2020 2020 7969  re....        yi
+00001ca0: 656c 6420 300d 0a0d 0a20 2020 2020 2020  eld 0....       
+00001cb0: 2077 6869 6c65 2054 7275 653a 0d0a 2020   while True:..  
+00001cc0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00001cd0: 662e 7072 6f63 6573 732e 7374 646f 7574  f.process.stdout
+00001ce0: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00001cf0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00001d00: 6e75 650d 0a0d 0a20 2020 2020 2020 2020  nue....         
+00001d10: 2020 2073 7464 6572 725f 6c69 6e65 203d     stderr_line =
+00001d20: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00001d30: 2020 2020 7365 6c66 2e70 726f 6365 7373      self.process
+00001d40: 2e73 7464 6f75 742e 7265 6164 6c69 6e65  .stdout.readline
+00001d50: 2829 2e64 6563 6f64 6528 2275 7466 2d38  ().decode("utf-8
+00001d60: 222c 2065 7272 6f72 733d 2272 6570 6c61  ", errors="repla
+00001d70: 6365 2229 2e73 7472 6970 2829 0d0a 2020  ce").strip()..  
+00001d80: 2020 2020 2020 2020 2020 290d 0a0d 0a20            ).... 
+00001d90: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00001da0: 6c66 2e73 7464 6572 725f 6361 6c6c 6261  lf.stderr_callba
+00001db0: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
+00001dc0: 2020 2020 2073 656c 662e 7374 6465 7272       self.stderr
+00001dd0: 5f63 616c 6c62 6163 6b28 7374 6465 7272  _callback(stderr
+00001de0: 5f6c 696e 6529 0d0a 0d0a 2020 2020 2020  _line)....      
+00001df0: 2020 2020 2020 6966 2073 7464 6572 725f        if stderr_
+00001e00: 6c69 6e65 203d 3d20 2727 2061 6e64 2073  line == '' and s
+00001e10: 656c 662e 7072 6f63 6573 732e 706f 6c6c  elf.process.poll
+00001e20: 2829 2069 7320 6e6f 7420 4e6f 6e65 3a0d  () is not None:.
 00001e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001e40: 2063 6f6e 7469 6e75 650d 0a0d 0a20 2020   continue....   
-00001e50: 2020 2020 2020 2020 2073 7464 6572 725f           stderr_
-00001e60: 6c69 6e65 203d 2028 0d0a 2020 2020 2020  line = (..      
-00001e70: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00001e80: 726f 6365 7373 2e73 7464 6f75 742e 7265  rocess.stdout.re
-00001e90: 6164 6c69 6e65 2829 2e64 6563 6f64 6528  adline().decode(
-00001ea0: 2275 7466 2d38 222c 2065 7272 6f72 733d  "utf-8", errors=
-00001eb0: 2272 6570 6c61 6365 2229 2e73 7472 6970  "replace").strip
-00001ec0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00001ed0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00001ee0: 2069 6620 7365 6c66 2e73 7464 6572 725f   if self.stderr_
-00001ef0: 6361 6c6c 6261 636b 3a0d 0a20 2020 2020  callback:..     
-00001f00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001f10: 7374 6465 7272 5f63 616c 6c62 6163 6b28  stderr_callback(
-00001f20: 7374 6465 7272 5f6c 696e 6529 0d0a 0d0a  stderr_line)....
-00001f30: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00001f40: 7464 6572 725f 6c69 6e65 203d 3d20 2727  tderr_line == ''
-00001f50: 2061 6e64 2073 656c 662e 7072 6f63 6573   and self.proces
-00001f60: 732e 706f 6c6c 2829 2069 7320 6e6f 7420  s.poll() is not 
-00001f70: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00001f80: 2020 2020 2020 2062 7265 616b 0d0a 0d0a         break....
-00001f90: 2020 2020 2020 2020 2020 2020 7374 6465              stde
-00001fa0: 7272 2e61 7070 656e 6428 7374 6465 7272  rr.append(stderr
-00001fb0: 5f6c 696e 652e 7374 7269 7028 2929 0d0a  _line.strip())..
-00001fc0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00001fd0: 6c66 2e73 7464 6572 7220 3d20 225c 6e22  lf.stderr = "\n"
-00001fe0: 2e6a 6f69 6e28 7374 6465 7272 290d 0a0d  .join(stderr)...
-00001ff0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002000: 746f 7461 6c5f 6475 7220 6973 204e 6f6e  total_dur is Non
-00002010: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002020: 2020 2020 746f 7461 6c5f 6475 725f 6d61      total_dur_ma
-00002030: 7463 6820 3d20 7365 6c66 2e44 5552 5f52  tch = self.DUR_R
-00002040: 4547 4558 2e73 6561 7263 6828 7374 6465  EGEX.search(stde
-00002050: 7272 5f6c 696e 6529 0d0a 2020 2020 2020  rr_line)..      
-00002060: 2020 2020 2020 2020 2020 6966 2074 6f74            if tot
-00002070: 616c 5f64 7572 5f6d 6174 6368 3a0d 0a20  al_dur_match:.. 
-00002080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002090: 2020 2074 6f74 616c 5f64 7572 203d 2074     total_dur = t
-000020a0: 6f5f 6d73 282a 2a74 6f74 616c 5f64 7572  o_ms(**total_dur
-000020b0: 5f6d 6174 6368 2e67 726f 7570 6469 6374  _match.groupdict
-000020c0: 2829 290d 0a20 2020 2020 2020 2020 2020  ())..           
-000020d0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-000020e0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-000020f0: 2020 2065 6c69 6620 6475 7261 7469 6f6e     elif duration
-00002100: 5f6f 7665 7272 6964 6520 6973 206e 6f74  _override is not
-00002110: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00002120: 2020 2020 2020 2020 2020 2020 2320 7573              # us
-00002130: 6520 7468 6520 6f76 6572 7269 6465 2028  e the override (
-00002140: 7368 6f75 6c64 2061 7070 6c79 2069 6e20  should apply in 
-00002150: 7468 6520 6669 7273 7420 6c6f 6f70 290d  the first loop).
-00002160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002170: 2020 2020 2074 6f74 616c 5f64 7572 203d       total_dur =
-00002180: 2069 6e74 2864 7572 6174 696f 6e5f 6f76   int(duration_ov
-00002190: 6572 7269 6465 202a 2031 3030 3029 0d0a  erride * 1000)..
-000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021b0: 2020 2020 636f 6e74 696e 7565 0d0a 0d0a      continue....
-000021c0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-000021d0: 6f74 616c 5f64 7572 3a0d 0a20 2020 2020  otal_dur:..     
-000021e0: 2020 2020 2020 2020 2020 2070 726f 6772             progr
-000021f0: 6573 735f 7469 6d65 203d 2046 666d 7065  ess_time = Ffmpe
-00002200: 6750 726f 6772 6573 732e 5449 4d45 5f52  gProgress.TIME_R
-00002210: 4547 4558 2e73 6561 7263 6828 7374 6465  EGEX.search(stde
-00002220: 7272 5f6c 696e 6529 0d0a 2020 2020 2020  rr_line)..      
-00002230: 2020 2020 2020 2020 2020 6966 2070 726f            if pro
-00002240: 6772 6573 735f 7469 6d65 3a0d 0a20 2020  gress_time:..   
-00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 2065 6c61 7073 6564 5f74 696d 6520 3d20   elapsed_time = 
-00002270: 746f 5f6d 7328 2a2a 7072 6f67 7265 7373  to_ms(**progress
-00002280: 5f74 696d 652e 6772 6f75 7064 6963 7428  _time.groupdict(
-00002290: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000022a0: 2020 2020 2020 2020 7969 656c 6420 696e          yield in
-000022b0: 7428 656c 6170 7365 645f 7469 6d65 202a  t(elapsed_time *
-000022c0: 2031 3030 2f20 746f 7461 6c5f 6475 7229   100/ total_dur)
-000022d0: 0d0a 0d0a 2020 2020 2020 2020 6966 2073  ....        if s
-000022e0: 656c 662e 7072 6f63 6573 7320 6973 204e  elf.process is N
-000022f0: 6f6e 6520 6f72 2073 656c 662e 7072 6f63  one or self.proc
-00002300: 6573 732e 7265 7475 726e 636f 6465 2021  ess.returncode !
-00002310: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
-00002320: 2020 5f70 7265 7474 795f 7374 6465 7272    _pretty_stderr
-00002330: 203d 2022 5c6e 222e 6a6f 696e 2873 7464   = "\n".join(std
-00002340: 6572 7229 0d0a 2020 2020 2020 2020 2020  err)..          
-00002350: 2020 7261 6973 6520 5275 6e74 696d 6545    raise RuntimeE
-00002360: 7272 6f72 2866 2245 7272 6f72 2072 756e  rror(f"Error run
-00002370: 6e69 6e67 2063 6f6d 6d61 6e64 207b 7365  ning command {se
-00002380: 6c66 2e63 6d64 7d3a 207b 5f70 7265 7474  lf.cmd}: {_prett
-00002390: 795f 7374 6465 7272 7d22 290d 0a0d 0a20  y_stderr}").... 
-000023a0: 2020 2020 2020 2079 6965 6c64 2031 3030         yield 100
-000023b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-000023c0: 726f 6365 7373 203d 204e 6f6e 650d 0a0d  rocess = None...
-000023d0: 0a20 2020 2064 6566 2071 7569 745f 6772  .    def quit_gr
-000023e0: 6163 6566 756c 6c79 2873 656c 6629 202d  acefully(self) -
-000023f0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
-00002400: 2027 2727 0d0a 2020 2020 2020 2020 5175   '''..        Qu
-00002410: 6974 2074 6865 2066 666d 7065 6720 7072  it the ffmpeg pr
-00002420: 6f63 6573 7320 6279 2073 656e 6469 6e67  ocess by sending
-00002430: 2027 7127 0d0a 0d0a 2020 2020 2020 2020   'q'....        
-00002440: 5261 6973 6573 3a0d 0a20 2020 2020 2020  Raises:..       
-00002450: 2020 2020 2052 756e 7469 6d65 4572 726f       RuntimeErro
-00002460: 723a 2049 6620 6e6f 2070 726f 6365 7373  r: If no process
-00002470: 2069 7320 666f 756e 642e 0d0a 2020 2020   is found...    
-00002480: 2020 2020 2727 270d 0a20 2020 2020 2020      '''..       
-00002490: 2069 6620 7365 6c66 2e70 726f 6365 7373   if self.process
-000024a0: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-000024b0: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
-000024c0: 7469 6d65 4572 726f 7228 224e 6f20 7072  timeError("No pr
-000024d0: 6f63 6573 7320 666f 756e 642e 2044 6964  ocess found. Did
-000024e0: 2079 6f75 2072 756e 2074 6865 2063 6f6d   you run the com
-000024f0: 6d61 6e64 3f22 290d 0a0d 0a20 2020 2020  mand?")....     
-00002500: 2020 2073 656c 662e 7072 6f63 6573 732e     self.process.
-00002510: 636f 6d6d 756e 6963 6174 6528 696e 7075  communicate(inpu
-00002520: 743d 6222 7122 290d 0a20 2020 2020 2020  t=b"q")..       
-00002530: 2073 656c 662e 7072 6f63 6573 732e 6b69   self.process.ki
-00002540: 6c6c 2829 0d0a 2020 2020 2020 2020 7365  ll()..        se
-00002550: 6c66 2e70 726f 6365 7373 203d 204e 6f6e  lf.process = Non
-00002560: 650d 0a0d 0a20 2020 2064 6566 2071 7569  e....    def qui
-00002570: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
-00002580: 0d0a 2020 2020 2020 2020 2727 270d 0a20  ..        '''.. 
-00002590: 2020 2020 2020 2051 7569 7420 7468 6520         Quit the 
-000025a0: 6666 6d70 6567 2070 726f 6365 7373 2062  ffmpeg process b
-000025b0: 7920 7365 6e64 696e 6720 5349 474b 494c  y sending SIGKIL
-000025c0: 4c2e 0d0a 0d0a 2020 2020 2020 2020 5261  L.....        Ra
-000025d0: 6973 6573 3a0d 0a20 2020 2020 2020 2020  ises:..         
-000025e0: 2020 2052 756e 7469 6d65 4572 726f 723a     RuntimeError:
-000025f0: 2049 6620 6e6f 2070 726f 6365 7373 2069   If no process i
-00002600: 7320 666f 756e 642e 0d0a 2020 2020 2020  s found...      
-00002610: 2020 2727 270d 0a20 2020 2020 2020 2069    '''..        i
-00002620: 6620 7365 6c66 2e70 726f 6365 7373 2069  f self.process i
-00002630: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00002640: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
-00002650: 6d65 4572 726f 7228 224e 6f20 7072 6f63  meError("No proc
-00002660: 6573 7320 666f 756e 642e 2044 6964 2079  ess found. Did y
-00002670: 6f75 2072 756e 2074 6865 2063 6f6d 6d61  ou run the comma
-00002680: 6e64 3f22 290d 0a0d 0a20 2020 2020 2020  nd?")....       
-00002690: 2073 656c 662e 7072 6f63 6573 732e 6b69   self.process.ki
-000026a0: 6c6c 2829 0d0a 2020 2020 2020 2020 7365  ll()..        se
-000026b0: 6c66 2e70 726f 6365 7373 203d 204e 6f6e  lf.process = Non
-000026c0: 650d 0a0d 0a0d 0a23 3d3d 3d3d 3d3d 3d3d  e......#========
-000026d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000026e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000026f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002700: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002710: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002720: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002730: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002740: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d23  ===============#
-00002750: 0d0a 0d0a 0d0a 6465 6620 7374 6f70 5f66  ......def stop_f
-00002760: 666d 7065 675f 7769 6e64 6f77 7328 6572  fmpeg_windows(er
-00002770: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-00002780: 6c62 6163 6b3d 4e6f 6e65 293a 0d0a 2020  lback=None):..  
-00002790: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-000027a0: 7461 736b 6c69 7374 5f6f 7574 7075 7420  tasklist_output 
-000027b0: 3d20 7375 6270 726f 6365 7373 2e63 6865  = subprocess.che
-000027c0: 636b 5f6f 7574 7075 7428 5b27 7461 736b  ck_output(['task
-000027d0: 6c69 7374 275d 2c20 6372 6561 7469 6f6e  list'], creation
-000027e0: 666c 6167 733d 7375 6270 726f 6365 7373  flags=subprocess
-000027f0: 2e43 5245 4154 455f 4e4f 5f57 494e 444f  .CREATE_NO_WINDO
-00002800: 5729 2e64 6563 6f64 6528 2775 7466 2d38  W).decode('utf-8
-00002810: 2729 0d0a 2020 2020 2020 2020 6666 6d70  ')..        ffmp
-00002820: 6567 5f70 6964 203d 204e 6f6e 650d 0a20  eg_pid = None.. 
-00002830: 2020 2020 2020 2066 6f72 206c 696e 6520         for line 
-00002840: 696e 2074 6173 6b6c 6973 745f 6f75 7470  in tasklist_outp
-00002850: 7574 2e73 706c 6974 2827 5c6e 2729 3a0d  ut.split('\n'):.
-00002860: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002870: 2266 666d 7065 6722 2069 6e20 6c69 6e65  "ffmpeg" in line
-00002880: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002890: 2020 2066 666d 7065 675f 7069 6420 3d20     ffmpeg_pid = 
-000028a0: 6c69 6e65 2e73 706c 6974 2829 5b31 5d0d  line.split()[1].
-000028b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000028c0: 2062 7265 616b 0d0a 2020 2020 2020 2020   break..        
-000028d0: 6966 2066 666d 7065 675f 7069 643a 0d0a  if ffmpeg_pid:..
-000028e0: 2020 2020 2020 2020 2020 2020 6465 766e              devn
-000028f0: 756c 6c20 3d20 6f70 656e 286f 732e 6465  ull = open(os.de
-00002900: 766e 756c 6c2c 2027 7727 290d 0a20 2020  vnull, 'w')..   
-00002910: 2020 2020 2020 2020 2073 7562 7072 6f63           subproc
-00002920: 6573 732e 506f 7065 6e28 5b27 7461 736b  ess.Popen(['task
-00002930: 6b69 6c6c 272c 2027 2f46 272c 2027 2f54  kill', '/F', '/T
-00002940: 272c 2027 2f50 4944 272c 2066 666d 7065  ', '/PID', ffmpe
-00002950: 675f 7069 645d 2c20 7374 646f 7574 3d73  g_pid], stdout=s
-00002960: 7562 7072 6f63 6573 732e 5049 5045 2c20  ubprocess.PIPE, 
-00002970: 7374 6465 7272 3d73 7562 7072 6f63 6573  stderr=subproces
-00002980: 732e 5354 444f 5554 2c20 7368 656c 6c3d  s.STDOUT, shell=
-00002990: 5472 7565 2c20 6372 6561 7469 6f6e 666c  True, creationfl
-000029a0: 6167 733d 7375 6270 726f 6365 7373 2e43  ags=subprocess.C
-000029b0: 5245 4154 455f 4e4f 5f57 494e 444f 5729  REATE_NO_WINDOW)
-000029c0: 0d0a 0d0a 2020 2020 6578 6365 7074 204b  ....    except K
-000029d0: 6579 626f 6172 6449 6e74 6572 7275 7074  eyboardInterrupt
-000029e0: 3a0d 0a20 2020 2020 2020 2069 6620 6572  :..        if er
-000029f0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-00002a00: 6c62 6163 6b3a 0d0a 2020 2020 2020 2020  lback:..        
-00002a10: 2020 2020 6572 726f 725f 6d65 7373 6167      error_messag
-00002a20: 6573 5f63 616c 6c62 6163 6b28 2243 616e  es_callback("Can
-00002a30: 6365 6c6c 696e 6720 616c 6c20 7461 736b  celling all task
-00002a40: 7322 290d 0a20 2020 2020 2020 2065 6c73  s")..        els
-00002a50: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002a60: 7072 696e 7428 2243 616e 6365 6c6c 696e  print("Cancellin
-00002a70: 6720 616c 6c20 7461 736b 7322 290d 0a20  g all tasks").. 
-00002a80: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
-00002a90: 0a20 2020 2065 7863 6570 7420 4578 6365  .    except Exce
-00002aa0: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
-00002ab0: 2020 2020 2069 6620 6572 726f 725f 6d65       if error_me
-00002ac0: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
-00002ad0: 0d0a 2020 2020 2020 2020 2020 2020 6572  ..            er
-00002ae0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-00002af0: 6c62 6163 6b28 6529 0d0a 2020 2020 2020  lback(e)..      
-00002b00: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00002b10: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
-00002b20: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
-00002b30: 0a0d 0a64 6566 2073 746f 705f 6666 6d70  ...def stop_ffmp
-00002b40: 6567 5f6c 696e 7578 2865 7272 6f72 5f6d  eg_linux(error_m
-00002b50: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
-00002b60: 3d4e 6f6e 6529 3a0d 0a20 2020 2070 726f  =None):..    pro
-00002b70: 6365 7373 5f6e 616d 6520 3d20 2766 666d  cess_name = 'ffm
-00002b80: 7065 6727 0d0a 2020 2020 7472 793a 0d0a  peg'..    try:..
-00002b90: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
-00002ba0: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
-00002bb0: 6b5f 6f75 7470 7574 285b 2770 7327 2c20  k_output(['ps', 
-00002bc0: 272d 6566 275d 290d 0a20 2020 2020 2020  '-ef'])..       
-00002bd0: 2070 6964 203d 205b 6c69 6e65 2e73 706c   pid = [line.spl
-00002be0: 6974 2829 5b31 5d20 666f 7220 6c69 6e65  it()[1] for line
-00002bf0: 2069 6e20 6f75 7470 7574 2e64 6563 6f64   in output.decod
-00002c00: 6528 2775 7466 2d38 2729 2e73 706c 6974  e('utf-8').split
-00002c10: 2827 5c6e 2729 2069 6620 7072 6f63 6573  ('\n') if proces
-00002c20: 735f 6e61 6d65 2069 6e20 6c69 6e65 5d5b  s_name in line][
-00002c30: 305d 0d0a 2020 2020 2020 2020 7375 6270  0]..        subp
-00002c40: 726f 6365 7373 2e63 616c 6c28 5b27 6b69  rocess.call(['ki
-00002c50: 6c6c 272c 2027 2d39 272c 2073 7472 2870  ll', '-9', str(p
-00002c60: 6964 295d 290d 0a20 2020 2065 7863 6570  id)])..    excep
-00002c70: 7420 496e 6465 7845 7272 6f72 3a0d 0a20  t IndexError:.. 
-00002c80: 2020 2020 2020 2070 6173 730d 0a0d 0a20         pass.... 
-00002c90: 2020 2065 7863 6570 7420 4b65 7962 6f61     except Keyboa
-00002ca0: 7264 496e 7465 7272 7570 743a 0d0a 2020  rdInterrupt:..  
-00002cb0: 2020 2020 2020 6966 2065 7272 6f72 5f6d        if error_m
-00002cc0: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
-00002cd0: 3a0d 0a20 2020 2020 2020 2020 2020 2065  :..            e
-00002ce0: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-00002cf0: 6c6c 6261 636b 2822 4361 6e63 656c 6c69  llback("Cancelli
-00002d00: 6e67 2061 6c6c 2074 6173 6b73 2229 0d0a  ng all tasks")..
-00002d10: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00002d20: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00002d30: 2822 4361 6e63 656c 6c69 6e67 2061 6c6c  ("Cancelling all
-00002d40: 2074 6173 6b73 2229 0d0a 2020 2020 2020   tasks")..      
-00002d50: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
-00002d60: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00002d70: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
-00002d80: 6966 2065 7272 6f72 5f6d 6573 7361 6765  if error_message
-00002d90: 735f 6361 6c6c 6261 636b 3a0d 0a20 2020  s_callback:..   
-00002da0: 2020 2020 2020 2020 2065 7272 6f72 5f6d           error_m
-00002db0: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
-00002dc0: 2865 290d 0a20 2020 2020 2020 2065 6c73  (e)..        els
-00002dd0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002de0: 7072 696e 7428 6529 0d0a 2020 2020 2020  print(e)..      
-00002df0: 2020 7265 7475 726e 0d0a 0d0a 0d0a 6465    return......de
-00002e00: 6620 7265 6d6f 7665 5f74 656d 705f 6669  f remove_temp_fi
-00002e10: 6c65 7328 6578 7465 6e73 696f 6e2c 2065  les(extension, e
-00002e20: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-00002e30: 6c6c 6261 636b 3d4e 6f6e 6529 3a0d 0a20  llback=None):.. 
-00002e40: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00002e50: 2074 656d 705f 6469 7220 3d20 7465 6d70   temp_dir = temp
-00002e60: 6669 6c65 2e67 6574 7465 6d70 6469 7228  file.gettempdir(
-00002e70: 290d 0a20 2020 2020 2020 2066 6f72 2072  )..        for r
-00002e80: 6f6f 742c 2064 6972 732c 2066 696c 6573  oot, dirs, files
-00002e90: 2069 6e20 6f73 2e77 616c 6b28 7465 6d70   in os.walk(temp
-00002ea0: 5f64 6972 293a 0d0a 2020 2020 2020 2020  _dir):..        
-00002eb0: 2020 2020 666f 7220 6669 6c65 2069 6e20      for file in 
-00002ec0: 6669 6c65 733a 0d0a 2020 2020 2020 2020  files:..        
-00002ed0: 2020 2020 2020 2020 6966 2066 696c 652e          if file.
-00002ee0: 656e 6473 7769 7468 2822 2e22 202b 2065  endswith("." + e
-00002ef0: 7874 656e 7369 6f6e 293a 0d0a 2020 2020  xtension):..    
-00002f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f10: 6f73 2e72 656d 6f76 6528 6f73 2e70 6174  os.remove(os.pat
-00002f20: 682e 6a6f 696e 2872 6f6f 742c 2066 696c  h.join(root, fil
-00002f30: 6529 290d 0a20 2020 2065 7863 6570 7420  e))..    except 
-00002f40: 4b65 7962 6f61 7264 496e 7465 7272 7570  KeyboardInterrup
-00002f50: 743a 0d0a 2020 2020 2020 2020 6966 2065  t:..        if e
-00002f60: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-00002f70: 6c6c 6261 636b 3a0d 0a20 2020 2020 2020  llback:..       
-00002f80: 2020 2020 2065 7272 6f72 5f6d 6573 7361       error_messa
-00002f90: 6765 735f 6361 6c6c 6261 636b 2822 4361  ges_callback("Ca
-00002fa0: 6e63 656c 6c69 6e67 2061 6c6c 2074 6173  ncelling all tas
-00002fb0: 6b73 2229 0d0a 2020 2020 2020 2020 656c  ks")..        el
-00002fc0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00002fd0: 2070 7269 6e74 2822 4361 6e63 656c 6c69   print("Cancelli
-00002fe0: 6e67 2061 6c6c 2074 6173 6b73 2229 0d0a  ng all tasks")..
-00002ff0: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
-00003000: 0d0a 2020 2020 6578 6365 7074 2045 7863  ..    except Exc
-00003010: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
-00003020: 2020 2020 2020 6966 2065 7272 6f72 5f6d        if error_m
-00003030: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
-00003040: 3a0d 0a20 2020 2020 2020 2020 2020 2065  :..            e
-00003050: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-00003060: 6c6c 6261 636b 2865 290d 0a20 2020 2020  llback(e)..     
-00003070: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00003080: 2020 2020 2020 7072 696e 7428 6529 0d0a        print(e)..
-00003090: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
-000030a0: 0d0a 0d0a 6465 6620 6973 5f73 616d 655f  ....def is_same_
-000030b0: 6c61 6e67 7561 6765 2873 7263 2c20 6473  language(src, ds
-000030c0: 742c 2065 7272 6f72 5f6d 6573 7361 6765  t, error_message
-000030d0: 735f 6361 6c6c 6261 636b 3d4e 6f6e 6529  s_callback=None)
-000030e0: 3a0d 0a20 2020 2074 7279 3a0d 0a20 2020  :..    try:..   
-000030f0: 2020 2020 2072 6574 7572 6e20 7372 632e       return src.
-00003100: 7370 6c69 7428 222d 2229 5b30 5d20 3d3d  split("-")[0] ==
-00003110: 2064 7374 2e73 706c 6974 2822 2d22 295b   dst.split("-")[
-00003120: 305d 0d0a 2020 2020 6578 6365 7074 2045  0]..    except E
-00003130: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
-00003140: 2020 2020 2020 2020 6966 2065 7272 6f72          if error
-00003150: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-00003160: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
-00003170: 2065 7272 6f72 5f6d 6573 7361 6765 735f   error_messages_
-00003180: 6361 6c6c 6261 636b 2865 290d 0a20 2020  callback(e)..   
-00003190: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-000031a0: 2020 2020 2020 2020 7072 696e 7428 6529          print(e)
-000031b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000031c0: 0d0a 0d0a 0d0a 6465 6620 6368 6563 6b5f  ......def check_
-000031d0: 6669 6c65 5f74 7970 6528 6669 6c65 5f70  file_type(file_p
-000031e0: 6174 682c 2065 7272 6f72 5f6d 6573 7361  ath, error_messa
-000031f0: 6765 735f 6361 6c6c 6261 636b 3d4e 6f6e  ges_callback=Non
-00003200: 6529 3a0d 0a20 2020 2074 7279 3a0d 0a20  e):..    try:.. 
-00003210: 2020 2020 2020 2066 6670 726f 6265 5f63         ffprobe_c
-00003220: 6d64 203d 205b 2766 6670 726f 6265 272c  md = ['ffprobe',
-00003230: 2027 2d76 272c 2027 6572 726f 7227 2c20   '-v', 'error', 
-00003240: 272d 7368 6f77 5f66 6f72 6d61 7427 2c20  '-show_format', 
-00003250: 272d 7368 6f77 5f73 7472 6561 6d73 272c  '-show_streams',
-00003260: 2027 2d70 7269 6e74 5f66 6f72 6d61 7427   '-print_format'
-00003270: 2c20 276a 736f 6e27 2c20 6669 6c65 5f70  , 'json', file_p
-00003280: 6174 685d 0d0a 2020 2020 2020 2020 6f75  ath]..        ou
-00003290: 7470 7574 203d 204e 6f6e 650d 0a20 2020  tput = None..   
-000032a0: 2020 2020 2069 6620 7379 732e 706c 6174       if sys.plat
-000032b0: 666f 726d 203d 3d20 2277 696e 3332 223a  form == "win32":
-000032c0: 0d0a 2020 2020 2020 2020 2020 2020 6f75  ..            ou
-000032d0: 7470 7574 203d 2073 7562 7072 6f63 6573  tput = subproces
-000032e0: 732e 6368 6563 6b5f 6f75 7470 7574 2866  s.check_output(f
-000032f0: 6670 726f 6265 5f63 6d64 2c20 6372 6561  fprobe_cmd, crea
-00003300: 7469 6f6e 666c 6167 733d 7375 6270 726f  tionflags=subpro
-00003310: 6365 7373 2e43 5245 4154 455f 4e4f 5f57  cess.CREATE_NO_W
-00003320: 494e 444f 5729 2e64 6563 6f64 6528 2775  INDOW).decode('u
-00003330: 7466 2d38 2729 0d0a 2020 2020 2020 2020  tf-8')..        
-00003340: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00003350: 2020 206f 7574 7075 7420 3d20 7375 6270     output = subp
-00003360: 726f 6365 7373 2e63 6865 636b 5f6f 7574  rocess.check_out
-00003370: 7075 7428 6666 7072 6f62 655f 636d 6429  put(ffprobe_cmd)
-00003380: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
-00003390: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-000033a0: 206a 736f 6e2e 6c6f 6164 7328 6f75 7470   json.loads(outp
-000033b0: 7574 290d 0a0d 0a20 2020 2020 2020 2069  ut)....        i
-000033c0: 6620 2773 7472 6561 6d73 2720 696e 2064  f 'streams' in d
-000033d0: 6174 613a 0d0a 2020 2020 2020 2020 2020  ata:..          
-000033e0: 2020 666f 7220 7374 7265 616d 2069 6e20    for stream in 
-000033f0: 6461 7461 5b27 7374 7265 616d 7327 5d3a  data['streams']:
-00003400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003410: 2020 6966 2027 636f 6465 635f 7479 7065    if 'codec_type
-00003420: 2720 696e 2073 7472 6561 6d20 616e 6420  ' in stream and 
-00003430: 7374 7265 616d 5b27 636f 6465 635f 7479  stream['codec_ty
-00003440: 7065 275d 203d 3d20 2761 7564 696f 273a  pe'] == 'audio':
-00003450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003460: 2020 2020 2020 7265 7475 726e 2027 6175        return 'au
-00003470: 6469 6f27 0d0a 2020 2020 2020 2020 2020  dio'..          
-00003480: 2020 2020 2020 656c 6966 2027 636f 6465        elif 'code
-00003490: 635f 7479 7065 2720 696e 2073 7472 6561  c_type' in strea
-000034a0: 6d20 616e 6420 7374 7265 616d 5b27 636f  m and stream['co
-000034b0: 6465 635f 7479 7065 275d 203d 3d20 2776  dec_type'] == 'v
-000034c0: 6964 656f 273a 0d0a 2020 2020 2020 2020  ideo':..        
-000034d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000034e0: 726e 2027 7669 6465 6f27 0d0a 2020 2020  rn 'video'..    
-000034f0: 6578 6365 7074 2028 7375 6270 726f 6365  except (subproce
-00003500: 7373 2e43 616c 6c65 6450 726f 6365 7373  ss.CalledProcess
-00003510: 4572 726f 722c 206a 736f 6e2e 4a53 4f4e  Error, json.JSON
-00003520: 4465 636f 6465 4572 726f 7229 3a0d 0a20  DecodeError):.. 
-00003530: 2020 2020 2020 2070 6173 730d 0a0d 0a20         pass.... 
-00003540: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00003550: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-00003560: 2020 2069 6620 6572 726f 725f 6d65 7373     if error_mess
-00003570: 6167 6573 5f63 616c 6c62 6163 6b3a 0d0a  ages_callback:..
-00003580: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-00003590: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-000035a0: 6163 6b28 6529 0d0a 2020 2020 2020 2020  ack(e)..        
-000035b0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000035c0: 2020 2070 7269 6e74 2865 290d 0a0d 0a20     print(e).... 
-000035d0: 2020 2072 6574 7572 6e20 4e6f 6e65 0d0a     return None..
-000035e0: 0d0a 0d0a 636c 6173 7320 5768 6973 7065  ....class Whispe
-000035f0: 724c 616e 6775 6167 653a 0d0a 2020 2020  rLanguage:..    
-00003600: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00003610: 6629 3a0d 0a20 2020 2020 2020 2073 656c  f):..        sel
-00003620: 662e 6c69 7374 5f63 6f64 6573 203d 205b  f.list_codes = [
-00003630: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
-00003640: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00003650: 6428 2261 6622 290d 0a20 2020 2020 2020  d("af")..       
-00003660: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00003670: 2e61 7070 656e 6428 2273 7122 290d 0a20  .append("sq").. 
-00003680: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00003690: 5f63 6f64 6573 2e61 7070 656e 6428 2261  _codes.append("a
-000036a0: 6d22 290d 0a20 2020 2020 2020 2073 656c  m")..        sel
-000036b0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-000036c0: 656e 6428 2261 7222 290d 0a20 2020 2020  end("ar")..     
-000036d0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-000036e0: 6573 2e61 7070 656e 6428 2268 7922 290d  es.append("hy").
-000036f0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00003700: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00003710: 2261 7322 290d 0a20 2020 2020 2020 2073  "as")..        s
-00003720: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00003730: 7070 656e 6428 2261 7a22 290d 0a20 2020  ppend("az")..   
-00003740: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00003750: 6f64 6573 2e61 7070 656e 6428 2262 6122  odes.append("ba"
-00003760: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003770: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00003780: 6428 2265 7522 290d 0a20 2020 2020 2020  d("eu")..       
-00003790: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-000037a0: 2e61 7070 656e 6428 2262 6522 290d 0a20  .append("be").. 
-000037b0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000037c0: 5f63 6f64 6573 2e61 7070 656e 6428 2262  _codes.append("b
-000037d0: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-000037e0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-000037f0: 656e 6428 2262 7322 290d 0a20 2020 2020  end("bs")..     
-00003800: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00003810: 6573 2e61 7070 656e 6428 2262 7222 290d  es.append("br").
-00003820: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00003830: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00003840: 2262 6722 290d 0a20 2020 2020 2020 2073  "bg")..        s
-00003850: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00003860: 7070 656e 6428 2263 6122 290d 0a20 2020  ppend("ca")..   
-00003870: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00003880: 6f64 6573 2e61 7070 656e 6428 227a 6822  odes.append("zh"
-00003890: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000038a0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-000038b0: 6428 2268 7222 290d 0a20 2020 2020 2020  d("hr")..       
-000038c0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-000038d0: 2e61 7070 656e 6428 2263 7322 290d 0a20  .append("cs").. 
-000038e0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000038f0: 5f63 6f64 6573 2e61 7070 656e 6428 2264  _codes.append("d
-00003900: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
-00003910: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00003920: 656e 6428 226e 6c22 290d 0a20 2020 2020  end("nl")..     
-00003930: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00003940: 6573 2e61 7070 656e 6428 2265 6e22 290d  es.append("en").
-00003950: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00003960: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00003970: 2265 7422 290d 0a20 2020 2020 2020 2073  "et")..        s
-00003980: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00003990: 7070 656e 6428 2266 6f22 290d 0a20 2020  ppend("fo")..   
-000039a0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-000039b0: 6f64 6573 2e61 7070 656e 6428 2266 6922  odes.append("fi"
-000039c0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000039d0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-000039e0: 6428 2266 7222 290d 0a20 2020 2020 2020  d("fr")..       
-000039f0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00003a00: 2e61 7070 656e 6428 2267 6c22 290d 0a20  .append("gl").. 
-00003a10: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00003a20: 5f63 6f64 6573 2e61 7070 656e 6428 226b  _codes.append("k
-00003a30: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
-00003a40: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00003a50: 656e 6428 2264 6522 290d 0a20 2020 2020  end("de")..     
-00003a60: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00003a70: 6573 2e61 7070 656e 6428 2265 6c22 290d  es.append("el").
-00003a80: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00003a90: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00003aa0: 2267 7522 290d 0a20 2020 2020 2020 2073  "gu")..        s
-00003ab0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00003ac0: 7070 656e 6428 2268 7422 290d 0a20 2020  ppend("ht")..   
-00003ad0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00003ae0: 6f64 6573 2e61 7070 656e 6428 2268 6122  odes.append("ha"
-00003af0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003b00: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00003b10: 6428 2268 6177 2229 0d0a 2020 2020 2020  d("haw")..      
-00003b20: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00003b30: 732e 6170 7065 6e64 2822 6865 2229 0d0a  s.append("he")..
-00003b40: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00003b50: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00003b60: 6869 2229 0d0a 2020 2020 2020 2020 7365  hi")..        se
-00003b70: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00003b80: 7065 6e64 2822 6875 2229 0d0a 2020 2020  pend("hu")..    
-00003b90: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00003ba0: 6465 732e 6170 7065 6e64 2822 6973 2229  des.append("is")
-00003bb0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00003bc0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00003bd0: 2822 6964 2229 0d0a 2020 2020 2020 2020  ("id")..        
-00003be0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00003bf0: 6170 7065 6e64 2822 6974 2229 0d0a 2020  append("it")..  
-00003c00: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00003c10: 636f 6465 732e 6170 7065 6e64 2822 6a61  codes.append("ja
-00003c20: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00003c30: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00003c40: 6e64 2822 6a76 2229 0d0a 2020 2020 2020  nd("jv")..      
-00003c50: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00003c60: 732e 6170 7065 6e64 2822 6b6e 2229 0d0a  s.append("kn")..
-00003c70: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00003c80: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00003c90: 6b6b 2229 0d0a 2020 2020 2020 2020 7365  kk")..        se
-00003ca0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00003cb0: 7065 6e64 2822 6b6d 2229 0d0a 2020 2020  pend("km")..    
-00003cc0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00003cd0: 6465 732e 6170 7065 6e64 2822 6b6f 2229  des.append("ko")
-00003ce0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00003cf0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00003d00: 2822 6c6f 2229 0d0a 2020 2020 2020 2020  ("lo")..        
-00003d10: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00003d20: 6170 7065 6e64 2822 6c61 2229 0d0a 2020  append("la")..  
-00003d30: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00003d40: 636f 6465 732e 6170 7065 6e64 2822 6c76  codes.append("lv
-00003d50: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00003d60: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00003d70: 6e64 2822 6c6e 2229 0d0a 2020 2020 2020  nd("ln")..      
-00003d80: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00003d90: 732e 6170 7065 6e64 2822 6c74 2229 0d0a  s.append("lt")..
-00003da0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00003db0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00003dc0: 6c62 2229 0d0a 2020 2020 2020 2020 7365  lb")..        se
-00003dd0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00003de0: 7065 6e64 2822 6d6b 2229 0d0a 2020 2020  pend("mk")..    
-00003df0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00003e00: 6465 732e 6170 7065 6e64 2822 6d67 2229  des.append("mg")
-00003e10: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00003e20: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00003e30: 2822 6d73 2229 0d0a 2020 2020 2020 2020  ("ms")..        
-00003e40: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00003e50: 6170 7065 6e64 2822 6d6c 2229 0d0a 2020  append("ml")..  
-00003e60: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00003e70: 636f 6465 732e 6170 7065 6e64 2822 6d74  codes.append("mt
-00003e80: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00003e90: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00003ea0: 6e64 2822 6d69 2229 0d0a 2020 2020 2020  nd("mi")..      
-00003eb0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00003ec0: 732e 6170 7065 6e64 2822 6d72 2229 0d0a  s.append("mr")..
-00003ed0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00003ee0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00003ef0: 6d6e 2229 0d0a 2020 2020 2020 2020 7365  mn")..        se
-00003f00: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00003f10: 7065 6e64 2822 6d79 2229 0d0a 2020 2020  pend("my")..    
-00003f20: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00003f30: 6465 732e 6170 7065 6e64 2822 6e65 2229  des.append("ne")
-00003f40: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00003f50: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00003f60: 2822 6e6f 2229 0d0a 2020 2020 2020 2020  ("no")..        
-00003f70: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00003f80: 6170 7065 6e64 2822 6e6e 2229 0d0a 2020  append("nn")..  
-00003f90: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00003fa0: 636f 6465 732e 6170 7065 6e64 2822 6f63  codes.append("oc
-00003fb0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00003fc0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00003fd0: 6e64 2822 7073 2229 0d0a 2020 2020 2020  nd("ps")..      
-00003fe0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00003ff0: 732e 6170 7065 6e64 2822 6661 2229 0d0a  s.append("fa")..
-00004000: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00004010: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00004020: 706c 2229 0d0a 2020 2020 2020 2020 7365  pl")..        se
-00004030: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00004040: 7065 6e64 2822 7074 2229 0d0a 2020 2020  pend("pt")..    
-00004050: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00004060: 6465 732e 6170 7065 6e64 2822 7061 2229  des.append("pa")
-00004070: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00004080: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00004090: 2822 726f 2229 0d0a 2020 2020 2020 2020  ("ro")..        
-000040a0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-000040b0: 6170 7065 6e64 2822 7275 2229 0d0a 2020  append("ru")..  
-000040c0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000040d0: 636f 6465 732e 6170 7065 6e64 2822 7361  codes.append("sa
-000040e0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000040f0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00004100: 6e64 2822 7372 2229 0d0a 2020 2020 2020  nd("sr")..      
-00004110: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00004120: 732e 6170 7065 6e64 2822 736e 2229 0d0a  s.append("sn")..
-00004130: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00004140: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00004150: 7364 2229 0d0a 2020 2020 2020 2020 7365  sd")..        se
-00004160: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00004170: 7065 6e64 2822 7369 2229 0d0a 2020 2020  pend("si")..    
-00004180: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00004190: 6465 732e 6170 7065 6e64 2822 736b 2229  des.append("sk")
-000041a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000041b0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-000041c0: 2822 736c 2229 0d0a 2020 2020 2020 2020  ("sl")..        
-000041d0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-000041e0: 6170 7065 6e64 2822 736f 2229 0d0a 2020  append("so")..  
-000041f0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00004200: 636f 6465 732e 6170 7065 6e64 2822 6573  codes.append("es
-00004210: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004220: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00004230: 6e64 2822 7375 2229 0d0a 2020 2020 2020  nd("su")..      
-00004240: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00004250: 732e 6170 7065 6e64 2822 7377 2229 0d0a  s.append("sw")..
-00004260: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00004270: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00004280: 7376 2229 0d0a 2020 2020 2020 2020 7365  sv")..        se
-00004290: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-000042a0: 7065 6e64 2822 746c 2229 0d0a 2020 2020  pend("tl")..    
-000042b0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000042c0: 6465 732e 6170 7065 6e64 2822 7467 2229  des.append("tg")
-000042d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000042e0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-000042f0: 2822 7461 2229 0d0a 2020 2020 2020 2020  ("ta")..        
-00004300: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00004310: 6170 7065 6e64 2822 7474 2229 0d0a 2020  append("tt")..  
-00004320: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00004330: 636f 6465 732e 6170 7065 6e64 2822 7465  codes.append("te
-00004340: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004350: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00004360: 6e64 2822 7468 2229 0d0a 2020 2020 2020  nd("th")..      
-00004370: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00004380: 732e 6170 7065 6e64 2822 626f 2229 0d0a  s.append("bo")..
-00004390: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000043a0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-000043b0: 7472 2229 0d0a 2020 2020 2020 2020 7365  tr")..        se
-000043c0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-000043d0: 7065 6e64 2822 746b 2229 0d0a 2020 2020  pend("tk")..    
-000043e0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000043f0: 6465 732e 6170 7065 6e64 2822 756b 2229  des.append("uk")
-00004400: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00004410: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00004420: 2822 7572 2229 0d0a 2020 2020 2020 2020  ("ur")..        
-00004430: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00004440: 6170 7065 6e64 2822 757a 2229 0d0a 2020  append("uz")..  
-00004450: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00004460: 636f 6465 732e 6170 7065 6e64 2822 7669  codes.append("vi
-00004470: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004480: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00004490: 6e64 2822 6379 2229 0d0a 2020 2020 2020  nd("cy")..      
-000044a0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-000044b0: 732e 6170 7065 6e64 2822 7969 2229 0d0a  s.append("yi")..
-000044c0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000044d0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-000044e0: 796f 2229 0d0a 0d0a 2020 2020 2020 2020  yo")....        
-000044f0: 7365 6c66 2e6c 6973 745f 6e61 6d65 7320  self.list_names 
-00004500: 3d20 5b5d 0d0a 2020 2020 2020 2020 7365  = []..        se
-00004510: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00004520: 7065 6e64 2822 4166 7269 6b61 616e 7322  pend("Afrikaans"
-00004530: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004540: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00004550: 6428 2241 6c62 616e 6961 6e22 290d 0a20  d("Albanian").. 
-00004560: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00004570: 5f6e 616d 6573 2e61 7070 656e 6428 2241  _names.append("A
-00004580: 6d68 6172 6963 2229 0d0a 2020 2020 2020  mharic")..      
-00004590: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-000045a0: 732e 6170 7065 6e64 2822 4172 6162 6963  s.append("Arabic
-000045b0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000045c0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-000045d0: 6e64 2822 4172 6d65 6e69 616e 2229 0d0a  nd("Armenian")..
-000045e0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000045f0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00004600: 4173 7361 6d65 7365 2229 0d0a 2020 2020  Assamese")..    
-00004610: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00004620: 6d65 732e 6170 7065 6e64 2822 417a 6572  mes.append("Azer
-00004630: 6261 696a 616e 6922 290d 0a20 2020 2020  baijani")..     
-00004640: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00004650: 6573 2e61 7070 656e 6428 2242 6173 686b  es.append("Bashk
-00004660: 6972 2229 0d0a 2020 2020 2020 2020 7365  ir")..        se
-00004670: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00004680: 7065 6e64 2822 4261 7371 7565 2229 0d0a  pend("Basque")..
-00004690: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000046a0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000046b0: 4265 6c61 7275 7369 616e 2229 0d0a 2020  Belarusian")..  
-000046c0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000046d0: 6e61 6d65 732e 6170 7065 6e64 2822 4265  names.append("Be
-000046e0: 6e67 616c 6922 290d 0a20 2020 2020 2020  ngali")..       
-000046f0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004700: 2e61 7070 656e 6428 2242 6f73 6e69 616e  .append("Bosnian
-00004710: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004720: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00004730: 6e64 2822 4272 6574 6f6e 2229 0d0a 2020  nd("Breton")..  
-00004740: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00004750: 6e61 6d65 732e 6170 7065 6e64 2822 4275  names.append("Bu
-00004760: 6c67 6172 6961 6e22 290d 0a20 2020 2020  lgarian")..     
-00004770: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00004780: 6573 2e61 7070 656e 6428 2243 6174 616c  es.append("Catal
-00004790: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
-000047a0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-000047b0: 7065 6e64 2822 4368 696e 6573 6522 290d  pend("Chinese").
-000047c0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000047d0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-000047e0: 2243 726f 6174 6961 6e22 290d 0a20 2020  "Croatian")..   
-000047f0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004800: 616d 6573 2e61 7070 656e 6428 2243 7a65  ames.append("Cze
-00004810: 6368 2229 0d0a 2020 2020 2020 2020 7365  ch")..        se
-00004820: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00004830: 7065 6e64 2822 4461 6e69 7368 2229 0d0a  pend("Danish")..
-00004840: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00004850: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00004860: 4475 7463 6822 290d 0a20 2020 2020 2020  Dutch")..       
-00004870: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004880: 2e61 7070 656e 6428 2245 6e67 6c69 7368  .append("English
-00004890: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000048a0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-000048b0: 6e64 2822 4573 746f 6e69 616e 2229 0d0a  nd("Estonian")..
-000048c0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000048d0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000048e0: 4661 726f 6573 6522 290d 0a20 2020 2020  Faroese")..     
-000048f0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00004900: 6573 2e61 7070 656e 6428 2246 696e 6e69  es.append("Finni
-00004910: 7368 2229 0d0a 2020 2020 2020 2020 7365  sh")..        se
-00004920: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00004930: 7065 6e64 2822 4672 656e 6368 2229 0d0a  pend("French")..
-00004940: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00004950: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00004960: 4761 6c69 6369 616e 2229 0d0a 2020 2020  Galician")..    
-00004970: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00004980: 6d65 732e 6170 7065 6e64 2822 4765 6f72  mes.append("Geor
-00004990: 6769 616e 2229 0d0a 2020 2020 2020 2020  gian")..        
-000049a0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-000049b0: 6170 7065 6e64 2822 4765 726d 616e 2229  append("German")
-000049c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000049d0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-000049e0: 2822 4772 6565 6b22 290d 0a20 2020 2020  ("Greek")..     
-000049f0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00004a00: 6573 2e61 7070 656e 6428 2247 756a 6172  es.append("Gujar
-00004a10: 6174 6922 290d 0a20 2020 2020 2020 2073  ati")..        s
-00004a20: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00004a30: 7070 656e 6428 2248 6169 7469 616e 2043  ppend("Haitian C
-00004a40: 7265 6f6c 6522 290d 0a20 2020 2020 2020  reole")..       
-00004a50: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004a60: 2e61 7070 656e 6428 2248 6175 7361 2229  .append("Hausa")
-00004a70: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00004a80: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00004a90: 2822 4861 7761 6969 616e 2229 0d0a 2020  ("Hawaiian")..  
-00004aa0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00004ab0: 6e61 6d65 732e 6170 7065 6e64 2822 4865  names.append("He
-00004ac0: 6272 6577 2229 0d0a 2020 2020 2020 2020  brew")..        
-00004ad0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00004ae0: 6170 7065 6e64 2822 4869 6e64 6922 290d  append("Hindi").
-00004af0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004b00: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00004b10: 2248 756e 6761 7269 616e 2229 0d0a 2020  "Hungarian")..  
-00004b20: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00004b30: 6e61 6d65 732e 6170 7065 6e64 2822 4963  names.append("Ic
-00004b40: 656c 616e 6469 6322 290d 0a20 2020 2020  elandic")..     
-00004b50: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00004b60: 6573 2e61 7070 656e 6428 2249 6e64 6f6e  es.append("Indon
-00004b70: 6573 6961 6e22 290d 0a20 2020 2020 2020  esian")..       
-00004b80: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004b90: 2e61 7070 656e 6428 2249 7461 6c69 616e  .append("Italian
-00004ba0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004bb0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00004bc0: 6e64 2822 4a61 7061 6e65 7365 2229 0d0a  nd("Japanese")..
-00004bd0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00004be0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00004bf0: 4a61 7661 6e65 7365 2229 0d0a 2020 2020  Javanese")..    
-00004c00: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00004c10: 6d65 732e 6170 7065 6e64 2822 4b61 6e6e  mes.append("Kann
-00004c20: 6164 6122 290d 0a20 2020 2020 2020 2073  ada")..        s
-00004c30: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00004c40: 7070 656e 6428 224b 617a 616b 6822 290d  ppend("Kazakh").
-00004c50: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004c60: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00004c70: 224b 686d 6572 2229 0d0a 2020 2020 2020  "Khmer")..      
-00004c80: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00004c90: 732e 6170 7065 6e64 2822 4b6f 7265 616e  s.append("Korean
-00004ca0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004cb0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00004cc0: 6e64 2822 4c61 6f22 290d 0a20 2020 2020  nd("Lao")..     
-00004cd0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00004ce0: 6573 2e61 7070 656e 6428 224c 6174 696e  es.append("Latin
-00004cf0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004d00: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00004d10: 6e64 2822 4c61 7476 6961 6e22 290d 0a20  nd("Latvian").. 
-00004d20: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00004d30: 5f6e 616d 6573 2e61 7070 656e 6428 224c  _names.append("L
-00004d40: 696e 6761 6c61 2229 0d0a 2020 2020 2020  ingala")..      
-00004d50: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00004d60: 732e 6170 7065 6e64 2822 4c69 7468 7561  s.append("Lithua
-00004d70: 6e69 616e 2229 0d0a 2020 2020 2020 2020  nian")..        
-00004d80: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00004d90: 6170 7065 6e64 2822 4c75 7865 6d62 6f75  append("Luxembou
-00004da0: 7267 6973 6822 290d 0a20 2020 2020 2020  rgish")..       
-00004db0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004dc0: 2e61 7070 656e 6428 224d 6163 6564 6f6e  .append("Macedon
-00004dd0: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
-00004de0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00004df0: 7070 656e 6428 224d 616c 6167 6173 7922  ppend("Malagasy"
-00004e00: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004e10: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00004e20: 6428 224d 616c 6179 2229 0d0a 2020 2020  d("Malay")..    
-00004e30: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00004e40: 6d65 732e 6170 7065 6e64 2822 4d61 6c61  mes.append("Mala
-00004e50: 7961 6c61 6d22 290d 0a20 2020 2020 2020  yalam")..       
-00004e60: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00004e70: 2e61 7070 656e 6428 224d 616c 7465 7365  .append("Maltese
-00004e80: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004e90: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00004ea0: 6e64 2822 4d61 6f72 6922 290d 0a20 2020  nd("Maori")..   
-00004eb0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00004ec0: 616d 6573 2e61 7070 656e 6428 224d 6172  ames.append("Mar
-00004ed0: 6174 6869 2229 0d0a 2020 2020 2020 2020  athi")..        
-00004ee0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00004ef0: 6170 7065 6e64 2822 4d6f 6e67 6f6c 6961  append("Mongolia
-00004f00: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
-00004f10: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00004f20: 656e 6428 224d 7961 6e6d 6172 2028 4275  end("Myanmar (Bu
-00004f30: 726d 6573 6529 2229 0d0a 2020 2020 2020  rmese)")..      
-00004f40: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00004f50: 732e 6170 7065 6e64 2822 4e65 7061 6c69  s.append("Nepali
-00004f60: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00004f70: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00004f80: 6e64 2822 4e6f 7277 6567 6961 6e22 290d  nd("Norwegian").
-00004f90: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00004fa0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00004fb0: 224e 796e 6f72 736b 2229 0d0a 2020 2020  "Nynorsk")..    
-00004fc0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00004fd0: 6d65 732e 6170 7065 6e64 2822 4f63 6369  mes.append("Occi
-00004fe0: 7461 6e22 290d 0a20 2020 2020 2020 2073  tan")..        s
-00004ff0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00005000: 7070 656e 6428 2250 6173 6874 6f22 290d  ppend("Pashto").
-00005010: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00005020: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00005030: 2250 6572 7369 616e 2229 0d0a 2020 2020  "Persian")..    
-00005040: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00005050: 6d65 732e 6170 7065 6e64 2822 506f 6c69  mes.append("Poli
-00005060: 7368 2229 0d0a 2020 2020 2020 2020 7365  sh")..        se
-00005070: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00005080: 7065 6e64 2822 506f 7274 7567 7565 7365  pend("Portuguese
-00005090: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000050a0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-000050b0: 6e64 2822 5075 6e6a 6162 6922 290d 0a20  nd("Punjabi").. 
-000050c0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000050d0: 5f6e 616d 6573 2e61 7070 656e 6428 2252  _names.append("R
-000050e0: 6f6d 616e 6961 6e22 290d 0a20 2020 2020  omanian")..     
-000050f0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00005100: 6573 2e61 7070 656e 6428 2252 7573 7369  es.append("Russi
-00005110: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
-00005120: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00005130: 7065 6e64 2822 5361 6e73 6b72 6974 2229  pend("Sanskrit")
-00005140: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00005150: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00005160: 2822 5365 7262 6961 6e22 290d 0a20 2020  ("Serbian")..   
-00005170: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00005180: 616d 6573 2e61 7070 656e 6428 2253 686f  ames.append("Sho
-00005190: 6e61 2229 0d0a 2020 2020 2020 2020 7365  na")..        se
-000051a0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-000051b0: 7065 6e64 2822 5369 6e64 6869 2229 0d0a  pend("Sindhi")..
-000051c0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000051d0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000051e0: 5369 6e68 616c 6122 290d 0a20 2020 2020  Sinhala")..     
-000051f0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00005200: 6573 2e61 7070 656e 6428 2253 6c6f 7661  es.append("Slova
-00005210: 6b22 290d 0a20 2020 2020 2020 2073 656c  k")..        sel
-00005220: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00005230: 656e 6428 2253 6c6f 7665 6e69 616e 2229  end("Slovenian")
-00005240: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00005250: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00005260: 2822 536f 6d61 6c69 2229 0d0a 2020 2020  ("Somali")..    
-00005270: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00005280: 6d65 732e 6170 7065 6e64 2822 5370 616e  mes.append("Span
-00005290: 6973 6822 290d 0a20 2020 2020 2020 2073  ish")..        s
-000052a0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-000052b0: 7070 656e 6428 2253 756e 6461 6e65 7365  ppend("Sundanese
-000052c0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000052d0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-000052e0: 6e64 2822 5377 6168 696c 6922 290d 0a20  nd("Swahili").. 
-000052f0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00005300: 5f6e 616d 6573 2e61 7070 656e 6428 2253  _names.append("S
-00005310: 7765 6469 7368 2229 0d0a 2020 2020 2020  wedish")..      
-00005320: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00005330: 732e 6170 7065 6e64 2822 5461 6761 6c6f  s.append("Tagalo
-00005340: 6722 290d 0a20 2020 2020 2020 2073 656c  g")..        sel
-00005350: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00005360: 656e 6428 2254 616a 696b 2229 0d0a 2020  end("Tajik")..  
-00005370: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00005380: 6e61 6d65 732e 6170 7065 6e64 2822 5461  names.append("Ta
-00005390: 6d69 6c22 290d 0a20 2020 2020 2020 2073  mil")..        s
-000053a0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-000053b0: 7070 656e 6428 2254 6174 6172 2229 0d0a  ppend("Tatar")..
-000053c0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000053d0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000053e0: 5465 6c75 6775 2229 0d0a 2020 2020 2020  Telugu")..      
-000053f0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00005400: 732e 6170 7065 6e64 2822 5468 6169 2229  s.append("Thai")
-00005410: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00005420: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00005430: 2822 5469 6265 7461 6e22 290d 0a20 2020  ("Tibetan")..   
-00005440: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00005450: 616d 6573 2e61 7070 656e 6428 2254 7572  ames.append("Tur
-00005460: 6b69 7368 2229 0d0a 2020 2020 2020 2020  kish")..        
-00005470: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00005480: 6170 7065 6e64 2822 5475 726b 6d65 6e22  append("Turkmen"
-00005490: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000054a0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-000054b0: 6428 2255 6b72 6169 6e69 616e 2229 0d0a  d("Ukrainian")..
-000054c0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000054d0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000054e0: 5572 6475 2229 0d0a 2020 2020 2020 2020  Urdu")..        
-000054f0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00005500: 6170 7065 6e64 2822 557a 6265 6b22 290d  append("Uzbek").
-00005510: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00005520: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00005530: 2256 6965 746e 616d 6573 6522 290d 0a20  "Vietnamese").. 
-00005540: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00005550: 5f6e 616d 6573 2e61 7070 656e 6428 2257  _names.append("W
-00005560: 656c 7368 2229 0d0a 2020 2020 2020 2020  elsh")..        
-00005570: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00005580: 6170 7065 6e64 2822 5969 6464 6973 6822  append("Yiddish"
-00005590: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000055a0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-000055b0: 6428 2259 6f72 7562 6122 290d 0a0d 0a20  d("Yoruba").... 
-000055c0: 2020 2020 2020 2073 656c 662e 636f 6465         self.code
-000055d0: 5f6f 665f 6e61 6d65 203d 2064 6963 7428  _of_name = dict(
-000055e0: 7a69 7028 7365 6c66 2e6c 6973 745f 6e61  zip(self.list_na
-000055f0: 6d65 732c 2073 656c 662e 6c69 7374 5f63  mes, self.list_c
-00005600: 6f64 6573 2929 0d0a 2020 2020 2020 2020  odes))..        
-00005610: 7365 6c66 2e6e 616d 655f 6f66 5f63 6f64  self.name_of_cod
-00005620: 6520 3d20 6469 6374 287a 6970 2873 656c  e = dict(zip(sel
-00005630: 662e 6c69 7374 5f63 6f64 6573 2c20 7365  f.list_codes, se
-00005640: 6c66 2e6c 6973 745f 6e61 6d65 7329 290d  lf.list_names)).
-00005650: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-00005660: 6469 6374 203d 207b 0d0a 2020 2020 2020  dict = {..      
-00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005680: 2020 2761 6627 3a20 2741 6672 696b 6161    'af': 'Afrikaa
-00005690: 6e73 272c 0d0a 2020 2020 2020 2020 2020  ns',..          
-000056a0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-000056b0: 7127 3a20 2741 6c62 616e 6961 6e27 2c0d  q': 'Albanian',.
-000056c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000056d0: 2020 2020 2020 2020 2027 616d 273a 2027           'am': '
-000056e0: 416d 6861 7269 6327 2c0d 0a20 2020 2020  Amharic',..     
-000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005700: 2020 2027 6172 273a 2027 4172 6162 6963     'ar': 'Arabic
-00005710: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005720: 2020 2020 2020 2020 2020 2020 2768 7927              'hy'
-00005730: 3a20 2741 726d 656e 6961 6e27 2c0d 0a20  : 'Armenian',.. 
-00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005750: 2020 2020 2020 2027 6173 273a 2027 4173         'as': 'As
-00005760: 7361 6d65 7365 272c 0d0a 2020 2020 2020  samese',..      
-00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005780: 2020 2761 7a27 3a20 2741 7a65 7262 6169    'az': 'Azerbai
-00005790: 6a61 6e69 272c 0d0a 2020 2020 2020 2020  jani',..        
-000057a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057b0: 2762 6127 3a20 2742 6173 686b 6972 272c  'ba': 'Bashkir',
-000057c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000057d0: 2020 2020 2020 2020 2020 2765 7527 3a20            'eu': 
-000057e0: 2742 6173 7175 6527 2c0d 0a20 2020 2020  'Basque',..     
-000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005800: 2020 2027 6265 273a 2027 4265 6c61 7275     'be': 'Belaru
-00005810: 7369 616e 272c 0d0a 2020 2020 2020 2020  sian',..        
-00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005830: 2762 6e27 3a20 2742 656e 6761 6c69 272c  'bn': 'Bengali',
-00005840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005850: 2020 2020 2020 2020 2020 2762 7327 3a20            'bs': 
-00005860: 2742 6f73 6e69 616e 272c 0d0a 2020 2020  'Bosnian',..    
-00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005880: 2020 2020 2762 7227 3a20 2742 7265 746f      'br': 'Breto
-00005890: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
-000058a0: 2020 2020 2020 2020 2020 2020 2027 6267               'bg
-000058b0: 273a 2027 4275 6c67 6172 6961 6e27 2c0d  ': 'Bulgarian',.
-000058c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000058d0: 2020 2020 2020 2020 2027 6361 273a 2027           'ca': '
-000058e0: 4361 7461 6c61 6e27 2c0d 0a20 2020 2020  Catalan',..     
-000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005900: 2020 2027 7a68 273a 2027 4368 696e 6573     'zh': 'Chines
-00005910: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
-00005920: 2020 2020 2020 2020 2020 2020 2027 6872               'hr
-00005930: 273a 2027 4372 6f61 7469 616e 272c 0d0a  ': 'Croatian',..
-00005940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005950: 2020 2020 2020 2020 2763 7327 3a20 2743          'cs': 'C
-00005960: 7a65 6368 272c 0d0a 2020 2020 2020 2020  zech',..        
+00001e40: 2062 7265 616b 0d0a 0d0a 2020 2020 2020   break....      
+00001e50: 2020 2020 2020 7374 6465 7272 2e61 7070        stderr.app
+00001e60: 656e 6428 7374 6465 7272 5f6c 696e 652e  end(stderr_line.
+00001e70: 7374 7269 7028 2929 0d0a 0d0a 2020 2020  strip())....    
+00001e80: 2020 2020 2020 2020 7365 6c66 2e73 7464          self.std
+00001e90: 6572 7220 3d20 225c 6e22 2e6a 6f69 6e28  err = "\n".join(
+00001ea0: 7374 6465 7272 290d 0a0d 0a20 2020 2020  stderr)....     
+00001eb0: 2020 2020 2020 2069 6620 746f 7461 6c5f         if total_
+00001ec0: 6475 7220 6973 204e 6f6e 653a 0d0a 2020  dur is None:..  
+00001ed0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00001ee0: 7461 6c5f 6475 725f 6d61 7463 6820 3d20  tal_dur_match = 
+00001ef0: 7365 6c66 2e44 5552 5f52 4547 4558 2e73  self.DUR_REGEX.s
+00001f00: 6561 7263 6828 7374 6465 7272 5f6c 696e  earch(stderr_lin
+00001f10: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00001f20: 2020 2020 6966 2074 6f74 616c 5f64 7572      if total_dur
+00001f30: 5f6d 6174 6368 3a0d 0a20 2020 2020 2020  _match:..       
+00001f40: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
+00001f50: 616c 5f64 7572 203d 2074 6f5f 6d73 282a  al_dur = to_ms(*
+00001f60: 2a74 6f74 616c 5f64 7572 5f6d 6174 6368  *total_dur_match
+00001f70: 2e67 726f 7570 6469 6374 2829 290d 0a20  .groupdict()).. 
+00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f90: 2020 2063 6f6e 7469 6e75 650d 0a20 2020     continue..   
+00001fa0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00001fb0: 6620 6475 7261 7469 6f6e 5f6f 7665 7272  f duration_overr
+00001fc0: 6964 6520 6973 206e 6f74 204e 6f6e 653a  ide is not None:
+00001fd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001fe0: 2020 2020 2020 2320 7573 6520 7468 6520        # use the 
+00001ff0: 6f76 6572 7269 6465 2028 7368 6f75 6c64  override (should
+00002000: 2061 7070 6c79 2069 6e20 7468 6520 6669   apply in the fi
+00002010: 7273 7420 6c6f 6f70 290d 0a20 2020 2020  rst loop)..     
+00002020: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00002030: 6f74 616c 5f64 7572 203d 2069 6e74 2864  otal_dur = int(d
+00002040: 7572 6174 696f 6e5f 6f76 6572 7269 6465  uration_override
+00002050: 202a 2031 3030 3029 0d0a 2020 2020 2020   * 1000)..      
+00002060: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00002070: 6e74 696e 7565 0d0a 0d0a 2020 2020 2020  ntinue....      
+00002080: 2020 2020 2020 6966 2074 6f74 616c 5f64        if total_d
+00002090: 7572 3a0d 0a20 2020 2020 2020 2020 2020  ur:..           
+000020a0: 2020 2020 2070 726f 6772 6573 735f 7469       progress_ti
+000020b0: 6d65 203d 2046 666d 7065 6750 726f 6772  me = FfmpegProgr
+000020c0: 6573 732e 5449 4d45 5f52 4547 4558 2e73  ess.TIME_REGEX.s
+000020d0: 6561 7263 6828 7374 6465 7272 5f6c 696e  earch(stderr_lin
+000020e0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+000020f0: 2020 2020 6966 2070 726f 6772 6573 735f      if progress_
+00002100: 7469 6d65 3a0d 0a20 2020 2020 2020 2020  time:..         
+00002110: 2020 2020 2020 2020 2020 2065 6c61 7073             elaps
+00002120: 6564 5f74 696d 6520 3d20 746f 5f6d 7328  ed_time = to_ms(
+00002130: 2a2a 7072 6f67 7265 7373 5f74 696d 652e  **progress_time.
+00002140: 6772 6f75 7064 6963 7428 2929 0d0a 2020  groupdict())..  
+00002150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002160: 2020 7969 656c 6420 696e 7428 656c 6170    yield int(elap
+00002170: 7365 645f 7469 6d65 202a 2031 3030 2f20  sed_time * 100/ 
+00002180: 746f 7461 6c5f 6475 7229 0d0a 0d0a 2020  total_dur)....  
+00002190: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+000021a0: 6f63 6573 7320 6973 204e 6f6e 6520 6f72  ocess is None or
+000021b0: 2073 656c 662e 7072 6f63 6573 732e 7265   self.process.re
+000021c0: 7475 726e 636f 6465 2021 3d20 303a 0d0a  turncode != 0:..
+000021d0: 2020 2020 2020 2020 2020 2020 5f70 7265              _pre
+000021e0: 7474 795f 7374 6465 7272 203d 2022 5c6e  tty_stderr = "\n
+000021f0: 222e 6a6f 696e 2873 7464 6572 7229 0d0a  ".join(stderr)..
+00002200: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00002210: 6520 5275 6e74 696d 6545 7272 6f72 2866  e RuntimeError(f
+00002220: 2245 7272 6f72 2072 756e 6e69 6e67 2063  "Error running c
+00002230: 6f6d 6d61 6e64 207b 7365 6c66 2e63 6d64  ommand {self.cmd
+00002240: 7d3a 207b 5f70 7265 7474 795f 7374 6465  }: {_pretty_stde
+00002250: 7272 7d22 290d 0a0d 0a20 2020 2020 2020  rr}")....       
+00002260: 2079 6965 6c64 2031 3030 0d0a 2020 2020   yield 100..    
+00002270: 2020 2020 7365 6c66 2e70 726f 6365 7373      self.process
+00002280: 203d 204e 6f6e 650d 0a0d 0a20 2020 2064   = None....    d
+00002290: 6566 2071 7569 745f 6772 6163 6566 756c  ef quit_graceful
+000022a0: 6c79 2873 656c 6629 202d 3e20 4e6f 6e65  ly(self) -> None
+000022b0: 3a0d 0a20 2020 2020 2020 2027 2727 0d0a  :..        '''..
+000022c0: 2020 2020 2020 2020 5175 6974 2074 6865          Quit the
+000022d0: 2066 666d 7065 6720 7072 6f63 6573 7320   ffmpeg process 
+000022e0: 6279 2073 656e 6469 6e67 2027 7127 0d0a  by sending 'q'..
+000022f0: 0d0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
+00002300: 3a0d 0a20 2020 2020 2020 2020 2020 2052  :..            R
+00002310: 756e 7469 6d65 4572 726f 723a 2049 6620  untimeError: If 
+00002320: 6e6f 2070 726f 6365 7373 2069 7320 666f  no process is fo
+00002330: 756e 642e 0d0a 2020 2020 2020 2020 2727  und...        ''
+00002340: 270d 0a20 2020 2020 2020 2069 6620 7365  '..        if se
+00002350: 6c66 2e70 726f 6365 7373 2069 7320 4e6f  lf.process is No
+00002360: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00002370: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
+00002380: 726f 7228 224e 6f20 7072 6f63 6573 7320  ror("No process 
+00002390: 666f 756e 642e 2044 6964 2079 6f75 2072  found. Did you r
+000023a0: 756e 2074 6865 2063 6f6d 6d61 6e64 3f22  un the command?"
+000023b0: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
+000023c0: 662e 7072 6f63 6573 732e 636f 6d6d 756e  f.process.commun
+000023d0: 6963 6174 6528 696e 7075 743d 6222 7122  icate(input=b"q"
+000023e0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000023f0: 7072 6f63 6573 732e 6b69 6c6c 2829 0d0a  process.kill()..
+00002400: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+00002410: 6365 7373 203d 204e 6f6e 650d 0a0d 0a20  cess = None.... 
+00002420: 2020 2064 6566 2071 7569 7428 7365 6c66     def quit(self
+00002430: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+00002440: 2020 2020 2727 270d 0a20 2020 2020 2020      '''..       
+00002450: 2051 7569 7420 7468 6520 6666 6d70 6567   Quit the ffmpeg
+00002460: 2070 726f 6365 7373 2062 7920 7365 6e64   process by send
+00002470: 696e 6720 5349 474b 494c 4c2e 0d0a 0d0a  ing SIGKILL.....
+00002480: 2020 2020 2020 2020 5261 6973 6573 3a0d          Raises:.
+00002490: 0a20 2020 2020 2020 2020 2020 2052 756e  .            Run
+000024a0: 7469 6d65 4572 726f 723a 2049 6620 6e6f  timeError: If no
+000024b0: 2070 726f 6365 7373 2069 7320 666f 756e   process is foun
+000024c0: 642e 0d0a 2020 2020 2020 2020 2727 270d  d...        '''.
+000024d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000024e0: 2e70 726f 6365 7373 2069 7320 4e6f 6e65  .process is None
+000024f0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00002500: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
+00002510: 7228 224e 6f20 7072 6f63 6573 7320 666f  r("No process fo
+00002520: 756e 642e 2044 6964 2079 6f75 2072 756e  und. Did you run
+00002530: 2074 6865 2063 6f6d 6d61 6e64 3f22 290d   the command?").
+00002540: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+00002550: 7072 6f63 6573 732e 6b69 6c6c 2829 0d0a  process.kill()..
+00002560: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+00002570: 6365 7373 203d 204e 6f6e 650d 0a0d 0a0d  cess = None.....
+00002580: 0a23 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .#==============
+00002590: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000025a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000025b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000025c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000025d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000025e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000025f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002600: 3d3d 3d3d 3d3d 3d3d 3d23 0d0a 0d0a 0d0a  =========#......
+00002610: 6465 6620 7374 6f70 5f66 666d 7065 675f  def stop_ffmpeg_
+00002620: 7769 6e64 6f77 7328 6572 726f 725f 6d65  windows(error_me
+00002630: 7373 6167 6573 5f63 616c 6c62 6163 6b3d  ssages_callback=
+00002640: 4e6f 6e65 293a 0d0a 2020 2020 7472 793a  None):..    try:
+00002650: 0d0a 2020 2020 2020 2020 7461 736b 6c69  ..        taskli
+00002660: 7374 5f6f 7574 7075 7420 3d20 7375 6270  st_output = subp
+00002670: 726f 6365 7373 2e63 6865 636b 5f6f 7574  rocess.check_out
+00002680: 7075 7428 5b27 7461 736b 6c69 7374 275d  put(['tasklist']
+00002690: 2c20 6372 6561 7469 6f6e 666c 6167 733d  , creationflags=
+000026a0: 7375 6270 726f 6365 7373 2e43 5245 4154  subprocess.CREAT
+000026b0: 455f 4e4f 5f57 494e 444f 5729 2e64 6563  E_NO_WINDOW).dec
+000026c0: 6f64 6528 2775 7466 2d38 2729 0d0a 2020  ode('utf-8')..  
+000026d0: 2020 2020 2020 6666 6d70 6567 5f70 6964        ffmpeg_pid
+000026e0: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
+000026f0: 2066 6f72 206c 696e 6520 696e 2074 6173   for line in tas
+00002700: 6b6c 6973 745f 6f75 7470 7574 2e73 706c  klist_output.spl
+00002710: 6974 2827 5c6e 2729 3a0d 0a20 2020 2020  it('\n'):..     
+00002720: 2020 2020 2020 2069 6620 2266 666d 7065         if "ffmpe
+00002730: 6722 2069 6e20 6c69 6e65 3a0d 0a20 2020  g" in line:..   
+00002740: 2020 2020 2020 2020 2020 2020 2066 666d               ffm
+00002750: 7065 675f 7069 6420 3d20 6c69 6e65 2e73  peg_pid = line.s
+00002760: 706c 6974 2829 5b31 5d0d 0a20 2020 2020  plit()[1]..     
+00002770: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00002780: 0d0a 2020 2020 2020 2020 6966 2066 666d  ..        if ffm
+00002790: 7065 675f 7069 643a 0d0a 2020 2020 2020  peg_pid:..      
+000027a0: 2020 2020 2020 6465 766e 756c 6c20 3d20        devnull = 
+000027b0: 6f70 656e 286f 732e 6465 766e 756c 6c2c  open(os.devnull,
+000027c0: 2027 7727 290d 0a20 2020 2020 2020 2020   'w')..         
+000027d0: 2020 2073 7562 7072 6f63 6573 732e 506f     subprocess.Po
+000027e0: 7065 6e28 5b27 7461 736b 6b69 6c6c 272c  pen(['taskkill',
+000027f0: 2027 2f46 272c 2027 2f54 272c 2027 2f50   '/F', '/T', '/P
+00002800: 4944 272c 2066 666d 7065 675f 7069 645d  ID', ffmpeg_pid]
+00002810: 2c20 7374 646f 7574 3d73 7562 7072 6f63  , stdout=subproc
+00002820: 6573 732e 5049 5045 2c20 7374 6465 7272  ess.PIPE, stderr
+00002830: 3d73 7562 7072 6f63 6573 732e 5354 444f  =subprocess.STDO
+00002840: 5554 2c20 7368 656c 6c3d 5472 7565 2c20  UT, shell=True, 
+00002850: 6372 6561 7469 6f6e 666c 6167 733d 7375  creationflags=su
+00002860: 6270 726f 6365 7373 2e43 5245 4154 455f  bprocess.CREATE_
+00002870: 4e4f 5f57 494e 444f 5729 0d0a 0d0a 2020  NO_WINDOW)....  
+00002880: 2020 6578 6365 7074 204b 6579 626f 6172    except Keyboar
+00002890: 6449 6e74 6572 7275 7074 3a0d 0a20 2020  dInterrupt:..   
+000028a0: 2020 2020 2069 6620 6572 726f 725f 6d65       if error_me
+000028b0: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
+000028c0: 0d0a 2020 2020 2020 2020 2020 2020 6572  ..            er
+000028d0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+000028e0: 6c62 6163 6b28 2243 616e 6365 6c6c 696e  lback("Cancellin
+000028f0: 6720 616c 6c20 7461 736b 7322 290d 0a20  g all tasks").. 
+00002900: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00002910: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00002920: 2243 616e 6365 6c6c 696e 6720 616c 6c20  "Cancelling all 
+00002930: 7461 736b 7322 290d 0a20 2020 2020 2020  tasks")..       
+00002940: 2072 6574 7572 6e0d 0a0d 0a20 2020 2065   return....    e
+00002950: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00002960: 6173 2065 3a0d 0a20 2020 2020 2020 2069  as e:..        i
+00002970: 6620 6572 726f 725f 6d65 7373 6167 6573  f error_messages
+00002980: 5f63 616c 6c62 6163 6b3a 0d0a 2020 2020  _callback:..    
+00002990: 2020 2020 2020 2020 6572 726f 725f 6d65          error_me
+000029a0: 7373 6167 6573 5f63 616c 6c62 6163 6b28  ssages_callback(
+000029b0: 6529 0d0a 2020 2020 2020 2020 656c 7365  e)..        else
+000029c0: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+000029d0: 7269 6e74 2865 290d 0a20 2020 2020 2020  rint(e)..       
+000029e0: 2072 6574 7572 6e0d 0a0d 0a0d 0a64 6566   return......def
+000029f0: 2073 746f 705f 6666 6d70 6567 5f6c 696e   stop_ffmpeg_lin
+00002a00: 7578 2865 7272 6f72 5f6d 6573 7361 6765  ux(error_message
+00002a10: 735f 6361 6c6c 6261 636b 3d4e 6f6e 6529  s_callback=None)
+00002a20: 3a0d 0a20 2020 2070 726f 6365 7373 5f6e  :..    process_n
+00002a30: 616d 6520 3d20 2766 666d 7065 6727 0d0a  ame = 'ffmpeg'..
+00002a40: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00002a50: 2020 6f75 7470 7574 203d 2073 7562 7072    output = subpr
+00002a60: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
+00002a70: 7574 285b 2770 7327 2c20 272d 6566 275d  ut(['ps', '-ef']
+00002a80: 290d 0a20 2020 2020 2020 2070 6964 203d  )..        pid =
+00002a90: 205b 6c69 6e65 2e73 706c 6974 2829 5b31   [line.split()[1
+00002aa0: 5d20 666f 7220 6c69 6e65 2069 6e20 6f75  ] for line in ou
+00002ab0: 7470 7574 2e64 6563 6f64 6528 2775 7466  tput.decode('utf
+00002ac0: 2d38 2729 2e73 706c 6974 2827 5c6e 2729  -8').split('\n')
+00002ad0: 2069 6620 7072 6f63 6573 735f 6e61 6d65   if process_name
+00002ae0: 2069 6e20 6c69 6e65 5d5b 305d 0d0a 2020   in line][0]..  
+00002af0: 2020 2020 2020 7375 6270 726f 6365 7373        subprocess
+00002b00: 2e63 616c 6c28 5b27 6b69 6c6c 272c 2027  .call(['kill', '
+00002b10: 2d39 272c 2073 7472 2870 6964 295d 290d  -9', str(pid)]).
+00002b20: 0a20 2020 2065 7863 6570 7420 496e 6465  .    except Inde
+00002b30: 7845 7272 6f72 3a0d 0a20 2020 2020 2020  xError:..       
+00002b40: 2070 6173 730d 0a0d 0a20 2020 2065 7863   pass....    exc
+00002b50: 6570 7420 4b65 7962 6f61 7264 496e 7465  ept KeyboardInte
+00002b60: 7272 7570 743a 0d0a 2020 2020 2020 2020  rrupt:..        
+00002b70: 6966 2065 7272 6f72 5f6d 6573 7361 6765  if error_message
+00002b80: 735f 6361 6c6c 6261 636b 3a0d 0a20 2020  s_callback:..   
+00002b90: 2020 2020 2020 2020 2065 7272 6f72 5f6d           error_m
+00002ba0: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+00002bb0: 2822 4361 6e63 656c 6c69 6e67 2061 6c6c  ("Cancelling all
+00002bc0: 2074 6173 6b73 2229 0d0a 2020 2020 2020   tasks")..      
+00002bd0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00002be0: 2020 2020 2070 7269 6e74 2822 4361 6e63       print("Canc
+00002bf0: 656c 6c69 6e67 2061 6c6c 2074 6173 6b73  elling all tasks
+00002c00: 2229 0d0a 2020 2020 2020 2020 7265 7475  ")..        retu
+00002c10: 726e 0d0a 0d0a 2020 2020 6578 6365 7074  rn....    except
+00002c20: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+00002c30: 0d0a 2020 2020 2020 2020 6966 2065 7272  ..        if err
+00002c40: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+00002c50: 6261 636b 3a0d 0a20 2020 2020 2020 2020  back:..         
+00002c60: 2020 2065 7272 6f72 5f6d 6573 7361 6765     error_message
+00002c70: 735f 6361 6c6c 6261 636b 2865 290d 0a20  s_callback(e).. 
+00002c80: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00002c90: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00002ca0: 6529 0d0a 2020 2020 2020 2020 7265 7475  e)..        retu
+00002cb0: 726e 0d0a 0d0a 0d0a 6465 6620 7265 6d6f  rn......def remo
+00002cc0: 7665 5f74 656d 705f 6669 6c65 7328 6578  ve_temp_files(ex
+00002cd0: 7465 6e73 696f 6e2c 2065 7272 6f72 5f6d  tension, error_m
+00002ce0: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+00002cf0: 3d4e 6f6e 6529 3a0d 0a20 2020 2074 7279  =None):..    try
+00002d00: 3a0d 0a20 2020 2020 2020 2074 656d 705f  :..        temp_
+00002d10: 6469 7220 3d20 7465 6d70 6669 6c65 2e67  dir = tempfile.g
+00002d20: 6574 7465 6d70 6469 7228 290d 0a20 2020  ettempdir()..   
+00002d30: 2020 2020 2066 6f72 2072 6f6f 742c 2064       for root, d
+00002d40: 6972 732c 2066 696c 6573 2069 6e20 6f73  irs, files in os
+00002d50: 2e77 616c 6b28 7465 6d70 5f64 6972 293a  .walk(temp_dir):
+00002d60: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+00002d70: 7220 6669 6c65 2069 6e20 6669 6c65 733a  r file in files:
+00002d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002d90: 2020 6966 2066 696c 652e 656e 6473 7769    if file.endswi
+00002da0: 7468 2822 2e22 202b 2065 7874 656e 7369  th("." + extensi
+00002db0: 6f6e 293a 0d0a 2020 2020 2020 2020 2020  on):..          
+00002dc0: 2020 2020 2020 2020 2020 6f73 2e72 656d            os.rem
+00002dd0: 6f76 6528 6f73 2e70 6174 682e 6a6f 696e  ove(os.path.join
+00002de0: 2872 6f6f 742c 2066 696c 6529 290d 0a20  (root, file)).. 
+00002df0: 2020 2065 7863 6570 7420 4b65 7962 6f61     except Keyboa
+00002e00: 7264 496e 7465 7272 7570 743a 0d0a 2020  rdInterrupt:..  
+00002e10: 2020 2020 2020 6966 2065 7272 6f72 5f6d        if error_m
+00002e20: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+00002e30: 3a0d 0a20 2020 2020 2020 2020 2020 2065  :..            e
+00002e40: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+00002e50: 6c6c 6261 636b 2822 4361 6e63 656c 6c69  llback("Cancelli
+00002e60: 6e67 2061 6c6c 2074 6173 6b73 2229 0d0a  ng all tasks")..
+00002e70: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00002e80: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00002e90: 2822 4361 6e63 656c 6c69 6e67 2061 6c6c  ("Cancelling all
+00002ea0: 2074 6173 6b73 2229 0d0a 2020 2020 2020   tasks")..      
+00002eb0: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
+00002ec0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00002ed0: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
+00002ee0: 6966 2065 7272 6f72 5f6d 6573 7361 6765  if error_message
+00002ef0: 735f 6361 6c6c 6261 636b 3a0d 0a20 2020  s_callback:..   
+00002f00: 2020 2020 2020 2020 2065 7272 6f72 5f6d           error_m
+00002f10: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+00002f20: 2865 290d 0a20 2020 2020 2020 2065 6c73  (e)..        els
+00002f30: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00002f40: 7072 696e 7428 6529 0d0a 2020 2020 2020  print(e)..      
+00002f50: 2020 7265 7475 726e 0d0a 0d0a 0d0a 6465    return......de
+00002f60: 6620 6973 5f73 616d 655f 6c61 6e67 7561  f is_same_langua
+00002f70: 6765 2873 7263 2c20 6473 742c 2065 7272  ge(src, dst, err
+00002f80: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+00002f90: 6261 636b 3d4e 6f6e 6529 3a0d 0a20 2020  back=None):..   
+00002fa0: 2074 7279 3a0d 0a20 2020 2020 2020 2072   try:..        r
+00002fb0: 6574 7572 6e20 7372 632e 7370 6c69 7428  eturn src.split(
+00002fc0: 222d 2229 5b30 5d20 3d3d 2064 7374 2e73  "-")[0] == dst.s
+00002fd0: 706c 6974 2822 2d22 295b 305d 0d0a 2020  plit("-")[0]..  
+00002fe0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00002ff0: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
+00003000: 2020 6966 2065 7272 6f72 5f6d 6573 7361    if error_messa
+00003010: 6765 735f 6361 6c6c 6261 636b 3a0d 0a20  ges_callback:.. 
+00003020: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+00003030: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+00003040: 636b 2865 290d 0a20 2020 2020 2020 2065  ck(e)..        e
+00003050: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00003060: 2020 7072 696e 7428 6529 0d0a 2020 2020    print(e)..    
+00003070: 2020 2020 7265 7475 726e 0d0a 0d0a 0d0a      return......
+00003080: 6465 6620 6368 6563 6b5f 6669 6c65 5f74  def check_file_t
+00003090: 7970 6528 6669 6c65 5f70 6174 682c 2065  ype(file_path, e
+000030a0: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
+000030b0: 6c6c 6261 636b 3d4e 6f6e 6529 3a0d 0a20  llback=None):.. 
+000030c0: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+000030d0: 2066 6670 726f 6265 5f63 6d64 203d 205b   ffprobe_cmd = [
+000030e0: 2766 6670 726f 6265 272c 2027 2d76 272c  'ffprobe', '-v',
+000030f0: 2027 6572 726f 7227 2c20 272d 7368 6f77   'error', '-show
+00003100: 5f66 6f72 6d61 7427 2c20 272d 7368 6f77  _format', '-show
+00003110: 5f73 7472 6561 6d73 272c 2027 2d70 7269  _streams', '-pri
+00003120: 6e74 5f66 6f72 6d61 7427 2c20 276a 736f  nt_format', 'jso
+00003130: 6e27 2c20 6669 6c65 5f70 6174 685d 0d0a  n', file_path]..
+00003140: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
+00003150: 204e 6f6e 650d 0a20 2020 2020 2020 2069   None..        i
+00003160: 6620 7379 732e 706c 6174 666f 726d 203d  f sys.platform =
+00003170: 3d20 2277 696e 3332 223a 0d0a 2020 2020  = "win32":..    
+00003180: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
+00003190: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
+000031a0: 6b5f 6f75 7470 7574 2866 6670 726f 6265  k_output(ffprobe
+000031b0: 5f63 6d64 2c20 6372 6561 7469 6f6e 666c  _cmd, creationfl
+000031c0: 6167 733d 7375 6270 726f 6365 7373 2e43  ags=subprocess.C
+000031d0: 5245 4154 455f 4e4f 5f57 494e 444f 5729  REATE_NO_WINDOW)
+000031e0: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
+000031f0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00003200: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+00003210: 7075 7420 3d20 7375 6270 726f 6365 7373  put = subprocess
+00003220: 2e63 6865 636b 5f6f 7574 7075 7428 6666  .check_output(ff
+00003230: 7072 6f62 655f 636d 6429 2e64 6563 6f64  probe_cmd).decod
+00003240: 6528 2775 7466 2d38 2729 0d0a 2020 2020  e('utf-8')..    
+00003250: 2020 2020 6461 7461 203d 206a 736f 6e2e      data = json.
+00003260: 6c6f 6164 7328 6f75 7470 7574 290d 0a0d  loads(output)...
+00003270: 0a20 2020 2020 2020 2069 6620 2773 7472  .        if 'str
+00003280: 6561 6d73 2720 696e 2064 6174 613a 0d0a  eams' in data:..
+00003290: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000032a0: 7374 7265 616d 2069 6e20 6461 7461 5b27  stream in data['
+000032b0: 7374 7265 616d 7327 5d3a 0d0a 2020 2020  streams']:..    
+000032c0: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+000032d0: 636f 6465 635f 7479 7065 2720 696e 2073  codec_type' in s
+000032e0: 7472 6561 6d20 616e 6420 7374 7265 616d  tream and stream
+000032f0: 5b27 636f 6465 635f 7479 7065 275d 203d  ['codec_type'] =
+00003300: 3d20 2761 7564 696f 273a 0d0a 2020 2020  = 'audio':..    
+00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003320: 7265 7475 726e 2027 6175 6469 6f27 0d0a  return 'audio'..
+00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003340: 656c 6966 2027 636f 6465 635f 7479 7065  elif 'codec_type
+00003350: 2720 696e 2073 7472 6561 6d20 616e 6420  ' in stream and 
+00003360: 7374 7265 616d 5b27 636f 6465 635f 7479  stream['codec_ty
+00003370: 7065 275d 203d 3d20 2776 6964 656f 273a  pe'] == 'video':
+00003380: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003390: 2020 2020 2020 7265 7475 726e 2027 7669        return 'vi
+000033a0: 6465 6f27 0d0a 2020 2020 6578 6365 7074  deo'..    except
+000033b0: 2028 7375 6270 726f 6365 7373 2e43 616c   (subprocess.Cal
+000033c0: 6c65 6450 726f 6365 7373 4572 726f 722c  ledProcessError,
+000033d0: 206a 736f 6e2e 4a53 4f4e 4465 636f 6465   json.JSONDecode
+000033e0: 4572 726f 7229 3a0d 0a20 2020 2020 2020  Error):..       
+000033f0: 2070 6173 730d 0a0d 0a20 2020 2065 7863   pass....    exc
+00003400: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00003410: 2065 3a0d 0a20 2020 2020 2020 2069 6620   e:..        if 
+00003420: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+00003430: 616c 6c62 6163 6b3a 0d0a 2020 2020 2020  allback:..      
+00003440: 2020 2020 2020 6572 726f 725f 6d65 7373        error_mess
+00003450: 6167 6573 5f63 616c 6c62 6163 6b28 6529  ages_callback(e)
+00003460: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00003470: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00003480: 6e74 2865 290d 0a0d 0a20 2020 2072 6574  nt(e)....    ret
+00003490: 7572 6e20 4e6f 6e65 0d0a 0d0a 0d0a 636c  urn None......cl
+000034a0: 6173 7320 5768 6973 7065 724c 616e 6775  ass WhisperLangu
+000034b0: 6167 653a 0d0a 2020 2020 6465 6620 5f5f  age:..    def __
+000034c0: 696e 6974 5f5f 2873 656c 6629 3a0d 0a20  init__(self):.. 
+000034d0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000034e0: 5f63 6f64 6573 203d 205b 5d0d 0a20 2020  _codes = []..   
+000034f0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00003500: 6f64 6573 2e61 7070 656e 6428 2261 6622  odes.append("af"
+00003510: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003520: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00003530: 6428 2273 7122 290d 0a20 2020 2020 2020  d("sq")..       
+00003540: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00003550: 2e61 7070 656e 6428 2261 6d22 290d 0a20  .append("am").. 
+00003560: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00003570: 5f63 6f64 6573 2e61 7070 656e 6428 2261  _codes.append("a
+00003580: 7222 290d 0a20 2020 2020 2020 2073 656c  r")..        sel
+00003590: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+000035a0: 656e 6428 2268 7922 290d 0a20 2020 2020  end("hy")..     
+000035b0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+000035c0: 6573 2e61 7070 656e 6428 2261 7322 290d  es.append("as").
+000035d0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000035e0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+000035f0: 2261 7a22 290d 0a20 2020 2020 2020 2073  "az")..        s
+00003600: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00003610: 7070 656e 6428 2262 6122 290d 0a20 2020  ppend("ba")..   
+00003620: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00003630: 6f64 6573 2e61 7070 656e 6428 2265 7522  odes.append("eu"
+00003640: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003650: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00003660: 6428 2262 6522 290d 0a20 2020 2020 2020  d("be")..       
+00003670: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00003680: 2e61 7070 656e 6428 2262 6e22 290d 0a20  .append("bn").. 
+00003690: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000036a0: 5f63 6f64 6573 2e61 7070 656e 6428 2262  _codes.append("b
+000036b0: 7322 290d 0a20 2020 2020 2020 2073 656c  s")..        sel
+000036c0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+000036d0: 656e 6428 2262 7222 290d 0a20 2020 2020  end("br")..     
+000036e0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+000036f0: 6573 2e61 7070 656e 6428 2262 6722 290d  es.append("bg").
+00003700: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00003710: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00003720: 2263 6122 290d 0a20 2020 2020 2020 2073  "ca")..        s
+00003730: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00003740: 7070 656e 6428 227a 6822 290d 0a20 2020  ppend("zh")..   
+00003750: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00003760: 6f64 6573 2e61 7070 656e 6428 2268 7222  odes.append("hr"
+00003770: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003780: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00003790: 6428 2263 7322 290d 0a20 2020 2020 2020  d("cs")..       
+000037a0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+000037b0: 2e61 7070 656e 6428 2264 6122 290d 0a20  .append("da").. 
+000037c0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000037d0: 5f63 6f64 6573 2e61 7070 656e 6428 226e  _codes.append("n
+000037e0: 6c22 290d 0a20 2020 2020 2020 2073 656c  l")..        sel
+000037f0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00003800: 656e 6428 2265 6e22 290d 0a20 2020 2020  end("en")..     
+00003810: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00003820: 6573 2e61 7070 656e 6428 2265 7422 290d  es.append("et").
+00003830: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00003840: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00003850: 2266 6f22 290d 0a20 2020 2020 2020 2073  "fo")..        s
+00003860: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00003870: 7070 656e 6428 2266 6922 290d 0a20 2020  ppend("fi")..   
+00003880: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00003890: 6f64 6573 2e61 7070 656e 6428 2266 7222  odes.append("fr"
+000038a0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000038b0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+000038c0: 6428 2267 6c22 290d 0a20 2020 2020 2020  d("gl")..       
+000038d0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+000038e0: 2e61 7070 656e 6428 226b 6122 290d 0a20  .append("ka").. 
+000038f0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00003900: 5f63 6f64 6573 2e61 7070 656e 6428 2264  _codes.append("d
+00003910: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
+00003920: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00003930: 656e 6428 2265 6c22 290d 0a20 2020 2020  end("el")..     
+00003940: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00003950: 6573 2e61 7070 656e 6428 2267 7522 290d  es.append("gu").
+00003960: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00003970: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00003980: 2268 7422 290d 0a20 2020 2020 2020 2073  "ht")..        s
+00003990: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+000039a0: 7070 656e 6428 2268 6122 290d 0a20 2020  ppend("ha")..   
+000039b0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+000039c0: 6f64 6573 2e61 7070 656e 6428 2268 6177  odes.append("haw
+000039d0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000039e0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+000039f0: 6e64 2822 6865 2229 0d0a 2020 2020 2020  nd("he")..      
+00003a00: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00003a10: 732e 6170 7065 6e64 2822 6869 2229 0d0a  s.append("hi")..
+00003a20: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00003a30: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00003a40: 6875 2229 0d0a 2020 2020 2020 2020 7365  hu")..        se
+00003a50: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00003a60: 7065 6e64 2822 6973 2229 0d0a 2020 2020  pend("is")..    
+00003a70: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00003a80: 6465 732e 6170 7065 6e64 2822 6964 2229  des.append("id")
+00003a90: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00003aa0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00003ab0: 2822 6974 2229 0d0a 2020 2020 2020 2020  ("it")..        
+00003ac0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00003ad0: 6170 7065 6e64 2822 6a61 2229 0d0a 2020  append("ja")..  
+00003ae0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00003af0: 636f 6465 732e 6170 7065 6e64 2822 6a76  codes.append("jv
+00003b00: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00003b10: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00003b20: 6e64 2822 6b6e 2229 0d0a 2020 2020 2020  nd("kn")..      
+00003b30: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00003b40: 732e 6170 7065 6e64 2822 6b6b 2229 0d0a  s.append("kk")..
+00003b50: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00003b60: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00003b70: 6b6d 2229 0d0a 2020 2020 2020 2020 7365  km")..        se
+00003b80: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00003b90: 7065 6e64 2822 6b6f 2229 0d0a 2020 2020  pend("ko")..    
+00003ba0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00003bb0: 6465 732e 6170 7065 6e64 2822 6c6f 2229  des.append("lo")
+00003bc0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00003bd0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00003be0: 2822 6c61 2229 0d0a 2020 2020 2020 2020  ("la")..        
+00003bf0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00003c00: 6170 7065 6e64 2822 6c76 2229 0d0a 2020  append("lv")..  
+00003c10: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00003c20: 636f 6465 732e 6170 7065 6e64 2822 6c6e  codes.append("ln
+00003c30: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00003c40: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00003c50: 6e64 2822 6c74 2229 0d0a 2020 2020 2020  nd("lt")..      
+00003c60: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00003c70: 732e 6170 7065 6e64 2822 6c62 2229 0d0a  s.append("lb")..
+00003c80: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00003c90: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00003ca0: 6d6b 2229 0d0a 2020 2020 2020 2020 7365  mk")..        se
+00003cb0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00003cc0: 7065 6e64 2822 6d67 2229 0d0a 2020 2020  pend("mg")..    
+00003cd0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00003ce0: 6465 732e 6170 7065 6e64 2822 6d73 2229  des.append("ms")
+00003cf0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00003d00: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00003d10: 2822 6d6c 2229 0d0a 2020 2020 2020 2020  ("ml")..        
+00003d20: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00003d30: 6170 7065 6e64 2822 6d74 2229 0d0a 2020  append("mt")..  
+00003d40: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00003d50: 636f 6465 732e 6170 7065 6e64 2822 6d69  codes.append("mi
+00003d60: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00003d70: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00003d80: 6e64 2822 6d72 2229 0d0a 2020 2020 2020  nd("mr")..      
+00003d90: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00003da0: 732e 6170 7065 6e64 2822 6d6e 2229 0d0a  s.append("mn")..
+00003db0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00003dc0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00003dd0: 6d79 2229 0d0a 2020 2020 2020 2020 7365  my")..        se
+00003de0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00003df0: 7065 6e64 2822 6e65 2229 0d0a 2020 2020  pend("ne")..    
+00003e00: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00003e10: 6465 732e 6170 7065 6e64 2822 6e6f 2229  des.append("no")
+00003e20: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00003e30: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00003e40: 2822 6e6e 2229 0d0a 2020 2020 2020 2020  ("nn")..        
+00003e50: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00003e60: 6170 7065 6e64 2822 6f63 2229 0d0a 2020  append("oc")..  
+00003e70: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00003e80: 636f 6465 732e 6170 7065 6e64 2822 7073  codes.append("ps
+00003e90: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00003ea0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00003eb0: 6e64 2822 6661 2229 0d0a 2020 2020 2020  nd("fa")..      
+00003ec0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00003ed0: 732e 6170 7065 6e64 2822 706c 2229 0d0a  s.append("pl")..
+00003ee0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00003ef0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00003f00: 7074 2229 0d0a 2020 2020 2020 2020 7365  pt")..        se
+00003f10: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00003f20: 7065 6e64 2822 7061 2229 0d0a 2020 2020  pend("pa")..    
+00003f30: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00003f40: 6465 732e 6170 7065 6e64 2822 726f 2229  des.append("ro")
+00003f50: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00003f60: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00003f70: 2822 7275 2229 0d0a 2020 2020 2020 2020  ("ru")..        
+00003f80: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00003f90: 6170 7065 6e64 2822 7361 2229 0d0a 2020  append("sa")..  
+00003fa0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00003fb0: 636f 6465 732e 6170 7065 6e64 2822 7372  codes.append("sr
+00003fc0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00003fd0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00003fe0: 6e64 2822 736e 2229 0d0a 2020 2020 2020  nd("sn")..      
+00003ff0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00004000: 732e 6170 7065 6e64 2822 7364 2229 0d0a  s.append("sd")..
+00004010: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004020: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00004030: 7369 2229 0d0a 2020 2020 2020 2020 7365  si")..        se
+00004040: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00004050: 7065 6e64 2822 736b 2229 0d0a 2020 2020  pend("sk")..    
+00004060: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00004070: 6465 732e 6170 7065 6e64 2822 736c 2229  des.append("sl")
+00004080: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00004090: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+000040a0: 2822 736f 2229 0d0a 2020 2020 2020 2020  ("so")..        
+000040b0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+000040c0: 6170 7065 6e64 2822 6573 2229 0d0a 2020  append("es")..  
+000040d0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000040e0: 636f 6465 732e 6170 7065 6e64 2822 7375  codes.append("su
+000040f0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004100: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00004110: 6e64 2822 7377 2229 0d0a 2020 2020 2020  nd("sw")..      
+00004120: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00004130: 732e 6170 7065 6e64 2822 7376 2229 0d0a  s.append("sv")..
+00004140: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004150: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00004160: 746c 2229 0d0a 2020 2020 2020 2020 7365  tl")..        se
+00004170: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00004180: 7065 6e64 2822 7467 2229 0d0a 2020 2020  pend("tg")..    
+00004190: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+000041a0: 6465 732e 6170 7065 6e64 2822 7461 2229  des.append("ta")
+000041b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000041c0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+000041d0: 2822 7474 2229 0d0a 2020 2020 2020 2020  ("tt")..        
+000041e0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+000041f0: 6170 7065 6e64 2822 7465 2229 0d0a 2020  append("te")..  
+00004200: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004210: 636f 6465 732e 6170 7065 6e64 2822 7468  codes.append("th
+00004220: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004230: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00004240: 6e64 2822 626f 2229 0d0a 2020 2020 2020  nd("bo")..      
+00004250: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00004260: 732e 6170 7065 6e64 2822 7472 2229 0d0a  s.append("tr")..
+00004270: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004280: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00004290: 746b 2229 0d0a 2020 2020 2020 2020 7365  tk")..        se
+000042a0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+000042b0: 7065 6e64 2822 756b 2229 0d0a 2020 2020  pend("uk")..    
+000042c0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+000042d0: 6465 732e 6170 7065 6e64 2822 7572 2229  des.append("ur")
+000042e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000042f0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00004300: 2822 757a 2229 0d0a 2020 2020 2020 2020  ("uz")..        
+00004310: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00004320: 6170 7065 6e64 2822 7669 2229 0d0a 2020  append("vi")..  
+00004330: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004340: 636f 6465 732e 6170 7065 6e64 2822 6379  codes.append("cy
+00004350: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004360: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00004370: 6e64 2822 7969 2229 0d0a 2020 2020 2020  nd("yi")..      
+00004380: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00004390: 732e 6170 7065 6e64 2822 796f 2229 0d0a  s.append("yo")..
+000043a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000043b0: 6973 745f 6e61 6d65 7320 3d20 5b5d 0d0a  ist_names = []..
+000043c0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000043d0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000043e0: 4166 7269 6b61 616e 7322 290d 0a20 2020  Afrikaans")..   
+000043f0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00004400: 616d 6573 2e61 7070 656e 6428 2241 6c62  ames.append("Alb
+00004410: 616e 6961 6e22 290d 0a20 2020 2020 2020  anian")..       
+00004420: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004430: 2e61 7070 656e 6428 2241 6d68 6172 6963  .append("Amharic
+00004440: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004450: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00004460: 6e64 2822 4172 6162 6963 2229 0d0a 2020  nd("Arabic")..  
+00004470: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004480: 6e61 6d65 732e 6170 7065 6e64 2822 4172  names.append("Ar
+00004490: 6d65 6e69 616e 2229 0d0a 2020 2020 2020  menian")..      
+000044a0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+000044b0: 732e 6170 7065 6e64 2822 4173 7361 6d65  s.append("Assame
+000044c0: 7365 2229 0d0a 2020 2020 2020 2020 7365  se")..        se
+000044d0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+000044e0: 7065 6e64 2822 417a 6572 6261 696a 616e  pend("Azerbaijan
+000044f0: 6922 290d 0a20 2020 2020 2020 2073 656c  i")..        sel
+00004500: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00004510: 656e 6428 2242 6173 686b 6972 2229 0d0a  end("Bashkir")..
+00004520: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004530: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00004540: 4261 7371 7565 2229 0d0a 2020 2020 2020  Basque")..      
+00004550: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00004560: 732e 6170 7065 6e64 2822 4265 6c61 7275  s.append("Belaru
+00004570: 7369 616e 2229 0d0a 2020 2020 2020 2020  sian")..        
+00004580: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00004590: 6170 7065 6e64 2822 4265 6e67 616c 6922  append("Bengali"
+000045a0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000045b0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+000045c0: 6428 2242 6f73 6e69 616e 2229 0d0a 2020  d("Bosnian")..  
+000045d0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000045e0: 6e61 6d65 732e 6170 7065 6e64 2822 4272  names.append("Br
+000045f0: 6574 6f6e 2229 0d0a 2020 2020 2020 2020  eton")..        
+00004600: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00004610: 6170 7065 6e64 2822 4275 6c67 6172 6961  append("Bulgaria
+00004620: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00004630: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00004640: 656e 6428 2243 6174 616c 616e 2229 0d0a  end("Catalan")..
+00004650: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004660: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00004670: 4368 696e 6573 6522 290d 0a20 2020 2020  Chinese")..     
+00004680: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004690: 6573 2e61 7070 656e 6428 2243 726f 6174  es.append("Croat
+000046a0: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
+000046b0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+000046c0: 7070 656e 6428 2243 7a65 6368 2229 0d0a  ppend("Czech")..
+000046d0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000046e0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000046f0: 4461 6e69 7368 2229 0d0a 2020 2020 2020  Danish")..      
+00004700: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00004710: 732e 6170 7065 6e64 2822 4475 7463 6822  s.append("Dutch"
+00004720: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004730: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00004740: 6428 2245 6e67 6c69 7368 2229 0d0a 2020  d("English")..  
+00004750: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004760: 6e61 6d65 732e 6170 7065 6e64 2822 4573  names.append("Es
+00004770: 746f 6e69 616e 2229 0d0a 2020 2020 2020  tonian")..      
+00004780: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00004790: 732e 6170 7065 6e64 2822 4661 726f 6573  s.append("Faroes
+000047a0: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
+000047b0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+000047c0: 656e 6428 2246 696e 6e69 7368 2229 0d0a  end("Finnish")..
+000047d0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000047e0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000047f0: 4672 656e 6368 2229 0d0a 2020 2020 2020  French")..      
+00004800: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00004810: 732e 6170 7065 6e64 2822 4761 6c69 6369  s.append("Galici
+00004820: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
+00004830: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00004840: 7065 6e64 2822 4765 6f72 6769 616e 2229  pend("Georgian")
+00004850: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00004860: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00004870: 2822 4765 726d 616e 2229 0d0a 2020 2020  ("German")..    
+00004880: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00004890: 6d65 732e 6170 7065 6e64 2822 4772 6565  mes.append("Gree
+000048a0: 6b22 290d 0a20 2020 2020 2020 2073 656c  k")..        sel
+000048b0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+000048c0: 656e 6428 2247 756a 6172 6174 6922 290d  end("Gujarati").
+000048d0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000048e0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+000048f0: 2248 6169 7469 616e 2043 7265 6f6c 6522  "Haitian Creole"
+00004900: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004910: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00004920: 6428 2248 6175 7361 2229 0d0a 2020 2020  d("Hausa")..    
+00004930: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00004940: 6d65 732e 6170 7065 6e64 2822 4861 7761  mes.append("Hawa
+00004950: 6969 616e 2229 0d0a 2020 2020 2020 2020  iian")..        
+00004960: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00004970: 6170 7065 6e64 2822 4865 6272 6577 2229  append("Hebrew")
+00004980: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00004990: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+000049a0: 2822 4869 6e64 6922 290d 0a20 2020 2020  ("Hindi")..     
+000049b0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+000049c0: 6573 2e61 7070 656e 6428 2248 756e 6761  es.append("Hunga
+000049d0: 7269 616e 2229 0d0a 2020 2020 2020 2020  rian")..        
+000049e0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+000049f0: 6170 7065 6e64 2822 4963 656c 616e 6469  append("Icelandi
+00004a00: 6322 290d 0a20 2020 2020 2020 2073 656c  c")..        sel
+00004a10: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00004a20: 656e 6428 2249 6e64 6f6e 6573 6961 6e22  end("Indonesian"
+00004a30: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004a40: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00004a50: 6428 2249 7461 6c69 616e 2229 0d0a 2020  d("Italian")..  
+00004a60: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004a70: 6e61 6d65 732e 6170 7065 6e64 2822 4a61  names.append("Ja
+00004a80: 7061 6e65 7365 2229 0d0a 2020 2020 2020  panese")..      
+00004a90: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00004aa0: 732e 6170 7065 6e64 2822 4a61 7661 6e65  s.append("Javane
+00004ab0: 7365 2229 0d0a 2020 2020 2020 2020 7365  se")..        se
+00004ac0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00004ad0: 7065 6e64 2822 4b61 6e6e 6164 6122 290d  pend("Kannada").
+00004ae0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004af0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00004b00: 224b 617a 616b 6822 290d 0a20 2020 2020  "Kazakh")..     
+00004b10: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004b20: 6573 2e61 7070 656e 6428 224b 686d 6572  es.append("Khmer
+00004b30: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004b40: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00004b50: 6e64 2822 4b6f 7265 616e 2229 0d0a 2020  nd("Korean")..  
+00004b60: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004b70: 6e61 6d65 732e 6170 7065 6e64 2822 4c61  names.append("La
+00004b80: 6f22 290d 0a20 2020 2020 2020 2073 656c  o")..        sel
+00004b90: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00004ba0: 656e 6428 224c 6174 696e 2229 0d0a 2020  end("Latin")..  
+00004bb0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004bc0: 6e61 6d65 732e 6170 7065 6e64 2822 4c61  names.append("La
+00004bd0: 7476 6961 6e22 290d 0a20 2020 2020 2020  tvian")..       
+00004be0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004bf0: 2e61 7070 656e 6428 224c 696e 6761 6c61  .append("Lingala
+00004c00: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004c10: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00004c20: 6e64 2822 4c69 7468 7561 6e69 616e 2229  nd("Lithuanian")
+00004c30: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00004c40: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00004c50: 2822 4c75 7865 6d62 6f75 7267 6973 6822  ("Luxembourgish"
+00004c60: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004c70: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00004c80: 6428 224d 6163 6564 6f6e 6961 6e22 290d  d("Macedonian").
+00004c90: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004ca0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00004cb0: 224d 616c 6167 6173 7922 290d 0a20 2020  "Malagasy")..   
+00004cc0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00004cd0: 616d 6573 2e61 7070 656e 6428 224d 616c  ames.append("Mal
+00004ce0: 6179 2229 0d0a 2020 2020 2020 2020 7365  ay")..        se
+00004cf0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00004d00: 7065 6e64 2822 4d61 6c61 7961 6c61 6d22  pend("Malayalam"
+00004d10: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004d20: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00004d30: 6428 224d 616c 7465 7365 2229 0d0a 2020  d("Maltese")..  
+00004d40: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004d50: 6e61 6d65 732e 6170 7065 6e64 2822 4d61  names.append("Ma
+00004d60: 6f72 6922 290d 0a20 2020 2020 2020 2073  ori")..        s
+00004d70: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00004d80: 7070 656e 6428 224d 6172 6174 6869 2229  ppend("Marathi")
+00004d90: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00004da0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00004db0: 2822 4d6f 6e67 6f6c 6961 6e22 290d 0a20  ("Mongolian").. 
+00004dc0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00004dd0: 5f6e 616d 6573 2e61 7070 656e 6428 224d  _names.append("M
+00004de0: 7961 6e6d 6172 2028 4275 726d 6573 6529  yanmar (Burmese)
+00004df0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00004e00: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00004e10: 6e64 2822 4e65 7061 6c69 2229 0d0a 2020  nd("Nepali")..  
+00004e20: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004e30: 6e61 6d65 732e 6170 7065 6e64 2822 4e6f  names.append("No
+00004e40: 7277 6567 6961 6e22 290d 0a20 2020 2020  rwegian")..     
+00004e50: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004e60: 6573 2e61 7070 656e 6428 224e 796e 6f72  es.append("Nynor
+00004e70: 736b 2229 0d0a 2020 2020 2020 2020 7365  sk")..        se
+00004e80: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00004e90: 7065 6e64 2822 4f63 6369 7461 6e22 290d  pend("Occitan").
+00004ea0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00004eb0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00004ec0: 2250 6173 6874 6f22 290d 0a20 2020 2020  "Pashto")..     
+00004ed0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00004ee0: 6573 2e61 7070 656e 6428 2250 6572 7369  es.append("Persi
+00004ef0: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
+00004f00: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00004f10: 7065 6e64 2822 506f 6c69 7368 2229 0d0a  pend("Polish")..
+00004f20: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004f30: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00004f40: 506f 7274 7567 7565 7365 2229 0d0a 2020  Portuguese")..  
+00004f50: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00004f60: 6e61 6d65 732e 6170 7065 6e64 2822 5075  names.append("Pu
+00004f70: 6e6a 6162 6922 290d 0a20 2020 2020 2020  njabi")..       
+00004f80: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00004f90: 2e61 7070 656e 6428 2252 6f6d 616e 6961  .append("Romania
+00004fa0: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00004fb0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00004fc0: 656e 6428 2252 7573 7369 616e 2229 0d0a  end("Russian")..
+00004fd0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00004fe0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00004ff0: 5361 6e73 6b72 6974 2229 0d0a 2020 2020  Sanskrit")..    
+00005000: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00005010: 6d65 732e 6170 7065 6e64 2822 5365 7262  mes.append("Serb
+00005020: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
+00005030: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00005040: 7070 656e 6428 2253 686f 6e61 2229 0d0a  ppend("Shona")..
+00005050: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00005060: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00005070: 5369 6e64 6869 2229 0d0a 2020 2020 2020  Sindhi")..      
+00005080: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00005090: 732e 6170 7065 6e64 2822 5369 6e68 616c  s.append("Sinhal
+000050a0: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
+000050b0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+000050c0: 656e 6428 2253 6c6f 7661 6b22 290d 0a20  end("Slovak").. 
+000050d0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000050e0: 5f6e 616d 6573 2e61 7070 656e 6428 2253  _names.append("S
+000050f0: 6c6f 7665 6e69 616e 2229 0d0a 2020 2020  lovenian")..    
+00005100: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00005110: 6d65 732e 6170 7065 6e64 2822 536f 6d61  mes.append("Soma
+00005120: 6c69 2229 0d0a 2020 2020 2020 2020 7365  li")..        se
+00005130: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00005140: 7065 6e64 2822 5370 616e 6973 6822 290d  pend("Spanish").
+00005150: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00005160: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00005170: 2253 756e 6461 6e65 7365 2229 0d0a 2020  "Sundanese")..  
+00005180: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00005190: 6e61 6d65 732e 6170 7065 6e64 2822 5377  names.append("Sw
+000051a0: 6168 696c 6922 290d 0a20 2020 2020 2020  ahili")..       
+000051b0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+000051c0: 2e61 7070 656e 6428 2253 7765 6469 7368  .append("Swedish
+000051d0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000051e0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+000051f0: 6e64 2822 5461 6761 6c6f 6722 290d 0a20  nd("Tagalog").. 
+00005200: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00005210: 5f6e 616d 6573 2e61 7070 656e 6428 2254  _names.append("T
+00005220: 616a 696b 2229 0d0a 2020 2020 2020 2020  ajik")..        
+00005230: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00005240: 6170 7065 6e64 2822 5461 6d69 6c22 290d  append("Tamil").
+00005250: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00005260: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00005270: 2254 6174 6172 2229 0d0a 2020 2020 2020  "Tatar")..      
+00005280: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00005290: 732e 6170 7065 6e64 2822 5465 6c75 6775  s.append("Telugu
+000052a0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000052b0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+000052c0: 6e64 2822 5468 6169 2229 0d0a 2020 2020  nd("Thai")..    
+000052d0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+000052e0: 6d65 732e 6170 7065 6e64 2822 5469 6265  mes.append("Tibe
+000052f0: 7461 6e22 290d 0a20 2020 2020 2020 2073  tan")..        s
+00005300: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00005310: 7070 656e 6428 2254 7572 6b69 7368 2229  ppend("Turkish")
+00005320: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00005330: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00005340: 2822 5475 726b 6d65 6e22 290d 0a20 2020  ("Turkmen")..   
+00005350: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00005360: 616d 6573 2e61 7070 656e 6428 2255 6b72  ames.append("Ukr
+00005370: 6169 6e69 616e 2229 0d0a 2020 2020 2020  ainian")..      
+00005380: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00005390: 732e 6170 7065 6e64 2822 5572 6475 2229  s.append("Urdu")
+000053a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000053b0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+000053c0: 2822 557a 6265 6b22 290d 0a20 2020 2020  ("Uzbek")..     
+000053d0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+000053e0: 6573 2e61 7070 656e 6428 2256 6965 746e  es.append("Vietn
+000053f0: 616d 6573 6522 290d 0a20 2020 2020 2020  amese")..       
+00005400: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00005410: 2e61 7070 656e 6428 2257 656c 7368 2229  .append("Welsh")
+00005420: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00005430: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00005440: 2822 5969 6464 6973 6822 290d 0a20 2020  ("Yiddish")..   
+00005450: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00005460: 616d 6573 2e61 7070 656e 6428 2259 6f72  ames.append("Yor
+00005470: 7562 6122 290d 0a0d 0a20 2020 2020 2020  uba")....       
+00005480: 2073 656c 662e 636f 6465 5f6f 665f 6e61   self.code_of_na
+00005490: 6d65 203d 2064 6963 7428 7a69 7028 7365  me = dict(zip(se
+000054a0: 6c66 2e6c 6973 745f 6e61 6d65 732c 2073  lf.list_names, s
+000054b0: 656c 662e 6c69 7374 5f63 6f64 6573 2929  elf.list_codes))
+000054c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
+000054d0: 616d 655f 6f66 5f63 6f64 6520 3d20 6469  ame_of_code = di
+000054e0: 6374 287a 6970 2873 656c 662e 6c69 7374  ct(zip(self.list
+000054f0: 5f63 6f64 6573 2c20 7365 6c66 2e6c 6973  _codes, self.lis
+00005500: 745f 6e61 6d65 7329 290d 0a0d 0a20 2020  t_names))....   
+00005510: 2020 2020 2073 656c 662e 6469 6374 203d       self.dict =
+00005520: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00005530: 2020 2020 2020 2020 2020 2020 2761 6627              'af'
+00005540: 3a20 2741 6672 696b 6161 6e73 272c 0d0a  : 'Afrikaans',..
+00005550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005560: 2020 2020 2020 2020 2773 7127 3a20 2741          'sq': 'A
+00005570: 6c62 616e 6961 6e27 2c0d 0a20 2020 2020  lbanian',..     
+00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005590: 2020 2027 616d 273a 2027 416d 6861 7269     'am': 'Amhari
+000055a0: 6327 2c0d 0a20 2020 2020 2020 2020 2020  c',..           
+000055b0: 2020 2020 2020 2020 2020 2020 2027 6172               'ar
+000055c0: 273a 2027 4172 6162 6963 272c 0d0a 2020  ': 'Arabic',..  
+000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055e0: 2020 2020 2020 2768 7927 3a20 2741 726d        'hy': 'Arm
+000055f0: 656e 6961 6e27 2c0d 0a20 2020 2020 2020  enian',..       
+00005600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005610: 2027 6173 273a 2027 4173 7361 6d65 7365   'as': 'Assamese
+00005620: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00005630: 2020 2020 2020 2020 2020 2020 2761 7a27              'az'
+00005640: 3a20 2741 7a65 7262 6169 6a61 6e69 272c  : 'Azerbaijani',
+00005650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005660: 2020 2020 2020 2020 2020 2762 6127 3a20            'ba': 
+00005670: 2742 6173 686b 6972 272c 0d0a 2020 2020  'Bashkir',..    
+00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005690: 2020 2020 2765 7527 3a20 2742 6173 7175      'eu': 'Basqu
+000056a0: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
+000056b0: 2020 2020 2020 2020 2020 2020 2027 6265               'be
+000056c0: 273a 2027 4265 6c61 7275 7369 616e 272c  ': 'Belarusian',
+000056d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000056e0: 2020 2020 2020 2020 2020 2762 6e27 3a20            'bn': 
+000056f0: 2742 656e 6761 6c69 272c 0d0a 2020 2020  'Bengali',..    
+00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005710: 2020 2020 2762 7327 3a20 2742 6f73 6e69      'bs': 'Bosni
+00005720: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
+00005730: 2020 2020 2020 2020 2020 2020 2020 2762                'b
+00005740: 7227 3a20 2742 7265 746f 6e27 2c0d 0a20  r': 'Breton',.. 
+00005750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005760: 2020 2020 2020 2027 6267 273a 2027 4275         'bg': 'Bu
+00005770: 6c67 6172 6961 6e27 2c0d 0a20 2020 2020  lgarian',..     
+00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005790: 2020 2027 6361 273a 2027 4361 7461 6c61     'ca': 'Catala
+000057a0: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+000057b0: 2020 2020 2020 2020 2020 2020 2027 7a68               'zh
+000057c0: 273a 2027 4368 696e 6573 6527 2c0d 0a20  ': 'Chinese',.. 
+000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057e0: 2020 2020 2020 2027 6872 273a 2027 4372         'hr': 'Cr
+000057f0: 6f61 7469 616e 272c 0d0a 2020 2020 2020  oatian',..      
+00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005810: 2020 2763 7327 3a20 2743 7a65 6368 272c    'cs': 'Czech',
+00005820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005830: 2020 2020 2020 2020 2020 2764 6127 3a20            'da': 
+00005840: 2744 616e 6973 6827 2c0d 0a20 2020 2020  'Danish',..     
+00005850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005860: 2020 2027 6e6c 273a 2027 4475 7463 6827     'nl': 'Dutch'
+00005870: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005880: 2020 2020 2020 2020 2020 2027 656e 273a             'en':
+00005890: 2027 456e 676c 6973 6827 2c0d 0a20 2020   'English',..   
+000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058b0: 2020 2020 2027 6574 273a 2027 4573 746f       'et': 'Esto
+000058c0: 6e69 616e 272c 0d0a 2020 2020 2020 2020  nian',..        
+000058d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058e0: 2766 6f27 3a20 2746 6172 6f65 7365 272c  'fo': 'Faroese',
+000058f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005900: 2020 2020 2020 2020 2020 2766 6927 3a20            'fi': 
+00005910: 2746 696e 6e69 7368 272c 0d0a 2020 2020  'Finnish',..    
+00005920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005930: 2020 2020 2766 7227 3a20 2746 7265 6e63      'fr': 'Frenc
+00005940: 6827 2c0d 0a20 2020 2020 2020 2020 2020  h',..           
+00005950: 2020 2020 2020 2020 2020 2020 2027 676c               'gl
+00005960: 273a 2027 4761 6c69 6369 616e 272c 0d0a  ': 'Galician',..
 00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005980: 2764 6127 3a20 2744 616e 6973 6827 2c0d  'da': 'Danish',.
-00005990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000059a0: 2020 2020 2020 2020 2027 6e6c 273a 2027           'nl': '
-000059b0: 4475 7463 6827 2c0d 0a20 2020 2020 2020  Dutch',..       
-000059c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059d0: 2027 656e 273a 2027 456e 676c 6973 6827   'en': 'English'
-000059e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000059f0: 2020 2020 2020 2020 2020 2027 6574 273a             'et':
-00005a00: 2027 4573 746f 6e69 616e 272c 0d0a 2020   'Estonian',..  
-00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a20: 2020 2020 2020 2766 6f27 3a20 2746 6172        'fo': 'Far
-00005a30: 6f65 7365 272c 0d0a 2020 2020 2020 2020  oese',..        
-00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a50: 2766 6927 3a20 2746 696e 6e69 7368 272c  'fi': 'Finnish',
-00005a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005a70: 2020 2020 2020 2020 2020 2766 7227 3a20            'fr': 
-00005a80: 2746 7265 6e63 6827 2c0d 0a20 2020 2020  'French',..     
-00005a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005aa0: 2020 2027 676c 273a 2027 4761 6c69 6369     'gl': 'Galici
-00005ab0: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
-00005ac0: 2020 2020 2020 2020 2020 2020 2020 276b                'k
-00005ad0: 6127 3a20 2747 656f 7267 6961 6e27 2c0d  a': 'Georgian',.
-00005ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005af0: 2020 2020 2020 2020 2027 6465 273a 2027           'de': '
-00005b00: 4765 726d 616e 272c 0d0a 2020 2020 2020  German',..      
-00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b20: 2020 2765 6c27 3a20 2747 7265 656b 272c    'el': 'Greek',
-00005b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005b40: 2020 2020 2020 2020 2020 2767 7527 3a20            'gu': 
-00005b50: 2747 756a 6172 6174 6927 2c0d 0a20 2020  'Gujarati',..   
-00005b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b70: 2020 2020 2027 6874 273a 2027 4861 6974       'ht': 'Hait
-00005b80: 6961 6e20 4372 656f 6c65 272c 0d0a 2020  ian Creole',..  
-00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ba0: 2020 2020 2020 2768 6127 3a20 2748 6175        'ha': 'Hau
-00005bb0: 7361 272c 0d0a 2020 2020 2020 2020 2020  sa',..          
-00005bc0: 2020 2020 2020 2020 2020 2020 2020 2768                'h
-00005bd0: 6177 273a 2027 4861 7761 6969 616e 272c  aw': 'Hawaiian',
-00005be0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005bf0: 2020 2020 2020 2020 2020 2768 6527 3a20            'he': 
-00005c00: 2748 6562 7265 7727 2c0d 0a20 2020 2020  'Hebrew',..     
-00005c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c20: 2020 2027 6869 273a 2027 4869 6e64 6927     'hi': 'Hindi'
-00005c30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005c40: 2020 2020 2020 2020 2020 2027 6875 273a             'hu':
-00005c50: 2027 4875 6e67 6172 6961 6e27 2c0d 0a20   'Hungarian',.. 
-00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c70: 2020 2020 2020 2027 6973 273a 2027 4963         'is': 'Ic
-00005c80: 656c 616e 6469 6327 2c0d 0a20 2020 2020  elandic',..     
-00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ca0: 2020 2027 6964 273a 2027 496e 646f 6e65     'id': 'Indone
-00005cb0: 7369 616e 272c 0d0a 2020 2020 2020 2020  sian',..        
+00005980: 2020 2020 2020 2020 276b 6127 3a20 2747          'ka': 'G
+00005990: 656f 7267 6961 6e27 2c0d 0a20 2020 2020  eorgian',..     
+000059a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059b0: 2020 2027 6465 273a 2027 4765 726d 616e     'de': 'German
+000059c0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+000059d0: 2020 2020 2020 2020 2020 2020 2765 6c27              'el'
+000059e0: 3a20 2747 7265 656b 272c 0d0a 2020 2020  : 'Greek',..    
+000059f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a00: 2020 2020 2767 7527 3a20 2747 756a 6172      'gu': 'Gujar
+00005a10: 6174 6927 2c0d 0a20 2020 2020 2020 2020  ati',..         
+00005a20: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00005a30: 6874 273a 2027 4861 6974 6961 6e20 4372  ht': 'Haitian Cr
+00005a40: 656f 6c65 272c 0d0a 2020 2020 2020 2020  eole',..        
+00005a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a60: 2768 6127 3a20 2748 6175 7361 272c 0d0a  'ha': 'Hausa',..
+00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a80: 2020 2020 2020 2020 2768 6177 273a 2027          'haw': '
+00005a90: 4861 7761 6969 616e 272c 0d0a 2020 2020  Hawaiian',..    
+00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ab0: 2020 2020 2768 6527 3a20 2748 6562 7265      'he': 'Hebre
+00005ac0: 7727 2c0d 0a20 2020 2020 2020 2020 2020  w',..           
+00005ad0: 2020 2020 2020 2020 2020 2020 2027 6869               'hi
+00005ae0: 273a 2027 4869 6e64 6927 2c0d 0a20 2020  ': 'Hindi',..   
+00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b00: 2020 2020 2027 6875 273a 2027 4875 6e67       'hu': 'Hung
+00005b10: 6172 6961 6e27 2c0d 0a20 2020 2020 2020  arian',..       
+00005b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b30: 2027 6973 273a 2027 4963 656c 616e 6469   'is': 'Icelandi
+00005b40: 6327 2c0d 0a20 2020 2020 2020 2020 2020  c',..           
+00005b50: 2020 2020 2020 2020 2020 2020 2027 6964               'id
+00005b60: 273a 2027 496e 646f 6e65 7369 616e 272c  ': 'Indonesian',
+00005b70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005b80: 2020 2020 2020 2020 2020 2769 7427 3a20            'it': 
+00005b90: 2749 7461 6c69 616e 272c 0d0a 2020 2020  'Italian',..    
+00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bb0: 2020 2020 276a 6127 3a20 274a 6170 616e      'ja': 'Japan
+00005bc0: 6573 6527 2c0d 0a20 2020 2020 2020 2020  ese',..         
+00005bd0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00005be0: 6a76 273a 2027 4a61 7661 6e65 7365 272c  jv': 'Javanese',
+00005bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005c00: 2020 2020 2020 2020 2020 276b 6e27 3a20            'kn': 
+00005c10: 274b 616e 6e61 6461 272c 0d0a 2020 2020  'Kannada',..    
+00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c30: 2020 2020 276b 6b27 3a20 274b 617a 616b      'kk': 'Kazak
+00005c40: 6827 2c0d 0a20 2020 2020 2020 2020 2020  h',..           
+00005c50: 2020 2020 2020 2020 2020 2020 2027 6b6d               'km
+00005c60: 273a 2027 4b68 6d65 7227 2c0d 0a20 2020  ': 'Khmer',..   
+00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c80: 2020 2020 2027 6b6f 273a 2027 4b6f 7265       'ko': 'Kore
+00005c90: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
+00005ca0: 2020 2020 2020 2020 2020 2020 2020 276c                'l
+00005cb0: 6f27 3a20 274c 616f 272c 0d0a 2020 2020  o': 'Lao',..    
 00005cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cd0: 2769 7427 3a20 2749 7461 6c69 616e 272c  'it': 'Italian',
-00005ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005cf0: 2020 2020 2020 2020 2020 276a 6127 3a20            'ja': 
-00005d00: 274a 6170 616e 6573 6527 2c0d 0a20 2020  'Japanese',..   
+00005cd0: 2020 2020 276c 6127 3a20 274c 6174 696e      'la': 'Latin
+00005ce0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00005cf0: 2020 2020 2020 2020 2020 2020 276c 7627              'lv'
+00005d00: 3a20 274c 6174 7669 616e 272c 0d0a 2020  : 'Latvian',..  
 00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d20: 2020 2020 2027 6a76 273a 2027 4a61 7661       'jv': 'Java
-00005d30: 6e65 7365 272c 0d0a 2020 2020 2020 2020  nese',..        
+00005d20: 2020 2020 2020 276c 6e27 3a20 274c 696e        'ln': 'Lin
+00005d30: 6761 6c61 272c 0d0a 2020 2020 2020 2020  gala',..        
 00005d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d50: 276b 6e27 3a20 274b 616e 6e61 6461 272c  'kn': 'Kannada',
-00005d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005d70: 2020 2020 2020 2020 2020 276b 6b27 3a20            'kk': 
-00005d80: 274b 617a 616b 6827 2c0d 0a20 2020 2020  'Kazakh',..     
-00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005da0: 2020 2027 6b6d 273a 2027 4b68 6d65 7227     'km': 'Khmer'
-00005db0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005dc0: 2020 2020 2020 2020 2020 2027 6b6f 273a             'ko':
-00005dd0: 2027 4b6f 7265 616e 272c 0d0a 2020 2020   'Korean',..    
-00005de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005df0: 2020 2020 276c 6f27 3a20 274c 616f 272c      'lo': 'Lao',
-00005e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005e10: 2020 2020 2020 2020 2020 276c 6127 3a20            'la': 
-00005e20: 274c 6174 696e 272c 0d0a 2020 2020 2020  'Latin',..      
-00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e40: 2020 276c 7627 3a20 274c 6174 7669 616e    'lv': 'Latvian
-00005e50: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005e60: 2020 2020 2020 2020 2020 2020 276c 6e27              'ln'
-00005e70: 3a20 274c 696e 6761 6c61 272c 0d0a 2020  : 'Lingala',..  
-00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e90: 2020 2020 2020 276c 7427 3a20 274c 6974        'lt': 'Lit
-00005ea0: 6875 616e 6961 6e27 2c0d 0a20 2020 2020  huanian',..     
-00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ec0: 2020 2027 6c62 273a 2027 4c75 7865 6d62     'lb': 'Luxemb
-00005ed0: 6f75 7267 6973 6827 2c0d 0a20 2020 2020  ourgish',..     
-00005ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ef0: 2020 2027 6d6b 273a 2027 4d61 6365 646f     'mk': 'Macedo
-00005f00: 6e69 616e 272c 0d0a 2020 2020 2020 2020  nian',..        
-00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f20: 276d 6727 3a20 274d 616c 6167 6173 7927  'mg': 'Malagasy'
-00005f30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005f40: 2020 2020 2020 2020 2020 2027 6d73 273a             'ms':
-00005f50: 2027 4d61 6c61 7927 2c0d 0a20 2020 2020   'Malay',..     
-00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f70: 2020 2027 6d6c 273a 2027 4d61 6c61 7961     'ml': 'Malaya
-00005f80: 6c61 6d27 2c0d 0a20 2020 2020 2020 2020  lam',..         
-00005f90: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00005fa0: 6d74 273a 2027 4d61 6c74 6573 6527 2c0d  mt': 'Maltese',.
-00005fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005fc0: 2020 2020 2020 2020 2027 6d69 273a 2027           'mi': '
-00005fd0: 4d61 6f72 6927 2c0d 0a20 2020 2020 2020  Maori',..       
-00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ff0: 2027 6d72 273a 2027 4d61 7261 7468 6927   'mr': 'Marathi'
-00006000: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00006010: 2020 2020 2020 2020 2020 2027 6d6e 273a             'mn':
-00006020: 2027 4d6f 6e67 6f6c 6961 6e27 2c0d 0a20   'Mongolian',.. 
-00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006040: 2020 2020 2020 2027 6d79 273a 2027 4d79         'my': 'My
-00006050: 616e 6d61 7220 2842 7572 6d65 7365 2927  anmar (Burmese)'
-00006060: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00006070: 2020 2020 2020 2020 2020 2027 6e65 273a             'ne':
-00006080: 2027 4e65 7061 6c69 272c 0d0a 2020 2020   'Nepali',..    
-00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060a0: 2020 2020 276e 6f27 3a20 274e 6f72 7765      'no': 'Norwe
-000060b0: 6769 616e 272c 0d0a 2020 2020 2020 2020  gian',..        
-000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060d0: 276e 6e27 3a20 274e 796e 6f72 736b 272c  'nn': 'Nynorsk',
-000060e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000060f0: 2020 2020 2020 2020 2020 276f 6327 3a20            'oc': 
-00006100: 274f 6363 6974 616e 272c 0d0a 2020 2020  'Occitan',..    
-00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006120: 2020 2020 2770 7327 3a20 2750 6173 6874      'ps': 'Pasht
-00006130: 6f27 2c0d 0a20 2020 2020 2020 2020 2020  o',..           
-00006140: 2020 2020 2020 2020 2020 2020 2027 6661               'fa
-00006150: 273a 2027 5065 7273 6961 6e27 2c0d 0a20  ': 'Persian',.. 
-00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006170: 2020 2020 2020 2027 706c 273a 2027 506f         'pl': 'Po
-00006180: 6c69 7368 272c 0d0a 2020 2020 2020 2020  lish',..        
-00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061a0: 2770 7427 3a20 2750 6f72 7475 6775 6573  'pt': 'Portugues
-000061b0: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
-000061c0: 2020 2020 2020 2020 2020 2020 2027 7061               'pa
-000061d0: 273a 2027 5075 6e6a 6162 6927 2c0d 0a20  ': 'Punjabi',.. 
-000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061f0: 2020 2020 2020 2027 726f 273a 2027 526f         'ro': 'Ro
-00006200: 6d61 6e69 616e 272c 0d0a 2020 2020 2020  manian',..      
-00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006220: 2020 2772 7527 3a20 2752 7573 7369 616e    'ru': 'Russian
-00006230: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00006240: 2020 2020 2020 2020 2020 2020 2773 6127              'sa'
-00006250: 3a20 2753 616e 736b 7269 7427 2c0d 0a20  : 'Sanskrit',.. 
-00006260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006270: 2020 2020 2020 2027 7372 273a 2027 5365         'sr': 'Se
-00006280: 7262 6961 6e27 2c0d 0a20 2020 2020 2020  rbian',..       
-00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062a0: 2027 736e 273a 2027 5368 6f6e 6127 2c0d   'sn': 'Shona',.
-000062b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000062c0: 2020 2020 2020 2020 2027 7364 273a 2027           'sd': '
-000062d0: 5369 6e64 6869 272c 0d0a 2020 2020 2020  Sindhi',..      
-000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062f0: 2020 2773 6927 3a20 2753 696e 6861 6c61    'si': 'Sinhala
-00006300: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00006310: 2020 2020 2020 2020 2020 2020 2773 6b27              'sk'
-00006320: 3a20 2753 6c6f 7661 6b27 2c0d 0a20 2020  : 'Slovak',..   
-00006330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006340: 2020 2020 2027 736c 273a 2027 536c 6f76       'sl': 'Slov
-00006350: 656e 6961 6e27 2c0d 0a20 2020 2020 2020  enian',..       
+00005d50: 276c 7427 3a20 274c 6974 6875 616e 6961  'lt': 'Lithuania
+00005d60: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+00005d70: 2020 2020 2020 2020 2020 2020 2027 6c62               'lb
+00005d80: 273a 2027 4c75 7865 6d62 6f75 7267 6973  ': 'Luxembourgis
+00005d90: 6827 2c0d 0a20 2020 2020 2020 2020 2020  h',..           
+00005da0: 2020 2020 2020 2020 2020 2020 2027 6d6b               'mk
+00005db0: 273a 2027 4d61 6365 646f 6e69 616e 272c  ': 'Macedonian',
+00005dc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005dd0: 2020 2020 2020 2020 2020 276d 6727 3a20            'mg': 
+00005de0: 274d 616c 6167 6173 7927 2c0d 0a20 2020  'Malagasy',..   
+00005df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e00: 2020 2020 2027 6d73 273a 2027 4d61 6c61       'ms': 'Mala
+00005e10: 7927 2c0d 0a20 2020 2020 2020 2020 2020  y',..           
+00005e20: 2020 2020 2020 2020 2020 2020 2027 6d6c               'ml
+00005e30: 273a 2027 4d61 6c61 7961 6c61 6d27 2c0d  ': 'Malayalam',.
+00005e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005e50: 2020 2020 2020 2020 2027 6d74 273a 2027           'mt': '
+00005e60: 4d61 6c74 6573 6527 2c0d 0a20 2020 2020  Maltese',..     
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e80: 2020 2027 6d69 273a 2027 4d61 6f72 6927     'mi': 'Maori'
+00005e90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00005ea0: 2020 2020 2020 2020 2020 2027 6d72 273a             'mr':
+00005eb0: 2027 4d61 7261 7468 6927 2c0d 0a20 2020   'Marathi',..   
+00005ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ed0: 2020 2020 2027 6d6e 273a 2027 4d6f 6e67       'mn': 'Mong
+00005ee0: 6f6c 6961 6e27 2c0d 0a20 2020 2020 2020  olian',..       
+00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f00: 2027 6d79 273a 2027 4d79 616e 6d61 7220   'my': 'Myanmar 
+00005f10: 2842 7572 6d65 7365 2927 2c0d 0a20 2020  (Burmese)',..   
+00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f30: 2020 2020 2027 6e65 273a 2027 4e65 7061       'ne': 'Nepa
+00005f40: 6c69 272c 0d0a 2020 2020 2020 2020 2020  li',..          
+00005f50: 2020 2020 2020 2020 2020 2020 2020 276e                'n
+00005f60: 6f27 3a20 274e 6f72 7765 6769 616e 272c  o': 'Norwegian',
+00005f70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005f80: 2020 2020 2020 2020 2020 276e 6e27 3a20            'nn': 
+00005f90: 274e 796e 6f72 736b 272c 0d0a 2020 2020  'Nynorsk',..    
+00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fb0: 2020 2020 276f 6327 3a20 274f 6363 6974      'oc': 'Occit
+00005fc0: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
+00005fd0: 2020 2020 2020 2020 2020 2020 2020 2770                'p
+00005fe0: 7327 3a20 2750 6173 6874 6f27 2c0d 0a20  s': 'Pashto',.. 
+00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006000: 2020 2020 2020 2027 6661 273a 2027 5065         'fa': 'Pe
+00006010: 7273 6961 6e27 2c0d 0a20 2020 2020 2020  rsian',..       
+00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006030: 2027 706c 273a 2027 506f 6c69 7368 272c   'pl': 'Polish',
+00006040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006050: 2020 2020 2020 2020 2020 2770 7427 3a20            'pt': 
+00006060: 2750 6f72 7475 6775 6573 6527 2c0d 0a20  'Portuguese',.. 
+00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006080: 2020 2020 2020 2027 7061 273a 2027 5075         'pa': 'Pu
+00006090: 6e6a 6162 6927 2c0d 0a20 2020 2020 2020  njabi',..       
+000060a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060b0: 2027 726f 273a 2027 526f 6d61 6e69 616e   'ro': 'Romanian
+000060c0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+000060d0: 2020 2020 2020 2020 2020 2020 2772 7527              'ru'
+000060e0: 3a20 2752 7573 7369 616e 272c 0d0a 2020  : 'Russian',..  
+000060f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006100: 2020 2020 2020 2773 6127 3a20 2753 616e        'sa': 'San
+00006110: 736b 7269 7427 2c0d 0a20 2020 2020 2020  skrit',..       
+00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006130: 2027 7372 273a 2027 5365 7262 6961 6e27   'sr': 'Serbian'
+00006140: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00006150: 2020 2020 2020 2020 2020 2027 736e 273a             'sn':
+00006160: 2027 5368 6f6e 6127 2c0d 0a20 2020 2020   'Shona',..     
+00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006180: 2020 2027 7364 273a 2027 5369 6e64 6869     'sd': 'Sindhi
+00006190: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+000061a0: 2020 2020 2020 2020 2020 2020 2773 6927              'si'
+000061b0: 3a20 2753 696e 6861 6c61 272c 0d0a 2020  : 'Sinhala',..  
+000061c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061d0: 2020 2020 2020 2773 6b27 3a20 2753 6c6f        'sk': 'Slo
+000061e0: 7661 6b27 2c0d 0a20 2020 2020 2020 2020  vak',..         
+000061f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00006200: 736c 273a 2027 536c 6f76 656e 6961 6e27  sl': 'Slovenian'
+00006210: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00006220: 2020 2020 2020 2020 2020 2027 736f 273a             'so':
+00006230: 2027 536f 6d61 6c69 272c 0d0a 2020 2020   'Somali',..    
+00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006250: 2020 2020 2765 7327 3a20 2753 7061 6e69      'es': 'Spani
+00006260: 7368 272c 0d0a 2020 2020 2020 2020 2020  sh',..          
+00006270: 2020 2020 2020 2020 2020 2020 2020 2773                's
+00006280: 7527 3a20 2753 756e 6461 6e65 7365 272c  u': 'Sundanese',
+00006290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000062a0: 2020 2020 2020 2020 2020 2773 7727 3a20            'sw': 
+000062b0: 2753 7761 6869 6c69 272c 0d0a 2020 2020  'Swahili',..    
+000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062d0: 2020 2020 2773 7627 3a20 2753 7765 6469      'sv': 'Swedi
+000062e0: 7368 272c 0d0a 2020 2020 2020 2020 2020  sh',..          
+000062f0: 2020 2020 2020 2020 2020 2020 2020 2774                't
+00006300: 6c27 3a20 2754 6167 616c 6f67 272c 0d0a  l': 'Tagalog',..
+00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006320: 2020 2020 2020 2020 2774 6727 3a20 2754          'tg': 'T
+00006330: 616a 696b 272c 0d0a 2020 2020 2020 2020  ajik',..        
+00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006350: 2774 6127 3a20 2754 616d 696c 272c 0d0a  'ta': 'Tamil',..
 00006360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006370: 2027 736f 273a 2027 536f 6d61 6c69 272c   'so': 'Somali',
-00006380: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006390: 2020 2020 2020 2020 2020 2765 7327 3a20            'es': 
-000063a0: 2753 7061 6e69 7368 272c 0d0a 2020 2020  'Spanish',..    
-000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063c0: 2020 2020 2773 7527 3a20 2753 756e 6461      'su': 'Sunda
-000063d0: 6e65 7365 272c 0d0a 2020 2020 2020 2020  nese',..        
+00006370: 2020 2020 2020 2020 2774 7427 3a20 2754          'tt': 'T
+00006380: 6174 6172 272c 0d0a 2020 2020 2020 2020  atar',..        
+00006390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063a0: 2774 6527 3a20 2754 656c 7567 7527 2c0d  'te': 'Telugu',.
+000063b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000063c0: 2020 2020 2020 2020 2027 7468 273a 2027           'th': '
+000063d0: 5468 6169 272c 0d0a 2020 2020 2020 2020  Thai',..        
 000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063f0: 2773 7727 3a20 2753 7761 6869 6c69 272c  'sw': 'Swahili',
+000063f0: 2762 6f27 3a20 2754 6962 6574 616e 272c  'bo': 'Tibetan',
 00006400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006410: 2020 2020 2020 2020 2020 2773 7627 3a20            'sv': 
-00006420: 2753 7765 6469 7368 272c 0d0a 2020 2020  'Swedish',..    
+00006410: 2020 2020 2020 2020 2020 2774 7227 3a20            'tr': 
+00006420: 2754 7572 6b69 7368 272c 0d0a 2020 2020  'Turkish',..    
 00006430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006440: 2020 2020 2774 6c27 3a20 2754 6167 616c      'tl': 'Tagal
-00006450: 6f67 272c 0d0a 2020 2020 2020 2020 2020  og',..          
-00006460: 2020 2020 2020 2020 2020 2020 2020 2774                't
-00006470: 6727 3a20 2754 616a 696b 272c 0d0a 2020  g': 'Tajik',..  
-00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006490: 2020 2020 2020 2774 6127 3a20 2754 616d        'ta': 'Tam
-000064a0: 696c 272c 0d0a 2020 2020 2020 2020 2020  il',..          
-000064b0: 2020 2020 2020 2020 2020 2020 2020 2774                't
-000064c0: 7427 3a20 2754 6174 6172 272c 0d0a 2020  t': 'Tatar',..  
-000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064e0: 2020 2020 2020 2774 6527 3a20 2754 656c        'te': 'Tel
-000064f0: 7567 7527 2c0d 0a20 2020 2020 2020 2020  ugu',..         
-00006500: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00006510: 7468 273a 2027 5468 6169 272c 0d0a 2020  th': 'Thai',..  
-00006520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006530: 2020 2020 2020 2762 6f27 3a20 2754 6962        'bo': 'Tib
-00006540: 6574 616e 272c 0d0a 2020 2020 2020 2020  etan',..        
+00006440: 2020 2020 2774 6b27 3a20 2754 7572 6b6d      'tk': 'Turkm
+00006450: 656e 272c 0d0a 2020 2020 2020 2020 2020  en',..          
+00006460: 2020 2020 2020 2020 2020 2020 2020 2775                'u
+00006470: 6b27 3a20 2755 6b72 6169 6e69 616e 272c  k': 'Ukrainian',
+00006480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006490: 2020 2020 2020 2020 2020 2775 7227 3a20            'ur': 
+000064a0: 2755 7264 7527 2c0d 0a20 2020 2020 2020  'Urdu',..       
+000064b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064c0: 2027 757a 273a 2027 557a 6265 6b27 2c0d   'uz': 'Uzbek',.
+000064d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000064e0: 2020 2020 2020 2020 2027 7669 273a 2027           'vi': '
+000064f0: 5669 6574 6e61 6d65 7365 272c 0d0a 2020  Vietnamese',..  
+00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006510: 2020 2020 2020 2763 7927 3a20 2757 656c        'cy': 'Wel
+00006520: 7368 272c 0d0a 2020 2020 2020 2020 2020  sh',..          
+00006530: 2020 2020 2020 2020 2020 2020 2020 2779                'y
+00006540: 6927 3a20 2759 6964 6469 7368 272c 0d0a  i': 'Yiddish',..
 00006550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006560: 2774 7227 3a20 2754 7572 6b69 7368 272c  'tr': 'Turkish',
-00006570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006580: 2020 2020 2020 2020 2020 2774 6b27 3a20            'tk': 
-00006590: 2754 7572 6b6d 656e 272c 0d0a 2020 2020  'Turkmen',..    
-000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065b0: 2020 2020 2775 6b27 3a20 2755 6b72 6169      'uk': 'Ukrai
-000065c0: 6e69 616e 272c 0d0a 2020 2020 2020 2020  nian',..        
-000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065e0: 2775 7227 3a20 2755 7264 7527 2c0d 0a20  'ur': 'Urdu',.. 
-000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006600: 2020 2020 2020 2027 757a 273a 2027 557a         'uz': 'Uz
-00006610: 6265 6b27 2c0d 0a20 2020 2020 2020 2020  bek',..         
-00006620: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00006630: 7669 273a 2027 5669 6574 6e61 6d65 7365  vi': 'Vietnamese
-00006640: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00006650: 2020 2020 2020 2020 2020 2020 2763 7927              'cy'
-00006660: 3a20 2757 656c 7368 272c 0d0a 2020 2020  : 'Welsh',..    
-00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006680: 2020 2020 2779 6927 3a20 2759 6964 6469      'yi': 'Yiddi
-00006690: 7368 272c 0d0a 2020 2020 2020 2020 2020  sh',..          
-000066a0: 2020 2020 2020 2020 2020 2020 2020 2779                'y
-000066b0: 6f27 3a20 2759 6f72 7562 6127 2c0d 0a20  o': 'Yoruba',.. 
-000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066d0: 2020 207d 0d0a 0d0a 2020 2020 6465 6620     }....    def 
-000066e0: 6765 745f 6e61 6d65 2873 656c 662c 2067  get_name(self, g
-000066f0: 6574 5f63 6f64 6529 3a0d 0a20 2020 2020  et_code):..     
-00006700: 2020 2072 6574 7572 6e20 7365 6c66 2e64     return self.d
-00006710: 6963 742e 6765 7428 6765 745f 636f 6465  ict.get(get_code
-00006720: 2e6c 6f77 6572 2829 2c20 2222 290d 0a0d  .lower(), "")...
-00006730: 0a20 2020 2064 6566 2067 6574 5f63 6f64  .    def get_cod
-00006740: 6528 7365 6c66 2c20 6c61 6e67 7561 6765  e(self, language
-00006750: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
-00006760: 6765 745f 636f 6465 2c20 6c61 6e67 2069  get_code, lang i
-00006770: 6e20 7365 6c66 2e64 6963 742e 6974 656d  n self.dict.item
-00006780: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-00006790: 2020 6966 206c 616e 672e 6c6f 7765 7228    if lang.lower(
-000067a0: 2920 3d3d 206c 616e 6775 6167 652e 6c6f  ) == language.lo
-000067b0: 7765 7228 293a 0d0a 2020 2020 2020 2020  wer():..        
-000067c0: 2020 2020 2020 2020 7265 7475 726e 2067          return g
-000067d0: 6574 5f63 6f64 650d 0a20 2020 2020 2020  et_code..       
-000067e0: 2072 6574 7572 6e20 2222 0d0a 0d0a 0d0a   return ""......
-000067f0: 636c 6173 7320 476f 6f67 6c65 4c61 6e67  class GoogleLang
-00006800: 7561 6765 3a0d 0a20 2020 2064 6566 205f  uage:..    def _
-00006810: 5f69 6e69 745f 5f28 7365 6c66 293a 0d0a  _init__(self):..
-00006820: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00006830: 745f 636f 6465 7320 3d20 5b5d 0d0a 2020  t_codes = []..  
-00006840: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00006850: 636f 6465 732e 6170 7065 6e64 2822 6166  codes.append("af
-00006860: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00006870: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00006880: 6e64 2822 7371 2229 0d0a 2020 2020 2020  nd("sq")..      
-00006890: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-000068a0: 732e 6170 7065 6e64 2822 616d 2229 0d0a  s.append("am")..
-000068b0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000068c0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-000068d0: 6172 2229 0d0a 2020 2020 2020 2020 7365  ar")..        se
-000068e0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-000068f0: 7065 6e64 2822 6879 2229 0d0a 2020 2020  pend("hy")..    
-00006900: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00006910: 6465 732e 6170 7065 6e64 2822 6173 2229  des.append("as")
-00006920: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00006930: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00006940: 2822 6179 2229 0d0a 2020 2020 2020 2020  ("ay")..        
-00006950: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00006960: 6170 7065 6e64 2822 617a 2229 0d0a 2020  append("az")..  
-00006970: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00006980: 636f 6465 732e 6170 7065 6e64 2822 626d  codes.append("bm
-00006990: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000069a0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-000069b0: 6e64 2822 6575 2229 0d0a 2020 2020 2020  nd("eu")..      
-000069c0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-000069d0: 732e 6170 7065 6e64 2822 6265 2229 0d0a  s.append("be")..
-000069e0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000069f0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00006a00: 626e 2229 0d0a 2020 2020 2020 2020 7365  bn")..        se
-00006a10: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00006a20: 7065 6e64 2822 6268 6f22 290d 0a20 2020  pend("bho")..   
-00006a30: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00006a40: 6f64 6573 2e61 7070 656e 6428 2262 7322  odes.append("bs"
-00006a50: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00006a60: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00006a70: 6428 2262 6722 290d 0a20 2020 2020 2020  d("bg")..       
-00006a80: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00006a90: 2e61 7070 656e 6428 2263 6122 290d 0a20  .append("ca").. 
-00006aa0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00006ab0: 5f63 6f64 6573 2e61 7070 656e 6428 2263  _codes.append("c
-00006ac0: 6562 2229 0d0a 2020 2020 2020 2020 7365  eb")..        se
-00006ad0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00006ae0: 7065 6e64 2822 6e79 2229 0d0a 2020 2020  pend("ny")..    
-00006af0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00006b00: 6465 732e 6170 7065 6e64 2822 7a68 2d43  des.append("zh-C
-00006b10: 4e22 290d 0a20 2020 2020 2020 2073 656c  N")..        sel
-00006b20: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00006b30: 656e 6428 227a 682d 5457 2229 0d0a 2020  end("zh-TW")..  
-00006b40: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00006b50: 636f 6465 732e 6170 7065 6e64 2822 636f  codes.append("co
-00006b60: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00006b70: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00006b80: 6e64 2822 6872 2229 0d0a 2020 2020 2020  nd("hr")..      
-00006b90: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00006ba0: 732e 6170 7065 6e64 2822 6373 2229 0d0a  s.append("cs")..
-00006bb0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00006bc0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00006bd0: 6461 2229 0d0a 2020 2020 2020 2020 7365  da")..        se
-00006be0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00006bf0: 7065 6e64 2822 6476 2229 0d0a 2020 2020  pend("dv")..    
-00006c00: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00006c10: 6465 732e 6170 7065 6e64 2822 646f 6922  des.append("doi"
-00006c20: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00006c30: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00006c40: 6428 226e 6c22 290d 0a20 2020 2020 2020  d("nl")..       
-00006c50: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00006c60: 2e61 7070 656e 6428 2265 6e22 290d 0a20  .append("en").. 
-00006c70: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00006c80: 5f63 6f64 6573 2e61 7070 656e 6428 2265  _codes.append("e
-00006c90: 6f22 290d 0a20 2020 2020 2020 2073 656c  o")..        sel
-00006ca0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00006cb0: 656e 6428 2265 7422 290d 0a20 2020 2020  end("et")..     
-00006cc0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00006cd0: 6573 2e61 7070 656e 6428 2265 6522 290d  es.append("ee").
-00006ce0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00006cf0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00006d00: 2266 696c 2229 0d0a 2020 2020 2020 2020  "fil")..        
-00006d10: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00006d20: 6170 7065 6e64 2822 6669 2229 0d0a 2020  append("fi")..  
-00006d30: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00006d40: 636f 6465 732e 6170 7065 6e64 2822 6672  codes.append("fr
-00006d50: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00006d60: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00006d70: 6e64 2822 6679 2229 0d0a 2020 2020 2020  nd("fy")..      
-00006d80: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00006d90: 732e 6170 7065 6e64 2822 676c 2229 0d0a  s.append("gl")..
-00006da0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00006db0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00006dc0: 6b61 2229 0d0a 2020 2020 2020 2020 7365  ka")..        se
-00006dd0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00006de0: 7065 6e64 2822 6465 2229 0d0a 2020 2020  pend("de")..    
-00006df0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-00006e00: 6465 732e 6170 7065 6e64 2822 656c 2229  des.append("el")
-00006e10: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00006e20: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00006e30: 2822 676e 2229 0d0a 2020 2020 2020 2020  ("gn")..        
-00006e40: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00006e50: 6170 7065 6e64 2822 6775 2229 0d0a 2020  append("gu")..  
-00006e60: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00006e70: 636f 6465 732e 6170 7065 6e64 2822 6874  codes.append("ht
-00006e80: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00006e90: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00006ea0: 6e64 2822 6861 2229 0d0a 2020 2020 2020  nd("ha")..      
-00006eb0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00006ec0: 732e 6170 7065 6e64 2822 6861 7722 290d  s.append("haw").
-00006ed0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00006ee0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00006ef0: 2268 6522 290d 0a20 2020 2020 2020 2073  "he")..        s
-00006f00: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00006f10: 7070 656e 6428 2268 6922 290d 0a20 2020  ppend("hi")..   
-00006f20: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00006f30: 6f64 6573 2e61 7070 656e 6428 2268 6d6e  odes.append("hmn
-00006f40: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00006f50: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00006f60: 6e64 2822 6875 2229 0d0a 2020 2020 2020  nd("hu")..      
-00006f70: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00006f80: 732e 6170 7065 6e64 2822 6973 2229 0d0a  s.append("is")..
-00006f90: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00006fa0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00006fb0: 6967 2229 0d0a 2020 2020 2020 2020 7365  ig")..        se
-00006fc0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00006fd0: 7065 6e64 2822 696c 6f22 290d 0a20 2020  pend("ilo")..   
-00006fe0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00006ff0: 6f64 6573 2e61 7070 656e 6428 2269 6422  odes.append("id"
-00007000: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007010: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00007020: 6428 2267 6122 290d 0a20 2020 2020 2020  d("ga")..       
-00007030: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00007040: 2e61 7070 656e 6428 2269 7422 290d 0a20  .append("it").. 
-00007050: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007060: 5f63 6f64 6573 2e61 7070 656e 6428 226a  _codes.append("j
-00007070: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
-00007080: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00007090: 656e 6428 226a 7622 290d 0a20 2020 2020  end("jv")..     
-000070a0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-000070b0: 6573 2e61 7070 656e 6428 226b 6e22 290d  es.append("kn").
-000070c0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000070d0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-000070e0: 226b 6b22 290d 0a20 2020 2020 2020 2073  "kk")..        s
-000070f0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00007100: 7070 656e 6428 226b 6d22 290d 0a20 2020  ppend("km")..   
-00007110: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00007120: 6f64 6573 2e61 7070 656e 6428 2272 7722  odes.append("rw"
-00007130: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007140: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00007150: 6428 2267 6f6d 2229 0d0a 2020 2020 2020  d("gom")..      
-00007160: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00007170: 732e 6170 7065 6e64 2822 6b6f 2229 0d0a  s.append("ko")..
-00007180: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007190: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-000071a0: 6b72 6922 290d 0a20 2020 2020 2020 2073  kri")..        s
-000071b0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-000071c0: 7070 656e 6428 226b 6d72 2229 0d0a 2020  ppend("kmr")..  
-000071d0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000071e0: 636f 6465 732e 6170 7065 6e64 2822 636b  codes.append("ck
-000071f0: 6222 290d 0a20 2020 2020 2020 2073 656c  b")..        sel
-00007200: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00007210: 656e 6428 226b 7922 290d 0a20 2020 2020  end("ky")..     
-00007220: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00007230: 6573 2e61 7070 656e 6428 226c 6f22 290d  es.append("lo").
-00007240: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00007250: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00007260: 226c 6122 290d 0a20 2020 2020 2020 2073  "la")..        s
-00007270: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00007280: 7070 656e 6428 226c 7622 290d 0a20 2020  ppend("lv")..   
-00007290: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-000072a0: 6f64 6573 2e61 7070 656e 6428 226c 6e22  odes.append("ln"
-000072b0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000072c0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-000072d0: 6428 226c 7422 290d 0a20 2020 2020 2020  d("lt")..       
-000072e0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-000072f0: 2e61 7070 656e 6428 226c 6722 290d 0a20  .append("lg").. 
-00007300: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007310: 5f63 6f64 6573 2e61 7070 656e 6428 226c  _codes.append("l
-00007320: 6222 290d 0a20 2020 2020 2020 2073 656c  b")..        sel
-00007330: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00007340: 656e 6428 226d 6b22 290d 0a20 2020 2020  end("mk")..     
-00007350: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00007360: 6573 2e61 7070 656e 6428 226d 6722 290d  es.append("mg").
-00007370: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00007380: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00007390: 226d 7322 290d 0a20 2020 2020 2020 2073  "ms")..        s
-000073a0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-000073b0: 7070 656e 6428 226d 6c22 290d 0a20 2020  ppend("ml")..   
-000073c0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-000073d0: 6f64 6573 2e61 7070 656e 6428 226d 7422  odes.append("mt"
-000073e0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000073f0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00007400: 6428 226d 6922 290d 0a20 2020 2020 2020  d("mi")..       
-00007410: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00007420: 2e61 7070 656e 6428 226d 7222 290d 0a20  .append("mr").. 
-00007430: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007440: 5f63 6f64 6573 2e61 7070 656e 6428 226d  _codes.append("m
-00007450: 6e69 2d4d 7465 6922 290d 0a20 2020 2020  ni-Mtei")..     
-00007460: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00007470: 6573 2e61 7070 656e 6428 226c 7573 2229  es.append("lus")
-00007480: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007490: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-000074a0: 2822 6d6e 2229 0d0a 2020 2020 2020 2020  ("mn")..        
-000074b0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-000074c0: 6170 7065 6e64 2822 6d79 2229 0d0a 2020  append("my")..  
-000074d0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000074e0: 636f 6465 732e 6170 7065 6e64 2822 6e65  codes.append("ne
-000074f0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007500: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00007510: 6e64 2822 6e6f 2229 0d0a 2020 2020 2020  nd("no")..      
-00007520: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00007530: 732e 6170 7065 6e64 2822 6f72 2229 0d0a  s.append("or")..
-00007540: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007550: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00007560: 6f6d 2229 0d0a 2020 2020 2020 2020 7365  om")..        se
-00007570: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-00007580: 7065 6e64 2822 7073 2229 0d0a 2020 2020  pend("ps")..    
-00007590: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000075a0: 6465 732e 6170 7065 6e64 2822 6661 2229  des.append("fa")
-000075b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000075c0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-000075d0: 2822 706c 2229 0d0a 2020 2020 2020 2020  ("pl")..        
-000075e0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-000075f0: 6170 7065 6e64 2822 7074 2229 0d0a 2020  append("pt")..  
-00007600: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007610: 636f 6465 732e 6170 7065 6e64 2822 7061  codes.append("pa
-00007620: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00007630: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
-00007640: 6e64 2822 7175 2229 0d0a 2020 2020 2020  nd("qu")..      
-00007650: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
-00007660: 732e 6170 7065 6e64 2822 726f 2229 0d0a  s.append("ro")..
-00007670: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007680: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
-00007690: 7275 2229 0d0a 2020 2020 2020 2020 7365  ru")..        se
-000076a0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
-000076b0: 7065 6e64 2822 736d 2229 0d0a 2020 2020  pend("sm")..    
-000076c0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
-000076d0: 6465 732e 6170 7065 6e64 2822 7361 2229  des.append("sa")
-000076e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000076f0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
-00007700: 2822 6764 2229 0d0a 2020 2020 2020 2020  ("gd")..        
-00007710: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
-00007720: 6170 7065 6e64 2822 6e73 6f22 290d 0a20  append("nso").. 
-00007730: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007740: 5f63 6f64 6573 2e61 7070 656e 6428 2273  _codes.append("s
-00007750: 7222 290d 0a20 2020 2020 2020 2073 656c  r")..        sel
-00007760: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00007770: 656e 6428 2273 7422 290d 0a20 2020 2020  end("st")..     
-00007780: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00007790: 6573 2e61 7070 656e 6428 2273 6e22 290d  es.append("sn").
-000077a0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000077b0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-000077c0: 2273 6422 290d 0a20 2020 2020 2020 2073  "sd")..        s
-000077d0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-000077e0: 7070 656e 6428 2273 6922 290d 0a20 2020  ppend("si")..   
-000077f0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00007800: 6f64 6573 2e61 7070 656e 6428 2273 6b22  odes.append("sk"
-00007810: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007820: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00007830: 6428 2273 6c22 290d 0a20 2020 2020 2020  d("sl")..       
-00007840: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00007850: 2e61 7070 656e 6428 2273 6f22 290d 0a20  .append("so").. 
-00007860: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007870: 5f63 6f64 6573 2e61 7070 656e 6428 2265  _codes.append("e
-00007880: 7322 290d 0a20 2020 2020 2020 2073 656c  s")..        sel
-00007890: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-000078a0: 656e 6428 2273 7522 290d 0a20 2020 2020  end("su")..     
-000078b0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-000078c0: 6573 2e61 7070 656e 6428 2273 7722 290d  es.append("sw").
-000078d0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000078e0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-000078f0: 2273 7622 290d 0a20 2020 2020 2020 2073  "sv")..        s
-00007900: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00007910: 7070 656e 6428 2274 6722 290d 0a20 2020  ppend("tg")..   
-00007920: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00007930: 6f64 6573 2e61 7070 656e 6428 2274 6122  odes.append("ta"
-00007940: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007950: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00007960: 6428 2274 7422 290d 0a20 2020 2020 2020  d("tt")..       
-00007970: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00007980: 2e61 7070 656e 6428 2274 6522 290d 0a20  .append("te").. 
-00007990: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-000079a0: 5f63 6f64 6573 2e61 7070 656e 6428 2274  _codes.append("t
-000079b0: 6822 290d 0a20 2020 2020 2020 2073 656c  h")..        sel
-000079c0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-000079d0: 656e 6428 2274 6922 290d 0a20 2020 2020  end("ti")..     
-000079e0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-000079f0: 6573 2e61 7070 656e 6428 2274 7322 290d  es.append("ts").
-00007a00: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00007a10: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00007a20: 2274 7222 290d 0a20 2020 2020 2020 2073  "tr")..        s
-00007a30: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00007a40: 7070 656e 6428 2274 6b22 290d 0a20 2020  ppend("tk")..   
-00007a50: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00007a60: 6f64 6573 2e61 7070 656e 6428 2274 7722  odes.append("tw"
-00007a70: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007a80: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00007a90: 6428 2275 6b22 290d 0a20 2020 2020 2020  d("uk")..       
-00007aa0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00007ab0: 2e61 7070 656e 6428 2275 7222 290d 0a20  .append("ur").. 
-00007ac0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007ad0: 5f63 6f64 6573 2e61 7070 656e 6428 2275  _codes.append("u
-00007ae0: 6722 290d 0a20 2020 2020 2020 2073 656c  g")..        sel
-00007af0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
-00007b00: 656e 6428 2275 7a22 290d 0a20 2020 2020  end("uz")..     
-00007b10: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
-00007b20: 6573 2e61 7070 656e 6428 2276 6922 290d  es.append("vi").
-00007b30: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00007b40: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
-00007b50: 2263 7922 290d 0a20 2020 2020 2020 2073  "cy")..        s
-00007b60: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
-00007b70: 7070 656e 6428 2278 6822 290d 0a20 2020  ppend("xh")..   
-00007b80: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
-00007b90: 6f64 6573 2e61 7070 656e 6428 2279 6922  odes.append("yi"
+00006560: 2020 2020 2020 2020 2779 6f27 3a20 2759          'yo': 'Y
+00006570: 6f72 7562 6127 2c0d 0a20 2020 2020 2020  oruba',..       
+00006580: 2020 2020 2020 2020 2020 2020 207d 0d0a               }..
+00006590: 0d0a 2020 2020 6465 6620 6765 745f 6e61  ..    def get_na
+000065a0: 6d65 2873 656c 662c 2067 6574 5f63 6f64  me(self, get_cod
+000065b0: 6529 3a0d 0a20 2020 2020 2020 2072 6574  e):..        ret
+000065c0: 7572 6e20 7365 6c66 2e64 6963 742e 6765  urn self.dict.ge
+000065d0: 7428 6765 745f 636f 6465 2e6c 6f77 6572  t(get_code.lower
+000065e0: 2829 2c20 2222 290d 0a0d 0a20 2020 2064  (), "")....    d
+000065f0: 6566 2067 6574 5f63 6f64 6528 7365 6c66  ef get_code(self
+00006600: 2c20 6c61 6e67 7561 6765 293a 0d0a 2020  , language):..  
+00006610: 2020 2020 2020 666f 7220 6765 745f 636f        for get_co
+00006620: 6465 2c20 6c61 6e67 2069 6e20 7365 6c66  de, lang in self
+00006630: 2e64 6963 742e 6974 656d 7328 293a 0d0a  .dict.items():..
+00006640: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00006650: 616e 672e 6c6f 7765 7228 2920 3d3d 206c  ang.lower() == l
+00006660: 616e 6775 6167 652e 6c6f 7765 7228 293a  anguage.lower():
+00006670: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006680: 2020 7265 7475 726e 2067 6574 5f63 6f64    return get_cod
+00006690: 650d 0a20 2020 2020 2020 2072 6574 7572  e..        retur
+000066a0: 6e20 2222 0d0a 0d0a 0d0a 636c 6173 7320  n ""......class 
+000066b0: 476f 6f67 6c65 4c61 6e67 7561 6765 3a0d  GoogleLanguage:.
+000066c0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000066d0: 5f28 7365 6c66 293a 0d0a 2020 2020 2020  _(self):..      
+000066e0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+000066f0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00006700: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00006710: 6170 7065 6e64 2822 6166 2229 0d0a 2020  append("af")..  
+00006720: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00006730: 636f 6465 732e 6170 7065 6e64 2822 7371  codes.append("sq
+00006740: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00006750: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00006760: 6e64 2822 616d 2229 0d0a 2020 2020 2020  nd("am")..      
+00006770: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00006780: 732e 6170 7065 6e64 2822 6172 2229 0d0a  s.append("ar")..
+00006790: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000067a0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+000067b0: 6879 2229 0d0a 2020 2020 2020 2020 7365  hy")..        se
+000067c0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+000067d0: 7065 6e64 2822 6173 2229 0d0a 2020 2020  pend("as")..    
+000067e0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+000067f0: 6465 732e 6170 7065 6e64 2822 6179 2229  des.append("ay")
+00006800: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00006810: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00006820: 2822 617a 2229 0d0a 2020 2020 2020 2020  ("az")..        
+00006830: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00006840: 6170 7065 6e64 2822 626d 2229 0d0a 2020  append("bm")..  
+00006850: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00006860: 636f 6465 732e 6170 7065 6e64 2822 6575  codes.append("eu
+00006870: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00006880: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00006890: 6e64 2822 6265 2229 0d0a 2020 2020 2020  nd("be")..      
+000068a0: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+000068b0: 732e 6170 7065 6e64 2822 626e 2229 0d0a  s.append("bn")..
+000068c0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000068d0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+000068e0: 6268 6f22 290d 0a20 2020 2020 2020 2073  bho")..        s
+000068f0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00006900: 7070 656e 6428 2262 7322 290d 0a20 2020  ppend("bs")..   
+00006910: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00006920: 6f64 6573 2e61 7070 656e 6428 2262 6722  odes.append("bg"
+00006930: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00006940: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00006950: 6428 2263 6122 290d 0a20 2020 2020 2020  d("ca")..       
+00006960: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00006970: 2e61 7070 656e 6428 2263 6562 2229 0d0a  .append("ceb")..
+00006980: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00006990: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+000069a0: 6e79 2229 0d0a 2020 2020 2020 2020 7365  ny")..        se
+000069b0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+000069c0: 7065 6e64 2822 7a68 2d43 4e22 290d 0a20  pend("zh-CN").. 
+000069d0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000069e0: 5f63 6f64 6573 2e61 7070 656e 6428 227a  _codes.append("z
+000069f0: 682d 5457 2229 0d0a 2020 2020 2020 2020  h-TW")..        
+00006a00: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00006a10: 6170 7065 6e64 2822 636f 2229 0d0a 2020  append("co")..  
+00006a20: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00006a30: 636f 6465 732e 6170 7065 6e64 2822 6872  codes.append("hr
+00006a40: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00006a50: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00006a60: 6e64 2822 6373 2229 0d0a 2020 2020 2020  nd("cs")..      
+00006a70: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00006a80: 732e 6170 7065 6e64 2822 6461 2229 0d0a  s.append("da")..
+00006a90: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00006aa0: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00006ab0: 6476 2229 0d0a 2020 2020 2020 2020 7365  dv")..        se
+00006ac0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00006ad0: 7065 6e64 2822 646f 6922 290d 0a20 2020  pend("doi")..   
+00006ae0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00006af0: 6f64 6573 2e61 7070 656e 6428 226e 6c22  odes.append("nl"
+00006b00: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00006b10: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00006b20: 6428 2265 6e22 290d 0a20 2020 2020 2020  d("en")..       
+00006b30: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00006b40: 2e61 7070 656e 6428 2265 6f22 290d 0a20  .append("eo").. 
+00006b50: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00006b60: 5f63 6f64 6573 2e61 7070 656e 6428 2265  _codes.append("e
+00006b70: 7422 290d 0a20 2020 2020 2020 2073 656c  t")..        sel
+00006b80: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00006b90: 656e 6428 2265 6522 290d 0a20 2020 2020  end("ee")..     
+00006ba0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00006bb0: 6573 2e61 7070 656e 6428 2266 696c 2229  es.append("fil")
+00006bc0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00006bd0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00006be0: 2822 6669 2229 0d0a 2020 2020 2020 2020  ("fi")..        
+00006bf0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00006c00: 6170 7065 6e64 2822 6672 2229 0d0a 2020  append("fr")..  
+00006c10: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00006c20: 636f 6465 732e 6170 7065 6e64 2822 6679  codes.append("fy
+00006c30: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00006c40: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00006c50: 6e64 2822 676c 2229 0d0a 2020 2020 2020  nd("gl")..      
+00006c60: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00006c70: 732e 6170 7065 6e64 2822 6b61 2229 0d0a  s.append("ka")..
+00006c80: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00006c90: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00006ca0: 6465 2229 0d0a 2020 2020 2020 2020 7365  de")..        se
+00006cb0: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00006cc0: 7065 6e64 2822 656c 2229 0d0a 2020 2020  pend("el")..    
+00006cd0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00006ce0: 6465 732e 6170 7065 6e64 2822 676e 2229  des.append("gn")
+00006cf0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00006d00: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00006d10: 2822 6775 2229 0d0a 2020 2020 2020 2020  ("gu")..        
+00006d20: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+00006d30: 6170 7065 6e64 2822 6874 2229 0d0a 2020  append("ht")..  
+00006d40: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00006d50: 636f 6465 732e 6170 7065 6e64 2822 6861  codes.append("ha
+00006d60: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00006d70: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00006d80: 6e64 2822 6861 7722 290d 0a20 2020 2020  nd("haw")..     
+00006d90: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00006da0: 6573 2e61 7070 656e 6428 2268 6522 290d  es.append("he").
+00006db0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00006dc0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00006dd0: 2268 6922 290d 0a20 2020 2020 2020 2073  "hi")..        s
+00006de0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00006df0: 7070 656e 6428 2268 6d6e 2229 0d0a 2020  ppend("hmn")..  
+00006e00: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00006e10: 636f 6465 732e 6170 7065 6e64 2822 6875  codes.append("hu
+00006e20: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00006e30: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00006e40: 6e64 2822 6973 2229 0d0a 2020 2020 2020  nd("is")..      
+00006e50: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00006e60: 732e 6170 7065 6e64 2822 6967 2229 0d0a  s.append("ig")..
+00006e70: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00006e80: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00006e90: 696c 6f22 290d 0a20 2020 2020 2020 2073  ilo")..        s
+00006ea0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00006eb0: 7070 656e 6428 2269 6422 290d 0a20 2020  ppend("id")..   
+00006ec0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00006ed0: 6f64 6573 2e61 7070 656e 6428 2267 6122  odes.append("ga"
+00006ee0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00006ef0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00006f00: 6428 2269 7422 290d 0a20 2020 2020 2020  d("it")..       
+00006f10: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00006f20: 2e61 7070 656e 6428 226a 6122 290d 0a20  .append("ja").. 
+00006f30: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00006f40: 5f63 6f64 6573 2e61 7070 656e 6428 226a  _codes.append("j
+00006f50: 7622 290d 0a20 2020 2020 2020 2073 656c  v")..        sel
+00006f60: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00006f70: 656e 6428 226b 6e22 290d 0a20 2020 2020  end("kn")..     
+00006f80: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00006f90: 6573 2e61 7070 656e 6428 226b 6b22 290d  es.append("kk").
+00006fa0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00006fb0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00006fc0: 226b 6d22 290d 0a20 2020 2020 2020 2073  "km")..        s
+00006fd0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00006fe0: 7070 656e 6428 2272 7722 290d 0a20 2020  ppend("rw")..   
+00006ff0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00007000: 6f64 6573 2e61 7070 656e 6428 2267 6f6d  odes.append("gom
+00007010: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00007020: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00007030: 6e64 2822 6b6f 2229 0d0a 2020 2020 2020  nd("ko")..      
+00007040: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00007050: 732e 6170 7065 6e64 2822 6b72 6922 290d  s.append("kri").
+00007060: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007070: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00007080: 226b 6d72 2229 0d0a 2020 2020 2020 2020  "kmr")..        
+00007090: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+000070a0: 6170 7065 6e64 2822 636b 6222 290d 0a20  append("ckb").. 
+000070b0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000070c0: 5f63 6f64 6573 2e61 7070 656e 6428 226b  _codes.append("k
+000070d0: 7922 290d 0a20 2020 2020 2020 2073 656c  y")..        sel
+000070e0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+000070f0: 656e 6428 226c 6f22 290d 0a20 2020 2020  end("lo")..     
+00007100: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00007110: 6573 2e61 7070 656e 6428 226c 6122 290d  es.append("la").
+00007120: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007130: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00007140: 226c 7622 290d 0a20 2020 2020 2020 2073  "lv")..        s
+00007150: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00007160: 7070 656e 6428 226c 6e22 290d 0a20 2020  ppend("ln")..   
+00007170: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00007180: 6f64 6573 2e61 7070 656e 6428 226c 7422  odes.append("lt"
+00007190: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000071a0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+000071b0: 6428 226c 6722 290d 0a20 2020 2020 2020  d("lg")..       
+000071c0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+000071d0: 2e61 7070 656e 6428 226c 6222 290d 0a20  .append("lb").. 
+000071e0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000071f0: 5f63 6f64 6573 2e61 7070 656e 6428 226d  _codes.append("m
+00007200: 6b22 290d 0a20 2020 2020 2020 2073 656c  k")..        sel
+00007210: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00007220: 656e 6428 226d 6722 290d 0a20 2020 2020  end("mg")..     
+00007230: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00007240: 6573 2e61 7070 656e 6428 226d 7322 290d  es.append("ms").
+00007250: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007260: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00007270: 226d 6c22 290d 0a20 2020 2020 2020 2073  "ml")..        s
+00007280: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00007290: 7070 656e 6428 226d 7422 290d 0a20 2020  ppend("mt")..   
+000072a0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+000072b0: 6f64 6573 2e61 7070 656e 6428 226d 6922  odes.append("mi"
+000072c0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000072d0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+000072e0: 6428 226d 7222 290d 0a20 2020 2020 2020  d("mr")..       
+000072f0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007300: 2e61 7070 656e 6428 226d 6e69 2d4d 7465  .append("mni-Mte
+00007310: 6922 290d 0a20 2020 2020 2020 2073 656c  i")..        sel
+00007320: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00007330: 656e 6428 226c 7573 2229 0d0a 2020 2020  end("lus")..    
+00007340: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00007350: 6465 732e 6170 7065 6e64 2822 6d6e 2229  des.append("mn")
+00007360: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00007370: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+00007380: 2822 6d79 2229 0d0a 2020 2020 2020 2020  ("my")..        
+00007390: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+000073a0: 6170 7065 6e64 2822 6e65 2229 0d0a 2020  append("ne")..  
+000073b0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000073c0: 636f 6465 732e 6170 7065 6e64 2822 6e6f  codes.append("no
+000073d0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000073e0: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+000073f0: 6e64 2822 6f72 2229 0d0a 2020 2020 2020  nd("or")..      
+00007400: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00007410: 732e 6170 7065 6e64 2822 6f6d 2229 0d0a  s.append("om")..
+00007420: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007430: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00007440: 7073 2229 0d0a 2020 2020 2020 2020 7365  ps")..        se
+00007450: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00007460: 7065 6e64 2822 6661 2229 0d0a 2020 2020  pend("fa")..    
+00007470: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+00007480: 6465 732e 6170 7065 6e64 2822 706c 2229  des.append("pl")
+00007490: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000074a0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+000074b0: 2822 7074 2229 0d0a 2020 2020 2020 2020  ("pt")..        
+000074c0: 7365 6c66 2e6c 6973 745f 636f 6465 732e  self.list_codes.
+000074d0: 6170 7065 6e64 2822 7061 2229 0d0a 2020  append("pa")..  
+000074e0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000074f0: 636f 6465 732e 6170 7065 6e64 2822 7175  codes.append("qu
+00007500: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00007510: 2e6c 6973 745f 636f 6465 732e 6170 7065  .list_codes.appe
+00007520: 6e64 2822 726f 2229 0d0a 2020 2020 2020  nd("ro")..      
+00007530: 2020 7365 6c66 2e6c 6973 745f 636f 6465    self.list_code
+00007540: 732e 6170 7065 6e64 2822 7275 2229 0d0a  s.append("ru")..
+00007550: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007560: 745f 636f 6465 732e 6170 7065 6e64 2822  t_codes.append("
+00007570: 736d 2229 0d0a 2020 2020 2020 2020 7365  sm")..        se
+00007580: 6c66 2e6c 6973 745f 636f 6465 732e 6170  lf.list_codes.ap
+00007590: 7065 6e64 2822 7361 2229 0d0a 2020 2020  pend("sa")..    
+000075a0: 2020 2020 7365 6c66 2e6c 6973 745f 636f      self.list_co
+000075b0: 6465 732e 6170 7065 6e64 2822 6764 2229  des.append("gd")
+000075c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000075d0: 6973 745f 636f 6465 732e 6170 7065 6e64  ist_codes.append
+000075e0: 2822 6e73 6f22 290d 0a20 2020 2020 2020  ("nso")..       
+000075f0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007600: 2e61 7070 656e 6428 2273 7222 290d 0a20  .append("sr").. 
+00007610: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007620: 5f63 6f64 6573 2e61 7070 656e 6428 2273  _codes.append("s
+00007630: 7422 290d 0a20 2020 2020 2020 2073 656c  t")..        sel
+00007640: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00007650: 656e 6428 2273 6e22 290d 0a20 2020 2020  end("sn")..     
+00007660: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00007670: 6573 2e61 7070 656e 6428 2273 6422 290d  es.append("sd").
+00007680: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007690: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+000076a0: 2273 6922 290d 0a20 2020 2020 2020 2073  "si")..        s
+000076b0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+000076c0: 7070 656e 6428 2273 6b22 290d 0a20 2020  ppend("sk")..   
+000076d0: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+000076e0: 6f64 6573 2e61 7070 656e 6428 2273 6c22  odes.append("sl"
+000076f0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007700: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007710: 6428 2273 6f22 290d 0a20 2020 2020 2020  d("so")..       
+00007720: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007730: 2e61 7070 656e 6428 2265 7322 290d 0a20  .append("es").. 
+00007740: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007750: 5f63 6f64 6573 2e61 7070 656e 6428 2273  _codes.append("s
+00007760: 7522 290d 0a20 2020 2020 2020 2073 656c  u")..        sel
+00007770: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+00007780: 656e 6428 2273 7722 290d 0a20 2020 2020  end("sw")..     
+00007790: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+000077a0: 6573 2e61 7070 656e 6428 2273 7622 290d  es.append("sv").
+000077b0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000077c0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+000077d0: 2274 6722 290d 0a20 2020 2020 2020 2073  "tg")..        s
+000077e0: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+000077f0: 7070 656e 6428 2274 6122 290d 0a20 2020  ppend("ta")..   
+00007800: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00007810: 6f64 6573 2e61 7070 656e 6428 2274 7422  odes.append("tt"
+00007820: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007830: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007840: 6428 2274 6522 290d 0a20 2020 2020 2020  d("te")..       
+00007850: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007860: 2e61 7070 656e 6428 2274 6822 290d 0a20  .append("th").. 
+00007870: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007880: 5f63 6f64 6573 2e61 7070 656e 6428 2274  _codes.append("t
+00007890: 6922 290d 0a20 2020 2020 2020 2073 656c  i")..        sel
+000078a0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+000078b0: 656e 6428 2274 7322 290d 0a20 2020 2020  end("ts")..     
+000078c0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+000078d0: 6573 2e61 7070 656e 6428 2274 7222 290d  es.append("tr").
+000078e0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000078f0: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00007900: 2274 6b22 290d 0a20 2020 2020 2020 2073  "tk")..        s
+00007910: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00007920: 7070 656e 6428 2274 7722 290d 0a20 2020  ppend("tw")..   
+00007930: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00007940: 6f64 6573 2e61 7070 656e 6428 2275 6b22  odes.append("uk"
+00007950: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007960: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007970: 6428 2275 7222 290d 0a20 2020 2020 2020  d("ur")..       
+00007980: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
+00007990: 2e61 7070 656e 6428 2275 6722 290d 0a20  .append("ug").. 
+000079a0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000079b0: 5f63 6f64 6573 2e61 7070 656e 6428 2275  _codes.append("u
+000079c0: 7a22 290d 0a20 2020 2020 2020 2073 656c  z")..        sel
+000079d0: 662e 6c69 7374 5f63 6f64 6573 2e61 7070  f.list_codes.app
+000079e0: 656e 6428 2276 6922 290d 0a20 2020 2020  end("vi")..     
+000079f0: 2020 2073 656c 662e 6c69 7374 5f63 6f64     self.list_cod
+00007a00: 6573 2e61 7070 656e 6428 2263 7922 290d  es.append("cy").
+00007a10: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00007a20: 7374 5f63 6f64 6573 2e61 7070 656e 6428  st_codes.append(
+00007a30: 2278 6822 290d 0a20 2020 2020 2020 2073  "xh")..        s
+00007a40: 656c 662e 6c69 7374 5f63 6f64 6573 2e61  elf.list_codes.a
+00007a50: 7070 656e 6428 2279 6922 290d 0a20 2020  ppend("yi")..   
+00007a60: 2020 2020 2073 656c 662e 6c69 7374 5f63       self.list_c
+00007a70: 6f64 6573 2e61 7070 656e 6428 2279 6f22  odes.append("yo"
+00007a80: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007a90: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
+00007aa0: 6428 227a 7522 290d 0a0d 0a20 2020 2020  d("zu")....     
+00007ab0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00007ac0: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
+00007ad0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00007ae0: 2e61 7070 656e 6428 2241 6672 696b 6161  .append("Afrikaa
+00007af0: 6e73 2229 0d0a 2020 2020 2020 2020 7365  ns")..        se
+00007b00: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00007b10: 7065 6e64 2822 416c 6261 6e69 616e 2229  pend("Albanian")
+00007b20: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00007b30: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00007b40: 2822 416d 6861 7269 6322 290d 0a20 2020  ("Amharic")..   
+00007b50: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00007b60: 616d 6573 2e61 7070 656e 6428 2241 7261  ames.append("Ara
+00007b70: 6269 6322 290d 0a20 2020 2020 2020 2073  bic")..        s
+00007b80: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00007b90: 7070 656e 6428 2241 726d 656e 6961 6e22  ppend("Armenian"
 00007ba0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007bb0: 6c69 7374 5f63 6f64 6573 2e61 7070 656e  list_codes.appen
-00007bc0: 6428 2279 6f22 290d 0a20 2020 2020 2020  d("yo")..       
-00007bd0: 2073 656c 662e 6c69 7374 5f63 6f64 6573   self.list_codes
-00007be0: 2e61 7070 656e 6428 227a 7522 290d 0a0d  .append("zu")...
-00007bf0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00007c00: 7374 5f6e 616d 6573 203d 205b 5d0d 0a20  st_names = [].. 
-00007c10: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007c20: 5f6e 616d 6573 2e61 7070 656e 6428 2241  _names.append("A
-00007c30: 6672 696b 6161 6e73 2229 0d0a 2020 2020  frikaans")..    
-00007c40: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00007c50: 6d65 732e 6170 7065 6e64 2822 416c 6261  mes.append("Alba
-00007c60: 6e69 616e 2229 0d0a 2020 2020 2020 2020  nian")..        
-00007c70: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00007c80: 6170 7065 6e64 2822 416d 6861 7269 6322  append("Amharic"
-00007c90: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007ca0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00007cb0: 6428 2241 7261 6269 6322 290d 0a20 2020  d("Arabic")..   
-00007cc0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00007cd0: 616d 6573 2e61 7070 656e 6428 2241 726d  ames.append("Arm
-00007ce0: 656e 6961 6e22 290d 0a20 2020 2020 2020  enian")..       
-00007cf0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00007d00: 2e61 7070 656e 6428 2241 7373 616d 6573  .append("Assames
-00007d10: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
-00007d20: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00007d30: 656e 6428 2241 796d 6172 6122 290d 0a20  end("Aymara").. 
-00007d40: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007d50: 5f6e 616d 6573 2e61 7070 656e 6428 2241  _names.append("A
-00007d60: 7a65 7262 6169 6a61 6e69 2229 0d0a 2020  zerbaijani")..  
-00007d70: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00007d80: 6e61 6d65 732e 6170 7065 6e64 2822 4261  names.append("Ba
-00007d90: 6d62 6172 6122 290d 0a20 2020 2020 2020  mbara")..       
-00007da0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00007db0: 2e61 7070 656e 6428 2242 6173 7175 6522  .append("Basque"
-00007dc0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007dd0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00007de0: 6428 2242 656c 6172 7573 6961 6e22 290d  d("Belarusian").
-00007df0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00007e00: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00007e10: 2242 656e 6761 6c69 2229 0d0a 2020 2020  "Bengali")..    
-00007e20: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00007e30: 6d65 732e 6170 7065 6e64 2822 4268 6f6a  mes.append("Bhoj
-00007e40: 7075 7269 2229 0d0a 2020 2020 2020 2020  puri")..        
-00007e50: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00007e60: 6170 7065 6e64 2822 426f 736e 6961 6e22  append("Bosnian"
-00007e70: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007e80: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00007e90: 6428 2242 756c 6761 7269 616e 2229 0d0a  d("Bulgarian")..
-00007ea0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00007eb0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00007ec0: 4361 7461 6c61 6e22 290d 0a20 2020 2020  Catalan")..     
-00007ed0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00007ee0: 6573 2e61 7070 656e 6428 2243 6562 7561  es.append("Cebua
-00007ef0: 6e6f 2229 0d0a 2020 2020 2020 2020 7365  no")..        se
-00007f00: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00007f10: 7065 6e64 2822 4368 6963 6865 7761 2229  pend("Chichewa")
-00007f20: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00007f30: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00007f40: 2822 4368 696e 6573 6520 2853 696d 706c  ("Chinese (Simpl
-00007f50: 6966 6965 6429 2229 0d0a 2020 2020 2020  ified)")..      
-00007f60: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00007f70: 732e 6170 7065 6e64 2822 4368 696e 6573  s.append("Chines
-00007f80: 6520 2854 7261 6469 7469 6f6e 616c 2922  e (Traditional)"
-00007f90: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00007fa0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00007fb0: 6428 2243 6f72 7369 6361 6e22 290d 0a20  d("Corsican").. 
-00007fc0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00007fd0: 5f6e 616d 6573 2e61 7070 656e 6428 2243  _names.append("C
-00007fe0: 726f 6174 6961 6e22 290d 0a20 2020 2020  roatian")..     
-00007ff0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00008000: 6573 2e61 7070 656e 6428 2243 7a65 6368  es.append("Czech
-00008010: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008020: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008030: 6e64 2822 4461 6e69 7368 2229 0d0a 2020  nd("Danish")..  
-00008040: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008050: 6e61 6d65 732e 6170 7065 6e64 2822 4468  names.append("Dh
-00008060: 6976 6568 6922 290d 0a20 2020 2020 2020  ivehi")..       
-00008070: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-00008080: 2e61 7070 656e 6428 2244 6f67 7269 2229  .append("Dogri")
-00008090: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000080a0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-000080b0: 2822 4475 7463 6822 290d 0a20 2020 2020  ("Dutch")..     
-000080c0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-000080d0: 6573 2e61 7070 656e 6428 2245 6e67 6c69  es.append("Engli
-000080e0: 7368 2229 0d0a 2020 2020 2020 2020 7365  sh")..        se
-000080f0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008100: 7065 6e64 2822 4573 7065 7261 6e74 6f22  pend("Esperanto"
-00008110: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008120: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008130: 6428 2245 7374 6f6e 6961 6e22 290d 0a20  d("Estonian").. 
-00008140: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008150: 5f6e 616d 6573 2e61 7070 656e 6428 2245  _names.append("E
-00008160: 7765 2229 0d0a 2020 2020 2020 2020 7365  we")..        se
-00008170: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008180: 7065 6e64 2822 4669 6c69 7069 6e6f 2229  pend("Filipino")
-00008190: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000081a0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-000081b0: 2822 4669 6e6e 6973 6822 290d 0a20 2020  ("Finnish")..   
-000081c0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-000081d0: 616d 6573 2e61 7070 656e 6428 2246 7265  ames.append("Fre
-000081e0: 6e63 6822 290d 0a20 2020 2020 2020 2073  nch")..        s
-000081f0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008200: 7070 656e 6428 2246 7269 7369 616e 2229  ppend("Frisian")
-00008210: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00008220: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00008230: 2822 4761 6c69 6369 616e 2229 0d0a 2020  ("Galician")..  
-00008240: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008250: 6e61 6d65 732e 6170 7065 6e64 2822 4765  names.append("Ge
-00008260: 6f72 6769 616e 2229 0d0a 2020 2020 2020  orgian")..      
-00008270: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00008280: 732e 6170 7065 6e64 2822 4765 726d 616e  s.append("German
-00008290: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000082a0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-000082b0: 6e64 2822 4772 6565 6b22 290d 0a20 2020  nd("Greek")..   
-000082c0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-000082d0: 616d 6573 2e61 7070 656e 6428 2247 7561  ames.append("Gua
-000082e0: 7261 6e69 2229 0d0a 2020 2020 2020 2020  rani")..        
-000082f0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00008300: 6170 7065 6e64 2822 4775 6a61 7261 7469  append("Gujarati
-00008310: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008320: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008330: 6e64 2822 4861 6974 6961 6e20 4372 656f  nd("Haitian Creo
-00008340: 6c65 2229 0d0a 2020 2020 2020 2020 7365  le")..        se
-00008350: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008360: 7065 6e64 2822 4861 7573 6122 290d 0a20  pend("Hausa").. 
-00008370: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008380: 5f6e 616d 6573 2e61 7070 656e 6428 2248  _names.append("H
-00008390: 6177 6169 6961 6e22 290d 0a20 2020 2020  awaiian")..     
-000083a0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-000083b0: 6573 2e61 7070 656e 6428 2248 6562 7265  es.append("Hebre
-000083c0: 7722 290d 0a20 2020 2020 2020 2073 656c  w")..        sel
-000083d0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-000083e0: 656e 6428 2248 696e 6469 2229 0d0a 2020  end("Hindi")..  
-000083f0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008400: 6e61 6d65 732e 6170 7065 6e64 2822 486d  names.append("Hm
-00008410: 6f6e 6722 290d 0a20 2020 2020 2020 2073  ong")..        s
-00008420: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008430: 7070 656e 6428 2248 756e 6761 7269 616e  ppend("Hungarian
-00008440: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008450: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008460: 6e64 2822 4963 656c 616e 6469 6322 290d  nd("Icelandic").
-00008470: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008480: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008490: 2249 6762 6f22 290d 0a20 2020 2020 2020  "Igbo")..       
-000084a0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-000084b0: 2e61 7070 656e 6428 2249 6c6f 6361 6e6f  .append("Ilocano
-000084c0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000084d0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-000084e0: 6e64 2822 496e 646f 6e65 7369 616e 2229  nd("Indonesian")
-000084f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00008500: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00008510: 2822 4972 6973 6822 290d 0a20 2020 2020  ("Irish")..     
-00008520: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00008530: 6573 2e61 7070 656e 6428 2249 7461 6c69  es.append("Itali
-00008540: 616e 2229 0d0a 2020 2020 2020 2020 7365  an")..        se
-00008550: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008560: 7065 6e64 2822 4a61 7061 6e65 7365 2229  pend("Japanese")
-00008570: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00008580: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00008590: 2822 4a61 7661 6e65 7365 2229 0d0a 2020  ("Javanese")..  
-000085a0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-000085b0: 6e61 6d65 732e 6170 7065 6e64 2822 4b61  names.append("Ka
-000085c0: 6e6e 6164 6122 290d 0a20 2020 2020 2020  nnada")..       
-000085d0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-000085e0: 2e61 7070 656e 6428 224b 617a 616b 6822  .append("Kazakh"
-000085f0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008600: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008610: 6428 224b 686d 6572 2229 0d0a 2020 2020  d("Khmer")..    
-00008620: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008630: 6d65 732e 6170 7065 6e64 2822 4b69 6e79  mes.append("Kiny
-00008640: 6172 7761 6e64 6122 290d 0a20 2020 2020  arwanda")..     
-00008650: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00008660: 6573 2e61 7070 656e 6428 224b 6f6e 6b61  es.append("Konka
-00008670: 6e69 2229 0d0a 2020 2020 2020 2020 7365  ni")..        se
-00008680: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008690: 7065 6e64 2822 4b6f 7265 616e 2229 0d0a  pend("Korean")..
-000086a0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000086b0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000086c0: 4b72 696f 2229 0d0a 2020 2020 2020 2020  Krio")..        
-000086d0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-000086e0: 6170 7065 6e64 2822 4b75 7264 6973 6820  append("Kurdish 
-000086f0: 284b 7572 6d61 6e6a 6929 2229 0d0a 2020  (Kurmanji)")..  
-00008700: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008710: 6e61 6d65 732e 6170 7065 6e64 2822 4b75  names.append("Ku
-00008720: 7264 6973 6820 2853 6f72 616e 6929 2229  rdish (Sorani)")
-00008730: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00008740: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00008750: 2822 4b79 7267 797a 2229 0d0a 2020 2020  ("Kyrgyz")..    
-00008760: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008770: 6d65 732e 6170 7065 6e64 2822 4c61 6f22  mes.append("Lao"
-00008780: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008790: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-000087a0: 6428 224c 6174 696e 2229 0d0a 2020 2020  d("Latin")..    
-000087b0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-000087c0: 6d65 732e 6170 7065 6e64 2822 4c61 7476  mes.append("Latv
-000087d0: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
-000087e0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-000087f0: 7070 656e 6428 224c 696e 6761 6c61 2229  ppend("Lingala")
-00008800: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00008810: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00008820: 2822 4c69 7468 7561 6e69 616e 2229 0d0a  ("Lithuanian")..
-00008830: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00008840: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00008850: 4c75 6761 6e64 6122 290d 0a20 2020 2020  Luganda")..     
-00008860: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00008870: 6573 2e61 7070 656e 6428 224c 7578 656d  es.append("Luxem
-00008880: 626f 7572 6769 7368 2229 0d0a 2020 2020  bourgish")..    
-00008890: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-000088a0: 6d65 732e 6170 7065 6e64 2822 4d61 6365  mes.append("Mace
-000088b0: 646f 6e69 616e 2229 0d0a 2020 2020 2020  donian")..      
-000088c0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-000088d0: 732e 6170 7065 6e64 2822 4d61 6c61 6761  s.append("Malaga
-000088e0: 7379 2229 0d0a 2020 2020 2020 2020 7365  sy")..        se
-000088f0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008900: 7065 6e64 2822 4d61 6c61 7922 290d 0a20  pend("Malay").. 
-00008910: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00008920: 5f6e 616d 6573 2e61 7070 656e 6428 224d  _names.append("M
-00008930: 616c 6179 616c 616d 2229 0d0a 2020 2020  alayalam")..    
-00008940: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008950: 6d65 732e 6170 7065 6e64 2822 4d61 6c74  mes.append("Malt
-00008960: 6573 6522 290d 0a20 2020 2020 2020 2073  ese")..        s
-00008970: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008980: 7070 656e 6428 224d 616f 7269 2229 0d0a  ppend("Maori")..
-00008990: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-000089a0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-000089b0: 4d61 7261 7468 6922 290d 0a20 2020 2020  Marathi")..     
-000089c0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-000089d0: 6573 2e61 7070 656e 6428 224d 6569 7465  es.append("Meite
-000089e0: 696c 6f6e 2028 4d61 6e69 7075 7269 2922  ilon (Manipuri)"
-000089f0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008a00: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008a10: 6428 224d 697a 6f22 290d 0a20 2020 2020  d("Mizo")..     
-00008a20: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00008a30: 6573 2e61 7070 656e 6428 224d 6f6e 676f  es.append("Mongo
-00008a40: 6c69 616e 2229 0d0a 2020 2020 2020 2020  lian")..        
-00008a50: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00008a60: 6170 7065 6e64 2822 4d79 616e 6d61 7220  append("Myanmar 
-00008a70: 2842 7572 6d65 7365 2922 290d 0a20 2020  (Burmese)")..   
-00008a80: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00008a90: 616d 6573 2e61 7070 656e 6428 224e 6570  ames.append("Nep
-00008aa0: 616c 6922 290d 0a20 2020 2020 2020 2073  ali")..        s
-00008ab0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008ac0: 7070 656e 6428 224e 6f72 7765 6769 616e  ppend("Norwegian
-00008ad0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008ae0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008af0: 6e64 2822 4f64 6979 6120 284f 7269 7961  nd("Odiya (Oriya
-00008b00: 2922 290d 0a20 2020 2020 2020 2073 656c  )")..        sel
-00008b10: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00008b20: 656e 6428 224f 726f 6d6f 2229 0d0a 2020  end("Oromo")..  
-00008b30: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008b40: 6e61 6d65 732e 6170 7065 6e64 2822 5061  names.append("Pa
-00008b50: 7368 746f 2229 0d0a 2020 2020 2020 2020  shto")..        
-00008b60: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00008b70: 6170 7065 6e64 2822 5065 7273 6961 6e22  append("Persian"
-00008b80: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008b90: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008ba0: 6428 2250 6f6c 6973 6822 290d 0a20 2020  d("Polish")..   
-00008bb0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00008bc0: 616d 6573 2e61 7070 656e 6428 2250 6f72  ames.append("Por
-00008bd0: 7475 6775 6573 6522 290d 0a20 2020 2020  tuguese")..     
-00008be0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00008bf0: 6573 2e61 7070 656e 6428 2250 756e 6a61  es.append("Punja
-00008c00: 6269 2229 0d0a 2020 2020 2020 2020 7365  bi")..        se
-00008c10: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008c20: 7065 6e64 2822 5175 6563 6875 6122 290d  pend("Quechua").
-00008c30: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008c40: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008c50: 2252 6f6d 616e 6961 6e22 290d 0a20 2020  "Romanian")..   
-00008c60: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00008c70: 616d 6573 2e61 7070 656e 6428 2252 7573  ames.append("Rus
-00008c80: 7369 616e 2229 0d0a 2020 2020 2020 2020  sian")..        
-00008c90: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00008ca0: 6170 7065 6e64 2822 5361 6d6f 616e 2229  append("Samoan")
-00008cb0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-00008cc0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00008cd0: 2822 5361 6e73 6b72 6974 2229 0d0a 2020  ("Sanskrit")..  
-00008ce0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008cf0: 6e61 6d65 732e 6170 7065 6e64 2822 5363  names.append("Sc
-00008d00: 6f74 7320 4761 656c 6963 2229 0d0a 2020  ots Gaelic")..  
-00008d10: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008d20: 6e61 6d65 732e 6170 7065 6e64 2822 5365  names.append("Se
-00008d30: 7065 6469 2229 0d0a 2020 2020 2020 2020  pedi")..        
-00008d40: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00008d50: 6170 7065 6e64 2822 5365 7262 6961 6e22  append("Serbian"
-00008d60: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008d70: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008d80: 6428 2253 6573 6f74 686f 2229 0d0a 2020  d("Sesotho")..  
-00008d90: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00008da0: 6e61 6d65 732e 6170 7065 6e64 2822 5368  names.append("Sh
-00008db0: 6f6e 6122 290d 0a20 2020 2020 2020 2073  ona")..        s
-00008dc0: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00008dd0: 7070 656e 6428 2253 696e 6468 6922 290d  ppend("Sindhi").
-00008de0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00008df0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00008e00: 2253 696e 6861 6c61 2229 0d0a 2020 2020  "Sinhala")..    
-00008e10: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
-00008e20: 6d65 732e 6170 7065 6e64 2822 536c 6f76  mes.append("Slov
-00008e30: 616b 2229 0d0a 2020 2020 2020 2020 7365  ak")..        se
-00008e40: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008e50: 7065 6e64 2822 536c 6f76 656e 6961 6e22  pend("Slovenian"
-00008e60: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00008e70: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
-00008e80: 6428 2253 6f6d 616c 6922 290d 0a20 2020  d("Somali")..   
-00008e90: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00008ea0: 616d 6573 2e61 7070 656e 6428 2253 7061  ames.append("Spa
-00008eb0: 6e69 7368 2229 0d0a 2020 2020 2020 2020  nish")..        
-00008ec0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00008ed0: 6170 7065 6e64 2822 5375 6e64 616e 6573  append("Sundanes
-00008ee0: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
-00008ef0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00008f00: 656e 6428 2253 7761 6869 6c69 2229 0d0a  end("Swahili")..
-00008f10: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00008f20: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00008f30: 5377 6564 6973 6822 290d 0a20 2020 2020  Swedish")..     
-00008f40: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
-00008f50: 6573 2e61 7070 656e 6428 2254 616a 696b  es.append("Tajik
-00008f60: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00008f70: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00008f80: 6e64 2822 5461 6d69 6c22 290d 0a20 2020  nd("Tamil")..   
-00008f90: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
-00008fa0: 616d 6573 2e61 7070 656e 6428 2254 6174  ames.append("Tat
-00008fb0: 6172 2229 0d0a 2020 2020 2020 2020 7365  ar")..        se
-00008fc0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
-00008fd0: 7065 6e64 2822 5465 6c75 6775 2229 0d0a  pend("Telugu")..
-00008fe0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
-00008ff0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
-00009000: 5468 6169 2229 0d0a 2020 2020 2020 2020  Thai")..        
-00009010: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-00009020: 6170 7065 6e64 2822 5469 6772 696e 7961  append("Tigrinya
-00009030: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00009040: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-00009050: 6e64 2822 5473 6f6e 6761 2229 0d0a 2020  nd("Tsonga")..  
-00009060: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00009070: 6e61 6d65 732e 6170 7065 6e64 2822 5475  names.append("Tu
-00009080: 726b 6973 6822 290d 0a20 2020 2020 2020  rkish")..       
-00009090: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
-000090a0: 2e61 7070 656e 6428 2254 7572 6b6d 656e  .append("Turkmen
-000090b0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-000090c0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
-000090d0: 6e64 2822 5477 6920 2841 6b61 6e29 2229  nd("Twi (Akan)")
-000090e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
-000090f0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
-00009100: 2822 556b 7261 696e 6961 6e22 290d 0a20  ("Ukrainian").. 
-00009110: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00009120: 5f6e 616d 6573 2e61 7070 656e 6428 2255  _names.append("U
-00009130: 7264 7522 290d 0a20 2020 2020 2020 2073  rdu")..        s
-00009140: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
-00009150: 7070 656e 6428 2255 7967 6875 7222 290d  ppend("Uyghur").
-00009160: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-00009170: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00009180: 2255 7a62 656b 2229 0d0a 2020 2020 2020  "Uzbek")..      
-00009190: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-000091a0: 732e 6170 7065 6e64 2822 5669 6574 6e61  s.append("Vietna
-000091b0: 6d65 7365 2229 0d0a 2020 2020 2020 2020  mese")..        
-000091c0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
-000091d0: 6170 7065 6e64 2822 5765 6c73 6822 290d  append("Welsh").
-000091e0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
-000091f0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
-00009200: 2258 686f 7361 2229 0d0a 2020 2020 2020  "Xhosa")..      
-00009210: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
-00009220: 732e 6170 7065 6e64 2822 5969 6464 6973  s.append("Yiddis
-00009230: 6822 290d 0a20 2020 2020 2020 2073 656c  h")..        sel
-00009240: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
-00009250: 656e 6428 2259 6f72 7562 6122 290d 0a20  end("Yoruba").. 
-00009260: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
-00009270: 5f6e 616d 6573 2e61 7070 656e 6428 225a  _names.append("Z
-00009280: 756c 7522 290d 0a0d 0a20 2020 2020 2020  ulu")....       
-00009290: 2073 656c 662e 636f 6465 5f6f 665f 6e61   self.code_of_na
-000092a0: 6d65 203d 2064 6963 7428 7a69 7028 7365  me = dict(zip(se
-000092b0: 6c66 2e6c 6973 745f 6e61 6d65 732c 2073  lf.list_names, s
-000092c0: 656c 662e 6c69 7374 5f63 6f64 6573 2929  elf.list_codes))
-000092d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
-000092e0: 616d 655f 6f66 5f63 6f64 6520 3d20 6469  ame_of_code = di
-000092f0: 6374 287a 6970 2873 656c 662e 6c69 7374  ct(zip(self.list
-00009300: 5f63 6f64 6573 2c20 7365 6c66 2e6c 6973  _codes, self.lis
-00009310: 745f 6e61 6d65 7329 290d 0a0d 0a20 2020  t_names))....   
-00009320: 2020 2020 2073 656c 662e 6469 6374 203d       self.dict =
-00009330: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00009340: 2020 2020 2020 2020 2020 2020 2761 6627              'af'
-00009350: 3a20 2741 6672 696b 6161 6e73 272c 0d0a  : 'Afrikaans',..
-00009360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009370: 2020 2020 2020 2020 2773 7127 3a20 2741          'sq': 'A
-00009380: 6c62 616e 6961 6e27 2c0d 0a20 2020 2020  lbanian',..     
-00009390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093a0: 2020 2027 616d 273a 2027 416d 6861 7269     'am': 'Amhari
-000093b0: 6327 2c0d 0a20 2020 2020 2020 2020 2020  c',..           
-000093c0: 2020 2020 2020 2020 2020 2020 2027 6172               'ar
-000093d0: 273a 2027 4172 6162 6963 272c 0d0a 2020  ': 'Arabic',..  
-000093e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093f0: 2020 2020 2020 2768 7927 3a20 2741 726d        'hy': 'Arm
-00009400: 656e 6961 6e27 2c0d 0a20 2020 2020 2020  enian',..       
-00009410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009420: 2027 6173 273a 2027 4173 7361 6d65 7365   'as': 'Assamese
-00009430: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00009440: 2020 2020 2020 2020 2020 2020 2761 7927              'ay'
-00009450: 3a20 2741 796d 6172 6127 2c0d 0a20 2020  : 'Aymara',..   
-00009460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009470: 2020 2020 2027 617a 273a 2027 417a 6572       'az': 'Azer
-00009480: 6261 696a 616e 6927 2c0d 0a20 2020 2020  baijani',..     
-00009490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094a0: 2020 2027 626d 273a 2027 4261 6d62 6172     'bm': 'Bambar
-000094b0: 6127 2c0d 0a20 2020 2020 2020 2020 2020  a',..           
-000094c0: 2020 2020 2020 2020 2020 2020 2027 6575               'eu
-000094d0: 273a 2027 4261 7371 7565 272c 0d0a 2020  ': 'Basque',..  
-000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094f0: 2020 2020 2020 2762 6527 3a20 2742 656c        'be': 'Bel
-00009500: 6172 7573 6961 6e27 2c0d 0a20 2020 2020  arusian',..     
-00009510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009520: 2020 2027 626e 273a 2027 4265 6e67 616c     'bn': 'Bengal
-00009530: 6927 2c0d 0a20 2020 2020 2020 2020 2020  i',..           
-00009540: 2020 2020 2020 2020 2020 2020 2027 6268               'bh
-00009550: 6f27 3a20 2742 686f 6a70 7572 6927 2c0d  o': 'Bhojpuri',.
-00009560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009570: 2020 2020 2020 2020 2027 6273 273a 2027           'bs': '
-00009580: 426f 736e 6961 6e27 2c0d 0a20 2020 2020  Bosnian',..     
-00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095a0: 2020 2027 6267 273a 2027 4275 6c67 6172     'bg': 'Bulgar
-000095b0: 6961 6e27 2c0d 0a20 2020 2020 2020 2020  ian',..         
-000095c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000095d0: 6361 273a 2027 4361 7461 6c61 6e27 2c0d  ca': 'Catalan',.
-000095e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000095f0: 2020 2020 2020 2020 2027 6365 6227 3a20           'ceb': 
-00009600: 2743 6562 7561 6e6f 272c 0d0a 2020 2020  'Cebuano',..    
+00007bb0: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00007bc0: 6428 2241 7373 616d 6573 6522 290d 0a20  d("Assamese").. 
+00007bd0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00007be0: 5f6e 616d 6573 2e61 7070 656e 6428 2241  _names.append("A
+00007bf0: 796d 6172 6122 290d 0a20 2020 2020 2020  ymara")..       
+00007c00: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00007c10: 2e61 7070 656e 6428 2241 7a65 7262 6169  .append("Azerbai
+00007c20: 6a61 6e69 2229 0d0a 2020 2020 2020 2020  jani")..        
+00007c30: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00007c40: 6170 7065 6e64 2822 4261 6d62 6172 6122  append("Bambara"
+00007c50: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007c60: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00007c70: 6428 2242 6173 7175 6522 290d 0a20 2020  d("Basque")..   
+00007c80: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00007c90: 616d 6573 2e61 7070 656e 6428 2242 656c  ames.append("Bel
+00007ca0: 6172 7573 6961 6e22 290d 0a20 2020 2020  arusian")..     
+00007cb0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00007cc0: 6573 2e61 7070 656e 6428 2242 656e 6761  es.append("Benga
+00007cd0: 6c69 2229 0d0a 2020 2020 2020 2020 7365  li")..        se
+00007ce0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00007cf0: 7065 6e64 2822 4268 6f6a 7075 7269 2229  pend("Bhojpuri")
+00007d00: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00007d10: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00007d20: 2822 426f 736e 6961 6e22 290d 0a20 2020  ("Bosnian")..   
+00007d30: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00007d40: 616d 6573 2e61 7070 656e 6428 2242 756c  ames.append("Bul
+00007d50: 6761 7269 616e 2229 0d0a 2020 2020 2020  garian")..      
+00007d60: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00007d70: 732e 6170 7065 6e64 2822 4361 7461 6c61  s.append("Catala
+00007d80: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00007d90: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00007da0: 656e 6428 2243 6562 7561 6e6f 2229 0d0a  end("Cebuano")..
+00007db0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007dc0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00007dd0: 4368 6963 6865 7761 2229 0d0a 2020 2020  Chichewa")..    
+00007de0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00007df0: 6d65 732e 6170 7065 6e64 2822 4368 696e  mes.append("Chin
+00007e00: 6573 6520 2853 696d 706c 6966 6965 6429  ese (Simplified)
+00007e10: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00007e20: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00007e30: 6e64 2822 4368 696e 6573 6520 2854 7261  nd("Chinese (Tra
+00007e40: 6469 7469 6f6e 616c 2922 290d 0a20 2020  ditional)")..   
+00007e50: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00007e60: 616d 6573 2e61 7070 656e 6428 2243 6f72  ames.append("Cor
+00007e70: 7369 6361 6e22 290d 0a20 2020 2020 2020  sican")..       
+00007e80: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00007e90: 2e61 7070 656e 6428 2243 726f 6174 6961  .append("Croatia
+00007ea0: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00007eb0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00007ec0: 656e 6428 2243 7a65 6368 2229 0d0a 2020  end("Czech")..  
+00007ed0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00007ee0: 6e61 6d65 732e 6170 7065 6e64 2822 4461  names.append("Da
+00007ef0: 6e69 7368 2229 0d0a 2020 2020 2020 2020  nish")..        
+00007f00: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00007f10: 6170 7065 6e64 2822 4468 6976 6568 6922  append("Dhivehi"
+00007f20: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007f30: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00007f40: 6428 2244 6f67 7269 2229 0d0a 2020 2020  d("Dogri")..    
+00007f50: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00007f60: 6d65 732e 6170 7065 6e64 2822 4475 7463  mes.append("Dutc
+00007f70: 6822 290d 0a20 2020 2020 2020 2073 656c  h")..        sel
+00007f80: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00007f90: 656e 6428 2245 6e67 6c69 7368 2229 0d0a  end("English")..
+00007fa0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00007fb0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00007fc0: 4573 7065 7261 6e74 6f22 290d 0a20 2020  Esperanto")..   
+00007fd0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00007fe0: 616d 6573 2e61 7070 656e 6428 2245 7374  ames.append("Est
+00007ff0: 6f6e 6961 6e22 290d 0a20 2020 2020 2020  onian")..       
+00008000: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00008010: 2e61 7070 656e 6428 2245 7765 2229 0d0a  .append("Ewe")..
+00008020: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00008030: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00008040: 4669 6c69 7069 6e6f 2229 0d0a 2020 2020  Filipino")..    
+00008050: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008060: 6d65 732e 6170 7065 6e64 2822 4669 6e6e  mes.append("Finn
+00008070: 6973 6822 290d 0a20 2020 2020 2020 2073  ish")..        s
+00008080: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008090: 7070 656e 6428 2246 7265 6e63 6822 290d  ppend("French").
+000080a0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000080b0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+000080c0: 2246 7269 7369 616e 2229 0d0a 2020 2020  "Frisian")..    
+000080d0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+000080e0: 6d65 732e 6170 7065 6e64 2822 4761 6c69  mes.append("Gali
+000080f0: 6369 616e 2229 0d0a 2020 2020 2020 2020  cian")..        
+00008100: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008110: 6170 7065 6e64 2822 4765 6f72 6769 616e  append("Georgian
+00008120: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008130: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00008140: 6e64 2822 4765 726d 616e 2229 0d0a 2020  nd("German")..  
+00008150: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008160: 6e61 6d65 732e 6170 7065 6e64 2822 4772  names.append("Gr
+00008170: 6565 6b22 290d 0a20 2020 2020 2020 2073  eek")..        s
+00008180: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008190: 7070 656e 6428 2247 7561 7261 6e69 2229  ppend("Guarani")
+000081a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+000081b0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+000081c0: 2822 4775 6a61 7261 7469 2229 0d0a 2020  ("Gujarati")..  
+000081d0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000081e0: 6e61 6d65 732e 6170 7065 6e64 2822 4861  names.append("Ha
+000081f0: 6974 6961 6e20 4372 656f 6c65 2229 0d0a  itian Creole")..
+00008200: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00008210: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00008220: 4861 7573 6122 290d 0a20 2020 2020 2020  Hausa")..       
+00008230: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00008240: 2e61 7070 656e 6428 2248 6177 6169 6961  .append("Hawaiia
+00008250: 6e22 290d 0a20 2020 2020 2020 2073 656c  n")..        sel
+00008260: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00008270: 656e 6428 2248 6562 7265 7722 290d 0a20  end("Hebrew").. 
+00008280: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00008290: 5f6e 616d 6573 2e61 7070 656e 6428 2248  _names.append("H
+000082a0: 696e 6469 2229 0d0a 2020 2020 2020 2020  indi")..        
+000082b0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+000082c0: 6170 7065 6e64 2822 486d 6f6e 6722 290d  append("Hmong").
+000082d0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000082e0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+000082f0: 2248 756e 6761 7269 616e 2229 0d0a 2020  "Hungarian")..  
+00008300: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008310: 6e61 6d65 732e 6170 7065 6e64 2822 4963  names.append("Ic
+00008320: 656c 616e 6469 6322 290d 0a20 2020 2020  elandic")..     
+00008330: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00008340: 6573 2e61 7070 656e 6428 2249 6762 6f22  es.append("Igbo"
+00008350: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008360: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008370: 6428 2249 6c6f 6361 6e6f 2229 0d0a 2020  d("Ilocano")..  
+00008380: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008390: 6e61 6d65 732e 6170 7065 6e64 2822 496e  names.append("In
+000083a0: 646f 6e65 7369 616e 2229 0d0a 2020 2020  donesian")..    
+000083b0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+000083c0: 6d65 732e 6170 7065 6e64 2822 4972 6973  mes.append("Iris
+000083d0: 6822 290d 0a20 2020 2020 2020 2073 656c  h")..        sel
+000083e0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+000083f0: 656e 6428 2249 7461 6c69 616e 2229 0d0a  end("Italian")..
+00008400: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00008410: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00008420: 4a61 7061 6e65 7365 2229 0d0a 2020 2020  Japanese")..    
+00008430: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008440: 6d65 732e 6170 7065 6e64 2822 4a61 7661  mes.append("Java
+00008450: 6e65 7365 2229 0d0a 2020 2020 2020 2020  nese")..        
+00008460: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008470: 6170 7065 6e64 2822 4b61 6e6e 6164 6122  append("Kannada"
+00008480: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008490: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+000084a0: 6428 224b 617a 616b 6822 290d 0a20 2020  d("Kazakh")..   
+000084b0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+000084c0: 616d 6573 2e61 7070 656e 6428 224b 686d  ames.append("Khm
+000084d0: 6572 2229 0d0a 2020 2020 2020 2020 7365  er")..        se
+000084e0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+000084f0: 7065 6e64 2822 4b69 6e79 6172 7761 6e64  pend("Kinyarwand
+00008500: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
+00008510: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00008520: 656e 6428 224b 6f6e 6b61 6e69 2229 0d0a  end("Konkani")..
+00008530: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00008540: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00008550: 4b6f 7265 616e 2229 0d0a 2020 2020 2020  Korean")..      
+00008560: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00008570: 732e 6170 7065 6e64 2822 4b72 696f 2229  s.append("Krio")
+00008580: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008590: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+000085a0: 2822 4b75 7264 6973 6820 284b 7572 6d61  ("Kurdish (Kurma
+000085b0: 6e6a 6929 2229 0d0a 2020 2020 2020 2020  nji)")..        
+000085c0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+000085d0: 6170 7065 6e64 2822 4b75 7264 6973 6820  append("Kurdish 
+000085e0: 2853 6f72 616e 6929 2229 0d0a 2020 2020  (Sorani)")..    
+000085f0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008600: 6d65 732e 6170 7065 6e64 2822 4b79 7267  mes.append("Kyrg
+00008610: 797a 2229 0d0a 2020 2020 2020 2020 7365  yz")..        se
+00008620: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008630: 7065 6e64 2822 4c61 6f22 290d 0a20 2020  pend("Lao")..   
+00008640: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00008650: 616d 6573 2e61 7070 656e 6428 224c 6174  ames.append("Lat
+00008660: 696e 2229 0d0a 2020 2020 2020 2020 7365  in")..        se
+00008670: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008680: 7065 6e64 2822 4c61 7476 6961 6e22 290d  pend("Latvian").
+00008690: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000086a0: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+000086b0: 224c 696e 6761 6c61 2229 0d0a 2020 2020  "Lingala")..    
+000086c0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+000086d0: 6d65 732e 6170 7065 6e64 2822 4c69 7468  mes.append("Lith
+000086e0: 7561 6e69 616e 2229 0d0a 2020 2020 2020  uanian")..      
+000086f0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00008700: 732e 6170 7065 6e64 2822 4c75 6761 6e64  s.append("Lugand
+00008710: 6122 290d 0a20 2020 2020 2020 2073 656c  a")..        sel
+00008720: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00008730: 656e 6428 224c 7578 656d 626f 7572 6769  end("Luxembourgi
+00008740: 7368 2229 0d0a 2020 2020 2020 2020 7365  sh")..        se
+00008750: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008760: 7065 6e64 2822 4d61 6365 646f 6e69 616e  pend("Macedonian
+00008770: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00008780: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00008790: 6e64 2822 4d61 6c61 6761 7379 2229 0d0a  nd("Malagasy")..
+000087a0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+000087b0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+000087c0: 4d61 6c61 7922 290d 0a20 2020 2020 2020  Malay")..       
+000087d0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+000087e0: 2e61 7070 656e 6428 224d 616c 6179 616c  .append("Malayal
+000087f0: 616d 2229 0d0a 2020 2020 2020 2020 7365  am")..        se
+00008800: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008810: 7065 6e64 2822 4d61 6c74 6573 6522 290d  pend("Maltese").
+00008820: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00008830: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00008840: 224d 616f 7269 2229 0d0a 2020 2020 2020  "Maori")..      
+00008850: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00008860: 732e 6170 7065 6e64 2822 4d61 7261 7468  s.append("Marath
+00008870: 6922 290d 0a20 2020 2020 2020 2073 656c  i")..        sel
+00008880: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00008890: 656e 6428 224d 6569 7465 696c 6f6e 2028  end("Meiteilon (
+000088a0: 4d61 6e69 7075 7269 2922 290d 0a20 2020  Manipuri)")..   
+000088b0: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+000088c0: 616d 6573 2e61 7070 656e 6428 224d 697a  ames.append("Miz
+000088d0: 6f22 290d 0a20 2020 2020 2020 2073 656c  o")..        sel
+000088e0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+000088f0: 656e 6428 224d 6f6e 676f 6c69 616e 2229  end("Mongolian")
+00008900: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008910: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008920: 2822 4d79 616e 6d61 7220 2842 7572 6d65  ("Myanmar (Burme
+00008930: 7365 2922 290d 0a20 2020 2020 2020 2073  se)")..        s
+00008940: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008950: 7070 656e 6428 224e 6570 616c 6922 290d  ppend("Nepali").
+00008960: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00008970: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00008980: 224e 6f72 7765 6769 616e 2229 0d0a 2020  "Norwegian")..  
+00008990: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+000089a0: 6e61 6d65 732e 6170 7065 6e64 2822 4f64  names.append("Od
+000089b0: 6979 6120 284f 7269 7961 2922 290d 0a20  iya (Oriya)").. 
+000089c0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+000089d0: 5f6e 616d 6573 2e61 7070 656e 6428 224f  _names.append("O
+000089e0: 726f 6d6f 2229 0d0a 2020 2020 2020 2020  romo")..        
+000089f0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008a00: 6170 7065 6e64 2822 5061 7368 746f 2229  append("Pashto")
+00008a10: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008a20: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008a30: 2822 5065 7273 6961 6e22 290d 0a20 2020  ("Persian")..   
+00008a40: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00008a50: 616d 6573 2e61 7070 656e 6428 2250 6f6c  ames.append("Pol
+00008a60: 6973 6822 290d 0a20 2020 2020 2020 2073  ish")..        s
+00008a70: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008a80: 7070 656e 6428 2250 6f72 7475 6775 6573  ppend("Portugues
+00008a90: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
+00008aa0: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00008ab0: 656e 6428 2250 756e 6a61 6269 2229 0d0a  end("Punjabi")..
+00008ac0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00008ad0: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00008ae0: 5175 6563 6875 6122 290d 0a20 2020 2020  Quechua")..     
+00008af0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00008b00: 6573 2e61 7070 656e 6428 2252 6f6d 616e  es.append("Roman
+00008b10: 6961 6e22 290d 0a20 2020 2020 2020 2073  ian")..        s
+00008b20: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008b30: 7070 656e 6428 2252 7573 7369 616e 2229  ppend("Russian")
+00008b40: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008b50: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008b60: 2822 5361 6d6f 616e 2229 0d0a 2020 2020  ("Samoan")..    
+00008b70: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008b80: 6d65 732e 6170 7065 6e64 2822 5361 6e73  mes.append("Sans
+00008b90: 6b72 6974 2229 0d0a 2020 2020 2020 2020  krit")..        
+00008ba0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008bb0: 6170 7065 6e64 2822 5363 6f74 7320 4761  append("Scots Ga
+00008bc0: 656c 6963 2229 0d0a 2020 2020 2020 2020  elic")..        
+00008bd0: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008be0: 6170 7065 6e64 2822 5365 7065 6469 2229  append("Sepedi")
+00008bf0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008c00: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008c10: 2822 5365 7262 6961 6e22 290d 0a20 2020  ("Serbian")..   
+00008c20: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00008c30: 616d 6573 2e61 7070 656e 6428 2253 6573  ames.append("Ses
+00008c40: 6f74 686f 2229 0d0a 2020 2020 2020 2020  otho")..        
+00008c50: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008c60: 6170 7065 6e64 2822 5368 6f6e 6122 290d  append("Shona").
+00008c70: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00008c80: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00008c90: 2253 696e 6468 6922 290d 0a20 2020 2020  "Sindhi")..     
+00008ca0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00008cb0: 6573 2e61 7070 656e 6428 2253 696e 6861  es.append("Sinha
+00008cc0: 6c61 2229 0d0a 2020 2020 2020 2020 7365  la")..        se
+00008cd0: 6c66 2e6c 6973 745f 6e61 6d65 732e 6170  lf.list_names.ap
+00008ce0: 7065 6e64 2822 536c 6f76 616b 2229 0d0a  pend("Slovak")..
+00008cf0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00008d00: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00008d10: 536c 6f76 656e 6961 6e22 290d 0a20 2020  Slovenian")..   
+00008d20: 2020 2020 2073 656c 662e 6c69 7374 5f6e       self.list_n
+00008d30: 616d 6573 2e61 7070 656e 6428 2253 6f6d  ames.append("Som
+00008d40: 616c 6922 290d 0a20 2020 2020 2020 2073  ali")..        s
+00008d50: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008d60: 7070 656e 6428 2253 7061 6e69 7368 2229  ppend("Spanish")
+00008d70: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008d80: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008d90: 2822 5375 6e64 616e 6573 6522 290d 0a20  ("Sundanese").. 
+00008da0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00008db0: 5f6e 616d 6573 2e61 7070 656e 6428 2253  _names.append("S
+00008dc0: 7761 6869 6c69 2229 0d0a 2020 2020 2020  wahili")..      
+00008dd0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00008de0: 732e 6170 7065 6e64 2822 5377 6564 6973  s.append("Swedis
+00008df0: 6822 290d 0a20 2020 2020 2020 2073 656c  h")..        sel
+00008e00: 662e 6c69 7374 5f6e 616d 6573 2e61 7070  f.list_names.app
+00008e10: 656e 6428 2254 616a 696b 2229 0d0a 2020  end("Tajik")..  
+00008e20: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008e30: 6e61 6d65 732e 6170 7065 6e64 2822 5461  names.append("Ta
+00008e40: 6d69 6c22 290d 0a20 2020 2020 2020 2073  mil")..        s
+00008e50: 656c 662e 6c69 7374 5f6e 616d 6573 2e61  elf.list_names.a
+00008e60: 7070 656e 6428 2254 6174 6172 2229 0d0a  ppend("Tatar")..
+00008e70: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+00008e80: 745f 6e61 6d65 732e 6170 7065 6e64 2822  t_names.append("
+00008e90: 5465 6c75 6775 2229 0d0a 2020 2020 2020  Telugu")..      
+00008ea0: 2020 7365 6c66 2e6c 6973 745f 6e61 6d65    self.list_name
+00008eb0: 732e 6170 7065 6e64 2822 5468 6169 2229  s.append("Thai")
+00008ec0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00008ed0: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00008ee0: 2822 5469 6772 696e 7961 2229 0d0a 2020  ("Tigrinya")..  
+00008ef0: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008f00: 6e61 6d65 732e 6170 7065 6e64 2822 5473  names.append("Ts
+00008f10: 6f6e 6761 2229 0d0a 2020 2020 2020 2020  onga")..        
+00008f20: 7365 6c66 2e6c 6973 745f 6e61 6d65 732e  self.list_names.
+00008f30: 6170 7065 6e64 2822 5475 726b 6973 6822  append("Turkish"
+00008f40: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008f50: 6c69 7374 5f6e 616d 6573 2e61 7070 656e  list_names.appen
+00008f60: 6428 2254 7572 6b6d 656e 2229 0d0a 2020  d("Turkmen")..  
+00008f70: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
+00008f80: 6e61 6d65 732e 6170 7065 6e64 2822 5477  names.append("Tw
+00008f90: 6920 2841 6b61 6e29 2229 0d0a 2020 2020  i (Akan)")..    
+00008fa0: 2020 2020 7365 6c66 2e6c 6973 745f 6e61      self.list_na
+00008fb0: 6d65 732e 6170 7065 6e64 2822 556b 7261  mes.append("Ukra
+00008fc0: 696e 6961 6e22 290d 0a20 2020 2020 2020  inian")..       
+00008fd0: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00008fe0: 2e61 7070 656e 6428 2255 7264 7522 290d  .append("Urdu").
+00008ff0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+00009000: 7374 5f6e 616d 6573 2e61 7070 656e 6428  st_names.append(
+00009010: 2255 7967 6875 7222 290d 0a20 2020 2020  "Uyghur")..     
+00009020: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+00009030: 6573 2e61 7070 656e 6428 2255 7a62 656b  es.append("Uzbek
+00009040: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00009050: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+00009060: 6e64 2822 5669 6574 6e61 6d65 7365 2229  nd("Vietnamese")
+00009070: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00009080: 6973 745f 6e61 6d65 732e 6170 7065 6e64  ist_names.append
+00009090: 2822 5765 6c73 6822 290d 0a20 2020 2020  ("Welsh")..     
+000090a0: 2020 2073 656c 662e 6c69 7374 5f6e 616d     self.list_nam
+000090b0: 6573 2e61 7070 656e 6428 2258 686f 7361  es.append("Xhosa
+000090c0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000090d0: 2e6c 6973 745f 6e61 6d65 732e 6170 7065  .list_names.appe
+000090e0: 6e64 2822 5969 6464 6973 6822 290d 0a20  nd("Yiddish").. 
+000090f0: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00009100: 5f6e 616d 6573 2e61 7070 656e 6428 2259  _names.append("Y
+00009110: 6f72 7562 6122 290d 0a20 2020 2020 2020  oruba")..       
+00009120: 2073 656c 662e 6c69 7374 5f6e 616d 6573   self.list_names
+00009130: 2e61 7070 656e 6428 225a 756c 7522 290d  .append("Zulu").
+00009140: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+00009150: 636f 6465 5f6f 665f 6e61 6d65 203d 2064  code_of_name = d
+00009160: 6963 7428 7a69 7028 7365 6c66 2e6c 6973  ict(zip(self.lis
+00009170: 745f 6e61 6d65 732c 2073 656c 662e 6c69  t_names, self.li
+00009180: 7374 5f63 6f64 6573 2929 0d0a 2020 2020  st_codes))..    
+00009190: 2020 2020 7365 6c66 2e6e 616d 655f 6f66      self.name_of
+000091a0: 5f63 6f64 6520 3d20 6469 6374 287a 6970  _code = dict(zip
+000091b0: 2873 656c 662e 6c69 7374 5f63 6f64 6573  (self.list_codes
+000091c0: 2c20 7365 6c66 2e6c 6973 745f 6e61 6d65  , self.list_name
+000091d0: 7329 290d 0a0d 0a20 2020 2020 2020 2073  s))....        s
+000091e0: 656c 662e 6469 6374 203d 207b 0d0a 2020  elf.dict = {..  
+000091f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009200: 2020 2020 2020 2761 6627 3a20 2741 6672        'af': 'Afr
+00009210: 696b 6161 6e73 272c 0d0a 2020 2020 2020  ikaans',..      
+00009220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009230: 2020 2773 7127 3a20 2741 6c62 616e 6961    'sq': 'Albania
+00009240: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+00009250: 2020 2020 2020 2020 2020 2020 2027 616d               'am
+00009260: 273a 2027 416d 6861 7269 6327 2c0d 0a20  ': 'Amharic',.. 
+00009270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009280: 2020 2020 2020 2027 6172 273a 2027 4172         'ar': 'Ar
+00009290: 6162 6963 272c 0d0a 2020 2020 2020 2020  abic',..        
+000092a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092b0: 2768 7927 3a20 2741 726d 656e 6961 6e27  'hy': 'Armenian'
+000092c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000092d0: 2020 2020 2020 2020 2020 2027 6173 273a             'as':
+000092e0: 2027 4173 7361 6d65 7365 272c 0d0a 2020   'Assamese',..  
+000092f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009300: 2020 2020 2020 2761 7927 3a20 2741 796d        'ay': 'Aym
+00009310: 6172 6127 2c0d 0a20 2020 2020 2020 2020  ara',..         
+00009320: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009330: 617a 273a 2027 417a 6572 6261 696a 616e  az': 'Azerbaijan
+00009340: 6927 2c0d 0a20 2020 2020 2020 2020 2020  i',..           
+00009350: 2020 2020 2020 2020 2020 2020 2027 626d               'bm
+00009360: 273a 2027 4261 6d62 6172 6127 2c0d 0a20  ': 'Bambara',.. 
+00009370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009380: 2020 2020 2020 2027 6575 273a 2027 4261         'eu': 'Ba
+00009390: 7371 7565 272c 0d0a 2020 2020 2020 2020  sque',..        
+000093a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093b0: 2762 6527 3a20 2742 656c 6172 7573 6961  'be': 'Belarusia
+000093c0: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+000093d0: 2020 2020 2020 2020 2020 2020 2027 626e               'bn
+000093e0: 273a 2027 4265 6e67 616c 6927 2c0d 0a20  ': 'Bengali',.. 
+000093f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009400: 2020 2020 2020 2027 6268 6f27 3a20 2742         'bho': 'B
+00009410: 686f 6a70 7572 6927 2c0d 0a20 2020 2020  hojpuri',..     
+00009420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009430: 2020 2027 6273 273a 2027 426f 736e 6961     'bs': 'Bosnia
+00009440: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+00009450: 2020 2020 2020 2020 2020 2020 2027 6267               'bg
+00009460: 273a 2027 4275 6c67 6172 6961 6e27 2c0d  ': 'Bulgarian',.
+00009470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009480: 2020 2020 2020 2020 2027 6361 273a 2027           'ca': '
+00009490: 4361 7461 6c61 6e27 2c0d 0a20 2020 2020  Catalan',..     
+000094a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094b0: 2020 2027 6365 6227 3a20 2743 6562 7561     'ceb': 'Cebua
+000094c0: 6e6f 272c 0d0a 2020 2020 2020 2020 2020  no',..          
+000094d0: 2020 2020 2020 2020 2020 2020 2020 276e                'n
+000094e0: 7927 3a20 2743 6869 6368 6577 6127 2c0d  y': 'Chichewa',.
+000094f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009500: 2020 2020 2020 2020 2027 7a68 2d43 4e27           'zh-CN'
+00009510: 3a20 2743 6869 6e65 7365 2028 5369 6d70  : 'Chinese (Simp
+00009520: 6c69 6669 6564 2927 2c0d 0a20 2020 2020  lified)',..     
+00009530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009540: 2020 2027 7a68 2d54 5727 3a20 2743 6869     'zh-TW': 'Chi
+00009550: 6e65 7365 2028 5472 6164 6974 696f 6e61  nese (Traditiona
+00009560: 6c29 272c 0d0a 2020 2020 2020 2020 2020  l)',..          
+00009570: 2020 2020 2020 2020 2020 2020 2020 2763                'c
+00009580: 6f27 3a20 2743 6f72 7369 6361 6e27 2c0d  o': 'Corsican',.
+00009590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000095a0: 2020 2020 2020 2020 2027 6872 273a 2027           'hr': '
+000095b0: 4372 6f61 7469 616e 272c 0d0a 2020 2020  Croatian',..    
+000095c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095d0: 2020 2020 2763 7327 3a20 2743 7a65 6368      'cs': 'Czech
+000095e0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+000095f0: 2020 2020 2020 2020 2020 2020 2764 6127              'da'
+00009600: 3a20 2744 616e 6973 6827 2c0d 0a20 2020  : 'Danish',..   
 00009610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009620: 2020 2020 276e 7927 3a20 2743 6869 6368      'ny': 'Chich
-00009630: 6577 6127 2c0d 0a20 2020 2020 2020 2020  ewa',..         
+00009620: 2020 2020 2027 6476 273a 2027 4468 6976       'dv': 'Dhiv
+00009630: 6568 6927 2c0d 0a20 2020 2020 2020 2020  ehi',..         
 00009640: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00009650: 7a68 2d43 4e27 3a20 2743 6869 6e65 7365  zh-CN': 'Chinese
-00009660: 2028 5369 6d70 6c69 6669 6564 2927 2c0d   (Simplified)',.
-00009670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009680: 2020 2020 2020 2020 2027 7a68 2d54 5727           'zh-TW'
-00009690: 3a20 2743 6869 6e65 7365 2028 5472 6164  : 'Chinese (Trad
-000096a0: 6974 696f 6e61 6c29 272c 0d0a 2020 2020  itional)',..    
-000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096c0: 2020 2020 2763 6f27 3a20 2743 6f72 7369      'co': 'Corsi
-000096d0: 6361 6e27 2c0d 0a20 2020 2020 2020 2020  can',..         
-000096e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000096f0: 6872 273a 2027 4372 6f61 7469 616e 272c  hr': 'Croatian',
-00009700: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009710: 2020 2020 2020 2020 2020 2763 7327 3a20            'cs': 
-00009720: 2743 7a65 6368 272c 0d0a 2020 2020 2020  'Czech',..      
+00009650: 646f 6927 3a20 2744 6f67 7269 272c 0d0a  doi': 'Dogri',..
+00009660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009670: 2020 2020 2020 2020 276e 6c27 3a20 2744          'nl': 'D
+00009680: 7574 6368 272c 0d0a 2020 2020 2020 2020  utch',..        
+00009690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096a0: 2765 6e27 3a20 2745 6e67 6c69 7368 272c  'en': 'English',
+000096b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000096c0: 2020 2020 2020 2020 2020 2765 6f27 3a20            'eo': 
+000096d0: 2745 7370 6572 616e 746f 272c 0d0a 2020  'Esperanto',..  
+000096e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096f0: 2020 2020 2020 2765 7427 3a20 2745 7374        'et': 'Est
+00009700: 6f6e 6961 6e27 2c0d 0a20 2020 2020 2020  onian',..       
+00009710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009720: 2027 6565 273a 2027 4577 6527 2c0d 0a20   'ee': 'Ewe',.. 
 00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009740: 2020 2764 6127 3a20 2744 616e 6973 6827    'da': 'Danish'
-00009750: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00009760: 2020 2020 2020 2020 2020 2027 6476 273a             'dv':
-00009770: 2027 4468 6976 6568 6927 2c0d 0a20 2020   'Dhivehi',..   
-00009780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009790: 2020 2020 2027 646f 6927 3a20 2744 6f67       'doi': 'Dog
-000097a0: 7269 272c 0d0a 2020 2020 2020 2020 2020  ri',..          
-000097b0: 2020 2020 2020 2020 2020 2020 2020 276e                'n
-000097c0: 6c27 3a20 2744 7574 6368 272c 0d0a 2020  l': 'Dutch',..  
-000097d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097e0: 2020 2020 2020 2765 6e27 3a20 2745 6e67        'en': 'Eng
-000097f0: 6c69 7368 272c 0d0a 2020 2020 2020 2020  lish',..        
-00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009810: 2765 6f27 3a20 2745 7370 6572 616e 746f  'eo': 'Esperanto
-00009820: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00009830: 2020 2020 2020 2020 2020 2020 2765 7427              'et'
-00009840: 3a20 2745 7374 6f6e 6961 6e27 2c0d 0a20  : 'Estonian',.. 
-00009850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009860: 2020 2020 2020 2027 6565 273a 2027 4577         'ee': 'Ew
-00009870: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
-00009880: 2020 2020 2020 2020 2020 2020 2027 6669               'fi
-00009890: 6c27 3a20 2746 696c 6970 696e 6f27 2c0d  l': 'Filipino',.
-000098a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000098b0: 2020 2020 2020 2020 2027 6669 273a 2027           'fi': '
-000098c0: 4669 6e6e 6973 6827 2c0d 0a20 2020 2020  Finnish',..     
-000098d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098e0: 2020 2027 6672 273a 2027 4672 656e 6368     'fr': 'French
-000098f0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00009900: 2020 2020 2020 2020 2020 2020 2766 7927              'fy'
-00009910: 3a20 2746 7269 7369 616e 272c 0d0a 2020  : 'Frisian',..  
-00009920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009930: 2020 2020 2020 2767 6c27 3a20 2747 616c        'gl': 'Gal
-00009940: 6963 6961 6e27 2c0d 0a20 2020 2020 2020  ician',..       
-00009950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009960: 2027 6b61 273a 2027 4765 6f72 6769 616e   'ka': 'Georgian
-00009970: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00009980: 2020 2020 2020 2020 2020 2020 2764 6527              'de'
-00009990: 3a20 2747 6572 6d61 6e27 2c0d 0a20 2020  : 'German',..   
-000099a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099b0: 2020 2020 2027 656c 273a 2027 4772 6565       'el': 'Gree
-000099c0: 6b27 2c0d 0a20 2020 2020 2020 2020 2020  k',..           
-000099d0: 2020 2020 2020 2020 2020 2020 2027 676e               'gn
-000099e0: 273a 2027 4775 6172 616e 6927 2c0d 0a20  ': 'Guarani',.. 
-000099f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a00: 2020 2020 2020 2027 6775 273a 2027 4775         'gu': 'Gu
-00009a10: 6a61 7261 7469 272c 0d0a 2020 2020 2020  jarati',..      
-00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a30: 2020 2768 7427 3a20 2748 6169 7469 616e    'ht': 'Haitian
-00009a40: 2043 7265 6f6c 6527 2c0d 0a20 2020 2020   Creole',..     
-00009a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a60: 2020 2027 6861 273a 2027 4861 7573 6127     'ha': 'Hausa'
-00009a70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00009a80: 2020 2020 2020 2020 2020 2027 6861 7727             'haw'
-00009a90: 3a20 2748 6177 6169 6961 6e27 2c0d 0a20  : 'Hawaiian',.. 
-00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ab0: 2020 2020 2020 2027 6865 273a 2027 4865         'he': 'He
-00009ac0: 6272 6577 272c 0d0a 2020 2020 2020 2020  brew',..        
-00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ae0: 2768 6927 3a20 2748 696e 6469 272c 0d0a  'hi': 'Hindi',..
-00009af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b00: 2020 2020 2020 2020 2768 6d6e 273a 2027          'hmn': '
-00009b10: 486d 6f6e 6727 2c0d 0a20 2020 2020 2020  Hmong',..       
-00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b30: 2027 6875 273a 2027 4875 6e67 6172 6961   'hu': 'Hungaria
-00009b40: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
-00009b50: 2020 2020 2020 2020 2020 2020 2027 6973               'is
-00009b60: 273a 2027 4963 656c 616e 6469 6327 2c0d  ': 'Icelandic',.
-00009b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009b80: 2020 2020 2020 2020 2027 6967 273a 2027           'ig': '
-00009b90: 4967 626f 272c 0d0a 2020 2020 2020 2020  Igbo',..        
-00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bb0: 2769 6c6f 273a 2027 496c 6f63 616e 6f27  'ilo': 'Ilocano'
-00009bc0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00009bd0: 2020 2020 2020 2020 2020 2027 6964 273a             'id':
-00009be0: 2027 496e 646f 6e65 7369 616e 272c 0d0a   'Indonesian',..
-00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c00: 2020 2020 2020 2020 2767 6127 3a20 2749          'ga': 'I
-00009c10: 7269 7368 272c 0d0a 2020 2020 2020 2020  rish',..        
-00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c30: 2769 7427 3a20 2749 7461 6c69 616e 272c  'it': 'Italian',
-00009c40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009c50: 2020 2020 2020 2020 2020 276a 6127 3a20            'ja': 
-00009c60: 274a 6170 616e 6573 6527 2c0d 0a20 2020  'Japanese',..   
-00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c80: 2020 2020 2027 6a76 273a 2027 4a61 7661       'jv': 'Java
-00009c90: 6e65 7365 272c 0d0a 2020 2020 2020 2020  nese',..        
-00009ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cb0: 276b 6e27 3a20 274b 616e 6e61 6461 272c  'kn': 'Kannada',
-00009cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009cd0: 2020 2020 2020 2020 2020 276b 6b27 3a20            'kk': 
-00009ce0: 274b 617a 616b 6827 2c0d 0a20 2020 2020  'Kazakh',..     
-00009cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d00: 2020 2027 6b6d 273a 2027 4b68 6d65 7227     'km': 'Khmer'
-00009d10: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00009d20: 2020 2020 2020 2020 2020 2027 7277 273a             'rw':
-00009d30: 2027 4b69 6e79 6172 7761 6e64 6127 2c0d   'Kinyarwanda',.
-00009d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009d50: 2020 2020 2020 2020 2027 676f 6d27 3a20           'gom': 
-00009d60: 274b 6f6e 6b61 6e69 272c 0d0a 2020 2020  'Konkani',..    
-00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d80: 2020 2020 276b 6f27 3a20 274b 6f72 6561      'ko': 'Korea
-00009d90: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
-00009da0: 2020 2020 2020 2020 2020 2020 2027 6b72               'kr
-00009db0: 6927 3a20 274b 7269 6f27 2c0d 0a20 2020  i': 'Krio',..   
-00009dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dd0: 2020 2020 2027 6b6d 7227 3a20 274b 7572       'kmr': 'Kur
-00009de0: 6469 7368 2028 4b75 726d 616e 6a69 2927  dish (Kurmanji)'
-00009df0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00009e00: 2020 2020 2020 2020 2020 2027 636b 6227             'ckb'
-00009e10: 3a20 274b 7572 6469 7368 2028 536f 7261  : 'Kurdish (Sora
-00009e20: 6e69 2927 2c0d 0a20 2020 2020 2020 2020  ni)',..         
-00009e30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00009e40: 6b79 273a 2027 4b79 7267 797a 272c 0d0a  ky': 'Kyrgyz',..
-00009e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e60: 2020 2020 2020 2020 276c 6f27 3a20 274c          'lo': 'L
-00009e70: 616f 272c 0d0a 2020 2020 2020 2020 2020  ao',..          
-00009e80: 2020 2020 2020 2020 2020 2020 2020 276c                'l
-00009e90: 6127 3a20 274c 6174 696e 272c 0d0a 2020  a': 'Latin',..  
-00009ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009eb0: 2020 2020 2020 276c 7627 3a20 274c 6174        'lv': 'Lat
-00009ec0: 7669 616e 272c 0d0a 2020 2020 2020 2020  vian',..        
-00009ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ee0: 276c 6e27 3a20 274c 696e 6761 6c61 272c  'ln': 'Lingala',
-00009ef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009f00: 2020 2020 2020 2020 2020 276c 7427 3a20            'lt': 
-00009f10: 274c 6974 6875 616e 6961 6e27 2c0d 0a20  'Lithuanian',.. 
-00009f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f30: 2020 2020 2020 2027 6c67 273a 2027 4c75         'lg': 'Lu
-00009f40: 6761 6e64 6127 2c0d 0a20 2020 2020 2020  ganda',..       
-00009f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f60: 2027 6c62 273a 2027 4c75 7865 6d62 6f75   'lb': 'Luxembou
-00009f70: 7267 6973 6827 2c0d 0a20 2020 2020 2020  rgish',..       
-00009f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f90: 2027 6d6b 273a 2027 4d61 6365 646f 6e69   'mk': 'Macedoni
-00009fa0: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
-00009fb0: 2020 2020 2020 2020 2020 2020 2020 276d                'm
-00009fc0: 6727 3a20 274d 616c 6167 6173 7927 2c0d  g': 'Malagasy',.
-00009fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009fe0: 2020 2020 2020 2020 2027 6d73 273a 2027           'ms': '
-00009ff0: 4d61 6c61 7927 2c0d 0a20 2020 2020 2020  Malay',..       
-0000a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a010: 2027 6d6c 273a 2027 4d61 6c61 7961 6c61   'ml': 'Malayala
-0000a020: 6d27 2c0d 0a20 2020 2020 2020 2020 2020  m',..           
-0000a030: 2020 2020 2020 2020 2020 2020 2027 6d74               'mt
-0000a040: 273a 2027 4d61 6c74 6573 6527 2c0d 0a20  ': 'Maltese',.. 
+00009740: 2020 2020 2020 2027 6669 6c27 3a20 2746         'fil': 'F
+00009750: 696c 6970 696e 6f27 2c0d 0a20 2020 2020  ilipino',..     
+00009760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009770: 2020 2027 6669 273a 2027 4669 6e6e 6973     'fi': 'Finnis
+00009780: 6827 2c0d 0a20 2020 2020 2020 2020 2020  h',..           
+00009790: 2020 2020 2020 2020 2020 2020 2027 6672               'fr
+000097a0: 273a 2027 4672 656e 6368 272c 0d0a 2020  ': 'French',..  
+000097b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097c0: 2020 2020 2020 2766 7927 3a20 2746 7269        'fy': 'Fri
+000097d0: 7369 616e 272c 0d0a 2020 2020 2020 2020  sian',..        
+000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097f0: 2767 6c27 3a20 2747 616c 6963 6961 6e27  'gl': 'Galician'
+00009800: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009810: 2020 2020 2020 2020 2020 2027 6b61 273a             'ka':
+00009820: 2027 4765 6f72 6769 616e 272c 0d0a 2020   'Georgian',..  
+00009830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009840: 2020 2020 2020 2764 6527 3a20 2747 6572        'de': 'Ger
+00009850: 6d61 6e27 2c0d 0a20 2020 2020 2020 2020  man',..         
+00009860: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009870: 656c 273a 2027 4772 6565 6b27 2c0d 0a20  el': 'Greek',.. 
+00009880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009890: 2020 2020 2020 2027 676e 273a 2027 4775         'gn': 'Gu
+000098a0: 6172 616e 6927 2c0d 0a20 2020 2020 2020  arani',..       
+000098b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098c0: 2027 6775 273a 2027 4775 6a61 7261 7469   'gu': 'Gujarati
+000098d0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+000098e0: 2020 2020 2020 2020 2020 2020 2768 7427              'ht'
+000098f0: 3a20 2748 6169 7469 616e 2043 7265 6f6c  : 'Haitian Creol
+00009900: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
+00009910: 2020 2020 2020 2020 2020 2020 2027 6861               'ha
+00009920: 273a 2027 4861 7573 6127 2c0d 0a20 2020  ': 'Hausa',..   
+00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009940: 2020 2020 2027 6861 7727 3a20 2748 6177       'haw': 'Haw
+00009950: 6169 6961 6e27 2c0d 0a20 2020 2020 2020  aiian',..       
+00009960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009970: 2027 6865 273a 2027 4865 6272 6577 272c   'he': 'Hebrew',
+00009980: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009990: 2020 2020 2020 2020 2020 2768 6927 3a20            'hi': 
+000099a0: 2748 696e 6469 272c 0d0a 2020 2020 2020  'Hindi',..      
+000099b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099c0: 2020 2768 6d6e 273a 2027 486d 6f6e 6727    'hmn': 'Hmong'
+000099d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000099e0: 2020 2020 2020 2020 2020 2027 6875 273a             'hu':
+000099f0: 2027 4875 6e67 6172 6961 6e27 2c0d 0a20   'Hungarian',.. 
+00009a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a10: 2020 2020 2020 2027 6973 273a 2027 4963         'is': 'Ic
+00009a20: 656c 616e 6469 6327 2c0d 0a20 2020 2020  elandic',..     
+00009a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a40: 2020 2027 6967 273a 2027 4967 626f 272c     'ig': 'Igbo',
+00009a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009a60: 2020 2020 2020 2020 2020 2769 6c6f 273a            'ilo':
+00009a70: 2027 496c 6f63 616e 6f27 2c0d 0a20 2020   'Ilocano',..   
+00009a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a90: 2020 2020 2027 6964 273a 2027 496e 646f       'id': 'Indo
+00009aa0: 6e65 7369 616e 272c 0d0a 2020 2020 2020  nesian',..      
+00009ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ac0: 2020 2767 6127 3a20 2749 7269 7368 272c    'ga': 'Irish',
+00009ad0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009ae0: 2020 2020 2020 2020 2020 2769 7427 3a20            'it': 
+00009af0: 2749 7461 6c69 616e 272c 0d0a 2020 2020  'Italian',..    
+00009b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b10: 2020 2020 276a 6127 3a20 274a 6170 616e      'ja': 'Japan
+00009b20: 6573 6527 2c0d 0a20 2020 2020 2020 2020  ese',..         
+00009b30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009b40: 6a76 273a 2027 4a61 7661 6e65 7365 272c  jv': 'Javanese',
+00009b50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009b60: 2020 2020 2020 2020 2020 276b 6e27 3a20            'kn': 
+00009b70: 274b 616e 6e61 6461 272c 0d0a 2020 2020  'Kannada',..    
+00009b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b90: 2020 2020 276b 6b27 3a20 274b 617a 616b      'kk': 'Kazak
+00009ba0: 6827 2c0d 0a20 2020 2020 2020 2020 2020  h',..           
+00009bb0: 2020 2020 2020 2020 2020 2020 2027 6b6d               'km
+00009bc0: 273a 2027 4b68 6d65 7227 2c0d 0a20 2020  ': 'Khmer',..   
+00009bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009be0: 2020 2020 2027 7277 273a 2027 4b69 6e79       'rw': 'Kiny
+00009bf0: 6172 7761 6e64 6127 2c0d 0a20 2020 2020  arwanda',..     
+00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c10: 2020 2027 676f 6d27 3a20 274b 6f6e 6b61     'gom': 'Konka
+00009c20: 6e69 272c 0d0a 2020 2020 2020 2020 2020  ni',..          
+00009c30: 2020 2020 2020 2020 2020 2020 2020 276b                'k
+00009c40: 6f27 3a20 274b 6f72 6561 6e27 2c0d 0a20  o': 'Korean',.. 
+00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c60: 2020 2020 2020 2027 6b72 6927 3a20 274b         'kri': 'K
+00009c70: 7269 6f27 2c0d 0a20 2020 2020 2020 2020  rio',..         
+00009c80: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009c90: 6b6d 7227 3a20 274b 7572 6469 7368 2028  kmr': 'Kurdish (
+00009ca0: 4b75 726d 616e 6a69 2927 2c0d 0a20 2020  Kurmanji)',..   
+00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cc0: 2020 2020 2027 636b 6227 3a20 274b 7572       'ckb': 'Kur
+00009cd0: 6469 7368 2028 536f 7261 6e69 2927 2c0d  dish (Sorani)',.
+00009ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009cf0: 2020 2020 2020 2020 2027 6b79 273a 2027           'ky': '
+00009d00: 4b79 7267 797a 272c 0d0a 2020 2020 2020  Kyrgyz',..      
+00009d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d20: 2020 276c 6f27 3a20 274c 616f 272c 0d0a    'lo': 'Lao',..
+00009d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d40: 2020 2020 2020 2020 276c 6127 3a20 274c          'la': 'L
+00009d50: 6174 696e 272c 0d0a 2020 2020 2020 2020  atin',..        
+00009d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d70: 276c 7627 3a20 274c 6174 7669 616e 272c  'lv': 'Latvian',
+00009d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009d90: 2020 2020 2020 2020 2020 276c 6e27 3a20            'ln': 
+00009da0: 274c 696e 6761 6c61 272c 0d0a 2020 2020  'Lingala',..    
+00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009dc0: 2020 2020 276c 7427 3a20 274c 6974 6875      'lt': 'Lithu
+00009dd0: 616e 6961 6e27 2c0d 0a20 2020 2020 2020  anian',..       
+00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009df0: 2027 6c67 273a 2027 4c75 6761 6e64 6127   'lg': 'Luganda'
+00009e00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009e10: 2020 2020 2020 2020 2020 2027 6c62 273a             'lb':
+00009e20: 2027 4c75 7865 6d62 6f75 7267 6973 6827   'Luxembourgish'
+00009e30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009e40: 2020 2020 2020 2020 2020 2027 6d6b 273a             'mk':
+00009e50: 2027 4d61 6365 646f 6e69 616e 272c 0d0a   'Macedonian',..
+00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e70: 2020 2020 2020 2020 276d 6727 3a20 274d          'mg': 'M
+00009e80: 616c 6167 6173 7927 2c0d 0a20 2020 2020  alagasy',..     
+00009e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ea0: 2020 2027 6d73 273a 2027 4d61 6c61 7927     'ms': 'Malay'
+00009eb0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00009ec0: 2020 2020 2020 2020 2020 2027 6d6c 273a             'ml':
+00009ed0: 2027 4d61 6c61 7961 6c61 6d27 2c0d 0a20   'Malayalam',.. 
+00009ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ef0: 2020 2020 2020 2027 6d74 273a 2027 4d61         'mt': 'Ma
+00009f00: 6c74 6573 6527 2c0d 0a20 2020 2020 2020  ltese',..       
+00009f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f20: 2027 6d69 273a 2027 4d61 6f72 6927 2c0d   'mi': 'Maori',.
+00009f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009f40: 2020 2020 2020 2020 2027 6d72 273a 2027           'mr': '
+00009f50: 4d61 7261 7468 6927 2c0d 0a20 2020 2020  Marathi',..     
+00009f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f70: 2020 2027 6d6e 692d 4d74 6569 273a 2027     'mni-Mtei': '
+00009f80: 4d65 6974 6569 6c6f 6e20 284d 616e 6970  Meiteilon (Manip
+00009f90: 7572 6929 272c 0d0a 2020 2020 2020 2020  uri)',..        
+00009fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fb0: 276c 7573 273a 2027 4d69 7a6f 272c 0d0a  'lus': 'Mizo',..
+00009fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fd0: 2020 2020 2020 2020 276d 6e27 3a20 274d          'mn': 'M
+00009fe0: 6f6e 676f 6c69 616e 272c 0d0a 2020 2020  ongolian',..    
+00009ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a000: 2020 2020 276d 7927 3a20 274d 7961 6e6d      'my': 'Myanm
+0000a010: 6172 2028 4275 726d 6573 6529 272c 0d0a  ar (Burmese)',..
+0000a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a030: 2020 2020 2020 2020 276e 6527 3a20 274e          'ne': 'N
+0000a040: 6570 616c 6927 2c0d 0a20 2020 2020 2020  epali',..       
 0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a060: 2020 2020 2020 2027 6d69 273a 2027 4d61         'mi': 'Ma
-0000a070: 6f72 6927 2c0d 0a20 2020 2020 2020 2020  ori',..         
-0000a080: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a090: 6d72 273a 2027 4d61 7261 7468 6927 2c0d  mr': 'Marathi',.
-0000a0a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a0b0: 2020 2020 2020 2020 2027 6d6e 692d 4d74           'mni-Mt
-0000a0c0: 6569 273a 2027 4d65 6974 6569 6c6f 6e20  ei': 'Meiteilon 
-0000a0d0: 284d 616e 6970 7572 6929 272c 0d0a 2020  (Manipuri)',..  
-0000a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0f0: 2020 2020 2020 276c 7573 273a 2027 4d69        'lus': 'Mi
-0000a100: 7a6f 272c 0d0a 2020 2020 2020 2020 2020  zo',..          
-0000a110: 2020 2020 2020 2020 2020 2020 2020 276d                'm
-0000a120: 6e27 3a20 274d 6f6e 676f 6c69 616e 272c  n': 'Mongolian',
-0000a130: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a140: 2020 2020 2020 2020 2020 276d 7927 3a20            'my': 
-0000a150: 274d 7961 6e6d 6172 2028 4275 726d 6573  'Myanmar (Burmes
-0000a160: 6529 272c 0d0a 2020 2020 2020 2020 2020  e)',..          
-0000a170: 2020 2020 2020 2020 2020 2020 2020 276e                'n
-0000a180: 6527 3a20 274e 6570 616c 6927 2c0d 0a20  e': 'Nepali',.. 
-0000a190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1a0: 2020 2020 2020 2027 6e6f 273a 2027 4e6f         'no': 'No
-0000a1b0: 7277 6567 6961 6e27 2c0d 0a20 2020 2020  rwegian',..     
-0000a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1d0: 2020 2027 6f72 273a 2027 4f64 6979 6120     'or': 'Odiya 
-0000a1e0: 284f 7269 7961 2927 2c0d 0a20 2020 2020  (Oriya)',..     
-0000a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a200: 2020 2027 6f6d 273a 2027 4f72 6f6d 6f27     'om': 'Oromo'
-0000a210: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a220: 2020 2020 2020 2020 2020 2027 7073 273a             'ps':
-0000a230: 2027 5061 7368 746f 272c 0d0a 2020 2020   'Pashto',..    
-0000a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a250: 2020 2020 2766 6127 3a20 2750 6572 7369      'fa': 'Persi
-0000a260: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
-0000a270: 2020 2020 2020 2020 2020 2020 2020 2770                'p
-0000a280: 6c27 3a20 2750 6f6c 6973 6827 2c0d 0a20  l': 'Polish',.. 
-0000a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2a0: 2020 2020 2020 2027 7074 273a 2027 506f         'pt': 'Po
-0000a2b0: 7274 7567 7565 7365 272c 0d0a 2020 2020  rtuguese',..    
-0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2d0: 2020 2020 2770 6127 3a20 2750 756e 6a61      'pa': 'Punja
-0000a2e0: 6269 272c 0d0a 2020 2020 2020 2020 2020  bi',..          
-0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2771                'q
-0000a300: 7527 3a20 2751 7565 6368 7561 272c 0d0a  u': 'Quechua',..
-0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a320: 2020 2020 2020 2020 2772 6f27 3a20 2752          'ro': 'R
-0000a330: 6f6d 616e 6961 6e27 2c0d 0a20 2020 2020  omanian',..     
-0000a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a350: 2020 2027 7275 273a 2027 5275 7373 6961     'ru': 'Russia
-0000a360: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
-0000a370: 2020 2020 2020 2020 2020 2020 2027 736d               'sm
-0000a380: 273a 2027 5361 6d6f 616e 272c 0d0a 2020  ': 'Samoan',..  
-0000a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3a0: 2020 2020 2020 2773 6127 3a20 2753 616e        'sa': 'San
-0000a3b0: 736b 7269 7427 2c0d 0a20 2020 2020 2020  skrit',..       
-0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3d0: 2027 6764 273a 2027 5363 6f74 7320 4761   'gd': 'Scots Ga
-0000a3e0: 656c 6963 272c 0d0a 2020 2020 2020 2020  elic',..        
+0000a060: 2027 6e6f 273a 2027 4e6f 7277 6567 6961   'no': 'Norwegia
+0000a070: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+0000a080: 2020 2020 2020 2020 2020 2020 2027 6f72               'or
+0000a090: 273a 2027 4f64 6979 6120 284f 7269 7961  ': 'Odiya (Oriya
+0000a0a0: 2927 2c0d 0a20 2020 2020 2020 2020 2020  )',..           
+0000a0b0: 2020 2020 2020 2020 2020 2020 2027 6f6d               'om
+0000a0c0: 273a 2027 4f72 6f6d 6f27 2c0d 0a20 2020  ': 'Oromo',..   
+0000a0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0e0: 2020 2020 2027 7073 273a 2027 5061 7368       'ps': 'Pash
+0000a0f0: 746f 272c 0d0a 2020 2020 2020 2020 2020  to',..          
+0000a100: 2020 2020 2020 2020 2020 2020 2020 2766                'f
+0000a110: 6127 3a20 2750 6572 7369 616e 272c 0d0a  a': 'Persian',..
+0000a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a130: 2020 2020 2020 2020 2770 6c27 3a20 2750          'pl': 'P
+0000a140: 6f6c 6973 6827 2c0d 0a20 2020 2020 2020  olish',..       
+0000a150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a160: 2027 7074 273a 2027 506f 7274 7567 7565   'pt': 'Portugue
+0000a170: 7365 272c 0d0a 2020 2020 2020 2020 2020  se',..          
+0000a180: 2020 2020 2020 2020 2020 2020 2020 2770                'p
+0000a190: 6127 3a20 2750 756e 6a61 6269 272c 0d0a  a': 'Punjabi',..
+0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1b0: 2020 2020 2020 2020 2771 7527 3a20 2751          'qu': 'Q
+0000a1c0: 7565 6368 7561 272c 0d0a 2020 2020 2020  uechua',..      
+0000a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1e0: 2020 2772 6f27 3a20 2752 6f6d 616e 6961    'ro': 'Romania
+0000a1f0: 6e27 2c0d 0a20 2020 2020 2020 2020 2020  n',..           
+0000a200: 2020 2020 2020 2020 2020 2020 2027 7275               'ru
+0000a210: 273a 2027 5275 7373 6961 6e27 2c0d 0a20  ': 'Russian',.. 
+0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a230: 2020 2020 2020 2027 736d 273a 2027 5361         'sm': 'Sa
+0000a240: 6d6f 616e 272c 0d0a 2020 2020 2020 2020  moan',..        
+0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a260: 2773 6127 3a20 2753 616e 736b 7269 7427  'sa': 'Sanskrit'
+0000a270: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a280: 2020 2020 2020 2020 2020 2027 6764 273a             'gd':
+0000a290: 2027 5363 6f74 7320 4761 656c 6963 272c   'Scots Gaelic',
+0000a2a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a2b0: 2020 2020 2020 2020 2020 276e 736f 273a            'nso':
+0000a2c0: 2027 5365 7065 6469 272c 0d0a 2020 2020   'Sepedi',..    
+0000a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2e0: 2020 2020 2773 7227 3a20 2753 6572 6269      'sr': 'Serbi
+0000a2f0: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
+0000a300: 2020 2020 2020 2020 2020 2020 2020 2773                's
+0000a310: 7427 3a20 2753 6573 6f74 686f 272c 0d0a  t': 'Sesotho',..
+0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a330: 2020 2020 2020 2020 2773 6e27 3a20 2753          'sn': 'S
+0000a340: 686f 6e61 272c 0d0a 2020 2020 2020 2020  hona',..        
+0000a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a360: 2773 6427 3a20 2753 696e 6468 6927 2c0d  'sd': 'Sindhi',.
+0000a370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a380: 2020 2020 2020 2020 2027 7369 273a 2027           'si': '
+0000a390: 5369 6e68 616c 6127 2c0d 0a20 2020 2020  Sinhala',..     
+0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3b0: 2020 2027 736b 273a 2027 536c 6f76 616b     'sk': 'Slovak
+0000a3c0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+0000a3d0: 2020 2020 2020 2020 2020 2020 2773 6c27              'sl'
+0000a3e0: 3a20 2753 6c6f 7665 6e69 616e 272c 0d0a  : 'Slovenian',..
 0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a400: 276e 736f 273a 2027 5365 7065 6469 272c  'nso': 'Sepedi',
-0000a410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a420: 2020 2020 2020 2020 2020 2773 7227 3a20            'sr': 
-0000a430: 2753 6572 6269 616e 272c 0d0a 2020 2020  'Serbian',..    
-0000a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a450: 2020 2020 2773 7427 3a20 2753 6573 6f74      'st': 'Sesot
-0000a460: 686f 272c 0d0a 2020 2020 2020 2020 2020  ho',..          
-0000a470: 2020 2020 2020 2020 2020 2020 2020 2773                's
-0000a480: 6e27 3a20 2753 686f 6e61 272c 0d0a 2020  n': 'Shona',..  
-0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4a0: 2020 2020 2020 2773 6427 3a20 2753 696e        'sd': 'Sin
-0000a4b0: 6468 6927 2c0d 0a20 2020 2020 2020 2020  dhi',..         
-0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a4d0: 7369 273a 2027 5369 6e68 616c 6127 2c0d  si': 'Sinhala',.
-0000a4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a4f0: 2020 2020 2020 2020 2027 736b 273a 2027           'sk': '
-0000a500: 536c 6f76 616b 272c 0d0a 2020 2020 2020  Slovak',..      
-0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a520: 2020 2773 6c27 3a20 2753 6c6f 7665 6e69    'sl': 'Sloveni
-0000a530: 616e 272c 0d0a 2020 2020 2020 2020 2020  an',..          
-0000a540: 2020 2020 2020 2020 2020 2020 2020 2773                's
-0000a550: 6f27 3a20 2753 6f6d 616c 6927 2c0d 0a20  o': 'Somali',.. 
-0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a570: 2020 2020 2020 2027 6573 273a 2027 5370         'es': 'Sp
-0000a580: 616e 6973 6827 2c0d 0a20 2020 2020 2020  anish',..       
+0000a400: 2020 2020 2020 2020 2773 6f27 3a20 2753          'so': 'S
+0000a410: 6f6d 616c 6927 2c0d 0a20 2020 2020 2020  omali',..       
+0000a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a430: 2027 6573 273a 2027 5370 616e 6973 6827   'es': 'Spanish'
+0000a440: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a450: 2020 2020 2020 2020 2020 2027 7375 273a             'su':
+0000a460: 2027 5375 6e64 616e 6573 6527 2c0d 0a20   'Sundanese',.. 
+0000a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a480: 2020 2020 2020 2027 7377 273a 2027 5377         'sw': 'Sw
+0000a490: 6168 696c 6927 2c0d 0a20 2020 2020 2020  ahili',..       
+0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4b0: 2027 7376 273a 2027 5377 6564 6973 6827   'sv': 'Swedish'
+0000a4c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a4d0: 2020 2020 2020 2020 2020 2027 7467 273a             'tg':
+0000a4e0: 2027 5461 6a69 6b27 2c0d 0a20 2020 2020   'Tajik',..     
+0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a500: 2020 2027 7461 273a 2027 5461 6d69 6c27     'ta': 'Tamil'
+0000a510: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a520: 2020 2020 2020 2020 2020 2027 7474 273a             'tt':
+0000a530: 2027 5461 7461 7227 2c0d 0a20 2020 2020   'Tatar',..     
+0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a550: 2020 2027 7465 273a 2027 5465 6c75 6775     'te': 'Telugu
+0000a560: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+0000a570: 2020 2020 2020 2020 2020 2020 2774 6827              'th'
+0000a580: 3a20 2754 6861 6927 2c0d 0a20 2020 2020  : 'Thai',..     
 0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5a0: 2027 7375 273a 2027 5375 6e64 616e 6573   'su': 'Sundanes
-0000a5b0: 6527 2c0d 0a20 2020 2020 2020 2020 2020  e',..           
-0000a5c0: 2020 2020 2020 2020 2020 2020 2027 7377               'sw
-0000a5d0: 273a 2027 5377 6168 696c 6927 2c0d 0a20  ': 'Swahili',.. 
+0000a5a0: 2020 2027 7469 273a 2027 5469 6772 696e     'ti': 'Tigrin
+0000a5b0: 7961 272c 0d0a 2020 2020 2020 2020 2020  ya',..          
+0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2774                't
+0000a5d0: 7327 3a20 2754 736f 6e67 6127 2c0d 0a20  s': 'Tsonga',.. 
 0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5f0: 2020 2020 2020 2027 7376 273a 2027 5377         'sv': 'Sw
-0000a600: 6564 6973 6827 2c0d 0a20 2020 2020 2020  edish',..       
+0000a5f0: 2020 2020 2020 2027 7472 273a 2027 5475         'tr': 'Tu
+0000a600: 726b 6973 6827 2c0d 0a20 2020 2020 2020  rkish',..       
 0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a620: 2027 7467 273a 2027 5461 6a69 6b27 2c0d   'tg': 'Tajik',.
-0000a630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a640: 2020 2020 2020 2020 2027 7461 273a 2027           'ta': '
-0000a650: 5461 6d69 6c27 2c0d 0a20 2020 2020 2020  Tamil',..       
+0000a620: 2027 746b 273a 2027 5475 726b 6d65 6e27   'tk': 'Turkmen'
+0000a630: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a640: 2020 2020 2020 2020 2020 2027 7477 273a             'tw':
+0000a650: 2027 5477 6920 2841 6b61 6e29 272c 0d0a   'Twi (Akan)',..
 0000a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a670: 2027 7474 273a 2027 5461 7461 7227 2c0d   'tt': 'Tatar',.
-0000a680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a690: 2020 2020 2020 2020 2027 7465 273a 2027           'te': '
-0000a6a0: 5465 6c75 6775 272c 0d0a 2020 2020 2020  Telugu',..      
-0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6c0: 2020 2774 6827 3a20 2754 6861 6927 2c0d    'th': 'Thai',.
-0000a6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a6e0: 2020 2020 2020 2020 2027 7469 273a 2027           'ti': '
-0000a6f0: 5469 6772 696e 7961 272c 0d0a 2020 2020  Tigrinya',..    
-0000a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a710: 2020 2020 2774 7327 3a20 2754 736f 6e67      'ts': 'Tsong
-0000a720: 6127 2c0d 0a20 2020 2020 2020 2020 2020  a',..           
-0000a730: 2020 2020 2020 2020 2020 2020 2027 7472               'tr
-0000a740: 273a 2027 5475 726b 6973 6827 2c0d 0a20  ': 'Turkish',.. 
-0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a760: 2020 2020 2020 2027 746b 273a 2027 5475         'tk': 'Tu
-0000a770: 726b 6d65 6e27 2c0d 0a20 2020 2020 2020  rkmen',..       
-0000a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a790: 2027 7477 273a 2027 5477 6920 2841 6b61   'tw': 'Twi (Aka
-0000a7a0: 6e29 272c 0d0a 2020 2020 2020 2020 2020  n)',..          
-0000a7b0: 2020 2020 2020 2020 2020 2020 2020 2775                'u
-0000a7c0: 6b27 3a20 2755 6b72 6169 6e69 616e 272c  k': 'Ukrainian',
-0000a7d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a7e0: 2020 2020 2020 2020 2020 2775 7227 3a20            'ur': 
-0000a7f0: 2755 7264 7527 2c0d 0a20 2020 2020 2020  'Urdu',..       
-0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a810: 2027 7567 273a 2027 5579 6768 7572 272c   'ug': 'Uyghur',
-0000a820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a830: 2020 2020 2020 2020 2020 2775 7a27 3a20            'uz': 
-0000a840: 2755 7a62 656b 272c 0d0a 2020 2020 2020  'Uzbek',..      
-0000a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a860: 2020 2776 6927 3a20 2756 6965 746e 616d    'vi': 'Vietnam
-0000a870: 6573 6527 2c0d 0a20 2020 2020 2020 2020  ese',..         
-0000a880: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a890: 6379 273a 2027 5765 6c73 6827 2c0d 0a20  cy': 'Welsh',.. 
-0000a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8b0: 2020 2020 2020 2027 7868 273a 2027 5868         'xh': 'Xh
-0000a8c0: 6f73 6127 2c0d 0a20 2020 2020 2020 2020  osa',..         
-0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000a8e0: 7969 273a 2027 5969 6464 6973 6827 2c0d  yi': 'Yiddish',.
-0000a8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a900: 2020 2020 2020 2020 2027 796f 273a 2027           'yo': '
-0000a910: 596f 7275 6261 272c 0d0a 2020 2020 2020  Yoruba',..      
-0000a920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a930: 2020 277a 7527 3a20 275a 756c 7527 2c0d    'zu': 'Zulu',.
-0000a940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a950: 2020 2020 207d 0d0a 0d0a 2020 2020 6465       }....    de
-0000a960: 6620 6765 745f 6e61 6d65 2873 656c 662c  f get_name(self,
-0000a970: 2067 6574 5f63 6f64 6529 3a0d 0a20 2020   get_code):..   
-0000a980: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000a990: 2e64 6963 742e 6765 7428 6765 745f 636f  .dict.get(get_co
-0000a9a0: 6465 2e6c 6f77 6572 2829 2c20 2222 290d  de.lower(), "").
-0000a9b0: 0a0d 0a20 2020 2064 6566 2067 6574 5f63  ...    def get_c
-0000a9c0: 6f64 6528 7365 6c66 2c20 6c61 6e67 7561  ode(self, langua
-0000a9d0: 6765 293a 0d0a 2020 2020 2020 2020 666f  ge):..        fo
-0000a9e0: 7220 6765 745f 636f 6465 2c20 6c61 6e67  r get_code, lang
-0000a9f0: 2069 6e20 7365 6c66 2e64 6963 742e 6974   in self.dict.it
-0000aa00: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-0000aa10: 2020 2020 6966 206c 616e 672e 6c6f 7765      if lang.lowe
-0000aa20: 7228 2920 3d3d 206c 616e 6775 6167 652e  r() == language.
-0000aa30: 6c6f 7765 7228 293a 0d0a 2020 2020 2020  lower():..      
-0000aa40: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000aa50: 2067 6574 5f63 6f64 650d 0a20 2020 2020   get_code..     
-0000aa60: 2020 2072 6574 7572 6e20 2222 0d0a 0d0a     return ""....
-0000aa70: 0d0a 636c 6173 7320 5761 7643 6f6e 7665  ..class WavConve
-0000aa80: 7274 6572 3a0d 0a20 2020 2040 7374 6174  rter:..    @stat
-0000aa90: 6963 6d65 7468 6f64 0d0a 2020 2020 6465  icmethod..    de
-0000aaa0: 6620 7768 6963 6828 7072 6f67 7261 6d29  f which(program)
-0000aab0: 3a0d 0a20 2020 2020 2020 2064 6566 2069  :..        def i
-0000aac0: 735f 6578 6528 6669 6c65 5f70 6174 6829  s_exe(file_path)
-0000aad0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0000aae0: 6574 7572 6e20 6f73 2e70 6174 682e 6973  eturn os.path.is
-0000aaf0: 6669 6c65 2866 696c 655f 7061 7468 2920  file(file_path) 
-0000ab00: 616e 6420 6f73 2e61 6363 6573 7328 6669  and os.access(fi
-0000ab10: 6c65 5f70 6174 682c 206f 732e 585f 4f4b  le_path, os.X_OK
-0000ab20: 290d 0a20 2020 2020 2020 2066 7061 7468  )..        fpath
-0000ab30: 2c20 5f20 3d20 6f73 2e70 6174 682e 7370  , _ = os.path.sp
-0000ab40: 6c69 7428 7072 6f67 7261 6d29 0d0a 2020  lit(program)..  
-0000ab50: 2020 2020 2020 6966 2066 7061 7468 3a0d        if fpath:.
-0000ab60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000ab70: 6973 5f65 7865 2870 726f 6772 616d 293a  is_exe(program):
-0000ab80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ab90: 2020 7265 7475 726e 2070 726f 6772 616d    return program
-0000aba0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-0000abb0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000abc0: 2070 6174 6820 696e 206f 732e 656e 7669   path in os.envi
-0000abd0: 726f 6e5b 2250 4154 4822 5d2e 7370 6c69  ron["PATH"].spli
-0000abe0: 7428 6f73 2e70 6174 6873 6570 293a 0d0a  t(os.pathsep):..
-0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac00: 7061 7468 203d 2070 6174 682e 7374 7269  path = path.stri
-0000ac10: 7028 2722 2729 0d0a 2020 2020 2020 2020  p('"')..        
-0000ac20: 2020 2020 2020 2020 6578 655f 6669 6c65          exe_file
-0000ac30: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-0000ac40: 7061 7468 2c20 7072 6f67 7261 6d29 0d0a  path, program)..
-0000ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac60: 6966 2069 735f 6578 6528 6578 655f 6669  if is_exe(exe_fi
-0000ac70: 6c65 293a 0d0a 2020 2020 2020 2020 2020  le):..          
-0000ac80: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000ac90: 2065 7865 5f66 696c 650d 0a20 2020 2020   exe_file..     
-0000aca0: 2020 2072 6574 7572 6e20 4e6f 6e65 0d0a     return None..
-0000acb0: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-0000acc0: 686f 640d 0a20 2020 2064 6566 2066 666d  hod..    def ffm
-0000acd0: 7065 675f 6368 6563 6b28 293a 0d0a 2020  peg_check():..  
-0000ace0: 2020 2020 2020 6966 2057 6176 436f 6e76        if WavConv
-0000acf0: 6572 7465 722e 7768 6963 6828 2266 666d  erter.which("ffm
-0000ad00: 7065 6722 293a 0d0a 2020 2020 2020 2020  peg"):..        
-0000ad10: 2020 2020 7265 7475 726e 2022 6666 6d70      return "ffmp
-0000ad20: 6567 220d 0a20 2020 2020 2020 2069 6620  eg"..        if 
-0000ad30: 5761 7643 6f6e 7665 7274 6572 2e77 6869  WavConverter.whi
-0000ad40: 6368 2822 6666 6d70 6567 2e65 7865 2229  ch("ffmpeg.exe")
-0000ad50: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0000ad60: 6574 7572 6e20 2266 666d 7065 672e 6578  eturn "ffmpeg.ex
-0000ad70: 6522 0d0a 2020 2020 2020 2020 7265 7475  e"..        retu
-0000ad80: 726e 204e 6f6e 650d 0a0d 0a20 2020 2064  rn None....    d
-0000ad90: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-0000ada0: 2c20 6368 616e 6e65 6c73 3d31 2c20 7261  , channels=1, ra
-0000adb0: 7465 3d34 3830 3030 2c20 7072 6f67 7265  te=48000, progre
-0000adc0: 7373 5f63 616c 6c62 6163 6b3d 4e6f 6e65  ss_callback=None
-0000add0: 2c20 6572 726f 725f 6d65 7373 6167 6573  , error_messages
-0000ade0: 5f63 616c 6c62 6163 6b3d 4e6f 6e65 293a  _callback=None):
-0000adf0: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-0000ae00: 6861 6e6e 656c 7320 3d20 6368 616e 6e65  hannels = channe
-0000ae10: 6c73 0d0a 2020 2020 2020 2020 7365 6c66  ls..        self
-0000ae20: 2e72 6174 6520 3d20 7261 7465 0d0a 2020  .rate = rate..  
-0000ae30: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-0000ae40: 6573 735f 6361 6c6c 6261 636b 203d 2070  ess_callback = p
-0000ae50: 726f 6772 6573 735f 6361 6c6c 6261 636b  rogress_callback
-0000ae60: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
-0000ae70: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000ae80: 6c6c 6261 636b 203d 2065 7272 6f72 5f6d  llback = error_m
-0000ae90: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
-0000aea0: 0d0a 0d0a 2020 2020 6465 6620 5f5f 6361  ....    def __ca
-0000aeb0: 6c6c 5f5f 2873 656c 662c 206d 6564 6961  ll__(self, media
-0000aec0: 5f66 696c 6570 6174 6829 3a0d 0a20 2020  _filepath):..   
-0000aed0: 2020 2020 2074 656d 7020 3d20 7465 6d70       temp = temp
-0000aee0: 6669 6c65 2e4e 616d 6564 5465 6d70 6f72  file.NamedTempor
-0000aef0: 6172 7946 696c 6528 7375 6666 6978 3d27  aryFile(suffix='
-0000af00: 2e77 6176 272c 2064 656c 6574 653d 4661  .wav', delete=Fa
-0000af10: 6c73 6529 0d0a 2020 2020 2020 2020 6966  lse)..        if
-0000af20: 206e 6f74 206f 732e 7061 7468 2e69 7366   not os.path.isf
-0000af30: 696c 6528 6d65 6469 615f 6669 6c65 7061  ile(media_filepa
-0000af40: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
-0000af50: 2020 6966 2073 656c 662e 6572 726f 725f    if self.error_
-0000af60: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000af70: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
-0000af80: 2020 2020 7365 6c66 2e65 7272 6f72 5f6d      self.error_m
-0000af90: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
-0000afa0: 2822 5468 6520 6769 7665 6e20 6669 6c65  ("The given file
-0000afb0: 2064 6f65 7320 6e6f 7420 6578 6973 743a   does not exist:
-0000afc0: 207b 307d 222e 666f 726d 6174 286d 6564   {0}".format(med
-0000afd0: 6961 5f66 696c 6570 6174 6829 290d 0a20  ia_filepath)).. 
-0000afe0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000aff0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b000: 2020 7072 696e 7428 2254 6865 2067 6976    print("The giv
-0000b010: 656e 2066 696c 6520 646f 6573 206e 6f74  en file does not
-0000b020: 2065 7869 7374 3a20 7b30 7d22 2e66 6f72   exist: {0}".for
-0000b030: 6d61 7428 6d65 6469 615f 6669 6c65 7061  mat(media_filepa
-0000b040: 7468 2929 0d0a 2020 2020 2020 2020 2020  th))..          
-0000b050: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
-0000b060: 7074 696f 6e28 2249 6e76 616c 6964 2066  ption("Invalid f
-0000b070: 696c 653a 207b 307d 222e 666f 726d 6174  ile: {0}".format
-0000b080: 286d 6564 6961 5f66 696c 6570 6174 6829  (media_filepath)
-0000b090: 290d 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
-0000b0a0: 7420 7365 6c66 2e66 666d 7065 675f 6368  t self.ffmpeg_ch
-0000b0b0: 6563 6b28 293a 0d0a 2020 2020 2020 2020  eck():..        
-0000b0c0: 2020 2020 6966 2073 656c 662e 6572 726f      if self.erro
-0000b0d0: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000b0e0: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
-0000b0f0: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
-0000b100: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000b110: 636b 2822 6666 6d70 6567 3a20 4578 6563  ck("ffmpeg: Exec
-0000b120: 7574 6162 6c65 206e 6f74 2066 6f75 6e64  utable not found
-0000b130: 206f 6e20 6d61 6368 696e 652e 2229 0d0a   on machine.")..
-0000b140: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000b150: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000b160: 2020 2070 7269 6e74 2822 6666 6d70 6567     print("ffmpeg
-0000b170: 3a20 4578 6563 7574 6162 6c65 206e 6f74  : Executable not
-0000b180: 2066 6f75 6e64 206f 6e20 6d61 6368 696e   found on machin
-0000b190: 652e 2229 0d0a 2020 2020 2020 2020 2020  e.")..          
-0000b1a0: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
-0000b1b0: 7074 696f 6e28 2244 6570 656e 6465 6e63  ption("Dependenc
-0000b1c0: 7920 6e6f 7420 666f 756e 643a 2066 666d  y not found: ffm
-0000b1d0: 7065 6722 290d 0a0d 0a20 2020 2020 2020  peg")....       
-0000b1e0: 2063 6f6d 6d61 6e64 203d 205b 0d0a 2020   command = [..  
-0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b200: 2020 2266 666d 7065 6722 2c0d 0a20 2020    "ffmpeg",..   
-0000b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b220: 2022 2d79 222c 0d0a 2020 2020 2020 2020   "-y",..        
-0000b230: 2020 2020 2020 2020 2020 2020 222d 6922              "-i"
-0000b240: 2c20 6d65 6469 615f 6669 6c65 7061 7468  , media_filepath
-0000b250: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000b260: 2020 2020 2020 2022 2d61 6322 2c20 7374         "-ac", st
-0000b270: 7228 7365 6c66 2e63 6861 6e6e 656c 7329  r(self.channels)
-0000b280: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000b290: 2020 2020 2020 2022 2d61 7222 2c20 7374         "-ar", st
-0000b2a0: 7228 7365 6c66 2e72 6174 6529 2c0d 0a20  r(self.rate),.. 
-0000b2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2c0: 2020 2022 2d6c 6f67 6c65 7665 6c22 2c20     "-loglevel", 
-0000b2d0: 2265 7272 6f72 222c 0d0a 2020 2020 2020  "error",..      
-0000b2e0: 2020 2020 2020 2020 2020 2020 2020 222d                "-
-0000b2f0: 6869 6465 5f62 616e 6e65 7222 2c0d 0a20  hide_banner",.. 
-0000b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b310: 2020 2074 656d 702e 6e61 6d65 0d0a 2020     temp.name..  
-0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b330: 5d0d 0a0d 0a20 2020 2020 2020 2074 7279  ]....        try
-0000b340: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-0000b350: 2052 554e 4e49 4e47 2066 666d 7065 6720   RUNNING ffmpeg 
-0000b360: 5749 5448 4f55 5420 5348 4f57 494e 4720  WITHOUT SHOWING 
-0000b370: 5052 4f47 5245 5353 530d 0a20 2020 2020  PROGRESSS..     
-0000b380: 2020 2020 2020 2023 7573 655f 7368 656c         #use_shel
-0000b390: 6c20 3d20 5472 7565 2069 6620 6f73 2e6e  l = True if os.n
-0000b3a0: 616d 6520 3d3d 2022 6e74 2220 656c 7365  ame == "nt" else
-0000b3b0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-0000b3c0: 2020 2020 2373 7562 7072 6f63 6573 732e      #subprocess.
-0000b3d0: 6368 6563 6b5f 6f75 7470 7574 2863 6f6d  check_output(com
-0000b3e0: 6d61 6e64 2c20 7374 6469 6e3d 6f70 656e  mand, stdin=open
-0000b3f0: 286f 732e 6465 766e 756c 6c29 2c20 7368  (os.devnull), sh
-0000b400: 656c 6c3d 7573 655f 7368 656c 6c29 0d0a  ell=use_shell)..
-0000b410: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000b420: 5255 4e4e 494e 4720 6666 6d70 6567 2057  RUNNING ffmpeg W
-0000b430: 4954 4820 5052 4f47 5245 5353 530d 0a20  ITH PROGRESSS.. 
-0000b440: 2020 2020 2020 2020 2020 2066 6620 3d20             ff = 
-0000b450: 4666 6d70 6567 5072 6f67 7265 7373 2863  FfmpegProgress(c
-0000b460: 6f6d 6d61 6e64 290d 0a20 2020 2020 2020  ommand)..       
-0000b470: 2020 2020 2070 6572 6365 6e74 6167 6520       percentage 
-0000b480: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
-0000b490: 2066 6f72 2070 726f 6772 6573 7320 696e   for progress in
-0000b4a0: 2066 662e 7275 6e5f 636f 6d6d 616e 645f   ff.run_command_
-0000b4b0: 7769 7468 5f70 726f 6772 6573 7328 293a  with_progress():
-0000b4c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b4d0: 2020 7065 7263 656e 7461 6765 203d 2070    percentage = p
-0000b4e0: 726f 6772 6573 730d 0a20 2020 2020 2020  rogress..       
-0000b4f0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000b500: 2e70 726f 6772 6573 735f 6361 6c6c 6261  .progress_callba
-0000b510: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
-0000b520: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000b530: 6f67 7265 7373 5f63 616c 6c62 6163 6b28  ogress_callback(
-0000b540: 6d65 6469 615f 6669 6c65 7061 7468 2c20  media_filepath, 
-0000b550: 7065 7263 656e 7461 6765 290d 0a20 2020  percentage)..   
-0000b560: 2020 2020 2020 2020 2074 656d 702e 636c           temp.cl
-0000b570: 6f73 6528 290d 0a0d 0a20 2020 2020 2020  ose()....       
-0000b580: 2020 2020 2072 6574 7572 6e20 7465 6d70       return temp
-0000b590: 2e6e 616d 652c 2073 656c 662e 7261 7465  .name, self.rate
-0000b5a0: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
-0000b5b0: 7074 204b 6579 626f 6172 6449 6e74 6572  pt KeyboardInter
-0000b5c0: 7275 7074 3a0d 0a20 2020 2020 2020 2020  rupt:..         
-0000b5d0: 2020 2069 6620 7365 6c66 2e65 7272 6f72     if self.error
-0000b5e0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000b5f0: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
-0000b600: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
-0000b610: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000b620: 6b28 2243 616e 6365 6c6c 696e 6720 616c  k("Cancelling al
-0000b630: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
-0000b640: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0000b650: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000b660: 696e 7428 2243 616e 6365 6c6c 696e 6720  int("Cancelling 
-0000b670: 616c 6c20 7461 736b 7322 290d 0a20 2020  all tasks")..   
-0000b680: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
-0000b690: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
-0000b6a0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-0000b6b0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-0000b6c0: 6620 7365 6c66 2e65 7272 6f72 5f6d 6573  f self.error_mes
-0000b6d0: 7361 6765 735f 6361 6c6c 6261 636b 3a0d  sages_callback:.
-0000b6e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b6f0: 2073 656c 662e 6572 726f 725f 6d65 7373   self.error_mess
-0000b700: 6167 6573 5f63 616c 6c62 6163 6b28 6529  ages_callback(e)
-0000b710: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0000b720: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000b730: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
-0000b740: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000b750: 6e0d 0a0d 0a0d 0a63 6c61 7373 2053 656e  n......class Sen
-0000b760: 7465 6e63 6554 7261 6e73 6c61 746f 7228  tenceTranslator(
-0000b770: 6f62 6a65 6374 293a 0d0a 2020 2020 6465  object):..    de
-0000b780: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-0000b790: 2073 7263 2c20 6473 742c 2070 6174 6965   src, dst, patie
-0000b7a0: 6e63 653d 2d31 2c20 7469 6d65 6f75 743d  nce=-1, timeout=
-0000b7b0: 3330 2c20 6572 726f 725f 6d65 7373 6167  30, error_messag
-0000b7c0: 6573 5f63 616c 6c62 6163 6b3d 4e6f 6e65  es_callback=None
-0000b7d0: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
-0000b7e0: 2e73 7263 203d 2073 7263 0d0a 2020 2020  .src = src..    
-0000b7f0: 2020 2020 7365 6c66 2e64 7374 203d 2064      self.dst = d
-0000b800: 7374 0d0a 2020 2020 2020 2020 7365 6c66  st..        self
-0000b810: 2e70 6174 6965 6e63 6520 3d20 7061 7469  .patience = pati
-0000b820: 656e 6365 0d0a 2020 2020 2020 2020 7365  ence..        se
-0000b830: 6c66 2e74 696d 656f 7574 203d 2074 696d  lf.timeout = tim
-0000b840: 656f 7574 0d0a 2020 2020 2020 2020 7365  eout..        se
-0000b850: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
-0000b860: 735f 6361 6c6c 6261 636b 203d 2065 7272  s_callback = err
-0000b870: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-0000b880: 6261 636b 0d0a 0d0a 2020 2020 6465 6620  back....    def 
-0000b890: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2073  __call__(self, s
-0000b8a0: 656e 7465 6e63 6529 3a0d 0a20 2020 2020  entence):..     
-0000b8b0: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-0000b8c0: 2020 2020 2074 7261 6e73 6c61 7465 645f       translated_
-0000b8d0: 7365 6e74 656e 6365 203d 205b 5d0d 0a20  sentence = [].. 
-0000b8e0: 2020 2020 2020 2020 2020 2023 2068 616e             # han
-0000b8f0: 646c 6520 7468 6520 7370 6563 6961 6c20  dle the special 
-0000b900: 6361 7365 3a20 656d 7074 7920 7374 7269  case: empty stri
-0000b910: 6e67 2e0d 0a20 2020 2020 2020 2020 2020  ng...           
-0000b920: 2069 6620 6e6f 7420 7365 6e74 656e 6365   if not sentence
-0000b930: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000b940: 2020 2072 6574 7572 6e20 4e6f 6e65 0d0a     return None..
-0000b950: 2020 2020 2020 2020 2020 2020 7472 616e              tran
-0000b960: 736c 6174 6564 5f73 656e 7465 6e63 6520  slated_sentence 
-0000b970: 3d20 7365 6c66 2e47 6f6f 676c 6554 7261  = self.GoogleTra
-0000b980: 6e73 6c61 7465 2873 656e 7465 6e63 652c  nslate(sentence,
-0000b990: 2073 7263 3d73 656c 662e 7372 632c 2064   src=self.src, d
-0000b9a0: 7374 3d73 656c 662e 6473 742c 2074 696d  st=self.dst, tim
-0000b9b0: 656f 7574 3d73 656c 662e 7469 6d65 6f75  eout=self.timeou
-0000b9c0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-0000b9d0: 6661 696c 5f74 6f5f 7472 616e 736c 6174  fail_to_translat
-0000b9e0: 6520 3d20 7472 616e 736c 6174 6564 5f73  e = translated_s
-0000b9f0: 656e 7465 6e63 655b 2d31 5d20 3d3d 2027  entence[-1] == '
-0000ba00: 5c6e 270d 0a20 2020 2020 2020 2020 2020  \n'..           
-0000ba10: 2077 6869 6c65 2066 6169 6c5f 746f 5f74   while fail_to_t
-0000ba20: 7261 6e73 6c61 7465 2061 6e64 2070 6174  ranslate and pat
-0000ba30: 6965 6e63 653a 0d0a 2020 2020 2020 2020  ience:..        
-0000ba40: 2020 2020 2020 2020 7472 616e 736c 6174          translat
-0000ba50: 6564 5f73 656e 7465 6e63 6520 3d20 7365  ed_sentence = se
-0000ba60: 6c66 2e47 6f6f 676c 6554 7261 6e73 6c61  lf.GoogleTransla
-0000ba70: 7465 2874 7261 6e73 6c61 7465 645f 7365  te(translated_se
-0000ba80: 6e74 656e 6365 2c20 7372 633d 7365 6c66  ntence, src=self
-0000ba90: 2e73 7263 2c20 6473 743d 7365 6c66 2e64  .src, dst=self.d
-0000baa0: 7374 2c20 7469 6d65 6f75 743d 7365 6c66  st, timeout=self
-0000bab0: 2e74 696d 656f 7574 292e 7465 7874 0d0a  .timeout).text..
-0000bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bad0: 6966 2074 7261 6e73 6c61 7465 645f 7365  if translated_se
-0000bae0: 6e74 656e 6365 5b2d 315d 203d 3d20 275c  ntence[-1] == '\
-0000baf0: 6e27 3a0d 0a20 2020 2020 2020 2020 2020  n':..           
-0000bb00: 2020 2020 2020 2020 2069 6620 7061 7469           if pati
-0000bb10: 656e 6365 203d 3d20 2d31 3a0d 0a20 2020  ence == -1:..   
-0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb30: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
-0000bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb50: 2020 2070 6174 6965 6e63 6520 2d3d 2031     patience -= 1
-0000bb60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bb70: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0000bb80: 2020 2020 2020 2020 2020 2020 2066 6169               fai
-0000bb90: 6c5f 746f 5f74 7261 6e73 6c61 7465 203d  l_to_translate =
-0000bba0: 2046 616c 7365 0d0a 0d0a 2020 2020 2020   False....      
-0000bbb0: 2020 2020 2020 7265 7475 726e 2074 7261        return tra
-0000bbc0: 6e73 6c61 7465 645f 7365 6e74 656e 6365  nslated_sentence
-0000bbd0: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
-0000bbe0: 7074 204b 6579 626f 6172 6449 6e74 6572  pt KeyboardInter
-0000bbf0: 7275 7074 3a0d 0a20 2020 2020 2020 2020  rupt:..         
-0000bc00: 2020 2069 6620 7365 6c66 2e65 7272 6f72     if self.error
-0000bc10: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000bc20: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
-0000bc30: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
-0000bc40: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000bc50: 6b28 2243 616e 6365 6c6c 696e 6720 616c  k("Cancelling al
-0000bc60: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
-0000bc70: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0000bc80: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000bc90: 696e 7428 2243 616e 6365 6c6c 696e 6720  int("Cancelling 
-0000bca0: 616c 6c20 7461 736b 7322 290d 0a20 2020  all tasks")..   
-0000bcb0: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
-0000bcc0: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
-0000bcd0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-0000bce0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-0000bcf0: 6620 7365 6c66 2e65 7272 6f72 5f6d 6573  f self.error_mes
-0000bd00: 7361 6765 735f 6361 6c6c 6261 636b 3a0d  sages_callback:.
-0000bd10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bd20: 2073 656c 662e 6572 726f 725f 6d65 7373   self.error_mess
-0000bd30: 6167 6573 5f63 616c 6c62 6163 6b28 6529  ages_callback(e)
-0000bd40: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0000bd50: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000bd60: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
-0000bd70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000bd80: 6e0d 0a0d 0a20 2020 2064 6566 2047 6f6f  n....    def Goo
-0000bd90: 676c 6554 7261 6e73 6c61 7465 2873 656c  gleTranslate(sel
-0000bda0: 662c 2074 6578 742c 2073 7263 2c20 6473  f, text, src, ds
-0000bdb0: 742c 2074 696d 656f 7574 3d33 3029 3a0d  t, timeout=30):.
-0000bdc0: 0a20 2020 2020 2020 2075 726c 203d 2027  .        url = '
-0000bdd0: 6874 7470 733a 2f2f 7472 616e 736c 6174  https://translat
-0000bde0: 652e 676f 6f67 6c65 6170 6973 2e63 6f6d  e.googleapis.com
-0000bdf0: 2f74 7261 6e73 6c61 7465 5f61 2f27 0d0a  /translate_a/'..
-0000be00: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
-0000be10: 2027 7369 6e67 6c65 3f63 6c69 656e 743d   'single?client=
-0000be20: 6774 7826 736c 3d27 2b73 7263 2b27 2674  gtx&sl='+src+'&t
-0000be30: 6c3d 272b 6473 742b 2726 6474 3d74 2671  l='+dst+'&dt=t&q
-0000be40: 3d27 2b74 6578 743b 0d0a 2020 2020 2020  ='+text;..      
-0000be50: 2020 6865 6164 6572 7320 3d20 7b27 5573    headers = {'Us
-0000be60: 6572 2d41 6765 6e74 273a 2027 4d6f 7a69  er-Agent': 'Mozi
-0000be70: 6c6c 612f 352e 3020 2857 696e 646f 7773  lla/5.0 (Windows
-0000be80: 204e 5420 3130 2e30 3b20 5769 6e36 343b   NT 10.0; Win64;
-0000be90: 2078 3634 2927 2c20 2752 6566 6572 6572   x64)', 'Referer
-0000bea0: 273a 2027 6874 7470 733a 2f2f 7472 616e  ': 'https://tran
-0000beb0: 736c 6174 652e 676f 6f67 6c65 2e63 6f6d  slate.google.com
-0000bec0: 272c 7d0d 0a0d 0a20 2020 2020 2020 2074  ',}....        t
-0000bed0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-0000bee0: 2072 6573 706f 6e73 6520 3d20 7265 7175   response = requ
-0000bef0: 6573 7473 2e67 6574 2875 726c 2b70 6172  ests.get(url+par
-0000bf00: 616d 732c 2068 6561 6465 7273 3d68 6561  ams, headers=hea
-0000bf10: 6465 7273 2c20 7469 6d65 6f75 743d 7365  ders, timeout=se
-0000bf20: 6c66 2e74 696d 656f 7574 290d 0a20 2020  lf.timeout)..   
-0000bf30: 2020 2020 2020 2020 2069 6620 7265 7370           if resp
-0000bf40: 6f6e 7365 2e73 7461 7475 735f 636f 6465  onse.status_code
-0000bf50: 203d 3d20 3230 303a 0d0a 2020 2020 2020   == 200:..      
-0000bf60: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
-0000bf70: 7365 5f6a 736f 6e20 3d20 7265 7370 6f6e  se_json = respon
-0000bf80: 7365 2e6a 736f 6e28 295b 305d 0d0a 2020  se.json()[0]..  
-0000bf90: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-0000bfa0: 6e67 7468 203d 206c 656e 2872 6573 706f  ngth = len(respo
-0000bfb0: 6e73 655f 6a73 6f6e 290d 0a20 2020 2020  nse_json)..     
-0000bfc0: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
-0000bfd0: 6c61 7469 6f6e 203d 2022 220d 0a20 2020  lation = ""..   
-0000bfe0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000bff0: 2069 2069 6e20 7261 6e67 6528 6c65 6e67   i in range(leng
-0000c000: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
-0000c010: 2020 2020 2020 2020 2020 7472 616e 736c            transl
-0000c020: 6174 696f 6e20 3d20 7472 616e 736c 6174  ation = translat
-0000c030: 696f 6e20 2b20 7265 7370 6f6e 7365 5f6a  ion + response_j
-0000c040: 736f 6e5b 695d 5b30 5d0d 0a20 2020 2020  son[i][0]..     
-0000c050: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000c060: 6e20 7472 616e 736c 6174 696f 6e0d 0a20  n translation.. 
-0000c070: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000c080: 6e0d 0a0d 0a20 2020 2020 2020 2065 7863  n....        exc
-0000c090: 6570 7420 7265 7175 6573 7473 2e65 7863  ept requests.exc
-0000c0a0: 6570 7469 6f6e 732e 436f 6e6e 6563 7469  eptions.Connecti
-0000c0b0: 6f6e 4572 726f 723a 0d0a 2020 2020 2020  onError:..      
-0000c0c0: 2020 2020 2020 7769 7468 2068 7474 7078        with httpx
-0000c0d0: 2e43 6c69 656e 7428 2920 6173 2063 6c69  .Client() as cli
-0000c0e0: 656e 743a 0d0a 2020 2020 2020 2020 2020  ent:..          
-0000c0f0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-0000c100: 2063 6c69 656e 742e 6765 7428 7572 6c2b   client.get(url+
-0000c110: 7061 7261 6d73 2c20 6865 6164 6572 733d  params, headers=
-0000c120: 6865 6164 6572 732c 2074 696d 656f 7574  headers, timeout
-0000c130: 3d73 656c 662e 7469 6d65 6f75 7429 0d0a  =self.timeout)..
-0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c150: 6966 2072 6573 706f 6e73 652e 7374 6174  if response.stat
-0000c160: 7573 5f63 6f64 6520 3d3d 2032 3030 3a0d  us_code == 200:.
-0000c170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c180: 2020 2020 2072 6573 706f 6e73 655f 6a73       response_js
-0000c190: 6f6e 203d 2072 6573 706f 6e73 652e 6a73  on = response.js
-0000c1a0: 6f6e 2829 5b30 5d0d 0a20 2020 2020 2020  on()[0]..       
-0000c1b0: 2020 2020 2020 2020 2020 2020 206c 656e               len
-0000c1c0: 6774 6820 3d20 6c65 6e28 7265 7370 6f6e  gth = len(respon
-0000c1d0: 7365 5f6a 736f 6e29 0d0a 2020 2020 2020  se_json)..      
-0000c1e0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0000c1f0: 616e 736c 6174 696f 6e20 3d20 2222 0d0a  anslation = ""..
-0000c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c210: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0000c220: 6765 286c 656e 6774 6829 3a0d 0a20 2020  ge(length):..   
-0000c230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c240: 2020 2020 2074 7261 6e73 6c61 7469 6f6e       translation
-0000c250: 203d 2074 7261 6e73 6c61 7469 6f6e 202b   = translation +
-0000c260: 2072 6573 706f 6e73 655f 6a73 6f6e 5b69   response_json[i
-0000c270: 5d5b 305d 0d0a 2020 2020 2020 2020 2020  ][0]..          
-0000c280: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000c290: 2074 7261 6e73 6c61 7469 6f6e 0d0a 2020   translation..  
-0000c2a0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000c2b0: 7475 726e 0d0a 0d0a 2020 2020 2020 2020  turn....        
-0000c2c0: 6578 6365 7074 204b 6579 626f 6172 6449  except KeyboardI
-0000c2d0: 6e74 6572 7275 7074 3a0d 0a20 2020 2020  nterrupt:..     
-0000c2e0: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-0000c2f0: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000c300: 6c6c 6261 636b 3a0d 0a20 2020 2020 2020  llback:..       
-0000c310: 2020 2020 2020 2020 2073 656c 662e 6572           self.er
-0000c320: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-0000c330: 6c62 6163 6b28 2243 616e 6365 6c6c 696e  lback("Cancellin
-0000c340: 6720 616c 6c20 7461 736b 7322 290d 0a20  g all tasks").. 
-0000c350: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000c360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c370: 2020 7072 696e 7428 2243 616e 6365 6c6c    print("Cancell
-0000c380: 696e 6720 616c 6c20 7461 736b 7322 290d  ing all tasks").
-0000c390: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000c3a0: 7572 6e0d 0a0d 0a20 2020 2020 2020 2065  urn....        e
-0000c3b0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-0000c3c0: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
-0000c3d0: 2020 2069 6620 7365 6c66 2e65 7272 6f72     if self.error
-0000c3e0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000c3f0: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
-0000c400: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
-0000c410: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000c420: 6b28 6529 0d0a 2020 2020 2020 2020 2020  k(e)..          
-0000c430: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0000c440: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
-0000c450: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-0000c460: 6574 7572 6e0d 0a0d 0a0d 0a63 6c61 7373  eturn......class
-0000c470: 2053 7562 7469 746c 6546 6f72 6d61 7474   SubtitleFormatt
-0000c480: 6572 3a0d 0a20 2020 2073 7570 706f 7274  er:..    support
-0000c490: 6564 5f66 6f72 6d61 7473 203d 205b 2773  ed_formats = ['s
-0000c4a0: 7274 272c 2027 7674 7427 2c20 276a 736f  rt', 'vtt', 'jso
-0000c4b0: 6e27 2c20 2772 6177 275d 0d0a 0d0a 2020  n', 'raw']....  
-0000c4c0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0000c4d0: 656c 662c 2066 6f72 6d61 745f 7479 7065  elf, format_type
-0000c4e0: 2c20 6572 726f 725f 6d65 7373 6167 6573  , error_messages
-0000c4f0: 5f63 616c 6c62 6163 6b3d 4e6f 6e65 293a  _callback=None):
-0000c500: 0d0a 2020 2020 2020 2020 7365 6c66 2e66  ..        self.f
-0000c510: 6f72 6d61 745f 7479 7065 203d 2066 6f72  ormat_type = for
-0000c520: 6d61 745f 7479 7065 2e6c 6f77 6572 2829  mat_type.lower()
-0000c530: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
-0000c540: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000c550: 6c6c 6261 636b 203d 2065 7272 6f72 5f6d  llback = error_m
-0000c560: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
-0000c570: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-0000c580: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
-0000c590: 662c 2073 7562 7469 746c 6573 2c20 7061  f, subtitles, pa
-0000c5a0: 6464 696e 675f 6265 666f 7265 3d30 2c20  dding_before=0, 
-0000c5b0: 7061 6464 696e 675f 6166 7465 723d 3029  padding_after=0)
-0000c5c0: 3a0d 0a20 2020 2020 2020 2074 7279 3a0d  :..        try:.
-0000c5d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c5e0: 7365 6c66 2e66 6f72 6d61 745f 7479 7065  self.format_type
-0000c5f0: 203d 3d20 2773 7274 273a 0d0a 2020 2020   == 'srt':..    
-0000c600: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c610: 726e 2073 656c 662e 7372 745f 666f 726d  rn self.srt_form
-0000c620: 6174 7465 7228 7375 6274 6974 6c65 732c  atter(subtitles,
-0000c630: 2070 6164 6469 6e67 5f62 6566 6f72 652c   padding_before,
-0000c640: 2070 6164 6469 6e67 5f61 6674 6572 290d   padding_after).
-0000c650: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-0000c660: 6620 7365 6c66 2e66 6f72 6d61 745f 7479  f self.format_ty
-0000c670: 7065 203d 3d20 2776 7474 273a 0d0a 2020  pe == 'vtt':..  
-0000c680: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000c690: 7475 726e 2073 656c 662e 7674 745f 666f  turn self.vtt_fo
-0000c6a0: 726d 6174 7465 7228 7375 6274 6974 6c65  rmatter(subtitle
-0000c6b0: 732c 2070 6164 6469 6e67 5f62 6566 6f72  s, padding_befor
-0000c6c0: 652c 2070 6164 6469 6e67 5f61 6674 6572  e, padding_after
-0000c6d0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-0000c6e0: 6c69 6620 7365 6c66 2e66 6f72 6d61 745f  lif self.format_
-0000c6f0: 7479 7065 203d 3d20 276a 736f 6e27 3a0d  type == 'json':.
-0000c700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c710: 2072 6574 7572 6e20 7365 6c66 2e6a 736f   return self.jso
-0000c720: 6e5f 666f 726d 6174 7465 7228 7375 6274  n_formatter(subt
-0000c730: 6974 6c65 7329 0d0a 2020 2020 2020 2020  itles)..        
-0000c740: 2020 2020 656c 6966 2073 656c 662e 666f      elif self.fo
-0000c750: 726d 6174 5f74 7970 6520 3d3d 2027 7261  rmat_type == 'ra
-0000c760: 7727 3a0d 0a20 2020 2020 2020 2020 2020  w':..           
-0000c770: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000c780: 2e72 6177 5f66 6f72 6d61 7474 6572 2873  .raw_formatter(s
-0000c790: 7562 7469 746c 6573 290d 0a20 2020 2020  ubtitles)..     
-0000c7a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0000c7b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000c7c0: 2065 7272 6f72 5f6d 6573 7361 6765 735f   error_messages_
-0000c7d0: 6361 6c6c 6261 636b 3a0d 0a20 2020 2020  callback:..     
-0000c7e0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000c7f0: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000c800: 6c6c 6261 636b 2866 2755 6e73 7570 706f  llback(f'Unsuppo
-0000c810: 7274 6564 2066 6f72 6d61 7420 7479 7065  rted format type
-0000c820: 3a20 7b73 656c 662e 666f 726d 6174 5f74  : {self.format_t
-0000c830: 7970 657d 2729 0d0a 2020 2020 2020 2020  ype}')..        
-0000c840: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c860: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000c870: 726f 7228 6627 556e 7375 7070 6f72 7465  ror(f'Unsupporte
-0000c880: 6420 666f 726d 6174 2074 7970 653a 207b  d format type: {
-0000c890: 7365 6c66 2e66 6f72 6d61 745f 7479 7065  self.format_type
-0000c8a0: 7d27 290d 0a0d 0a20 2020 2020 2020 2065  }')....        e
-0000c8b0: 7863 6570 7420 4b65 7962 6f61 7264 496e  xcept KeyboardIn
-0000c8c0: 7465 7272 7570 743a 0d0a 2020 2020 2020  terrupt:..      
-0000c8d0: 2020 2020 2020 6966 2073 656c 662e 6572        if self.er
-0000c8e0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-0000c8f0: 6c62 6163 6b3a 0d0a 2020 2020 2020 2020  lback:..        
-0000c900: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
-0000c910: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-0000c920: 6261 636b 2822 4361 6e63 656c 6c69 6e67  back("Cancelling
-0000c930: 2061 6c6c 2074 6173 6b73 2229 0d0a 2020   all tasks")..  
-0000c940: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-0000c950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c960: 2070 7269 6e74 2822 4361 6e63 656c 6c69   print("Cancelli
-0000c970: 6e67 2061 6c6c 2074 6173 6b73 2229 0d0a  ng all tasks")..
-0000c980: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c990: 726e 0d0a 0d0a 2020 2020 2020 2020 6578  rn....        ex
-0000c9a0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-0000c9b0: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
-0000c9c0: 2020 6966 2073 656c 662e 6572 726f 725f    if self.error_
-0000c9d0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000c9e0: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
-0000c9f0: 2020 2020 7365 6c66 2e65 7272 6f72 5f6d      self.error_m
-0000ca00: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
-0000ca10: 2865 290d 0a20 2020 2020 2020 2020 2020  (e)..           
-0000ca20: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0000ca30: 2020 2020 2020 2020 7072 696e 7428 6529          print(e)
-0000ca40: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0000ca50: 7475 726e 0d0a 0d0a 2020 2020 6465 6620  turn....    def 
-0000ca60: 7372 745f 666f 726d 6174 7465 7228 7365  srt_formatter(se
-0000ca70: 6c66 2c20 7375 6274 6974 6c65 732c 2070  lf, subtitles, p
-0000ca80: 6164 6469 6e67 5f62 6566 6f72 653d 302c  adding_before=0,
-0000ca90: 2070 6164 6469 6e67 5f61 6674 6572 3d30   padding_after=0
-0000caa0: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
-0000cab0: 0a20 2020 2020 2020 2053 6572 6961 6c69  .        Seriali
-0000cac0: 7a65 2061 206c 6973 7420 6f66 2073 7562  ze a list of sub
-0000cad0: 7469 746c 6573 2061 6363 6f72 6469 6e67  titles according
-0000cae0: 2074 6f20 7468 6520 5352 5420 666f 726d   to the SRT form
-0000caf0: 6174 2c20 7769 7468 206f 7074 696f 6e61  at, with optiona
-0000cb00: 6c20 7469 6d65 2070 6164 6469 6e67 2e0d  l time padding..
-0000cb10: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0000cb20: 2020 2020 2020 7375 625f 7269 705f 6669        sub_rip_fi
-0000cb30: 6c65 203d 2070 7973 7274 2e53 7562 5269  le = pysrt.SubRi
-0000cb40: 7046 696c 6528 290d 0a20 2020 2020 2020  pFile()..       
-0000cb50: 2066 6f72 2069 2c20 2828 7374 6172 742c   for i, ((start,
-0000cb60: 2065 6e64 292c 2074 6578 7429 2069 6e20   end), text) in 
-0000cb70: 656e 756d 6572 6174 6528 7375 6274 6974  enumerate(subtit
-0000cb80: 6c65 732c 2073 7461 7274 3d31 293a 0d0a  les, start=1):..
-0000cb90: 2020 2020 2020 2020 2020 2020 6974 656d              item
-0000cba0: 203d 2070 7973 7274 2e53 7562 5269 7049   = pysrt.SubRipI
-0000cbb0: 7465 6d28 290d 0a20 2020 2020 2020 2020  tem()..         
-0000cbc0: 2020 2069 7465 6d2e 696e 6465 7820 3d20     item.index = 
-0000cbd0: 690d 0a20 2020 2020 2020 2020 2020 2069  i..            i
-0000cbe0: 7465 6d2e 7465 7874 203d 2073 6978 2e74  tem.text = six.t
-0000cbf0: 6578 745f 7479 7065 2874 6578 7429 0d0a  ext_type(text)..
-0000cc00: 2020 2020 2020 2020 2020 2020 6974 656d              item
-0000cc10: 2e73 7461 7274 2e73 6563 6f6e 6473 203d  .start.seconds =
-0000cc20: 206d 6178 2830 2c20 7374 6172 7420 2d20   max(0, start - 
-0000cc30: 7061 6464 696e 675f 6265 666f 7265 290d  padding_before).
-0000cc40: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
-0000cc50: 6d2e 656e 642e 7365 636f 6e64 7320 3d20  m.end.seconds = 
-0000cc60: 656e 6420 2b20 7061 6464 696e 675f 6166  end + padding_af
-0000cc70: 7465 720d 0a20 2020 2020 2020 2020 2020  ter..           
-0000cc80: 2073 7562 5f72 6970 5f66 696c 652e 6170   sub_rip_file.ap
-0000cc90: 7065 6e64 2869 7465 6d29 0d0a 2020 2020  pend(item)..    
-0000cca0: 2020 2020 7265 7475 726e 2027 5c6e 272e      return '\n'.
-0000ccb0: 6a6f 696e 2873 6978 2e74 6578 745f 7479  join(six.text_ty
-0000ccc0: 7065 2869 7465 6d29 2066 6f72 2069 7465  pe(item) for ite
-0000ccd0: 6d20 696e 2073 7562 5f72 6970 5f66 696c  m in sub_rip_fil
-0000cce0: 6529 0d0a 0d0a 2020 2020 6465 6620 7674  e)....    def vt
-0000ccf0: 745f 666f 726d 6174 7465 7228 7365 6c66  t_formatter(self
-0000cd00: 2c20 7375 6274 6974 6c65 732c 2070 6164  , subtitles, pad
-0000cd10: 6469 6e67 5f62 6566 6f72 653d 302c 2070  ding_before=0, p
-0000cd20: 6164 6469 6e67 5f61 6674 6572 3d30 293a  adding_after=0):
-0000cd30: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-0000cd40: 2020 2020 2020 2053 6572 6961 6c69 7a65         Serialize
-0000cd50: 2061 206c 6973 7420 6f66 2073 7562 7469   a list of subti
-0000cd60: 746c 6573 2061 6363 6f72 6469 6e67 2074  tles according t
-0000cd70: 6f20 7468 6520 5654 5420 666f 726d 6174  o the VTT format
-0000cd80: 2c20 7769 7468 206f 7074 696f 6e61 6c20  , with optional 
-0000cd90: 7469 6d65 2070 6164 6469 6e67 2e0d 0a20  time padding... 
-0000cda0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-0000cdb0: 2020 2020 7465 7874 203d 2073 656c 662e      text = self.
-0000cdc0: 7372 745f 666f 726d 6174 7465 7228 7375  srt_formatter(su
-0000cdd0: 6274 6974 6c65 732c 2070 6164 6469 6e67  btitles, padding
-0000cde0: 5f62 6566 6f72 652c 2070 6164 6469 6e67  _before, padding
-0000cdf0: 5f61 6674 6572 290d 0a20 2020 2020 2020  _after)..       
-0000ce00: 2074 6578 7420 3d20 2757 4542 5654 545c   text = 'WEBVTT\
-0000ce10: 6e5c 6e27 202b 2074 6578 742e 7265 706c  n\n' + text.repl
-0000ce20: 6163 6528 272c 272c 2027 2e27 290d 0a20  ace(',', '.').. 
-0000ce30: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
-0000ce40: 7874 0d0a 0d0a 2020 2020 6465 6620 6a73  xt....    def js
-0000ce50: 6f6e 5f66 6f72 6d61 7474 6572 2873 656c  on_formatter(sel
-0000ce60: 662c 2073 7562 7469 746c 6573 293a 0d0a  f, subtitles):..
-0000ce70: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0000ce80: 2020 2020 2053 6572 6961 6c69 7a65 2061       Serialize a
-0000ce90: 206c 6973 7420 6f66 2073 7562 7469 746c   list of subtitl
-0000cea0: 6573 2061 7320 6120 4a53 4f4e 2062 6c6f  es as a JSON blo
-0000ceb0: 622e 0d0a 2020 2020 2020 2020 2222 220d  b...        """.
-0000cec0: 0a20 2020 2020 2020 2073 7562 7469 746c  .        subtitl
-0000ced0: 655f 6469 6374 7320 3d20 5b0d 0a20 2020  e_dicts = [..   
-0000cee0: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
-0000cef0: 2020 2020 2020 2020 2020 2020 2773 7461              'sta
-0000cf00: 7274 273a 2073 7461 7274 2c0d 0a20 2020  rt': start,..   
-0000cf10: 2020 2020 2020 2020 2020 2020 2027 656e               'en
-0000cf20: 6427 3a20 656e 642c 0d0a 2020 2020 2020  d': end,..      
-0000cf30: 2020 2020 2020 2020 2020 2763 6f6e 7465            'conte
-0000cf40: 6e74 273a 2074 6578 742c 0d0a 2020 2020  nt': text,..    
-0000cf50: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-0000cf60: 2020 2020 2020 2066 6f72 2028 2873 7461         for ((sta
-0000cf70: 7274 2c20 656e 6429 2c20 7465 7874 290d  rt, end), text).
-0000cf80: 0a20 2020 2020 2020 2020 2020 2069 6e20  .            in 
-0000cf90: 7375 6274 6974 6c65 730d 0a20 2020 2020  subtitles..     
-0000cfa0: 2020 205d 0d0a 2020 2020 2020 2020 7265     ]..        re
-0000cfb0: 7475 726e 206a 736f 6e2e 6475 6d70 7328  turn json.dumps(
-0000cfc0: 7375 6274 6974 6c65 5f64 6963 7473 290d  subtitle_dicts).
-0000cfd0: 0a0d 0a20 2020 2064 6566 2072 6177 5f66  ...    def raw_f
-0000cfe0: 6f72 6d61 7474 6572 2873 656c 662c 2073  ormatter(self, s
-0000cff0: 7562 7469 746c 6573 293a 0d0a 2020 2020  ubtitles):..    
-0000d000: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-0000d010: 2053 6572 6961 6c69 7a65 2061 206c 6973   Serialize a lis
-0000d020: 7420 6f66 2073 7562 7469 746c 6573 2061  t of subtitles a
-0000d030: 7320 6120 6e65 776c 696e 652d 6465 6c69  s a newline-deli
-0000d040: 6d69 7465 6420 7374 7269 6e67 2e0d 0a20  mited string... 
-0000d050: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-0000d060: 2020 2020 7265 7475 726e 2027 2027 2e6a      return ' '.j
-0000d070: 6f69 6e28 7465 7874 2066 6f72 2028 5f72  oin(text for (_r
-0000d080: 6e67 2c20 7465 7874 2920 696e 2073 7562  ng, text) in sub
-0000d090: 7469 746c 6573 290d 0a0d 0a0d 0a63 6c61  titles)......cla
-0000d0a0: 7373 2053 7562 7469 746c 6557 7269 7465  ss SubtitleWrite
-0000d0b0: 723a 0d0a 2020 2020 6465 6620 5f5f 696e  r:..    def __in
-0000d0c0: 6974 5f5f 2873 656c 662c 2072 6567 696f  it__(self, regio
-0000d0d0: 6e73 2c20 7472 616e 7363 7269 7074 732c  ns, transcripts,
-0000d0e0: 2066 6f72 6d61 742c 2065 7272 6f72 5f6d   format, error_m
-0000d0f0: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
-0000d100: 3d4e 6f6e 6529 3a0d 0a20 2020 2020 2020  =None):..       
-0000d110: 2073 656c 662e 7265 6769 6f6e 7320 3d20   self.regions = 
-0000d120: 7265 6769 6f6e 730d 0a20 2020 2020 2020  regions..       
-0000d130: 2073 656c 662e 7472 616e 7363 7269 7074   self.transcript
-0000d140: 7320 3d20 7472 616e 7363 7269 7074 730d  s = transcripts.
-0000d150: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-0000d160: 726d 6174 203d 2066 6f72 6d61 740d 0a20  rmat = format.. 
-0000d170: 2020 2020 2020 2073 656c 662e 7469 6d65         self.time
-0000d180: 645f 7375 6274 6974 6c65 7320 3d20 5b28  d_subtitles = [(
-0000d190: 722c 2074 2920 666f 7220 722c 2074 2069  r, t) for r, t i
-0000d1a0: 6e20 7a69 7028 7365 6c66 2e72 6567 696f  n zip(self.regio
-0000d1b0: 6e73 2c20 7365 6c66 2e74 7261 6e73 6372  ns, self.transcr
-0000d1c0: 6970 7473 2920 6966 2074 5d0d 0a20 2020  ipts) if t]..   
-0000d1d0: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
-0000d1e0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-0000d1f0: 6b20 3d20 6572 726f 725f 6d65 7373 6167  k = error_messag
-0000d200: 6573 5f63 616c 6c62 6163 6b0d 0a0d 0a20  es_callback.... 
-0000d210: 2020 2064 6566 2067 6574 5f74 696d 6564     def get_timed
-0000d220: 5f73 7562 7469 746c 6573 2873 656c 6629  _subtitles(self)
-0000d230: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-0000d240: 6e20 7365 6c66 2e74 696d 6564 5f73 7562  n self.timed_sub
-0000d250: 7469 746c 6573 0d0a 0d0a 2020 2020 6465  titles....    de
-0000d260: 6620 7772 6974 6528 7365 6c66 2c20 6465  f write(self, de
-0000d270: 636c 6172 6564 5f73 7562 7469 746c 655f  clared_subtitle_
-0000d280: 6669 6c65 7061 7468 293a 0d0a 2020 2020  filepath):..    
-0000d290: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-0000d2a0: 2020 2020 2020 666f 726d 6174 7465 7220        formatter 
-0000d2b0: 3d20 5375 6274 6974 6c65 466f 726d 6174  = SubtitleFormat
-0000d2c0: 7465 7228 7365 6c66 2e66 6f72 6d61 7429  ter(self.format)
-0000d2d0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-0000d2e0: 726d 6174 7465 645f 7375 6274 6974 6c65  rmatted_subtitle
-0000d2f0: 7320 3d20 666f 726d 6174 7465 7228 7365  s = formatter(se
-0000d300: 6c66 2e74 696d 6564 5f73 7562 7469 746c  lf.timed_subtitl
-0000d310: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
-0000d320: 2073 6176 6564 5f73 7562 7469 746c 655f   saved_subtitle_
-0000d330: 6669 6c65 7061 7468 203d 2064 6563 6c61  filepath = decla
-0000d340: 7265 645f 7375 6274 6974 6c65 5f66 696c  red_subtitle_fil
-0000d350: 6570 6174 680d 0a20 2020 2020 2020 2020  epath..         
-0000d360: 2020 2069 6620 7361 7665 645f 7375 6274     if saved_subt
-0000d370: 6974 6c65 5f66 696c 6570 6174 683a 0d0a  itle_filepath:..
-0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d390: 7375 6274 6974 6c65 5f66 696c 655f 6261  subtitle_file_ba
-0000d3a0: 7365 2c20 7375 6274 6974 6c65 5f66 696c  se, subtitle_fil
-0000d3b0: 655f 6578 7420 3d20 6f73 2e70 6174 682e  e_ext = os.path.
-0000d3c0: 7370 6c69 7465 7874 2873 6176 6564 5f73  splitext(saved_s
-0000d3d0: 7562 7469 746c 655f 6669 6c65 7061 7468  ubtitle_filepath
-0000d3e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000d3f0: 2020 2069 6620 6e6f 7420 7375 6274 6974     if not subtit
-0000d400: 6c65 5f66 696c 655f 6578 743a 0d0a 2020  le_file_ext:..  
-0000d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d420: 2020 7361 7665 645f 7375 6274 6974 6c65    saved_subtitle
-0000d430: 5f66 696c 6570 6174 6820 3d20 227b 6261  _filepath = "{ba
-0000d440: 7365 7d2e 7b66 6f72 6d61 747d 222e 666f  se}.{format}".fo
-0000d450: 726d 6174 2862 6173 653d 7375 6274 6974  rmat(base=subtit
-0000d460: 6c65 5f66 696c 655f 6261 7365 2c20 666f  le_file_base, fo
-0000d470: 726d 6174 3d73 656c 662e 666f 726d 6174  rmat=self.format
-0000d480: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000d490: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0000d4a0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-0000d4b0: 7665 645f 7375 6274 6974 6c65 5f66 696c  ved_subtitle_fil
-0000d4c0: 6570 6174 6820 3d20 6465 636c 6172 6564  epath = declared
-0000d4d0: 5f73 7562 7469 746c 655f 6669 6c65 7061  _subtitle_filepa
-0000d4e0: 7468 0d0a 2020 2020 2020 2020 2020 2020  th..            
-0000d4f0: 7769 7468 206f 7065 6e28 7361 7665 645f  with open(saved_
-0000d500: 7375 6274 6974 6c65 5f66 696c 6570 6174  subtitle_filepat
-0000d510: 682c 2027 7762 2729 2061 7320 663a 0d0a  h, 'wb') as f:..
+0000a670: 2020 2020 2020 2020 2775 6b27 3a20 2755          'uk': 'U
+0000a680: 6b72 6169 6e69 616e 272c 0d0a 2020 2020  krainian',..    
+0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6a0: 2020 2020 2775 7227 3a20 2755 7264 7527      'ur': 'Urdu'
+0000a6b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000a6c0: 2020 2020 2020 2020 2020 2027 7567 273a             'ug':
+0000a6d0: 2027 5579 6768 7572 272c 0d0a 2020 2020   'Uyghur',..    
+0000a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6f0: 2020 2020 2775 7a27 3a20 2755 7a62 656b      'uz': 'Uzbek
+0000a700: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+0000a710: 2020 2020 2020 2020 2020 2020 2776 6927              'vi'
+0000a720: 3a20 2756 6965 746e 616d 6573 6527 2c0d  : 'Vietnamese',.
+0000a730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a740: 2020 2020 2020 2020 2027 6379 273a 2027           'cy': '
+0000a750: 5765 6c73 6827 2c0d 0a20 2020 2020 2020  Welsh',..       
+0000a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a770: 2027 7868 273a 2027 5868 6f73 6127 2c0d   'xh': 'Xhosa',.
+0000a780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a790: 2020 2020 2020 2020 2027 7969 273a 2027           'yi': '
+0000a7a0: 5969 6464 6973 6827 2c0d 0a20 2020 2020  Yiddish',..     
+0000a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7c0: 2020 2027 796f 273a 2027 596f 7275 6261     'yo': 'Yoruba
+0000a7d0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+0000a7e0: 2020 2020 2020 2020 2020 2020 277a 7527              'zu'
+0000a7f0: 3a20 275a 756c 7527 2c0d 0a20 2020 2020  : 'Zulu',..     
+0000a800: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+0000a810: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
+0000a820: 6e61 6d65 2873 656c 662c 2067 6574 5f63  name(self, get_c
+0000a830: 6f64 6529 3a0d 0a20 2020 2020 2020 2072  ode):..        r
+0000a840: 6574 7572 6e20 7365 6c66 2e64 6963 742e  eturn self.dict.
+0000a850: 6765 7428 6765 745f 636f 6465 2e6c 6f77  get(get_code.low
+0000a860: 6572 2829 2c20 2222 290d 0a0d 0a20 2020  er(), "")....   
+0000a870: 2064 6566 2067 6574 5f63 6f64 6528 7365   def get_code(se
+0000a880: 6c66 2c20 6c61 6e67 7561 6765 293a 0d0a  lf, language):..
+0000a890: 2020 2020 2020 2020 666f 7220 6765 745f          for get_
+0000a8a0: 636f 6465 2c20 6c61 6e67 2069 6e20 7365  code, lang in se
+0000a8b0: 6c66 2e64 6963 742e 6974 656d 7328 293a  lf.dict.items():
+0000a8c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000a8d0: 206c 616e 672e 6c6f 7765 7228 2920 3d3d   lang.lower() ==
+0000a8e0: 206c 616e 6775 6167 652e 6c6f 7765 7228   language.lower(
+0000a8f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000a900: 2020 2020 7265 7475 726e 2067 6574 5f63      return get_c
+0000a910: 6f64 650d 0a20 2020 2020 2020 2072 6574  ode..        ret
+0000a920: 7572 6e20 2222 0d0a 0d0a 0d0a 636c 6173  urn ""......clas
+0000a930: 7320 5761 7643 6f6e 7665 7274 6572 3a0d  s WavConverter:.
+0000a940: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+0000a950: 6f64 0d0a 2020 2020 6465 6620 7768 6963  od..    def whic
+0000a960: 6828 7072 6f67 7261 6d29 3a0d 0a20 2020  h(program):..   
+0000a970: 2020 2020 2064 6566 2069 735f 6578 6528       def is_exe(
+0000a980: 6669 6c65 5f70 6174 6829 3a0d 0a20 2020  file_path):..   
+0000a990: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000a9a0: 6f73 2e70 6174 682e 6973 6669 6c65 2866  os.path.isfile(f
+0000a9b0: 696c 655f 7061 7468 2920 616e 6420 6f73  ile_path) and os
+0000a9c0: 2e61 6363 6573 7328 6669 6c65 5f70 6174  .access(file_pat
+0000a9d0: 682c 206f 732e 585f 4f4b 290d 0a20 2020  h, os.X_OK)..   
+0000a9e0: 2020 2020 2066 7061 7468 2c20 5f20 3d20       fpath, _ = 
+0000a9f0: 6f73 2e70 6174 682e 7370 6c69 7428 7072  os.path.split(pr
+0000aa00: 6f67 7261 6d29 0d0a 2020 2020 2020 2020  ogram)..        
+0000aa10: 6966 2066 7061 7468 3a0d 0a20 2020 2020  if fpath:..     
+0000aa20: 2020 2020 2020 2069 6620 6973 5f65 7865         if is_exe
+0000aa30: 2870 726f 6772 616d 293a 0d0a 2020 2020  (program):..    
+0000aa40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000aa50: 726e 2070 726f 6772 616d 0d0a 2020 2020  rn program..    
+0000aa60: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0000aa70: 2020 2020 2020 2066 6f72 2070 6174 6820         for path 
+0000aa80: 696e 206f 732e 656e 7669 726f 6e5b 2250  in os.environ["P
+0000aa90: 4154 4822 5d2e 7370 6c69 7428 6f73 2e70  ATH"].split(os.p
+0000aaa0: 6174 6873 6570 293a 0d0a 2020 2020 2020  athsep):..      
+0000aab0: 2020 2020 2020 2020 2020 7061 7468 203d            path =
+0000aac0: 2070 6174 682e 7374 7269 7028 2722 2729   path.strip('"')
+0000aad0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000aae0: 2020 6578 655f 6669 6c65 203d 206f 732e    exe_file = os.
+0000aaf0: 7061 7468 2e6a 6f69 6e28 7061 7468 2c20  path.join(path, 
+0000ab00: 7072 6f67 7261 6d29 0d0a 2020 2020 2020  program)..      
+0000ab10: 2020 2020 2020 2020 2020 6966 2069 735f            if is_
+0000ab20: 6578 6528 6578 655f 6669 6c65 293a 0d0a  exe(exe_file):..
+0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab40: 2020 2020 7265 7475 726e 2065 7865 5f66      return exe_f
+0000ab50: 696c 650d 0a20 2020 2020 2020 2072 6574  ile..        ret
+0000ab60: 7572 6e20 4e6f 6e65 0d0a 0d0a 2020 2020  urn None....    
+0000ab70: 4073 7461 7469 636d 6574 686f 640d 0a20  @staticmethod.. 
+0000ab80: 2020 2064 6566 2066 666d 7065 675f 6368     def ffmpeg_ch
+0000ab90: 6563 6b28 293a 0d0a 2020 2020 2020 2020  eck():..        
+0000aba0: 6966 2057 6176 436f 6e76 6572 7465 722e  if WavConverter.
+0000abb0: 7768 6963 6828 2266 666d 7065 6722 293a  which("ffmpeg"):
+0000abc0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000abd0: 7475 726e 2022 6666 6d70 6567 220d 0a20  turn "ffmpeg".. 
+0000abe0: 2020 2020 2020 2069 6620 5761 7643 6f6e         if WavCon
+0000abf0: 7665 7274 6572 2e77 6869 6368 2822 6666  verter.which("ff
+0000ac00: 6d70 6567 2e65 7865 2229 3a0d 0a20 2020  mpeg.exe"):..   
+0000ac10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000ac20: 2266 666d 7065 672e 6578 6522 0d0a 2020  "ffmpeg.exe"..  
+0000ac30: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+0000ac40: 650d 0a0d 0a20 2020 2064 6566 205f 5f69  e....    def __i
+0000ac50: 6e69 745f 5f28 7365 6c66 2c20 6368 616e  nit__(self, chan
+0000ac60: 6e65 6c73 3d31 2c20 7261 7465 3d34 3830  nels=1, rate=480
+0000ac70: 3030 2c20 7072 6f67 7265 7373 5f63 616c  00, progress_cal
+0000ac80: 6c62 6163 6b3d 4e6f 6e65 2c20 6572 726f  lback=None, erro
+0000ac90: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000aca0: 6163 6b3d 4e6f 6e65 293a 0d0a 2020 2020  ack=None):..    
+0000acb0: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+0000acc0: 7320 3d20 6368 616e 6e65 6c73 0d0a 2020  s = channels..  
+0000acd0: 2020 2020 2020 7365 6c66 2e72 6174 6520        self.rate 
+0000ace0: 3d20 7261 7465 0d0a 2020 2020 2020 2020  = rate..        
+0000acf0: 7365 6c66 2e70 726f 6772 6573 735f 6361  self.progress_ca
+0000ad00: 6c6c 6261 636b 203d 2070 726f 6772 6573  llback = progres
+0000ad10: 735f 6361 6c6c 6261 636b 0d0a 2020 2020  s_callback..    
+0000ad20: 2020 2020 7365 6c66 2e65 7272 6f72 5f6d      self.error_m
+0000ad30: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+0000ad40: 203d 2065 7272 6f72 5f6d 6573 7361 6765   = error_message
+0000ad50: 735f 6361 6c6c 6261 636b 0d0a 0d0a 2020  s_callback....  
+0000ad60: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2873    def __call__(s
+0000ad70: 656c 662c 206d 6564 6961 5f66 696c 6570  elf, media_filep
+0000ad80: 6174 6829 3a0d 0a20 2020 2020 2020 2074  ath):..        t
+0000ad90: 656d 7020 3d20 7465 6d70 6669 6c65 2e4e  emp = tempfile.N
+0000ada0: 616d 6564 5465 6d70 6f72 6172 7946 696c  amedTemporaryFil
+0000adb0: 6528 7375 6666 6978 3d27 2e77 6176 272c  e(suffix='.wav',
+0000adc0: 2064 656c 6574 653d 4661 6c73 6529 0d0a   delete=False)..
+0000add0: 2020 2020 2020 2020 6966 206e 6f74 206f          if not o
+0000ade0: 732e 7061 7468 2e69 7366 696c 6528 6d65  s.path.isfile(me
+0000adf0: 6469 615f 6669 6c65 7061 7468 293a 0d0a  dia_filepath):..
+0000ae00: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000ae10: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
+0000ae20: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
+0000ae30: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ae40: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
+0000ae50: 735f 6361 6c6c 6261 636b 2822 5468 6520  s_callback("The 
+0000ae60: 6769 7665 6e20 6669 6c65 2064 6f65 7320  given file does 
+0000ae70: 6e6f 7420 6578 6973 743a 207b 307d 222e  not exist: {0}".
+0000ae80: 666f 726d 6174 286d 6564 6961 5f66 696c  format(media_fil
+0000ae90: 6570 6174 6829 290d 0a20 2020 2020 2020  epath))..       
+0000aea0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000aeb0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000aec0: 7428 2254 6865 2067 6976 656e 2066 696c  t("The given fil
+0000aed0: 6520 646f 6573 206e 6f74 2065 7869 7374  e does not exist
+0000aee0: 3a20 7b30 7d22 2e66 6f72 6d61 7428 6d65  : {0}".format(me
+0000aef0: 6469 615f 6669 6c65 7061 7468 2929 0d0a  dia_filepath))..
+0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af10: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+0000af20: 2249 6e76 616c 6964 2066 696c 653a 207b  "Invalid file: {
+0000af30: 307d 222e 666f 726d 6174 286d 6564 6961  0}".format(media
+0000af40: 5f66 696c 6570 6174 6829 290d 0a20 2020  _filepath))..   
+0000af50: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+0000af60: 2e66 666d 7065 675f 6368 6563 6b28 293a  .ffmpeg_check():
+0000af70: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000af80: 2073 656c 662e 6572 726f 725f 6d65 7373   self.error_mess
+0000af90: 6167 6573 5f63 616c 6c62 6163 6b3a 0d0a  ages_callback:..
+0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afb0: 7365 6c66 2e65 7272 6f72 5f6d 6573 7361  self.error_messa
+0000afc0: 6765 735f 6361 6c6c 6261 636b 2822 6666  ges_callback("ff
+0000afd0: 6d70 6567 3a20 4578 6563 7574 6162 6c65  mpeg: Executable
+0000afe0: 206e 6f74 2066 6f75 6e64 206f 6e20 6d61   not found on ma
+0000aff0: 6368 696e 652e 2229 0d0a 2020 2020 2020  chine.")..      
+0000b000: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0000b010: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+0000b020: 6e74 2822 6666 6d70 6567 3a20 4578 6563  nt("ffmpeg: Exec
+0000b030: 7574 6162 6c65 206e 6f74 2066 6f75 6e64  utable not found
+0000b040: 206f 6e20 6d61 6368 696e 652e 2229 0d0a   on machine.")..
+0000b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b060: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+0000b070: 2244 6570 656e 6465 6e63 7920 6e6f 7420  "Dependency not 
+0000b080: 666f 756e 643a 2066 666d 7065 6722 290d  found: ffmpeg").
+0000b090: 0a0d 0a20 2020 2020 2020 2063 6f6d 6d61  ...        comma
+0000b0a0: 6e64 203d 205b 0d0a 2020 2020 2020 2020  nd = [..        
+0000b0b0: 2020 2020 2020 2020 2020 2020 2266 666d              "ffm
+0000b0c0: 7065 6722 2c0d 0a20 2020 2020 2020 2020  peg",..         
+0000b0d0: 2020 2020 2020 2020 2020 2022 2d79 222c             "-y",
+0000b0e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b0f0: 2020 2020 2020 222d 6922 2c20 6d65 6469        "-i", medi
+0000b100: 615f 6669 6c65 7061 7468 2c0d 0a20 2020  a_filepath,..   
+0000b110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b120: 2022 2d61 6322 2c20 7374 7228 7365 6c66   "-ac", str(self
+0000b130: 2e63 6861 6e6e 656c 7329 2c0d 0a20 2020  .channels),..   
+0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b150: 2022 2d61 7222 2c20 7374 7228 7365 6c66   "-ar", str(self
+0000b160: 2e72 6174 6529 2c0d 0a20 2020 2020 2020  .rate),..       
+0000b170: 2020 2020 2020 2020 2020 2020 2022 2d6c               "-l
+0000b180: 6f67 6c65 7665 6c22 2c20 2265 7272 6f72  oglevel", "error
+0000b190: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0000b1a0: 2020 2020 2020 2020 222d 6869 6465 5f62          "-hide_b
+0000b1b0: 616e 6e65 7222 2c0d 0a20 2020 2020 2020  anner",..       
+0000b1c0: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000b1d0: 702e 6e61 6d65 0d0a 2020 2020 2020 2020  p.name..        
+0000b1e0: 2020 2020 2020 2020 2020 5d0d 0a0d 0a20            ].... 
+0000b1f0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+0000b200: 2020 2020 2020 2020 2023 2052 554e 4e49           # RUNNI
+0000b210: 4e47 2066 666d 7065 6720 5749 5448 4f55  NG ffmpeg WITHOU
+0000b220: 5420 5348 4f57 494e 4720 5052 4f47 5245  T SHOWING PROGRE
+0000b230: 5353 530d 0a20 2020 2020 2020 2020 2020  SSS..           
+0000b240: 2023 7573 655f 7368 656c 6c20 3d20 5472   #use_shell = Tr
+0000b250: 7565 2069 6620 6f73 2e6e 616d 6520 3d3d  ue if os.name ==
+0000b260: 2022 6e74 2220 656c 7365 2046 616c 7365   "nt" else False
+0000b270: 0d0a 2020 2020 2020 2020 2020 2020 2373  ..            #s
+0000b280: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
+0000b290: 6f75 7470 7574 2863 6f6d 6d61 6e64 2c20  output(command, 
+0000b2a0: 7374 6469 6e3d 6f70 656e 286f 732e 6465  stdin=open(os.de
+0000b2b0: 766e 756c 6c29 2c20 7368 656c 6c3d 7573  vnull), shell=us
+0000b2c0: 655f 7368 656c 6c29 0d0a 0d0a 2020 2020  e_shell)....    
+0000b2d0: 2020 2020 2020 2020 2320 5255 4e4e 494e          # RUNNIN
+0000b2e0: 4720 6666 6d70 6567 2057 4954 4820 5052  G ffmpeg WITH PR
+0000b2f0: 4f47 5245 5353 530d 0a20 2020 2020 2020  OGRESSS..       
+0000b300: 2020 2020 2066 6620 3d20 4666 6d70 6567       ff = Ffmpeg
+0000b310: 5072 6f67 7265 7373 2863 6f6d 6d61 6e64  Progress(command
+0000b320: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
+0000b330: 6572 6365 6e74 6167 6520 3d20 300d 0a20  ercentage = 0.. 
+0000b340: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
+0000b350: 726f 6772 6573 7320 696e 2066 662e 7275  rogress in ff.ru
+0000b360: 6e5f 636f 6d6d 616e 645f 7769 7468 5f70  n_command_with_p
+0000b370: 726f 6772 6573 7328 293a 0d0a 2020 2020  rogress():..    
+0000b380: 2020 2020 2020 2020 2020 2020 7065 7263              perc
+0000b390: 656e 7461 6765 203d 2070 726f 6772 6573  entage = progres
+0000b3a0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+0000b3b0: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
+0000b3c0: 6573 735f 6361 6c6c 6261 636b 3a0d 0a20  ess_callback:.. 
+0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3e0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+0000b3f0: 5f63 616c 6c62 6163 6b28 6d65 6469 615f  _callback(media_
+0000b400: 6669 6c65 7061 7468 2c20 7065 7263 656e  filepath, percen
+0000b410: 7461 6765 290d 0a20 2020 2020 2020 2020  tage)..         
+0000b420: 2020 2074 656d 702e 636c 6f73 6528 290d     temp.close().
+0000b430: 0a0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
+0000b440: 6574 7572 6e20 7465 6d70 2e6e 616d 652c  eturn temp.name,
+0000b450: 2073 656c 662e 7261 7465 0d0a 0d0a 2020   self.rate....  
+0000b460: 2020 2020 2020 6578 6365 7074 204b 6579        except Key
+0000b470: 626f 6172 6449 6e74 6572 7275 7074 3a0d  boardInterrupt:.
+0000b480: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000b490: 7365 6c66 2e65 7272 6f72 5f6d 6573 7361  self.error_messa
+0000b4a0: 6765 735f 6361 6c6c 6261 636b 3a0d 0a20  ges_callback:.. 
+0000b4b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b4c0: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
+0000b4d0: 6573 5f63 616c 6c62 6163 6b28 2243 616e  es_callback("Can
+0000b4e0: 6365 6c6c 696e 6720 616c 6c20 7461 736b  celling all task
+0000b4f0: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
+0000b500: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0000b510: 2020 2020 2020 2020 7072 696e 7428 2243          print("C
+0000b520: 616e 6365 6c6c 696e 6720 616c 6c20 7461  ancelling all ta
+0000b530: 736b 7322 290d 0a20 2020 2020 2020 2020  sks")..         
+0000b540: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
+0000b550: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+0000b560: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
+0000b570: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000b580: 2e65 7272 6f72 5f6d 6573 7361 6765 735f  .error_messages_
+0000b590: 6361 6c6c 6261 636b 3a0d 0a20 2020 2020  callback:..     
+0000b5a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b5b0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+0000b5c0: 616c 6c62 6163 6b28 6529 0d0a 2020 2020  allback(e)..    
+0000b5d0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0000b5e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000b5f0: 7269 6e74 2865 290d 0a20 2020 2020 2020  rint(e)..       
+0000b600: 2020 2020 2072 6574 7572 6e0d 0a0d 0a0d       return.....
+0000b610: 0a63 6c61 7373 2053 656e 7465 6e63 6554  .class SentenceT
+0000b620: 7261 6e73 6c61 746f 7228 6f62 6a65 6374  ranslator(object
+0000b630: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
+0000b640: 6974 5f5f 2873 656c 662c 2073 7263 2c20  it__(self, src, 
+0000b650: 6473 742c 2070 6174 6965 6e63 653d 2d31  dst, patience=-1
+0000b660: 2c20 7469 6d65 6f75 743d 3330 2c20 6572  , timeout=30, er
+0000b670: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+0000b680: 6c62 6163 6b3d 4e6f 6e65 293a 0d0a 2020  lback=None):..  
+0000b690: 2020 2020 2020 7365 6c66 2e73 7263 203d        self.src =
+0000b6a0: 2073 7263 0d0a 2020 2020 2020 2020 7365   src..        se
+0000b6b0: 6c66 2e64 7374 203d 2064 7374 0d0a 2020  lf.dst = dst..  
+0000b6c0: 2020 2020 2020 7365 6c66 2e70 6174 6965        self.patie
+0000b6d0: 6e63 6520 3d20 7061 7469 656e 6365 0d0a  nce = patience..
+0000b6e0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+0000b6f0: 656f 7574 203d 2074 696d 656f 7574 0d0a  eout = timeout..
+0000b700: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
+0000b710: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000b720: 6261 636b 203d 2065 7272 6f72 5f6d 6573  back = error_mes
+0000b730: 7361 6765 735f 6361 6c6c 6261 636b 0d0a  sages_callback..
+0000b740: 0d0a 2020 2020 6465 6620 5f5f 6361 6c6c  ..    def __call
+0000b750: 5f5f 2873 656c 662c 2073 656e 7465 6e63  __(self, sentenc
+0000b760: 6529 3a0d 0a20 2020 2020 2020 2074 7279  e):..        try
+0000b770: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+0000b780: 7261 6e73 6c61 7465 645f 7365 6e74 656e  ranslated_senten
+0000b790: 6365 203d 205b 5d0d 0a20 2020 2020 2020  ce = []..       
+0000b7a0: 2020 2020 2023 2068 616e 646c 6520 7468       # handle th
+0000b7b0: 6520 7370 6563 6961 6c20 6361 7365 3a20  e special case: 
+0000b7c0: 656d 7074 7920 7374 7269 6e67 2e0d 0a20  empty string... 
+0000b7d0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0000b7e0: 7420 7365 6e74 656e 6365 3a0d 0a20 2020  t sentence:..   
+0000b7f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000b800: 7572 6e20 4e6f 6e65 0d0a 2020 2020 2020  urn None..      
+0000b810: 2020 2020 2020 7472 616e 736c 6174 6564        translated
+0000b820: 5f73 656e 7465 6e63 6520 3d20 7365 6c66  _sentence = self
+0000b830: 2e47 6f6f 676c 6554 7261 6e73 6c61 7465  .GoogleTranslate
+0000b840: 2873 656e 7465 6e63 652c 2073 7263 3d73  (sentence, src=s
+0000b850: 656c 662e 7372 632c 2064 7374 3d73 656c  elf.src, dst=sel
+0000b860: 662e 6473 742c 2074 696d 656f 7574 3d73  f.dst, timeout=s
+0000b870: 656c 662e 7469 6d65 6f75 7429 0d0a 2020  elf.timeout)..  
+0000b880: 2020 2020 2020 2020 2020 6661 696c 5f74            fail_t
+0000b890: 6f5f 7472 616e 736c 6174 6520 3d20 7472  o_translate = tr
+0000b8a0: 616e 736c 6174 6564 5f73 656e 7465 6e63  anslated_sentenc
+0000b8b0: 655b 2d31 5d20 3d3d 2027 5c6e 270d 0a20  e[-1] == '\n'.. 
+0000b8c0: 2020 2020 2020 2020 2020 2077 6869 6c65             while
+0000b8d0: 2066 6169 6c5f 746f 5f74 7261 6e73 6c61   fail_to_transla
+0000b8e0: 7465 2061 6e64 2070 6174 6965 6e63 653a  te and patience:
+0000b8f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b900: 2020 7472 616e 736c 6174 6564 5f73 656e    translated_sen
+0000b910: 7465 6e63 6520 3d20 7365 6c66 2e47 6f6f  tence = self.Goo
+0000b920: 676c 6554 7261 6e73 6c61 7465 2874 7261  gleTranslate(tra
+0000b930: 6e73 6c61 7465 645f 7365 6e74 656e 6365  nslated_sentence
+0000b940: 2c20 7372 633d 7365 6c66 2e73 7263 2c20  , src=self.src, 
+0000b950: 6473 743d 7365 6c66 2e64 7374 2c20 7469  dst=self.dst, ti
+0000b960: 6d65 6f75 743d 7365 6c66 2e74 696d 656f  meout=self.timeo
+0000b970: 7574 292e 7465 7874 0d0a 2020 2020 2020  ut).text..      
+0000b980: 2020 2020 2020 2020 2020 6966 2074 7261            if tra
+0000b990: 6e73 6c61 7465 645f 7365 6e74 656e 6365  nslated_sentence
+0000b9a0: 5b2d 315d 203d 3d20 275c 6e27 3a0d 0a20  [-1] == '\n':.. 
+0000b9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9c0: 2020 2069 6620 7061 7469 656e 6365 203d     if patience =
+0000b9d0: 3d20 2d31 3a0d 0a20 2020 2020 2020 2020  = -1:..         
+0000b9e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000b9f0: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
+0000ba00: 2020 2020 2020 2020 2020 2020 2070 6174               pat
+0000ba10: 6965 6e63 6520 2d3d 2031 0d0a 2020 2020  ience -= 1..    
+0000ba20: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000ba30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000ba40: 2020 2020 2020 2066 6169 6c5f 746f 5f74         fail_to_t
+0000ba50: 7261 6e73 6c61 7465 203d 2046 616c 7365  ranslate = False
+0000ba60: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000ba70: 7265 7475 726e 2074 7261 6e73 6c61 7465  return translate
+0000ba80: 645f 7365 6e74 656e 6365 0d0a 0d0a 2020  d_sentence....  
+0000ba90: 2020 2020 2020 6578 6365 7074 204b 6579        except Key
+0000baa0: 626f 6172 6449 6e74 6572 7275 7074 3a0d  boardInterrupt:.
+0000bab0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000bac0: 7365 6c66 2e65 7272 6f72 5f6d 6573 7361  self.error_messa
+0000bad0: 6765 735f 6361 6c6c 6261 636b 3a0d 0a20  ges_callback:.. 
+0000bae0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000baf0: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
+0000bb00: 6573 5f63 616c 6c62 6163 6b28 2243 616e  es_callback("Can
+0000bb10: 6365 6c6c 696e 6720 616c 6c20 7461 736b  celling all task
+0000bb20: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
+0000bb30: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0000bb40: 2020 2020 2020 2020 7072 696e 7428 2243          print("C
+0000bb50: 616e 6365 6c6c 696e 6720 616c 6c20 7461  ancelling all ta
+0000bb60: 736b 7322 290d 0a20 2020 2020 2020 2020  sks")..         
+0000bb70: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
+0000bb80: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+0000bb90: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
+0000bba0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000bbb0: 2e65 7272 6f72 5f6d 6573 7361 6765 735f  .error_messages_
+0000bbc0: 6361 6c6c 6261 636b 3a0d 0a20 2020 2020  callback:..     
+0000bbd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000bbe0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+0000bbf0: 616c 6c62 6163 6b28 6529 0d0a 2020 2020  allback(e)..    
+0000bc00: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0000bc10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000bc20: 7269 6e74 2865 290d 0a20 2020 2020 2020  rint(e)..       
+0000bc30: 2020 2020 2072 6574 7572 6e0d 0a0d 0a20       return.... 
+0000bc40: 2020 2064 6566 2047 6f6f 676c 6554 7261     def GoogleTra
+0000bc50: 6e73 6c61 7465 2873 656c 662c 2074 6578  nslate(self, tex
+0000bc60: 742c 2073 7263 2c20 6473 742c 2074 696d  t, src, dst, tim
+0000bc70: 656f 7574 3d33 3029 3a0d 0a20 2020 2020  eout=30):..     
+0000bc80: 2020 2075 726c 203d 2027 6874 7470 733a     url = 'https:
+0000bc90: 2f2f 7472 616e 736c 6174 652e 676f 6f67  //translate.goog
+0000bca0: 6c65 6170 6973 2e63 6f6d 2f74 7261 6e73  leapis.com/trans
+0000bcb0: 6c61 7465 5f61 2f27 0d0a 2020 2020 2020  late_a/'..      
+0000bcc0: 2020 7061 7261 6d73 203d 2027 7369 6e67    params = 'sing
+0000bcd0: 6c65 3f63 6c69 656e 743d 6774 7826 736c  le?client=gtx&sl
+0000bce0: 3d27 2b73 7263 2b27 2674 6c3d 272b 6473  ='+src+'&tl='+ds
+0000bcf0: 742b 2726 6474 3d74 2671 3d27 2b74 6578  t+'&dt=t&q='+tex
+0000bd00: 743b 0d0a 2020 2020 2020 2020 6865 6164  t;..        head
+0000bd10: 6572 7320 3d20 7b27 5573 6572 2d41 6765  ers = {'User-Age
+0000bd20: 6e74 273a 2027 4d6f 7a69 6c6c 612f 352e  nt': 'Mozilla/5.
+0000bd30: 3020 2857 696e 646f 7773 204e 5420 3130  0 (Windows NT 10
+0000bd40: 2e30 3b20 5769 6e36 343b 2078 3634 2927  .0; Win64; x64)'
+0000bd50: 2c20 2752 6566 6572 6572 273a 2027 6874  , 'Referer': 'ht
+0000bd60: 7470 733a 2f2f 7472 616e 736c 6174 652e  tps://translate.
+0000bd70: 676f 6f67 6c65 2e63 6f6d 272c 7d0d 0a0d  google.com',}...
+0000bd80: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+0000bd90: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+0000bda0: 6e73 6520 3d20 7265 7175 6573 7473 2e67  nse = requests.g
+0000bdb0: 6574 2875 726c 2b70 6172 616d 732c 2068  et(url+params, h
+0000bdc0: 6561 6465 7273 3d68 6561 6465 7273 2c20  eaders=headers, 
+0000bdd0: 7469 6d65 6f75 743d 7365 6c66 2e74 696d  timeout=self.tim
+0000bde0: 656f 7574 290d 0a20 2020 2020 2020 2020  eout)..         
+0000bdf0: 2020 2069 6620 7265 7370 6f6e 7365 2e73     if response.s
+0000be00: 7461 7475 735f 636f 6465 203d 3d20 3230  tatus_code == 20
+0000be10: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+0000be20: 2020 2020 7265 7370 6f6e 7365 5f6a 736f      response_jso
+0000be30: 6e20 3d20 7265 7370 6f6e 7365 2e6a 736f  n = response.jso
+0000be40: 6e28 295b 305d 0d0a 2020 2020 2020 2020  n()[0]..        
+0000be50: 2020 2020 2020 2020 6c65 6e67 7468 203d          length =
+0000be60: 206c 656e 2872 6573 706f 6e73 655f 6a73   len(response_js
+0000be70: 6f6e 290d 0a20 2020 2020 2020 2020 2020  on)..           
+0000be80: 2020 2020 2074 7261 6e73 6c61 7469 6f6e       translation
+0000be90: 203d 2022 220d 0a20 2020 2020 2020 2020   = ""..         
+0000bea0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+0000beb0: 7261 6e67 6528 6c65 6e67 7468 293a 0d0a  range(length):..
+0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bed0: 2020 2020 7472 616e 736c 6174 696f 6e20      translation 
+0000bee0: 3d20 7472 616e 736c 6174 696f 6e20 2b20  = translation + 
+0000bef0: 7265 7370 6f6e 7365 5f6a 736f 6e5b 695d  response_json[i]
+0000bf00: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+0000bf10: 2020 2020 2072 6574 7572 6e20 7472 616e       return tran
+0000bf20: 736c 6174 696f 6e0d 0a20 2020 2020 2020  slation..       
+0000bf30: 2020 2020 2072 6574 7572 6e0d 0a0d 0a20       return.... 
+0000bf40: 2020 2020 2020 2065 7863 6570 7420 7265         except re
+0000bf50: 7175 6573 7473 2e65 7863 6570 7469 6f6e  quests.exception
+0000bf60: 732e 436f 6e6e 6563 7469 6f6e 4572 726f  s.ConnectionErro
+0000bf70: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+0000bf80: 7769 7468 2068 7474 7078 2e43 6c69 656e  with httpx.Clien
+0000bf90: 7428 2920 6173 2063 6c69 656e 743a 0d0a  t() as client:..
+0000bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfb0: 7265 7370 6f6e 7365 203d 2063 6c69 656e  response = clien
+0000bfc0: 742e 6765 7428 7572 6c2b 7061 7261 6d73  t.get(url+params
+0000bfd0: 2c20 6865 6164 6572 733d 6865 6164 6572  , headers=header
+0000bfe0: 732c 2074 696d 656f 7574 3d73 656c 662e  s, timeout=self.
+0000bff0: 7469 6d65 6f75 7429 0d0a 2020 2020 2020  timeout)..      
+0000c000: 2020 2020 2020 2020 2020 6966 2072 6573            if res
+0000c010: 706f 6e73 652e 7374 6174 7573 5f63 6f64  ponse.status_cod
+0000c020: 6520 3d3d 2032 3030 3a0d 0a20 2020 2020  e == 200:..     
+0000c030: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000c040: 6573 706f 6e73 655f 6a73 6f6e 203d 2072  esponse_json = r
+0000c050: 6573 706f 6e73 652e 6a73 6f6e 2829 5b30  esponse.json()[0
+0000c060: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000c070: 2020 2020 2020 206c 656e 6774 6820 3d20         length = 
+0000c080: 6c65 6e28 7265 7370 6f6e 7365 5f6a 736f  len(response_jso
+0000c090: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+0000c0a0: 2020 2020 2020 2020 7472 616e 736c 6174          translat
+0000c0b0: 696f 6e20 3d20 2222 0d0a 2020 2020 2020  ion = ""..      
+0000c0c0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000c0d0: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+0000c0e0: 6774 6829 3a0d 0a20 2020 2020 2020 2020  gth):..         
+0000c0f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000c100: 7261 6e73 6c61 7469 6f6e 203d 2074 7261  ranslation = tra
+0000c110: 6e73 6c61 7469 6f6e 202b 2072 6573 706f  nslation + respo
+0000c120: 6e73 655f 6a73 6f6e 5b69 5d5b 305d 0d0a  nse_json[i][0]..
+0000c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c140: 2020 2020 7265 7475 726e 2074 7261 6e73      return trans
+0000c150: 6c61 7469 6f6e 0d0a 2020 2020 2020 2020  lation..        
+0000c160: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+0000c170: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
+0000c180: 204b 6579 626f 6172 6449 6e74 6572 7275   KeyboardInterru
+0000c190: 7074 3a0d 0a20 2020 2020 2020 2020 2020  pt:..           
+0000c1a0: 2069 6620 7365 6c66 2e65 7272 6f72 5f6d   if self.error_m
+0000c1b0: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+0000c1c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000c1d0: 2020 2073 656c 662e 6572 726f 725f 6d65     self.error_me
+0000c1e0: 7373 6167 6573 5f63 616c 6c62 6163 6b28  ssages_callback(
+0000c1f0: 2243 616e 6365 6c6c 696e 6720 616c 6c20  "Cancelling all 
+0000c200: 7461 736b 7322 290d 0a20 2020 2020 2020  tasks")..       
+0000c210: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000c220: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000c230: 7428 2243 616e 6365 6c6c 696e 6720 616c  t("Cancelling al
+0000c240: 6c20 7461 736b 7322 290d 0a20 2020 2020  l tasks")..     
+0000c250: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
+0000c260: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0000c270: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
+0000c280: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000c290: 7365 6c66 2e65 7272 6f72 5f6d 6573 7361  self.error_messa
+0000c2a0: 6765 735f 6361 6c6c 6261 636b 3a0d 0a20  ges_callback:.. 
+0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c2c0: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
+0000c2d0: 6573 5f63 616c 6c62 6163 6b28 6529 0d0a  es_callback(e)..
+0000c2e0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000c2f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000c300: 2020 2070 7269 6e74 2865 290d 0a20 2020     print(e)..   
+0000c310: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
+0000c320: 0a0d 0a0d 0a63 6c61 7373 2053 7562 7469  .....class Subti
+0000c330: 746c 6546 6f72 6d61 7474 6572 3a0d 0a20  tleFormatter:.. 
+0000c340: 2020 2073 7570 706f 7274 6564 5f66 6f72     supported_for
+0000c350: 6d61 7473 203d 205b 2773 7274 272c 2027  mats = ['srt', '
+0000c360: 7674 7427 2c20 276a 736f 6e27 2c20 2772  vtt', 'json', 'r
+0000c370: 6177 275d 0d0a 0d0a 2020 2020 6465 6620  aw']....    def 
+0000c380: 5f5f 696e 6974 5f5f 2873 656c 662c 2066  __init__(self, f
+0000c390: 6f72 6d61 745f 7479 7065 2c20 6572 726f  ormat_type, erro
+0000c3a0: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000c3b0: 6163 6b3d 4e6f 6e65 293a 0d0a 2020 2020  ack=None):..    
+0000c3c0: 2020 2020 7365 6c66 2e66 6f72 6d61 745f      self.format_
+0000c3d0: 7479 7065 203d 2066 6f72 6d61 745f 7479  type = format_ty
+0000c3e0: 7065 2e6c 6f77 6572 2829 0d0a 2020 2020  pe.lower()..    
+0000c3f0: 2020 2020 7365 6c66 2e65 7272 6f72 5f6d      self.error_m
+0000c400: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+0000c410: 203d 2065 7272 6f72 5f6d 6573 7361 6765   = error_message
+0000c420: 735f 6361 6c6c 6261 636b 0d0a 2020 2020  s_callback..    
+0000c430: 2020 2020 0d0a 2020 2020 6465 6620 5f5f      ..    def __
+0000c440: 6361 6c6c 5f5f 2873 656c 662c 2073 7562  call__(self, sub
+0000c450: 7469 746c 6573 2c20 7061 6464 696e 675f  titles, padding_
+0000c460: 6265 666f 7265 3d30 2c20 7061 6464 696e  before=0, paddin
+0000c470: 675f 6166 7465 723d 3029 3a0d 0a20 2020  g_after=0):..   
+0000c480: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+0000c490: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
+0000c4a0: 6f72 6d61 745f 7479 7065 203d 3d20 2773  ormat_type == 's
+0000c4b0: 7274 273a 0d0a 2020 2020 2020 2020 2020  rt':..          
+0000c4c0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000c4d0: 662e 7372 745f 666f 726d 6174 7465 7228  f.srt_formatter(
+0000c4e0: 7375 6274 6974 6c65 732c 2070 6164 6469  subtitles, paddi
+0000c4f0: 6e67 5f62 6566 6f72 652c 2070 6164 6469  ng_before, paddi
+0000c500: 6e67 5f61 6674 6572 290d 0a20 2020 2020  ng_after)..     
+0000c510: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+0000c520: 2e66 6f72 6d61 745f 7479 7065 203d 3d20  .format_type == 
+0000c530: 2776 7474 273a 0d0a 2020 2020 2020 2020  'vtt':..        
+0000c540: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000c550: 656c 662e 7674 745f 666f 726d 6174 7465  elf.vtt_formatte
+0000c560: 7228 7375 6274 6974 6c65 732c 2070 6164  r(subtitles, pad
+0000c570: 6469 6e67 5f62 6566 6f72 652c 2070 6164  ding_before, pad
+0000c580: 6469 6e67 5f61 6674 6572 290d 0a20 2020  ding_after)..   
+0000c590: 2020 2020 2020 2020 2065 6c69 6620 7365           elif se
+0000c5a0: 6c66 2e66 6f72 6d61 745f 7479 7065 203d  lf.format_type =
+0000c5b0: 3d20 276a 736f 6e27 3a0d 0a20 2020 2020  = 'json':..     
+0000c5c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000c5d0: 6e20 7365 6c66 2e6a 736f 6e5f 666f 726d  n self.json_form
+0000c5e0: 6174 7465 7228 7375 6274 6974 6c65 7329  atter(subtitles)
+0000c5f0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+0000c600: 6966 2073 656c 662e 666f 726d 6174 5f74  if self.format_t
+0000c610: 7970 6520 3d3d 2027 7261 7727 3a0d 0a20  ype == 'raw':.. 
+0000c620: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000c630: 6574 7572 6e20 7365 6c66 2e72 6177 5f66  eturn self.raw_f
+0000c640: 6f72 6d61 7474 6572 2873 7562 7469 746c  ormatter(subtitl
+0000c650: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
+0000c660: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0000c670: 2020 2020 2020 2020 6966 2065 7272 6f72          if error
+0000c680: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000c690: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
+0000c6a0: 2020 2020 2020 2020 2065 7272 6f72 5f6d           error_m
+0000c6b0: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+0000c6c0: 2866 2755 6e73 7570 706f 7274 6564 2066  (f'Unsupported f
+0000c6d0: 6f72 6d61 7420 7479 7065 3a20 7b73 656c  ormat type: {sel
+0000c6e0: 662e 666f 726d 6174 5f74 7970 657d 2729  f.format_type}')
+0000c6f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c700: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0000c710: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+0000c720: 7365 2056 616c 7565 4572 726f 7228 6627  se ValueError(f'
+0000c730: 556e 7375 7070 6f72 7465 6420 666f 726d  Unsupported form
+0000c740: 6174 2074 7970 653a 207b 7365 6c66 2e66  at type: {self.f
+0000c750: 6f72 6d61 745f 7479 7065 7d27 290d 0a0d  ormat_type}')...
+0000c760: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0000c770: 4b65 7962 6f61 7264 496e 7465 7272 7570  KeyboardInterrup
+0000c780: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+0000c790: 6966 2073 656c 662e 6572 726f 725f 6d65  if self.error_me
+0000c7a0: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
+0000c7b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c7c0: 2020 7365 6c66 2e65 7272 6f72 5f6d 6573    self.error_mes
+0000c7d0: 7361 6765 735f 6361 6c6c 6261 636b 2822  sages_callback("
+0000c7e0: 4361 6e63 656c 6c69 6e67 2061 6c6c 2074  Cancelling all t
+0000c7f0: 6173 6b73 2229 0d0a 2020 2020 2020 2020  asks")..        
+0000c800: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0000c810: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000c820: 2822 4361 6e63 656c 6c69 6e67 2061 6c6c  ("Cancelling all
+0000c830: 2074 6173 6b73 2229 0d0a 2020 2020 2020   tasks")..      
+0000c840: 2020 2020 2020 7265 7475 726e 0d0a 0d0a        return....
+0000c850: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+0000c860: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
+0000c870: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000c880: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
+0000c890: 6573 5f63 616c 6c62 6163 6b3a 0d0a 2020  es_callback:..  
+0000c8a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000c8b0: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
+0000c8c0: 735f 6361 6c6c 6261 636b 2865 290d 0a20  s_callback(e).. 
+0000c8d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000c8e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c8f0: 2020 7072 696e 7428 6529 0d0a 2020 2020    print(e)..    
+0000c900: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+0000c910: 0d0a 2020 2020 6465 6620 7372 745f 666f  ..    def srt_fo
+0000c920: 726d 6174 7465 7228 7365 6c66 2c20 7375  rmatter(self, su
+0000c930: 6274 6974 6c65 732c 2070 6164 6469 6e67  btitles, padding
+0000c940: 5f62 6566 6f72 653d 302c 2070 6164 6469  _before=0, paddi
+0000c950: 6e67 5f61 6674 6572 3d30 293a 0d0a 2020  ng_after=0):..  
+0000c960: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0000c970: 2020 2053 6572 6961 6c69 7a65 2061 206c     Serialize a l
+0000c980: 6973 7420 6f66 2073 7562 7469 746c 6573  ist of subtitles
+0000c990: 2061 6363 6f72 6469 6e67 2074 6f20 7468   according to th
+0000c9a0: 6520 5352 5420 666f 726d 6174 2c20 7769  e SRT format, wi
+0000c9b0: 7468 206f 7074 696f 6e61 6c20 7469 6d65  th optional time
+0000c9c0: 2070 6164 6469 6e67 2e0d 0a20 2020 2020   padding...     
+0000c9d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+0000c9e0: 7375 625f 7269 705f 6669 6c65 203d 2070  sub_rip_file = p
+0000c9f0: 7973 7274 2e53 7562 5269 7046 696c 6528  ysrt.SubRipFile(
+0000ca00: 290d 0a20 2020 2020 2020 2066 6f72 2069  )..        for i
+0000ca10: 2c20 2828 7374 6172 742c 2065 6e64 292c  , ((start, end),
+0000ca20: 2074 6578 7429 2069 6e20 656e 756d 6572   text) in enumer
+0000ca30: 6174 6528 7375 6274 6974 6c65 732c 2073  ate(subtitles, s
+0000ca40: 7461 7274 3d31 293a 0d0a 2020 2020 2020  tart=1):..      
+0000ca50: 2020 2020 2020 6974 656d 203d 2070 7973        item = pys
+0000ca60: 7274 2e53 7562 5269 7049 7465 6d28 290d  rt.SubRipItem().
+0000ca70: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
+0000ca80: 6d2e 696e 6465 7820 3d20 690d 0a20 2020  m.index = i..   
+0000ca90: 2020 2020 2020 2020 2069 7465 6d2e 7465           item.te
+0000caa0: 7874 203d 2073 6978 2e74 6578 745f 7479  xt = six.text_ty
+0000cab0: 7065 2874 6578 7429 0d0a 2020 2020 2020  pe(text)..      
+0000cac0: 2020 2020 2020 6974 656d 2e73 7461 7274        item.start
+0000cad0: 2e73 6563 6f6e 6473 203d 206d 6178 2830  .seconds = max(0
+0000cae0: 2c20 7374 6172 7420 2d20 7061 6464 696e  , start - paddin
+0000caf0: 675f 6265 666f 7265 290d 0a20 2020 2020  g_before)..     
+0000cb00: 2020 2020 2020 2069 7465 6d2e 656e 642e         item.end.
+0000cb10: 7365 636f 6e64 7320 3d20 656e 6420 2b20  seconds = end + 
+0000cb20: 7061 6464 696e 675f 6166 7465 720d 0a20  padding_after.. 
+0000cb30: 2020 2020 2020 2020 2020 2073 7562 5f72             sub_r
+0000cb40: 6970 5f66 696c 652e 6170 7065 6e64 2869  ip_file.append(i
+0000cb50: 7465 6d29 0d0a 2020 2020 2020 2020 7265  tem)..        re
+0000cb60: 7475 726e 2027 5c6e 272e 6a6f 696e 2873  turn '\n'.join(s
+0000cb70: 6978 2e74 6578 745f 7479 7065 2869 7465  ix.text_type(ite
+0000cb80: 6d29 2066 6f72 2069 7465 6d20 696e 2073  m) for item in s
+0000cb90: 7562 5f72 6970 5f66 696c 6529 0d0a 0d0a  ub_rip_file)....
+0000cba0: 2020 2020 6465 6620 7674 745f 666f 726d      def vtt_form
+0000cbb0: 6174 7465 7228 7365 6c66 2c20 7375 6274  atter(self, subt
+0000cbc0: 6974 6c65 732c 2070 6164 6469 6e67 5f62  itles, padding_b
+0000cbd0: 6566 6f72 653d 302c 2070 6164 6469 6e67  efore=0, padding
+0000cbe0: 5f61 6674 6572 3d30 293a 0d0a 2020 2020  _after=0):..    
+0000cbf0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+0000cc00: 2053 6572 6961 6c69 7a65 2061 206c 6973   Serialize a lis
+0000cc10: 7420 6f66 2073 7562 7469 746c 6573 2061  t of subtitles a
+0000cc20: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
+0000cc30: 5654 5420 666f 726d 6174 2c20 7769 7468  VTT format, with
+0000cc40: 206f 7074 696f 6e61 6c20 7469 6d65 2070   optional time p
+0000cc50: 6164 6469 6e67 2e0d 0a20 2020 2020 2020  adding...       
+0000cc60: 2022 2222 0d0a 2020 2020 2020 2020 7465   """..        te
+0000cc70: 7874 203d 2073 656c 662e 7372 745f 666f  xt = self.srt_fo
+0000cc80: 726d 6174 7465 7228 7375 6274 6974 6c65  rmatter(subtitle
+0000cc90: 732c 2070 6164 6469 6e67 5f62 6566 6f72  s, padding_befor
+0000cca0: 652c 2070 6164 6469 6e67 5f61 6674 6572  e, padding_after
+0000ccb0: 290d 0a20 2020 2020 2020 2074 6578 7420  )..        text 
+0000ccc0: 3d20 2757 4542 5654 545c 6e5c 6e27 202b  = 'WEBVTT\n\n' +
+0000ccd0: 2074 6578 742e 7265 706c 6163 6528 272c   text.replace(',
+0000cce0: 272c 2027 2e27 290d 0a20 2020 2020 2020  ', '.')..       
+0000ccf0: 2072 6574 7572 6e20 7465 7874 0d0a 0d0a   return text....
+0000cd00: 2020 2020 6465 6620 6a73 6f6e 5f66 6f72      def json_for
+0000cd10: 6d61 7474 6572 2873 656c 662c 2073 7562  matter(self, sub
+0000cd20: 7469 746c 6573 293a 0d0a 2020 2020 2020  titles):..      
+0000cd30: 2020 2222 220d 0a20 2020 2020 2020 2053    """..        S
+0000cd40: 6572 6961 6c69 7a65 2061 206c 6973 7420  erialize a list 
+0000cd50: 6f66 2073 7562 7469 746c 6573 2061 7320  of subtitles as 
+0000cd60: 6120 4a53 4f4e 2062 6c6f 622e 0d0a 2020  a JSON blob...  
+0000cd70: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0000cd80: 2020 2073 7562 7469 746c 655f 6469 6374     subtitle_dict
+0000cd90: 7320 3d20 5b0d 0a20 2020 2020 2020 2020  s = [..         
+0000cda0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+0000cdb0: 2020 2020 2020 2773 7461 7274 273a 2073        'start': s
+0000cdc0: 7461 7274 2c0d 0a20 2020 2020 2020 2020  tart,..         
+0000cdd0: 2020 2020 2020 2027 656e 6427 3a20 656e         'end': en
+0000cde0: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
+0000cdf0: 2020 2020 2763 6f6e 7465 6e74 273a 2074      'content': t
+0000ce00: 6578 742c 0d0a 2020 2020 2020 2020 2020  ext,..          
+0000ce10: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
+0000ce20: 2066 6f72 2028 2873 7461 7274 2c20 656e   for ((start, en
+0000ce30: 6429 2c20 7465 7874 290d 0a20 2020 2020  d), text)..     
+0000ce40: 2020 2020 2020 2069 6e20 7375 6274 6974         in subtit
+0000ce50: 6c65 730d 0a20 2020 2020 2020 205d 0d0a  les..        ]..
+0000ce60: 2020 2020 2020 2020 7265 7475 726e 206a          return j
+0000ce70: 736f 6e2e 6475 6d70 7328 7375 6274 6974  son.dumps(subtit
+0000ce80: 6c65 5f64 6963 7473 290d 0a0d 0a20 2020  le_dicts)....   
+0000ce90: 2064 6566 2072 6177 5f66 6f72 6d61 7474   def raw_formatt
+0000cea0: 6572 2873 656c 662c 2073 7562 7469 746c  er(self, subtitl
+0000ceb0: 6573 293a 0d0a 2020 2020 2020 2020 2222  es):..        ""
+0000cec0: 220d 0a20 2020 2020 2020 2053 6572 6961  "..        Seria
+0000ced0: 6c69 7a65 2061 206c 6973 7420 6f66 2073  lize a list of s
+0000cee0: 7562 7469 746c 6573 2061 7320 6120 6e65  ubtitles as a ne
+0000cef0: 776c 696e 652d 6465 6c69 6d69 7465 6420  wline-delimited 
+0000cf00: 7374 7269 6e67 2e0d 0a20 2020 2020 2020  string...       
+0000cf10: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
+0000cf20: 7475 726e 2027 2027 2e6a 6f69 6e28 7465  turn ' '.join(te
+0000cf30: 7874 2066 6f72 2028 5f72 6e67 2c20 7465  xt for (_rng, te
+0000cf40: 7874 2920 696e 2073 7562 7469 746c 6573  xt) in subtitles
+0000cf50: 290d 0a0d 0a0d 0a63 6c61 7373 2053 7562  )......class Sub
+0000cf60: 7469 746c 6557 7269 7465 723a 0d0a 2020  titleWriter:..  
+0000cf70: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000cf80: 656c 662c 2072 6567 696f 6e73 2c20 7472  elf, regions, tr
+0000cf90: 616e 7363 7269 7074 732c 2066 6f72 6d61  anscripts, forma
+0000cfa0: 742c 2065 7272 6f72 5f6d 6573 7361 6765  t, error_message
+0000cfb0: 735f 6361 6c6c 6261 636b 3d4e 6f6e 6529  s_callback=None)
+0000cfc0: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
+0000cfd0: 7265 6769 6f6e 7320 3d20 7265 6769 6f6e  regions = region
+0000cfe0: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
+0000cff0: 7472 616e 7363 7269 7074 7320 3d20 7472  transcripts = tr
+0000d000: 616e 7363 7269 7074 730d 0a20 2020 2020  anscripts..     
+0000d010: 2020 2073 656c 662e 666f 726d 6174 203d     self.format =
+0000d020: 2066 6f72 6d61 740d 0a20 2020 2020 2020   format..       
+0000d030: 2073 656c 662e 7469 6d65 645f 7375 6274   self.timed_subt
+0000d040: 6974 6c65 7320 3d20 5b28 722c 2074 2920  itles = [(r, t) 
+0000d050: 666f 7220 722c 2074 2069 6e20 7a69 7028  for r, t in zip(
+0000d060: 7365 6c66 2e72 6567 696f 6e73 2c20 7365  self.regions, se
+0000d070: 6c66 2e74 7261 6e73 6372 6970 7473 2920  lf.transcripts) 
+0000d080: 6966 2074 5d0d 0a20 2020 2020 2020 2073  if t]..        s
+0000d090: 656c 662e 6572 726f 725f 6d65 7373 6167  elf.error_messag
+0000d0a0: 6573 5f63 616c 6c62 6163 6b20 3d20 6572  es_callback = er
+0000d0b0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+0000d0c0: 6c62 6163 6b0d 0a0d 0a20 2020 2064 6566  lback....    def
+0000d0d0: 2067 6574 5f74 696d 6564 5f73 7562 7469   get_timed_subti
+0000d0e0: 746c 6573 2873 656c 6629 3a0d 0a20 2020  tles(self):..   
+0000d0f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000d100: 2e74 696d 6564 5f73 7562 7469 746c 6573  .timed_subtitles
+0000d110: 0d0a 0d0a 2020 2020 6465 6620 7772 6974  ....    def writ
+0000d120: 6528 7365 6c66 2c20 6465 636c 6172 6564  e(self, declared
+0000d130: 5f73 7562 7469 746c 655f 6669 6c65 7061  _subtitle_filepa
+0000d140: 7468 293a 0d0a 2020 2020 2020 2020 7472  th):..        tr
+0000d150: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+0000d160: 666f 726d 6174 7465 7220 3d20 5375 6274  formatter = Subt
+0000d170: 6974 6c65 466f 726d 6174 7465 7228 7365  itleFormatter(se
+0000d180: 6c66 2e66 6f72 6d61 7429 0d0a 2020 2020  lf.format)..    
+0000d190: 2020 2020 2020 2020 666f 726d 6174 7465          formatte
+0000d1a0: 645f 7375 6274 6974 6c65 7320 3d20 666f  d_subtitles = fo
+0000d1b0: 726d 6174 7465 7228 7365 6c66 2e74 696d  rmatter(self.tim
+0000d1c0: 6564 5f73 7562 7469 746c 6573 290d 0a20  ed_subtitles).. 
+0000d1d0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+0000d1e0: 5f73 7562 7469 746c 655f 6669 6c65 7061  _subtitle_filepa
+0000d1f0: 7468 203d 2064 6563 6c61 7265 645f 7375  th = declared_su
+0000d200: 6274 6974 6c65 5f66 696c 6570 6174 680d  btitle_filepath.
+0000d210: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000d220: 7361 7665 645f 7375 6274 6974 6c65 5f66  saved_subtitle_f
+0000d230: 696c 6570 6174 683a 0d0a 2020 2020 2020  ilepath:..      
+0000d240: 2020 2020 2020 2020 2020 7375 6274 6974            subtit
+0000d250: 6c65 5f66 696c 655f 6261 7365 2c20 7375  le_file_base, su
+0000d260: 6274 6974 6c65 5f66 696c 655f 6578 7420  btitle_file_ext 
+0000d270: 3d20 6f73 2e70 6174 682e 7370 6c69 7465  = os.path.splite
+0000d280: 7874 2873 6176 6564 5f73 7562 7469 746c  xt(saved_subtitl
+0000d290: 655f 6669 6c65 7061 7468 290d 0a20 2020  e_filepath)..   
+0000d2a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d2b0: 6e6f 7420 7375 6274 6974 6c65 5f66 696c  not subtitle_fil
+0000d2c0: 655f 6578 743a 0d0a 2020 2020 2020 2020  e_ext:..        
+0000d2d0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+0000d2e0: 645f 7375 6274 6974 6c65 5f66 696c 6570  d_subtitle_filep
+0000d2f0: 6174 6820 3d20 227b 6261 7365 7d2e 7b66  ath = "{base}.{f
+0000d300: 6f72 6d61 747d 222e 666f 726d 6174 2862  ormat}".format(b
+0000d310: 6173 653d 7375 6274 6974 6c65 5f66 696c  ase=subtitle_fil
+0000d320: 655f 6261 7365 2c20 666f 726d 6174 3d73  e_base, format=s
+0000d330: 656c 662e 666f 726d 6174 290d 0a20 2020  elf.format)..   
+0000d340: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000d350: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000d360: 2020 2020 2020 2020 7361 7665 645f 7375          saved_su
+0000d370: 6274 6974 6c65 5f66 696c 6570 6174 6820  btitle_filepath 
+0000d380: 3d20 6465 636c 6172 6564 5f73 7562 7469  = declared_subti
+0000d390: 746c 655f 6669 6c65 7061 7468 0d0a 2020  tle_filepath..  
+0000d3a0: 2020 2020 2020 2020 2020 7769 7468 206f            with o
+0000d3b0: 7065 6e28 7361 7665 645f 7375 6274 6974  pen(saved_subtit
+0000d3c0: 6c65 5f66 696c 6570 6174 682c 2027 7762  le_filepath, 'wb
+0000d3d0: 2729 2061 7320 663a 0d0a 2020 2020 2020  ') as f:..      
+0000d3e0: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
+0000d3f0: 6528 666f 726d 6174 7465 645f 7375 6274  e(formatted_subt
+0000d400: 6974 6c65 732e 656e 636f 6465 2822 7574  itles.encode("ut
+0000d410: 662d 3822 2929 0d0a 2020 2020 2020 2020  f-8"))..        
+0000d420: 2020 2020 2377 6974 6820 6f70 656e 2873      #with open(s
+0000d430: 6176 6564 5f73 7562 7469 746c 655f 6669  aved_subtitle_fi
+0000d440: 6c65 7061 7468 2c20 2761 2729 2061 7320  lepath, 'a') as 
+0000d450: 663a 0d0a 2020 2020 2020 2020 2020 2020  f:..            
+0000d460: 2320 2020 2066 2e77 7269 7465 2822 5c6e  #    f.write("\n
+0000d470: 2229 0d0a 0d0a 2020 2020 2020 2020 6578  ")....        ex
+0000d480: 6365 7074 204b 6579 626f 6172 6449 6e74  cept KeyboardInt
+0000d490: 6572 7275 7074 3a0d 0a20 2020 2020 2020  errupt:..       
+0000d4a0: 2020 2020 2069 6620 7365 6c66 2e65 7272       if self.err
+0000d4b0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000d4c0: 6261 636b 3a0d 0a20 2020 2020 2020 2020  back:..         
+0000d4d0: 2020 2020 2020 2073 656c 662e 6572 726f         self.erro
+0000d4e0: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000d4f0: 6163 6b28 2243 616e 6365 6c6c 696e 6720  ack("Cancelling 
+0000d500: 616c 6c20 7461 736b 7322 290d 0a20 2020  all tasks")..   
+0000d510: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
 0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d530: 662e 7772 6974 6528 666f 726d 6174 7465  f.write(formatte
-0000d540: 645f 7375 6274 6974 6c65 732e 656e 636f  d_subtitles.enco
-0000d550: 6465 2822 7574 662d 3822 2929 0d0a 2020  de("utf-8"))..  
-0000d560: 2020 2020 2020 2020 2020 2377 6974 6820            #with 
-0000d570: 6f70 656e 2873 6176 6564 5f73 7562 7469  open(saved_subti
-0000d580: 746c 655f 6669 6c65 7061 7468 2c20 2761  tle_filepath, 'a
-0000d590: 2729 2061 7320 663a 0d0a 2020 2020 2020  ') as f:..      
-0000d5a0: 2020 2020 2020 2320 2020 2066 2e77 7269        #    f.wri
-0000d5b0: 7465 2822 5c6e 2229 0d0a 0d0a 2020 2020  te("\n")....    
-0000d5c0: 2020 2020 6578 6365 7074 204b 6579 626f      except Keybo
-0000d5d0: 6172 6449 6e74 6572 7275 7074 3a0d 0a20  ardInterrupt:.. 
-0000d5e0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000d5f0: 6c66 2e65 7272 6f72 5f6d 6573 7361 6765  lf.error_message
-0000d600: 735f 6361 6c6c 6261 636b 3a0d 0a20 2020  s_callback:..   
-0000d610: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000d620: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
-0000d630: 5f63 616c 6c62 6163 6b28 2243 616e 6365  _callback("Cance
-0000d640: 6c6c 696e 6720 616c 6c20 7461 736b 7322  lling all tasks"
-0000d650: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-0000d660: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0000d670: 2020 2020 2020 7072 696e 7428 2243 616e        print("Can
-0000d680: 6365 6c6c 696e 6720 616c 6c20 7461 736b  celling all task
-0000d690: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
-0000d6a0: 2072 6574 7572 6e0d 0a0d 0a20 2020 2020   return....     
-0000d6b0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-0000d6c0: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-0000d6d0: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-0000d6e0: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000d6f0: 6c6c 6261 636b 3a0d 0a20 2020 2020 2020  llback:..       
-0000d700: 2020 2020 2020 2020 2073 656c 662e 6572           self.er
-0000d710: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-0000d720: 6c62 6163 6b28 6529 0d0a 2020 2020 2020  lback(e)..      
-0000d730: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-0000d740: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-0000d750: 6e74 2865 290d 0a20 2020 2020 2020 2020  nt(e)..         
-0000d760: 2020 2072 6574 7572 6e0d 0a0d 0a0d 0a63     return......c
-0000d770: 6c61 7373 2053 5254 4669 6c65 5265 6164  lass SRTFileRead
-0000d780: 6572 3a0d 0a20 2020 2064 6566 205f 5f69  er:..    def __i
-0000d790: 6e69 745f 5f28 7365 6c66 2c20 7372 745f  nit__(self, srt_
-0000d7a0: 6669 6c65 5f70 6174 682c 2065 7272 6f72  file_path, error
-0000d7b0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000d7c0: 636b 3d4e 6f6e 6529 3a0d 0a20 2020 2020  ck=None):..     
-0000d7d0: 2020 2073 656c 662e 7469 6d65 645f 7375     self.timed_su
-0000d7e0: 6274 6974 6c65 7320 3d20 7365 6c66 2873  btitles = self(s
-0000d7f0: 7274 5f66 696c 655f 7061 7468 290d 0a20  rt_file_path).. 
-0000d800: 2020 2020 2020 2073 656c 662e 6572 726f         self.erro
-0000d810: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
-0000d820: 6163 6b20 3d20 6572 726f 725f 6d65 7373  ack = error_mess
-0000d830: 6167 6573 5f63 616c 6c62 6163 6b0d 0a0d  ages_callback...
-0000d840: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-0000d850: 6f64 0d0a 2020 2020 6465 6620 5f5f 6361  od..    def __ca
-0000d860: 6c6c 5f5f 2873 7274 5f66 696c 655f 7061  ll__(srt_file_pa
-0000d870: 7468 293a 0d0a 2020 2020 2020 2020 7472  th):..        tr
-0000d880: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-0000d890: 2222 220d 0a20 2020 2020 2020 2020 2020  """..           
-0000d8a0: 2052 6561 6420 5352 5420 666f 726d 6174   Read SRT format
-0000d8b0: 7465 6420 7375 6274 6974 6c65 2066 696c  ted subtitle fil
-0000d8c0: 6520 616e 6420 7265 7475 726e 2073 7562  e and return sub
-0000d8d0: 7469 746c 6573 2061 7320 6c69 7374 206f  titles as list o
-0000d8e0: 6620 7475 706c 6573 0d0a 2020 2020 2020  f tuples..      
-0000d8f0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-0000d900: 2020 2020 2020 2074 696d 6564 5f73 7562         timed_sub
-0000d910: 7469 746c 6573 203d 205b 5d0d 0a20 2020  titles = []..   
-0000d920: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-0000d930: 656e 2873 7274 5f66 696c 655f 7061 7468  en(srt_file_path
-0000d940: 2c20 2772 2729 2061 7320 7372 745f 6669  , 'r') as srt_fi
-0000d950: 6c65 3a0d 0a20 2020 2020 2020 2020 2020  le:..           
-0000d960: 2020 2020 206c 696e 6573 203d 2073 7274       lines = srt
-0000d970: 5f66 696c 652e 7265 6164 6c69 6e65 7328  _file.readlines(
-0000d980: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000d990: 2020 2023 2053 706c 6974 2074 6865 2073     # Split the s
-0000d9a0: 7562 7469 746c 6520 6669 6c65 2069 6e74  ubtitle file int
-0000d9b0: 6f20 7375 6274 6974 6c65 2062 6c6f 636b  o subtitle block
-0000d9c0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-0000d9d0: 2020 2073 7562 7469 746c 655f 626c 6f63     subtitle_bloc
-0000d9e0: 6b73 203d 205b 5d0d 0a20 2020 2020 2020  ks = []..       
-0000d9f0: 2020 2020 2020 2020 2062 6c6f 636b 203d           block =
-0000da00: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-0000da10: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
-0000da20: 206c 696e 6573 3a0d 0a20 2020 2020 2020   lines:..       
-0000da30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000da40: 6c69 6e65 2e73 7472 6970 2829 203d 3d20  line.strip() == 
-0000da50: 2727 3a0d 0a20 2020 2020 2020 2020 2020  '':..           
-0000da60: 2020 2020 2020 2020 2020 2020 2073 7562               sub
-0000da70: 7469 746c 655f 626c 6f63 6b73 2e61 7070  title_blocks.app
-0000da80: 656e 6428 626c 6f63 6b29 0d0a 2020 2020  end(block)..    
+0000d530: 7072 696e 7428 2243 616e 6365 6c6c 696e  print("Cancellin
+0000d540: 6720 616c 6c20 7461 736b 7322 290d 0a20  g all tasks").. 
+0000d550: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000d560: 6e0d 0a0d 0a20 2020 2020 2020 2065 7863  n....        exc
+0000d570: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+0000d580: 2065 3a0d 0a20 2020 2020 2020 2020 2020   e:..           
+0000d590: 2069 6620 7365 6c66 2e65 7272 6f72 5f6d   if self.error_m
+0000d5a0: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
+0000d5b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000d5c0: 2020 2073 656c 662e 6572 726f 725f 6d65     self.error_me
+0000d5d0: 7373 6167 6573 5f63 616c 6c62 6163 6b28  ssages_callback(
+0000d5e0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+0000d5f0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0000d600: 2020 2020 2020 2070 7269 6e74 2865 290d         print(e).
+0000d610: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000d620: 7572 6e0d 0a0d 0a0d 0a63 6c61 7373 2053  urn......class S
+0000d630: 5254 4669 6c65 5265 6164 6572 3a0d 0a20  RTFileReader:.. 
+0000d640: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0000d650: 7365 6c66 2c20 7372 745f 6669 6c65 5f70  self, srt_file_p
+0000d660: 6174 682c 2065 7272 6f72 5f6d 6573 7361  ath, error_messa
+0000d670: 6765 735f 6361 6c6c 6261 636b 3d4e 6f6e  ges_callback=Non
+0000d680: 6529 3a0d 0a20 2020 2020 2020 2073 656c  e):..        sel
+0000d690: 662e 7469 6d65 645f 7375 6274 6974 6c65  f.timed_subtitle
+0000d6a0: 7320 3d20 7365 6c66 2873 7274 5f66 696c  s = self(srt_fil
+0000d6b0: 655f 7061 7468 290d 0a20 2020 2020 2020  e_path)..       
+0000d6c0: 2073 656c 662e 6572 726f 725f 6d65 7373   self.error_mess
+0000d6d0: 6167 6573 5f63 616c 6c62 6163 6b20 3d20  ages_callback = 
+0000d6e0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
+0000d6f0: 616c 6c62 6163 6b0d 0a0d 0a20 2020 2040  allback....    @
+0000d700: 7374 6174 6963 6d65 7468 6f64 0d0a 2020  staticmethod..  
+0000d710: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2873    def __call__(s
+0000d720: 7274 5f66 696c 655f 7061 7468 293a 0d0a  rt_file_path):..
+0000d730: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+0000d740: 2020 2020 2020 2020 2020 2222 220d 0a20            """.. 
+0000d750: 2020 2020 2020 2020 2020 2052 6561 6420             Read 
+0000d760: 5352 5420 666f 726d 6174 7465 6420 7375  SRT formatted su
+0000d770: 6274 6974 6c65 2066 696c 6520 616e 6420  btitle file and 
+0000d780: 7265 7475 726e 2073 7562 7469 746c 6573  return subtitles
+0000d790: 2061 7320 6c69 7374 206f 6620 7475 706c   as list of tupl
+0000d7a0: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
+0000d7b0: 2222 220d 0a20 2020 2020 2020 2020 2020  """..           
+0000d7c0: 2074 696d 6564 5f73 7562 7469 746c 6573   timed_subtitles
+0000d7d0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+0000d7e0: 2020 2077 6974 6820 6f70 656e 2873 7274     with open(srt
+0000d7f0: 5f66 696c 655f 7061 7468 2c20 2772 2729  _file_path, 'r')
+0000d800: 2061 7320 7372 745f 6669 6c65 3a0d 0a20   as srt_file:.. 
+0000d810: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000d820: 696e 6573 203d 2073 7274 5f66 696c 652e  ines = srt_file.
+0000d830: 7265 6164 6c69 6e65 7328 290d 0a20 2020  readlines()..   
+0000d840: 2020 2020 2020 2020 2020 2020 2023 2053               # S
+0000d850: 706c 6974 2074 6865 2073 7562 7469 746c  plit the subtitl
+0000d860: 6520 6669 6c65 2069 6e74 6f20 7375 6274  e file into subt
+0000d870: 6974 6c65 2062 6c6f 636b 730d 0a20 2020  itle blocks..   
+0000d880: 2020 2020 2020 2020 2020 2020 2073 7562               sub
+0000d890: 7469 746c 655f 626c 6f63 6b73 203d 205b  title_blocks = [
+0000d8a0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000d8b0: 2020 2062 6c6f 636b 203d 205b 5d0d 0a20     block = [].. 
+0000d8c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000d8d0: 6f72 206c 696e 6520 696e 206c 696e 6573  or line in lines
+0000d8e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000d8f0: 2020 2020 2020 2069 6620 6c69 6e65 2e73         if line.s
+0000d900: 7472 6970 2829 203d 3d20 2727 3a0d 0a20  trip() == '':.. 
+0000d910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d920: 2020 2020 2020 2073 7562 7469 746c 655f         subtitle_
+0000d930: 626c 6f63 6b73 2e61 7070 656e 6428 626c  blocks.append(bl
+0000d940: 6f63 6b29 0d0a 2020 2020 2020 2020 2020  ock)..          
+0000d950: 2020 2020 2020 2020 2020 2020 2020 626c                bl
+0000d960: 6f63 6b20 3d20 5b5d 0d0a 2020 2020 2020  ock = []..      
+0000d970: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000d980: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000d990: 2020 2020 2020 2020 2020 2020 2062 6c6f               blo
+0000d9a0: 636b 2e61 7070 656e 6428 6c69 6e65 2e73  ck.append(line.s
+0000d9b0: 7472 6970 2829 290d 0a20 2020 2020 2020  trip())..       
+0000d9c0: 2020 2020 2020 2020 2073 7562 7469 746c           subtitl
+0000d9d0: 655f 626c 6f63 6b73 2e61 7070 656e 6428  e_blocks.append(
+0000d9e0: 626c 6f63 6b29 0d0a 0d0a 2020 2020 2020  block)....      
+0000d9f0: 2020 2020 2020 2020 2020 2320 5061 7273            # Pars
+0000da00: 6520 6561 6368 2073 7562 7469 746c 6520  e each subtitle 
+0000da10: 626c 6f63 6b20 616e 6420 7374 6f72 6520  block and store 
+0000da20: 6173 2074 7570 6c65 2069 6e20 7469 6d65  as tuple in time
+0000da30: 645f 7375 6274 6974 6c65 7320 6c69 7374  d_subtitles list
+0000da40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000da50: 2020 666f 7220 626c 6f63 6b20 696e 2073    for block in s
+0000da60: 7562 7469 746c 655f 626c 6f63 6b73 3a0d  ubtitle_blocks:.
+0000da70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000da80: 2020 2020 2069 6620 626c 6f63 6b3a 0d0a       if block:..
 0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daa0: 2020 2020 626c 6f63 6b20 3d20 5b5d 0d0a      block = []..
-0000dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dac0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dae0: 2020 2062 6c6f 636b 2e61 7070 656e 6428     block.append(
-0000daf0: 6c69 6e65 2e73 7472 6970 2829 290d 0a20  line.strip()).. 
-0000db00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000db10: 7562 7469 746c 655f 626c 6f63 6b73 2e61  ubtitle_blocks.a
-0000db20: 7070 656e 6428 626c 6f63 6b29 0d0a 0d0a  ppend(block)....
+0000daa0: 2020 2020 2020 2020 2320 4578 7472 6163          # Extrac
+0000dab0: 7420 7374 6172 7420 616e 6420 656e 6420  t start and end 
+0000dac0: 7469 6d65 7320 6672 6f6d 2073 7562 7469  times from subti
+0000dad0: 746c 6520 626c 6f63 6b0d 0a20 2020 2020  tle block..     
+0000dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000daf0: 2020 2073 7461 7274 5f74 696d 655f 7374     start_time_st
+0000db00: 722c 2065 6e64 5f74 696d 655f 7374 7220  r, end_time_str 
+0000db10: 3d20 626c 6f63 6b5b 315d 2e73 706c 6974  = block[1].split
+0000db20: 2827 202d 2d3e 2027 290d 0a20 2020 2020  (' --> ')..     
 0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db40: 2320 5061 7273 6520 6561 6368 2073 7562  # Parse each sub
-0000db50: 7469 746c 6520 626c 6f63 6b20 616e 6420  title block and 
-0000db60: 7374 6f72 6520 6173 2074 7570 6c65 2069  store as tuple i
-0000db70: 6e20 7469 6d65 645f 7375 6274 6974 6c65  n timed_subtitle
-0000db80: 7320 6c69 7374 0d0a 2020 2020 2020 2020  s list..        
-0000db90: 2020 2020 2020 2020 666f 7220 626c 6f63          for bloc
-0000dba0: 6b20 696e 2073 7562 7469 746c 655f 626c  k in subtitle_bl
-0000dbb0: 6f63 6b73 3a0d 0a20 2020 2020 2020 2020  ocks:..         
-0000dbc0: 2020 2020 2020 2020 2020 2069 6620 626c             if bl
-0000dbd0: 6f63 6b3a 0d0a 2020 2020 2020 2020 2020  ock:..          
-0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000dbf0: 4578 7472 6163 7420 7374 6172 7420 616e  Extract start an
-0000dc00: 6420 656e 6420 7469 6d65 7320 6672 6f6d  d end times from
-0000dc10: 2073 7562 7469 746c 6520 626c 6f63 6b0d   subtitle block.
-0000dc20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dc30: 2020 2020 2020 2020 2073 7461 7274 5f74           start_t
-0000dc40: 696d 655f 7374 722c 2065 6e64 5f74 696d  ime_str, end_tim
-0000dc50: 655f 7374 7220 3d20 626c 6f63 6b5b 315d  e_str = block[1]
-0000dc60: 2e73 706c 6974 2827 202d 2d3e 2027 290d  .split(' --> ').
-0000dc70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dc80: 2020 2020 2020 2020 2074 696d 655f 666f           time_fo
-0000dc90: 726d 6174 203d 2027 2548 3a25 4d3a 2553  rmat = '%H:%M:%S
-0000dca0: 2c25 6627 0d0a 2020 2020 2020 2020 2020  ,%f'..          
-0000dcb0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0000dcc0: 6172 745f 7469 6d65 5f74 696d 655f 6465  art_time_time_de
-0000dcd0: 6c74 6120 3d20 6461 7465 7469 6d65 2e73  lta = datetime.s
-0000dce0: 7472 7074 696d 6528 7374 6172 745f 7469  trptime(start_ti
-0000dcf0: 6d65 5f73 7472 2c20 7469 6d65 5f66 6f72  me_str, time_for
-0000dd00: 6d61 7429 202d 2064 6174 6574 696d 652e  mat) - datetime.
-0000dd10: 7374 7270 7469 6d65 2827 3030 3a30 303a  strptime('00:00:
-0000dd20: 3030 2c30 3030 272c 2074 696d 655f 666f  00,000', time_fo
-0000dd30: 726d 6174 290d 0a20 2020 2020 2020 2020  rmat)..         
-0000dd40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000dd50: 7461 7274 5f74 696d 655f 746f 7461 6c5f  tart_time_total_
-0000dd60: 7365 636f 6e64 7320 3d20 7374 6172 745f  seconds = start_
-0000dd70: 7469 6d65 5f74 696d 655f 6465 6c74 612e  time_time_delta.
-0000dd80: 746f 7461 6c5f 7365 636f 6e64 7328 290d  total_seconds().
-0000dd90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dda0: 2020 2020 2020 2020 2065 6e64 5f74 696d           end_tim
-0000ddb0: 655f 7469 6d65 5f64 656c 7461 203d 2064  e_time_delta = d
-0000ddc0: 6174 6574 696d 652e 7374 7270 7469 6d65  atetime.strptime
-0000ddd0: 2865 6e64 5f74 696d 655f 7374 722c 2074  (end_time_str, t
-0000dde0: 696d 655f 666f 726d 6174 2920 2d20 6461  ime_format) - da
-0000ddf0: 7465 7469 6d65 2e73 7472 7074 696d 6528  tetime.strptime(
-0000de00: 2730 303a 3030 3a30 302c 3030 3027 2c20  '00:00:00,000', 
-0000de10: 7469 6d65 5f66 6f72 6d61 7429 0d0a 2020  time_format)..  
-0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de30: 2020 2020 2020 656e 645f 7469 6d65 5f74        end_time_t
-0000de40: 6f74 616c 5f73 6563 6f6e 6473 203d 2065  otal_seconds = e
-0000de50: 6e64 5f74 696d 655f 7469 6d65 5f64 656c  nd_time_time_del
-0000de60: 7461 2e74 6f74 616c 5f73 6563 6f6e 6473  ta.total_seconds
-0000de70: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000de80: 2020 2020 2020 2020 2020 2020 2320 4578              # Ex
-0000de90: 7472 6163 7420 7375 6274 6974 6c65 2074  tract subtitle t
-0000dea0: 6578 7420 6672 6f6d 2073 7562 7469 746c  ext from subtitl
-0000deb0: 6520 626c 6f63 6b0d 0a20 2020 2020 2020  e block..       
-0000dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ded0: 2073 7562 7469 746c 6520 3d20 2720 272e   subtitle = ' '.
-0000dee0: 6a6f 696e 2862 6c6f 636b 5b32 3a5d 290d  join(block[2:]).
-0000def0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000df00: 2020 2020 2020 2020 2074 696d 6564 5f73           timed_s
-0000df10: 7562 7469 746c 6573 2e61 7070 656e 6428  ubtitles.append(
-0000df20: 2828 7374 6172 745f 7469 6d65 5f74 6f74  ((start_time_tot
-0000df30: 616c 5f73 6563 6f6e 6473 2c20 656e 645f  al_seconds, end_
-0000df40: 7469 6d65 5f74 6f74 616c 5f73 6563 6f6e  time_total_secon
-0000df50: 6473 292c 2073 7562 7469 746c 6529 290d  ds), subtitle)).
-0000df60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000df70: 2072 6574 7572 6e20 7469 6d65 645f 7375   return timed_su
-0000df80: 6274 6974 6c65 730d 0a0d 0a20 2020 2020  btitles....     
-0000df90: 2020 2065 7863 6570 7420 4b65 7962 6f61     except Keyboa
-0000dfa0: 7264 496e 7465 7272 7570 743a 0d0a 2020  rdInterrupt:..  
-0000dfb0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000dfc0: 662e 6572 726f 725f 6d65 7373 6167 6573  f.error_messages
-0000dfd0: 5f63 616c 6c62 6163 6b3a 0d0a 2020 2020  _callback:..    
-0000dfe0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000dff0: 2e65 7272 6f72 5f6d 6573 7361 6765 735f  .error_messages_
-0000e000: 6361 6c6c 6261 636b 2822 4361 6e63 656c  callback("Cancel
-0000e010: 6c69 6e67 2061 6c6c 2074 6173 6b73 2229  ling all tasks")
-0000e020: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0000e030: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000e040: 2020 2020 2070 7269 6e74 2822 4361 6e63       print("Canc
-0000e050: 656c 6c69 6e67 2061 6c6c 2074 6173 6b73  elling all tasks
-0000e060: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000e070: 7265 7475 726e 0d0a 0d0a 2020 2020 2020  return....      
-0000e080: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-0000e090: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
-0000e0a0: 2020 2020 2020 6966 2073 656c 662e 6572        if self.er
-0000e0b0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-0000e0c0: 6c62 6163 6b3a 0d0a 2020 2020 2020 2020  lback:..        
-0000e0d0: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
-0000e0e0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-0000e0f0: 6261 636b 2865 290d 0a20 2020 2020 2020  back(e)..       
-0000e100: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-0000e110: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000e120: 7428 6529 0d0a 2020 2020 2020 2020 2020  t(e)..          
-0000e130: 2020 7265 7475 726e 0d0a 0d0a 0d0a 6465    return......de
-0000e140: 6620 7368 6f77 5f70 726f 6772 6573 7328  f show_progress(
-0000e150: 6d65 6469 615f 6669 6c65 7061 7468 2c20  media_filepath, 
-0000e160: 7072 6f67 7265 7373 293a 0d0a 2020 2020  progress):..    
-0000e170: 676c 6f62 616c 2070 6261 720d 0a20 2020  global pbar..   
-0000e180: 2070 6261 722e 7570 6461 7465 2870 726f   pbar.update(pro
-0000e190: 6772 6573 7329 0d0a 0d0a 0d0a 6465 6620  gress)......def 
-0000e1a0: 7368 6f77 5f65 7272 6f72 5f6d 6573 7361  show_error_messa
-0000e1b0: 6765 7328 6d65 7373 6167 6573 293a 0d0a  ges(messages):..
-0000e1c0: 2020 2020 7072 696e 7428 6d65 7373 6167      print(messag
-0000e1d0: 6573 290d 0a0d 0a0d 0a64 6566 206d 6169  es)......def mai
-0000e1e0: 6e28 293a 0d0a 2020 2020 676c 6f62 616c  n():..    global
-0000e1f0: 2070 6261 720d 0a0d 0a20 2020 2069 6620   pbar....    if 
-0000e200: 7379 732e 706c 6174 666f 726d 203d 3d20  sys.platform == 
-0000e210: 2277 696e 3332 223a 0d0a 2020 2020 2020  "win32":..      
-0000e220: 2020 7374 6f70 5f66 666d 7065 675f 7769    stop_ffmpeg_wi
-0000e230: 6e64 6f77 7328 6572 726f 725f 6d65 7373  ndows(error_mess
-0000e240: 6167 6573 5f63 616c 6c62 6163 6b3d 7368  ages_callback=sh
-0000e250: 6f77 5f65 7272 6f72 5f6d 6573 7361 6765  ow_error_message
-0000e260: 7329 0d0a 2020 2020 656c 7365 3a0d 0a20  s)..    else:.. 
-0000e270: 2020 2020 2020 2073 746f 705f 6666 6d70         stop_ffmp
-0000e280: 6567 5f6c 696e 7578 2865 7272 6f72 5f6d  eg_linux(error_m
-0000e290: 6573 7361 6765 735f 6361 6c6c 6261 636b  essages_callback
-0000e2a0: 3d73 686f 775f 6572 726f 725f 6d65 7373  =show_error_mess
-0000e2b0: 6167 6573 290d 0a0d 0a20 2020 2072 656d  ages)....    rem
-0000e2c0: 6f76 655f 7465 6d70 5f66 696c 6573 2822  ove_temp_files("
-0000e2d0: 666c 6163 222c 2065 7272 6f72 5f6d 6573  flac", error_mes
-0000e2e0: 7361 6765 735f 6361 6c6c 6261 636b 3d73  sages_callback=s
-0000e2f0: 686f 775f 6572 726f 725f 6d65 7373 6167  how_error_messag
-0000e300: 6573 290d 0a20 2020 2072 656d 6f76 655f  es)..    remove_
-0000e310: 7465 6d70 5f66 696c 6573 2822 7761 7622  temp_files("wav"
-0000e320: 2c20 6572 726f 725f 6d65 7373 6167 6573  , error_messages
-0000e330: 5f63 616c 6c62 6163 6b3d 7368 6f77 5f65  _callback=show_e
-0000e340: 7272 6f72 5f6d 6573 7361 6765 7329 0d0a  rror_messages)..
-0000e350: 0d0a 2020 2020 7061 7273 6572 203d 2061  ..    parser = a
-0000e360: 7267 7061 7273 652e 4172 6775 6d65 6e74  rgparse.Argument
-0000e370: 5061 7273 6572 2829 0d0a 2020 2020 7061  Parser()..    pa
-0000e380: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
-0000e390: 7428 2773 6f75 7263 655f 7061 7468 272c  t('source_path',
-0000e3a0: 2068 656c 703d 2250 6174 6820 746f 2074   help="Path to t
-0000e3b0: 6865 2076 6964 656f 206f 7220 6175 6469  he video or audi
-0000e3c0: 6f20 6669 6c65 7320 746f 2067 656e 6572  o files to gener
-0000e3d0: 6174 6520 7375 6274 6974 6c65 7320 6669  ate subtitles fi
-0000e3e0: 6c65 7320 2875 7365 2077 696c 6463 6172  les (use wildcar
-0000e3f0: 6420 666f 7220 6d75 6c74 6970 6c65 2066  d for multiple f
-0000e400: 696c 6573 206f 7220 7365 7061 7261 7465  iles or separate
-0000e410: 2074 6865 6d20 7769 7468 2061 2073 7061   them with a spa
-0000e420: 6365 2063 6861 7261 6374 6572 2065 2e67  ce character e.g
-0000e430: 2e20 5c22 6669 6c65 2031 2e6d 7034 5c22  . \"file 1.mp4\"
-0000e440: 205c 2266 696c 6520 322e 6d70 345c 2229   \"file 2.mp4\")
-0000e450: 222c 206e 6172 6773 3d27 2a27 290d 0a20  ", nargs='*').. 
-0000e460: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
-0000e470: 6775 6d65 6e74 2827 2d6d 272c 2027 2d2d  gument('-m', '--
-0000e480: 6d6f 6465 6c2d 6e61 6d65 272c 2064 6566  model-name', def
-0000e490: 6175 6c74 3d22 736d 616c 6c22 2c20 6865  ault="small", he
-0000e4a0: 6c70 3d22 6e61 6d65 206f 6620 7468 6520  lp="name of the 
-0000e4b0: 5768 6973 7065 7220 6d6f 6465 6c20 746f  Whisper model to
-0000e4c0: 2075 7365 2229 0d0a 2020 2020 7061 7273   use")..    pars
-0000e4d0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-0000e4e0: 272d 6c6d 272c 2027 2d2d 6c69 7374 2d6d  '-lm', '--list-m
-0000e4f0: 6f64 656c 7327 2c20 6865 6c70 3d22 4c69  odels', help="Li
-0000e500: 7374 206f 6620 5768 6973 7065 7220 6d6f  st of Whisper mo
-0000e510: 6465 6c73 206e 616d 6522 2c20 6163 7469  dels name", acti
-0000e520: 6f6e 3d27 7374 6f72 655f 7472 7565 2729  on='store_true')
-0000e530: 0d0a 2020 2020 7061 7273 6572 2e61 6464  ..    parser.add
-0000e540: 5f61 7267 756d 656e 7428 272d 5327 2c20  _argument('-S', 
-0000e550: 272d 2d73 7263 2d6c 616e 6775 6167 6527  '--src-language'
-0000e560: 2c20 6865 6c70 3d22 4c61 6e67 7561 6765  , help="Language
-0000e570: 2063 6f64 6520 6f66 2074 6865 2061 7564   code of the aud
-0000e580: 696f 206c 616e 6775 6167 6520 7370 6f6b  io language spok
-0000e590: 656e 2069 6e20 7669 6465 6f2f 6175 6469  en in video/audi
-0000e5a0: 6f20 736f 7572 6365 5f70 6174 6822 2c20  o source_path", 
-0000e5b0: 6465 6661 756c 743d 2265 6e22 290d 0a20  default="en").. 
-0000e5c0: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
-0000e5d0: 6775 6d65 6e74 2827 2d44 272c 2027 2d2d  gument('-D', '--
-0000e5e0: 6473 742d 6c61 6e67 7561 6765 272c 2068  dst-language', h
-0000e5f0: 656c 703d 2244 6573 6972 6564 2074 7261  elp="Desired tra
-0000e600: 6e73 6c61 7469 6f6e 206c 616e 6775 6167  nslation languag
-0000e610: 6520 636f 6465 2066 6f72 2074 6865 2073  e code for the s
-0000e620: 7562 7469 746c 6573 222c 2064 6566 6175  ubtitles", defau
-0000e630: 6c74 3d4e 6f6e 6529 0d0a 2020 2020 7061  lt=None)..    pa
-0000e640: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
-0000e650: 7428 272d 6c77 6c27 2c20 272d 2d6c 6973  t('-lwl', '--lis
-0000e660: 742d 7768 6973 7065 722d 6c61 6e67 7561  t-whisper-langua
-0000e670: 6765 7327 2c20 6865 6c70 3d22 4c69 7374  ges', help="List
-0000e680: 2061 6c6c 2077 6869 7370 6572 2073 7570   all whisper sup
-0000e690: 706f 7274 6564 206c 616e 6775 6167 6573  ported languages
-0000e6a0: 222c 2061 6374 696f 6e3d 2773 746f 7265  ", action='store
-0000e6b0: 5f74 7275 6527 290d 0a20 2020 2070 6172  _true')..    par
-0000e6c0: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
-0000e6d0: 2827 2d6c 676c 272c 2027 2d2d 6c69 7374  ('-lgl', '--list
-0000e6e0: 2d67 6f6f 676c 652d 6c61 6e67 7561 6765  -google-language
-0000e6f0: 7327 2c20 6865 6c70 3d22 4c69 7374 2061  s', help="List a
-0000e700: 6c6c 2067 6f6f 676c 6520 7472 616e 736c  ll google transl
-0000e710: 6174 6520 7375 7070 6f72 7465 6420 6c61  ate supported la
-0000e720: 6e67 7561 6765 7322 2c20 6163 7469 6f6e  nguages", action
-0000e730: 3d27 7374 6f72 655f 7472 7565 2729 0d0a  ='store_true')..
-0000e740: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
-0000e750: 7267 756d 656e 7428 272d 4627 2c20 272d  rgument('-F', '-
-0000e760: 2d66 6f72 6d61 7427 2c20 6865 6c70 3d22  -format', help="
-0000e770: 4465 7369 7265 6420 7375 6274 6974 6c65  Desired subtitle
-0000e780: 2066 6f72 6d61 7422 2c20 6465 6661 756c   format", defaul
-0000e790: 743d 2273 7274 2229 0d0a 2020 2020 7061  t="srt")..    pa
-0000e7a0: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
-0000e7b0: 7428 272d 6c66 272c 2027 2d2d 6c69 7374  t('-lf', '--list
-0000e7c0: 2d66 6f72 6d61 7473 272c 2068 656c 703d  -formats', help=
-0000e7d0: 224c 6973 7420 616c 6c20 7375 7070 6f72  "List all suppor
-0000e7e0: 7465 6420 7375 6274 6974 6c65 2066 6f72  ted subtitle for
-0000e7f0: 6d61 7473 222c 2061 6374 696f 6e3d 2773  mats", action='s
-0000e800: 746f 7265 5f74 7275 6527 290d 0a20 2020  tore_true')..   
-0000e810: 2070 6172 7365 722e 6164 645f 6172 6775   parser.add_argu
-0000e820: 6d65 6e74 2827 2d43 272c 2027 2d2d 636f  ment('-C', '--co
-0000e830: 6e63 7572 7265 6e63 7927 2c20 6865 6c70  ncurrency', help
-0000e840: 3d22 4e75 6d62 6572 206f 6620 636f 6e63  ="Number of conc
-0000e850: 7572 7265 6e74 2041 5049 2072 6571 7565  urrent API reque
-0000e860: 7374 7320 746f 206d 616b 6522 2c20 7479  sts to make", ty
-0000e870: 7065 3d69 6e74 2c20 6465 6661 756c 743d  pe=int, default=
-0000e880: 3130 290d 0a20 2020 2070 6172 7365 722e  10)..    parser.
-0000e890: 6164 645f 6172 6775 6d65 6e74 2827 2d76  add_argument('-v
-0000e8a0: 272c 2027 2d2d 7665 7273 696f 6e27 2c20  ', '--version', 
-0000e8b0: 6163 7469 6f6e 3d27 7665 7273 696f 6e27  action='version'
-0000e8c0: 2c20 7665 7273 696f 6e3d 5645 5253 494f  , version=VERSIO
-0000e8d0: 4e29 0d0a 0d0a 2020 2020 6172 6773 203d  N)....    args =
-0000e8e0: 2070 6172 7365 722e 7061 7273 655f 6172   parser.parse_ar
-0000e8f0: 6773 2829 0d0a 0d0a 2020 2020 7372 635f  gs()....    src_
-0000e900: 6c61 6e67 7561 6765 203d 2061 7267 732e  language = args.
-0000e910: 7372 635f 6c61 6e67 7561 6765 0d0a 2020  src_language..  
-0000e920: 2020 6473 745f 6c61 6e67 7561 6765 203d    dst_language =
-0000e930: 2061 7267 732e 6473 745f 6c61 6e67 7561   args.dst_langua
-0000e940: 6765 0d0a 0d0a 2020 2020 6d6f 6465 6c5f  ge....    model_
-0000e950: 6e61 6d65 203d 2061 7267 732e 6d6f 6465  name = args.mode
-0000e960: 6c5f 6e61 6d65 0d0a 2020 2020 6966 206d  l_name..    if m
-0000e970: 6f64 656c 5f6e 616d 652e 656e 6473 7769  odel_name.endswi
-0000e980: 7468 2822 2e65 6e22 293a 0d0a 2020 2020  th(".en"):..    
-0000e990: 2020 2020 7072 696e 7428 6622 7b6d 6f64      print(f"{mod
-0000e9a0: 656c 5f6e 616d 657d 2069 7320 616e 2045  el_name} is an E
-0000e9b0: 6e67 6c69 7368 2d6f 6e6c 7920 6d6f 6465  nglish-only mode
-0000e9c0: 6c2c 2066 6f72 6369 6e67 2045 6e67 6c69  l, forcing Engli
-0000e9d0: 7368 2064 6574 6563 7469 6f6e 2e22 290d  sh detection.").
-0000e9e0: 0a20 2020 2020 2020 2061 7267 732e 7372  .        args.sr
-0000e9f0: 635f 6c61 6e67 7561 6765 203d 2022 656e  c_language = "en
-0000ea00: 220d 0a20 2020 2065 6c69 6620 6172 6773  "..    elif args
-0000ea10: 2e73 7263 5f6c 616e 6775 6167 6520 213d  .src_language !=
-0000ea20: 2022 6175 746f 223a 0d0a 2020 2020 2020   "auto":..      
-0000ea30: 2020 6172 6773 2e73 7263 5f6c 616e 6775    args.src_langu
-0000ea40: 6167 6520 3d20 7372 635f 6c61 6e67 7561  age = src_langua
-0000ea50: 6765 0d0a 0d0a 2020 2020 236d 6f64 656c  ge....    #model
-0000ea60: 203d 2057 6869 7370 6572 4d6f 6465 6c28   = WhisperModel(
-0000ea70: 6d6f 6465 6c5f 6e61 6d65 2c20 636f 6d70  model_name, comp
-0000ea80: 7574 655f 7479 7065 3d22 666c 6f61 7433  ute_type="float3
-0000ea90: 3222 2c20 6370 755f 7468 7265 6164 733d  2", cpu_threads=
-0000eaa0: 342c 206e 756d 5f77 6f72 6b65 7273 3d31  4, num_workers=1
-0000eab0: 3629 0d0a 2020 2020 6d6f 6465 6c20 3d20  6)..    model = 
-0000eac0: 5768 6973 7065 724d 6f64 656c 286d 6f64  WhisperModel(mod
-0000ead0: 656c 5f6e 616d 652c 2063 6f6d 7075 7465  el_name, compute
-0000eae0: 5f74 7970 653d 2266 6c6f 6174 3332 2229  _type="float32")
-0000eaf0: 0d0a 0d0a 2020 2020 6966 2061 7267 732e  ....    if args.
-0000eb00: 6c69 7374 5f6d 6f64 656c 733a 0d0a 2020  list_models:..  
-0000eb10: 2020 2020 2020 7072 696e 7428 224c 6973        print("Lis
-0000eb20: 7420 6f66 2077 6869 7370 6572 206d 6f64  t of whisper mod
-0000eb30: 656c 733a 2229 0d0a 2020 2020 2020 2020  els:")..        
-0000eb40: 2366 6f72 206d 6f64 656c 5f6e 616d 6520  #for model_name 
-0000eb50: 696e 2077 6869 7370 6572 2e61 7661 696c  in whisper.avail
-0000eb60: 6162 6c65 5f6d 6f64 656c 7328 293a 0d0a  able_models():..
-0000eb70: 2020 2020 2020 2020 666f 7220 6d6f 6465          for mode
-0000eb80: 6c5f 6e61 6d65 2069 6e20 7768 6973 7065  l_name in whispe
-0000eb90: 725f 6d6f 6465 6c73 3a0d 0a20 2020 2020  r_models:..     
-0000eba0: 2020 2020 2020 2070 7269 6e74 286d 6f64         print(mod
-0000ebb0: 656c 5f6e 616d 6529 0d0a 2020 2020 2020  el_name)..      
-0000ebc0: 2020 7265 7475 726e 2030 0d0a 0d0a 2020    return 0....  
-0000ebd0: 2020 7768 6973 7065 725f 6c61 6e67 7561    whisper_langua
-0000ebe0: 6765 203d 2057 6869 7370 6572 4c61 6e67  ge = WhisperLang
-0000ebf0: 7561 6765 2829 0d0a 2020 2020 676f 6f67  uage()..    goog
-0000ec00: 6c65 5f6c 616e 6775 6167 6520 3d20 476f  le_language = Go
-0000ec10: 6f67 6c65 4c61 6e67 7561 6765 2829 0d0a  ogleLanguage()..
-0000ec20: 0d0a 2020 2020 6966 2061 7267 732e 6c69  ..    if args.li
-0000ec30: 7374 5f77 6869 7370 6572 5f6c 616e 6775  st_whisper_langu
-0000ec40: 6167 6573 3a0d 0a20 2020 2020 2020 2070  ages:..        p
-0000ec50: 7269 6e74 2822 4c69 7374 206f 6620 7768  rint("List of wh
-0000ec60: 6973 7065 7220 7375 7070 6f72 7465 6420  isper supported 
-0000ec70: 6c61 6e67 7561 6765 733a 2229 0d0a 2020  languages:")..  
-0000ec80: 2020 2020 2020 666f 7220 7768 6973 7065        for whispe
-0000ec90: 725f 636f 6465 2c20 7768 6973 7065 725f  r_code, whisper_
-0000eca0: 6c61 6e67 7561 6765 2069 6e20 736f 7274  language in sort
-0000ecb0: 6564 2877 6869 7370 6572 5f6c 616e 6775  ed(whisper_langu
-0000ecc0: 6167 652e 6e61 6d65 5f6f 665f 636f 6465  age.name_of_code
-0000ecd0: 2e69 7465 6d73 2829 293a 0d0a 2020 2020  .items()):..    
-0000ece0: 2020 2020 2020 2020 7072 696e 7428 2225          print("%
-0000ecf0: 2d38 7320 3a20 2573 2220 2528 7768 6973  -8s : %s" %(whis
-0000ed00: 7065 725f 636f 6465 2c20 7768 6973 7065  per_code, whispe
-0000ed10: 725f 6c61 6e67 7561 6765 2929 0d0a 2020  r_language))..  
-0000ed20: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
-0000ed30: 0d0a 2020 2020 6966 2061 7267 732e 6c69  ..    if args.li
-0000ed40: 7374 5f67 6f6f 676c 655f 6c61 6e67 7561  st_google_langua
-0000ed50: 6765 733a 0d0a 2020 2020 2020 2020 7072  ges:..        pr
-0000ed60: 696e 7428 224c 6973 7420 6f66 2067 6f6f  int("List of goo
-0000ed70: 676c 6520 7472 616e 736c 6174 6520 7375  gle translate su
-0000ed80: 7070 6f72 7465 6420 6c61 6e67 7561 6765  pported language
-0000ed90: 733a 2229 0d0a 2020 2020 2020 2020 666f  s:")..        fo
-0000eda0: 7220 676f 6f67 6c65 5f63 6f64 652c 2067  r google_code, g
-0000edb0: 6f6f 676c 655f 6c61 6e67 7561 6765 2069  oogle_language i
-0000edc0: 6e20 736f 7274 6564 2867 6f6f 676c 655f  n sorted(google_
-0000edd0: 6c61 6e67 7561 6765 2e6e 616d 655f 6f66  language.name_of
-0000ede0: 5f63 6f64 652e 6974 656d 7328 2929 3a0d  _code.items()):.
-0000edf0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-0000ee00: 6e74 2822 252d 3873 203a 2025 7322 2025  nt("%-8s : %s" %
-0000ee10: 2867 6f6f 676c 655f 636f 6465 2c20 676f  (google_code, go
-0000ee20: 6f67 6c65 5f6c 616e 6775 6167 6529 290d  ogle_language)).
-0000ee30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000ee40: 300d 0a0d 0a20 2020 2069 6620 6172 6773  0....    if args
-0000ee50: 2e73 7263 5f6c 616e 6775 6167 6520 6e6f  .src_language no
-0000ee60: 7420 696e 2077 6869 7370 6572 5f6c 616e  t in whisper_lan
-0000ee70: 6775 6167 652e 6e61 6d65 5f6f 665f 636f  guage.name_of_co
-0000ee80: 6465 2e6b 6579 7328 293a 0d0a 2020 2020  de.keys():..    
-0000ee90: 2020 2020 7072 696e 7428 2253 6f75 7263      print("Sourc
-0000eea0: 6520 6c61 6e67 7561 6765 2069 7320 6e6f  e language is no
-0000eeb0: 7420 7375 7070 6f72 7465 642e 2052 756e  t supported. Run
-0000eec0: 2077 6974 6820 2d2d 6c69 7374 2d77 6869   with --list-whi
-0000eed0: 7370 6572 2d6c 616e 6775 6167 6573 2074  sper-languages t
-0000eee0: 6f20 7365 6520 616c 6c20 7768 6973 7065  o see all whispe
-0000eef0: 7220 7375 7070 6f72 7465 6420 6c61 6e67  r supported lang
-0000ef00: 7561 6765 732e 2229 0d0a 2020 2020 2020  uages.")..      
-0000ef10: 2020 7265 7475 726e 2031 0d0a 0d0a 2020    return 1....  
-0000ef20: 2020 6966 2061 7267 732e 6473 745f 6c61    if args.dst_la
-0000ef30: 6e67 7561 6765 3a0d 0a20 2020 2020 2020  nguage:..       
-0000ef40: 2069 6620 6e6f 7420 6172 6773 2e64 7374   if not args.dst
-0000ef50: 5f6c 616e 6775 6167 6520 696e 2067 6f6f  _language in goo
-0000ef60: 676c 655f 6c61 6e67 7561 6765 2e6e 616d  gle_language.nam
-0000ef70: 655f 6f66 5f63 6f64 652e 6b65 7973 2829  e_of_code.keys()
-0000ef80: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-0000ef90: 7269 6e74 2822 4465 7374 696e 6174 696f  rint("Destinatio
-0000efa0: 6e20 6c61 6e67 7561 6765 2069 7320 6e6f  n language is no
-0000efb0: 7420 7375 7070 6f72 7465 642e 2052 756e  t supported. Run
-0000efc0: 2077 6974 6820 2d2d 6c69 7374 2d67 6f6f   with --list-goo
-0000efd0: 676c 652d 6c61 6e67 7561 6765 7320 746f  gle-languages to
-0000efe0: 2073 6565 2061 6c6c 2067 6f6f 676c 6520   see all google 
-0000eff0: 7472 616e 736c 6174 6520 7375 7070 6f72  translate suppor
-0000f000: 7465 6420 6c61 6e67 7561 6765 732e 2229  ted languages.")
-0000f010: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0000f020: 7475 726e 2031 0d0a 2020 2020 2020 2020  turn 1..        
-0000f030: 6966 206e 6f74 2069 735f 7361 6d65 5f6c  if not is_same_l
-0000f040: 616e 6775 6167 6528 6172 6773 2e73 7263  anguage(args.src
-0000f050: 5f6c 616e 6775 6167 652c 2061 7267 732e  _language, args.
-0000f060: 6473 745f 6c61 6e67 7561 6765 2c20 6572  dst_language, er
-0000f070: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
-0000f080: 6c62 6163 6b3d 7368 6f77 5f65 7272 6f72  lback=show_error
-0000f090: 5f6d 6573 7361 6765 7329 3a0d 0a20 2020  _messages):..   
-0000f0a0: 2020 2020 2020 2020 2064 6f5f 7472 616e           do_tran
-0000f0b0: 736c 6174 6520 3d20 5472 7565 0d0a 2020  slate = True..  
-0000f0c0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-0000f0d0: 2020 2020 2020 2020 2064 6f5f 7472 616e           do_tran
-0000f0e0: 736c 6174 6520 3d20 4661 6c73 650d 0a20  slate = False.. 
-0000f0f0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0000f100: 2020 646f 5f74 7261 6e73 6c61 7465 203d    do_translate =
-0000f110: 2046 616c 7365 0d0a 0d0a 2020 2020 6966   False....    if
-0000f120: 2061 7267 732e 6c69 7374 5f66 6f72 6d61   args.list_forma
-0000f130: 7473 3a0d 0a20 2020 2020 2020 2070 7269  ts:..        pri
-0000f140: 6e74 2822 4c69 7374 206f 6620 7375 7070  nt("List of supp
-0000f150: 6f72 7465 6420 7375 6274 6974 6c65 2066  orted subtitle f
-0000f160: 6f72 6d61 7473 3a22 290d 0a20 2020 2020  ormats:")..     
-0000f170: 2020 2066 6f72 2073 7562 7469 746c 655f     for subtitle_
-0000f180: 666f 726d 6174 2069 6e20 5375 6274 6974  format in Subtit
-0000f190: 6c65 466f 726d 6174 7465 722e 7375 7070  leFormatter.supp
-0000f1a0: 6f72 7465 645f 666f 726d 6174 733a 0d0a  orted_formats:..
-0000f1b0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000f1c0: 7428 227b 666f 726d 6174 7d22 2e66 6f72  t("{format}".for
-0000f1d0: 6d61 7428 666f 726d 6174 3d73 7562 7469  mat(format=subti
-0000f1e0: 746c 655f 666f 726d 6174 2929 0d0a 2020  tle_format))..  
-0000f1f0: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
-0000f200: 0d0a 2020 2020 6966 2061 7267 732e 666f  ..    if args.fo
-0000f210: 726d 6174 206e 6f74 2069 6e20 5375 6274  rmat not in Subt
-0000f220: 6974 6c65 466f 726d 6174 7465 722e 7375  itleFormatter.su
-0000f230: 7070 6f72 7465 645f 666f 726d 6174 733a  pported_formats:
-0000f240: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-0000f250: 2253 7562 7469 746c 6520 666f 726d 6174  "Subtitle format
-0000f260: 2069 7320 6e6f 7420 7375 7070 6f72 7465   is not supporte
-0000f270: 642e 2052 756e 2077 6974 6820 2d2d 6c69  d. Run with --li
-0000f280: 7374 2d66 6f72 6d61 7473 2074 6f20 7365  st-formats to se
-0000f290: 6520 616c 6c20 7375 7070 6f72 7465 6420  e all supported 
-0000f2a0: 666f 726d 6174 732e 2229 0d0a 2020 2020  formats.")..    
-0000f2b0: 2020 2020 7265 7475 726e 2031 0d0a 0d0a      return 1....
-0000f2c0: 2020 2020 6966 206e 6f74 2061 7267 732e      if not args.
-0000f2d0: 736f 7572 6365 5f70 6174 683a 0d0a 2020  source_path:..  
-0000f2e0: 2020 2020 2020 7061 7273 6572 2e70 7269        parser.pri
-0000f2f0: 6e74 5f68 656c 7028 7379 732e 7374 6465  nt_help(sys.stde
-0000f300: 7272 290d 0a20 2020 2020 2020 2072 6574  rr)..        ret
-0000f310: 7572 6e20 310d 0a0d 0a20 2020 2063 6f6d  urn 1....    com
-0000f320: 706c 6574 6564 5f74 6173 6b73 203d 2030  pleted_tasks = 0
-0000f330: 0d0a 2020 2020 6d65 6469 615f 6669 6c65  ..    media_file
-0000f340: 7061 7468 7320 3d20 5b5d 0d0a 2020 2020  paths = []..    
-0000f350: 6172 675f 6669 6c65 7061 7468 7320 3d20  arg_filepaths = 
-0000f360: 5b5d 0d0a 2020 2020 696e 7661 6c69 645f  []..    invalid_
-0000f370: 6d65 6469 615f 6669 6c65 7061 7468 7320  media_filepaths 
-0000f380: 3d20 5b5d 0d0a 2020 2020 6e6f 745f 6578  = []..    not_ex
-0000f390: 6973 745f 6669 6c65 7061 7468 7320 3d20  ist_filepaths = 
-0000f3a0: 5b5d 0d0a 2020 2020 6172 6770 6174 6820  []..    argpath 
-0000f3b0: 3d20 4e6f 6e65 0d0a 0d0a 2020 2020 6172  = None....    ar
-0000f3c0: 6773 5f73 6f75 7263 655f 7061 7468 203d  gs_source_path =
-0000f3d0: 2061 7267 732e 736f 7572 6365 5f70 6174   args.source_pat
-0000f3e0: 680d 0a0d 0a20 2020 2069 6620 286e 6f74  h....    if (not
-0000f3f0: 2022 2a22 2069 6e20 7374 7228 6172 6773   "*" in str(args
-0000f400: 5f73 6f75 7263 655f 7061 7468 2929 2061  _source_path)) a
-0000f410: 6e64 2028 6e6f 7420 223f 2220 696e 2073  nd (not "?" in s
-0000f420: 7472 2861 7267 735f 736f 7572 6365 5f70  tr(args_source_p
-0000f430: 6174 6829 293a 0d0a 2020 2020 2020 2020  ath)):..        
-0000f440: 666f 7220 6669 6c65 7061 7468 2069 6e20  for filepath in 
-0000f450: 6172 6773 5f73 6f75 7263 655f 7061 7468  args_source_path
-0000f460: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-0000f470: 7061 7468 203d 2050 6174 6828 6669 6c65  path = Path(file
-0000f480: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
-0000f490: 2020 2069 6620 6e6f 7420 6f73 2e70 6174     if not os.pat
-0000f4a0: 682e 6973 6669 6c65 2866 7061 7468 293a  h.isfile(fpath):
-0000f4b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f4c0: 2020 6e6f 745f 6578 6973 745f 6669 6c65    not_exist_file
-0000f4d0: 7061 7468 732e 6170 7065 6e64 2866 696c  paths.append(fil
-0000f4e0: 6570 6174 6829 0d0a 0d0a 2020 2020 6966  epath)....    if
-0000f4f0: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
-0000f500: 2022 7769 6e33 3222 3a0d 0a20 2020 2020   "win32":..     
-0000f510: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0000f520: 6528 6c65 6e28 6172 6773 2e73 6f75 7263  e(len(args.sourc
-0000f530: 655f 7061 7468 2929 3a0d 0a20 2020 2020  e_path)):..     
-0000f540: 2020 2020 2020 2069 6620 2822 5b22 206f         if ("[" o
-0000f550: 7220 225d 2229 2069 6e20 6172 6773 2e73  r "]") in args.s
-0000f560: 6f75 7263 655f 7061 7468 5b69 5d3a 0d0a  ource_path[i]:..
-0000f570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f580: 706c 6163 6568 6f6c 6465 7220 3d20 2223  placeholder = "#
-0000f590: 5445 4d50 2322 0d0a 2020 2020 2020 2020  TEMP#"..        
-0000f5a0: 2020 2020 2020 2020 6172 6773 5f73 6f75          args_sou
-0000f5b0: 7263 655f 7061 7468 5b69 5d20 3d20 6172  rce_path[i] = ar
-0000f5c0: 6773 2e73 6f75 7263 655f 7061 7468 5b69  gs.source_path[i
-0000f5d0: 5d2e 7265 706c 6163 6528 225b 222c 2070  ].replace("[", p
-0000f5e0: 6c61 6365 686f 6c64 6572 290d 0a20 2020  laceholder)..   
-0000f5f0: 2020 2020 2020 2020 2020 2020 2061 7267               arg
-0000f600: 735f 736f 7572 6365 5f70 6174 685b 695d  s_source_path[i]
-0000f610: 203d 2061 7267 735f 736f 7572 6365 5f70   = args_source_p
-0000f620: 6174 685b 695d 2e72 6570 6c61 6365 2822  ath[i].replace("
-0000f630: 5d22 2c20 225b 5d5d 2229 0d0a 2020 2020  ]", "[]]")..    
-0000f640: 2020 2020 2020 2020 2020 2020 6172 6773              args
-0000f650: 5f73 6f75 7263 655f 7061 7468 5b69 5d20  _source_path[i] 
-0000f660: 3d20 6172 6773 5f73 6f75 7263 655f 7061  = args_source_pa
-0000f670: 7468 5b69 5d2e 7265 706c 6163 6528 706c  th[i].replace(pl
-0000f680: 6163 6568 6f6c 6465 722c 2022 5b5b 5d22  aceholder, "[[]"
-0000f690: 290d 0a0d 0a20 2020 2066 6f72 2061 7267  )....    for arg
-0000f6a0: 2069 6e20 6172 6773 5f73 6f75 7263 655f   in args_source_
-0000f6b0: 7061 7468 3a0d 0a20 2020 2020 2020 2069  path:..        i
-0000f6c0: 6620 6e6f 7420 7379 732e 706c 6174 666f  f not sys.platfo
-0000f6d0: 726d 203d 3d20 2277 696e 3332 2220 3a0d  rm == "win32" :.
-0000f6e0: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
-0000f6f0: 203d 2065 7363 6170 6528 6172 6729 0d0a   = escape(arg)..
-0000f700: 0d0a 2020 2020 2020 2020 6172 675f 6669  ..        arg_fi
-0000f710: 6c65 7061 7468 7320 2b3d 2067 6c6f 6228  lepaths += glob(
-0000f720: 6172 6729 0d0a 0d0a 2020 2020 6966 2061  arg)....    if a
-0000f730: 7267 5f66 696c 6570 6174 6873 3a0d 0a20  rg_filepaths:.. 
-0000f740: 2020 2020 2020 2066 6f72 2061 7267 7061         for argpa
-0000f750: 7468 2069 6e20 6172 675f 6669 6c65 7061  th in arg_filepa
-0000f760: 7468 733a 0d0a 2020 2020 2020 2020 2020  ths:..          
-0000f770: 2020 6966 206f 732e 7061 7468 2e69 7366    if os.path.isf
-0000f780: 696c 6528 6172 6770 6174 6829 3a0d 0a20  ile(argpath):.. 
-0000f790: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f7a0: 6620 6368 6563 6b5f 6669 6c65 5f74 7970  f check_file_typ
-0000f7b0: 6528 6172 6770 6174 682c 2065 7272 6f72  e(argpath, error
-0000f7c0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
-0000f7d0: 636b 3d73 686f 775f 6572 726f 725f 6d65  ck=show_error_me
-0000f7e0: 7373 6167 6573 2920 3d3d 2027 7669 6465  ssages) == 'vide
-0000f7f0: 6f27 206f 7220 6368 6563 6b5f 6669 6c65  o' or check_file
-0000f800: 5f74 7970 6528 6172 6770 6174 682c 2065  _type(argpath, e
-0000f810: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000f820: 6c6c 6261 636b 3d73 686f 775f 6572 726f  llback=show_erro
-0000f830: 725f 6d65 7373 6167 6573 2920 3d3d 2027  r_messages) == '
-0000f840: 6175 6469 6f27 3a0d 0a20 2020 2020 2020  audio':..       
-0000f850: 2020 2020 2020 2020 2020 2020 206d 6564               med
-0000f860: 6961 5f66 696c 6570 6174 6873 2e61 7070  ia_filepaths.app
-0000f870: 656e 6428 6172 6770 6174 6829 0d0a 2020  end(argpath)..  
-0000f880: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000f890: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000f8a0: 2020 2020 2020 2020 2069 6e76 616c 6964           invalid
-0000f8b0: 5f6d 6564 6961 5f66 696c 6570 6174 6873  _media_filepaths
-0000f8c0: 2e61 7070 656e 6428 6172 6770 6174 6829  .append(argpath)
-0000f8d0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0000f8e0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000f8f0: 2020 2020 206e 6f74 5f65 7869 7374 5f66       not_exist_f
-0000f900: 696c 6570 6174 6873 2e61 7070 656e 6428  ilepaths.append(
-0000f910: 6172 6770 6174 6829 0d0a 0d0a 2020 2020  argpath)....    
-0000f920: 2020 2020 6966 2069 6e76 616c 6964 5f6d      if invalid_m
-0000f930: 6564 6961 5f66 696c 6570 6174 6873 3a0d  edia_filepaths:.
-0000f940: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000f950: 2069 6e76 616c 6964 5f6d 6564 6961 5f66   invalid_media_f
-0000f960: 696c 6570 6174 6820 696e 2069 6e76 616c  ilepath in inval
-0000f970: 6964 5f6d 6564 6961 5f66 696c 6570 6174  id_media_filepat
-0000f980: 6873 3a0d 0a20 2020 2020 2020 2020 2020  hs:..           
-0000f990: 2020 2020 206d 7367 203d 2022 7b7d 2069       msg = "{} i
-0000f9a0: 7320 6e6f 7420 7661 6c69 6420 7669 6465  s not valid vide
-0000f9b0: 6f20 6f72 2061 7564 696f 2066 696c 6573  o or audio files
-0000f9c0: 222e 666f 726d 6174 2869 6e76 616c 6964  ".format(invalid
-0000f9d0: 5f6d 6564 6961 5f66 696c 6570 6174 6829  _media_filepath)
-0000f9e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f9f0: 2020 7072 696e 7428 6d73 6729 0d0a 0d0a    print(msg)....
-0000fa00: 2020 2020 6966 206e 6f74 5f65 7869 7374      if not_exist
-0000fa10: 5f66 696c 6570 6174 6873 3a0d 0a20 2020  _filepaths:..   
-0000fa20: 2020 2020 2066 6f72 206e 6f74 5f65 7869       for not_exi
-0000fa30: 7374 5f66 696c 6570 6174 6820 696e 206e  st_filepath in n
-0000fa40: 6f74 5f65 7869 7374 5f66 696c 6570 6174  ot_exist_filepat
-0000fa50: 6873 3a0d 0a20 2020 2020 2020 2020 2020  hs:..           
-0000fa60: 206d 7367 203d 2022 7b7d 2069 7320 6e6f   msg = "{} is no
-0000fa70: 7420 6578 6973 7422 2e66 6f72 6d61 7428  t exist".format(
-0000fa80: 6e6f 745f 6578 6973 745f 6669 6c65 7061  not_exist_filepa
-0000fa90: 7468 290d 0a20 2020 2020 2020 2020 2020  th)..           
-0000faa0: 2070 7269 6e74 286d 7367 290d 0a20 2020   print(msg)..   
-0000fab0: 2020 2020 2069 6620 286e 6f74 2028 222a       if (not ("*
-0000fac0: 2220 616e 6420 223f 2229 2069 6e20 7374  " and "?") in st
-0000fad0: 7228 6172 6773 5f73 6f75 7263 655f 7061  r(args_source_pa
-0000fae0: 7468 2929 3a0d 0a20 2020 2020 2020 2020  th)):..         
-0000faf0: 2020 2073 7973 2e65 7869 7428 3029 0d0a     sys.exit(0)..
-0000fb00: 0d0a 2020 2020 6966 206e 6f74 2061 7267  ..    if not arg
-0000fb10: 5f66 696c 6570 6174 6873 2061 6e64 206e  _filepaths and n
-0000fb20: 6f74 206e 6f74 5f65 7869 7374 5f66 696c  ot not_exist_fil
-0000fb30: 6570 6174 6873 3a0d 0a20 2020 2020 2020  epaths:..       
-0000fb40: 2070 7269 6e74 2822 4e6f 2061 6e79 2066   print("No any f
-0000fb50: 696c 6573 206d 6174 6368 696e 6720 6669  iles matching fi
-0000fb60: 6c65 6e61 6d65 7320 796f 7520 7479 7065  lenames you type
-0000fb70: 6422 290d 0a20 2020 2020 2020 2073 7973  d")..        sys
-0000fb80: 2e65 7869 7428 3029 0d0a 0d0a 2020 2020  .exit(0)....    
-0000fb90: 706f 6f6c 203d 206d 756c 7469 7072 6f63  pool = multiproc
-0000fba0: 6573 7369 6e67 2e50 6f6f 6c28 6172 6773  essing.Pool(args
-0000fbb0: 2e63 6f6e 6375 7272 656e 6379 290d 0a0d  .concurrency)...
-0000fbc0: 0a20 2020 2074 7261 6e73 6372 6962 655f  .    transcribe_
-0000fbd0: 656e 645f 7469 6d65 203d 204e 6f6e 650d  end_time = None.
-0000fbe0: 0a20 2020 2074 7261 6e73 6372 6962 655f  .    transcribe_
-0000fbf0: 656c 6170 7365 645f 7469 6d65 203d 204e  elapsed_time = N
-0000fc00: 6f6e 650d 0a20 2020 2074 7261 6e73 6372  one..    transcr
-0000fc10: 6962 655f 7374 6172 745f 7469 6d65 203d  ibe_start_time =
-0000fc20: 2074 696d 652e 7469 6d65 2829 0d0a 2020   time.time()..  
-0000fc30: 2020 7461 736b 203d 2022 7472 616e 7363    task = "transc
-0000fc40: 7269 6265 220d 0a0d 0a20 2020 2069 6620  ribe"....    if 
-0000fc50: 6172 6773 2e73 7263 5f6c 616e 6775 6167  args.src_languag
-0000fc60: 6520 3d3d 2028 2262 6122 206f 7220 2262  e == ("ba" or "b
-0000fc70: 7222 206f 7220 2266 6f22 206f 7220 226e  r" or "fo" or "n
-0000fc80: 6e22 206f 7220 226f 6322 206f 7220 2274  n" or "oc" or "t
-0000fc90: 6c22 206f 7220 2262 6f22 2920 616e 6420  l" or "bo") and 
-0000fca0: 646f 5f74 7261 6e73 6c61 7465 3a0d 0a20  do_translate:.. 
-0000fcb0: 2020 2020 2020 2074 6173 6b20 3d20 2274         task = "t
-0000fcc0: 7261 6e73 6c61 7465 220d 0a20 2020 2020  ranslate"..     
-0000fcd0: 2020 2073 7263 5f6c 616e 6775 6167 6520     src_language 
-0000fce0: 3d20 2265 6e22 0d0a 0d0a 2020 2020 666f  = "en"....    fo
-0000fcf0: 7220 6d65 6469 615f 6669 6c65 7061 7468  r media_filepath
-0000fd00: 2069 6e20 6d65 6469 615f 6669 6c65 7061   in media_filepa
-0000fd10: 7468 733a 0d0a 2020 2020 2020 2020 7072  ths:..        pr
-0000fd20: 696e 7428 2250 726f 6365 7373 696e 6720  int("Processing 
-0000fd30: 7b7d 203a 222e 666f 726d 6174 286d 6564  {} :".format(med
-0000fd40: 6961 5f66 696c 6570 6174 6829 290d 0a0d  ia_filepath))...
-0000fd50: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-0000fd60: 2020 2020 2020 2020 2020 2023 6d61 726b             #mark
-0000fd70: 6572 3d27 e296 8827 0d0a 2020 2020 2020  er='...'..      
-0000fd80: 2020 2020 2020 7769 6467 6574 7320 3d20        widgets = 
-0000fd90: 5b22 436f 6e76 6572 7469 6e67 2074 6f20  ["Converting to 
-0000fda0: 6120 7465 6d70 6f72 6172 7920 5741 5620  a temporary WAV 
-0000fdb0: 6669 6c65 2020 2020 2020 3a20 222c 2050  file      : ", P
-0000fdc0: 6572 6365 6e74 6167 6528 292c 2027 2027  ercentage(), ' '
-0000fdd0: 2c20 4261 7228 6d61 726b 6572 3d27 2327  , Bar(marker='#'
-0000fde0: 292c 2027 2027 2c20 4554 4128 295d 0d0a  ), ' ', ETA()]..
-0000fdf0: 2020 2020 2020 2020 2020 2020 7062 6172              pbar
-0000fe00: 203d 2050 726f 6772 6573 7342 6172 2877   = ProgressBar(w
-0000fe10: 6964 6765 7473 3d77 6964 6765 7473 2c20  idgets=widgets, 
-0000fe20: 6d61 7876 616c 3d31 3030 292e 7374 6172  maxval=100).star
-0000fe30: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
-0000fe40: 2077 6176 5f63 6f6e 7665 7274 6572 203d   wav_converter =
-0000fe50: 2057 6176 436f 6e76 6572 7465 7228 7072   WavConverter(pr
-0000fe60: 6f67 7265 7373 5f63 616c 6c62 6163 6b3d  ogress_callback=
-0000fe70: 7368 6f77 5f70 726f 6772 6573 732c 2065  show_progress, e
-0000fe80: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-0000fe90: 6c6c 6261 636b 3d73 686f 775f 6572 726f  llback=show_erro
-0000fea0: 725f 6d65 7373 6167 6573 290d 0a20 2020  r_messages)..   
-0000feb0: 2020 2020 2020 2020 2077 6176 5f66 696c           wav_fil
-0000fec0: 6570 6174 682c 2073 616d 706c 655f 7261  epath, sample_ra
-0000fed0: 7465 203d 2077 6176 5f63 6f6e 7665 7274  te = wav_convert
-0000fee0: 6572 286d 6564 6961 5f66 696c 6570 6174  er(media_filepat
-0000fef0: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
-0000ff00: 7062 6172 2e66 696e 6973 6828 290d 0a0d  pbar.finish()...
-0000ff10: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
-0000ff20: 6465 7220 3d20 7761 7665 2e6f 7065 6e28  der = wave.open(
-0000ff30: 7761 765f 6669 6c65 7061 7468 290d 0a20  wav_filepath).. 
-0000ff40: 2020 2020 2020 2020 2020 2072 6174 6520             rate 
-0000ff50: 3d20 7265 6164 6572 2e67 6574 6672 616d  = reader.getfram
-0000ff60: 6572 6174 6528 290d 0a20 2020 2020 2020  erate()..       
-0000ff70: 2020 2020 2074 6f74 616c 5f64 7572 6174       total_durat
-0000ff80: 696f 6e20 3d20 7265 6164 6572 2e67 6574  ion = reader.get
-0000ff90: 6e66 7261 6d65 7328 2920 2f20 7261 7465  nframes() / rate
-0000ffa0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0000ffb0: 6164 6572 2e63 6c6f 7365 2829 0d0a 0d0a  ader.close()....
-0000ffc0: 2020 2020 2020 2020 2020 2020 7365 676d              segm
-0000ffd0: 656e 7473 2c20 696e 666f 203d 206d 6f64  ents, info = mod
-0000ffe0: 656c 2e74 7261 6e73 6372 6962 6528 7761  el.transcribe(wa
-0000fff0: 765f 6669 6c65 7061 7468 2c20 6265 616d  v_filepath, beam
-00010000: 5f73 697a 653d 352c 206c 616e 6775 6167  _size=5, languag
-00010010: 653d 7372 635f 6c61 6e67 7561 6765 2c20  e=src_language, 
-00010020: 7461 736b 3d74 6173 6b29 0d0a 0d0a 2020  task=task)....  
-00010030: 2020 2020 2020 2020 2020 7769 6467 6574            widget
-00010040: 7320 3d20 5b22 5065 7266 6f72 6d69 6e67  s = ["Performing
-00010050: 2073 7065 6563 6820 7265 636f 676e 6974   speech recognit
-00010060: 696f 6e20 2020 2020 2020 2020 2020 3a20  ion           : 
-00010070: 222c 2050 6572 6365 6e74 6167 6528 292c  ", Percentage(),
-00010080: 2027 2027 2c20 4261 7228 6d61 726b 6572   ' ', Bar(marker
-00010090: 3d27 2327 292c 2027 2027 2c20 4554 4128  ='#'), ' ', ETA(
-000100a0: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
-000100b0: 7062 6172 203d 2050 726f 6772 6573 7342  pbar = ProgressB
-000100c0: 6172 2877 6964 6765 7473 3d77 6964 6765  ar(widgets=widge
-000100d0: 7473 2c20 6d61 7876 616c 3d31 3030 292e  ts, maxval=100).
-000100e0: 7374 6172 7428 290d 0a0d 0a20 2020 2020  start()....     
-000100f0: 2020 2020 2020 2074 696d 6564 5f73 7562         timed_sub
-00010100: 7469 746c 6573 203d 205b 5d0d 0a20 2020  titles = []..   
-00010110: 2020 2020 2020 2020 2072 6567 696f 6e73           regions
-00010120: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00010130: 2020 2074 7261 6e73 6372 6970 7473 203d     transcripts =
-00010140: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00010150: 2066 6f72 2073 6567 6d65 6e74 2069 6e20   for segment in 
-00010160: 7365 676d 656e 7473 3a0d 0a20 2020 2020  segments:..     
-00010170: 2020 2020 2020 2020 2020 2073 7461 7274             start
-00010180: 203d 2073 6567 6d65 6e74 2e73 7461 7274   = segment.start
-00010190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000101a0: 2020 656e 6420 3d20 7365 676d 656e 742e    end = segment.
-000101b0: 656e 640d 0a20 2020 2020 2020 2020 2020  end..           
-000101c0: 2020 2020 2074 6578 7420 3d20 7365 676d       text = segm
-000101d0: 656e 742e 7465 7874 0d0a 2020 2020 2020  ent.text..      
-000101e0: 2020 2020 2020 2020 2020 7265 6769 6f6e            region
-000101f0: 732e 6170 7065 6e64 2828 7374 6172 742c  s.append((start,
-00010200: 2065 6e64 2929 0d0a 2020 2020 2020 2020   end))..        
-00010210: 2020 2020 2020 2020 7472 616e 7363 7269          transcri
-00010220: 7074 732e 6170 7065 6e64 2874 6578 7429  pts.append(text)
-00010230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010240: 2020 7072 6f67 7265 7373 203d 2069 6e74    progress = int
-00010250: 2865 6e64 292a 3130 302f 746f 7461 6c5f  (end)*100/total_
-00010260: 6475 7261 7469 6f6e 0d0a 2020 2020 2020  duration..      
-00010270: 2020 2020 2020 2020 2020 7062 6172 2e75            pbar.u
-00010280: 7064 6174 6528 7072 6f67 7265 7373 290d  pdate(progress).
-00010290: 0a20 2020 2020 2020 2020 2020 2070 6261  .            pba
-000102a0: 722e 6669 6e69 7368 2829 0d0a 2020 2020  r.finish()..    
-000102b0: 2020 2020 2020 2020 7469 6d65 645f 7375          timed_su
-000102c0: 6274 6974 6c65 7320 3d20 5b28 722c 2074  btitles = [(r, t
-000102d0: 2920 666f 7220 722c 2074 2069 6e20 7a69  ) for r, t in zi
-000102e0: 7028 7265 6769 6f6e 732c 2074 7261 6e73  p(regions, trans
-000102f0: 6372 6970 7473 2920 6966 2074 5d0d 0a0d  cripts) if t]...
-00010300: 0a20 2020 2020 2020 2020 2020 2073 7562  .            sub
-00010310: 7469 746c 655f 666f 726d 6174 203d 2061  title_format = a
-00010320: 7267 732e 666f 726d 6174 0d0a 2020 2020  rgs.format..    
-00010330: 2020 2020 2020 2020 6261 7365 2c20 6578          base, ex
-00010340: 7420 3d20 6f73 2e70 6174 682e 7370 6c69  t = os.path.spli
-00010350: 7465 7874 286d 6564 6961 5f66 696c 6570  text(media_filep
-00010360: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
-00010370: 2020 7375 6274 6974 6c65 5f66 696c 6570    subtitle_filep
-00010380: 6174 6820 3d20 227b 6261 7365 7d2e 7b66  ath = "{base}.{f
-00010390: 6f72 6d61 747d 222e 666f 726d 6174 2862  ormat}".format(b
-000103a0: 6173 653d 6261 7365 2c20 666f 726d 6174  ase=base, format
-000103b0: 3d73 7562 7469 746c 655f 666f 726d 6174  =subtitle_format
-000103c0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000103d0: 2077 7269 7465 7220 3d20 5375 6274 6974   writer = Subtit
-000103e0: 6c65 5772 6974 6572 2872 6567 696f 6e73  leWriter(regions
-000103f0: 2c20 7472 616e 7363 7269 7074 732c 2073  , transcripts, s
-00010400: 7562 7469 746c 655f 666f 726d 6174 2c20  ubtitle_format, 
-00010410: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-00010420: 616c 6c62 6163 6b3d 7368 6f77 5f65 7272  allback=show_err
-00010430: 6f72 5f6d 6573 7361 6765 7329 0d0a 2020  or_messages)..  
-00010440: 2020 2020 2020 2020 2020 7772 6974 6572            writer
-00010450: 2e77 7269 7465 2873 7562 7469 746c 655f  .write(subtitle_
-00010460: 6669 6c65 7061 7468 290d 0a0d 0a20 2020  filepath)....   
-00010470: 2020 2020 2020 2020 2069 6620 646f 5f74           if do_t
-00010480: 7261 6e73 6c61 7465 3a0d 0a20 2020 2020  ranslate:..     
-00010490: 2020 2020 2020 2020 2020 2023 2043 4f4e             # CON
-000104a0: 4355 5252 454e 5420 5452 414e 534c 4154  CURRENT TRANSLAT
-000104b0: 494f 4e20 5553 494e 4720 636c 6173 7320  ION USING class 
-000104c0: 5365 6e74 656e 6365 5472 616e 736c 6174  SentenceTranslat
-000104d0: 6f72 286f 626a 6563 7429 0d0a 2020 2020  or(object)..    
-000104e0: 2020 2020 2020 2020 2020 2020 2320 4e4f              # NO
-000104f0: 204e 4545 4420 544f 2054 5241 4e53 4c41   NEED TO TRANSLA
-00010500: 5445 2041 4c4c 2074 7261 6e73 6372 6970  TE ALL transcrip
-00010510: 7420 494e 2074 7261 6e73 6372 6970 7473  t IN transcripts
-00010520: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010530: 2020 2320 4245 4341 5553 4520 534f 4d45    # BECAUSE SOME
-00010540: 2072 6567 696f 6e20 494e 2072 6567 696f   region IN regio
-00010550: 6e73 204d 4159 204a 5553 5420 4841 5645  ns MAY JUST HAVE
-00010560: 2074 7261 6e73 6372 6970 7420 5749 5448   transcript WITH
-00010570: 2045 4d50 5459 2053 5452 494e 470d 0a20   EMPTY STRING.. 
-00010580: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00010590: 204a 5553 5420 5452 414e 534c 4154 4520   JUST TRANSLATE 
-000105a0: 414c 5245 4144 5920 4352 4541 5445 4420  ALREADY CREATED 
-000105b0: 7375 6274 6974 6c65 7320 454e 5452 4945  subtitles ENTRIE
-000105c0: 5320 4652 4f4d 2074 696d 6564 5f73 7562  S FROM timed_sub
-000105d0: 7469 746c 6573 0d0a 2020 2020 2020 2020  titles..        
-000105e0: 2020 2020 2020 2020 7469 6d65 645f 7375          timed_su
-000105f0: 6274 6974 6c65 7320 3d20 7772 6974 6572  btitles = writer
-00010600: 2e74 696d 6564 5f73 7562 7469 746c 6573  .timed_subtitles
-00010610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010620: 2020 6372 6561 7465 645f 7265 6769 6f6e    created_region
-00010630: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00010640: 2020 2020 2020 2020 6372 6561 7465 645f          created_
-00010650: 7375 6274 6974 6c65 7320 3d20 5b5d 0d0a  subtitles = []..
-00010660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010670: 666f 7220 656e 7472 7920 696e 2074 696d  for entry in tim
-00010680: 6564 5f73 7562 7469 746c 6573 3a0d 0a20  ed_subtitles:.. 
-00010690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106a0: 2020 2063 7265 6174 6564 5f72 6567 696f     created_regio
-000106b0: 6e73 2e61 7070 656e 6428 656e 7472 795b  ns.append(entry[
-000106c0: 305d 290d 0a20 2020 2020 2020 2020 2020  0])..           
-000106d0: 2020 2020 2020 2020 2063 7265 6174 6564           created
-000106e0: 5f73 7562 7469 746c 6573 2e61 7070 656e  _subtitles.appen
-000106f0: 6428 656e 7472 795b 315d 290d 0a0d 0a20  d(entry[1]).... 
-00010700: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00010710: 726f 6d70 7420 3d20 2254 7261 6e73 6c61  rompt = "Transla
-00010720: 7469 6e67 2066 726f 6d20 2573 2074 6f20  ting from %s to 
-00010730: 2573 2020 203a 2022 2025 2873 7263 5f6c  %s   : " %(src_l
-00010740: 616e 6775 6167 652e 6365 6e74 6572 2838  anguage.center(8
-00010750: 292c 2064 7374 5f6c 616e 6775 6167 652e  ), dst_language.
-00010760: 6365 6e74 6572 2838 2929 0d0a 2020 2020  center(8))..    
-00010770: 2020 2020 2020 2020 2020 2020 7769 6467              widg
-00010780: 6574 7320 3d20 5b70 726f 6d70 742c 2050  ets = [prompt, P
-00010790: 6572 6365 6e74 6167 6528 292c 2027 2027  ercentage(), ' '
-000107a0: 2c20 4261 7228 6d61 726b 6572 3d27 2327  , Bar(marker='#'
-000107b0: 292c 2027 2027 2c20 4554 4128 295d 0d0a  ), ' ', ETA()]..
-000107c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107d0: 7062 6172 203d 2050 726f 6772 6573 7342  pbar = ProgressB
-000107e0: 6172 2877 6964 6765 7473 3d77 6964 6765  ar(widgets=widge
-000107f0: 7473 2c20 6d61 7876 616c 3d6c 656e 2874  ts, maxval=len(t
-00010800: 696d 6564 5f73 7562 7469 746c 6573 2929  imed_subtitles))
-00010810: 2e73 7461 7274 2829 0d0a 0d0a 2020 2020  .start()....    
-00010820: 2020 2020 2020 2020 2020 2020 7472 616e              tran
-00010830: 7363 7269 7074 5f74 7261 6e73 6c61 746f  script_translato
-00010840: 7220 3d20 5365 6e74 656e 6365 5472 616e  r = SentenceTran
-00010850: 736c 6174 6f72 2873 7263 3d61 7267 732e  slator(src=args.
-00010860: 7372 635f 6c61 6e67 7561 6765 2c20 6473  src_language, ds
-00010870: 743d 6172 6773 2e64 7374 5f6c 616e 6775  t=args.dst_langu
-00010880: 6167 652c 2065 7272 6f72 5f6d 6573 7361  age, error_messa
-00010890: 6765 735f 6361 6c6c 6261 636b 3d73 686f  ges_callback=sho
-000108a0: 775f 6572 726f 725f 6d65 7373 6167 6573  w_error_messages
-000108b0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000108c0: 2020 2020 2074 7261 6e73 6c61 7465 645f       translated_
-000108d0: 7375 6274 6974 6c65 7320 3d20 5b5d 0d0a  subtitles = []..
-000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108f0: 666f 7220 692c 2074 7261 6e73 6c61 7465  for i, translate
-00010900: 645f 7375 6274 6974 6c65 2069 6e20 656e  d_subtitle in en
-00010910: 756d 6572 6174 6528 706f 6f6c 2e69 6d61  umerate(pool.ima
-00010920: 7028 7472 616e 7363 7269 7074 5f74 7261  p(transcript_tra
-00010930: 6e73 6c61 746f 722c 2063 7265 6174 6564  nslator, created
-00010940: 5f73 7562 7469 746c 6573 2929 3a0d 0a20  _subtitles)):.. 
-00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010960: 2020 2074 7261 6e73 6c61 7465 645f 7375     translated_su
-00010970: 6274 6974 6c65 732e 6170 7065 6e64 2874  btitles.append(t
-00010980: 7261 6e73 6c61 7465 645f 7375 6274 6974  ranslated_subtit
-00010990: 6c65 290d 0a20 2020 2020 2020 2020 2020  le)..           
-000109a0: 2020 2020 2020 2020 2070 6261 722e 7570           pbar.up
-000109b0: 6461 7465 2869 290d 0a20 2020 2020 2020  date(i)..       
-000109c0: 2020 2020 2020 2020 2070 6261 722e 6669           pbar.fi
-000109d0: 6e69 7368 2829 0d0a 0d0a 2020 2020 2020  nish()....      
-000109e0: 2020 2020 2020 2020 2020 7472 616e 736c            transl
-000109f0: 6174 6564 5f73 7562 7469 746c 655f 6669  ated_subtitle_fi
-00010a00: 6c65 7061 7468 203d 2073 7562 7469 746c  lepath = subtitl
-00010a10: 655f 6669 6c65 7061 7468 5b20 3a2d 345d  e_filepath[ :-4]
-00010a20: 202b 2027 2e74 7261 6e73 6c61 7465 642e   + '.translated.
-00010a30: 2720 2b20 7375 6274 6974 6c65 5f66 6f72  ' + subtitle_for
-00010a40: 6d61 740d 0a20 2020 2020 2020 2020 2020  mat..           
-00010a50: 2020 2020 2074 7261 6e73 6c61 7469 6f6e       translation
-00010a60: 5f77 7269 7465 7220 3d20 5375 6274 6974  _writer = Subtit
-00010a70: 6c65 5772 6974 6572 2863 7265 6174 6564  leWriter(created
-00010a80: 5f72 6567 696f 6e73 2c20 7472 616e 736c  _regions, transl
-00010a90: 6174 6564 5f73 7562 7469 746c 6573 2c20  ated_subtitles, 
-00010aa0: 7375 6274 6974 6c65 5f66 6f72 6d61 742c  subtitle_format,
-00010ab0: 2065 7272 6f72 5f6d 6573 7361 6765 735f   error_messages_
-00010ac0: 6361 6c6c 6261 636b 3d73 686f 775f 6572  callback=show_er
-00010ad0: 726f 725f 6d65 7373 6167 6573 290d 0a20  ror_messages).. 
-00010ae0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00010af0: 7261 6e73 6c61 7469 6f6e 5f77 7269 7465  ranslation_write
-00010b00: 722e 7772 6974 6528 7472 616e 736c 6174  r.write(translat
-00010b10: 6564 5f73 7562 7469 746c 655f 6669 6c65  ed_subtitle_file
-00010b20: 7061 7468 290d 0a0d 0a20 2020 2020 2020  path)....       
-00010b30: 2020 2020 2070 7269 6e74 2827 446f 6e65       print('Done
-00010b40: 2e27 290d 0a20 2020 2020 2020 2020 2020  .')..           
-00010b50: 2069 6620 646f 5f74 7261 6e73 6c61 7465   if do_translate
-00010b60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00010b70: 2020 206f 732e 7265 6d6f 7665 2873 7562     os.remove(sub
-00010b80: 7469 746c 655f 6669 6c65 7061 7468 290d  title_filepath).
-00010b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010ba0: 2070 7269 6e74 2827 5472 616e 736c 6174   print('Translat
-00010bb0: 6564 2073 7562 7469 746c 6573 2066 696c  ed subtitles fil
-00010bc0: 6520 6372 6561 7465 6420 6174 2020 2020  e created at    
-00010bd0: 3a20 7b7d 2720 2e66 6f72 6d61 7428 7472  : {}' .format(tr
-00010be0: 616e 736c 6174 6564 5f73 7562 7469 746c  anslated_subtitl
-00010bf0: 655f 6669 6c65 7061 7468 2929 0d0a 2020  e_filepath))..  
-00010c00: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00010c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010c20: 2070 7269 6e74 2822 5375 6274 6974 6c65   print("Subtitle
-00010c30: 7320 6669 6c65 2063 7265 6174 6564 2061  s file created a
-00010c40: 7420 2020 2020 2020 2020 2020 2020 2020  t               
-00010c50: 3a20 7b7d 222e 666f 726d 6174 2873 7562  : {}".format(sub
-00010c60: 7469 746c 655f 6669 6c65 7061 7468 2929  title_filepath))
-00010c70: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00010c80: 696e 7428 2727 290d 0a20 2020 2020 2020  int('')..       
-00010c90: 2020 2020 2063 6f6d 706c 6574 6564 5f74       completed_t
-00010ca0: 6173 6b73 202b 3d20 310d 0a0d 0a20 2020  asks += 1....   
-00010cb0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00010cc0: 6d65 6469 615f 6669 6c65 7061 7468 7329  media_filepaths)
-00010cd0: 3e30 2061 6e64 2063 6f6d 706c 6574 6564  >0 and completed
-00010ce0: 5f74 6173 6b73 203d 3d20 6c65 6e28 6d65  _tasks == len(me
-00010cf0: 6469 615f 6669 6c65 7061 7468 7329 3a0d  dia_filepaths):.
-00010d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010d10: 2074 7261 6e73 6372 6962 655f 656e 645f   transcribe_end_
-00010d20: 7469 6d65 203d 2074 696d 652e 7469 6d65  time = time.time
-00010d30: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00010d40: 2020 2020 7472 616e 7363 7269 6265 5f65      transcribe_e
-00010d50: 6c61 7073 6564 5f74 696d 6520 3d20 7472  lapsed_time = tr
-00010d60: 616e 7363 7269 6265 5f65 6e64 5f74 696d  anscribe_end_tim
-00010d70: 6520 2d20 7472 616e 7363 7269 6265 5f73  e - transcribe_s
-00010d80: 7461 7274 5f74 696d 650d 0a20 2020 2020  tart_time..     
-00010d90: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
-00010da0: 6372 6962 655f 656c 6170 7365 645f 7469  cribe_elapsed_ti
-00010db0: 6d65 5f73 6563 6f6e 6473 203d 2074 696d  me_seconds = tim
-00010dc0: 6564 656c 7461 2873 6563 6f6e 6473 3d69  edelta(seconds=i
-00010dd0: 6e74 2874 7261 6e73 6372 6962 655f 656c  nt(transcribe_el
-00010de0: 6170 7365 645f 7469 6d65 2929 0d0a 2020  apsed_time))..  
-00010df0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00010e00: 616e 7363 7269 6265 5f65 6c61 7073 6564  anscribe_elapsed
-00010e10: 5f74 696d 655f 7374 7220 3d20 7374 7228  _time_str = str(
-00010e20: 7472 616e 7363 7269 6265 5f65 6c61 7073  transcribe_elaps
-00010e30: 6564 5f74 696d 655f 7365 636f 6e64 7329  ed_time_seconds)
-00010e40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010e50: 2020 686f 7572 2c20 6d69 6e75 7465 2c20    hour, minute, 
-00010e60: 7365 636f 6e64 203d 2074 7261 6e73 6372  second = transcr
-00010e70: 6962 655f 656c 6170 7365 645f 7469 6d65  ibe_elapsed_time
-00010e80: 5f73 7472 2e73 706c 6974 2822 3a22 290d  _str.split(":").
-00010e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010ea0: 206d 7367 203d 2022 546f 7461 6c20 7472   msg = "Total tr
-00010eb0: 616e 7363 7269 6265 2074 696d 6520 2020  anscribe time   
-00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ed0: 3a20 2573 3a25 733a 2573 2220 2528 686f  : %s:%s:%s" %(ho
-00010ee0: 7572 2e7a 6669 6c6c 2832 292c 206d 696e  ur.zfill(2), min
-00010ef0: 7574 652c 2073 6563 6f6e 6429 0d0a 2020  ute, second)..  
-00010f00: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00010f10: 696e 7428 6d73 6729 0d0a 0d0a 2020 2020  int(msg)....    
-00010f20: 2020 2020 6578 6365 7074 204b 6579 626f      except Keybo
-00010f30: 6172 6449 6e74 6572 7275 7074 3a0d 0a20  ardInterrupt:.. 
-00010f40: 2020 2020 2020 2020 2020 2070 6261 722e             pbar.
-00010f50: 6669 6e69 7368 2829 0d0a 2020 2020 2020  finish()..      
-00010f60: 2020 2020 2020 706f 6f6c 2e74 6572 6d69        pool.termi
-00010f70: 6e61 7465 2829 0d0a 2020 2020 2020 2020  nate()..        
-00010f80: 2020 2020 706f 6f6c 2e63 6c6f 7365 2829      pool.close()
-00010f90: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
-00010fa0: 6f6c 2e6a 6f69 6e28 290d 0a20 2020 2020  ol.join()..     
-00010fb0: 2020 2020 2020 2070 7269 6e74 2822 4361         print("Ca
-00010fc0: 6e63 656c 6c69 6e67 2061 6c6c 2074 6173  ncelling all tas
-00010fd0: 6b73 2229 0d0a 0d0a 2020 2020 2020 2020  ks")....        
-00010fe0: 2020 2020 6966 2073 7973 2e70 6c61 7466      if sys.platf
-00010ff0: 6f72 6d20 3d3d 2022 7769 6e33 3222 3a0d  orm == "win32":.
-00011000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011010: 2073 746f 705f 6666 6d70 6567 5f77 696e   stop_ffmpeg_win
-00011020: 646f 7773 2865 7272 6f72 5f6d 6573 7361  dows(error_messa
-00011030: 6765 735f 6361 6c6c 6261 636b 3d73 686f  ges_callback=sho
-00011040: 775f 6572 726f 725f 6d65 7373 6167 6573  w_error_messages
-00011050: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00011060: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00011070: 2020 2020 2020 7374 6f70 5f66 666d 7065        stop_ffmpe
-00011080: 675f 6c69 6e75 7828 6572 726f 725f 6d65  g_linux(error_me
-00011090: 7373 6167 6573 5f63 616c 6c62 6163 6b3d  ssages_callback=
-000110a0: 7368 6f77 5f65 7272 6f72 5f6d 6573 7361  show_error_messa
-000110b0: 6765 7329 0d0a 0d0a 2020 2020 2020 2020  ges)....        
-000110c0: 2020 2020 7265 6d6f 7665 5f74 656d 705f      remove_temp_
-000110d0: 6669 6c65 7328 2277 6176 2229 0d0a 2020  files("wav")..  
-000110e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000110f0: 2031 0d0a 0d0a 2020 2020 2020 2020 6578   1....        ex
-00011100: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00011110: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
-00011120: 2020 6966 206e 6f74 204b 6579 626f 6172    if not Keyboar
-00011130: 6449 6e74 6572 7275 7074 2069 6e20 653a  dInterrupt in e:
-00011140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011150: 2020 7062 6172 2e66 696e 6973 6828 290d    pbar.finish().
-00011160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011170: 2070 6f6f 6c2e 7465 726d 696e 6174 6528   pool.terminate(
-00011180: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00011190: 2020 2070 6f6f 6c2e 636c 6f73 6528 290d     pool.close().
-000111a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000111b0: 2070 6f6f 6c2e 6a6f 696e 2829 0d0a 2020   pool.join()..  
-000111c0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000111d0: 696e 7428 6529 0d0a 0d0a 2020 2020 2020  int(e)....      
-000111e0: 2020 2020 2020 2020 2020 6966 2073 7973            if sys
-000111f0: 2e70 6c61 7466 6f72 6d20 3d3d 2022 7769  .platform == "wi
-00011200: 6e33 3222 3a0d 0a20 2020 2020 2020 2020  n32":..         
-00011210: 2020 2020 2020 2020 2020 2073 746f 705f             stop_
-00011220: 6666 6d70 6567 5f77 696e 646f 7773 2865  ffmpeg_windows(e
-00011230: 7272 6f72 5f6d 6573 7361 6765 735f 6361  rror_messages_ca
-00011240: 6c6c 6261 636b 3d73 686f 775f 6572 726f  llback=show_erro
-00011250: 725f 6d65 7373 6167 6573 290d 0a20 2020  r_messages)..   
-00011260: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00011270: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00011280: 2020 2020 2020 2020 7374 6f70 5f66 666d          stop_ffm
-00011290: 7065 675f 6c69 6e75 7828 6572 726f 725f  peg_linux(error_
-000112a0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
-000112b0: 6b3d 7368 6f77 5f65 7272 6f72 5f6d 6573  k=show_error_mes
-000112c0: 7361 6765 7329 0d0a 0d0a 2020 2020 2020  sages)....      
-000112d0: 2020 2020 2020 2020 2020 7265 6d6f 7665            remove
-000112e0: 5f74 656d 705f 6669 6c65 7328 2277 6176  _temp_files("wav
-000112f0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00011300: 2020 2020 7265 7475 726e 2031 0d0a 0d0a      return 1....
-00011310: 2020 2020 6966 2070 6f6f 6c3a 0d0a 2020      if pool:..  
-00011320: 2020 2020 2020 706f 6f6c 2e63 6c6f 7365        pool.close
-00011330: 2829 0d0a 2020 2020 2020 2020 706f 6f6c  ()..        pool
-00011340: 2e6a 6f69 6e28 290d 0a20 2020 2020 2020  .join()..       
-00011350: 2070 6f6f 6c20 3d20 4e6f 6e65 0d0a 0d0a   pool = None....
-00011360: 2020 2020 6966 2073 7973 2e70 6c61 7466      if sys.platf
-00011370: 6f72 6d20 3d3d 2022 7769 6e33 3222 3a0d  orm == "win32":.
-00011380: 0a20 2020 2020 2020 2073 746f 705f 6666  .        stop_ff
-00011390: 6d70 6567 5f77 696e 646f 7773 2865 7272  mpeg_windows(err
-000113a0: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
-000113b0: 6261 636b 3d73 686f 775f 6572 726f 725f  back=show_error_
-000113c0: 6d65 7373 6167 6573 290d 0a20 2020 2065  messages)..    e
-000113d0: 6c73 653a 0d0a 2020 2020 2020 2020 7374  lse:..        st
-000113e0: 6f70 5f66 666d 7065 675f 6c69 6e75 7828  op_ffmpeg_linux(
-000113f0: 6572 726f 725f 6d65 7373 6167 6573 5f63  error_messages_c
-00011400: 616c 6c62 6163 6b3d 7368 6f77 5f65 7272  allback=show_err
-00011410: 6f72 5f6d 6573 7361 6765 7329 0d0a 0d0a  or_messages)....
-00011420: 2020 2020 7265 6d6f 7665 5f74 656d 705f      remove_temp_
-00011430: 6669 6c65 7328 2277 6176 2229 0d0a 0d0a  files("wav")....
-00011440: 6966 205f 5f6e 616d 655f 5f20 3d3d 2027  if __name__ == '
-00011450: 5f5f 6d61 696e 5f5f 273a 0d0a 2020 2020  __main__':..    
-00011460: 6d75 6c74 6970 726f 6365 7373 696e 672e  multiprocessing.
-00011470: 6672 6565 7a65 5f73 7570 706f 7274 2829  freeze_support()
-00011480: 0d0a 2020 2020 7379 732e 6578 6974 286d  ..    sys.exit(m
-00011490: 6169 6e28 2929 0d0a                      ain())..
+0000db40: 2020 2074 696d 655f 666f 726d 6174 203d     time_format =
+0000db50: 2027 2548 3a25 4d3a 2553 2c25 6627 0d0a   '%H:%M:%S,%f'..
+0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db70: 2020 2020 2020 2020 7374 6172 745f 7469          start_ti
+0000db80: 6d65 5f74 696d 655f 6465 6c74 6120 3d20  me_time_delta = 
+0000db90: 6461 7465 7469 6d65 2e73 7472 7074 696d  datetime.strptim
+0000dba0: 6528 7374 6172 745f 7469 6d65 5f73 7472  e(start_time_str
+0000dbb0: 2c20 7469 6d65 5f66 6f72 6d61 7429 202d  , time_format) -
+0000dbc0: 2064 6174 6574 696d 652e 7374 7270 7469   datetime.strpti
+0000dbd0: 6d65 2827 3030 3a30 303a 3030 2c30 3030  me('00:00:00,000
+0000dbe0: 272c 2074 696d 655f 666f 726d 6174 290d  ', time_format).
+0000dbf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dc00: 2020 2020 2020 2020 2073 7461 7274 5f74           start_t
+0000dc10: 696d 655f 746f 7461 6c5f 7365 636f 6e64  ime_total_second
+0000dc20: 7320 3d20 7374 6172 745f 7469 6d65 5f74  s = start_time_t
+0000dc30: 696d 655f 6465 6c74 612e 746f 7461 6c5f  ime_delta.total_
+0000dc40: 7365 636f 6e64 7328 290d 0a20 2020 2020  seconds()..     
+0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc60: 2020 2065 6e64 5f74 696d 655f 7469 6d65     end_time_time
+0000dc70: 5f64 656c 7461 203d 2064 6174 6574 696d  _delta = datetim
+0000dc80: 652e 7374 7270 7469 6d65 2865 6e64 5f74  e.strptime(end_t
+0000dc90: 696d 655f 7374 722c 2074 696d 655f 666f  ime_str, time_fo
+0000dca0: 726d 6174 2920 2d20 6461 7465 7469 6d65  rmat) - datetime
+0000dcb0: 2e73 7472 7074 696d 6528 2730 303a 3030  .strptime('00:00
+0000dcc0: 3a30 302c 3030 3027 2c20 7469 6d65 5f66  :00,000', time_f
+0000dcd0: 6f72 6d61 7429 0d0a 2020 2020 2020 2020  ormat)..        
+0000dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcf0: 656e 645f 7469 6d65 5f74 6f74 616c 5f73  end_time_total_s
+0000dd00: 6563 6f6e 6473 203d 2065 6e64 5f74 696d  econds = end_tim
+0000dd10: 655f 7469 6d65 5f64 656c 7461 2e74 6f74  e_time_delta.tot
+0000dd20: 616c 5f73 6563 6f6e 6473 2829 0d0a 2020  al_seconds()..  
+0000dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd40: 2020 2020 2020 2320 4578 7472 6163 7420        # Extract 
+0000dd50: 7375 6274 6974 6c65 2074 6578 7420 6672  subtitle text fr
+0000dd60: 6f6d 2073 7562 7469 746c 6520 626c 6f63  om subtitle bloc
+0000dd70: 6b0d 0a20 2020 2020 2020 2020 2020 2020  k..             
+0000dd80: 2020 2020 2020 2020 2020 2073 7562 7469             subti
+0000dd90: 746c 6520 3d20 2720 272e 6a6f 696e 2862  tle = ' '.join(b
+0000dda0: 6c6f 636b 5b32 3a5d 290d 0a20 2020 2020  lock[2:])..     
+0000ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddc0: 2020 2074 696d 6564 5f73 7562 7469 746c     timed_subtitl
+0000ddd0: 6573 2e61 7070 656e 6428 2828 7374 6172  es.append(((star
+0000dde0: 745f 7469 6d65 5f74 6f74 616c 5f73 6563  t_time_total_sec
+0000ddf0: 6f6e 6473 2c20 656e 645f 7469 6d65 5f74  onds, end_time_t
+0000de00: 6f74 616c 5f73 6563 6f6e 6473 292c 2073  otal_seconds), s
+0000de10: 7562 7469 746c 6529 290d 0a20 2020 2020  ubtitle))..     
+0000de20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000de30: 6e20 7469 6d65 645f 7375 6274 6974 6c65  n timed_subtitle
+0000de40: 730d 0a0d 0a20 2020 2020 2020 2065 7863  s....        exc
+0000de50: 6570 7420 4b65 7962 6f61 7264 496e 7465  ept KeyboardInte
+0000de60: 7272 7570 743a 0d0a 2020 2020 2020 2020  rrupt:..        
+0000de70: 2020 2020 6966 2073 656c 662e 6572 726f      if self.erro
+0000de80: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000de90: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
+0000dea0: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
+0000deb0: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000dec0: 636b 2822 4361 6e63 656c 6c69 6e67 2061  ck("Cancelling a
+0000ded0: 6c6c 2074 6173 6b73 2229 0d0a 2020 2020  ll tasks")..    
+0000dee0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0000def0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000df00: 7269 6e74 2822 4361 6e63 656c 6c69 6e67  rint("Cancelling
+0000df10: 2061 6c6c 2074 6173 6b73 2229 0d0a 2020   all tasks")..  
+0000df20: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000df30: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
+0000df40: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+0000df50: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000df60: 6966 2073 656c 662e 6572 726f 725f 6d65  if self.error_me
+0000df70: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
+0000df80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000df90: 2020 7365 6c66 2e65 7272 6f72 5f6d 6573    self.error_mes
+0000dfa0: 7361 6765 735f 6361 6c6c 6261 636b 2865  sages_callback(e
+0000dfb0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+0000dfc0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0000dfd0: 2020 2020 2020 7072 696e 7428 6529 0d0a        print(e)..
+0000dfe0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000dff0: 726e 0d0a 0d0a 0d0a 6465 6620 7368 6f77  rn......def show
+0000e000: 5f70 726f 6772 6573 7328 6d65 6469 615f  _progress(media_
+0000e010: 6669 6c65 7061 7468 2c20 7072 6f67 7265  filepath, progre
+0000e020: 7373 293a 0d0a 2020 2020 676c 6f62 616c  ss):..    global
+0000e030: 2070 6261 720d 0a20 2020 2070 6261 722e   pbar..    pbar.
+0000e040: 7570 6461 7465 2870 726f 6772 6573 7329  update(progress)
+0000e050: 0d0a 0d0a 0d0a 6465 6620 7368 6f77 5f65  ......def show_e
+0000e060: 7272 6f72 5f6d 6573 7361 6765 7328 6d65  rror_messages(me
+0000e070: 7373 6167 6573 293a 0d0a 2020 2020 7072  ssages):..    pr
+0000e080: 696e 7428 6d65 7373 6167 6573 290d 0a0d  int(messages)...
+0000e090: 0a0d 0a64 6566 2067 6574 5f76 6964 656f  ...def get_video
+0000e0a0: 5f64 7572 6174 696f 6e28 6669 6c65 6e61  _duration(filena
+0000e0b0: 6d65 2c20 6572 726f 725f 6d65 7373 6167  me, error_messag
+0000e0c0: 6573 5f63 616c 6c62 6163 6b3d 4e6f 6e65  es_callback=None
+0000e0d0: 293a 0d0a 2020 2020 7472 793a 0d0a 2020  ):..    try:..  
+0000e0e0: 2020 2020 2020 636f 6d6d 616e 6420 3d20        command = 
+0000e0f0: 6627 6666 7072 6f62 6520 2d76 2065 7272  f'ffprobe -v err
+0000e100: 6f72 202d 7368 6f77 5f65 6e74 7269 6573  or -show_entries
+0000e110: 2066 6f72 6d61 743d 6475 7261 7469 6f6e   format=duration
+0000e120: 202d 6f66 2064 6566 6175 6c74 3d6e 6f70   -of default=nop
+0000e130: 7269 6e74 5f77 7261 7070 6572 733d 313a  rint_wrappers=1:
+0000e140: 6e6f 6b65 793d 3120 227b 6669 6c65 6e61  nokey=1 "{filena
+0000e150: 6d65 7d22 270d 0a20 2020 2020 2020 2072  me}"'..        r
+0000e160: 6573 756c 7420 3d20 7375 6270 726f 6365  esult = subproce
+0000e170: 7373 2e72 756e 2863 6f6d 6d61 6e64 2c20  ss.run(command, 
+0000e180: 6361 7074 7572 655f 6f75 7470 7574 3d54  capture_output=T
+0000e190: 7275 652c 2074 6578 743d 5472 7565 2c20  rue, text=True, 
+0000e1a0: 7368 656c 6c3d 5472 7565 290d 0a0d 0a20  shell=True).... 
+0000e1b0: 2020 2020 2020 2069 6620 7265 7375 6c74         if result
+0000e1c0: 2e72 6574 7572 6e63 6f64 6520 3d3d 2030  .returncode == 0
+0000e1d0: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+0000e1e0: 7572 6174 696f 6e20 3d20 666c 6f61 7428  uration = float(
+0000e1f0: 7265 7375 6c74 2e73 7464 6f75 7429 0d0a  result.stdout)..
+0000e200: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000e210: 726e 2064 7572 6174 696f 6e0d 0a20 2020  rn duration..   
+0000e220: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000e230: 2020 2020 2020 2020 6d73 6720 3d20 6622          msg = f"
+0000e240: 4661 696c 6564 2074 6f20 6765 7420 6475  Failed to get du
+0000e250: 7261 7469 6f6e 2066 6f72 207b 6669 6c65  ration for {file
+0000e260: 6e61 6d65 7d2e 220d 0a20 2020 2020 2020  name}."..       
+0000e270: 2020 2020 2069 6620 6572 726f 725f 6d65       if error_me
+0000e280: 7373 6167 6573 5f63 616c 6c62 6163 6b3a  ssages_callback:
+0000e290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e2a0: 2020 6572 726f 725f 6d65 7373 6167 6573    error_messages
+0000e2b0: 5f63 616c 6c62 6163 6b28 6d73 6729 0d0a  _callback(msg)..
+0000e2c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000e2d0: 726e 204e 6f6e 650d 0a0d 0a20 2020 2065  rn None....    e
+0000e2e0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+0000e2f0: 6173 2065 3a0d 0a20 2020 2020 2020 2069  as e:..        i
+0000e300: 6620 6572 726f 725f 6d65 7373 6167 6573  f error_messages
+0000e310: 5f63 616c 6c62 6163 6b3a 0d0a 2020 2020  _callback:..    
+0000e320: 2020 2020 2020 2020 6572 726f 725f 6d65          error_me
+0000e330: 7373 6167 6573 5f63 616c 6c62 6163 6b28  ssages_callback(
+0000e340: 6529 0d0a 2020 2020 2020 2020 656c 7365  e)..        else
+0000e350: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+0000e360: 7269 6e74 2865 290d 0a20 2020 2020 2020  rint(e)..       
+0000e370: 2072 6574 7572 6e0d 0a0d 0a0d 0a64 6566   return......def
+0000e380: 206d 6169 6e28 293a 0d0a 2020 2020 676c   main():..    gl
+0000e390: 6f62 616c 2070 6261 720d 0a0d 0a20 2020  obal pbar....   
+0000e3a0: 2077 6869 7370 6572 5f6d 6f64 656c 7320   whisper_models 
+0000e3b0: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
+0000e3c0: 2020 2020 2020 2020 2020 2020 2022 7469               "ti
+0000e3d0: 6e79 2e65 6e22 2c0d 0a20 2020 2020 2020  ny.en",..       
+0000e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3f0: 2022 7469 6e79 222c 0d0a 2020 2020 2020   "tiny",..      
+0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e410: 2020 2262 6173 652e 656e 222c 0d0a 2020    "base.en",..  
+0000e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e430: 2020 2020 2020 2262 6173 6522 2c0d 0a20        "base",.. 
+0000e440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e450: 2020 2020 2020 2022 736d 616c 6c2e 656e         "small.en
+0000e460: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0000e470: 2020 2020 2020 2020 2020 2020 2273 6d61              "sma
+0000e480: 6c6c 222c 0d0a 2020 2020 2020 2020 2020  ll",..          
+0000e490: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+0000e4a0: 6564 6975 6d2e 656e 222c 0d0a 2020 2020  edium.en",..    
+0000e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4c0: 2020 2020 226d 6564 6975 6d22 2c0d 0a20      "medium",.. 
+0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4e0: 2020 2020 2020 2022 6c61 7267 652d 7631         "large-v1
+0000e4f0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0000e500: 2020 2020 2020 2020 2020 2020 226c 6172              "lar
+0000e510: 6765 2d76 3222 2c0d 0a20 2020 2020 2020  ge-v2",..       
+0000e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e530: 2022 6c61 7267 6522 0d0a 2020 2020 5d0d   "large"..    ].
+0000e540: 0a0d 0a20 2020 2064 6576 6963 6573 203d  ...    devices =
+0000e550: 205b 2261 7574 6f22 2c20 2263 7564 6122   ["auto", "cuda"
+0000e560: 2c20 2263 7075 225d 0d0a 0d0a 2020 2020  , "cpu"]....    
+0000e570: 636f 6d70 7574 655f 7479 7065 7320 3d20  compute_types = 
+0000e580: 5b22 6465 6661 756c 7422 2c20 2261 7574  ["default", "aut
+0000e590: 6f22 2c20 2269 6e74 3822 2c20 2269 6e74  o", "int8", "int
+0000e5a0: 385f 666c 6f61 7431 3622 2c20 2269 6e74  8_float16", "int
+0000e5b0: 3136 222c 2022 666c 6f61 7431 3622 2c20  16", "float16", 
+0000e5c0: 2266 6c6f 6174 3332 225d 0d0a 0d0a 2020  "float32"]....  
+0000e5d0: 2020 6966 2073 7973 2e70 6c61 7466 6f72    if sys.platfor
+0000e5e0: 6d20 3d3d 2022 7769 6e33 3222 3a0d 0a20  m == "win32":.. 
+0000e5f0: 2020 2020 2020 2073 746f 705f 6666 6d70         stop_ffmp
+0000e600: 6567 5f77 696e 646f 7773 2865 7272 6f72  eg_windows(error
+0000e610: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+0000e620: 636b 3d73 686f 775f 6572 726f 725f 6d65  ck=show_error_me
+0000e630: 7373 6167 6573 290d 0a20 2020 2065 6c73  ssages)..    els
+0000e640: 653a 0d0a 2020 2020 2020 2020 7374 6f70  e:..        stop
+0000e650: 5f66 666d 7065 675f 6c69 6e75 7828 6572  _ffmpeg_linux(er
+0000e660: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+0000e670: 6c62 6163 6b3d 7368 6f77 5f65 7272 6f72  lback=show_error
+0000e680: 5f6d 6573 7361 6765 7329 0d0a 0d0a 2020  _messages)....  
+0000e690: 2020 7265 6d6f 7665 5f74 656d 705f 6669    remove_temp_fi
+0000e6a0: 6c65 7328 2266 6c61 6322 2c20 6572 726f  les("flac", erro
+0000e6b0: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+0000e6c0: 6163 6b3d 7368 6f77 5f65 7272 6f72 5f6d  ack=show_error_m
+0000e6d0: 6573 7361 6765 7329 0d0a 2020 2020 7265  essages)..    re
+0000e6e0: 6d6f 7665 5f74 656d 705f 6669 6c65 7328  move_temp_files(
+0000e6f0: 2277 6176 222c 2065 7272 6f72 5f6d 6573  "wav", error_mes
+0000e700: 7361 6765 735f 6361 6c6c 6261 636b 3d73  sages_callback=s
+0000e710: 686f 775f 6572 726f 725f 6d65 7373 6167  how_error_messag
+0000e720: 6573 290d 0a0d 0a20 2020 2070 6172 7365  es)....    parse
+0000e730: 7220 3d20 6172 6770 6172 7365 2e41 7267  r = argparse.Arg
+0000e740: 756d 656e 7450 6172 7365 7228 290d 0a20  umentParser().. 
+0000e750: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
+0000e760: 6775 6d65 6e74 2827 736f 7572 6365 5f70  gument('source_p
+0000e770: 6174 6827 2c20 6865 6c70 3d22 5061 7468  ath', help="Path
+0000e780: 2074 6f20 7468 6520 7669 6465 6f20 6f72   to the video or
+0000e790: 2061 7564 696f 2066 696c 6573 2074 6f20   audio files to 
+0000e7a0: 6765 6e65 7261 7465 2073 7562 7469 746c  generate subtitl
+0000e7b0: 6573 2066 696c 6573 2028 7573 6520 7769  es files (use wi
+0000e7c0: 6c64 6361 7264 2066 6f72 206d 756c 7469  ldcard for multi
+0000e7d0: 706c 6520 6669 6c65 7320 6f72 2073 6570  ple files or sep
+0000e7e0: 6172 6174 6520 7468 656d 2077 6974 6820  arate them with 
+0000e7f0: 6120 7370 6163 6520 6368 6172 6163 7465  a space characte
+0000e800: 7220 652e 672e 205c 2266 696c 6520 312e  r e.g. \"file 1.
+0000e810: 6d70 345c 2220 5c22 6669 6c65 2032 2e6d  mp4\" \"file 2.m
+0000e820: 7034 5c22 2922 2c20 6e61 7267 733d 272a  p4\")", nargs='*
+0000e830: 2729 0d0a 2020 2020 7061 7273 6572 2e61  ')..    parser.a
+0000e840: 6464 5f61 7267 756d 656e 7428 272d 6d27  dd_argument('-m'
+0000e850: 2c20 272d 2d6d 6f64 656c 2d6e 616d 6527  , '--model-name'
+0000e860: 2c20 6465 6661 756c 743d 2273 6d61 6c6c  , default="small
+0000e870: 222c 2068 656c 703d 226e 616d 6520 6f66  ", help="name of
+0000e880: 2077 6869 7370 6572 206d 6f64 656c 2074   whisper model t
+0000e890: 6f20 7573 6522 290d 0a20 2020 2070 6172  o use")..    par
+0000e8a0: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
+0000e8b0: 2827 2d6c 6d27 2c20 272d 2d6c 6973 742d  ('-lm', '--list-
+0000e8c0: 6d6f 6465 6c73 272c 2068 656c 703d 224c  models', help="L
+0000e8d0: 6973 7420 6f66 2077 6869 7370 6572 206d  ist of whisper m
+0000e8e0: 6f64 656c 7320 6e61 6d65 222c 2061 6374  odels name", act
+0000e8f0: 696f 6e3d 2773 746f 7265 5f74 7275 6527  ion='store_true'
+0000e900: 290d 0a20 2020 2070 6172 7365 722e 6164  )..    parser.ad
+0000e910: 645f 6172 6775 6d65 6e74 2827 2d64 272c  d_argument('-d',
+0000e920: 2027 2d2d 6465 7669 6365 272c 2064 6566   '--device', def
+0000e930: 6175 6c74 3d22 6175 746f 222c 2068 656c  ault="auto", hel
+0000e940: 703d 226e 616d 6520 6f66 2074 6865 2064  p="name of the d
+0000e950: 6576 6963 6520 746f 2075 7365 2229 0d0a  evice to use")..
+0000e960: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
+0000e970: 7267 756d 656e 7428 272d 6c64 272c 2027  rgument('-ld', '
+0000e980: 2d2d 6c69 7374 2d64 6576 6963 6573 272c  --list-devices',
+0000e990: 2068 656c 703d 224c 6973 7420 6f66 2073   help="List of s
+0000e9a0: 7570 706f 7274 6564 2064 6576 6963 6522  upported device"
+0000e9b0: 2c20 6163 7469 6f6e 3d27 7374 6f72 655f  , action='store_
+0000e9c0: 7472 7565 2729 0d0a 2020 2020 7061 7273  true')..    pars
+0000e9d0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
+0000e9e0: 272d 6374 272c 2027 2d2d 636f 6d70 7574  '-ct', '--comput
+0000e9f0: 652d 7479 7065 272c 2064 6566 6175 6c74  e-type', default
+0000ea00: 3d22 6175 746f 222c 2068 656c 703d 226e  ="auto", help="n
+0000ea10: 616d 6520 6f66 2074 6865 2063 6f6d 7075  ame of the compu
+0000ea20: 7465 2074 7970 6520 2871 7561 6e74 697a  te type (quantiz
+0000ea30: 6174 696f 6e29 2074 6f20 7573 6522 290d  ation) to use").
+0000ea40: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
+0000ea50: 6172 6775 6d65 6e74 2827 2d6c 6374 272c  argument('-lct',
+0000ea60: 2027 2d2d 6c69 7374 2d63 6f6d 7075 7465   '--list-compute
+0000ea70: 2d74 7970 6573 272c 2068 656c 703d 224c  -types', help="L
+0000ea80: 6973 7420 6f66 2073 7570 706f 7274 6564  ist of supported
+0000ea90: 2063 6f6d 7075 7465 2074 7970 6573 222c   compute types",
+0000eaa0: 2061 6374 696f 6e3d 2773 746f 7265 5f74   action='store_t
+0000eab0: 7275 6527 290d 0a20 2020 2070 6172 7365  rue')..    parse
+0000eac0: 722e 6164 645f 6172 6775 6d65 6e74 2827  r.add_argument('
+0000ead0: 2d63 7075 272c 2027 2d2d 6370 752d 7468  -cpu', '--cpu-th
+0000eae0: 7265 6164 7327 2c20 6465 6661 756c 743d  reads', default=
+0000eaf0: 302c 2068 656c 703d 224e 756d 6265 7220  0, help="Number 
+0000eb00: 6f66 2074 6872 6561 6473 2074 6f20 7573  of threads to us
+0000eb10: 6520 7768 656e 2072 756e 6e69 6e67 206f  e when running o
+0000eb20: 6e20 4350 5522 290d 0a20 2020 2070 6172  n CPU")..    par
+0000eb30: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
+0000eb40: 2827 2d6e 7727 2c20 272d 2d6e 756d 2d77  ('-nw', '--num-w
+0000eb50: 6f72 6b65 7273 272c 2064 6566 6175 6c74  orkers', default
+0000eb60: 3d31 2c20 6865 6c70 3d22 4e75 6d62 6572  =1, help="Number
+0000eb70: 206f 6620 636f 6e63 7572 7265 6e74 2063   of concurrent c
+0000eb80: 616c 6c73 2077 6865 6e20 7275 6e6e 696e  alls when runnin
+0000eb90: 6720 7468 6520 6d6f 6465 6c22 290d 0a20  g the model").. 
+0000eba0: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
+0000ebb0: 6775 6d65 6e74 2827 2d53 272c 2027 2d2d  gument('-S', '--
+0000ebc0: 7372 632d 6c61 6e67 7561 6765 272c 2068  src-language', h
+0000ebd0: 656c 703d 224c 616e 6775 6167 6520 636f  elp="Language co
+0000ebe0: 6465 206f 6620 7468 6520 6175 6469 6f20  de of the audio 
+0000ebf0: 6c61 6e67 7561 6765 2073 706f 6b65 6e20  language spoken 
+0000ec00: 696e 2076 6964 656f 2f61 7564 696f 2073  in video/audio s
+0000ec10: 6f75 7263 655f 7061 7468 222c 2064 6566  ource_path", def
+0000ec20: 6175 6c74 3d22 656e 2229 0d0a 2020 2020  ault="en")..    
+0000ec30: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+0000ec40: 656e 7428 272d 4427 2c20 272d 2d64 7374  ent('-D', '--dst
+0000ec50: 2d6c 616e 6775 6167 6527 2c20 6865 6c70  -language', help
+0000ec60: 3d22 4465 7369 7265 6420 7472 616e 736c  ="Desired transl
+0000ec70: 6174 696f 6e20 6c61 6e67 7561 6765 2063  ation language c
+0000ec80: 6f64 6520 666f 7220 7468 6520 7375 6274  ode for the subt
+0000ec90: 6974 6c65 7322 2c20 6465 6661 756c 743d  itles", default=
+0000eca0: 4e6f 6e65 290d 0a20 2020 2070 6172 7365  None)..    parse
+0000ecb0: 722e 6164 645f 6172 6775 6d65 6e74 2827  r.add_argument('
+0000ecc0: 2d6c 776c 272c 2027 2d2d 6c69 7374 2d77  -lwl', '--list-w
+0000ecd0: 6869 7370 6572 2d6c 616e 6775 6167 6573  hisper-languages
+0000ece0: 272c 2068 656c 703d 224c 6973 7420 616c  ', help="List al
+0000ecf0: 6c20 7768 6973 7065 7220 7375 7070 6f72  l whisper suppor
+0000ed00: 7465 6420 6c61 6e67 7561 6765 7320 2873  ted languages (s
+0000ed10: 7263 5f6c 616e 6775 6167 6573 2922 2c20  rc_languages)", 
+0000ed20: 6163 7469 6f6e 3d27 7374 6f72 655f 7472  action='store_tr
+0000ed30: 7565 2729 0d0a 2020 2020 7061 7273 6572  ue')..    parser
+0000ed40: 2e61 6464 5f61 7267 756d 656e 7428 272d  .add_argument('-
+0000ed50: 6c67 6c27 2c20 272d 2d6c 6973 742d 676f  lgl', '--list-go
+0000ed60: 6f67 6c65 2d6c 616e 6775 6167 6573 272c  ogle-languages',
+0000ed70: 2068 656c 703d 224c 6973 7420 616c 6c20   help="List all 
+0000ed80: 676f 6f67 6c65 2074 7261 6e73 6c61 7465  google translate
+0000ed90: 2073 7570 706f 7274 6564 206c 616e 6775   supported langu
+0000eda0: 6167 6573 2028 6473 745f 6c61 6e67 7561  ages (dst_langua
+0000edb0: 6765 7329 222c 2061 6374 696f 6e3d 2773  ges)", action='s
+0000edc0: 746f 7265 5f74 7275 6527 290d 0a20 2020  tore_true')..   
+0000edd0: 2070 6172 7365 722e 6164 645f 6172 6775   parser.add_argu
+0000ede0: 6d65 6e74 2827 2d46 272c 2027 2d2d 666f  ment('-F', '--fo
+0000edf0: 726d 6174 272c 2068 656c 703d 2244 6573  rmat', help="Des
+0000ee00: 6972 6564 2073 7562 7469 746c 6520 666f  ired subtitle fo
+0000ee10: 726d 6174 222c 2064 6566 6175 6c74 3d22  rmat", default="
+0000ee20: 7372 7422 290d 0a20 2020 2070 6172 7365  srt")..    parse
+0000ee30: 722e 6164 645f 6172 6775 6d65 6e74 2827  r.add_argument('
+0000ee40: 2d6c 6627 2c20 272d 2d6c 6973 742d 666f  -lf', '--list-fo
+0000ee50: 726d 6174 7327 2c20 6865 6c70 3d22 4c69  rmats', help="Li
+0000ee60: 7374 2061 6c6c 2073 7570 706f 7274 6564  st all supported
+0000ee70: 2073 7562 7469 746c 6520 666f 726d 6174   subtitle format
+0000ee80: 7322 2c20 6163 7469 6f6e 3d27 7374 6f72  s", action='stor
+0000ee90: 655f 7472 7565 2729 0d0a 2020 2020 7061  e_true')..    pa
+0000eea0: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+0000eeb0: 7428 272d 4327 2c20 272d 2d63 6f6e 6375  t('-C', '--concu
+0000eec0: 7272 656e 6379 272c 2068 656c 703d 224e  rrency', help="N
+0000eed0: 756d 6265 7220 6f66 2063 6f6e 6375 7272  umber of concurr
+0000eee0: 656e 7420 7472 616e 736c 6174 6520 4150  ent translate AP
+0000eef0: 4920 7265 7175 6573 7473 2074 6f20 6d61  I requests to ma
+0000ef00: 6b65 222c 2074 7970 653d 696e 742c 2064  ke", type=int, d
+0000ef10: 6566 6175 6c74 3d31 3029 0d0a 2020 2020  efault=10)..    
+0000ef20: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+0000ef30: 656e 7428 272d 7627 2c20 272d 2d76 6572  ent('-v', '--ver
+0000ef40: 7369 6f6e 272c 2061 6374 696f 6e3d 2776  sion', action='v
+0000ef50: 6572 7369 6f6e 272c 2076 6572 7369 6f6e  ersion', version
+0000ef60: 3d56 4552 5349 4f4e 290d 0a0d 0a20 2020  =VERSION)....   
+0000ef70: 2061 7267 7320 3d20 7061 7273 6572 2e70   args = parser.p
+0000ef80: 6172 7365 5f61 7267 7328 290d 0a0d 0a20  arse_args().... 
+0000ef90: 2020 2073 7263 5f6c 616e 6775 6167 6520     src_language 
+0000efa0: 3d20 6172 6773 2e73 7263 5f6c 616e 6775  = args.src_langu
+0000efb0: 6167 650d 0a20 2020 2064 7374 5f6c 616e  age..    dst_lan
+0000efc0: 6775 6167 6520 3d20 6172 6773 2e64 7374  guage = args.dst
+0000efd0: 5f6c 616e 6775 6167 650d 0a0d 0a20 2020  _language....   
+0000efe0: 206d 6f64 656c 5f6e 616d 6520 3d20 6172   model_name = ar
+0000eff0: 6773 2e6d 6f64 656c 5f6e 616d 650d 0a20  gs.model_name.. 
+0000f000: 2020 2069 6620 6d6f 6465 6c5f 6e61 6d65     if model_name
+0000f010: 2e65 6e64 7377 6974 6828 222e 656e 2229  .endswith(".en")
+0000f020: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
+0000f030: 2866 227b 6d6f 6465 6c5f 6e61 6d65 7d20  (f"{model_name} 
+0000f040: 6973 2061 6e20 456e 676c 6973 682d 6f6e  is an English-on
+0000f050: 6c79 206d 6f64 656c 2c20 666f 7263 696e  ly model, forcin
+0000f060: 6720 456e 676c 6973 6820 6465 7465 6374  g English detect
+0000f070: 696f 6e2e 2229 0d0a 2020 2020 2020 2020  ion.")..        
+0000f080: 6172 6773 2e73 7263 5f6c 616e 6775 6167  args.src_languag
+0000f090: 6520 3d20 2265 6e22 0d0a 2020 2020 656c  e = "en"..    el
+0000f0a0: 6966 2061 7267 732e 7372 635f 6c61 6e67  if args.src_lang
+0000f0b0: 7561 6765 2021 3d20 2261 7574 6f22 3a0d  uage != "auto":.
+0000f0c0: 0a20 2020 2020 2020 2061 7267 732e 7372  .        args.sr
+0000f0d0: 635f 6c61 6e67 7561 6765 203d 2073 7263  c_language = src
+0000f0e0: 5f6c 616e 6775 6167 650d 0a0d 0a20 2020  _language....   
+0000f0f0: 206d 6f64 656c 203d 2057 6869 7370 6572   model = Whisper
+0000f100: 4d6f 6465 6c28 6d6f 6465 6c5f 6e61 6d65  Model(model_name
+0000f110: 2c20 6465 7669 6365 3d61 7267 732e 6465  , device=args.de
+0000f120: 7669 6365 2c20 636f 6d70 7574 655f 7479  vice, compute_ty
+0000f130: 7065 3d61 7267 732e 636f 6d70 7574 655f  pe=args.compute_
+0000f140: 7479 7065 2c20 6370 755f 7468 7265 6164  type, cpu_thread
+0000f150: 733d 696e 7428 6172 6773 2e63 7075 5f74  s=int(args.cpu_t
+0000f160: 6872 6561 6473 292c 206e 756d 5f77 6f72  hreads), num_wor
+0000f170: 6b65 7273 3d69 6e74 2861 7267 732e 6e75  kers=int(args.nu
+0000f180: 6d5f 776f 726b 6572 7329 290d 0a0d 0a20  m_workers)).... 
+0000f190: 2020 2069 6620 6172 6773 2e6c 6973 745f     if args.list_
+0000f1a0: 6d6f 6465 6c73 3a0d 0a20 2020 2020 2020  models:..       
+0000f1b0: 2070 7269 6e74 2822 4c69 7374 206f 6620   print("List of 
+0000f1c0: 7768 6973 7065 7220 6d6f 6465 6c73 3a22  whisper models:"
+0000f1d0: 290d 0a20 2020 2020 2020 2066 6f72 206d  )..        for m
+0000f1e0: 6f64 656c 5f6e 616d 6520 696e 2077 6869  odel_name in whi
+0000f1f0: 7370 6572 5f6d 6f64 656c 733a 0d0a 2020  sper_models:..  
+0000f200: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000f210: 6d6f 6465 6c5f 6e61 6d65 290d 0a20 2020  model_name)..   
+0000f220: 2020 2020 2072 6574 7572 6e20 300d 0a0d       return 0...
+0000f230: 0a20 2020 2069 6620 6172 6773 2e6c 6973  .    if args.lis
+0000f240: 745f 6465 7669 6365 733a 0d0a 2020 2020  t_devices:..    
+0000f250: 2020 2020 7072 696e 7428 224c 6973 7420      print("List 
+0000f260: 6f66 2073 7570 706f 7274 6564 2064 6576  of supported dev
+0000f270: 6963 6573 3a22 290d 0a20 2020 2020 2020  ices:")..       
+0000f280: 2066 6f72 2064 6576 6963 6520 696e 2064   for device in d
+0000f290: 6576 6963 6573 3a0d 0a20 2020 2020 2020  evices:..       
+0000f2a0: 2020 2020 2070 7269 6e74 2864 6576 6963       print(devic
+0000f2b0: 6529 0d0a 2020 2020 2020 2020 7265 7475  e)..        retu
+0000f2c0: 726e 2030 0d0a 0d0a 2020 2020 6966 2061  rn 0....    if a
+0000f2d0: 7267 732e 6c69 7374 5f63 6f6d 7075 7465  rgs.list_compute
+0000f2e0: 5f74 7970 6573 3a0d 0a20 2020 2020 2020  _types:..       
+0000f2f0: 2070 7269 6e74 2822 4c69 7374 206f 6620   print("List of 
+0000f300: 7375 7070 6f72 7465 6420 636f 6d70 7574  supported comput
+0000f310: 6520 7479 7065 733a 2229 0d0a 2020 2020  e types:")..    
+0000f320: 2020 2020 666f 7220 636f 6d70 7574 655f      for compute_
+0000f330: 7479 7065 2069 6e20 636f 6d70 7574 655f  type in compute_
+0000f340: 7479 7065 733a 0d0a 2020 2020 2020 2020  types:..        
+0000f350: 2020 2020 7072 696e 7428 636f 6d70 7574      print(comput
+0000f360: 655f 7479 7065 290d 0a20 2020 2020 2020  e_type)..       
+0000f370: 2072 6574 7572 6e20 300d 0a0d 0a20 2020   return 0....   
+0000f380: 2077 6869 7370 6572 5f6c 616e 6775 6167   whisper_languag
+0000f390: 6520 3d20 5768 6973 7065 724c 616e 6775  e = WhisperLangu
+0000f3a0: 6167 6528 290d 0a20 2020 2067 6f6f 676c  age()..    googl
+0000f3b0: 655f 6c61 6e67 7561 6765 203d 2047 6f6f  e_language = Goo
+0000f3c0: 676c 654c 616e 6775 6167 6528 290d 0a0d  gleLanguage()...
+0000f3d0: 0a20 2020 2069 6620 6172 6773 2e6c 6973  .    if args.lis
+0000f3e0: 745f 7768 6973 7065 725f 6c61 6e67 7561  t_whisper_langua
+0000f3f0: 6765 733a 0d0a 2020 2020 2020 2020 7072  ges:..        pr
+0000f400: 696e 7428 224c 6973 7420 6f66 2077 6869  int("List of whi
+0000f410: 7370 6572 2073 7570 706f 7274 6564 206c  sper supported l
+0000f420: 616e 6775 6167 6573 3a22 290d 0a20 2020  anguages:")..   
+0000f430: 2020 2020 2066 6f72 2077 6869 7370 6572       for whisper
+0000f440: 5f63 6f64 652c 2077 6869 7370 6572 5f6c  _code, whisper_l
+0000f450: 616e 6775 6167 6520 696e 2073 6f72 7465  anguage in sorte
+0000f460: 6428 7768 6973 7065 725f 6c61 6e67 7561  d(whisper_langua
+0000f470: 6765 2e6e 616d 655f 6f66 5f63 6f64 652e  ge.name_of_code.
+0000f480: 6974 656d 7328 2929 3a0d 0a20 2020 2020  items()):..     
+0000f490: 2020 2020 2020 2070 7269 6e74 2822 252d         print("%-
+0000f4a0: 3873 203a 2025 7322 2025 2877 6869 7370  8s : %s" %(whisp
+0000f4b0: 6572 5f63 6f64 652c 2077 6869 7370 6572  er_code, whisper
+0000f4c0: 5f6c 616e 6775 6167 6529 290d 0a20 2020  _language))..   
+0000f4d0: 2020 2020 2072 6574 7572 6e20 300d 0a0d       return 0...
+0000f4e0: 0a20 2020 2069 6620 6172 6773 2e6c 6973  .    if args.lis
+0000f4f0: 745f 676f 6f67 6c65 5f6c 616e 6775 6167  t_google_languag
+0000f500: 6573 3a0d 0a20 2020 2020 2020 2070 7269  es:..        pri
+0000f510: 6e74 2822 4c69 7374 206f 6620 676f 6f67  nt("List of goog
+0000f520: 6c65 2074 7261 6e73 6c61 7465 2073 7570  le translate sup
+0000f530: 706f 7274 6564 206c 616e 6775 6167 6573  ported languages
+0000f540: 3a22 290d 0a20 2020 2020 2020 2066 6f72  :")..        for
+0000f550: 2067 6f6f 676c 655f 636f 6465 2c20 676f   google_code, go
+0000f560: 6f67 6c65 5f6c 616e 6775 6167 6520 696e  ogle_language in
+0000f570: 2073 6f72 7465 6428 676f 6f67 6c65 5f6c   sorted(google_l
+0000f580: 616e 6775 6167 652e 6e61 6d65 5f6f 665f  anguage.name_of_
+0000f590: 636f 6465 2e69 7465 6d73 2829 293a 0d0a  code.items()):..
+0000f5a0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000f5b0: 7428 2225 2d38 7320 3a20 2573 2220 2528  t("%-8s : %s" %(
+0000f5c0: 676f 6f67 6c65 5f63 6f64 652c 2067 6f6f  google_code, goo
+0000f5d0: 676c 655f 6c61 6e67 7561 6765 2929 0d0a  gle_language))..
+0000f5e0: 2020 2020 2020 2020 7265 7475 726e 2030          return 0
+0000f5f0: 0d0a 0d0a 2020 2020 6966 2061 7267 732e  ....    if args.
+0000f600: 7372 635f 6c61 6e67 7561 6765 206e 6f74  src_language not
+0000f610: 2069 6e20 7768 6973 7065 725f 6c61 6e67   in whisper_lang
+0000f620: 7561 6765 2e6e 616d 655f 6f66 5f63 6f64  uage.name_of_cod
+0000f630: 652e 6b65 7973 2829 3a0d 0a20 2020 2020  e.keys():..     
+0000f640: 2020 2070 7269 6e74 2822 536f 7572 6365     print("Source
+0000f650: 206c 616e 6775 6167 6520 6973 206e 6f74   language is not
+0000f660: 2073 7570 706f 7274 6564 2e20 5275 6e20   supported. Run 
+0000f670: 7769 7468 202d 2d6c 6973 742d 7768 6973  with --list-whis
+0000f680: 7065 722d 6c61 6e67 7561 6765 7320 746f  per-languages to
+0000f690: 2073 6565 2061 6c6c 2077 6869 7370 6572   see all whisper
+0000f6a0: 2073 7570 706f 7274 6564 206c 616e 6775   supported langu
+0000f6b0: 6167 6573 2e22 290d 0a20 2020 2020 2020  ages.")..       
+0000f6c0: 2072 6574 7572 6e20 310d 0a0d 0a20 2020   return 1....   
+0000f6d0: 2069 6620 6172 6773 2e64 7374 5f6c 616e   if args.dst_lan
+0000f6e0: 6775 6167 653a 0d0a 2020 2020 2020 2020  guage:..        
+0000f6f0: 6966 206e 6f74 2061 7267 732e 6473 745f  if not args.dst_
+0000f700: 6c61 6e67 7561 6765 2069 6e20 676f 6f67  language in goog
+0000f710: 6c65 5f6c 616e 6775 6167 652e 6e61 6d65  le_language.name
+0000f720: 5f6f 665f 636f 6465 2e6b 6579 7328 293a  _of_code.keys():
+0000f730: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+0000f740: 696e 7428 2244 6573 7469 6e61 7469 6f6e  int("Destination
+0000f750: 206c 616e 6775 6167 6520 6973 206e 6f74   language is not
+0000f760: 2073 7570 706f 7274 6564 2e20 5275 6e20   supported. Run 
+0000f770: 7769 7468 202d 2d6c 6973 742d 676f 6f67  with --list-goog
+0000f780: 6c65 2d6c 616e 6775 6167 6573 2074 6f20  le-languages to 
+0000f790: 7365 6520 616c 6c20 676f 6f67 6c65 2074  see all google t
+0000f7a0: 7261 6e73 6c61 7465 2073 7570 706f 7274  ranslate support
+0000f7b0: 6564 206c 616e 6775 6167 6573 2e22 290d  ed languages.").
+0000f7c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000f7d0: 7572 6e20 310d 0a20 2020 2020 2020 2069  urn 1..        i
+0000f7e0: 6620 6e6f 7420 6973 5f73 616d 655f 6c61  f not is_same_la
+0000f7f0: 6e67 7561 6765 2861 7267 732e 7372 635f  nguage(args.src_
+0000f800: 6c61 6e67 7561 6765 2c20 6172 6773 2e64  language, args.d
+0000f810: 7374 5f6c 616e 6775 6167 652c 2065 7272  st_language, err
+0000f820: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+0000f830: 6261 636b 3d73 686f 775f 6572 726f 725f  back=show_error_
+0000f840: 6d65 7373 6167 6573 293a 0d0a 2020 2020  messages):..    
+0000f850: 2020 2020 2020 2020 646f 5f74 7261 6e73          do_trans
+0000f860: 6c61 7465 203d 2054 7275 650d 0a20 2020  late = True..   
+0000f870: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000f880: 2020 2020 2020 2020 646f 5f74 7261 6e73          do_trans
+0000f890: 6c61 7465 203d 2046 616c 7365 0d0a 2020  late = False..  
+0000f8a0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0000f8b0: 2064 6f5f 7472 616e 736c 6174 6520 3d20   do_translate = 
+0000f8c0: 4661 6c73 650d 0a0d 0a20 2020 2069 6620  False....    if 
+0000f8d0: 6172 6773 2e6c 6973 745f 666f 726d 6174  args.list_format
+0000f8e0: 733a 0d0a 2020 2020 2020 2020 7072 696e  s:..        prin
+0000f8f0: 7428 224c 6973 7420 6f66 2073 7570 706f  t("List of suppo
+0000f900: 7274 6564 2073 7562 7469 746c 6520 666f  rted subtitle fo
+0000f910: 726d 6174 733a 2229 0d0a 2020 2020 2020  rmats:")..      
+0000f920: 2020 666f 7220 7375 6274 6974 6c65 5f66    for subtitle_f
+0000f930: 6f72 6d61 7420 696e 2053 7562 7469 746c  ormat in Subtitl
+0000f940: 6546 6f72 6d61 7474 6572 2e73 7570 706f  eFormatter.suppo
+0000f950: 7274 6564 5f66 6f72 6d61 7473 3a0d 0a20  rted_formats:.. 
+0000f960: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000f970: 2822 7b66 6f72 6d61 747d 222e 666f 726d  ("{format}".form
+0000f980: 6174 2866 6f72 6d61 743d 7375 6274 6974  at(format=subtit
+0000f990: 6c65 5f66 6f72 6d61 7429 290d 0a20 2020  le_format))..   
+0000f9a0: 2020 2020 2072 6574 7572 6e20 300d 0a0d       return 0...
+0000f9b0: 0a20 2020 2069 6620 6172 6773 2e66 6f72  .    if args.for
+0000f9c0: 6d61 7420 6e6f 7420 696e 2053 7562 7469  mat not in Subti
+0000f9d0: 746c 6546 6f72 6d61 7474 6572 2e73 7570  tleFormatter.sup
+0000f9e0: 706f 7274 6564 5f66 6f72 6d61 7473 3a0d  ported_formats:.
+0000f9f0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+0000fa00: 5375 6274 6974 6c65 2066 6f72 6d61 7420  Subtitle format 
+0000fa10: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
+0000fa20: 2e20 5275 6e20 7769 7468 202d 2d6c 6973  . Run with --lis
+0000fa30: 742d 666f 726d 6174 7320 746f 2073 6565  t-formats to see
+0000fa40: 2061 6c6c 2073 7570 706f 7274 6564 2066   all supported f
+0000fa50: 6f72 6d61 7473 2e22 290d 0a20 2020 2020  ormats.")..     
+0000fa60: 2020 2072 6574 7572 6e20 310d 0a0d 0a20     return 1.... 
+0000fa70: 2020 2069 6620 6e6f 7420 6172 6773 2e73     if not args.s
+0000fa80: 6f75 7263 655f 7061 7468 3a0d 0a20 2020  ource_path:..   
+0000fa90: 2020 2020 2070 6172 7365 722e 7072 696e       parser.prin
+0000faa0: 745f 6865 6c70 2873 7973 2e73 7464 6572  t_help(sys.stder
+0000fab0: 7229 0d0a 2020 2020 2020 2020 7265 7475  r)..        retu
+0000fac0: 726e 2031 0d0a 0d0a 2020 2020 636f 6d70  rn 1....    comp
+0000fad0: 6c65 7465 645f 7461 736b 7320 3d20 300d  leted_tasks = 0.
+0000fae0: 0a20 2020 206d 6564 6961 5f66 696c 6570  .    media_filep
+0000faf0: 6174 6873 203d 205b 5d0d 0a20 2020 2061  aths = []..    a
+0000fb00: 7267 5f66 696c 6570 6174 6873 203d 205b  rg_filepaths = [
+0000fb10: 5d0d 0a20 2020 2069 6e76 616c 6964 5f6d  ]..    invalid_m
+0000fb20: 6564 6961 5f66 696c 6570 6174 6873 203d  edia_filepaths =
+0000fb30: 205b 5d0d 0a20 2020 206e 6f74 5f65 7869   []..    not_exi
+0000fb40: 7374 5f66 696c 6570 6174 6873 203d 205b  st_filepaths = [
+0000fb50: 5d0d 0a20 2020 2061 7267 7061 7468 203d  ]..    argpath =
+0000fb60: 204e 6f6e 650d 0a0d 0a20 2020 2061 7267   None....    arg
+0000fb70: 735f 736f 7572 6365 5f70 6174 6820 3d20  s_source_path = 
+0000fb80: 6172 6773 2e73 6f75 7263 655f 7061 7468  args.source_path
+0000fb90: 0d0a 0d0a 2020 2020 6966 2028 6e6f 7420  ....    if (not 
+0000fba0: 222a 2220 696e 2073 7472 2861 7267 735f  "*" in str(args_
+0000fbb0: 736f 7572 6365 5f70 6174 6829 2920 616e  source_path)) an
+0000fbc0: 6420 286e 6f74 2022 3f22 2069 6e20 7374  d (not "?" in st
+0000fbd0: 7228 6172 6773 5f73 6f75 7263 655f 7061  r(args_source_pa
+0000fbe0: 7468 2929 3a0d 0a20 2020 2020 2020 2066  th)):..        f
+0000fbf0: 6f72 2066 696c 6570 6174 6820 696e 2061  or filepath in a
+0000fc00: 7267 735f 736f 7572 6365 5f70 6174 683a  rgs_source_path:
+0000fc10: 0d0a 2020 2020 2020 2020 2020 2020 6670  ..            fp
+0000fc20: 6174 6820 3d20 5061 7468 2866 696c 6570  ath = Path(filep
+0000fc30: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
+0000fc40: 2020 6966 206e 6f74 206f 732e 7061 7468    if not os.path
+0000fc50: 2e69 7366 696c 6528 6670 6174 6829 3a0d  .isfile(fpath):.
+0000fc60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fc70: 206e 6f74 5f65 7869 7374 5f66 696c 6570   not_exist_filep
+0000fc80: 6174 6873 2e61 7070 656e 6428 6669 6c65  aths.append(file
+0000fc90: 7061 7468 290d 0a0d 0a20 2020 2069 6620  path)....    if 
+0000fca0: 7379 732e 706c 6174 666f 726d 203d 3d20  sys.platform == 
+0000fcb0: 2277 696e 3332 223a 0d0a 2020 2020 2020  "win32":..      
+0000fcc0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+0000fcd0: 286c 656e 2861 7267 732e 736f 7572 6365  (len(args.source
+0000fce0: 5f70 6174 6829 293a 0d0a 2020 2020 2020  _path)):..      
+0000fcf0: 2020 2020 2020 6966 2028 225b 2220 6f72        if ("[" or
+0000fd00: 2022 5d22 2920 696e 2061 7267 732e 736f   "]") in args.so
+0000fd10: 7572 6365 5f70 6174 685b 695d 3a0d 0a20  urce_path[i]:.. 
+0000fd20: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000fd30: 6c61 6365 686f 6c64 6572 203d 2022 2354  laceholder = "#T
+0000fd40: 454d 5023 220d 0a20 2020 2020 2020 2020  EMP#"..         
+0000fd50: 2020 2020 2020 2061 7267 735f 736f 7572         args_sour
+0000fd60: 6365 5f70 6174 685b 695d 203d 2061 7267  ce_path[i] = arg
+0000fd70: 732e 736f 7572 6365 5f70 6174 685b 695d  s.source_path[i]
+0000fd80: 2e72 6570 6c61 6365 2822 5b22 2c20 706c  .replace("[", pl
+0000fd90: 6163 6568 6f6c 6465 7229 0d0a 2020 2020  aceholder)..    
+0000fda0: 2020 2020 2020 2020 2020 2020 6172 6773              args
+0000fdb0: 5f73 6f75 7263 655f 7061 7468 5b69 5d20  _source_path[i] 
+0000fdc0: 3d20 6172 6773 5f73 6f75 7263 655f 7061  = args_source_pa
+0000fdd0: 7468 5b69 5d2e 7265 706c 6163 6528 225d  th[i].replace("]
+0000fde0: 222c 2022 5b5d 5d22 290d 0a20 2020 2020  ", "[]]")..     
+0000fdf0: 2020 2020 2020 2020 2020 2061 7267 735f             args_
+0000fe00: 736f 7572 6365 5f70 6174 685b 695d 203d  source_path[i] =
+0000fe10: 2061 7267 735f 736f 7572 6365 5f70 6174   args_source_pat
+0000fe20: 685b 695d 2e72 6570 6c61 6365 2870 6c61  h[i].replace(pla
+0000fe30: 6365 686f 6c64 6572 2c20 225b 5b5d 2229  ceholder, "[[]")
+0000fe40: 0d0a 0d0a 2020 2020 666f 7220 6172 6720  ....    for arg 
+0000fe50: 696e 2061 7267 735f 736f 7572 6365 5f70  in args_source_p
+0000fe60: 6174 683a 0d0a 2020 2020 2020 2020 6966  ath:..        if
+0000fe70: 206e 6f74 2073 7973 2e70 6c61 7466 6f72   not sys.platfor
+0000fe80: 6d20 3d3d 2022 7769 6e33 3222 203a 0d0a  m == "win32" :..
+0000fe90: 2020 2020 2020 2020 2020 2020 6172 6720              arg 
+0000fea0: 3d20 6573 6361 7065 2861 7267 290d 0a0d  = escape(arg)...
+0000feb0: 0a20 2020 2020 2020 2061 7267 5f66 696c  .        arg_fil
+0000fec0: 6570 6174 6873 202b 3d20 676c 6f62 2861  epaths += glob(a
+0000fed0: 7267 290d 0a0d 0a20 2020 2069 6620 6172  rg)....    if ar
+0000fee0: 675f 6669 6c65 7061 7468 733a 0d0a 2020  g_filepaths:..  
+0000fef0: 2020 2020 2020 666f 7220 6172 6770 6174        for argpat
+0000ff00: 6820 696e 2061 7267 5f66 696c 6570 6174  h in arg_filepat
+0000ff10: 6873 3a0d 0a20 2020 2020 2020 2020 2020  hs:..           
+0000ff20: 2069 6620 6f73 2e70 6174 682e 6973 6669   if os.path.isfi
+0000ff30: 6c65 2861 7267 7061 7468 293a 0d0a 2020  le(argpath):..  
+0000ff40: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000ff50: 2063 6865 636b 5f66 696c 655f 7479 7065   check_file_type
+0000ff60: 2861 7267 7061 7468 2c20 6572 726f 725f  (argpath, error_
+0000ff70: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+0000ff80: 6b3d 7368 6f77 5f65 7272 6f72 5f6d 6573  k=show_error_mes
+0000ff90: 7361 6765 7329 203d 3d20 2776 6964 656f  sages) == 'video
+0000ffa0: 2720 6f72 2063 6865 636b 5f66 696c 655f  ' or check_file_
+0000ffb0: 7479 7065 2861 7267 7061 7468 2c20 6572  type(argpath, er
+0000ffc0: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+0000ffd0: 6c62 6163 6b3d 7368 6f77 5f65 7272 6f72  lback=show_error
+0000ffe0: 5f6d 6573 7361 6765 7329 203d 3d20 2761  _messages) == 'a
+0000fff0: 7564 696f 273a 0d0a 2020 2020 2020 2020  udio':..        
+00010000: 2020 2020 2020 2020 2020 2020 6d65 6469              medi
+00010010: 615f 6669 6c65 7061 7468 732e 6170 7065  a_filepaths.appe
+00010020: 6e64 2861 7267 7061 7468 290d 0a20 2020  nd(argpath)..   
+00010030: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00010040: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00010050: 2020 2020 2020 2020 696e 7661 6c69 645f          invalid_
+00010060: 6d65 6469 615f 6669 6c65 7061 7468 732e  media_filepaths.
+00010070: 6170 7065 6e64 2861 7267 7061 7468 290d  append(argpath).
+00010080: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00010090: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000100a0: 2020 2020 6e6f 745f 6578 6973 745f 6669      not_exist_fi
+000100b0: 6c65 7061 7468 732e 6170 7065 6e64 2861  lepaths.append(a
+000100c0: 7267 7061 7468 290d 0a0d 0a20 2020 2020  rgpath)....     
+000100d0: 2020 2069 6620 696e 7661 6c69 645f 6d65     if invalid_me
+000100e0: 6469 615f 6669 6c65 7061 7468 733a 0d0a  dia_filepaths:..
+000100f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00010100: 696e 7661 6c69 645f 6d65 6469 615f 6669  invalid_media_fi
+00010110: 6c65 7061 7468 2069 6e20 696e 7661 6c69  lepath in invali
+00010120: 645f 6d65 6469 615f 6669 6c65 7061 7468  d_media_filepath
+00010130: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00010140: 2020 2020 6d73 6720 3d20 227b 7d20 6973      msg = "{} is
+00010150: 206e 6f74 2076 616c 6964 2076 6964 656f   not valid video
+00010160: 206f 7220 6175 6469 6f20 6669 6c65 7322   or audio files"
+00010170: 2e66 6f72 6d61 7428 696e 7661 6c69 645f  .format(invalid_
+00010180: 6d65 6469 615f 6669 6c65 7061 7468 290d  media_filepath).
+00010190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000101a0: 2070 7269 6e74 286d 7367 290d 0a0d 0a20   print(msg).... 
+000101b0: 2020 2069 6620 6e6f 745f 6578 6973 745f     if not_exist_
+000101c0: 6669 6c65 7061 7468 733a 0d0a 2020 2020  filepaths:..    
+000101d0: 2020 2020 666f 7220 6e6f 745f 6578 6973      for not_exis
+000101e0: 745f 6669 6c65 7061 7468 2069 6e20 6e6f  t_filepath in no
+000101f0: 745f 6578 6973 745f 6669 6c65 7061 7468  t_exist_filepath
+00010200: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00010210: 6d73 6720 3d20 227b 7d20 6973 206e 6f74  msg = "{} is not
+00010220: 2065 7869 7374 222e 666f 726d 6174 286e   exist".format(n
+00010230: 6f74 5f65 7869 7374 5f66 696c 6570 6174  ot_exist_filepat
+00010240: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
+00010250: 7072 696e 7428 6d73 6729 0d0a 2020 2020  print(msg)..    
+00010260: 2020 2020 6966 2028 6e6f 7420 222a 2220      if (not "*" 
+00010270: 696e 2073 7472 2861 7267 735f 736f 7572  in str(args_sour
+00010280: 6365 5f70 6174 6829 2920 616e 6420 286e  ce_path)) and (n
+00010290: 6f74 2022 3f22 2069 6e20 7374 7228 6172  ot "?" in str(ar
+000102a0: 6773 5f73 6f75 7263 655f 7061 7468 2929  gs_source_path))
+000102b0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+000102c0: 7973 2e65 7869 7428 3029 0d0a 0d0a 2020  ys.exit(0)....  
+000102d0: 2020 6966 206e 6f74 2061 7267 5f66 696c    if not arg_fil
+000102e0: 6570 6174 6873 2061 6e64 206e 6f74 206e  epaths and not n
+000102f0: 6f74 5f65 7869 7374 5f66 696c 6570 6174  ot_exist_filepat
+00010300: 6873 3a0d 0a20 2020 2020 2020 2070 7269  hs:..        pri
+00010310: 6e74 2822 4e6f 2061 6e79 2066 696c 6573  nt("No any files
+00010320: 206d 6174 6368 696e 6720 6669 6c65 6e61   matching filena
+00010330: 6d65 7320 796f 7520 7479 7065 6422 290d  mes you typed").
+00010340: 0a20 2020 2020 2020 2073 7973 2e65 7869  .        sys.exi
+00010350: 7428 3029 0d0a 0d0a 2020 2020 706f 6f6c  t(0)....    pool
+00010360: 203d 206d 756c 7469 7072 6f63 6573 7369   = multiprocessi
+00010370: 6e67 2e50 6f6f 6c28 6172 6773 2e63 6f6e  ng.Pool(args.con
+00010380: 6375 7272 656e 6379 290d 0a0d 0a20 2020  currency)....   
+00010390: 2074 7261 6e73 6372 6962 655f 656e 645f   transcribe_end_
+000103a0: 7469 6d65 203d 204e 6f6e 650d 0a20 2020  time = None..   
+000103b0: 2074 7261 6e73 6372 6962 655f 656c 6170   transcribe_elap
+000103c0: 7365 645f 7469 6d65 203d 204e 6f6e 650d  sed_time = None.
+000103d0: 0a20 2020 2074 7261 6e73 6372 6962 655f  .    transcribe_
+000103e0: 7374 6172 745f 7469 6d65 203d 2074 696d  start_time = tim
+000103f0: 652e 7469 6d65 2829 0d0a 2020 2020 7461  e.time()..    ta
+00010400: 736b 203d 2022 7472 616e 7363 7269 6265  sk = "transcribe
+00010410: 220d 0a0d 0a20 2020 2069 6620 6172 6773  "....    if args
+00010420: 2e73 7263 5f6c 616e 6775 6167 6520 3d3d  .src_language ==
+00010430: 2028 2262 6122 206f 7220 2262 7222 206f   ("ba" or "br" o
+00010440: 7220 2266 6f22 206f 7220 226e 6e22 206f  r "fo" or "nn" o
+00010450: 7220 226f 6322 206f 7220 2274 6c22 206f  r "oc" or "tl" o
+00010460: 7220 2262 6f22 2920 616e 6420 646f 5f74  r "bo") and do_t
+00010470: 7261 6e73 6c61 7465 3a0d 0a20 2020 2020  ranslate:..     
+00010480: 2020 2074 6173 6b20 3d20 2274 7261 6e73     task = "trans
+00010490: 6c61 7465 220d 0a20 2020 2020 2020 2073  late"..        s
+000104a0: 7263 5f6c 616e 6775 6167 6520 3d20 2265  rc_language = "e
+000104b0: 6e22 0d0a 0d0a 2020 2020 666f 7220 6d65  n"....    for me
+000104c0: 6469 615f 6669 6c65 7061 7468 2069 6e20  dia_filepath in 
+000104d0: 6d65 6469 615f 6669 6c65 7061 7468 733a  media_filepaths:
+000104e0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+000104f0: 2250 726f 6365 7373 696e 6720 7b7d 203a  "Processing {} :
+00010500: 222e 666f 726d 6174 286d 6564 6961 5f66  ".format(media_f
+00010510: 696c 6570 6174 6829 290d 0a0d 0a20 2020  ilepath))....   
+00010520: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+00010530: 2020 2020 2020 2074 6f74 616c 5f64 7572         total_dur
+00010540: 6174 696f 6e20 3d20 6765 745f 7669 6465  ation = get_vide
+00010550: 6f5f 6475 7261 7469 6f6e 286d 6564 6961  o_duration(media
+00010560: 5f66 696c 6570 6174 682c 2065 7272 6f72  _filepath, error
+00010570: 5f6d 6573 7361 6765 735f 6361 6c6c 6261  _messages_callba
+00010580: 636b 3d73 686f 775f 6572 726f 725f 6d65  ck=show_error_me
+00010590: 7373 6167 6573 290d 0a20 2020 2020 2020  ssages)..       
+000105a0: 2020 2020 2073 6567 6d65 6e74 732c 2069       segments, i
+000105b0: 6e66 6f20 3d20 6d6f 6465 6c2e 7472 616e  nfo = model.tran
+000105c0: 7363 7269 6265 286d 6564 6961 5f66 696c  scribe(media_fil
+000105d0: 6570 6174 682c 2062 6561 6d5f 7369 7a65  epath, beam_size
+000105e0: 3d35 2c20 6c61 6e67 7561 6765 3d73 7263  =5, language=src
+000105f0: 5f6c 616e 6775 6167 652c 2074 6173 6b3d  _language, task=
+00010600: 7461 736b 290d 0a20 2020 2020 2020 2020  task)..         
+00010610: 2020 2023 6d61 726b 6572 3d27 e296 8827     #marker='...'
+00010620: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+00010630: 6467 6574 7320 3d20 5b22 5065 7266 6f72  dgets = ["Perfor
+00010640: 6d69 6e67 2073 7065 6563 6820 7265 636f  ming speech reco
+00010650: 676e 6974 696f 6e20 2020 2020 2020 2020  gnition         
+00010660: 2020 3a20 222c 2050 6572 6365 6e74 6167    : ", Percentag
+00010670: 6528 292c 2027 2027 2c20 4261 7228 6d61  e(), ' ', Bar(ma
+00010680: 726b 6572 3d27 2327 292c 2027 2027 2c20  rker='#'), ' ', 
+00010690: 4554 4128 295d 0d0a 2020 2020 2020 2020  ETA()]..        
+000106a0: 2020 2020 7062 6172 203d 2050 726f 6772      pbar = Progr
+000106b0: 6573 7342 6172 2877 6964 6765 7473 3d77  essBar(widgets=w
+000106c0: 6964 6765 7473 2c20 6d61 7876 616c 3d31  idgets, maxval=1
+000106d0: 3030 292e 7374 6172 7428 290d 0a0d 0a20  00).start().... 
+000106e0: 2020 2020 2020 2020 2020 2074 696d 6564             timed
+000106f0: 5f73 7562 7469 746c 6573 203d 205b 5d0d  _subtitles = [].
+00010700: 0a20 2020 2020 2020 2020 2020 2072 6567  .            reg
+00010710: 696f 6e73 203d 205b 5d0d 0a20 2020 2020  ions = []..     
+00010720: 2020 2020 2020 2074 7261 6e73 6372 6970         transcrip
+00010730: 7473 203d 205b 5d0d 0a20 2020 2020 2020  ts = []..       
+00010740: 2020 2020 2066 6f72 2073 6567 6d65 6e74       for segment
+00010750: 2069 6e20 7365 676d 656e 7473 3a0d 0a20   in segments:.. 
+00010760: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00010770: 6567 696f 6e73 2e61 7070 656e 6428 2873  egions.append((s
+00010780: 6567 6d65 6e74 2e73 7461 7274 2c20 7365  egment.start, se
+00010790: 676d 656e 742e 656e 6429 290d 0a20 2020  gment.end))..   
+000107a0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+000107b0: 6e73 6372 6970 7473 2e61 7070 656e 6428  nscripts.append(
+000107c0: 7365 676d 656e 742e 7465 7874 290d 0a20  segment.text).. 
+000107d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000107e0: 726f 6772 6573 7320 3d20 696e 7428 696e  rogress = int(in
+000107f0: 7428 7365 676d 656e 742e 656e 6429 2a31  t(segment.end)*1
+00010800: 3030 2f74 6f74 616c 5f64 7572 6174 696f  00/total_duratio
+00010810: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+00010820: 2020 2020 7062 6172 2e75 7064 6174 6528      pbar.update(
+00010830: 7072 6f67 7265 7373 290d 0a20 2020 2020  progress)..     
+00010840: 2020 2020 2020 2070 6261 722e 6669 6e69         pbar.fini
+00010850: 7368 2829 0d0a 2020 2020 2020 2020 2020  sh()..          
+00010860: 2020 7469 6d65 645f 7375 6274 6974 6c65    timed_subtitle
+00010870: 7320 3d20 5b28 722c 2074 2920 666f 7220  s = [(r, t) for 
+00010880: 722c 2074 2069 6e20 7a69 7028 7265 6769  r, t in zip(regi
+00010890: 6f6e 732c 2074 7261 6e73 6372 6970 7473  ons, transcripts
+000108a0: 2920 6966 2074 5d0d 0a0d 0a20 2020 2020  ) if t]....     
+000108b0: 2020 2020 2020 2073 7562 7469 746c 655f         subtitle_
+000108c0: 666f 726d 6174 203d 2061 7267 732e 666f  format = args.fo
+000108d0: 726d 6174 0d0a 2020 2020 2020 2020 2020  rmat..          
+000108e0: 2020 6261 7365 2c20 6578 7420 3d20 6f73    base, ext = os
+000108f0: 2e70 6174 682e 7370 6c69 7465 7874 286d  .path.splitext(m
+00010900: 6564 6961 5f66 696c 6570 6174 6829 0d0a  edia_filepath)..
+00010910: 2020 2020 2020 2020 2020 2020 7375 6274              subt
+00010920: 6974 6c65 5f66 696c 6570 6174 6820 3d20  itle_filepath = 
+00010930: 227b 6261 7365 7d2e 7b66 6f72 6d61 747d  "{base}.{format}
+00010940: 222e 666f 726d 6174 2862 6173 653d 6261  ".format(base=ba
+00010950: 7365 2c20 666f 726d 6174 3d73 7562 7469  se, format=subti
+00010960: 746c 655f 666f 726d 6174 290d 0a0d 0a20  tle_format).... 
+00010970: 2020 2020 2020 2020 2020 2077 7269 7465             write
+00010980: 7220 3d20 5375 6274 6974 6c65 5772 6974  r = SubtitleWrit
+00010990: 6572 2872 6567 696f 6e73 2c20 7472 616e  er(regions, tran
+000109a0: 7363 7269 7074 732c 2073 7562 7469 746c  scripts, subtitl
+000109b0: 655f 666f 726d 6174 2c20 6572 726f 725f  e_format, error_
+000109c0: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+000109d0: 6b3d 7368 6f77 5f65 7272 6f72 5f6d 6573  k=show_error_mes
+000109e0: 7361 6765 7329 0d0a 2020 2020 2020 2020  sages)..        
+000109f0: 2020 2020 7772 6974 6572 2e77 7269 7465      writer.write
+00010a00: 2873 7562 7469 746c 655f 6669 6c65 7061  (subtitle_filepa
+00010a10: 7468 290d 0a0d 0a20 2020 2020 2020 2020  th)....         
+00010a20: 2020 2069 6620 646f 5f74 7261 6e73 6c61     if do_transla
+00010a30: 7465 3a0d 0a20 2020 2020 2020 2020 2020  te:..           
+00010a40: 2020 2020 2074 696d 6564 5f73 7562 7469       timed_subti
+00010a50: 746c 6573 203d 2077 7269 7465 722e 7469  tles = writer.ti
+00010a60: 6d65 645f 7375 6274 6974 6c65 730d 0a20  med_subtitles.. 
+00010a70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00010a80: 7265 6174 6564 5f72 6567 696f 6e73 203d  reated_regions =
+00010a90: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00010aa0: 2020 2020 2063 7265 6174 6564 5f73 7562       created_sub
+00010ab0: 7469 746c 6573 203d 205b 5d0d 0a20 2020  titles = []..   
+00010ac0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00010ad0: 2065 6e74 7279 2069 6e20 7469 6d65 645f   entry in timed_
+00010ae0: 7375 6274 6974 6c65 733a 0d0a 2020 2020  subtitles:..    
+00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b00: 6372 6561 7465 645f 7265 6769 6f6e 732e  created_regions.
+00010b10: 6170 7065 6e64 2865 6e74 7279 5b30 5d29  append(entry[0])
+00010b20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010b30: 2020 2020 2020 6372 6561 7465 645f 7375        created_su
+00010b40: 6274 6974 6c65 732e 6170 7065 6e64 2865  btitles.append(e
+00010b50: 6e74 7279 5b31 5d29 0d0a 0d0a 2020 2020  ntry[1])....    
+00010b60: 2020 2020 2020 2020 2020 2020 7072 6f6d              prom
+00010b70: 7074 203d 2022 5472 616e 736c 6174 696e  pt = "Translatin
+00010b80: 6720 6672 6f6d 2025 7320 746f 2025 7320  g from %s to %s 
+00010b90: 2020 3a20 2220 2528 7372 635f 6c61 6e67    : " %(src_lang
+00010ba0: 7561 6765 2e63 656e 7465 7228 3829 2c20  uage.center(8), 
+00010bb0: 6473 745f 6c61 6e67 7561 6765 2e63 656e  dst_language.cen
+00010bc0: 7465 7228 3829 290d 0a20 2020 2020 2020  ter(8))..       
+00010bd0: 2020 2020 2020 2020 2077 6964 6765 7473           widgets
+00010be0: 203d 205b 7072 6f6d 7074 2c20 5065 7263   = [prompt, Perc
+00010bf0: 656e 7461 6765 2829 2c20 2720 272c 2042  entage(), ' ', B
+00010c00: 6172 286d 6172 6b65 723d 2723 2729 2c20  ar(marker='#'), 
+00010c10: 2720 272c 2045 5441 2829 5d0d 0a20 2020  ' ', ETA()]..   
+00010c20: 2020 2020 2020 2020 2020 2020 2070 6261               pba
+00010c30: 7220 3d20 5072 6f67 7265 7373 4261 7228  r = ProgressBar(
+00010c40: 7769 6467 6574 733d 7769 6467 6574 732c  widgets=widgets,
+00010c50: 206d 6178 7661 6c3d 6c65 6e28 7469 6d65   maxval=len(time
+00010c60: 645f 7375 6274 6974 6c65 7329 292e 7374  d_subtitles)).st
+00010c70: 6172 7428 290d 0a0d 0a20 2020 2020 2020  art()....       
+00010c80: 2020 2020 2020 2020 2074 7261 6e73 6372           transcr
+00010c90: 6970 745f 7472 616e 736c 6174 6f72 203d  ipt_translator =
+00010ca0: 2053 656e 7465 6e63 6554 7261 6e73 6c61   SentenceTransla
+00010cb0: 746f 7228 7372 633d 6172 6773 2e73 7263  tor(src=args.src
+00010cc0: 5f6c 616e 6775 6167 652c 2064 7374 3d61  _language, dst=a
+00010cd0: 7267 732e 6473 745f 6c61 6e67 7561 6765  rgs.dst_language
+00010ce0: 2c20 6572 726f 725f 6d65 7373 6167 6573  , error_messages
+00010cf0: 5f63 616c 6c62 6163 6b3d 7368 6f77 5f65  _callback=show_e
+00010d00: 7272 6f72 5f6d 6573 7361 6765 7329 0d0a  rror_messages)..
+00010d10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010d20: 2020 7472 616e 736c 6174 6564 5f73 7562    translated_sub
+00010d30: 7469 746c 6573 203d 205b 5d0d 0a20 2020  titles = []..   
+00010d40: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00010d50: 2069 2c20 7472 616e 736c 6174 6564 5f73   i, translated_s
+00010d60: 7562 7469 746c 6520 696e 2065 6e75 6d65  ubtitle in enume
+00010d70: 7261 7465 2870 6f6f 6c2e 696d 6170 2874  rate(pool.imap(t
+00010d80: 7261 6e73 6372 6970 745f 7472 616e 736c  ranscript_transl
+00010d90: 6174 6f72 2c20 6372 6561 7465 645f 7375  ator, created_su
+00010da0: 6274 6974 6c65 7329 293a 0d0a 2020 2020  btitles)):..    
+00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010dc0: 7472 616e 736c 6174 6564 5f73 7562 7469  translated_subti
+00010dd0: 746c 6573 2e61 7070 656e 6428 7472 616e  tles.append(tran
+00010de0: 736c 6174 6564 5f73 7562 7469 746c 6529  slated_subtitle)
+00010df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010e00: 2020 2020 2020 7062 6172 2e75 7064 6174        pbar.updat
+00010e10: 6528 6929 0d0a 2020 2020 2020 2020 2020  e(i)..          
+00010e20: 2020 2020 2020 7062 6172 2e66 696e 6973        pbar.finis
+00010e30: 6828 290d 0a0d 0a20 2020 2020 2020 2020  h()....         
+00010e40: 2020 2020 2020 2074 7261 6e73 6c61 7465         translate
+00010e50: 645f 7375 6274 6974 6c65 5f66 696c 6570  d_subtitle_filep
+00010e60: 6174 6820 3d20 7375 6274 6974 6c65 5f66  ath = subtitle_f
+00010e70: 696c 6570 6174 685b 203a 2d34 5d20 2b20  ilepath[ :-4] + 
+00010e80: 272e 7472 616e 736c 6174 6564 2e27 202b  '.translated.' +
+00010e90: 2073 7562 7469 746c 655f 666f 726d 6174   subtitle_format
+00010ea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010eb0: 2020 7472 616e 736c 6174 696f 6e5f 7772    translation_wr
+00010ec0: 6974 6572 203d 2053 7562 7469 746c 6557  iter = SubtitleW
+00010ed0: 7269 7465 7228 6372 6561 7465 645f 7265  riter(created_re
+00010ee0: 6769 6f6e 732c 2074 7261 6e73 6c61 7465  gions, translate
+00010ef0: 645f 7375 6274 6974 6c65 732c 2073 7562  d_subtitles, sub
+00010f00: 7469 746c 655f 666f 726d 6174 2c20 6572  title_format, er
+00010f10: 726f 725f 6d65 7373 6167 6573 5f63 616c  ror_messages_cal
+00010f20: 6c62 6163 6b3d 7368 6f77 5f65 7272 6f72  lback=show_error
+00010f30: 5f6d 6573 7361 6765 7329 0d0a 2020 2020  _messages)..    
+00010f40: 2020 2020 2020 2020 2020 2020 7472 616e              tran
+00010f50: 736c 6174 696f 6e5f 7772 6974 6572 2e77  slation_writer.w
+00010f60: 7269 7465 2874 7261 6e73 6c61 7465 645f  rite(translated_
+00010f70: 7375 6274 6974 6c65 5f66 696c 6570 6174  subtitle_filepat
+00010f80: 6829 0d0a 0d0a 2020 2020 2020 2020 2020  h)....          
+00010f90: 2020 7072 696e 7428 2744 6f6e 652e 2729    print('Done.')
+00010fa0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00010fb0: 2064 6f5f 7472 616e 736c 6174 653a 0d0a   do_translate:..
+00010fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fd0: 6f73 2e72 656d 6f76 6528 7375 6274 6974  os.remove(subtit
+00010fe0: 6c65 5f66 696c 6570 6174 6829 0d0a 2020  le_filepath)..  
+00010ff0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00011000: 696e 7428 2754 7261 6e73 6c61 7465 6420  int('Translated 
+00011010: 7375 6274 6974 6c65 7320 6669 6c65 2063  subtitles file c
+00011020: 7265 6174 6564 2061 7420 2020 203a 207b  reated at    : {
+00011030: 7d27 202e 666f 726d 6174 2874 7261 6e73  }' .format(trans
+00011040: 6c61 7465 645f 7375 6274 6974 6c65 5f66  lated_subtitle_f
+00011050: 696c 6570 6174 6829 290d 0a20 2020 2020  ilepath))..     
+00011060: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00011070: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00011080: 696e 7428 2253 7562 7469 746c 6573 2066  int("Subtitles f
+00011090: 696c 6520 6372 6561 7465 6420 6174 2020  ile created at  
+000110a0: 2020 2020 2020 2020 2020 2020 203a 207b               : {
+000110b0: 7d22 2e66 6f72 6d61 7428 7375 6274 6974  }".format(subtit
+000110c0: 6c65 5f66 696c 6570 6174 6829 290d 0a20  le_filepath)).. 
+000110d0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000110e0: 2827 2729 0d0a 2020 2020 2020 2020 2020  ('')..          
+000110f0: 2020 636f 6d70 6c65 7465 645f 7461 736b    completed_task
+00011100: 7320 2b3d 2031 0d0a 0d0a 2020 2020 2020  s += 1....      
+00011110: 2020 2020 2020 6966 206c 656e 286d 6564        if len(med
+00011120: 6961 5f66 696c 6570 6174 6873 293e 3020  ia_filepaths)>0 
+00011130: 616e 6420 636f 6d70 6c65 7465 645f 7461  and completed_ta
+00011140: 736b 7320 3d3d 206c 656e 286d 6564 6961  sks == len(media
+00011150: 5f66 696c 6570 6174 6873 293a 0d0a 2020  _filepaths):..  
+00011160: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00011170: 616e 7363 7269 6265 5f65 6e64 5f74 696d  anscribe_end_tim
+00011180: 6520 3d20 7469 6d65 2e74 696d 6528 290d  e = time.time().
+00011190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000111a0: 2074 7261 6e73 6372 6962 655f 656c 6170   transcribe_elap
+000111b0: 7365 645f 7469 6d65 203d 2074 7261 6e73  sed_time = trans
+000111c0: 6372 6962 655f 656e 645f 7469 6d65 202d  cribe_end_time -
+000111d0: 2074 7261 6e73 6372 6962 655f 7374 6172   transcribe_star
+000111e0: 745f 7469 6d65 0d0a 2020 2020 2020 2020  t_time..        
+000111f0: 2020 2020 2020 2020 7472 616e 7363 7269          transcri
+00011200: 6265 5f65 6c61 7073 6564 5f74 696d 655f  be_elapsed_time_
+00011210: 7365 636f 6e64 7320 3d20 7469 6d65 6465  seconds = timede
+00011220: 6c74 6128 7365 636f 6e64 733d 696e 7428  lta(seconds=int(
+00011230: 7472 616e 7363 7269 6265 5f65 6c61 7073  transcribe_elaps
+00011240: 6564 5f74 696d 6529 290d 0a20 2020 2020  ed_time))..     
+00011250: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
+00011260: 6372 6962 655f 656c 6170 7365 645f 7469  cribe_elapsed_ti
+00011270: 6d65 5f73 7472 203d 2073 7472 2874 7261  me_str = str(tra
+00011280: 6e73 6372 6962 655f 656c 6170 7365 645f  nscribe_elapsed_
+00011290: 7469 6d65 5f73 6563 6f6e 6473 290d 0a20  time_seconds).. 
+000112a0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+000112b0: 6f75 722c 206d 696e 7574 652c 2073 6563  our, minute, sec
+000112c0: 6f6e 6420 3d20 7472 616e 7363 7269 6265  ond = transcribe
+000112d0: 5f65 6c61 7073 6564 5f74 696d 655f 7374  _elapsed_time_st
+000112e0: 722e 7370 6c69 7428 223a 2229 0d0a 2020  r.split(":")..  
+000112f0: 2020 2020 2020 2020 2020 2020 2020 6d73                ms
+00011300: 6720 3d20 2254 6f74 616c 2074 7261 6e73  g = "Total trans
+00011310: 6372 6962 6520 7469 6d65 2020 2020 2020  cribe time      
+00011320: 2020 2020 2020 2020 2020 2020 203a 2025               : %
+00011330: 733a 2573 3a25 7322 2025 2868 6f75 722e  s:%s:%s" %(hour.
+00011340: 7a66 696c 6c28 3229 2c20 6d69 6e75 7465  zfill(2), minute
+00011350: 2c20 7365 636f 6e64 290d 0a20 2020 2020  , second)..     
+00011360: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00011370: 286d 7367 290d 0a0d 0a20 2020 2020 2020  (msg)....       
+00011380: 2065 7863 6570 7420 4b65 7962 6f61 7264   except Keyboard
+00011390: 496e 7465 7272 7570 743a 0d0a 2020 2020  Interrupt:..    
+000113a0: 2020 2020 2020 2020 7062 6172 2e66 696e          pbar.fin
+000113b0: 6973 6828 290d 0a20 2020 2020 2020 2020  ish()..         
+000113c0: 2020 2070 6f6f 6c2e 7465 726d 696e 6174     pool.terminat
+000113d0: 6528 290d 0a20 2020 2020 2020 2020 2020  e()..           
+000113e0: 2070 6f6f 6c2e 636c 6f73 6528 290d 0a20   pool.close().. 
+000113f0: 2020 2020 2020 2020 2020 2070 6f6f 6c2e             pool.
+00011400: 6a6f 696e 2829 0d0a 2020 2020 2020 2020  join()..        
+00011410: 2020 2020 7072 696e 7428 2243 616e 6365      print("Cance
+00011420: 6c6c 696e 6720 616c 6c20 7461 736b 7322  lling all tasks"
+00011430: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00011440: 2069 6620 7379 732e 706c 6174 666f 726d   if sys.platform
+00011450: 203d 3d20 2277 696e 3332 223a 0d0a 2020   == "win32":..  
+00011460: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00011470: 6f70 5f66 666d 7065 675f 7769 6e64 6f77  op_ffmpeg_window
+00011480: 7328 6572 726f 725f 6d65 7373 6167 6573  s(error_messages
+00011490: 5f63 616c 6c62 6163 6b3d 7368 6f77 5f65  _callback=show_e
+000114a0: 7272 6f72 5f6d 6573 7361 6765 7329 0d0a  rror_messages)..
+000114b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000114c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000114d0: 2020 2073 746f 705f 6666 6d70 6567 5f6c     stop_ffmpeg_l
+000114e0: 696e 7578 2865 7272 6f72 5f6d 6573 7361  inux(error_messa
+000114f0: 6765 735f 6361 6c6c 6261 636b 3d73 686f  ges_callback=sho
+00011500: 775f 6572 726f 725f 6d65 7373 6167 6573  w_error_messages
+00011510: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00011520: 2072 656d 6f76 655f 7465 6d70 5f66 696c   remove_temp_fil
+00011530: 6573 2822 7761 7622 290d 0a20 2020 2020  es("wav")..     
+00011540: 2020 2020 2020 2072 6574 7572 6e20 310d         return 1.
+00011550: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
+00011560: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00011570: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+00011580: 6620 6e6f 7420 4b65 7962 6f61 7264 496e  f not KeyboardIn
+00011590: 7465 7272 7570 7420 696e 2065 3a0d 0a20  terrupt in e:.. 
+000115a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000115b0: 6261 722e 6669 6e69 7368 2829 0d0a 2020  bar.finish()..  
+000115c0: 2020 2020 2020 2020 2020 2020 2020 706f                po
+000115d0: 6f6c 2e74 6572 6d69 6e61 7465 2829 0d0a  ol.terminate()..
+000115e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115f0: 706f 6f6c 2e63 6c6f 7365 2829 0d0a 2020  pool.close()..  
+00011600: 2020 2020 2020 2020 2020 2020 2020 706f                po
+00011610: 6f6c 2e6a 6f69 6e28 290d 0a20 2020 2020  ol.join()..     
+00011620: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00011630: 2865 290d 0a0d 0a20 2020 2020 2020 2020  (e)....         
+00011640: 2020 2020 2020 2069 6620 7379 732e 706c         if sys.pl
+00011650: 6174 666f 726d 203d 3d20 2277 696e 3332  atform == "win32
+00011660: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+00011670: 2020 2020 2020 2020 7374 6f70 5f66 666d          stop_ffm
+00011680: 7065 675f 7769 6e64 6f77 7328 6572 726f  peg_windows(erro
+00011690: 725f 6d65 7373 6167 6573 5f63 616c 6c62  r_messages_callb
+000116a0: 6163 6b3d 7368 6f77 5f65 7272 6f72 5f6d  ack=show_error_m
+000116b0: 6573 7361 6765 7329 0d0a 2020 2020 2020  essages)..      
+000116c0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+000116d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000116e0: 2020 2020 2073 746f 705f 6666 6d70 6567       stop_ffmpeg
+000116f0: 5f6c 696e 7578 2865 7272 6f72 5f6d 6573  _linux(error_mes
+00011700: 7361 6765 735f 6361 6c6c 6261 636b 3d73  sages_callback=s
+00011710: 686f 775f 6572 726f 725f 6d65 7373 6167  how_error_messag
+00011720: 6573 290d 0a0d 0a20 2020 2020 2020 2020  es)....         
+00011730: 2020 2020 2020 2072 656d 6f76 655f 7465         remove_te
+00011740: 6d70 5f66 696c 6573 2822 7761 7622 290d  mp_files("wav").
+00011750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011760: 2072 6574 7572 6e20 310d 0a0d 0a20 2020   return 1....   
+00011770: 2069 6620 706f 6f6c 3a0d 0a20 2020 2020   if pool:..     
+00011780: 2020 2070 6f6f 6c2e 636c 6f73 6528 290d     pool.close().
+00011790: 0a20 2020 2020 2020 2070 6f6f 6c2e 6a6f  .        pool.jo
+000117a0: 696e 2829 0d0a 2020 2020 2020 2020 706f  in()..        po
+000117b0: 6f6c 203d 204e 6f6e 650d 0a0d 0a20 2020  ol = None....   
+000117c0: 2069 6620 7379 732e 706c 6174 666f 726d   if sys.platform
+000117d0: 203d 3d20 2277 696e 3332 223a 0d0a 2020   == "win32":..  
+000117e0: 2020 2020 2020 7374 6f70 5f66 666d 7065        stop_ffmpe
+000117f0: 675f 7769 6e64 6f77 7328 6572 726f 725f  g_windows(error_
+00011800: 6d65 7373 6167 6573 5f63 616c 6c62 6163  messages_callbac
+00011810: 6b3d 7368 6f77 5f65 7272 6f72 5f6d 6573  k=show_error_mes
+00011820: 7361 6765 7329 0d0a 2020 2020 656c 7365  sages)..    else
+00011830: 3a0d 0a20 2020 2020 2020 2073 746f 705f  :..        stop_
+00011840: 6666 6d70 6567 5f6c 696e 7578 2865 7272  ffmpeg_linux(err
+00011850: 6f72 5f6d 6573 7361 6765 735f 6361 6c6c  or_messages_call
+00011860: 6261 636b 3d73 686f 775f 6572 726f 725f  back=show_error_
+00011870: 6d65 7373 6167 6573 290d 0a0d 0a20 2020  messages)....   
+00011880: 2072 656d 6f76 655f 7465 6d70 5f66 696c   remove_temp_fil
+00011890: 6573 2822 7761 7622 290d 0a0d 0a69 6620  es("wav")....if 
+000118a0: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
+000118b0: 6169 6e5f 5f27 3a0d 0a20 2020 206d 756c  ain__':..    mul
+000118c0: 7469 7072 6f63 6573 7369 6e67 2e66 7265  tiprocessing.fre
+000118d0: 657a 655f 7375 7070 6f72 7428 290d 0a20  eze_support().. 
+000118e0: 2020 2073 7973 2e65 7869 7428 6d61 696e     sys.exit(main
+000118f0: 2829 290d 0a                             ())..
```

### Comparing `whisper_autosrt-0.0.5/whisper_autosrt.egg-info/PKG-INFO` & `whisper_autosrt-0.0.6/whisper_autosrt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-autosrt
-Version: 0.0.5
+Version: 0.0.6
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
@@ -24,8 +24,8 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 
-whisper_autosrt is a utility for automatic speech recognition and subtitle generation.  It takes video or audio files as input, convert it to a temporary wav file then generatetranscriptions for that wav file, and optionally translates them to a different languageand finally saves the resulting subtitles file to disk.                                 It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT, JSON, and RAW format.
+whisper_autosrt is a command line utility for automatic speech recognition and subtitle generation. It takes video or audio files as input, generate transcriptions for them and optionally translates  them to a different language, and finally saves the resulting subtitles file to disk.               It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT,JSON, and RAW format.
```

