# Comparing `tmp/locate_pixelcolor_c-0.11.tar.gz` & `tmp/locate_pixelcolor_c-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locate_pixelcolor_c-0.11.tar", last modified: Sat Apr 15 00:33:34 2023, max compression
+gzip compressed data, was "locate_pixelcolor_c-0.12.tar", last modified: Tue May 30 16:31:56 2023, max compression
```

## Comparing `locate_pixelcolor_c-0.11.tar` & `locate_pixelcolor_c-0.12.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 00:33:34.616262 locate_pixelcolor_c-0.11/
--rw-rw-rw-   0        0        0     1148 2023-04-15 00:33:29.000000 locate_pixelcolor_c-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      166 2023-04-15 00:33:28.000000 locate_pixelcolor_c-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     3361 2023-04-15 00:33:34.616262 locate_pixelcolor_c-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     2700 2023-04-15 00:17:54.000000 locate_pixelcolor_c-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 00:33:34.610280 locate_pixelcolor_c-0.11/locate_pixelcolor_c/
--rw-rw-rw-   0        0        0     2700 2023-04-15 00:17:54.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c/README.md
--rw-rw-rw-   0        0        0     4204 2023-04-15 00:17:54.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c/__init__.py
--rw-rw-rw-   0        0        0    45876 2023-04-15 00:17:54.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c/cloop.so
--rw-rw-rw-   0        0        0        5 2023-04-15 00:33:32.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c/requirements.txt
--rw-rw-rw-   0        0        0     2342 2023-04-15 00:33:32.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-15 00:33:34.615265 locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/
--rw-rw-rw-   0        0        0     3361 2023-04-15 00:33:34.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-04-15 00:33:34.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 00:33:34.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-15 00:33:34.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-15 00:33:34.000000 locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-15 00:33:34.617263 locate_pixelcolor_c-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1315 2023-04-15 00:33:32.000000 locate_pixelcolor_c-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:31:56.695670 locate_pixelcolor_c-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-05-30 16:31:51.000000 locate_pixelcolor_c-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      203 2023-05-30 16:31:51.000000 locate_pixelcolor_c-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     3410 2023-05-30 16:31:56.695670 locate_pixelcolor_c-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     2767 2023-05-30 16:30:44.000000 locate_pixelcolor_c-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 16:31:56.690684 locate_pixelcolor_c-0.12/locate_pixelcolor_c/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 locate_pixelcolor_c-0.12/locate_pixelcolor_c/LICENSE
+-rw-rw-rw-   0        0        0     2767 2023-05-30 16:30:44.000000 locate_pixelcolor_c-0.12/locate_pixelcolor_c/README.md
+-rw-rw-rw-   0        0        0     4261 2023-05-30 16:30:09.000000 locate_pixelcolor_c-0.12/locate_pixelcolor_c/__init__.py
+-rw-rw-rw-   0        0        0    45876 2023-05-30 16:25:52.000000 locate_pixelcolor_c-0.12/locate_pixelcolor_c/cloop.so
+-rw-rw-rw-   0        0        0        5 2023-05-30 16:31:55.000000 locate_pixelcolor_c-0.12/locate_pixelcolor_c/requirements.txt
+-rw-rw-rw-   0        0        0    49102 2023-05-30 16:31:55.000000 locate_pixelcolor_c-0.12/locate_pixelcolor_c/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-30 16:31:56.694673 locate_pixelcolor_c-0.12/locate_pixelcolor_c.egg-info/
+-rw-rw-rw-   0        0        0     3410 2023-05-30 16:31:56.000000 locate_pixelcolor_c-0.12/locate_pixelcolor_c.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2023-05-30 16:31:56.000000 locate_pixelcolor_c-0.12/locate_pixelcolor_c.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 16:31:56.000000 locate_pixelcolor_c-0.12/locate_pixelcolor_c.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 16:31:56.000000 locate_pixelcolor_c-0.12/locate_pixelcolor_c.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-30 16:31:56.000000 locate_pixelcolor_c-0.12/locate_pixelcolor_c.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-30 16:31:56.696668 locate_pixelcolor_c-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1299 2023-05-30 16:31:55.000000 locate_pixelcolor_c-0.12/setup.py
```

### Comparing `locate_pixelcolor_c-0.11/LICENSE.rst` & `locate_pixelcolor_c-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_c-0.11/PKG-INFO` & `locate_pixelcolor_c-0.12/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: locate_pixelcolor_c
-Version: 0.11
+Version: 0.12
 Summary: Detects colors in images 10 x faster than Numpy 
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_c
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: C,image,search,rgb
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+
 # Detects colors in images 10 x faster than Numpy 
 
 ### pip install locate-pixelcolor-c
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda
 
 
@@ -34,45 +35,48 @@
 pic = cv2.imread(picx)
 colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
 resus0 = search_colors(pic=pic, colors=colors0)
 colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
 resus1 =  search_colors(pic=pic, colors=colors1)
 ####################################################################
 %timeit search_colors(pic=pic, colors=colors0)
