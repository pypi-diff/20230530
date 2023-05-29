# Comparing `tmp/andreani_aa_testing-0.0.20.tar.gz` & `tmp/andreani_aa_testing-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andreani_aa_testing-0.0.20.tar", last modified: Mon May 29 22:56:30 2023, max compression
+gzip compressed data, was "andreani_aa_testing-0.0.21.tar", last modified: Mon May 29 23:02:14 2023, max compression
```

## Comparing `andreani_aa_testing-0.0.20.tar` & `andreani_aa_testing-0.0.21.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 22:56:30.391143 andreani_aa_testing-0.0.20/
--rw-rw-rw-   0        0        0     1092 2023-05-29 19:17:26.000000 andreani_aa_testing-0.0.20/LICENSE
--rw-rw-rw-   0        0        0     2872 2023-05-29 22:56:30.392148 andreani_aa_testing-0.0.20/PKG-INFO
--rw-rw-rw-   0        0        0      568 2023-05-29 19:17:26.000000 andreani_aa_testing-0.0.20/README.md
--rw-rw-rw-   0        0        0     1345 2023-05-29 22:53:55.000000 andreani_aa_testing-0.0.20/pyproject.toml
--rw-rw-rw-   0        0        0      625 2023-05-29 22:56:30.393142 andreani_aa_testing-0.0.20/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 22:56:30.364410 andreani_aa_testing-0.0.20/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 22:56:30.379023 andreani_aa_testing-0.0.20/src/aa_testing/
--rw-rw-rw-   0        0        0       28 2023-05-29 19:19:54.000000 andreani_aa_testing-0.0.20/src/aa_testing/__init__.py
--rw-rw-rw-   0        0        0      789 2023-05-29 22:54:40.000000 andreani_aa_testing-0.0.20/src/aa_testing/testing.py
-drwxrwxrwx   0        0        0        0 2023-05-29 22:56:30.390202 andreani_aa_testing-0.0.20/src/andreani_aa_testing.egg-info/
--rw-rw-rw-   0        0        0     2872 2023-05-29 22:56:30.000000 andreani_aa_testing-0.0.20/src/andreani_aa_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-05-29 22:56:30.000000 andreani_aa_testing-0.0.20/src/andreani_aa_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 22:56:30.000000 andreani_aa_testing-0.0.20/src/andreani_aa_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-29 22:56:30.000000 andreani_aa_testing-0.0.20/src/andreani_aa_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 23:02:14.696093 andreani_aa_testing-0.0.21/
+-rw-rw-rw-   0        0        0     1092 2023-05-29 19:17:26.000000 andreani_aa_testing-0.0.21/LICENSE
+-rw-rw-rw-   0        0        0     2872 2023-05-29 23:02:14.696093 andreani_aa_testing-0.0.21/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2023-05-29 19:17:26.000000 andreani_aa_testing-0.0.21/README.md
+-rw-rw-rw-   0        0        0     1345 2023-05-29 23:02:00.000000 andreani_aa_testing-0.0.21/pyproject.toml
+-rw-rw-rw-   0        0        0      625 2023-05-29 23:02:14.698713 andreani_aa_testing-0.0.21/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 23:02:14.670259 andreani_aa_testing-0.0.21/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 23:02:14.684347 andreani_aa_testing-0.0.21/src/aa_testing/
+-rw-rw-rw-   0        0        0       28 2023-05-29 19:19:54.000000 andreani_aa_testing-0.0.21/src/aa_testing/__init__.py
+-rw-rw-rw-   0        0        0      789 2023-05-29 22:58:58.000000 andreani_aa_testing-0.0.21/src/aa_testing/testing.py
+drwxrwxrwx   0        0        0        0 2023-05-29 23:02:14.694538 andreani_aa_testing-0.0.21/src/andreani_aa_testing.egg-info/
+-rw-rw-rw-   0        0        0     2872 2023-05-29 23:02:14.000000 andreani_aa_testing-0.0.21/src/andreani_aa_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-05-29 23:02:14.000000 andreani_aa_testing-0.0.21/src/andreani_aa_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 23:02:14.000000 andreani_aa_testing-0.0.21/src/andreani_aa_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-29 23:02:14.000000 andreani_aa_testing-0.0.21/src/andreani_aa_testing.egg-info/top_level.txt
```

### Comparing `andreani_aa_testing-0.0.20/LICENSE` & `andreani_aa_testing-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `andreani_aa_testing-0.0.20/PKG-INFO` & `andreani_aa_testing-0.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andreani_aa_testing
-Version: 0.0.20
+Version: 0.0.21
 Summary: Testing and comparison used by the Andreani Advanced Analytics team
 Home-page: https://github.com/pypa/sampleproject
 Author-email: Gabriel Aranda <garanda@andreani.com>, Mariana Liu <mliu@andreani.com>, Yasmin Ojeda <yojeda@andreani.com>, Daiana Alonso <dalonso@andreani.com>, Facundo Silvestre <fsilvestre@andreani.com>, Santiago Bergman <sbergman@andreani.com>, Matías Moyano <matmoyano@andreani.com>, Giuliana Vera <gvera@andreani.com>, Eloy Chang <echang@andreani.com>, Ezequiel Brodschi <ebrodschi@andreani.com>, Sol Cari <scari@andreani.com>
 License: MIT License
         
         Copyright (c) 2023 Gabriel Aranda
```

