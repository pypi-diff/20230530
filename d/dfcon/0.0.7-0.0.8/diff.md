# Comparing `tmp/dfcon-0.0.7.tar.gz` & `tmp/dfcon-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfcon-0.0.7.tar", last modified: Tue May 30 12:48:27 2023, max compression
+gzip compressed data, was "dfcon-0.0.8.tar", last modified: Tue May 30 15:12:22 2023, max compression
```

## Comparing `dfcon-0.0.7.tar` & `dfcon-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 12:48:27.255458 dfcon-0.0.7/
--rw-rw-rw-   0        0        0     1070 2023-05-30 12:47:36.000000 dfcon-0.0.7/CHANGELOG.md
--rw-rw-rw-   0        0        0     1082 2023-01-30 05:00:07.000000 dfcon-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       53 2023-01-30 14:43:14.000000 dfcon-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2884 2023-05-30 12:48:27.256452 dfcon-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2097 2023-01-30 15:37:22.000000 dfcon-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 12:48:27.211449 dfcon-0.0.7/dfcon/
--rw-rw-rw-   0        0        0      420 2023-05-30 12:45:45.000000 dfcon-0.0.7/dfcon/__init__.py
--rw-rw-rw-   0        0        0    15645 2023-05-30 12:42:55.000000 dfcon-0.0.7/dfcon/directory.py
--rw-rw-rw-   0        0        0     3150 2023-01-30 14:12:01.000000 dfcon-0.0.7/dfcon/filters.py
--rw-rw-rw-   0        0        0    13314 2023-01-30 07:06:17.000000 dfcon-0.0.7/dfcon/path_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:48:27.251452 dfcon-0.0.7/dfcon.egg-info/
--rw-rw-rw-   0        0        0     2884 2023-05-30 12:48:27.000000 dfcon-0.0.7/dfcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-30 12:48:27.000000 dfcon-0.0.7/dfcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 12:48:27.000000 dfcon-0.0.7/dfcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 12:48:27.000000 dfcon-0.0.7/dfcon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 12:48:27.258459 dfcon-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2032 2023-01-30 15:39:25.000000 dfcon-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:48:27.253965 dfcon-0.0.7/test/
--rw-rw-rw-   0        0        0     2300 2023-05-30 09:22:33.000000 dfcon-0.0.7/test/test1.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:12:22.281090 dfcon-0.0.8/
+-rw-rw-rw-   0        0        0     1159 2023-05-30 15:11:14.000000 dfcon-0.0.8/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1082 2023-01-30 05:00:07.000000 dfcon-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-01-30 14:43:14.000000 dfcon-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2884 2023-05-30 15:12:22.281589 dfcon-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2097 2023-01-30 15:37:22.000000 dfcon-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 15:12:22.244593 dfcon-0.0.8/dfcon/
+-rw-rw-rw-   0        0        0      420 2023-05-30 15:09:40.000000 dfcon-0.0.8/dfcon/__init__.py
+-rw-rw-rw-   0        0        0    17070 2023-05-30 15:09:20.000000 dfcon-0.0.8/dfcon/directory.py
+-rw-rw-rw-   0        0        0     3150 2023-01-30 14:12:01.000000 dfcon-0.0.8/dfcon/filters.py
+-rw-rw-rw-   0        0        0    13314 2023-01-30 07:06:17.000000 dfcon-0.0.8/dfcon/path_filter.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:12:22.275633 dfcon-0.0.8/dfcon.egg-info/
+-rw-rw-rw-   0        0        0     2884 2023-05-30 15:12:22.000000 dfcon-0.0.8/dfcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-30 15:12:22.000000 dfcon-0.0.8/dfcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 15:12:22.000000 dfcon-0.0.8/dfcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 15:12:22.000000 dfcon-0.0.8/dfcon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 15:12:22.283093 dfcon-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2032 2023-01-30 15:39:25.000000 dfcon-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:12:22.278103 dfcon-0.0.8/test/
+-rw-rw-rw-   0        0        0     2300 2023-05-30 09:22:33.000000 dfcon-0.0.8/test/test1.py
```

### Comparing `dfcon-0.0.7/CHANGELOG.md` & `dfcon-0.0.8/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,12 +24,16 @@
 
 ## [0.0.5] - 2023-01-31
 ### Added
 - Supported stability of `Directory`'s `get_file_path()` results from @MTamon
 
 ## [0.0.6] - 2023-05-30
 ### Added
