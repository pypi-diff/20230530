# Comparing `tmp/locate_pixelcolor_cpppragma-0.11.tar.gz` & `tmp/locate_pixelcolor_cpppragma-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locate_pixelcolor_cpppragma-0.11.tar", last modified: Sat Apr 15 00:38:01 2023, max compression
+gzip compressed data, was "locate_pixelcolor_cpppragma-0.12.tar", last modified: Tue May 30 19:03:34 2023, max compression
```

## Comparing `locate_pixelcolor_cpppragma-0.11.tar` & `locate_pixelcolor_cpppragma-0.12.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 00:38:01.220240 locate_pixelcolor_cpppragma-0.11/
--rw-rw-rw-   0        0        0     1148 2023-04-15 00:37:56.000000 locate_pixelcolor_cpppragma-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      202 2023-04-15 00:37:55.000000 locate_pixelcolor_cpppragma-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     4363 2023-04-15 00:38:01.220240 locate_pixelcolor_cpppragma-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     3670 2023-04-15 00:17:54.000000 locate_pixelcolor_cpppragma-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 00:38:01.216250 locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma/
--rw-rw-rw-   0        0        0     3670 2023-04-15 00:17:54.000000 locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma/README.md
--rw-rw-rw-   0        0        0     4360 2023-04-15 00:17:54.000000 locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma/__init__.py
--rw-rw-rw-   0        0        0    10240 2023-04-15 00:17:54.000000 locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma/clooppra.dll
--rw-rw-rw-   0        0        0        5 2023-04-15 00:37:59.000000 locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma/requirements.txt
--rw-rw-rw-   0        0        0     2342 2023-04-15 00:37:59.000000 locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-15 00:38:01.219242 locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma.egg-info/
--rw-rw-rw-   0        0        0     4363 2023-04-15 00:38:01.000000 locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2023-04-15 00:38:01.000000 locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 00:38:01.000000 locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-15 00:38:01.000000 locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-15 00:38:01.000000 locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-15 00:38:01.220240 locate_pixelcolor_cpppragma-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1351 2023-04-15 00:37:59.000000 locate_pixelcolor_cpppragma-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:03:34.560554 locate_pixelcolor_cpppragma-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-05-30 19:03:30.000000 locate_pixelcolor_cpppragma-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      202 2023-05-30 19:03:29.000000 locate_pixelcolor_cpppragma-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     5644 2023-05-30 19:03:34.560554 locate_pixelcolor_cpppragma-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     4946 2023-05-30 19:02:09.000000 locate_pixelcolor_cpppragma-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 19:03:34.556565 locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma/
+-rw-rw-rw-   0        0        0     4946 2023-05-30 19:02:09.000000 locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma/README.md
+-rw-rw-rw-   0        0        0     5948 2023-05-30 18:58:15.000000 locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma/__init__.py
+-rw-rw-rw-   0        0        0    10752 2023-05-30 18:51:10.000000 locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma/clooppra.dll
+-rw-rw-rw-   0        0        0        5 2023-05-30 19:03:33.000000 locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma/requirements.txt
+-rw-rw-rw-   0        0        0    49102 2023-05-30 19:03:33.000000 locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-30 19:03:34.559557 locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma.egg-info/
+-rw-rw-rw-   0        0        0     5644 2023-05-30 19:03:34.000000 locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2023-05-30 19:03:34.000000 locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 19:03:34.000000 locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 19:03:34.000000 locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-05-30 19:03:34.000000 locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-30 19:03:34.561551 locate_pixelcolor_cpppragma-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1360 2023-05-30 19:03:33.000000 locate_pixelcolor_cpppragma-0.12/setup.py
```

### Comparing `locate_pixelcolor_cpppragma-0.11/LICENSE.rst` & `locate_pixelcolor_cpppragma-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cpppragma-0.11/PKG-INFO` & `locate_pixelcolor_cpppragma-0.12/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,8 @@
-Metadata-Version: 2.1
-Name: locate_pixelcolor_cpppragma
-Version: 0.11
-Summary: Detect colors in images - 20x faster than Numpy
-Home-page: https://github.com/hansalemaos/locate_pixelcolor_cpppragma
-Author: Johannes Fischer
-Author-email: aulasparticularesdealemaosp@gmail.com
-License: MIT
-Keywords: cpp,c++,image,search,parallel,rgb
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
-# Detect colors in images - 20 x faster than Numpy 
+# Detect colors in images - 20 x faster than Numpy / 430 x faster than PIL
 
 ### pip install locate-pixelcolor-cpppragma
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda
 
 ### Important!
 The module imports a function from a compiled .dll (C++). 
