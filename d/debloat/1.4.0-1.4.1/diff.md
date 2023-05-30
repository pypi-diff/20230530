# Comparing `tmp/debloat-1.4.0.tar.gz` & `tmp/debloat-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debloat-1.4.0.tar", last modified: Tue May 30 12:17:38 2023, max compression
+gzip compressed data, was "debloat-1.4.1.tar", last modified: Tue May 30 12:35:13 2023, max compression
```

## Comparing `debloat-1.4.0.tar` & `debloat-1.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 12:17:38.258473 debloat-1.4.0/
--rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     7405 2023-05-30 12:17:38.258973 debloat-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     6851 2023-04-19 22:52:19.000000 debloat-1.4.0/README.md
--rw-rw-rw-   0        0        0      788 2023-05-30 12:15:47.000000 debloat-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      166 2023-05-30 12:17:38.264474 debloat-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:17:38.199962 debloat-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 12:17:38.219466 debloat-1.4.0/src/debloat/
--rw-rw-rw-   0        0        0        0 2023-05-09 12:13:11.000000 debloat-1.4.0/src/debloat/__init__.py
--rw-rw-rw-   0        0        0     1102 2023-05-09 12:20:28.000000 debloat-1.4.0/src/debloat/archive_processor.py
--rw-rw-rw-   0        0        0      510 2023-03-27 10:51:40.000000 debloat-1.4.0/src/debloat/auxiliary.py
--rw-rw-rw-   0        0        0     3835 2023-04-20 03:29:34.000000 debloat-1.4.0/src/debloat/gui.py
--rw-rw-rw-   0        0        0     1679 2023-05-30 12:10:27.000000 debloat-1.4.0/src/debloat/main.py
--rw-rw-rw-   0        0        0     2536 2023-05-23 11:34:28.000000 debloat-1.4.0/src/debloat/pkreader.py
--rw-rw-rw-   0        0        0    25547 2023-05-30 12:09:28.000000 debloat-1.4.0/src/debloat/processor.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:17:38.256971 debloat-1.4.0/src/debloat/tests/
--rw-rw-rw-   0        0        0        0 2023-05-24 09:41:28.000000 debloat-1.4.0/src/debloat/tests/__init__.py
--rw-rw-rw-   0        0        0     1027 2023-05-25 09:39:42.000000 debloat-1.4.0/src/debloat/tests/debloat_test.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:17:38.253971 debloat-1.4.0/src/debloat.egg-info/
--rw-rw-rw-   0        0        0     7405 2023-05-30 12:17:38.000000 debloat-1.4.0/src/debloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      497 2023-05-30 12:17:38.000000 debloat-1.4.0/src/debloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 12:17:38.000000 debloat-1.4.0/src/debloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-30 12:17:38.000000 debloat-1.4.0/src/debloat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-05-30 12:17:38.000000 debloat-1.4.0/src/debloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 12:17:38.000000 debloat-1.4.0/src/debloat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 12:35:13.553452 debloat-1.4.1/
+-rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0     7405 2023-05-30 12:35:13.553452 debloat-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6851 2023-04-19 22:52:19.000000 debloat-1.4.1/README.md
+-rw-rw-rw-   0        0        0      788 2023-05-30 12:34:12.000000 debloat-1.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0      166 2023-05-30 12:35:13.558951 debloat-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:35:13.505443 debloat-1.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 12:35:13.526446 debloat-1.4.1/src/debloat/
+-rw-rw-rw-   0        0        0        0 2023-05-09 12:13:11.000000 debloat-1.4.1/src/debloat/__init__.py
+-rw-rw-rw-   0        0        0     1102 2023-05-09 12:20:28.000000 debloat-1.4.1/src/debloat/archive_processor.py
+-rw-rw-rw-   0        0        0      510 2023-03-27 10:51:40.000000 debloat-1.4.1/src/debloat/auxiliary.py
+-rw-rw-rw-   0        0        0     3958 2023-05-30 12:28:52.000000 debloat-1.4.1/src/debloat/gui.py
+-rw-rw-rw-   0        0        0     1679 2023-05-30 12:10:27.000000 debloat-1.4.1/src/debloat/main.py
+-rw-rw-rw-   0        0        0     2536 2023-05-23 11:34:28.000000 debloat-1.4.1/src/debloat/pkreader.py
+-rw-rw-rw-   0        0        0    25547 2023-05-30 12:09:28.000000 debloat-1.4.1/src/debloat/processor.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:35:13.551951 debloat-1.4.1/src/debloat/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-24 09:41:28.000000 debloat-1.4.1/src/debloat/tests/__init__.py
+-rw-rw-rw-   0        0        0     1027 2023-05-25 09:39:42.000000 debloat-1.4.1/src/debloat/tests/debloat_test.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:35:13.548951 debloat-1.4.1/src/debloat.egg-info/
+-rw-rw-rw-   0        0        0     7405 2023-05-30 12:35:13.000000 debloat-1.4.1/src/debloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2023-05-30 12:35:13.000000 debloat-1.4.1/src/debloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 12:35:13.000000 debloat-1.4.1/src/debloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-30 12:35:13.000000 debloat-1.4.1/src/debloat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-05-30 12:35:13.000000 debloat-1.4.1/src/debloat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 12:35:13.000000 debloat-1.4.1/src/debloat.egg-info/top_level.txt
```

### Comparing `debloat-1.4.0/LICENSE` & `debloat-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `debloat-1.4.0/PKG-INFO` & `debloat-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.4.0
+Version: 1.4.1
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `debloat-1.4.0/README.md` & `debloat-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `debloat-1.4.0/pyproject.toml` & `debloat-1.4.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debloat"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
   { name="Squiblydoo", email="Squiblydoo@pm.me" },
 ]
 description = "Debloat is an tool to remove excess garbage from bloated executables."
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
```

### Comparing `debloat-1.4.0/src/debloat/archive_processor.py` & `debloat-1.4.1/src/debloat/archive_processor.py`

 * *Files identical despite different names*

### Comparing `debloat-1.4.0/src/debloat/gui.py` & `debloat-1.4.1/src/debloat/gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,15 +68,17 @@
 
     def process(self) -> None:
         '''Process the file at the user provided path.'''
         start_time = time.time()
         file_path = Path(self.pathbox.get())
         self.output_scrollbox_handler("Processing. Please wait.")
         try:
-            pe = pefile.PE(file_path)
+            with open(file_path, "rb") as bloated_file:
+                pe_data = bloated_file.read()
+            pe = pefile.PE(data=pe_data, fast_load=True)
         except Exception:
             self.output_scrollbox_handler('''
 Provided file is not an executable! Please try again 
 with an executable. Maybe it needs unzipped?''')
             self.clear_pathbox()
             return
         out_path = file_path.parent \
```

### Comparing `debloat-1.4.0/src/debloat/main.py` & `debloat-1.4.1/src/debloat/main.py`

 * *Files identical despite different names*

### Comparing `debloat-1.4.0/src/debloat/pkreader.py` & `debloat-1.4.1/src/debloat/pkreader.py`

 * *Files identical despite different names*

### Comparing `debloat-1.4.0/src/debloat/processor.py` & `debloat-1.4.1/src/debloat/processor.py`

 * *Files identical despite different names*

### Comparing `debloat-1.4.0/src/debloat/tests/debloat_test.py` & `debloat-1.4.1/src/debloat/tests/debloat_test.py`

 * *Files identical despite different names*

### Comparing `debloat-1.4.0/src/debloat.egg-info/PKG-INFO` & `debloat-1.4.1/src/debloat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.4.0
+Version: 1.4.1
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

