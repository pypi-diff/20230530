# Comparing `tmp/gravitas-0.1.2.tar.gz` & `tmp/gravitas-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitas-0.1.2.tar", last modified: Tue May 30 02:26:04 2023, max compression
+gzip compressed data, was "gravitas-0.1.3.tar", last modified: Tue May 30 04:55:34 2023, max compression
```

## Comparing `gravitas-0.1.2.tar` & `gravitas-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:26:04.117716 gravitas-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-30 02:26:04.117716 gravitas-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 02:25:52.000000 gravitas-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:26:04.117716 gravitas-0.1.2/gravitas/
--rw-r--r--   0 runner    (1001) docker     (123)  2750335 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/EGM96.c
--rw-r--r--   0 runner    (1001) docker     (123)  2750581 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/GRGM360.c
--rw-r--r--   0 runner    (1001) docker     (123)   300782 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/MRO120F.c
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/gravlib.c
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/libgrav.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:26:04.117716 gravitas-0.1.2/gravitas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-30 02:26:04.000000 gravitas-0.1.2/gravitas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 02:26:04.000000 gravitas-0.1.2/gravitas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 02:26:04.000000 gravitas-0.1.2/gravitas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 02:26:03.000000 gravitas-0.1.2/gravitas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 02:26:04.000000 gravitas-0.1.2/gravitas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 02:26:04.000000 gravitas-0.1.2/gravitas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-30 02:25:52.000000 gravitas-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 02:26:04.117716 gravitas-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-30 02:25:52.000000 gravitas-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:55:34.142473 gravitas-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-30 04:55:34.142473 gravitas-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 04:55:21.000000 gravitas-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:55:34.138473 gravitas-0.1.3/gravitas/
+-rw-r--r--   0 runner    (1001) docker     (123)  2750335 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/EGM96.c
+-rw-r--r--   0 runner    (1001) docker     (123)  2750581 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/GRGM360.c
+-rw-r--r--   0 runner    (1001) docker     (123)   300782 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/MRO120F.c
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/gravlib.c
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-30 04:55:21.000000 gravitas-0.1.3/gravitas/libgrav.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:55:34.142473 gravitas-0.1.3/gravitas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-30 04:55:34.000000 gravitas-0.1.3/gravitas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 04:55:34.000000 gravitas-0.1.3/gravitas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 04:55:34.000000 gravitas-0.1.3/gravitas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 04:55:33.000000 gravitas-0.1.3/gravitas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 04:55:34.000000 gravitas-0.1.3/gravitas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 04:55:34.000000 gravitas-0.1.3/gravitas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-30 04:55:21.000000 gravitas-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 04:55:34.142473 gravitas-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-30 04:55:21.000000 gravitas-0.1.3/setup.py
```

### Comparing `gravitas-0.1.2/gravitas/EGM96.c` & `gravitas-0.1.3/gravitas/EGM96.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.2/gravitas/GRGM360.c` & `gravitas-0.1.3/gravitas/GRGM360.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.2/gravitas/MRO120F.c` & `gravitas-0.1.3/gravitas/MRO120F.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.2/gravitas/__init__.py` & `gravitas-0.1.3/gravitas/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.2/gravitas/gravlib.c` & `gravitas-0.1.3/gravitas/gravlib.c`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #include <stdio.h>
 #include <stdlib.h>
 #include <math.h>
-#include <time.h>
-#include <sys/time.h>
 #include <string.h>
 #include "libgrav.h"
-#include <pthread.h>
+// #include <pthread.h>
 
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 
 #define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 #include <numpy/arrayobject.h>
 
 
-#define NUM_THREADS 10
+#define NUM_THREADS 1
 #define MAX_RF 100000
 
 
 // Vector3 type
 typedef struct Vector3 {
     double x;
     double y;
@@ -52,30 +50,14 @@
 double req;
 double mu;
 int model_index;
 int body_index;
 Vector3 rfs[MAX_RF];
 Vector3 gs[MAX_RF];
 
-
-// uint64_t GetTimeStamp() {
-//     struct timeval tv;
-//     gettimeofday(&tv,NULL);
-//     return tv.tv_sec*(uint64_t)1000000+tv.tv_usec;
-// }
-
-// uint64_t dt;
-// void tic() {
-//     dt = GetTimeStamp();
-// }
-
-// void toc() {
-//     printf("Elapsed time: %.2e\n", (float) ((GetTimeStamp()-dt)) / 1000000);
-// }
-
 double Vector3Norm(Vector3 v) {
     return sqrt(v.x*v.x + v.y*v.y + v.z*v.z);
 }
 
 Vector3 Vector3Scale(Vector3 v, double s) {
     return (Vector3) {v.x*s, v.y*s, v.z*s};
 }
@@ -172,24 +154,29 @@
         if(*(m+i) == nmax) {
             break;
         }
     }
 
     snm[0] = 0.0;
     cnm[0] = 1.0;
+    // free((void*) n); //ansi-c but also not working
+    // free((void*) m);
+    // free((void*) c);
+    // free((void*) s);
     return;
 }
 
 Vector3 pinesnorm(Vector3 rf, double cnm[],
                double snm[], int nmax, double mu, double req) {
     // Based on pinesnorm() from: https://core.ac.uk/download/pdf/76424485.pdf
     double rmag = Vector3Norm(rf);
     Vector3 stu = Vector3Hat(rf);
     int anm_sz = nm2i(nmax+3, nmax+3);
-    double anm[anm_sz];
+    double *anm = malloc(anm_sz * sizeof(double)); //ansi-c
+    // double anm[anm_sz];
     anm[0] = sqrt(2.0);
      
     for(int m = 0; m <= nmax+2; m++) {
         if(m != 0) { // DIAGONAL RECURSION
             anm[nm2i(m,m)] = sqrt(1.0+1.0/(2.0*m))*anm[nm2i(m-1,m-1)];
         }
         if(m != nmax+2) { // FIRST OFF-DIAGONAL RECURSION 
@@ -207,16 +194,18 @@
             }
         }
     }
     for(int n = 0; n <= nmax+2; n++) {
         anm[nm2i(n,0)] *= sqrt(0.50);
     }
      
-    double rm[nmax+2];
-    double im[nmax+2];
+    double* rm = (double*) malloc((nmax+2) * sizeof(double)); //ansi-c
+    double* im = (double*) malloc((nmax+2) * sizeof(double)); //ansi-c
+    // double rm[nmax+2];
+    // double im[nmax+2];
     rm[0] = 0.00; rm[1] = 1.00; 
     im[0] = 0.00; im[1] = 0.00; 
     for(int m = 2; m < nmax+2; m++) {
         rm[m] = stu.x*rm[m-1] - stu.y*im[m-1]; 
         im[m] = stu.x*im[m-1] + stu.y*rm[m-1];
     }
     double rho  = mu/(req*rmag);
@@ -253,14 +242,17 @@
         g2 += rho*g2t; 
         g3 += rho*g3t; 
         g4 += rho*g4t;
         // printf("n=%d, g1 = %.2e, g2 = %.2e, g3 = %.2e, g4 = %.2e\n", 
         // n, g1, g2, g3, g4);
     }
     Vector3 rv = (Vector3) {g1-g4*stu.x, g2-g4*stu.y, g3-g4*stu.z};
+
+    free(anm);
+
     return rv;
 }
 
 typedef struct thread_args{
     int start_ind;
     int end_ind;
     int nmax;
@@ -290,58 +282,63 @@
     
     if (PyArray_DESCR(r_ecef)->type_num != NPY_DOUBLE)
         return failure(PyExc_TypeError, "Type np.float64 expected for input ECEF position array.");
     if (PyArray_NDIM(r_ecef) != 2)
         return failure(PyExc_TypeError, "ECEF position must be [n x 3].");
 
     int npts = PyArray_DIM(r_ecef, 0);
-    double x[npts];
-    double y[npts];
-    double z[npts];
+    double* x = (double*) malloc(npts * sizeof(double)); //ansi-c
+    double* y = (double*) malloc(npts * sizeof(double));
+    double* z = (double*) malloc(npts * sizeof(double));
+    // double x[npts];
+    // double y[npts];
+    // double z[npts];
     PyObject* accel_vector = PyList_New(3 * npts);
     numpy_nx3_to_xyz(r_ecef, x, y, z);
 
     set_indices(model_name, &model_index, &body_index);
     set_body_params(body_index, &mu, &req);
     int sz = nm2i(nmax+2, nmax+2);
-    double cnm[sz];
-    double snm[sz];
+    double* cnm = (double*) malloc(sz * sizeof(double)); //ansi-c
+    double* snm = (double*) malloc(sz * sizeof(double));
+    // double cnm[sz];
+    // double snm[sz];
     read_cnm_snm(nmax, model_index, cnm, snm);
 
     for(int i = 0; i < npts; i++) {
-        rfs[i] = (Vector3) (Vector3){x[i], y[i], z[i]};
+        rfs[i] = (Vector3){x[i], y[i], z[i]};
     }
 
-    pthread_t thread[NUM_THREADS];
-    pthread_attr_t attr;
-    pthread_attr_init(&attr);
-    size_t stacksize;
-    pthread_attr_getstacksize(&attr, &stacksize);
-    pthread_attr_setstacksize(&attr, 2*stacksize);
-
-    thread_args targs[NUM_THREADS];
+    // pthread_t thread[NUM_THREADS];
+    // pthread_attr_t attr;
+    // pthread_attr_init(&attr);
+    // size_t stacksize;
+    // pthread_attr_getstacksize(&attr, &stacksize);
+    // pthread_attr_setstacksize(&attr, 2*stacksize);
+
+    // thread_args targs[NUM_THREADS];
+
+    // for(int i = 0; i < NUM_THREADS; i++) {
+    //     int start_ind = i * npts / NUM_THREADS;
+    //     int end_ind = (i+1) * npts / NUM_THREADS;
+    //     targs[i] = (thread_args) {start_ind, end_ind, nmax, &cnm, &snm};
+    // }
+
+    // for(int i = 0; i < NUM_THREADS; i++) {
+    //     pthread_create(&thread[i], &attr, &thread_func, &targs[i]);
+    // }
+    // for(int i = 0; i < NUM_THREADS; i++) {
+    //     if (pthread_join(thread[i], NULL) != 0) {
+    //         printf("ERROR : pthread join failed.\n");
+    //         return (0);
+    //     }
+    // }
 
-    for(int i = 0; i < NUM_THREADS; i++) {
-        int start_ind = i * npts / NUM_THREADS;
-        int end_ind = (i+1) * npts / NUM_THREADS;
-        targs[i] = (thread_args) {start_ind, end_ind, nmax, &cnm, &snm};
-    }
-
-    for(int i = 0; i < NUM_THREADS; i++) {
-        pthread_create(&thread[i], &attr, &thread_func, &targs[i]);
-    }
-    for(int i = 0; i < NUM_THREADS; i++) {
-        if (pthread_join(thread[i], NULL) != 0) {
-            printf("ERROR : pthread join failed.\n");
-            return (0);
-        }
-    }
-    // printf("Running one with one thread!\n");
-    // thread_func(&(thread_args) {0, npts, nmax, &cnm, &snm});
-    
+    // If we just want to run on one thread
+    thread_func(&(thread_args) {0, npts, nmax, cnm, snm});
     
     double* res = (double*) malloc(3 * npts * sizeof(double));
     for(int i = 0; i < npts; i++) {
         res[3*i + 0] = gs[i].x;
         res[3*i + 1] = gs[i].y;
         res[3*i + 2] = gs[i].z;
```

