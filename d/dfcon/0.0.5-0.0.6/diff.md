# Comparing `tmp/dfcon-0.0.5.tar.gz` & `tmp/dfcon-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfcon-0.0.5.tar", last modified: Tue Jan 31 05:33:30 2023, max compression
+gzip compressed data, was "dfcon-0.0.6.tar", last modified: Tue May 30 09:41:34 2023, max compression
```

## Comparing `dfcon-0.0.5.tar` & `dfcon-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 05:33:30.427790 dfcon-0.0.5/
--rw-rw-rw-   0        0        0      897 2023-01-31 05:31:42.000000 dfcon-0.0.5/CHANGELOG.md
--rw-rw-rw-   0        0        0     1082 2023-01-30 05:00:07.000000 dfcon-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       53 2023-01-30 14:43:14.000000 dfcon-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2884 2023-01-31 05:33:30.427790 dfcon-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2097 2023-01-30 15:37:22.000000 dfcon-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-01-31 05:33:30.384262 dfcon-0.0.5/dfcon/
--rw-rw-rw-   0        0        0      420 2023-01-31 05:25:16.000000 dfcon-0.0.5/dfcon/__init__.py
--rw-rw-rw-   0        0        0    14232 2023-01-31 05:23:46.000000 dfcon-0.0.5/dfcon/directory.py
--rw-rw-rw-   0        0        0     3150 2023-01-30 14:12:01.000000 dfcon-0.0.5/dfcon/filters.py
--rw-rw-rw-   0        0        0    13314 2023-01-30 07:06:17.000000 dfcon-0.0.5/dfcon/path_filter.py
-drwxrwxrwx   0        0        0        0 2023-01-31 05:33:30.414982 dfcon-0.0.5/dfcon.egg-info/
--rw-rw-rw-   0        0        0     2884 2023-01-31 05:33:30.000000 dfcon-0.0.5/dfcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-01-31 05:33:30.000000 dfcon-0.0.5/dfcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 05:33:30.000000 dfcon-0.0.5/dfcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-01-31 05:33:30.000000 dfcon-0.0.5/dfcon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-31 05:33:30.429761 dfcon-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2032 2023-01-30 15:39:25.000000 dfcon-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-31 05:33:30.425764 dfcon-0.0.5/test/
--rw-rw-rw-   0        0        0     1918 2023-01-30 15:35:03.000000 dfcon-0.0.5/test/test1.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:41:34.948757 dfcon-0.0.6/
+-rw-rw-rw-   0        0        0      981 2023-05-30 09:25:19.000000 dfcon-0.0.6/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1082 2023-01-30 05:00:07.000000 dfcon-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-01-30 14:43:14.000000 dfcon-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2884 2023-05-30 09:41:34.949743 dfcon-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2097 2023-01-30 15:37:22.000000 dfcon-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 09:41:34.896743 dfcon-0.0.6/dfcon/
+-rw-rw-rw-   0        0        0      420 2023-05-30 09:40:24.000000 dfcon-0.0.6/dfcon/__init__.py
+-rw-rw-rw-   0        0        0    15624 2023-05-30 07:00:31.000000 dfcon-0.0.6/dfcon/directory.py
+-rw-rw-rw-   0        0        0     3150 2023-01-30 14:12:01.000000 dfcon-0.0.6/dfcon/filters.py
+-rw-rw-rw-   0        0        0    13314 2023-01-30 07:06:17.000000 dfcon-0.0.6/dfcon/path_filter.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:41:34.918243 dfcon-0.0.6/dfcon.egg-info/
+-rw-rw-rw-   0        0        0     2884 2023-05-30 09:41:34.000000 dfcon-0.0.6/dfcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-30 09:41:34.000000 dfcon-0.0.6/dfcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 09:41:34.000000 dfcon-0.0.6/dfcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 09:41:34.000000 dfcon-0.0.6/dfcon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 09:41:34.951743 dfcon-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2032 2023-01-30 15:39:25.000000 dfcon-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:41:34.945743 dfcon-0.0.6/test/
+-rw-rw-rw-   0        0        0     2300 2023-05-30 09:22:33.000000 dfcon-0.0.6/test/test1.py
```

### Comparing `dfcon-0.0.5/CHANGELOG.md` & `dfcon-0.0.6/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -20,8 +20,12 @@
 
 ## [0.0.4] - 2023-01-31
 ### Fixed
 - Module import method fixed for module classification from @MTamon
 
 ## [0.0.5] - 2023-01-31
 ### Added