@@ -38,57 +21,95 @@
 colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
 resus0 = search_colors(pic=pic, colors=colors0, cpus=5)
 colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
 resus1 =  search_colors(pic=pic, colors=colors1, cpus=4)
 
 ####################################################################
 %timeit resus0 = search_colors(pic=pic, colors=colors0, cpus=5)
-23.4 ms Â± 40.6 Âµs per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+23.4 ms ± 40.6 µs per loop (mean ± std. dev. of 7 runs, 10 loops each) # 10.9 ms after last update
 
 b,g,r = pic[...,0],pic[...,1],pic[...,2]
 %timeit np.where(((b==255)&(g==255)&(r==255)))
-150 ms Â± 209 Âµs per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+150 ms ± 209 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
 ####################################################################
 %timeit resus1 =  search_colors(pic=pic, colors=colors1, cpus=4)
-46.6 ms Â± 988 Âµs per loop (mean Â± std. dev. of 7 runs, 10 loops each)
+46.6 ms ± 988 µs per loop (mean ± std. dev. of 7 runs, 10 loops each) # 43.6 after last update
 
 %timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
-1 s Â± 16.1 ms per loop (mean Â± std. dev. of 7 runs, 1 loop each)
+1 s ± 16.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 ####################################################################
 ```
 
 
 ### The C++ Code 
 
 ```cpp
 #include <omp.h>
 #include <atomic>  
 std::atomic<int> value(0);
 int create_id() {
     return value++;
     }
 
