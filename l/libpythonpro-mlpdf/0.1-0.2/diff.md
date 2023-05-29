# Comparing `tmp/libpythonpro_mlpdf-0.1.tar.gz` & `tmp/libpythonpro_mlpdf-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libpythonpro_mlpdf-0.1.tar", last modified: Mon May 29 01:43:53 2023, max compression
+gzip compressed data, was "libpythonpro_mlpdf-0.2.tar", last modified: Mon May 29 22:40:14 2023, max compression
```

## Comparing `libpythonpro_mlpdf-0.1.tar` & `libpythonpro_mlpdf-0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)        0 2023-05-29 01:43:53.525534 libpythonpro_mlpdf-0.1/
--rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)    35184 2023-05-21 00:21:10.000000 libpythonpro_mlpdf-0.1/LICENSE
--rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)    41000 2023-05-29 01:43:53.515272 libpythonpro_mlpdf-0.1/PKG-INFO
--rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)      509 2023-05-28 14:53:41.000000 libpythonpro_mlpdf-0.1/README.md
-drwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)        0 2023-05-29 01:43:52.965763 libpythonpro_mlpdf-0.1/libpythonpro_mlpdf/
--rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)       21 2023-05-25 23:50:16.000000 libpythonpro_mlpdf-0.1/libpythonpro_mlpdf/__init__.py
--rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)      404 2023-05-24 20:50:26.000000 libpythonpro_mlpdf-0.1/libpythonpro_mlpdf/github_api.py
-drwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)        0 2023-05-29 01:43:53.388021 libpythonpro_mlpdf-0.1/libpythonpro_mlpdf.egg-info/
--rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)    41000 2023-05-29 01:43:52.000000 libpythonpro_mlpdf-0.1/libpythonpro_mlpdf.egg-info/PKG-INFO
--rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)      340 2023-05-29 01:43:52.000000 libpythonpro_mlpdf-0.1/libpythonpro_mlpdf.egg-info/SOURCES.txt
--rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)        1 2023-05-29 01:43:52.000000 libpythonpro_mlpdf-0.1/libpythonpro_mlpdf.egg-info/dependency_links.txt
--rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)        1 2023-05-29 01:43:52.000000 libpythonpro_mlpdf-0.1/libpythonpro_mlpdf.egg-info/not-zip-safe
--rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)        9 2023-05-29 01:43:52.000000 libpythonpro_mlpdf-0.1/libpythonpro_mlpdf.egg-info/requires.txt
--rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)       19 2023-05-29 01:43:52.000000 libpythonpro_mlpdf-0.1/libpythonpro_mlpdf.egg-info/top_level.txt
--rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)       38 2023-05-29 01:43:53.529537 libpythonpro_mlpdf-0.1/setup.cfg
--rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)     5384 2023-05-28 16:22:24.000000 libpythonpro_mlpdf-0.1/setup.py
+drwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)        0 2023-05-29 22:40:14.482836 libpythonpro_mlpdf-0.2/
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)    35184 2023-05-21 00:21:10.000000 libpythonpro_mlpdf-0.2/LICENSE
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)       34 2023-05-29 22:39:01.000000 libpythonpro_mlpdf-0.2/MANIFEST.in
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)    41000 2023-05-29 22:40:14.469291 libpythonpro_mlpdf-0.2/PKG-INFO
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)      509 2023-05-28 14:53:41.000000 libpythonpro_mlpdf-0.2/README.md
+drwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)        0 2023-05-29 22:40:13.804275 libpythonpro_mlpdf-0.2/libpythonpro_mlpdf/
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)       21 2023-05-29 22:39:13.000000 libpythonpro_mlpdf-0.2/libpythonpro_mlpdf/__init__.py
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)      404 2023-05-29 21:57:42.000000 libpythonpro_mlpdf-0.2/libpythonpro_mlpdf/github_api.py
+drwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)        0 2023-05-29 22:40:14.365902 libpythonpro_mlpdf-0.2/libpythonpro_mlpdf.egg-info/
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)    41000 2023-05-29 22:40:12.000000 libpythonpro_mlpdf-0.2/libpythonpro_mlpdf.egg-info/PKG-INFO
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)      352 2023-05-29 22:40:13.000000 libpythonpro_mlpdf-0.2/libpythonpro_mlpdf.egg-info/SOURCES.txt
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)        1 2023-05-29 22:40:12.000000 libpythonpro_mlpdf-0.2/libpythonpro_mlpdf.egg-info/dependency_links.txt
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)        1 2023-05-29 01:43:52.000000 libpythonpro_mlpdf-0.2/libpythonpro_mlpdf.egg-info/not-zip-safe
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)        9 2023-05-29 22:40:12.000000 libpythonpro_mlpdf-0.2/libpythonpro_mlpdf.egg-info/requires.txt
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)       19 2023-05-29 22:40:13.000000 libpythonpro_mlpdf-0.2/libpythonpro_mlpdf.egg-info/top_level.txt
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)       38 2023-05-29 22:40:14.486334 libpythonpro_mlpdf-0.2/setup.cfg
+-rwxrwxrwx   0 matheuslopespdf  (1000) matheuslopespdf  (1000)     5384 2023-05-29 21:48:02.000000 libpythonpro_mlpdf-0.2/setup.py
```

### Comparing `libpythonpro_mlpdf-0.1/LICENSE` & `libpythonpro_mlpdf-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libpythonpro_mlpdf-0.1/PKG-INFO` & `libpythonpro_mlpdf-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libpythonpro_mlpdf
-Version: 0.1
+Version: 0.2
 Summary: Módulo para exemplificar construção de projetos Python no curso PyTools
 Home-page: https://github.com/matheuspdf/libpythonpro
 Author: Matheus Lopes
 Author-email: matheuslopes.pdf@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

### Comparing `libpythonpro_mlpdf-0.1/libpythonpro_mlpdf.egg-info/PKG-INFO` & `libpythonpro_mlpdf-0.2/libpythonpro_mlpdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libpythonpro-mlpdf
-Version: 0.1
+Version: 0.2
 Summary: Módulo para exemplificar construção de projetos Python no curso PyTools
 Home-page: https://github.com/matheuspdf/libpythonpro
 Author: Matheus Lopes
 Author-email: matheuslopes.pdf@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

### Comparing `libpythonpro_mlpdf-0.1/setup.py` & `libpythonpro_mlpdf-0.2/setup.py`

 * *Files identical despite different names*