### Comparing `andreani_aa_testing-0.0.20/README.md` & `andreani_aa_testing-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `andreani_aa_testing-0.0.20/pyproject.toml` & `andreani_aa_testing-0.0.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "andreani_aa_testing"
-version = "0.0.20"
+version = "0.0.21"
 authors = [
   { name = "Gabriel Aranda", email = "garanda@andreani.com" },
   { name = "Mariana Liu", email = "mliu@andreani.com" },
   { name = "Yasmin Ojeda", email = "yojeda@andreani.com" },
   { name = "Daiana Alonso", email = "dalonso@andreani.com" },
   { name = "Facundo Silvestre", email = "fsilvestre@andreani.com" },
   { name = "Santiago Bergman", email = "sbergman@andreani.com" },
```

### Comparing `andreani_aa_testing-0.0.20/setup.cfg` & `andreani_aa_testing-0.0.21/setup.cfg`

 * *Files identical despite different names*

### Comparing `andreani_aa_testing-0.0.20/src/aa_testing/testing.py` & `andreani_aa_testing-0.0.21/src/aa_testing/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 
-class Testing():
+class testing():
     def __init__(self, first_function, second_function, dataset):
         self.first_function = first_function
         self.second_function = second_function
         self.dataset = dataset
 
     def compare_functions(self):
         start_time = time.time()
```

### Comparing `andreani_aa_testing-0.0.20/src/andreani_aa_testing.egg-info/PKG-INFO` & `andreani_aa_testing-0.0.21/src/andreani_aa_testing.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andreani-aa-testing
-Version: 0.0.20
+Version: 0.0.21
 Summary: Testing and comparison used by the Andreani Advanced Analytics team
 Home-page: https://github.com/pypa/sampleproject
 Author-email: Gabriel Aranda <garanda@andreani.com>, Mariana Liu <mliu@andreani.com>, Yasmin Ojeda <yojeda@andreani.com>, Daiana Alonso <dalonso@andreani.com>, Facundo Silvestre <fsilvestre@andreani.com>, Santiago Bergman <sbergman@andreani.com>, Matías Moyano <matmoyano@andreani.com>, Giuliana Vera <gvera@andreani.com>, Eloy Chang <echang@andreani.com>, Ezequiel Brodschi <ebrodschi@andreani.com>, Sol Cari <scari@andreani.com>
 License: MIT License
         
         Copyright (c) 2023 Gabriel Aranda
```

