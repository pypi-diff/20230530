# Comparing `tmp/dfcon-0.0.6.tar.gz` & `tmp/dfcon-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfcon-0.0.6.tar", last modified: Tue May 30 09:41:34 2023, max compression
+gzip compressed data, was "dfcon-0.0.7.tar", last modified: Tue May 30 12:48:27 2023, max compression
```

## Comparing `dfcon-0.0.6.tar` & `dfcon-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 09:41:34.948757 dfcon-0.0.6/
--rw-rw-rw-   0        0        0      981 2023-05-30 09:25:19.000000 dfcon-0.0.6/CHANGELOG.md
--rw-rw-rw-   0        0        0     1082 2023-01-30 05:00:07.000000 dfcon-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       53 2023-01-30 14:43:14.000000 dfcon-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2884 2023-05-30 09:41:34.949743 dfcon-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2097 2023-01-30 15:37:22.000000 dfcon-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 09:41:34.896743 dfcon-0.0.6/dfcon/
--rw-rw-rw-   0        0        0      420 2023-05-30 09:40:24.000000 dfcon-0.0.6/dfcon/__init__.py
--rw-rw-rw-   0        0        0    15624 2023-05-30 07:00:31.000000 dfcon-0.0.6/dfcon/directory.py
--rw-rw-rw-   0        0        0     3150 2023-01-30 14:12:01.000000 dfcon-0.0.6/dfcon/filters.py
--rw-rw-rw-   0        0        0    13314 2023-01-30 07:06:17.000000 dfcon-0.0.6/dfcon/path_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:41:34.918243 dfcon-0.0.6/dfcon.egg-info/
--rw-rw-rw-   0        0        0     2884 2023-05-30 09:41:34.000000 dfcon-0.0.6/dfcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-30 09:41:34.000000 dfcon-0.0.6/dfcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 09:41:34.000000 dfcon-0.0.6/dfcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 09:41:34.000000 dfcon-0.0.6/dfcon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 09:41:34.951743 dfcon-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2032 2023-01-30 15:39:25.000000 dfcon-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:41:34.945743 dfcon-0.0.6/test/
--rw-rw-rw-   0        0        0     2300 2023-05-30 09:22:33.000000 dfcon-0.0.6/test/test1.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:48:27.255458 dfcon-0.0.7/
+-rw-rw-rw-   0        0        0     1070 2023-05-30 12:47:36.000000 dfcon-0.0.7/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1082 2023-01-30 05:00:07.000000 dfcon-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-01-30 14:43:14.000000 dfcon-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2884 2023-05-30 12:48:27.256452 dfcon-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2097 2023-01-30 15:37:22.000000 dfcon-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 12:48:27.211449 dfcon-0.0.7/dfcon/
+-rw-rw-rw-   0        0        0      420 2023-05-30 12:45:45.000000 dfcon-0.0.7/dfcon/__init__.py
+-rw-rw-rw-   0        0        0    15645 2023-05-30 12:42:55.000000 dfcon-0.0.7/dfcon/directory.py
+-rw-rw-rw-   0        0        0     3150 2023-01-30 14:12:01.000000 dfcon-0.0.7/dfcon/filters.py
+-rw-rw-rw-   0        0        0    13314 2023-01-30 07:06:17.000000 dfcon-0.0.7/dfcon/path_filter.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:48:27.251452 dfcon-0.0.7/dfcon.egg-info/
+-rw-rw-rw-   0        0        0     2884 2023-05-30 12:48:27.000000 dfcon-0.0.7/dfcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-30 12:48:27.000000 dfcon-0.0.7/dfcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 12:48:27.000000 dfcon-0.0.7/dfcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 12:48:27.000000 dfcon-0.0.7/dfcon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 12:48:27.258459 dfcon-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2032 2023-01-30 15:39:25.000000 dfcon-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:48:27.253965 dfcon-0.0.7/test/
+-rw-rw-rw-   0        0        0     2300 2023-05-30 09:22:33.000000 dfcon-0.0.7/test/test1.py
```

### Comparing `dfcon-0.0.6/CHANGELOG.md` & `dfcon-0.0.7/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,8 +24,12 @@
 
 ## [0.0.5] - 2023-01-31
 ### Added
 - Supported stability of `Directory`'s `get_file_path()` results from @MTamon
 
 ## [0.0.6] - 2023-05-30
 ### Added
-- Supported fuction for change Directory's name.
+- Supported fuction for change Directory's name.
+
+## [0.0.7] - 2023-05-30
+### Fixed
+- Change update_dir_name() return value: None -> self
```

### Comparing `dfcon-0.0.6/LICENSE` & `dfcon-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.6/PKG-INFO` & `dfcon-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfcon
-Version: 0.0.6
+Version: 0.0.7
 Summary: To make access to the database easier.
 Home-page: https://github.com/MTamon/dataFileController.git
 Author: Tamon Mikawa
 Author-email: mtamon.engineering@gmail.com
 License: MIT License
 Keywords: DataSet,File-Search,File-Controle
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dfcon-0.0.6/README.md` & `dfcon-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.6/dfcon/directory.py` & `dfcon-0.0.7/dfcon/directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,14 +399,16 @@
         new_file_member = []
         for file_path in self.file_member:
             filename = os.path.basename(file_path)
             new_file_member.append(os.path.join(self.path, filename))
 
         self.file_member = new_file_member
 
+        return self
+
     def sub_update_dir_name(self, parent_path: str):
         """Sub function for update_dir_name."""
         split_path = re.split(r"[\\|/]", parent_path)
         split_path.append(self.name)
         self.path = os.sep.join(split_path)
 
         for direc in self.dirc_member:
```

### Comparing `dfcon-0.0.6/dfcon/filters.py` & `dfcon-0.0.7/dfcon/filters.py`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.6/dfcon/path_filter.py` & `dfcon-0.0.7/dfcon/path_filter.py`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.6/dfcon.egg-info/PKG-INFO` & `dfcon-0.0.7/dfcon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfcon
-Version: 0.0.6
+Version: 0.0.7
 Summary: To make access to the database easier.
 Home-page: https://github.com/MTamon/dataFileController.git
 Author: Tamon Mikawa
 Author-email: mtamon.engineering@gmail.com
 License: MIT License
 Keywords: DataSet,File-Search,File-Controle
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dfcon-0.0.6/setup.py` & `dfcon-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.6/test/test1.py` & `dfcon-0.0.7/test/test1.py`

 * *Files identical despite different names*