-- Supported stability of `Directory`'s `get_file_path()` results from @MTamon
+- Supported stability of `Directory`'s `get_file_path()` results from @MTamon
+
+## [0.0.6] - 2023-05-30
+### Added
+- Supported fuction for change Directory's name.
```

### Comparing `dfcon-0.0.5/LICENSE` & `dfcon-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.5/PKG-INFO` & `dfcon-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfcon
-Version: 0.0.5
+Version: 0.0.6
 Summary: To make access to the database easier.
 Home-page: https://github.com/MTamon/dataFileController.git
 Author: Tamon Mikawa
 Author-email: mtamon.engineering@gmail.com
 License: MIT License
 Keywords: DataSet,File-Search,File-Controle
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dfcon-0.0.5/README.md` & `dfcon-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.5/dfcon/directory.py` & `dfcon-0.0.6/dfcon/directory.py`

 * *Files 10% similar despite different names*

```diff
@@ -268,23 +268,22 @@
     ) -> Directory:
         """
         Incarnating instance as an actual directory.
         If a `filters` is specified, the corresponding file will also be copied.
 
         Args:
             path (str):
-                target site for incarnation.
+                Target site for incarnation.
             filters (Filter):
                 Criteria for incarnation.
             printer (Callable[[str], Any]):
                 To print log. When `printer=None`, log can't be output.
 
         Returns
-        -------
-        Directory: incarnated directory instance.
+            Directory: incarnated directory instance.
         """
         if printer is None:
 
             def no_wark(_):
                 pass
 
             printer = no_wark
@@ -370,14 +369,60 @@
         ]
         self.file_member = file_member
 
         self.terminal = len(dirc_member) == 0
         for dirc in self.dirc_member:
             dirc.update_member(filters, empty)
 
+    def update_dir_name(self, new_dir_name: str):
+        """Update Directory's Name
+
+        Args:
+            new_dir_name (str):
+                New name of directory.
+
+        Returns:
+            Directory: Updated Directory instance.
+        """
+
+        if re.match(r"[\\|/]", self.path[-1]):
+            self.path = self.path[:-1]
+
+        self.name = new_dir_name
+
+        split_path = re.split(r"[\\|/]", self.path)
+        split_path[:-1].append(self.name)
+        self.path = os.sep.join(split_path)
+
+        for direc in self.dirc_member:
+            direc.sub_update_dir_name(self.path)
+
+        new_file_member = []
+        for file_path in self.file_member:
+            filename = os.path.basename(file_path)
+            new_file_member.append(os.path.join(self.path, filename))
+
+        self.file_member = new_file_member
+
+    def sub_update_dir_name(self, parent_path: str):
+        """Sub function for update_dir_name."""
+        split_path = re.split(r"[\\|/]", parent_path)
+        split_path.append(self.name)
+        self.path = os.sep.join(split_path)
+
+        for direc in self.dirc_member:
+            direc.sub_update_dir_name(self.path)
+
+        new_file_member = []
+        for file_path in self.file_member:
+            filename = os.path.basename(file_path)
+            new_file_member.append(os.path.join(self.path, filename))
+
+        self.file_member = new_file_member
+
     def remove_member(
         self,
         filters: Filter = None,
         printer: Callable[[str], Any] = print,
     ) -> int:
         """Remove file members
```

### Comparing `dfcon-0.0.5/dfcon/filters.py` & `dfcon-0.0.6/dfcon/filters.py`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.5/dfcon/path_filter.py` & `dfcon-0.0.6/dfcon/path_filter.py`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.5/dfcon.egg-info/PKG-INFO` & `dfcon-0.0.6/dfcon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfcon
-Version: 0.0.5
+Version: 0.0.6
 Summary: To make access to the database easier.
 Home-page: https://github.com/MTamon/dataFileController.git
 Author: Tamon Mikawa
 Author-email: mtamon.engineering@gmail.com
 License: MIT License
 Keywords: DataSet,File-Search,File-Controle
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dfcon-0.0.5/setup.py` & `dfcon-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `dfcon-0.0.5/test/test1.py` & `dfcon-0.0.6/test/test1.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from dfcon.directory import Directory
 from dfcon.path_filter import FileFilter, DircFilter, Filter
 
 
 if __name__ == "__main__":
     if os.path.exists("test/out/exp1/ABCD"):
         shutil.rmtree("test/out/exp1/ABCD")
+    if os.path.exists("test/out/out"):
+        shutil.rmtree("test/out/out")
+    os.mkdir("test/out/out")
 
     dirc = Directory(path="test/out/exp1").build_structure()
 
     print("################# EX1 #################\n")
 
     # example1
     file_filter = FileFilter().include_extention(["py", "txt"])
@@ -65,7 +68,17 @@
     print()
 
     print(
         "incarnated:", cloned.incarnate("test/out/out", filters=filters, printer=print)
     )
 
     cloned.destruct()
+
+    print("\n################# EX3 #################\n")
+
+    cloned = dirc.clone(filters=filters)
+    cloned.update_dir_name(new_dir_name="exp2")
+    print(
+        "incarnated:", cloned.incarnate("test/out/out", filters=filters, printer=print)
+    )
+
+    cloned.destruct()
```

