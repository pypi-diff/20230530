# Comparing `tmp/gravitas-0.1.1.tar.gz` & `tmp/gravitas-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitas-0.1.1.tar", last modified: Mon May 29 23:22:06 2023, max compression
+gzip compressed data, was "gravitas-0.1.2.tar", last modified: Tue May 30 02:26:04 2023, max compression
```

## Comparing `gravitas-0.1.1.tar` & `gravitas-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:22:06.397531 gravitas-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-29 23:22:06.397531 gravitas-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 23:21:56.000000 gravitas-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:22:06.393531 gravitas-0.1.1/gravitas/
--rw-r--r--   0 runner    (1001) docker     (123)  2750335 2023-05-29 23:21:56.000000 gravitas-0.1.1/gravitas/EGM96.c
--rw-r--r--   0 runner    (1001) docker     (123)  2750581 2023-05-29 23:21:56.000000 gravitas-0.1.1/gravitas/GRGM360.c
--rw-r--r--   0 runner    (1001) docker     (123)   300782 2023-05-29 23:21:56.000000 gravitas-0.1.1/gravitas/MRO120F.c
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-29 23:21:56.000000 gravitas-0.1.1/gravitas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-05-29 23:21:56.000000 gravitas-0.1.1/gravitas/gravlib.c
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-29 23:21:56.000000 gravitas-0.1.1/gravitas/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:22:06.393531 gravitas-0.1.1/gravitas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-29 23:22:06.000000 gravitas-0.1.1/gravitas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-29 23:22:06.000000 gravitas-0.1.1/gravitas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:22:06.000000 gravitas-0.1.1/gravitas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:22:06.000000 gravitas-0.1.1/gravitas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 23:22:06.000000 gravitas-0.1.1/gravitas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 23:22:06.000000 gravitas-0.1.1/gravitas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-29 23:21:56.000000 gravitas-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:22:06.397531 gravitas-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-29 23:21:56.000000 gravitas-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:26:04.117716 gravitas-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-30 02:26:04.117716 gravitas-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 02:25:52.000000 gravitas-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:26:04.117716 gravitas-0.1.2/gravitas/
+-rw-r--r--   0 runner    (1001) docker     (123)  2750335 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/EGM96.c
+-rw-r--r--   0 runner    (1001) docker     (123)  2750581 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/GRGM360.c
+-rw-r--r--   0 runner    (1001) docker     (123)   300782 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/MRO120F.c
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/gravlib.c
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-30 02:25:52.000000 gravitas-0.1.2/gravitas/libgrav.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:26:04.117716 gravitas-0.1.2/gravitas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-30 02:26:04.000000 gravitas-0.1.2/gravitas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 02:26:04.000000 gravitas-0.1.2/gravitas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 02:26:04.000000 gravitas-0.1.2/gravitas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 02:26:03.000000 gravitas-0.1.2/gravitas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 02:26:04.000000 gravitas-0.1.2/gravitas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 02:26:04.000000 gravitas-0.1.2/gravitas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-30 02:25:52.000000 gravitas-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 02:26:04.117716 gravitas-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-30 02:25:52.000000 gravitas-0.1.2/setup.py
```

### Comparing `gravitas-0.1.1/gravitas/EGM96.c` & `gravitas-0.1.2/gravitas/EGM96.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.1/gravitas/GRGM360.c` & `gravitas-0.1.2/gravitas/GRGM360.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.1/gravitas/MRO120F.c` & `gravitas-0.1.2/gravitas/MRO120F.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.1/gravitas/__init__.py` & `gravitas-0.1.2/gravitas/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.1/gravitas/gravlib.c` & `gravitas-0.1.2/gravitas/gravlib.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.1/gravitas/lib.py` & `gravitas-0.1.2/gravitas/lib.py`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.1/setup.py` & `gravitas-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 import numpy as np
 
 _SOURCES = [os.path.join('gravitas', x) for x in os.listdir('gravitas') if '.c' == x[-2:]]
 _INCDIR = ['gravitas', np.get_include()]
 # _LIB_DIR
 setup(
     name='gravitas',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     license='GPL-2',
     long_description="""High-fidelity gravity fields for satellite propagation""",
     long_description_content_type='text/markdown',
     author="Liam Robinson",
     author_email="robin502@purdue.edu",
     install_requires=['numpy'],
+    package_data={'gravitas': ['libgrav.h']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: MacOS",
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
-    include_package_data=True,  # Include non-Python files in packages
     zip_safe=False,  # Allow the package to be unzipped without modification
 )
```

