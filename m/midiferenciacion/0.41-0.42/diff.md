# Comparing `tmp/midiferenciacion-0.41.tar.gz` & `tmp/midiferenciacion-0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midiferenciacion-0.41.tar", last modified: Thu May 18 18:46:28 2023, max compression
+gzip compressed data, was "midiferenciacion-0.42.tar", last modified: Tue May 30 17:40:19 2023, max compression
```

## Comparing `midiferenciacion-0.41.tar` & `midiferenciacion-0.42.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-18 18:46:28.781356 midiferenciacion-0.41/
--rw-r--r--   0 sarboledab   (501) staff       (20)     1134 2023-05-16 14:58:24.000000 midiferenciacion-0.41/LICENSE
--rw-r--r--   0 sarboledab   (501) staff       (20)      522 2023-05-18 18:46:28.780700 midiferenciacion-0.41/PKG-INFO
--rw-r--r--   0 sarboledab   (501) staff       (20)     1585 2023-05-18 18:45:10.000000 midiferenciacion-0.41/README.md
-drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-18 18:46:28.774412 midiferenciacion-0.41/midiferenciacion/
--rw-r--r--   0 sarboledab   (501) staff       (20)      158 2023-05-18 18:43:35.000000 midiferenciacion-0.41/midiferenciacion/__init__.py
-drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-18 18:46:28.779762 midiferenciacion-0.41/midiferenciacion.egg-info/
--rw-r--r--   0 sarboledab   (501) staff       (20)      522 2023-05-18 18:46:28.000000 midiferenciacion-0.41/midiferenciacion.egg-info/PKG-INFO
--rw-r--r--   0 sarboledab   (501) staff       (20)      314 2023-05-18 18:46:28.000000 midiferenciacion-0.41/midiferenciacion.egg-info/SOURCES.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)        1 2023-05-18 18:46:28.000000 midiferenciacion-0.41/midiferenciacion.egg-info/dependency_links.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)       48 2023-05-18 18:46:28.000000 midiferenciacion-0.41/midiferenciacion.egg-info/entry_points.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)       11 2023-05-18 18:46:28.000000 midiferenciacion-0.41/midiferenciacion.egg-info/requires.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)       17 2023-05-18 18:46:28.000000 midiferenciacion-0.41/midiferenciacion.egg-info/top_level.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)      131 2023-05-16 14:58:32.000000 midiferenciacion-0.41/pyproject.toml
--rw-r--r--   0 sarboledab   (501) staff       (20)       38 2023-05-18 18:46:28.781556 midiferenciacion-0.41/setup.cfg
--rw-r--r--   0 sarboledab   (501) staff       (20)     2239 2023-05-18 18:46:12.000000 midiferenciacion-0.41/setup.py
+drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-30 17:40:19.027711 midiferenciacion-0.42/
+-rw-r--r--   0 sarboledab   (501) staff       (20)     1134 2023-05-16 14:58:24.000000 midiferenciacion-0.42/LICENSE
+-rw-r--r--   0 sarboledab   (501) staff       (20)      522 2023-05-30 17:40:19.027338 midiferenciacion-0.42/PKG-INFO
+-rw-r--r--   0 sarboledab   (501) staff       (20)     1585 2023-05-18 18:45:10.000000 midiferenciacion-0.42/README.md
+drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-30 17:40:19.022746 midiferenciacion-0.42/midiferenciacion/
+-rw-r--r--   0 sarboledab   (501) staff       (20)      158 2023-05-18 18:43:35.000000 midiferenciacion-0.42/midiferenciacion/__init__.py
+drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-30 17:40:19.026807 midiferenciacion-0.42/midiferenciacion.egg-info/
+-rw-r--r--   0 sarboledab   (501) staff       (20)      522 2023-05-30 17:40:18.000000 midiferenciacion-0.42/midiferenciacion.egg-info/PKG-INFO
+-rw-r--r--   0 sarboledab   (501) staff       (20)      314 2023-05-30 17:40:18.000000 midiferenciacion-0.42/midiferenciacion.egg-info/SOURCES.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)        1 2023-05-30 17:40:18.000000 midiferenciacion-0.42/midiferenciacion.egg-info/dependency_links.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)       58 2023-05-30 17:40:18.000000 midiferenciacion-0.42/midiferenciacion.egg-info/entry_points.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)       23 2023-05-30 17:40:18.000000 midiferenciacion-0.42/midiferenciacion.egg-info/requires.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)       17 2023-05-30 17:40:18.000000 midiferenciacion-0.42/midiferenciacion.egg-info/top_level.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)      131 2023-05-16 14:58:32.000000 midiferenciacion-0.42/pyproject.toml
+-rw-r--r--   0 sarboledab   (501) staff       (20)       38 2023-05-30 17:40:19.027842 midiferenciacion-0.42/setup.cfg
+-rw-r--r--   0 sarboledab   (501) staff       (20)     2267 2023-05-30 17:39:34.000000 midiferenciacion-0.42/setup.py
```

### Comparing `midiferenciacion-0.41/LICENSE` & `midiferenciacion-0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `midiferenciacion-0.41/PKG-INFO` & `midiferenciacion-0.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midiferenciacion
-Version: 0.41
+Version: 0.42
 Summary: Make a diferentiation of a given function
 Home-page: https://pypi.org/project/midiferenciacion
 Author: Sofia Arboleda-Bolivar
 Author-email: sofia.arboledab@udea.edu.co
 License: MIT
 Keywords: Dif math
 Classifier: Programming Language :: Python :: 3
```

### Comparing `midiferenciacion-0.41/README.md` & `midiferenciacion-0.42/README.md`

 * *Files identical despite different names*

### Comparing `midiferenciacion-0.41/midiferenciacion.egg-info/PKG-INFO` & `midiferenciacion-0.42/midiferenciacion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midiferenciacion
-Version: 0.41
+Version: 0.42
 Summary: Make a diferentiation of a given function
 Home-page: https://pypi.org/project/midiferenciacion
 Author: Sofia Arboleda-Bolivar
 Author-email: sofia.arboledab@udea.edu.co
 License: MIT
 Keywords: Dif math
 Classifier: Programming Language :: Python :: 3
```

### Comparing `midiferenciacion-0.41/setup.py` & `midiferenciacion-0.42/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,39 +21,39 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.41',
+    version='0.42',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
     
     # ######################################################################
     # ENTRY POINTS
     # ######################################################################
     entry_points={
-        'console_scripts': ['install=midiff.install:main'],
+        'console_scripts': ['install=midiferenciacion.install:main'],
     },
 
     # ######################################################################
     # TESTS
     # ######################################################################
     test_suite='nose.collector',
     tests_require=['nose'],
 
     # ######################################################################
     # DEPENDENCIES
     # ######################################################################
-    install_requires=['matplotlib'],
+    install_requires=['matplotlib', 'scipy', 'numpy'],
 
     # ######################################################################
     # OPTIONS
     # ######################################################################
     include_package_data=True,
     package_data={'': ['data/*.*', 'tests/*.*']},
 )
```