-17.6 ms Â± 245 Âµs per loop (mean Â± std. dev. of 7 runs, 100 loops each)
+17.6 ms ± 245 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
+# last update: 16.3 ms
 
 b,g,r = pic[...,0],pic[...,1],pic[...,2]
 %timeit np.where(((b==255)&(g==255)&(r==255)))
-150 ms Â± 209 Âµs per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+150 ms ± 209 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
 ####################################################################
 %timeit resus1 =  search_colors(pic=pic, colors=colors1)
-138 ms Â± 10 ms per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+138 ms ± 10 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
+# last update: 117 ms
+
 
 %timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
-1 s Â± 16.1 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+1 s ± 16.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 ####################################################################
 ```
 
 
 ### The C Code 
 
 ```c
 
-void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+void colorsearch(unsigned char *pic, unsigned char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
 {
     int counter = 0;
 
     for (int i = 0; i <= totallengthcolor; i += 3)
     {
-        int r = i;
-        int g = i + 1;
-        int b = i + 2;
+        int r = colors[i];
+        int g = colors[i + 1];
+        int b = colors[i + 2];
         for (int j = 0; j <= totallengthpic; j += 3)
         {
-            if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
+            if ((r == pic[j]) && (g == pic[j + 1]) && (b == pic[j + 2]))
             {
 
                 int dividend = j / 3;
                 int quotient = dividend / width;
                 int remainder = dividend % width;
                 int upcounter = counter;
                 outputx[upcounter] = quotient;
```

### Comparing `locate_pixelcolor_c-0.11/README.md` & `locate_pixelcolor_c-0.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,44 +18,47 @@
 colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
 resus0 = search_colors(pic=pic, colors=colors0)
 colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
 resus1 =  search_colors(pic=pic, colors=colors1)
 ####################################################################
 %timeit search_colors(pic=pic, colors=colors0)
 17.6 ms ± 245 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
+# last update: 16.3 ms
 
 b,g,r = pic[...,0],pic[...,1],pic[...,2]
 %timeit np.where(((b==255)&(g==255)&(r==255)))
 150 ms ± 209 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
 ####################################################################
 %timeit resus1 =  search_colors(pic=pic, colors=colors1)
 138 ms ± 10 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
+# last update: 117 ms
+
 
 %timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
 1 s ± 16.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 ####################################################################
 ```
 
 
 ### The C Code 
 
 ```c
 
-void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+void colorsearch(unsigned char *pic, unsigned char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
 {
     int counter = 0;
 
     for (int i = 0; i <= totallengthcolor; i += 3)
     {
-        int r = i;
-        int g = i + 1;
-        int b = i + 2;
+        int r = colors[i];
+        int g = colors[i + 1];
+        int b = colors[i + 2];
         for (int j = 0; j <= totallengthpic; j += 3)
         {
-            if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
+            if ((r == pic[j]) && (g == pic[j + 1]) && (b == pic[j + 2]))
             {
 
                 int dividend = j / 3;
                 int quotient = dividend / width;
                 int remainder = dividend % width;
                 int upcounter = counter;
                 outputx[upcounter] = quotient;
```

### Comparing `locate_pixelcolor_c-0.11/locate_pixelcolor_c/README.md` & `locate_pixelcolor_c-0.12/locate_pixelcolor_c/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,44 +18,47 @@
 colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
 resus0 = search_colors(pic=pic, colors=colors0)
 colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
 resus1 =  search_colors(pic=pic, colors=colors1)
 ####################################################################
 %timeit search_colors(pic=pic, colors=colors0)
 17.6 ms ± 245 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
+# last update: 16.3 ms
 
 b,g,r = pic[...,0],pic[...,1],pic[...,2]
 %timeit np.where(((b==255)&(g==255)&(r==255)))
 150 ms ± 209 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
 ####################################################################
 %timeit resus1 =  search_colors(pic=pic, colors=colors1)
 138 ms ± 10 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
+# last update: 117 ms
+
 
 %timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
 1 s ± 16.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 ####################################################################
 ```
 
 
 ### The C Code 
 
 ```c
 
-void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+void colorsearch(unsigned char *pic, unsigned char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
 {
     int counter = 0;
 
     for (int i = 0; i <= totallengthcolor; i += 3)
     {
-        int r = i;
-        int g = i + 1;
-        int b = i + 2;
+        int r = colors[i];
+        int g = colors[i + 1];
+        int b = colors[i + 2];
         for (int j = 0; j <= totallengthpic; j += 3)
         {
-            if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
+            if ((r == pic[j]) && (g == pic[j + 1]) && (b == pic[j + 2]))
             {
 
                 int dividend = j / 3;
                 int quotient = dividend / width;
                 int remainder = dividend % width;
                 int upcounter = counter;
                 outputx[upcounter] = quotient;
```

### Comparing `locate_pixelcolor_c-0.11/locate_pixelcolor_c/__init__.py` & `locate_pixelcolor_c-0.12/locate_pixelcolor_c/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 cppfile = "cloop.so"
 dllpath = os.path.normpath(os.path.join(os.path.dirname(__file__), cppfile))
 cta = ctypes.cdll.LoadLibrary(dllpath)
 colorsearch = cta.colorsearch
 ccode = r"""
 
 
-void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+void colorsearch(unsigned char *pic, unsigned char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
 {
     int counter = 0;
 
     for (int i = 0; i <= totallengthcolor; i += 3)
     {
-        int r = i;
-        int g = i + 1;
-        int b = i + 2;
+        int r = colors[i];
+        int g = colors[i + 1];
+        int b = colors[i + 2];
         for (int j = 0; j <= totallengthpic; j += 3)
         {
-            if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
+            if ((r == pic[j]) && (g == pic[j + 1]) && (b == pic[j + 2]))
             {
 
                 int dividend = j / 3;
                 int quotient = dividend / width;
                 int remainder = dividend % width;
                 int upcounter = counter;
                 outputx[upcounter] = quotient;
@@ -50,22 +50,22 @@
     pic = cv2.imread(picx)
     colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
     resus0 = search_colors(pic=pic, colors=colors0)
     colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
     resus1 =  search_colors(pic=pic, colors=colors1)
     ####################################################################
     %timeit search_colors(pic=pic, colors=colors0)
-    17.6 ms ± 245 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
+    17.6 ms ± 245 µs per loop (mean ± std. dev. of 7 runs, 100 loops each) # last update: 16.3
 
     b,g,r = pic[...,0],pic[...,1],pic[...,2]
     %timeit np.where(((b==255)&(g==255)&(r==255)))
     150 ms ± 209 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
     ####################################################################
     %timeit resus1 =  search_colors(pic=pic, colors=colors1)
-    138 ms ± 10 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
+    138 ms ± 10 ms per loop (mean ± std. dev. of 7 runs, 10 loops each) # last update: 117
 
     %timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
     1 s ± 16.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
     ####################################################################
 
     """
     if not pic.flags["C_CONTIGUOUS"]:
```

### Comparing `locate_pixelcolor_c-0.11/locate_pixelcolor_c/cloop.so` & `locate_pixelcolor_c-0.12/locate_pixelcolor_c/cloop.so`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 13 23:47:48 2023
+Time/Date		Tue May 30 16:25:52 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	39
 SizeOfCode		0000000000001600
 SizeOfInitializedData	0000000000003200
 SizeOfUninitializedData	0000000000000200
 AddressOfEntryPoint	0000000000001320
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00013000
 SizeOfHeaders		00000600
-CheckSum		0000cee1
+CheckSum		0000c0b8
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
@@ -142,15 +142,15 @@
  0000908c	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x1cc948000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		643894a4
+Time/Date stamp 		64762390
 Major/Minor 			0/0
 Name 				0000000000008032 cloop.so
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000001
 	[Name Pointer/Ordinal] Table	00000001
 Table Addresses
@@ -169,15 +169,15 @@
  00000001cc945000:	00000001cc941000 00000001cc94100c 00000001cc946000
  00000001cc94500c:	00000001cc941010 00000001cc9411cf 00000001cc946004
  00000001cc945018:	00000001cc9411d0 00000001cc941314 00000001cc946018
  00000001cc945024:	00000001cc941320 00000001cc941332 00000001cc946028
  00000001cc945030:	00000001cc941340 00000001cc94134f 00000001cc94602c
  00000001cc94503c:	00000001cc941350 00000001cc94135c 00000001cc946030
  00000001cc945048:	00000001cc941360 00000001cc941361 00000001cc946034
- 00000001cc945054:	00000001cc941370 00000001cc941432 00000001cc946038
+ 00000001cc945054:	00000001cc941370 00000001cc94143a 00000001cc946038
  00000001cc945060:	00000001cc941440 00000001cc94147a 00000001cc94604c
  00000001cc94506c:	00000001cc941480 00000001cc9414ea 00000001cc946054
  00000001cc945078:	00000001cc9414f0 00000001cc94150f 00000001cc946060
  00000001cc945084:	00000001cc941510 00000001cc94153f 00000001cc946064
  00000001cc945090:	00000001cc941540 00000001cc9415c1 00000001cc94606c
  00000001cc94509c:	00000001cc9415d0 00000001cc9415d3 00000001cc946078
  00000001cc9450a8:	00000001cc9415e0 00000001cc941649 00000001cc94607c
@@ -243,15 +243,15 @@
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
  00000001cc946030 (rva: 00006030): 00000001cc941350 - 00000001cc94135c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
  00000001cc946034 (rva: 00006034): 00000001cc941360 - 00000001cc941361
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000001cc946038 (rva: 00006038): 00000001cc941370 - 00000001cc941432
+ 00000001cc946038 (rva: 00006038): 00000001cc941370 - 00000001cc94143a
 	Version: 1, Flags: none
 	Nbr codes: 8, Prologue size: 0x0c, Frame offset: 0x0, Frame reg: none
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push rbp
 	  pc+0x08: push r12
@@ -583,15 +583,15 @@
 [ 53](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000003c .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
 [ 55](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000047 cloop.c
 File 
 [ 57](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000000370 colorsearch
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [ 59](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000370 .text
-AUX scnlen 0xc2 nreloc 0 nlnno 0
+AUX scnlen 0xca nreloc 0 nlnno 0
 [ 61](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [ 63](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [ 65](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000038 .xdata
 AUX scnlen 0x14 nreloc 0 nlnno 0
 [ 67](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000054 .pdata
@@ -1857,79 +1857,70 @@
    1cc941372:	push   %r14
    1cc941374:	push   %r13
    1cc941376:	push   %r12
    1cc941378:	push   %rbp
    1cc941379:	push   %rdi
    1cc94137a:	push   %rsi
    1cc94137b:	push   %rbx
-   1cc94137c:	xor    %ebx,%ebx
-   1cc94137e:	mov    $0xaaaaaaab,%ebp
-   1cc941383:	mov    0x68(%rsp),%esi
-   1cc941387:	mov    0x70(%rsp),%r14
-   1cc94138c:	mov    0x78(%rsp),%r13
-   1cc941391:	mov    0x80(%rsp),%r12
-   1cc941399:	mov    %r8d,%edi
-   1cc94139c:	xor    %r8d,%r8d
-   1cc94139f:	test   %esi,%esi
-   1cc9413a1:	mov    %rcx,%r11
-   1cc9413a4:	mov    %rdx,%r10
-   1cc9413a7:	js     1cc941425 <colorsearch+0xb5>
-   1cc9413a9:	nopl   0x0(%rax)
-   1cc9413b0:	test   %r9d,%r9d
-   1cc9413b3:	js     1cc941418 <colorsearch+0xa8>
-   1cc9413b5:	xor    %ecx,%ecx
-   1cc9413b7:	jmp    1cc9413c9 <colorsearch+0x59>
-   1cc9413b9:	nopl   0x0(%rax)
+   1cc94137c:	mov    0x68(%rsp),%r12d
+   1cc941381:	test   %r12d,%r12d
+   1cc941384:	mov    %rcx,%r10
+   1cc941387:	mov    %rdx,%rsi
+   1cc94138a:	mov    %r8d,%r13d
+   1cc94138d:	js     1cc94142d <colorsearch+0xbd>
+   1cc941393:	xor    %r8d,%r8d
+   1cc941396:	xor    %ebp,%ebp
+   1cc941398:	nopl   0x0(%rax,%rax,1)
+   1cc9413a0:	test   %r9d,%r9d
+   1cc9413a3:	movzbl (%rsi,%r8,1),%r11d
+   1cc9413a8:	movzbl 0x1(%rsi,%r8,1),%ebx
+   1cc9413ae:	movzbl 0x2(%rsi,%r8,1),%edi
+   1cc9413b4:	js     1cc941420 <colorsearch+0xb0>
+   1cc9413b6:	xor    %ecx,%ecx
+   1cc9413b8:	jmp    1cc9413c9 <colorsearch+0x59>
+   1cc9413ba:	nopw   0x0(%rax,%rax,1)
    1cc9413c0:	add    $0x3,%rcx
    1cc9413c4:	cmp    %ecx,%r9d
-   1cc9413c7:	jl     1cc941418 <colorsearch+0xa8>
-   1cc9413c9:	movzbl (%r11,%rcx,1),%eax
-   1cc9413ce:	cmp    %al,(%r10)
-   1cc9413d1:	jne    1cc9413c0 <colorsearch+0x50>
-   1cc9413d3:	movzbl 0x1(%r11,%rcx,1),%eax
-   1cc9413d9:	cmp    %al,0x1(%r10)
-   1cc9413dd:	jne    1cc9413c0 <colorsearch+0x50>
-   1cc9413df:	movzbl 0x2(%r11,%rcx,1),%eax
-   1cc9413e5:	cmp    %al,0x2(%r10)
-   1cc9413e9:	jne    1cc9413c0 <colorsearch+0x50>
-   1cc9413eb:	mov    %ecx,%eax
-   1cc9413ed:	movslq %ebx,%r15
+   1cc9413c7:	jl     1cc941420 <colorsearch+0xb0>
+   1cc9413c9:	cmp    (%r10,%rcx,1),%r11b
+   1cc9413cd:	jne    1cc9413c0 <colorsearch+0x50>
+   1cc9413cf:	cmp    0x1(%r10,%rcx,1),%bl
+   1cc9413d4:	jne    1cc9413c0 <colorsearch+0x50>
+   1cc9413d6:	cmp    0x2(%r10,%rcx,1),%dil
+   1cc9413db:	jne    1cc9413c0 <colorsearch+0x50>
+   1cc9413dd:	mov    %ecx,%eax
+   1cc9413df:	mov    $0xaaaaaaab,%edx
+   1cc9413e4:	mov    0x70(%rsp),%r14
+   1cc9413e9:	movslq %ebp,%r15
+   1cc9413ec:	imul   %rdx,%rax
    1cc9413f0:	add    $0x3,%rcx
-   1cc9413f4:	imul   %rbp,%rax
-   1cc9413f8:	shr    $0x21,%rax
-   1cc9413fc:	cltd
-   1cc9413fd:	idiv   %edi
-   1cc9413ff:	mov    %eax,(%r14,%r15,4)
-   1cc941403:	mov    %edx,0x0(%r13,%r15,4)
-   1cc941408:	mov    %ebx,(%r12)
-   1cc94140c:	add    $0x1,%ebx
-   1cc94140f:	cmp    %ecx,%r9d
-   1cc941412:	jge    1cc9413c9 <colorsearch+0x59>
-   1cc941414:	nopl   0x0(%rax)
-   1cc941418:	add    $0x3,%r8d
-   1cc94141c:	add    $0x3,%r10
-   1cc941420:	cmp    %r8d,%esi
-   1cc941423:	jge    1cc9413b0 <colorsearch+0x40>
-   1cc941425:	pop    %rbx
-   1cc941426:	pop    %rsi
-   1cc941427:	pop    %rdi
-   1cc941428:	pop    %rbp
-   1cc941429:	pop    %r12
-   1cc94142b:	pop    %r13
-   1cc94142d:	pop    %r14
-   1cc94142f:	pop    %r15
-   1cc941431:	ret
-   1cc941432:	nop
-   1cc941433:	nop
-   1cc941434:	nop
-   1cc941435:	nop
-   1cc941436:	nop
-   1cc941437:	nop
-   1cc941438:	nop
-   1cc941439:	nop
+   1cc9413f4:	shr    $0x21,%rax
+   1cc9413f8:	cltd
+   1cc9413f9:	idiv   %r13d
+   1cc9413fc:	mov    %eax,(%r14,%r15,4)
+   1cc941400:	mov    0x78(%rsp),%rax
+   1cc941405:	mov    %edx,(%rax,%r15,4)
+   1cc941409:	mov    0x80(%rsp),%rax
+   1cc941411:	mov    %ebp,(%rax)
+   1cc941413:	add    $0x1,%ebp
+   1cc941416:	cmp    %ecx,%r9d
+   1cc941419:	jge    1cc9413c9 <colorsearch+0x59>
+   1cc94141b:	nopl   0x0(%rax,%rax,1)
+   1cc941420:	add    $0x3,%r8
+   1cc941424:	cmp    %r8d,%r12d
+   1cc941427:	jge    1cc9413a0 <colorsearch+0x30>
+   1cc94142d:	pop    %rbx
+   1cc94142e:	pop    %rsi
+   1cc94142f:	pop    %rdi
+   1cc941430:	pop    %rbp
+   1cc941431:	pop    %r12
+   1cc941433:	pop    %r13
+   1cc941435:	pop    %r14
+   1cc941437:	pop    %r15
+   1cc941439:	ret
    1cc94143a:	nop
    1cc94143b:	nop
    1cc94143c:	nop
    1cc94143d:	nop
    1cc94143e:	nop
    1cc94143f:	nop
 
@@ -3912,15 +3903,15 @@
    1cc94504e:	add    %al,(%rax)
    1cc945050:	xor    $0x60,%al
 	...
 
 00000001cc945054 <.pdata>:
    1cc945054:	jo     1cc945069 <.pdata+0x9>
    1cc945056:	add    %al,(%rax)
-   1cc945058:	xor    (%rax,%rax,1),%dl
+   1cc945058:	cmp    (%rax,%rax,1),%dl
    1cc94505b:	add    %bh,(%rax)
    1cc94505d:	(bad)
 	...
 
 00000001cc945060 <.pdata>:
    1cc945060:	rex adc $0x0,%al
    1cc945063:	add    %bh,0x14(%rdx)
@@ -4400,17 +4391,17 @@
 	...
 
 Disassembly of section .edata:
 
 00000001cc948000 <.edata>:
    1cc948000:	add    %al,(%rax)
    1cc948002:	add    %al,(%rax)
-   1cc948004:	movsb  %ds:(%rsi),%es:(%rdi)
-   1cc948005:	xchg   %eax,%esp
-   1cc948006:	cmp    %ah,0x0(%rax,%rax,1)
+   1cc948004:	nop
+   1cc948005:	and    0x64(%rsi),%esi
+   1cc948008:	add    %al,(%rax)
    1cc94800a:	add    %al,(%rax)
    1cc94800c:	xor    0x10000(%rax),%al
    1cc948012:	add    %al,(%rax)
    1cc948014:	add    %eax,(%rax)
    1cc948016:	add    %al,(%rax)
    1cc948018:	add    %eax,(%rax)
    1cc94801a:	add    %al,(%rax)
```

### Comparing `locate_pixelcolor_c-0.11/locate_pixelcolor_c.egg-info/PKG-INFO` & `locate_pixelcolor_c-0.12/locate_pixelcolor_c.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: locate-pixelcolor-c
-Version: 0.11
+Version: 0.12
 Summary: Detects colors in images 10 x faster than Numpy 
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_c
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: C,image,search,rgb
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+
 # Detects colors in images 10 x faster than Numpy 
 
 ### pip install locate-pixelcolor-c
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda
 
 
@@ -34,45 +35,48 @@
 pic = cv2.imread(picx)
 colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
 resus0 = search_colors(pic=pic, colors=colors0)
 colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
 resus1 =  search_colors(pic=pic, colors=colors1)
 ####################################################################
 %timeit search_colors(pic=pic, colors=colors0)
-17.6 ms Â± 245 Âµs per loop (mean Â± std. dev. of 7 runs, 100 loops each)
+17.6 ms ± 245 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
+# last update: 16.3 ms
 
 b,g,r = pic[...,0],pic[...,1],pic[...,2]
 %timeit np.where(((b==255)&(g==255)&(r==255)))
-150 ms Â± 209 Âµs per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+150 ms ± 209 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
 ####################################################################
 %timeit resus1 =  search_colors(pic=pic, colors=colors1)
-138 ms Â± 10 ms per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+138 ms ± 10 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
+# last update: 117 ms
+
 
 %timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
-1 s Â± 16.1 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+1 s ± 16.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 ####################################################################
 ```
 
 
 ### The C Code 
 
 ```c
 
-void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+void colorsearch(unsigned char *pic, unsigned char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
 {
     int counter = 0;
 
     for (int i = 0; i <= totallengthcolor; i += 3)
     {
-        int r = i;
-        int g = i + 1;
-        int b = i + 2;
+        int r = colors[i];
+        int g = colors[i + 1];
+        int b = colors[i + 2];
         for (int j = 0; j <= totallengthpic; j += 3)
         {
-            if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
+            if ((r == pic[j]) && (g == pic[j + 1]) && (b == pic[j + 2]))
             {
 
                 int dividend = j / 3;
                 int quotient = dividend / width;
                 int remainder = dividend % width;
                 int upcounter = counter;
                 outputx[upcounter] = quotient;
```

### Comparing `locate_pixelcolor_c-0.11/setup.py` & `locate_pixelcolor_c-0.12/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
-# import codecs
-# import os
+import codecs
+import os
 # 
-# here = os.path.abspath(os.path.dirname(__file__))
+here = os.path.abspath(os.path.dirname(__file__))
 # 
-# with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
-#     long_description = "\n" + fh.read()\
+with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
+#long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''Detects colors in images 10 x faster than Numpy '''
 
 # Setting up
 setup(
     name="locate_pixelcolor_c",
     version=VERSION,
     license='MIT',
```

