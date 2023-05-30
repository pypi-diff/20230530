# Comparing `tmp/pySettle-0.1.2.tar.gz` & `tmp/pySettle-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySettle-0.1.2.tar", last modified: Wed Apr  5 06:06:07 2023, max compression
+gzip compressed data, was "pySettle-1.0.0.tar", last modified: Tue May 30 07:54:44 2023, max compression
```

## Comparing `pySettle-0.1.2.tar` & `pySettle-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 adelle     (503) staff       (20)        0 2023-04-05 06:06:07.157711 pySettle-0.1.2/
--rw-r--r--   0 adelle     (503) staff       (20)     1073 2023-04-05 05:41:44.000000 pySettle-0.1.2/LICENSE
--rw-r--r--   0 adelle     (503) staff       (20)      112 2023-04-05 05:41:44.000000 pySettle-0.1.2/MANIFEST.in
--rw-r--r--   0 adelle     (503) staff       (20)     3685 2023-04-05 06:06:07.157385 pySettle-0.1.2/PKG-INFO
--rw-r--r--   0 adelle     (503) staff       (20)     2875 2023-04-05 05:41:44.000000 pySettle-0.1.2/README.rst
-drwxr-xr-x   0 adelle     (503) staff       (20)        0 2023-04-05 06:06:07.153458 pySettle-0.1.2/libsettle/
--rw-r--r--   0 adelle     (503) staff       (20)     1513 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/Makefile
--rw-r--r--   0 adelle     (503) staff       (20)    34620 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/eos.cc
--rw-r--r--   0 adelle     (503) staff       (20)     2043 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/eos.h
--rw-r--r--   0 adelle     (503) staff       (20)     1401 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/gasdev.c
--rw-r--r--   0 adelle     (503) staff       (20)      378 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/gasdev.h
--rw-r--r--   0 adelle     (503) staff       (20)    16212 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/nrutil.c
--rw-r--r--   0 adelle     (503) staff       (20)     2584 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/nrutil.h
--rw-r--r--   0 adelle     (503) staff       (20)    17837 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/odeint.cc
--rw-r--r--   0 adelle     (503) staff       (20)     2533 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/odeint.h
--rw-r--r--   0 adelle     (503) staff       (20)     7705 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/root.c
--rw-r--r--   0 adelle     (503) staff       (20)      414 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/root.h
--rw-r--r--   0 adelle     (503) staff       (20)    13400 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/settle.cc
--rw-r--r--   0 adelle     (503) staff       (20)     6231 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/spline.cc
--rw-r--r--   0 adelle     (503) staff       (20)      701 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/spline.h
--rw-r--r--   0 adelle     (503) staff       (20)     2670 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/useful.cc
--rw-r--r--   0 adelle     (503) staff       (20)      233 2023-04-05 05:41:44.000000 pySettle-0.1.2/libsettle/useful.h
-drwxr-xr-x   0 adelle     (503) staff       (20)        0 2023-04-05 06:06:07.154886 pySettle-0.1.2/pySettle/
--rw-r--r--   0 adelle     (503) staff       (20)      161 2023-04-05 05:41:44.000000 pySettle-0.1.2/pySettle/__init__.py
--rw-r--r--   0 adelle     (503) staff       (20)     7403 2023-04-05 05:41:44.000000 pySettle-0.1.2/pySettle/settler.py
-drwxr-xr-x   0 adelle     (503) staff       (20)        0 2023-04-05 06:06:07.156995 pySettle-0.1.2/pySettle.egg-info/
--rw-r--r--   0 adelle     (503) staff       (20)     3685 2023-04-05 06:06:07.000000 pySettle-0.1.2/pySettle.egg-info/PKG-INFO
--rw-r--r--   0 adelle     (503) staff       (20)      538 2023-04-05 06:06:07.000000 pySettle-0.1.2/pySettle.egg-info/SOURCES.txt
--rw-r--r--   0 adelle     (503) staff       (20)        1 2023-04-05 06:06:07.000000 pySettle-0.1.2/pySettle.egg-info/dependency_links.txt
--rw-r--r--   0 adelle     (503) staff       (20)       12 2023-04-05 06:06:07.000000 pySettle-0.1.2/pySettle.egg-info/requires.txt
--rw-r--r--   0 adelle     (503) staff       (20)       16 2023-04-05 06:06:07.000000 pySettle-0.1.2/pySettle.egg-info/top_level.txt
--rw-r--r--   0 adelle     (503) staff       (20)       38 2023-04-05 06:06:07.157815 pySettle-0.1.2/setup.cfg
--rw-r--r--   0 adelle     (503) staff       (20)     3973 2023-04-05 05:41:44.000000 pySettle-0.1.2/setup.py
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-30 07:54:44.276108 pySettle-1.0.0/
+-rw-rw-r--   0 duncan     (504) staff       (20)     1073 2023-05-25 18:43:00.000000 pySettle-1.0.0/LICENSE
+-rw-rw-r--   0 duncan     (504) staff       (20)      112 2023-05-25 18:43:00.000000 pySettle-1.0.0/MANIFEST.in
+-rw-rw-r--   0 duncan     (504) staff       (20)     2256 2023-05-30 07:54:44.275935 pySettle-1.0.0/PKG-INFO
+-rw-rw-r--   0 duncan     (504) staff       (20)     1446 2023-05-25 18:43:00.000000 pySettle-1.0.0/README.rst
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-30 07:54:44.273132 pySettle-1.0.0/libsettle/
+-rw-rw-r--   0 duncan     (504) staff       (20)     1513 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/Makefile
+-rw-rw-r--   0 duncan     (504) staff       (20)    34620 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/eos.cc
+-rw-rw-r--   0 duncan     (504) staff       (20)     2043 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/eos.h
+-rw-rw-r--   0 duncan     (504) staff       (20)     1401 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/gasdev.c
+-rw-rw-r--   0 duncan     (504) staff       (20)      378 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/gasdev.h
+-rw-rw-r--   0 duncan     (504) staff       (20)    16212 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/nrutil.c
+-rw-rw-r--   0 duncan     (504) staff       (20)     2584 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/nrutil.h
+-rw-rw-r--   0 duncan     (504) staff       (20)    17837 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/odeint.cc
+-rw-rw-r--   0 duncan     (504) staff       (20)     2533 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/odeint.h
+-rw-rw-r--   0 duncan     (504) staff       (20)     7705 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/root.c
+-rw-rw-r--   0 duncan     (504) staff       (20)      414 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/root.h
+-rw-rw-r--   0 duncan     (504) staff       (20)    13585 2023-05-30 07:21:16.000000 pySettle-1.0.0/libsettle/settle.cc
+-rw-rw-r--   0 duncan     (504) staff       (20)     6231 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/spline.cc
+-rw-rw-r--   0 duncan     (504) staff       (20)      701 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/spline.h
+-rw-rw-r--   0 duncan     (504) staff       (20)     2670 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/useful.cc
+-rw-rw-r--   0 duncan     (504) staff       (20)      233 2023-05-25 18:43:00.000000 pySettle-1.0.0/libsettle/useful.h
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-30 07:54:44.274567 pySettle-1.0.0/pySettle/
+-rw-rw-r--   0 duncan     (504) staff       (20)      161 2023-05-30 07:49:19.000000 pySettle-1.0.0/pySettle/__init__.py
+-rw-rw-r--   0 duncan     (504) staff       (20)     7511 2023-05-30 07:21:16.000000 pySettle-1.0.0/pySettle/settler.py
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-30 07:54:44.275668 pySettle-1.0.0/pySettle.egg-info/
+-rw-rw-r--   0 duncan     (504) staff       (20)     2256 2023-05-30 07:54:44.000000 pySettle-1.0.0/pySettle.egg-info/PKG-INFO
+-rw-rw-r--   0 duncan     (504) staff       (20)      538 2023-05-30 07:54:44.000000 pySettle-1.0.0/pySettle.egg-info/SOURCES.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)        1 2023-05-30 07:54:44.000000 pySettle-1.0.0/pySettle.egg-info/dependency_links.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)       12 2023-05-30 07:54:44.000000 pySettle-1.0.0/pySettle.egg-info/requires.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)       16 2023-05-30 07:54:44.000000 pySettle-1.0.0/pySettle.egg-info/top_level.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)       38 2023-05-30 07:54:44.276167 pySettle-1.0.0/setup.cfg
+-rw-rw-r--   0 duncan     (504) staff       (20)     3973 2023-05-25 18:43:00.000000 pySettle-1.0.0/setup.py
```

### Comparing `pySettle-0.1.2/LICENSE` & `pySettle-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/libsettle/Makefile` & `pySettle-1.0.0/libsettle/Makefile`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/libsettle/eos.cc` & `pySettle-1.0.0/libsettle/eos.cc`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/libsettle/eos.h` & `pySettle-1.0.0/libsettle/eos.h`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/libsettle/gasdev.c` & `pySettle-1.0.0/libsettle/gasdev.c`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/libsettle/nrutil.c` & `pySettle-1.0.0/libsettle/nrutil.c`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/libsettle/nrutil.h` & `pySettle-1.0.0/libsettle/nrutil.h`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/libsettle/odeint.cc` & `pySettle-1.0.0/libsettle/odeint.cc`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/libsettle/odeint.h` & `pySettle-1.0.0/libsettle/odeint.h`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/libsettle/root.c` & `pySettle-1.0.0/libsettle/root.c`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/libsettle/settle.cc` & `pySettle-1.0.0/libsettle/settle.cc`

 * *Files 2% similar despite different names*

