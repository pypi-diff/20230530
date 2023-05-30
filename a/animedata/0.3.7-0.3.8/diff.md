# Comparing `tmp/animedata-0.3.7.tar.gz` & `tmp/animedata-0.3.8.tar.gz`

## Comparing `animedata-0.3.7.tar` & `animedata-0.3.8.tar`

### file list

```diff
@@ -1,6 +1,15 @@
--rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 animedata-0.3.7/animedata/resources/animedata_source.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 animedata-0.3.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 animedata-0.3.7/LICENSE
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 animedata-0.3.7/README.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 animedata-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 animedata-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/common/__init__.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/common/dict_checking.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/common/lib_interactions.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/common/metadata.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/common/saving_process.py
+-rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/resources/animedata_source.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/tests/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/tests/test_dict_checking.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 animedata-0.3.8/animedata/tests/test_lib_interaction.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 animedata-0.3.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 animedata-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 animedata-0.3.8/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 animedata-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 animedata-0.3.8/PKG-INFO
```

### Comparing `animedata-0.3.7/animedata/resources/animedata_source.json` & `animedata-0.3.8/animedata/resources/animedata_source.json`

 * *Files identical despite different names*

### Comparing `animedata-0.3.7/LICENSE` & `animedata-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `animedata-0.3.7/README.md` & `animedata-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `animedata-0.3.7/pyproject.toml` & `animedata-0.3.8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -5,44 +5,42 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 746f 6f6c 2e68 6174 6368 2e62 7569 6c64  tool.hatch.build
 00000060: 5d0d 0a65 7863 6c75 6465 203d 205b 0d0a  ]..exclude = [..
 00000070: 2020 222f 6469 7374 222c 0d0a 2020 222f    "/dist",..  "/
 00000080: 2e67 6974 222c 0d0a 2020 222e 6769 7469  .git",..  ".giti
 00000090: 676e 6f72 6522 0d0a 2020 5d0d 0a69 6e63  gnore"..  ]..inc
 000000a0: 6c75 6465 203d 205b 0d0a 2020 2261 6e69  lude = [..  "ani
-000000b0: 6d65 6461 7461 2f72 6573 6f75 7263 6573  medata/resources
-000000c0: 2f61 6e69 6d65 6461 7461 5f73 6f75 7263  /animedata_sourc
-000000d0: 652e 6a73 6f6e 220d 0a5d 0d0a 0d0a 5b70  e.json"..]....[p
-000000e0: 726f 6a65 6374 5d0d 0a6e 616d 6520 3d20  roject]..name = 
-000000f0: 2261 6e69 6d65 6461 7461 220d 0a76 6572  "animedata"..ver
-00000100: 7369 6f6e 203d 2022 302e 332e 3722 0d0a  sion = "0.3.7"..
-00000110: 6175 7468 6f72 7320 3d20 5b0d 0a20 7b6e  authors = [.. {n
-00000120: 616d 653d 2273 7761 7274 6875 7222 7d0d  ame="swarthur"}.
-00000130: 0a5d 0d0a 6465 7363 7269 7074 696f 6e20  .]..description 
-00000140: 3d20 224f 7065 6e2d 736f 7572 6365 206c  = "Open-source l
-00000150: 6962 7261 7279 2063 6f6e 7461 696e 696e  ibrary containin
-00000160: 6720 7061 636b 6167 6520 6162 6f75 7420  g package about 
-00000170: 616e 696d 6573 2f73 6572 6965 7320 616e  animes/series an
-00000180: 6420 696e 636c 7564 696e 6720 6120 6275  d including a bu
-00000190: 696c 742d 696e 2075 7469 6c69 7479 2e22  ilt-in utility."
-000001a0: 0d0a 7265 6164 6d65 203d 2022 5245 4144  ..readme = "READ
-000001b0: 4d45 2e6d 6422 0d0a 7265 7175 6972 6573  ME.md"..requires
-000001c0: 2d70 7974 686f 6e20 3d20 223e 3d33 2e31  -python = ">=3.1
-000001d0: 3122 0d0a 6c69 6365 6e73 6520 3d20 224d  1"..license = "M
-000001e0: 4954 220d 0a63 6c61 7373 6966 6965 7273  IT"..classifiers
-000001f0: 203d 205b 0d0a 2020 2020 2250 726f 6772   = [..    "Progr
-00000200: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000210: 3a3a 2050 7974 686f 6e20 3a3a 2033 222c  :: Python :: 3",
-00000220: 0d0a 2020 2020 224c 6963 656e 7365 203a  ..    "License :
-00000230: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000240: 3a20 4d49 5420 4c69 6365 6e73 6522 2c0d  : MIT License",.
-00000250: 0a20 2020 2022 4f70 6572 6174 696e 6720  .    "Operating 
-00000260: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000270: 6570 656e 6465 6e74 222c 0d0a 5d0d 0a0d  ependent",..]...
-00000280: 0a5b 7072 6f6a 6563 742e 7572 6c73 5d0d  .[project.urls].
-00000290: 0a22 4769 7468 7562 2220 3d20 2268 7474  ."Github" = "htt
-000002a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000002b0: 7377 6172 7468 7572 2f61 6e69 6d65 6461  swarthur/animeda
-000002c0: 7461 220d 0a22 4275 6722 203d 2022 6874  ta".."Bug" = "ht
-000002d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000002e0: 2f73 7761 7274 6875 722f 616e 696d 6564  /swarthur/animed
-000002f0: 6174 612f 6973 7375 6573 220d 0a         ata/issues"..
+000000b0: 6d65 6461 7461 2f2a 220d 0a5d 0d0a 0d0a  medata/*"..]....
+000000c0: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
+000000d0: 3d20 2261 6e69 6d65 6461 7461 220d 0a76  = "animedata"..v
+000000e0: 6572 7369 6f6e 203d 2022 302e 332e 3822  ersion = "0.3.8"
+000000f0: 0d0a 6175 7468 6f72 7320 3d20 5b0d 0a20  ..authors = [.. 
+00000100: 7b6e 616d 653d 2273 7761 7274 6875 7222  {name="swarthur"
+00000110: 7d0d 0a5d 0d0a 6465 7363 7269 7074 696f  }..]..descriptio
+00000120: 6e20 3d20 224f 7065 6e2d 736f 7572 6365  n = "Open-source
+00000130: 206c 6962 7261 7279 2063 6f6e 7461 696e   library contain
+00000140: 696e 6720 7061 636b 6167 6520 6162 6f75  ing package abou
+00000150: 7420 616e 696d 6573 2f73 6572 6965 7320  t animes/series 
+00000160: 616e 6420 696e 636c 7564 696e 6720 6120  and including a 
+00000170: 6275 696c 742d 696e 2075 7469 6c69 7479  built-in utility
+00000180: 2e22 0d0a 7265 6164 6d65 203d 2022 5245  ."..readme = "RE
+00000190: 4144 4d45 2e6d 6422 0d0a 7265 7175 6972  ADME.md"..requir
+000001a0: 6573 2d70 7974 686f 6e20 3d20 223e 3d33  es-python = ">=3
+000001b0: 2e31 3122 0d0a 6c69 6365 6e73 6520 3d20  .11"..license = 
+000001c0: 224d 4954 220d 0a63 6c61 7373 6966 6965  "MIT"..classifie
+000001d0: 7273 203d 205b 0d0a 2020 2020 2250 726f  rs = [..    "Pro
+000001e0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001f0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000200: 222c 0d0a 2020 2020 224c 6963 656e 7365  ",..    "License
+00000210: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000220: 203a 3a20 4d49 5420 4c69 6365 6e73 6522   :: MIT License"
+00000230: 2c0d 0a20 2020 2022 4f70 6572 6174 696e  ,..    "Operatin
+00000240: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+00000250: 6e64 6570 656e 6465 6e74 222c 0d0a 5d0d  ndependent",..].
+00000260: 0a0d 0a5b 7072 6f6a 6563 742e 7572 6c73  ...[project.urls
+00000270: 5d0d 0a22 4769 7468 7562 2220 3d20 2268  ].."Github" = "h
+00000280: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000290: 6d2f 7377 6172 7468 7572 2f61 6e69 6d65  m/swarthur/anime
+000002a0: 6461 7461 220d 0a22 4275 6722 203d 2022  data".."Bug" = "
+000002b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000002c0: 6f6d 2f73 7761 7274 6875 722f 616e 696d  om/swarthur/anim
+000002d0: 6564 6174 612f 6973 7375 6573 220d 0a    edata/issues"..
```

### Comparing `animedata-0.3.7/PKG-INFO` & `animedata-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animedata
-Version: 0.3.7
+Version: 0.3.8
 Summary: Open-source library containing package about animes/series and including a built-in utility.
 Project-URL: Github, https://github.com/swarthur/animedata
 Project-URL: Bug, https://github.com/swarthur/animedata/issues
 Author: swarthur
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

