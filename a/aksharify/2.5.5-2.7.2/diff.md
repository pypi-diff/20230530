# Comparing `tmp/aksharify-2.5.5.tar.gz` & `tmp/aksharify-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-2.5.5.tar", max compression
+gzip compressed data, was "aksharify-2.7.2.tar", max compression
```

## Comparing `aksharify-2.5.5.tar` & `aksharify-2.7.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       24 2023-05-29 15:23:03.528860 aksharify-2.5.5/aksharify/__init__.py
--rw-r--r--   0        0        0     6793 2023-05-29 15:26:23.653035 aksharify-2.5.5/aksharify/aksharify.py
--rw-r--r--   0        0        0      901 2023-05-29 15:55:21.776703 aksharify-2.5.5/pyproject.toml
--rw-r--r--   0        0        0     4358 2023-05-29 15:59:45.530987 aksharify-2.5.5/README.md
--rw-r--r--   0        0        0     5132 1970-01-01 00:00:00.000000 aksharify-2.5.5/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-05-29 15:23:03.528860 aksharify-2.7.2/aksharify/__init__.py
+-rw-r--r--   0        0        0     7234 2023-05-30 14:05:22.226629 aksharify-2.7.2/aksharify/aksharify.py
+-rw-r--r--   0        0        0      901 2023-05-30 14:33:38.944602 aksharify-2.7.2/pyproject.toml
+-rw-r--r--   0        0        0     5864 2023-05-30 14:27:02.119233 aksharify-2.7.2/README.md
+-rw-r--r--   0        0        0     6619 1970-01-01 00:00:00.000000 aksharify-2.7.2/PKG-INFO
```

### Comparing `aksharify-2.5.5/aksharify/aksharify.py` & `aksharify-2.7.2/aksharify/aksharify.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 # -*- coding: utf-8-*-
 
 from PIL import Image
+import requests
+from io import BytesIO
 
 
 SVG_HEADER = '<?xml version="1.0" standalone="no"?><svg width="{}" height="{}" version="1.1" xmlns="http://www.w3.org/2000/svg" style="font-family: {}; font-size:{};"><desc>Aksharify Art</desc><rect width="100%" height="100%" fill="{}"/>'
 HTML_HEADER = '<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1.0"><title>Aksharify Art</title></head><body><a href="https://primepatel.github.io/aksharify-docs/">{}</a></body></html>'
 SORTEDCHARS = """ `.-_',~:*;!"^/\+><r=?()|7LxtcYivTljsz[]1Jnufy{}oI#FC4VX2ehk3aZw5ASbdpqUP6%9G8mKO&0EDHg$MWRNQB@"""
 
+def URLtoImg(url):
+    response = requests.get(url)
+    image_data = response.content
+    try:
+        Image.open(BytesIO(image_data))
+        return BytesIO(image_data)
+    except:
+        print("The provided URL does not correspond to an image.")
+
+
 class AksharArt:
     
     def __init__(self, image, chars="01") -> None:
         self.image = Image.open(image)
         self.w, self.h = self.image.size
         self.chars = list(set(chars))
         self.CH_CONSTANT = 2.143
         self.H_dis, self.V_dis = 11.1, 20