```diff
@@ -219,15 +219,18 @@
   //printf("Recurrence time =%lg hours\n", *trec);
 
   if (EOS.X[1]==0.0) Xbar=0.5*G.X*G.yd/y;
   else Xbar=G.X*(1.0-0.5*y/G.yd);
   //printf("Xbar=%lg, Q=%lg, Energy=%lg\n", Xbar, 1.6+4.0*Xbar,
   //       4*PI*G.R*G.R*y*9.64e17*(1.6+4.0*Xbar)/ZZ);
 
-  *alpha = 290. / (1.35 + 6.05 * Xbar);
+  // value of 290 was incorrect; correct calculation also depends on redshift
+  // updated prefactor is the mass energy of 1u
+  //*alpha = 290. / (1.35 + 6.05 * Xbar);
+  *alpha = 931.5 *(G.ZZ-1.)/G.ZZ / (1.35 + 6.05 * Xbar);
 
   *fluen = (4*M_PI*G.R*G.R*y*9.64e17*(1.35+6.05*Xbar)/G.ZZ)/1e39; //units of 1e39 erg/g
 
   //printf("eps (14C+alpha) is %lg\n", EOS.C14AG());
   //printf("eps (3a) is %lg\n", EOS.triple_alpha());
 
   //printf("kappa=%lg\n", EOS.opac());
```