### Comparing `gravitas-0.1.2/gravitas/lib.py` & `gravitas-0.1.3/gravitas/lib.py`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.2/gravitas/libgrav.h` & `gravitas-0.1.3/gravitas/libgrav.h`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.2/setup.py` & `gravitas-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,50 @@
 from setuptools import setup, find_packages, Extension
+from setuptools.command.build_ext import build_ext
+
 import os
 import numpy as np
 
 _SOURCES = [os.path.join('gravitas', x) for x in os.listdir('gravitas') if '.c' == x[-2:]]
 _INCDIR = ['gravitas', np.get_include()]
+
+class CustomBuildExt(build_ext):
+    def build_extensions(self):
+        # for ext in self.extensions:
+        #     if self.compiler.compiler_type == 'msvc':
+        #         ext.extra_compile_args.append('/std:c90')
+        super().build_extensions()
+
 # _LIB_DIR
 setup(
     name='gravitas',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     license='GPL-2',
     long_description="""High-fidelity gravity fields for satellite propagation""",
     long_description_content_type='text/markdown',
     author="Liam Robinson",
     author_email="robin502@purdue.edu",
     install_requires=['numpy'],
     package_data={'gravitas': ['libgrav.h']},
     classifiers=[
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: MacOS",
+        "Operating System :: Microsoft :: Windows",
     ],
     ext_modules=[
         Extension(
             # the qualified name of the extension module to build
             'gravitas._grav',
             # the files to compile into our module relative to ``setup.py``
             sources=_SOURCES,
             include_dirs=_INCDIR
         ),
     ],
+    cmdclass={
+        'build_ext': CustomBuildExt,
+    },
     zip_safe=False,  # Allow the package to be unzipped without modification
 )
```