+        self.font_size = 20
 
     def set_dim(self, width=None, height=None):
         if width != None and height == None:
             self.w, self.h = width, int(
                 (self.h/self.w * width)/self.CH_CONSTANT)
         elif width == None and height != None:
             self.w, self.h = int((self.w/self.h * height)
@@ -71,15 +84,15 @@
     def rgb2hex(self, rgba):
         return '#{:02x}{:02x}{:02x}'.format(rgba[0], rgba[1], rgba[2])
 
     def svgify(self, bg_color="None"):
         file = SVG_HEADER.format(
             int(self.w*self.H_dis)+41, 
             int(self.h*self.V_dis)+41,
-            "monospace", 20, bg_color
+            "monospace", self.font_size, bg_color
             )
         file += f'<a href="https://primepatel.github.io/aksharify-docs/">'
         x, y = 20, 30
         for line_no in range(self.h):
             file += f'<text x="{x}" y="{y}">'
             for char_no in range(self.w):
                 file += self.tspan(
@@ -107,35 +120,36 @@
         self.ascii_html = HTML_HEADER.format(html_content)
     
     def html_output(self, fname):
         with open(fname + ".html", "w") as file:
             file.write(self.ascii_html)
 
     def svg_output(self, fname):
-        with open(fname + ".svg", "w") as file:
+        with open(fname + ".svg", "w", encoding="utf-8-sig") as file:
             file.write(self.ascii_svg)
     
     def png_output(self, fname, svg2png, bg_color="None", height=None, width=None):
         self.svgify(bg_color)
         if height == None and width != None:
             svg2png(bytestring=self.ascii_svg,write_to=fname+'.png',output_width=width)
         elif width == None and height != None:
             svg2png(bytestring=self.ascii_svg,write_to=fname+'.png',output_height=height)
         elif height == None and width == None:
             svg2png(bytestring=self.ascii_svg, write_to=fname+'.png')
         else:
             svg2png(bytestring=self.ascii_svg,write_to=fname+'.png',output_height=height,output_width=width)
 
 
-class TextArt(AksharArt):
-    """_summary_
+class EmojiArt(AksharArt):
+    def __init__(self, image, chars="🙂😅") -> None:
+        super().__init__(image, chars)
+        self.H_dis = 20
 
-    Args:
-        AksharArt (_type_): _description_
-    """
+class TextArt(AksharArt):
+    
     def __init__(self, image, chars=SORTEDCHARS, ordered=False) -> None:
         super().__init__(image)
         self.chars = list(set(chars))
         if not ordered:
             chars = []
             for char in SORTEDCHARS:
                 if char in self.chars:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharify-2.5.5/pyproject.toml` & `aksharify-2.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2261 6b73 6861 7269 6679  ame = "aksharify
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 322e  "..version = "2.
-00000030: 352e 3522 0d0a 6465 7363 7269 7074 696f  5.5"..descriptio
+00000030: 372e 3222 0d0a 6465 7363 7269 7074 696f  7.2"..descriptio
 00000040: 6e20 3d20 2250 7974 686f 6e20 4173 6369  n = "Python Asci
 00000050: 6920 2b20 456d 6f6a 6920 4172 7420 4d6f  i + Emoji Art Mo
 00000060: 6475 6c65 220d 0a61 7574 686f 7273 203d  dule"..authors =
 00000070: 205b 2250 7269 6d65 2050 6174 656c 203c   ["Prime Patel <
 00000080: 7072 696d 6573 7061 7465 6c40 676d 6169  primespatel@gmai
 00000090: 6c2e 636f 6d3e 225d 0d0a 6c69 6365 6e73  l.com>"]..licens
 000000a0: 6520 3d20 224d 4954 220d 0a72 6561 646d  e = "MIT"..readm
```

### Comparing `aksharify-2.5.5/PKG-INFO` & `aksharify-2.7.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 616b 7368  : 2.1.Name: aksh
 00000020: 6172 6966 790a 5665 7273 696f 6e3a 2032  arify.Version: 2
-00000030: 2e35 2e35 0a53 756d 6d61 7279 3a20 5079  .5.5.Summary: Py
+00000030: 2e37 2e32 0a53 756d 6d61 7279 3a20 5079  .7.2.Summary: Py
 00000040: 7468 6f6e 2041 7363 6969 202b 2045 6d6f  thon Ascii + Emo
 00000050: 6a69 2041 7274 204d 6f64 756c 650a 486f  ji Art Module.Ho
 00000060: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 00000070: 2f70 7269 6d65 7061 7465 6c2e 6769 7468  /primepatel.gith
 00000080: 7562 2e69 6f2f 616b 7368 6172 6966 792d  ub.io/aksharify-
 00000090: 646f 6373 2f0a 4c69 6365 6e73 653a 204d  docs/.License: M
 000000a0: 4954 0a4b 6579 776f 7264 733a 2041 7363  IT.Keywords: Asc
@@ -74,248 +74,341 @@
 00000490: 6e5d 5b6c 696e 6b65 6469 6e2d 7368 6965  n][linkedin-shie
 000004a0: 6c64 5d5d 5b6c 696e 6b65 6469 6e2d 7572  ld]][linkedin-ur
 000004b0: 6c5d 0a5b 215b 5079 5049 202d 2044 6f77  l].[![PyPI - Dow
 000004c0: 6e6c 6f61 6473 5d5b 446f 776e 6c6f 6164  nloads][Download
 000004d0: 732d 7368 6965 6c64 5d5d 2868 7474 7073  s-shield]](https
 000004e0: 3a2f 2f70 7970 6973 7461 7473 2e6f 7267  ://pypistats.org
 000004f0: 2f70 6163 6b61 6765 732f 616b 7368 6172  /packages/akshar
-00000500: 6966 7929 0a0a 3c62 7220 2f3e 0a0a 3c21  ify)..<br />..<!
-00000510: 2d2d 2041 424f 5554 2054 4845 2050 524f  -- ABOUT THE PRO
-00000520: 4a45 4354 202d 2d3e 0a23 2320 4162 6f75  JECT -->.## Abou
-00000530: 7420 7468 6520 6d6f 6475 6c65 0a0a 5468  t the module..Th
-00000540: 6520 696e 7370 6972 6174 696f 6e20 666f  e inspiration fo
-00000550: 7220 7468 6973 206d 6f64 756c 6520 6361  r this module ca
-00000560: 6d65 2066 726f 6d20 6120 4e75 6d62 6572  me from a Number
-00000570: 7068 696c 6520 7669 6465 6f20 6361 6c6c  phile video call
-00000580: 6564 2022 5468 6520 5472 696e 6974 7920  ed "The Trinity 
-00000590: 4861 6c6c 2050 7269 6d65 2c22 2077 6869  Hall Prime," whi
-000005a0: 6368 2049 2066 6972 7374 2073 6177 2069  ch I first saw i
-000005b0: 6e20 6869 6768 2073 6368 6f6f 6c20 6461  n high school da
-000005c0: 7973 2e20 4974 206d 6f74 6976 6174 6564  ys. It motivated
-000005d0: 206d 6520 746f 2065 7870 6c6f 7265 2074   me to explore t
-000005e0: 6865 2070 6f73 7369 6269 6c69 7469 6573  he possibilities
-000005f0: 206f 6620 7375 6368 2061 2070 7269 6d65   of such a prime
-00000600: 206e 756d 6265 722e 2049 2063 7265 6174   number. I creat
-00000610: 6564 2061 2050 7974 686f 6e20 6d6f 6475  ed a Python modu
-00000620: 6c65 2074 6861 7420 7573 6573 2061 2070  le that uses a p
-00000630: 7265 6465 7465 726d 696e 6564 2063 6861  redetermined cha
-00000640: 7261 6374 6572 2073 6574 2074 6f20 7475  racter set to tu
-00000650: 726e 2070 686f 746f 7320 696e 746f 2041  rn photos into A
-00000660: 5343 4949 2061 7274 2e20 4974 206d 616e  SCII art. It man
-00000670: 6970 756c 6174 6573 2069 6d61 6765 7320  ipulates images 
-00000680: 7573 696e 6720 7468 6520 5049 4c20 7061  using the PIL pa
-00000690: 636b 6167 652c 2074 7261 6e73 666f 726d  ckage, transform
-000006a0: 696e 6720 7468 656d 2074 6f20 6772 6179  ing them to gray
-000006b0: 7363 616c 6520 6265 666f 7265 206d 6170  scale before map
-000006c0: 7069 6e67 2070 6978 656c 2076 616c 7565  ping pixel value
-000006d0: 7320 746f 2041 5343 4949 206c 6574 7465  s to ASCII lette
-000006e0: 7273 2e20 5573 6572 7320 6361 6e20 6368  rs. Users can ch
-000006f0: 616e 6765 2074 6865 2063 6861 7261 6374  ange the charact
-00000700: 6572 2073 6574 2074 6f20 6765 7420 6469  er set to get di
-00000710: 6666 6572 656e 7420 6566 6665 6374 732e  fferent effects.
-00000720: 0a0a 3c21 2d2d 2047 4554 5449 4e47 2053  ..<!-- GETTING S
-00000730: 5441 5254 4544 202d 2d3e 0a23 2320 4765  TARTED -->.## Ge
-00000740: 7474 696e 6720 5374 6172 7465 640a 0a42  tting Started..B
-00000750: 6566 6f72 6520 7765 2062 6567 696e 2c20  efore we begin, 
-00000760: 6d61 6b65 2073 7572 6520 796f 7520 6861  make sure you ha
-00000770: 7665 206f 6e65 206f 6620 7265 6365 6e74  ve one of recent
-00000780: 2076 6572 7369 6f6e 7320 6f66 2050 7974   versions of Pyt
-00000790: 686f 6e20 696e 7374 616c 6c65 6420 6f6e  hon installed on
-000007a0: 2079 6f75 7220 636f 6d70 7574 6572 2e0a   your computer..
-000007b0: 0a23 2323 2049 6e73 7461 6c6c 6174 696f  .### Installatio
-000007c0: 6e0a 0a60 6060 7368 0a70 7974 686f 6e20  n..```sh.python 
-000007d0: 2d6d 2070 6970 2069 6e73 7461 6c6c 2061  -m pip install a
-000007e0: 6b73 6861 7269 6679 0a60 6060 0a0a 2323  ksharify.```..##
-000007f0: 2055 7361 6765 0a0a 6060 6070 7974 686f   Usage..```pytho
-00000800: 6e0a 6672 6f6d 2061 6b73 6861 7269 6679  n.from aksharify
-00000810: 2069 6d70 6f72 7420 5465 7874 4172 740a   import TextArt.
-00000820: 0a23 2069 6e70 7574 2069 6d61 6765 2066  .# input image f
-00000830: 696c 650a 6172 7420 3d20 5465 7874 4172  ile.art = TextAr
-00000840: 7428 224a 756c 6961 2e70 6e67 2229 0a0a  t("Julia.png")..
-00000850: 2320 7365 6520 696d 6167 650a 6172 742e  # see image.art.
-00000860: 696d 6167 652e 7368 6f77 2829 0a0a 2320  image.show()..# 
-00000870: 7365 7420 6469 6d65 6e73 696f 6e20 6f66  set dimension of
-00000880: 206f 7574 7075 7420 7465 7874 0a61 7274   output text.art
-00000890: 2e73 6574 5f64 696d 2838 3029 0a0a 2320  .set_dim(80)..# 
-000008a0: 6765 6e65 7461 7465 2074 6578 740a 6172  genetate text.ar
-000008b0: 742e 6173 6369 6966 7928 290a 0a23 206f  t.asciify()..# o
-000008c0: 7574 7075 7420 696e 746f 202e 7478 7420  utput into .txt 
-000008d0: 6669 6c65 0a61 7274 2e74 6578 745f 6f75  file.art.text_ou
-000008e0: 7470 7574 2822 6f75 7470 7574 2229 0a0a  tput("output")..
-000008f0: 2320 6765 6e65 7261 7465 2063 6f6c 6f72  # generate color
-00000900: 6564 2074 6578 7420 7573 696e 6720 6874  ed text using ht
-00000910: 6d6c 0a61 7274 2e63 6f6c 6f72 6966 7928  ml.art.colorify(
-00000920: 290a 0a23 206f 7574 7075 7420 696e 746f  )..# output into
-00000930: 202e 6874 6d6c 2066 696c 650a 6172 742e   .html file.art.
-00000940: 636f 6c6f 725f 6f75 7470 7574 2822 6f75  color_output("ou
-00000950: 7470 7574 2229 0a60 6060 0a0a 5f46 6f72  tput").```.._For
-00000960: 2065 7861 6d70 6c65 7320 6672 6f6d 2075   examples from u
-00000970: 7365 7220 636f 6d6d 756e 6974 792c 2070  ser community, p
-00000980: 6c65 6173 6520 7265 6665 7220 746f 2074  lease refer to t
-00000990: 6865 205b 7072 696d 6570 6174 656c 2e67  he [primepatel.g
-000009a0: 6974 6875 622e 696f 2f61 6b73 6861 7269  ithub.io/akshari
-000009b0: 6679 5d28 6874 7470 733a 2f2f 7072 696d  fy](https://prim
-000009c0: 6570 6174 656c 2e67 6974 6875 622e 696f  epatel.github.io
-000009d0: 2f61 6b73 6861 7269 6679 295f 0a0a 0a3c  /aksharify)_...<
-000009e0: 212d 2d20 524f 4144 4d41 5020 2d2d 3e0a  !-- ROADMAP -->.
-000009f0: 2323 2052 6f61 646d 6170 0a0a 2d20 5b78  ## Roadmap..- [x
-00000a00: 5d20 4e75 6d62 6572 6946 790a 2d20 5b2d  ] NumberiFy.- [-
-00000a10: 5d20 5072 6564 6966 696e 6564 206f 7264  ] Predifined ord
-00000a20: 6572 206f 6620 6368 6172 6163 7465 7273  er of characters
-00000a30: 0a2d 205b 2d5d 2047 6574 7469 6e67 2069  .- [-] Getting i
-00000a40: 6d61 6765 7320 6672 6f6d 2055 524c 0a2d  mages from URL.-
-00000a50: 205b 2d5d 2045 6d6f 6a69 4679 0a0a 5365   [-] EmojiFy..Se
-00000a60: 6520 7468 6520 5b6f 7065 6e20 6973 7375  e the [open issu
-00000a70: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-00000a80: 7562 2e63 6f6d 2f67 6974 6875 625f 7573  ub.com/github_us
-00000a90: 6572 6e61 6d65 2f72 6570 6f5f 6e61 6d65  ername/repo_name
-00000aa0: 2f69 7373 7565 7329 2066 6f72 2061 2066  /issues) for a f
-00000ab0: 756c 6c20 6c69 7374 206f 6620 7072 6f70  ull list of prop
-00000ac0: 6f73 6564 2066 6561 7475 7265 7320 2861  osed features (a
-00000ad0: 6e64 206b 6e6f 776e 2069 7373 7565 7329  nd known issues)
-00000ae0: 2e0a 0a3c 212d 2d20 434f 4e54 5249 4255  ...<!-- CONTRIBU
-00000af0: 5449 4e47 202d 2d3e 0a23 2320 436f 6e74  TING -->.## Cont
-00000b00: 7269 6275 7469 6e67 0a0a 436f 6e74 7269  ributing..Contri
-00000b10: 6275 7469 6f6e 7320 6172 6520 7768 6174  butions are what
-00000b20: 206d 616b 6520 7468 6520 6f70 656e 2073   make the open s
-00000b30: 6f75 7263 6520 636f 6d6d 756e 6974 7920  ource community 
-00000b40: 7375 6368 2061 2077 6f6e 6465 7266 756c  such a wonderful
-00000b50: 2070 6c61 6365 2074 6f20 6c65 6172 6e2c   place to learn,
-00000b60: 2062 6520 696e 7370 6972 6564 2c20 616e   be inspired, an
-00000b70: 6420 6372 6561 7465 2e20 416e 7920 636f  d create. Any co
-00000b80: 6e74 7269 6275 7469 6f6e 7320 796f 7520  ntributions you 
-00000b90: 6d61 6b65 2061 7265 2060 6170 7072 6563  make are `apprec
-00000ba0: 6961 7465 6420 6772 6561 746c 7960 2e0a  iated greatly`..
-00000bb0: 0a49 6620 796f 7520 6861 7665 2061 2073  .If you have a s
-00000bc0: 7567 6765 7374 696f 6e20 7468 6174 2077  uggestion that w
-00000bd0: 6f75 6c64 206d 616b 6520 7468 6973 2062  ould make this b
-00000be0: 6574 7465 722c 2070 6c65 6173 6520 666f  etter, please fo
-00000bf0: 726b 2074 6865 2072 6570 6f20 616e 6420  rk the repo and 
-00000c00: 6372 6561 7465 2061 2070 756c 6c20 7265  create a pull re
-00000c10: 7175 6573 742e 2059 6f75 2063 616e 2061  quest. You can a
-00000c20: 6c73 6f20 7369 6d70 6c79 206f 7065 6e20  lso simply open 
-00000c30: 616e 2069 7373 7565 2077 6974 6820 7468  an issue with th
-00000c40: 6520 7461 6720 2265 6e68 616e 6365 6d65  e tag "enhanceme
-00000c50: 6e74 222e 0a44 6f6e 2774 2066 6f72 6765  nt"..Don't forge
-00000c60: 7420 746f 2067 6976 6520 7468 6520 7072  t to give the pr
-00000c70: 6f6a 6563 7420 6120 7374 6172 2120 5468  oject a star! Th
-00000c80: 616e 6b73 2061 6761 696e 210a 0a31 2e20  anks again!..1. 
-00000c90: 466f 726b 2074 6865 2050 726f 6a65 6374  Fork the Project
-00000ca0: 0a32 2e20 4372 6561 7465 2079 6f75 7220  .2. Create your 
-00000cb0: 4665 6174 7572 6520 4272 616e 6368 2028  Feature Branch (
-00000cc0: 6067 6974 2063 6865 636b 6f75 7420 2d62  `git checkout -b
-00000cd0: 2066 6561 7475 7265 2f41 6d61 7a69 6e67   feature/Amazing
-00000ce0: 4665 6174 7572 6560 290a 332e 2043 6f6d  Feature`).3. Com
-00000cf0: 6d69 7420 796f 7572 2043 6861 6e67 6573  mit your Changes
-00000d00: 2028 6067 6974 2063 6f6d 6d69 7420 2d6d   (`git commit -m
-00000d10: 2027 4164 6420 736f 6d65 2041 6d61 7a69   'Add some Amazi
-00000d20: 6e67 4665 6174 7572 6527 6029 0a34 2e20  ngFeature'`).4. 
-00000d30: 5075 7368 2074 6f20 7468 6520 4272 616e  Push to the Bran
-00000d40: 6368 2028 6067 6974 2070 7573 6820 6f72  ch (`git push or
-00000d50: 6967 696e 2066 6561 7475 7265 2f41 6d61  igin feature/Ama
-00000d60: 7a69 6e67 4665 6174 7572 6560 290a 352e  zingFeature`).5.
-00000d70: 204f 7065 6e20 6120 5075 6c6c 2052 6571   Open a Pull Req
-00000d80: 7565 7374 0a0a 3c21 2d2d 204c 4943 454e  uest..<!-- LICEN
-00000d90: 5345 202d 2d3e 0a23 2320 4c69 6365 6e73  SE -->.## Licens
-00000da0: 650a 0a44 6973 7472 6962 7574 6564 2075  e..Distributed u
-00000db0: 6e64 6572 2074 6865 204d 4954 204c 6963  nder the MIT Lic
-00000dc0: 656e 7365 2e20 5365 6520 604c 4943 454e  ense. See `LICEN
-00000dd0: 5345 2e74 7874 6020 666f 7220 6d6f 7265  SE.txt` for more
-00000de0: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 0a3c   information...<
-00000df0: 212d 2d20 434f 4e54 4143 5420 2d2d 3e0a  !-- CONTACT -->.
-00000e00: 2323 2043 6f6e 7461 6374 0a0a 5072 696d  ## Contact..Prim
-00000e10: 6520 5061 7465 6c20 2d20 5b40 7072 696d  e Patel - [@prim
-00000e20: 6570 6174 656c 5d28 6874 7470 733a 2f2f  epatel](https://
-00000e30: 7477 6974 7465 722e 636f 6d2f 7072 696d  twitter.com/prim
-00000e40: 6573 7061 7465 6c29 202d 2070 7269 6d65  espatel) - prime
-00000e50: 7370 6174 656c 4067 6d61 696c 2e63 6f6d  spatel@gmail.com
-00000e60: 0a0a 5072 6f6a 6563 7420 4c69 6e6b 3a20  ..Project Link: 
-00000e70: 5b68 7474 7073 3a2f 2f67 6974 6875 622e  [https://github.
-00000e80: 636f 6d2f 7072 696d 6570 6174 656c 2f61  com/primepatel/a
-00000e90: 6b73 6861 7269 6679 5d28 6874 7470 733a  ksharify](https:
-00000ea0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7269  //github.com/pri
-00000eb0: 6d65 7061 7465 6c2f 616b 7368 6172 6966  mepatel/aksharif
-00000ec0: 7929 0a0a 0a3c 212d 2d20 4143 4b4e 4f57  y)...<!-- ACKNOW
-00000ed0: 4c45 4447 4d45 4e54 5320 2d2d 3e0a 3c21  LEDGMENTS -->.<!
-00000ee0: 2d2d 2023 2320 4163 6b6e 6f77 6c65 6467  -- ## Acknowledg
-00000ef0: 6d65 6e74 730a 0a2a 205b 5d28 290a 2a20  ments..* []().* 
-00000f00: 5b5d 2829 0a2a 205b 5d28 2920 2d2d 3e0a  []().* []() -->.
-00000f10: 0a3c 7020 616c 6967 6e3d 2272 6967 6874  .<p align="right
-00000f20: 223e 283c 6120 6872 6566 3d22 2372 6561  ">(<a href="#rea
-00000f30: 646d 652d 746f 7022 3e62 6163 6b20 746f  dme-top">back to
-00000f40: 2074 6f70 3c2f 613e 293c 2f70 3e0a 0a0a   top</a>)</p>...
-00000f50: 0a3c 212d 2d20 4d41 524b 444f 574e 204c  .<!-- MARKDOWN L
-00000f60: 494e 4b53 2026 2049 4d41 4745 5320 2d2d  INKS & IMAGES --
-00000f70: 3e0a 3c21 2d2d 2068 7474 7073 3a2f 2f77  >.<!-- https://w
-00000f80: 7777 2e6d 6172 6b64 6f77 6e67 7569 6465  ww.markdownguide
-00000f90: 2e6f 7267 2f62 6173 6963 2d73 796e 7461  .org/basic-synta
-00000fa0: 782f 2372 6566 6572 656e 6365 2d73 7479  x/#reference-sty
-00000fb0: 6c65 2d6c 696e 6b73 202d 2d3e 0a5b 636f  le-links -->.[co
-00000fc0: 6e74 7269 6275 746f 7273 2d73 6869 656c  ntributors-shiel
-00000fd0: 645d 3a20 6874 7470 733a 2f2f 696d 672e  d]: https://img.
-00000fe0: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00000ff0: 622f 636f 6e74 7269 6275 746f 7273 2f70  b/contributors/p
-00001000: 7269 6d65 7061 7465 6c2f 416b 7368 6172  rimepatel/Akshar
-00001010: 6966 792e 7376 673f 7374 796c 653d 666f  ify.svg?style=fo
-00001020: 722d 7468 652d 6261 6467 650a 5b63 6f6e  r-the-badge.[con
-00001030: 7472 6962 7574 6f72 732d 7572 6c5d 3a20  tributors-url]: 
-00001040: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001050: 6f6d 2f70 7269 6d65 7061 7465 6c2f 416b  om/primepatel/Ak
-00001060: 7368 6172 6966 792f 6772 6170 6873 2f63  sharify/graphs/c
-00001070: 6f6e 7472 6962 7574 6f72 730a 5b66 6f72  ontributors.[for
-00001080: 6b73 2d73 6869 656c 645d 3a20 6874 7470  ks-shield]: http
-00001090: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000010a0: 696f 2f67 6974 6875 622f 666f 726b 732f  io/github/forks/
-000010b0: 7072 696d 6570 6174 656c 2f41 6b73 6861  primepatel/Aksha
-000010c0: 7269 6679 2e73 7667 3f73 7479 6c65 3d66  rify.svg?style=f
-000010d0: 6f72 2d74 6865 2d62 6164 6765 0a5b 666f  or-the-badge.[fo
-000010e0: 726b 732d 7572 6c5d 3a20 6874 7470 733a  rks-url]: https:
-000010f0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7269  //github.com/pri
-00001100: 6d65 7061 7465 6c2f 416b 7368 6172 6966  mepatel/Aksharif
-00001110: 792f 6e65 7477 6f72 6b2f 6d65 6d62 6572  y/network/member
-00001120: 730a 5b73 7461 7273 2d73 6869 656c 645d  s.[stars-shield]
-00001130: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00001140: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00001150: 7374 6172 732f 7072 696d 6570 6174 656c  stars/primepatel
-00001160: 2f41 6b73 6861 7269 6679 2e73 7667 3f73  /Aksharify.svg?s
-00001170: 7479 6c65 3d66 6f72 2d74 6865 2d62 6164  tyle=for-the-bad
-00001180: 6765 0a5b 7374 6172 732d 7572 6c5d 3a20  ge.[stars-url]: 
-00001190: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000011a0: 6f6d 2f70 7269 6d65 7061 7465 6c2f 416b  om/primepatel/Ak
-000011b0: 7368 6172 6966 792f 7374 6172 6761 7a65  sharify/stargaze
-000011c0: 7273 0a5b 6973 7375 6573 2d73 6869 656c  rs.[issues-shiel
-000011d0: 645d 3a20 6874 7470 733a 2f2f 696d 672e  d]: https://img.
-000011e0: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-000011f0: 622f 6973 7375 6573 2f70 7269 6d65 7061  b/issues/primepa
-00001200: 7465 6c2f 416b 7368 6172 6966 792e 7376  tel/Aksharify.sv
-00001210: 673f 7374 796c 653d 666f 722d 7468 652d  g?style=for-the-
-00001220: 6261 6467 650a 5b69 7373 7565 732d 7572  badge.[issues-ur
-00001230: 6c5d 3a20 6874 7470 733a 2f2f 6769 7468  l]: https://gith
-00001240: 7562 2e63 6f6d 2f70 7269 6d65 7061 7465  ub.com/primepate
-00001250: 6c2f 416b 7368 6172 6966 792f 6973 7375  l/Aksharify/issu
-00001260: 6573 0a5b 6c69 6365 6e73 652d 7368 6965  es.[license-shie
-00001270: 6c64 5d3a 2068 7474 7073 3a2f 2f69 6d67  ld]: https://img
-00001280: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-00001290: 7562 2f6c 6963 656e 7365 2f70 7269 6d65  ub/license/prime
-000012a0: 7061 7465 6c2f 416b 7368 6172 6966 792e  patel/Aksharify.
-000012b0: 7376 673f 7374 796c 653d 666f 722d 7468  svg?style=for-th
-000012c0: 652d 6261 6467 650a 5b6c 6963 656e 7365  e-badge.[license
-000012d0: 2d75 726c 5d3a 2068 7474 7073 3a2f 2f67  -url]: https://g
-000012e0: 6974 6875 622e 636f 6d2f 7072 696d 6570  ithub.com/primep
-000012f0: 6174 656c 2f41 6b73 6861 7269 6679 2f62  atel/Aksharify/b
-00001300: 6c6f 622f 6d61 7374 6572 2f4c 4943 454e  lob/master/LICEN
-00001310: 5345 2e74 7874 0a5b 6c69 6e6b 6564 696e  SE.txt.[linkedin
-00001320: 2d73 6869 656c 645d 3a20 6874 7470 733a  -shield]: https:
-00001330: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00001340: 2f62 6164 6765 2f2d 4c69 6e6b 6564 496e  /badge/-LinkedIn
-00001350: 2d62 6c61 636b 2e73 7667 3f73 7479 6c65  -black.svg?style
-00001360: 3d66 6f72 2d74 6865 2d62 6164 6765 266c  =for-the-badge&l
-00001370: 6f67 6f3d 6c69 6e6b 6564 696e 2663 6f6c  ogo=linkedin&col
-00001380: 6f72 423d 3535 350a 5b6c 696e 6b65 6469  orB=555.[linkedi
-00001390: 6e2d 7572 6c5d 3a20 6874 7470 733a 2f2f  n-url]: https://
-000013a0: 6c69 6e6b 6564 696e 2e63 6f6d 2f69 6e2f  linkedin.com/in/
-000013b0: 7072 696d 6570 6174 656c 0a5b 446f 776e  primepatel.[Down
-000013c0: 6c6f 6164 732d 7368 6965 6c64 5d3a 2068  loads-shield]: h
-000013d0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000013e0: 6473 2e69 6f2f 7079 7069 2f64 6d2f 616b  ds.io/pypi/dm/ak
-000013f0: 7368 6172 6966 793f 7374 796c 653d 666f  sharify?style=fo
-00001400: 722d 7468 652d 6261 6467 650a            r-the-badge.
+00000500: 6966 7929 0a0a 3c62 7220 2f3e 0a0a 2323  ify)..<br />..##
+00000510: 2041 626f 7574 2054 6865 204d 6f64 756c   About The Modul
+00000520: 650a 0a41 6b73 6861 7269 6679 2069 7320  e..Aksharify is 
+00000530: 616e 206f 7065 6e2d 736f 7572 6365 2070  an open-source p
+00000540: 7974 686f 6e20 7061 636b 6167 6520 686f  ython package ho
+00000550: 7374 6564 206f 6e20 4769 7448 7562 2074  sted on GitHub t
+00000560: 6861 7420 616c 6c6f 7773 2079 6f75 2074  hat allows you t
+00000570: 6f20 6566 666f 7274 6c65 7373 6c79 2074  o effortlessly t
+00000580: 7261 6e73 666f 726d 2069 6d61 6765 7320  ransform images 
+00000590: 696e 746f 2063 6170 7469 7661 7469 6e67  into captivating
+000005a0: 2041 5343 4949 2061 7274 2072 6570 7265   ASCII art repre
+000005b0: 7365 6e74 6174 696f 6e73 2e20 5769 7468  sentations. With
+000005c0: 2041 6b73 6861 7269 6679 2c20 796f 7520   Aksharify, you 
+000005d0: 6361 6e20 636f 6e76 6572 7420 796f 7572  can convert your
+000005e0: 2066 6176 6f72 6974 6520 696d 6167 6573   favorite images
+000005f0: 2069 6e74 6f20 616e 2061 7274 6973 7469   into an artisti
+00000600: 6320 6172 7261 6e67 656d 656e 7420 6f66  c arrangement of
+00000610: 2041 5343 4949 2063 6861 7261 6374 6572   ASCII character
+00000620: 732c 2061 6464 696e 6720 6120 756e 6971  s, adding a uniq
+00000630: 7565 2061 6e64 206e 6f73 7461 6c67 6963  ue and nostalgic
+00000640: 2074 6f75 6368 2074 6f20 796f 7572 2070   touch to your p
+00000650: 726f 6a65 6374 732e 0a0a 5374 6172 7420  rojects...Start 
+00000660: 7472 616e 7366 6f72 6d69 6e67 2079 6f75  transforming you
+00000670: 7220 7068 6f74 6f73 2069 6e74 6f20 6361  r photos into ca
+00000680: 7074 6976 6174 696e 6720 4153 4349 4920  ptivating ASCII 
+00000690: 6172 7420 7769 7468 2041 6b73 6861 7269  art with Akshari
+000006a0: 6679 2061 6e64 2075 6e6c 6561 7368 2079  fy and unleash y
+000006b0: 6f75 7220 6372 6561 7469 7669 7479 2069  our creativity i
+000006c0: 6e20 7468 6520 776f 726c 6420 6f66 2076  n the world of v
+000006d0: 6973 7561 6c20 7265 7072 6573 656e 7461  isual representa
+000006e0: 7469 6f6e 210a 2323 204b 6579 2046 6561  tion!.## Key Fea
+000006f0: 7475 7265 730a 0a2d 2043 6f6e 7665 7274  tures..- Convert
+00000700: 2070 686f 746f 7320 616e 6420 696d 6167   photos and imag
+00000710: 6573 2069 6e74 6f20 4153 4349 4920 6172  es into ASCII ar
+00000720: 7420 7769 7468 2061 2073 696e 676c 6520  t with a single 
+00000730: 6675 6e63 7469 6f6e 2063 616c 6c2e 0a0a  function call...
+00000740: 2d20 4669 6e65 2d74 756e 6520 7468 6520  - Fine-tune the 
+00000750: 6f75 7470 7574 2062 7920 6164 6a75 7374  output by adjust
+00000760: 696e 6720 7061 7261 6d65 7465 7273 2073  ing parameters s
+00000770: 7563 6820 6173 2063 6861 7261 6374 6572  uch as character
+00000780: 2073 6574 2c20 7265 736f 6c75 7469 6f6e   set, resolution
+00000790: 2065 7463 2e0a 0a2d 2053 7570 706f 7274   etc...- Support
+000007a0: 2066 6f72 2076 6172 696f 7573 2063 6861   for various cha
+000007b0: 7261 6374 6572 2073 6574 732c 2061 6c6c  racter sets, all
+000007c0: 6f77 696e 6720 796f 7520 746f 2063 7573  owing you to cus
+000007d0: 746f 6d69 7a65 2074 6865 2073 7479 6c65  tomize the style
+000007e0: 206f 6620 7468 6520 6765 6e65 7261 7465   of the generate
+000007f0: 6420 4153 4349 4920 6172 742e 0a0a 2d20  d ASCII art...- 
+00000800: 4578 706f 7274 2074 6865 2041 5343 4949  Export the ASCII
+00000810: 2061 7274 2061 7320 706c 6169 6e20 7465   art as plain te
+00000820: 7874 206f 7220 7361 7665 2069 7420 6173  xt or save it as
+00000830: 2061 6e20 696d 6167 6520 6669 6c65 2066   an image file f
+00000840: 6f72 2065 6173 7920 7368 6172 696e 6720  or easy sharing 
+00000850: 616e 6420 696e 7465 6772 6174 696f 6e2e  and integration.
+00000860: 0a0a 2323 2057 6861 7420 6973 2041 7363  ..## What is Asc
+00000870: 6969 4172 740a 0a41 5343 4949 2061 7274  iiArt..ASCII art
+00000880: 2069 7320 6120 7374 796c 6520 6f66 2061   is a style of a
+00000890: 7274 2069 6e20 7768 6963 6820 7065 6f70  rt in which peop
+000008a0: 6c65 206d 616b 6520 6772 6170 6869 6373  le make graphics
+000008b0: 2061 6e64 2064 6573 6967 6e73 2062 7920   and designs by 
+000008c0: 7573 696e 6720 6c65 7474 6572 732c 206e  using letters, n
+000008d0: 756d 6265 7273 2c20 616e 6420 7379 6d62  umbers, and symb
+000008e0: 6f6c 7320 6672 6f6d 2061 2075 6e69 7175  ols from a uniqu
+000008f0: 6520 7365 7420 6f66 2063 6861 7261 6374  e set of charact
+00000900: 6572 7320 6b6e 6f77 6e20 6173 2041 5343  ers known as ASC
+00000910: 4949 2e20 4153 4349 4920 7061 696e 7465  II. ASCII painte
+00000920: 7273 2063 7265 6174 6520 696e 7472 6967  rs create intrig
+00000930: 7569 6e67 2069 6d61 6765 7320 6279 2061  uing images by a
+00000940: 7272 616e 6769 6e67 2074 6865 7365 2063  rranging these c
+00000950: 6861 7261 6374 6572 7320 696e 2070 6174  haracters in pat
+00000960: 7465 726e 7320 616e 6420 666f 726d 7320  terns and forms 
+00000970: 7261 7468 6572 2074 6861 6e20 7573 696e  rather than usin
+00000980: 6720 636f 6c6f 7572 7320 616e 6420 6272  g colours and br
+00000990: 7573 6865 7320 6173 2069 6e20 7472 6164  ushes as in trad
+000009a0: 6974 696f 6e61 6c20 6172 742e 2054 6865  itional art. The
+000009b0: 7920 6d65 7469 6375 6c6f 7573 6c79 2073  y meticulously s
+000009c0: 656c 6563 7420 7468 6520 6170 7072 6f70  elect the approp
+000009d0: 7269 6174 6520 6368 6172 6163 7465 7273  riate characters
+000009e0: 2061 6e64 2063 6f6d 6269 6e65 2074 6865   and combine the
+000009f0: 6d20 746f 2070 726f 6475 6365 2069 6d61  m to produce ima
+00000a00: 6765 7320 6f66 2061 6e69 6d61 6c73 2c20  ges of animals, 
+00000a10: 7065 6f70 6c65 2c20 6f72 2065 7665 6e20  people, or even 
+00000a20: 6c61 6e64 7363 6170 6573 2e20 4974 2773  landscapes. It's
+00000a30: 2061 6c6d 6f73 7420 6173 2069 6620 796f   almost as if yo
+00000a40: 7527 7265 2073 6b65 7463 6869 6e67 2077  u're sketching w
+00000a50: 6974 6820 6c65 7474 6572 7320 616e 6420  ith letters and 
+00000a60: 7379 6d62 6f6c 7321 2041 5343 4949 2061  symbols! ASCII a
+00000a70: 7274 2069 7320 6120 6675 6e20 7761 7920  rt is a fun way 
+00000a80: 666f 7220 6172 7469 7374 7320 746f 2065  for artists to e
+00000a90: 7870 7265 7373 2074 6865 6d73 656c 7665  xpress themselve
+00000aa0: 7320 7573 696e 6720 6f6e 6c79 2074 6865  s using only the
+00000ab0: 2062 6173 6963 2063 6861 7261 6374 6572   basic character
+00000ac0: 7320 7072 6573 656e 7420 6f6e 2061 2063  s present on a c
+00000ad0: 6f6d 7075 7465 7220 6b65 7962 6f61 7264  omputer keyboard
+00000ae0: 2e0a 0a3c 212d 2d20 4142 4f55 5420 5448  ...<!-- ABOUT TH
+00000af0: 4520 5052 4f4a 4543 5420 2d2d 3e0a 2323  E PROJECT -->.##
+00000b00: 204d 6f74 6976 6174 696f 6e0a 0a54 6865   Motivation..The
+00000b10: 2069 6e73 7069 7261 7469 6f6e 2066 6f72   inspiration for
+00000b20: 2074 6869 7320 6d6f 6475 6c65 2063 616d   this module cam
+00000b30: 6520 6672 6f6d 2061 204e 756d 6265 7270  e from a Numberp
+00000b40: 6869 6c65 2076 6964 656f 2063 616c 6c65  hile video calle
+00000b50: 6420 2254 6865 2054 7269 6e69 7479 2048  d "The Trinity H
+00000b60: 616c 6c20 5072 696d 652c 2220 7768 6963  all Prime," whic
+00000b70: 6820 4920 6669 7273 7420 7361 7720 696e  h I first saw in
+00000b80: 2068 6967 6820 7363 686f 6f6c 2064 6179   high school day
+00000b90: 732e 2049 7420 6d6f 7469 7661 7465 6420  s. It motivated 
+00000ba0: 6d65 2074 6f20 6578 706c 6f72 6520 7468  me to explore th
+00000bb0: 6520 706f 7373 6962 696c 6974 6965 7320  e possibilities 
+00000bc0: 6f66 2073 7563 6820 6120 7072 696d 6520  of such a prime 
+00000bd0: 6e75 6d62 6572 2e20 4920 6372 6561 7465  number. I create
+00000be0: 6420 6120 5079 7468 6f6e 206d 6f64 756c  d a Python modul
+00000bf0: 6520 7468 6174 2075 7365 7320 6120 7072  e that uses a pr
+00000c00: 6564 6574 6572 6d69 6e65 6420 6368 6172  edetermined char
+00000c10: 6163 7465 7220 7365 7420 746f 2074 7572  acter set to tur
+00000c20: 6e20 7068 6f74 6f73 2069 6e74 6f20 4153  n photos into AS
+00000c30: 4349 4920 6172 742e 2049 7420 6d61 6e69  CII art. It mani
+00000c40: 7075 6c61 7465 7320 696d 6167 6573 2075  pulates images u
+00000c50: 7369 6e67 2074 6865 2050 494c 2070 6163  sing the PIL pac
+00000c60: 6b61 6765 2c20 7472 616e 7366 6f72 6d69  kage, transformi
+00000c70: 6e67 2074 6865 6d20 746f 2067 7261 7973  ng them to grays
+00000c80: 6361 6c65 2062 6566 6f72 6520 6d61 7070  cale before mapp
+00000c90: 696e 6720 7069 7865 6c20 7661 6c75 6573  ing pixel values
+00000ca0: 2074 6f20 4153 4349 4920 6c65 7474 6572   to ASCII letter
+00000cb0: 732e 2055 7365 7273 2063 616e 2063 6861  s. Users can cha
+00000cc0: 6e67 6520 7468 6520 6368 6172 6163 7465  nge the characte
+00000cd0: 7220 7365 7420 746f 2067 6574 2064 6966  r set to get dif
+00000ce0: 6665 7265 6e74 2065 6666 6563 7473 2e0a  ferent effects..
+00000cf0: 0a3c 212d 2d20 4745 5454 494e 4720 5354  .<!-- GETTING ST
+00000d00: 4152 5445 4420 2d2d 3e0a 2323 2047 6574  ARTED -->.## Get
+00000d10: 7469 6e67 2053 7461 7274 6564 0a0a 4265  ting Started..Be
+00000d20: 666f 7265 2077 6520 6265 6769 6e2c 206d  fore we begin, m
+00000d30: 616b 6520 7375 7265 2079 6f75 2068 6176  ake sure you hav
+00000d40: 6520 6f6e 6520 6f66 2072 6563 656e 7420  e one of recent 
+00000d50: 7665 7273 696f 6e73 206f 6620 5079 7468  versions of Pyth
+00000d60: 6f6e 2069 6e73 7461 6c6c 6564 206f 6e20  on installed on 
+00000d70: 796f 7572 2063 6f6d 7075 7465 722e 0a0a  your computer...
+00000d80: 2323 2320 496e 7374 616c 6c61 7469 6f6e  ### Installation
+00000d90: 0a0a 6060 6073 680a 7079 7468 6f6e 202d  ..```sh.python -
+00000da0: 6d20 7069 7020 696e 7374 616c 6c20 616b  m pip install ak
+00000db0: 7368 6172 6966 790a 6060 600a 0a23 2320  sharify.```..## 
+00000dc0: 5573 6167 650a 0a60 6060 7079 7468 6f6e  Usage..```python
+00000dd0: 0a66 726f 6d20 616b 7368 6172 6966 7920  .from aksharify 
+00000de0: 696d 706f 7274 2054 6578 7441 7274 0a0a  import TextArt..
+00000df0: 2320 696e 7075 7420 696d 6167 6520 6669  # input image fi
+00000e00: 6c65 0a61 7274 203d 2054 6578 7441 7274  le.art = TextArt
+00000e10: 2822 4a75 6c69 612e 706e 6722 290a 0a23  ("Julia.png")..#
+00000e20: 2073 6565 2069 6d61 6765 0a61 7274 2e69   see image.art.i
+00000e30: 6d61 6765 2e73 686f 7728 290a 0a23 2073  mage.show()..# s
+00000e40: 6574 2064 696d 656e 7369 6f6e 206f 6620  et dimension of 
+00000e50: 6f75 7470 7574 2074 6578 740a 6172 742e  output text.art.
+00000e60: 7365 745f 6469 6d28 3830 290a 0a23 2067  set_dim(80)..# g
+00000e70: 656e 6574 6174 6520 7465 7874 0a61 7274  enetate text.art
+00000e80: 2e61 7363 6969 6679 2829 0a0a 2320 6f75  .asciify()..# ou
+00000e90: 7470 7574 2069 6e74 6f20 2e74 7874 2066  tput into .txt f
+00000ea0: 696c 650a 6172 742e 7465 7874 5f6f 7574  ile.art.text_out
+00000eb0: 7075 7428 226f 7574 7075 7422 290a 0a23  put("output")..#
+00000ec0: 2067 656e 6572 6174 6520 636f 6c6f 7265   generate colore
+00000ed0: 6420 7465 7874 2075 7369 6e67 2068 746d  d text using htm
+00000ee0: 6c0a 6172 742e 636f 6c6f 7269 6679 2829  l.art.colorify()
+00000ef0: 0a0a 2320 6f75 7470 7574 2069 6e74 6f20  ..# output into 
+00000f00: 2e68 746d 6c20 6669 6c65 0a61 7274 2e63  .html file.art.c
+00000f10: 6f6c 6f72 5f6f 7574 7075 7428 226f 7574  olor_output("out
+00000f20: 7075 7422 290a 6060 600a 0a5f 466f 7220  put").```.._For 
+00000f30: 6578 616d 706c 6573 2066 726f 6d20 7573  examples from us
+00000f40: 6572 2063 6f6d 6d75 6e69 7479 2c20 706c  er community, pl
+00000f50: 6561 7365 2072 6566 6572 2074 6f20 7468  ease refer to th
+00000f60: 6520 5b70 7269 6d65 7061 7465 6c2e 6769  e [primepatel.gi
+00000f70: 7468 7562 2e69 6f2f 616b 7368 6172 6966  thub.io/aksharif
+00000f80: 795d 2868 7474 7073 3a2f 2f70 7269 6d65  y](https://prime
+00000f90: 7061 7465 6c2e 6769 7468 7562 2e69 6f2f  patel.github.io/
+00000fa0: 616b 7368 6172 6966 7929 5f0a 0a0a 3c21  aksharify)_...<!
+00000fb0: 2d2d 2052 4f41 444d 4150 202d 2d3e 0a23  -- ROADMAP -->.#
+00000fc0: 2320 526f 6164 6d61 700a 0a2d 205b 785d  # Roadmap..- [x]
+00000fd0: 204e 756d 6265 7269 4679 0a2d 205b 2d5d   NumberiFy.- [-]
+00000fe0: 2050 7265 6469 6669 6e65 6420 6f72 6465   Predifined orde
+00000ff0: 7220 6f66 2063 6861 7261 6374 6572 730a  r of characters.
+00001000: 2d20 5b2d 5d20 4765 7474 696e 6720 696d  - [-] Getting im
+00001010: 6167 6573 2066 726f 6d20 5552 4c0a 2d20  ages from URL.- 
+00001020: 5b2d 5d20 456d 6f6a 6946 790a 0a53 6565  [-] EmojiFy..See
+00001030: 2074 6865 205b 6f70 656e 2069 7373 7565   the [open issue
+00001040: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00001050: 622e 636f 6d2f 6769 7468 7562 5f75 7365  b.com/github_use
+00001060: 726e 616d 652f 7265 706f 5f6e 616d 652f  rname/repo_name/
+00001070: 6973 7375 6573 2920 666f 7220 6120 6675  issues) for a fu
+00001080: 6c6c 206c 6973 7420 6f66 2070 726f 706f  ll list of propo
+00001090: 7365 6420 6665 6174 7572 6573 2028 616e  sed features (an
+000010a0: 6420 6b6e 6f77 6e20 6973 7375 6573 292e  d known issues).
+000010b0: 0a0a 3c21 2d2d 2043 4f4e 5452 4942 5554  ..<!-- CONTRIBUT
+000010c0: 494e 4720 2d2d 3e0a 2323 2043 6f6e 7472  ING -->.## Contr
+000010d0: 6962 7574 696e 670a 0a43 6f6e 7472 6962  ibuting..Contrib
+000010e0: 7574 696f 6e73 2061 7265 2077 6861 7420  utions are what 
+000010f0: 6d61 6b65 2074 6865 206f 7065 6e20 736f  make the open so
+00001100: 7572 6365 2063 6f6d 6d75 6e69 7479 2073  urce community s
+00001110: 7563 6820 6120 776f 6e64 6572 6675 6c20  uch a wonderful 
+00001120: 706c 6163 6520 746f 206c 6561 726e 2c20  place to learn, 
+00001130: 6265 2069 6e73 7069 7265 642c 2061 6e64  be inspired, and
+00001140: 2063 7265 6174 652e 2041 6e79 2063 6f6e   create. Any con
+00001150: 7472 6962 7574 696f 6e73 2079 6f75 206d  tributions you m
+00001160: 616b 6520 6172 6520 6061 7070 7265 6369  ake are `appreci
+00001170: 6174 6564 2067 7265 6174 6c79 602e 0a0a  ated greatly`...
+00001180: 4966 2079 6f75 2068 6176 6520 6120 7375  If you have a su
+00001190: 6767 6573 7469 6f6e 2074 6861 7420 776f  ggestion that wo
+000011a0: 756c 6420 6d61 6b65 2074 6869 7320 6265  uld make this be
+000011b0: 7474 6572 2c20 706c 6561 7365 2066 6f72  tter, please for
+000011c0: 6b20 7468 6520 7265 706f 2061 6e64 2063  k the repo and c
+000011d0: 7265 6174 6520 6120 7075 6c6c 2072 6571  reate a pull req
+000011e0: 7565 7374 2e20 596f 7520 6361 6e20 616c  uest. You can al
+000011f0: 736f 2073 696d 706c 7920 6f70 656e 2061  so simply open a
+00001200: 6e20 6973 7375 6520 7769 7468 2074 6865  n issue with the
+00001210: 2074 6167 2022 656e 6861 6e63 656d 656e   tag "enhancemen
+00001220: 7422 2e0a 446f 6e27 7420 666f 7267 6574  t"..Don't forget
+00001230: 2074 6f20 6769 7665 2074 6865 2070 726f   to give the pro
+00001240: 6a65 6374 2061 2073 7461 7221 2054 6861  ject a star! Tha
+00001250: 6e6b 7320 6167 6169 6e21 0a0a 312e 2046  nks again!..1. F
+00001260: 6f72 6b20 7468 6520 5072 6f6a 6563 740a  ork the Project.
+00001270: 322e 2043 7265 6174 6520 796f 7572 2046  2. Create your F
+00001280: 6561 7475 7265 2042 7261 6e63 6820 2860  eature Branch (`
+00001290: 6769 7420 6368 6563 6b6f 7574 202d 6220  git checkout -b 
+000012a0: 6665 6174 7572 652f 416d 617a 696e 6746  feature/AmazingF
+000012b0: 6561 7475 7265 6029 0a33 2e20 436f 6d6d  eature`).3. Comm
+000012c0: 6974 2079 6f75 7220 4368 616e 6765 7320  it your Changes 
+000012d0: 2860 6769 7420 636f 6d6d 6974 202d 6d20  (`git commit -m 
+000012e0: 2741 6464 2073 6f6d 6520 416d 617a 696e  'Add some Amazin
+000012f0: 6746 6561 7475 7265 2760 290a 342e 2050  gFeature'`).4. P
+00001300: 7573 6820 746f 2074 6865 2042 7261 6e63  ush to the Branc
+00001310: 6820 2860 6769 7420 7075 7368 206f 7269  h (`git push ori
+00001320: 6769 6e20 6665 6174 7572 652f 416d 617a  gin feature/Amaz
+00001330: 696e 6746 6561 7475 7265 6029 0a35 2e20  ingFeature`).5. 
+00001340: 4f70 656e 2061 2050 756c 6c20 5265 7175  Open a Pull Requ
+00001350: 6573 740a 0a3c 212d 2d20 4c49 4345 4e53  est..<!-- LICENS
+00001360: 4520 2d2d 3e0a 2323 204c 6963 656e 7365  E -->.## License
+00001370: 0a0a 4469 7374 7269 6275 7465 6420 756e  ..Distributed un
+00001380: 6465 7220 7468 6520 4d49 5420 4c69 6365  der the MIT Lice
+00001390: 6e73 652e 2053 6565 2060 4c49 4345 4e53  nse. See `LICENS
+000013a0: 452e 7478 7460 2066 6f72 206d 6f72 6520  E.txt` for more 
+000013b0: 696e 666f 726d 6174 696f 6e2e 0a0a 3c21  information...<!
+000013c0: 2d2d 2043 4f4e 5441 4354 202d 2d3e 0a23  -- CONTACT -->.#
+000013d0: 2320 436f 6e74 6163 740a 0a50 7269 6d65  # Contact..Prime
+000013e0: 2050 6174 656c 202d 205b 4070 7269 6d65   Patel - [@prime
+000013f0: 7061 7465 6c5d 2868 7474 7073 3a2f 2f74  patel](https://t
+00001400: 7769 7474 6572 2e63 6f6d 2f70 7269 6d65  witter.com/prime
+00001410: 7370 6174 656c 2920 2d20 7072 696d 6573  spatel) - primes
+00001420: 7061 7465 6c40 676d 6169 6c2e 636f 6d0a  patel@gmail.com.
+00001430: 0a50 726f 6a65 6374 204c 696e 6b3a 205b  .Project Link: [
+00001440: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001450: 6f6d 2f70 7269 6d65 7061 7465 6c2f 616b  om/primepatel/ak
+00001460: 7368 6172 6966 795d 2868 7474 7073 3a2f  sharify](https:/
+00001470: 2f67 6974 6875 622e 636f 6d2f 7072 696d  /github.com/prim
+00001480: 6570 6174 656c 2f61 6b73 6861 7269 6679  epatel/aksharify
+00001490: 290a 0a0a 3c21 2d2d 2041 434b 4e4f 574c  )...<!-- ACKNOWL
+000014a0: 4544 474d 454e 5453 202d 2d3e 0a3c 212d  EDGMENTS -->.<!-
+000014b0: 2d20 2323 2041 636b 6e6f 776c 6564 676d  - ## Acknowledgm
+000014c0: 656e 7473 0a0a 2a20 5b5d 2829 0a2a 205b  ents..* []().* [
+000014d0: 5d28 290a 2a20 5b5d 2829 202d 2d3e 0a0a  ]().* []() -->..
+000014e0: 3c70 2061 6c69 676e 3d22 7269 6768 7422  <p align="right"
+000014f0: 3e28 3c61 2068 7265 663d 2223 7265 6164  >(<a href="#read
+00001500: 6d65 2d74 6f70 223e 6261 636b 2074 6f20  me-top">back to 
+00001510: 746f 703c 2f61 3e29 3c2f 703e 0a0a 0a0a  top</a>)</p>....
+00001520: 3c21 2d2d 204d 4152 4b44 4f57 4e20 4c49  <!-- MARKDOWN LI
+00001530: 4e4b 5320 2620 494d 4147 4553 202d 2d3e  NKS & IMAGES -->
+00001540: 0a3c 212d 2d20 6874 7470 733a 2f2f 7777  .<!-- https://ww
+00001550: 772e 6d61 726b 646f 776e 6775 6964 652e  w.markdownguide.
+00001560: 6f72 672f 6261 7369 632d 7379 6e74 6178  org/basic-syntax
+00001570: 2f23 7265 6665 7265 6e63 652d 7374 796c  /#reference-styl
+00001580: 652d 6c69 6e6b 7320 2d2d 3e0a 5b63 6f6e  e-links -->.[con
+00001590: 7472 6962 7574 6f72 732d 7368 6965 6c64  tributors-shield
+000015a0: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
+000015b0: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+000015c0: 2f63 6f6e 7472 6962 7574 6f72 732f 7072  /contributors/pr
+000015d0: 696d 6570 6174 656c 2f41 6b73 6861 7269  imepatel/Akshari
+000015e0: 6679 2e73 7667 3f73 7479 6c65 3d66 6f72  fy.svg?style=for
+000015f0: 2d74 6865 2d62 6164 6765 0a5b 636f 6e74  -the-badge.[cont
+00001600: 7269 6275 746f 7273 2d75 726c 5d3a 2068  ributors-url]: h
+00001610: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001620: 6d2f 7072 696d 6570 6174 656c 2f41 6b73  m/primepatel/Aks
+00001630: 6861 7269 6679 2f67 7261 7068 732f 636f  harify/graphs/co
+00001640: 6e74 7269 6275 746f 7273 0a5b 666f 726b  ntributors.[fork
+00001650: 732d 7368 6965 6c64 5d3a 2068 7474 7073  s-shield]: https
+00001660: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00001670: 6f2f 6769 7468 7562 2f66 6f72 6b73 2f70  o/github/forks/p
+00001680: 7269 6d65 7061 7465 6c2f 416b 7368 6172  rimepatel/Akshar
+00001690: 6966 792e 7376 673f 7374 796c 653d 666f  ify.svg?style=fo
+000016a0: 722d 7468 652d 6261 6467 650a 5b66 6f72  r-the-badge.[for
+000016b0: 6b73 2d75 726c 5d3a 2068 7474 7073 3a2f  ks-url]: https:/
+000016c0: 2f67 6974 6875 622e 636f 6d2f 7072 696d  /github.com/prim
+000016d0: 6570 6174 656c 2f41 6b73 6861 7269 6679  epatel/Aksharify
+000016e0: 2f6e 6574 776f 726b 2f6d 656d 6265 7273  /network/members
+000016f0: 0a5b 7374 6172 732d 7368 6965 6c64 5d3a  .[stars-shield]:
+00001700: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
+00001710: 656c 6473 2e69 6f2f 6769 7468 7562 2f73  elds.io/github/s
+00001720: 7461 7273 2f70 7269 6d65 7061 7465 6c2f  tars/primepatel/
+00001730: 416b 7368 6172 6966 792e 7376 673f 7374  Aksharify.svg?st
+00001740: 796c 653d 666f 722d 7468 652d 6261 6467  yle=for-the-badg
+00001750: 650a 5b73 7461 7273 2d75 726c 5d3a 2068  e.[stars-url]: h
+00001760: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001770: 6d2f 7072 696d 6570 6174 656c 2f41 6b73  m/primepatel/Aks
+00001780: 6861 7269 6679 2f73 7461 7267 617a 6572  harify/stargazer
+00001790: 730a 5b69 7373 7565 732d 7368 6965 6c64  s.[issues-shield
+000017a0: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
+000017b0: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+000017c0: 2f69 7373 7565 732f 7072 696d 6570 6174  /issues/primepat
+000017d0: 656c 2f41 6b73 6861 7269 6679 2e73 7667  el/Aksharify.svg
+000017e0: 3f73 7479 6c65 3d66 6f72 2d74 6865 2d62  ?style=for-the-b
+000017f0: 6164 6765 0a5b 6973 7375 6573 2d75 726c  adge.[issues-url
+00001800: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
+00001810: 622e 636f 6d2f 7072 696d 6570 6174 656c  b.com/primepatel
+00001820: 2f41 6b73 6861 7269 6679 2f69 7373 7565  /Aksharify/issue
+00001830: 730a 5b6c 6963 656e 7365 2d73 6869 656c  s.[license-shiel
+00001840: 645d 3a20 6874 7470 733a 2f2f 696d 672e  d]: https://img.
+00001850: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+00001860: 622f 6c69 6365 6e73 652f 7072 696d 6570  b/license/primep
+00001870: 6174 656c 2f41 6b73 6861 7269 6679 2e73  atel/Aksharify.s
+00001880: 7667 3f73 7479 6c65 3d66 6f72 2d74 6865  vg?style=for-the
+00001890: 2d62 6164 6765 0a5b 6c69 6365 6e73 652d  -badge.[license-
+000018a0: 7572 6c5d 3a20 6874 7470 733a 2f2f 6769  url]: https://gi
+000018b0: 7468 7562 2e63 6f6d 2f70 7269 6d65 7061  thub.com/primepa
+000018c0: 7465 6c2f 416b 7368 6172 6966 792f 626c  tel/Aksharify/bl
+000018d0: 6f62 2f6d 6173 7465 722f 4c49 4345 4e53  ob/master/LICENS
+000018e0: 452e 7478 740a 5b6c 696e 6b65 6469 6e2d  E.txt.[linkedin-
+000018f0: 7368 6965 6c64 5d3a 2068 7474 7073 3a2f  shield]: https:/
+00001900: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00001910: 6261 6467 652f 2d4c 696e 6b65 6449 6e2d  badge/-LinkedIn-
+00001920: 626c 6163 6b2e 7376 673f 7374 796c 653d  black.svg?style=
+00001930: 666f 722d 7468 652d 6261 6467 6526 6c6f  for-the-badge&lo
+00001940: 676f 3d6c 696e 6b65 6469 6e26 636f 6c6f  go=linkedin&colo
+00001950: 7242 3d35 3535 0a5b 6c69 6e6b 6564 696e  rB=555.[linkedin
+00001960: 2d75 726c 5d3a 2068 7474 7073 3a2f 2f6c  -url]: https://l
+00001970: 696e 6b65 6469 6e2e 636f 6d2f 696e 2f70  inkedin.com/in/p
+00001980: 7269 6d65 7061 7465 6c0a 5b44 6f77 6e6c  rimepatel.[Downl
+00001990: 6f61 6473 2d73 6869 656c 645d 3a20 6874  oads-shield]: ht
+000019a0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000019b0: 732e 696f 2f70 7970 692f 646d 2f61 6b73  s.io/pypi/dm/aks
+000019c0: 6861 7269 6679 3f73 7479 6c65 3d66 6f72  harify?style=for
+000019d0: 2d74 6865 2d62 6164 6765 0a              -the-badge.
```