-extern "C" __declspec(dllexport) void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+
+extern "C" __declspec(dllexport) void colorsearch(unsigned char *pic, unsigned char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+{
+    value = 0;
+    int counter = 0;
+
+#pragma omp parallel reduction(+ : counter)
+    {
+
+
+        for (int i = 0; i <= totallengthcolor; i += 3)
+        {
+            int r = colors[i];
+            int g = colors[i + 1];
+            int b = colors[i + 2];
+#pragma omp for schedule(static)            
+            for (int j = 0; j <= totallengthpic; j += 3)
+            {
+                if ((r == pic[j]) && (g == pic[j + 1]) && (b == pic[j + 2]))
+                {
+
+#pragma omp critical
+                    {
+                        int dividend = j / 3;
+                        int quotient = dividend / width;
+                        int remainder = dividend % width;
+                        int upcounter = create_id();
+                        outputx[upcounter] = quotient;
+                        outputy[upcounter] = remainder;
+                        lastresult[0] = upcounter;
+                    }
+                }
+            }
+        }
+    }
+}
+
+
+extern "C" __declspec(dllexport) void colorsearch2(unsigned char *pic, unsigned char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
 {
     value=0;
     int counter = 0;
 
 #pragma omp parallel reduction(+ \
                                : counter)
     {
 
 #pragma omp for schedule(static)
         for (int i = 0; i <= totallengthcolor; i += 3)
         {
-            int r = i;
-            int g = i + 1;
-            int b = i + 2;
+        int r = colors[i];
+        int g = colors[i + 1];
+        int b = colors[i + 2];
             for (int j = 0; j <= totallengthpic; j += 3)
             {
-                if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
+                 if ((r == pic[j]) && (g == pic[j + 1]) && (b == pic[j + 2]))
                 {
 
 #pragma omp critical
                     {
                         int dividend = j / 3;
                         int quotient = dividend / width;
                         int remainder = dividend % width;
@@ -101,8 +122,8 @@
             }
         }
     }
 }
 // Compile:
 // cl.exe /std:c++20 /fp:fast /EHsc /MT /Og /Oi /Ot /Oy /Ob3 /GF /Gy /MD /openmp /LD clooppra.cpp /Fe:clooppra.dll
 // or
-// cl.exe /std:c++20 /fp:fast /EHsc /O2 /MD /openmp /LD clooppra.cpp /Fe:clooppra.dll
+// cl.exe /std:c++20 /fp:fast /EHsc /O2 /MD /openmp /LD clooppra.cpp /Fe:clooppra.dll
```

### Comparing `locate_pixelcolor_cpppragma-0.11/README.md` & `locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Detect colors in images - 20 x faster than Numpy 
+# Detect colors in images - 20 x faster than Numpy / 430 x faster than PIL
 
 ### pip install locate-pixelcolor-cpppragma
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda
 
 ### Important!
 The module imports a function from a compiled .dll (C++). 
@@ -21,22 +21,22 @@
 colors0 = np.array([[255, 255, 255]],dtype=np.uint8)
 resus0 = search_colors(pic=pic, colors=colors0, cpus=5)
 colors1=np.array([(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),],dtype=np.uint8)
 resus1 =  search_colors(pic=pic, colors=colors1, cpus=4)
 
 ####################################################################
 %timeit resus0 = search_colors(pic=pic, colors=colors0, cpus=5)
-23.4 ms ± 40.6 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
+23.4 ms ± 40.6 µs per loop (mean ± std. dev. of 7 runs, 10 loops each) # 10.9 ms after last update
 
 b,g,r = pic[...,0],pic[...,1],pic[...,2]
 %timeit np.where(((b==255)&(g==255)&(r==255)))
 150 ms ± 209 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
 ####################################################################
 %timeit resus1 =  search_colors(pic=pic, colors=colors1, cpus=4)
-46.6 ms ± 988 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
+46.6 ms ± 988 µs per loop (mean ± std. dev. of 7 runs, 10 loops each) # 43.6 after last update
 
 %timeit np.where(((b==66)&(g==71)&(r==69))|((b==62)&(g==67)&(r==65))|((b==144)&(g==155)&(r==153))|((b==52)&(g==57)&(r==55))|((b==127)&(g==138)&(r==136))|((b==53)&(g==58)&(r==56))|((b==51)&(g==56)&(r==54))|((b==32)&(g==27)&(r==18))|((b==24)&(g==17)&(r==8)))
 1 s ± 16.1 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 ####################################################################
 ```
 
 
@@ -46,32 +46,70 @@
 #include <omp.h>
 #include <atomic>  
 std::atomic<int> value(0);
 int create_id() {
     return value++;
     }
 
-extern "C" __declspec(dllexport) void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+
+extern "C" __declspec(dllexport) void colorsearch(unsigned char *pic, unsigned char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+{
+    value = 0;
+    int counter = 0;
+
+#pragma omp parallel reduction(+ : counter)
+    {
+
+
+        for (int i = 0; i <= totallengthcolor; i += 3)
+        {
+            int r = colors[i];
+            int g = colors[i + 1];
+            int b = colors[i + 2];
+#pragma omp for schedule(static)            
+            for (int j = 0; j <= totallengthpic; j += 3)
+            {
+                if ((r == pic[j]) && (g == pic[j + 1]) && (b == pic[j + 2]))
+                {
+
+#pragma omp critical
+                    {
+                        int dividend = j / 3;
+                        int quotient = dividend / width;
+                        int remainder = dividend % width;
+                        int upcounter = create_id();
+                        outputx[upcounter] = quotient;
+                        outputy[upcounter] = remainder;
+                        lastresult[0] = upcounter;
+                    }
+                }
+            }
+        }
+    }
+}
+
+
+extern "C" __declspec(dllexport) void colorsearch2(unsigned char *pic, unsigned char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
 {
     value=0;
     int counter = 0;
 
 #pragma omp parallel reduction(+ \
                                : counter)
     {
 
 #pragma omp for schedule(static)
         for (int i = 0; i <= totallengthcolor; i += 3)
         {
-            int r = i;
-            int g = i + 1;
-            int b = i + 2;
+        int r = colors[i];
+        int g = colors[i + 1];
+        int b = colors[i + 2];
             for (int j = 0; j <= totallengthpic; j += 3)
             {
-                if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
+                 if ((r == pic[j]) && (g == pic[j + 1]) && (b == pic[j + 2]))
                 {
 
 #pragma omp critical
                     {
                         int dividend = j / 3;
                         int quotient = dividend / width;
                         int remainder = dividend % width;
```

### Comparing `locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma/__init__.py` & `locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,41 +2,80 @@
 import numpy as np
 import os
 cppfile = 'clooppra.dll'
 dllpath = os.path.normpath(os.path.join(os.path.dirname(__file__),cppfile))
 lib = ctypes.CDLL(dllpath)
 cpp_function = "colorsearch"
 colorsearch = lib.__getattr__(cpp_function)
-
+cpp_function2 = "colorsearch2"
+colorsearch2 = lib.__getattr__(cpp_function2)
 cppcode = r"""
 #include <omp.h>
 #include <atomic>  
 std::atomic<int> value(0);
 int create_id() {
     return value++;
     }
 
-extern "C" __declspec(dllexport) void colorsearch(char *pic, char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+
+extern "C" __declspec(dllexport) void colorsearch(unsigned char *pic, unsigned char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
+{
+    value = 0;
+    int counter = 0;
+
+#pragma omp parallel reduction(+ : counter)
+    {
+
+
+        for (int i = 0; i <= totallengthcolor; i += 3)
+        {
+            int r = colors[i];
+            int g = colors[i + 1];
+            int b = colors[i + 2];
+#pragma omp for schedule(static)            
+            for (int j = 0; j <= totallengthpic; j += 3)
+            {
+                if ((r == pic[j]) && (g == pic[j + 1]) && (b == pic[j + 2]))
+                {
+
+#pragma omp critical
+                    {
+                        int dividend = j / 3;
+                        int quotient = dividend / width;
+                        int remainder = dividend % width;
+                        int upcounter = create_id();
+                        outputx[upcounter] = quotient;
+                        outputy[upcounter] = remainder;
+                        lastresult[0] = upcounter;
+                    }
+                }
+            }
+        }
+    }
+}
+
+
+extern "C" __declspec(dllexport) void colorsearch2(unsigned char *pic, unsigned char *colors, int width, int totallengthpic, int totallengthcolor, int *outputx, int *outputy, int *lastresult)
 {
     value=0;
     int counter = 0;
 
 #pragma omp parallel reduction(+ \
                                : counter)
     {
 
 #pragma omp for schedule(static)
         for (int i = 0; i <= totallengthcolor; i += 3)
         {
-            int r = i;
-            int g = i + 1;
-            int b = i + 2;
+        int r = colors[i];
+        int g = colors[i + 1];
+        int b = colors[i + 2];
             for (int j = 0; j <= totallengthpic; j += 3)
             {
-                if ((colors[r] == pic[j]) && (colors[g] == pic[j + 1]) && (colors[b] == pic[j + 2]))
+                 if ((r == pic[j]) && (g == pic[j + 1]) && (b == pic[j + 2]))
                 {
 
 #pragma omp critical
                     {
                         int dividend = j / 3;
                         int quotient = dividend / width;
                         int remainder = dividend % width;
@@ -97,19 +136,30 @@
     colorsb = colors.ctypes.data_as(ctypes.POINTER(ctypes.c_uint8))
     totallengthpicb = ctypes.c_int(totallenghtpic)
     totallengthcolorcb = ctypes.c_int(totallengthcolor)
     outputxb = outputx.ctypes.data_as(ctypes.POINTER(ctypes.c_int))
     outputyb = outputy.ctypes.data_as(ctypes.POINTER(ctypes.c_int))
     endresultsb = endresults.ctypes.data_as(ctypes.POINTER(ctypes.c_int))
     widthb = ctypes.c_int(width)
-
-    colorsearch(
-        picb,
-        colorsb,
-        widthb,
-        totallengthpicb,
-        totallengthcolorcb,
-        outputxb,
-        outputyb,
-        endresultsb,
-    )
+    if totallengthcolor == 2:
+        colorsearch(
+            picb,
+            colorsb,
+            widthb,
+            totallengthpicb,
+            totallengthcolorcb,
+            outputxb,
+            outputyb,
+            endresultsb,
+        )
+    else:
+        colorsearch2(
+            picb,
+            colorsb,
+            widthb,
+            totallengthpicb,
+            totallengthcolorcb,
+            outputxb,
+            outputyb,
+            endresultsb,
+        )
     return np.dstack([outputx[:endresults[0]+1], outputy[:endresults[0]+1]])[0]
```

### Comparing `locate_pixelcolor_cpppragma-0.11/locate_pixelcolor_cpppragma.egg-info/SOURCES.txt` & `locate_pixelcolor_cpppragma-0.12/locate_pixelcolor_cpppragma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_cpppragma-0.11/setup.py` & `locate_pixelcolor_cpppragma-0.12/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
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
-DESCRIPTION = '''Detect colors in images - 20x faster than Numpy'''
+VERSION = '''0.12'''
+DESCRIPTION = '''Detect colors in images - 20 x faster than Numpy / 430 x faster than PIL'''
 
 # Setting up
 setup(
     name="locate_pixelcolor_cpppragma",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/locate_pixelcolor_cpppragma',
```

