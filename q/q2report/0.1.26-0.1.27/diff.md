# Comparing `tmp/q2report-0.1.26.tar.gz` & `tmp/q2report-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2report-0.1.26.tar", max compression
+gzip compressed data, was "q2report-0.1.27.tar", max compression
```

## Comparing `q2report-0.1.26.tar` & `q2report-0.1.27.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0      475 2023-04-17 10:50:10.817499 q2report-0.1.26/pyproject.toml
--rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.26/q2report/__init__.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.26/q2report/q2engine/__init__.py
--rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.26/q2report/q2engine/q2engine_core.py
--rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.26/q2report/q2engine/q2engine_pyqt.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.26/q2report/q2printer/__init__.py
--rw-r--r--   0        0        0     8053 2023-02-19 21:22:41.218242 q2report-0.1.26/q2report/q2printer/docx_parts.py
--rw-r--r--   0        0        0     7798 2023-04-17 10:49:37.697724 q2report-0.1.26/q2report/q2printer/q2printer.py
--rw-r--r--   0        0        0    18203 2023-02-24 12:25:39.270036 q2report-0.1.26/q2report/q2printer/q2printer_docx.py
--rw-r--r--   0        0        0     5484 2023-02-21 23:03:03.550305 q2report-0.1.26/q2report/q2printer/q2printer_html.py
--rw-r--r--   0        0        0    20036 2023-02-24 12:27:18.839233 q2report-0.1.26/q2report/q2printer/q2printer_xlsx.py
--rw-r--r--   0        0        0     8167 2023-02-20 10:32:47.795979 q2report-0.1.26/q2report/q2printer/xlsx_parts.py
--rw-r--r--   0        0        0    15542 2023-04-17 10:49:55.447800 q2report-0.1.26/q2report/q2report.py
--rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.26/q2report/q2utils.py
--rw-r--r--   0        0        0       22 2023-04-17 10:50:13.570402 q2report-0.1.26/q2report/version.py
--rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.26/README.md
--rw-r--r--   0        0        0     2131 1970-01-01 00:00:00.000000 q2report-0.1.26/setup.py
--rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 q2report-0.1.26/PKG-INFO
+-rw-r--r--   0        0        0      475 2023-05-29 23:26:57.923189 q2report-0.1.27/pyproject.toml
+-rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.27/q2report/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.27/q2report/q2engine/__init__.py
+-rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.27/q2report/q2engine/q2engine_core.py
+-rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.27/q2report/q2engine/q2engine_pyqt.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.27/q2report/q2printer/__init__.py
+-rw-r--r--   0        0        0     8053 2023-02-19 21:22:41.218242 q2report-0.1.27/q2report/q2printer/docx_parts.py
+-rw-r--r--   0        0        0     7873 2023-04-27 21:17:04.262353 q2report-0.1.27/q2report/q2printer/q2printer.py
+-rw-r--r--   0        0        0    18203 2023-02-24 12:25:39.270036 q2report-0.1.27/q2report/q2printer/q2printer_docx.py
+-rw-r--r--   0        0        0     5484 2023-02-21 23:03:03.550305 q2report-0.1.27/q2report/q2printer/q2printer_html.py
+-rw-r--r--   0        0        0    20036 2023-02-24 12:27:18.839233 q2report-0.1.27/q2report/q2printer/q2printer_xlsx.py
+-rw-r--r--   0        0        0     8167 2023-02-20 10:32:47.795979 q2report-0.1.27/q2report/q2printer/xlsx_parts.py
+-rw-r--r--   0        0        0    15542 2023-04-17 10:49:55.447800 q2report-0.1.27/q2report/q2report.py
+-rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.27/q2report/q2utils.py
+-rw-r--r--   0        0        0       22 2023-05-29 23:27:00.308095 q2report-0.1.27/q2report/version.py
+-rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.27/README.md
+-rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 q2report-0.1.27/PKG-INFO
```

### Comparing `q2report-0.1.26/q2report/q2printer/docx_parts.py` & `q2report-0.1.27/q2report/q2printer/docx_parts.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.26/q2report/q2printer/q2printer.py` & `q2report-0.1.27/q2report/q2printer/q2printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,19 +160,20 @@
         return width, height, imageIndex
 
     def save(self):
         self._OF.close()
 
     def show(self):
         if os.path.isfile(self.output_file):
-            if sys.platform[:3] == "win":
+            if sys.platform == "win32":
                 os.startfile(os.path.abspath(self.output_file))
                 # subprocess.Popen(
                 #     ["start", os.path.abspath(self.output_file)],
                 #     close_fds=True,
                 #     shell=True,
                 #     creationflags=subprocess.DETACHED_PROCESS,
                 # )
             # elif sys.platform == 'darwin':
             #     subprocess.Popen(["open", self.output_file], close_fds=True, shell=False)
             else:
-                subprocess.Popen(["open", self.output_file], close_fds=True, shell=False)
+                opener = "open" if sys.platform == "darwin" else "xdg-open"
+                subprocess.Popen([opener, self.output_file], close_fds=True, shell=False)
```

### Comparing `q2report-0.1.26/q2report/q2printer/q2printer_docx.py` & `q2report-0.1.27/q2report/q2printer/q2printer_docx.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.26/q2report/q2printer/q2printer_html.py` & `q2report-0.1.27/q2report/q2printer/q2printer_html.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.26/q2report/q2printer/q2printer_xlsx.py` & `q2report-0.1.27/q2report/q2printer/q2printer_xlsx.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.26/q2report/q2printer/xlsx_parts.py` & `q2report-0.1.27/q2report/q2printer/xlsx_parts.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.26/q2report/q2report.py` & `q2report-0.1.27/q2report/q2report.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.26/q2report/q2utils.py` & `q2report-0.1.27/q2report/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.26/README.md` & `q2report-0.1.27/README.md`

 * *Files identical despite different names*

### Comparing `q2report-0.1.26/PKG-INFO` & `q2report-0.1.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2report
-Version: 0.1.26
+Version: 0.1.27
 Summary: 
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