### Comparing `pySettle-0.1.2/libsettle/spline.cc` & `pySettle-1.0.0/libsettle/spline.cc`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/libsettle/spline.h` & `pySettle-1.0.0/libsettle/spline.h`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/libsettle/useful.cc` & `pySettle-1.0.0/libsettle/useful.cc`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/pySettle/settler.py` & `pySettle-1.0.0/pySettle/settler.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,21 @@
         Will just return a convenient object to call settle
 
         Has methods:
 
         full: calls settle with all arguments, in case you want to change paramenters,
               it overrides the default F and C, but does not overwrite them
               Takes f, m, x, z, c
-              Returns alpha, trec, fluence
         run : more compact call, which assumes f and c from initialization.
               Takes m, x, and z
-              Returns alpha, trec, fluence
+
+        :param F: the flux from the bottom
+        :param C: include compressional heating (1) or not (0)
+
+        :return: alpha, trec [hr, observer frame], fluence [1e39 erg, observer frame]
         """
         #        path_to_data_file = (
         #            pathlib.Path(__file__).resolve().parent.parent / "settle" / "libsettle.so"
         #        )
 
         # MCU note:
         # Option A:
```

### Comparing `pySettle-0.1.2/pySettle.egg-info/SOURCES.txt` & `pySettle-1.0.0/pySettle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pySettle-0.1.2/setup.py` & `pySettle-1.0.0/setup.py`

 * *Files identical despite different names*