-- Supported fuction for change Directory's name.
+- Supported fuction for changing Directory's name.
 
 ## [0.0.7] - 2023-05-30
 ### Fixed
-- Change update_dir_name() return value: None -> self
+- Change update_dir_name() return value: None -> self
+
+## [0.0.8] - 2023-05-31
+### Added
+- Supported fuction for copying files in hierarchy.
```

### Comparing `dfcon-0.0.7/LICENSE` & `dfcon-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.7/PKG-INFO` & `dfcon-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfcon
-Version: 0.0.7
+Version: 0.0.8
 Summary: To make access to the database easier.
 Home-page: https://github.com/MTamon/dataFileController.git
 Author: Tamon Mikawa
 Author-email: mtamon.engineering@gmail.com
 License: MIT License
 Keywords: DataSet,File-Search,File-Controle
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dfcon-0.0.7/README.md` & `dfcon-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.7/dfcon/directory.py` & `dfcon-0.0.8/dfcon/directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -513,7 +513,43 @@
                     shutil.copyfile(file_path, target_path)
                     if os.path.isfile(target_path) and override:
                         printer(f"ovrd: {file_path} -> {target_path}")
                     else:
                         printer(f"copy: {file_path} -> {target_path}")
                 else:
                     printer(f"exst: {file_path} -> {target_path}")
+
+    def copy_files(
+        self,
+        path: str,
+        filters: Filter = None,
+        printer: Callable[[str], Any] = print,
+        override: bool = False,
+    ):
+        """copy member files in directory & child directorys to path (option: with `filters` for criteria)
+
+        Args:
+            path (str):
+                Path for copy site.
+            filters (Filter, optional):
+                Criteria for copy. Defaults to None.
+            printer (Callable[[str], Any], optional):
+                When `printer=None`, output stream is stopped. Defaults to print.
+            override (bool, optional):
+                Flag whether or not to overwrite existing files. Defaults to False.
+        """
+        if re.match(r"[\\|/]", path[-1]):
+            path = path[:-1]
+        path = os.sep.join(re.split(r"[\\|/]", path))
+
+        files = self.get_file_path(filters, serialize=True)
+
+        for file_path in files:
+            target_path = os.path.join(path, os.path.basename(file_path))
+            if not os.path.isfile(target_path) or override:
+                shutil.copyfile(file_path, target_path)
+                if os.path.isfile(target_path) and override:
+                    printer(f"ovrd: {file_path} -> {target_path}")
+                else:
+                    printer(f"copy: {file_path} -> {target_path}")
+            else:
+                printer(f"exst: {file_path} -> {target_path}")
```

### Comparing `dfcon-0.0.7/dfcon/filters.py` & `dfcon-0.0.8/dfcon/filters.py`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.7/dfcon/path_filter.py` & `dfcon-0.0.8/dfcon/path_filter.py`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.7/dfcon.egg-info/PKG-INFO` & `dfcon-0.0.8/dfcon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfcon
-Version: 0.0.7
+Version: 0.0.8
 Summary: To make access to the database easier.
 Home-page: https://github.com/MTamon/dataFileController.git
 Author: Tamon Mikawa
 Author-email: mtamon.engineering@gmail.com
 License: MIT License
 Keywords: DataSet,File-Search,File-Controle
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dfcon-0.0.7/setup.py` & `dfcon-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.7/test/test1.py` & `dfcon-0.0.8/test/test1.py`

 * *Files identical despite different names*

