# Comparing `tmp/Pytanggalmerah-2.0.1.tar.gz` & `tmp/Pytanggalmerah-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pytanggalmerah-2.0.1.tar", last modified: Fri Mar 25 03:08:48 2022, max compression
+gzip compressed data, was "Pytanggalmerah-3.0.0.tar", last modified: Tue May 30 12:07:02 2023, max compression
```

## Comparing `Pytanggalmerah-2.0.1.tar` & `Pytanggalmerah-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 03:08:48.627195 Pytanggalmerah-2.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2022-03-25 03:08:38.000000 Pytanggalmerah-2.0.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1863 2022-03-25 03:08:48.627195 Pytanggalmerah-2.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 03:08:48.625194 Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1863 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      348 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1488 2022-03-25 03:08:38.000000 Pytanggalmerah-2.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      495 2022-03-25 03:08:38.000000 Pytanggalmerah-2.0.1/harilibur
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 03:08:48.626195 Pytanggalmerah-2.0.1/pytanggalmerah/
--rw-rw-rw-   0 root         (0) root         (0)     1549 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/pytanggalmerah/TanggalMerah.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-03-25 03:08:48.000000 Pytanggalmerah-2.0.1/pytanggalmerah/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2022-03-25 03:08:47.000000 Pytanggalmerah-2.0.1/pytanggalmerah/myrequests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 03:08:48.627195 Pytanggalmerah-2.0.1/pytanggalmerahcache/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-25 03:08:38.000000 Pytanggalmerah-2.0.1/pytanggalmerahcache/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-25 03:08:48.627195 Pytanggalmerah-2.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      829 2022-03-25 03:08:47.000000 Pytanggalmerah-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:07:02.381678 Pytanggalmerah-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-05-30 12:06:53.000000 Pytanggalmerah-3.0.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-30 12:07:02.381678 Pytanggalmerah-3.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:07:02.380678 Pytanggalmerah-3.0.0/Pytanggalmerah.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-30 12:07:02.000000 Pytanggalmerah-3.0.0/Pytanggalmerah.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-30 12:07:02.000000 Pytanggalmerah-3.0.0/Pytanggalmerah.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 12:07:02.000000 Pytanggalmerah-3.0.0/Pytanggalmerah.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-30 12:07:02.000000 Pytanggalmerah-3.0.0/Pytanggalmerah.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-30 12:07:02.000000 Pytanggalmerah-3.0.0/Pytanggalmerah.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-30 12:06:53.000000 Pytanggalmerah-3.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-05-30 12:06:53.000000 Pytanggalmerah-3.0.0/harilibur
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:07:02.381678 Pytanggalmerah-3.0.0/pytanggalmerah/
+-rw-rw-rw-   0 root         (0) root         (0)     1588 2023-05-30 12:07:01.000000 Pytanggalmerah-3.0.0/pytanggalmerah/TanggalMerah.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-05-30 12:07:01.000000 Pytanggalmerah-3.0.0/pytanggalmerah/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-05-30 12:07:01.000000 Pytanggalmerah-3.0.0/pytanggalmerah/myrequests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:07:02.381678 Pytanggalmerah-3.0.0/pytanggalmerahcache/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 12:06:53.000000 Pytanggalmerah-3.0.0/pytanggalmerahcache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 12:07:02.381678 Pytanggalmerah-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-05-30 12:07:01.000000 Pytanggalmerah-3.0.0/setup.py
```

### Comparing `Pytanggalmerah-2.0.1/LICENSE.txt` & `Pytanggalmerah-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Pytanggalmerah-2.0.1/PKG-INFO` & `Pytanggalmerah-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: Pytanggalmerah
-Version: 2.0.1
+Version: 3.0.0
 Summary: python module to check indonesia holiday calendar (include sunday)
 Home-page: https://github.com/guangrei/pytanggalmerah
 Author: guangrei
 Author-email: myawn@pm.me
 License: MIT
 Keywords: holiday indonesia calendar sunday
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![Build Status](https://travis-ci.org/guangrei/pytanggalmerah.svg?branch=master)](https://travis-ci.org/guangrei/pytanggalmerah)
 
 **Pytanggalmerah** adalah module python untuk mengecek tanggal merah berdasarkan hari minggu dan hari libur nasional.
 
@@ -57,8 +56,7 @@
 
 ```
 
 > harilibur command hanya mengecek tanggal merah dan tidak termasuk hari minggu.
 ### sumber data
 
 **pytanggalmerah** menggunakan data yang bersumber dari google calendar, data yang telah lampau mungkin tidak tersedia & data yang sekarang masih bisa direvisi.
-
```

### Comparing `Pytanggalmerah-2.0.1/Pytanggalmerah.egg-info/PKG-INFO` & `Pytanggalmerah-3.0.0/Pytanggalmerah.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: Pytanggalmerah
-Version: 2.0.1
+Version: 3.0.0
 Summary: python module to check indonesia holiday calendar (include sunday)
 Home-page: https://github.com/guangrei/pytanggalmerah
 Author: guangrei
 Author-email: myawn@pm.me
 License: MIT
 Keywords: holiday indonesia calendar sunday
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![Build Status](https://travis-ci.org/guangrei/pytanggalmerah.svg?branch=master)](https://travis-ci.org/guangrei/pytanggalmerah)
 
 **Pytanggalmerah** adalah module python untuk mengecek tanggal merah berdasarkan hari minggu dan hari libur nasional.
 
@@ -57,8 +56,7 @@
 
 ```
 
 > harilibur command hanya mengecek tanggal merah dan tidak termasuk hari minggu.
 ### sumber data
 
 **pytanggalmerah** menggunakan data yang bersumber dari google calendar, data yang telah lampau mungkin tidak tersedia & data yang sekarang masih bisa direvisi.
-
```

### Comparing `Pytanggalmerah-2.0.1/README.md` & `Pytanggalmerah-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `Pytanggalmerah-2.0.1/pytanggalmerah/TanggalMerah.py` & `Pytanggalmerah-3.0.0/pytanggalmerah/TanggalMerah.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,19 +34,19 @@
             return True
         else:
             return False
 
     # end is_sunday()
 
     def is_holiday(self):
-        try:
-            d = self.date
-            self.event.add(self.data[d.strftime("%Y%m%d")]['deskripsi'])
+        d = self.date.strftime("%Y-%m-%d")
+        if d in self.data and self.data[d]['holiday']:
+            self.event.add(" | ".join(self.data[d]['summary']))
             return True
-        except KeyError:
+        else:
             return False
 
     # end is_holiday()
 
     def set_date(self, y, m, d):
         self.date = datetime(int(y), int(m), int(d), 0, 0)
         return self.date
```

### Comparing `Pytanggalmerah-2.0.1/pytanggalmerah/myrequests.py` & `Pytanggalmerah-3.0.0/pytanggalmerah/myrequests.py`

 * *Files identical despite different names*

### Comparing `Pytanggalmerah-2.0.1/setup.py` & `Pytanggalmerah-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='Pytanggalmerah',
-    version='2.0.1',
+    version='3.0.0',
     packages=['pytanggalmerah', 'pytanggalmerahcache'],
     scripts=["harilibur"],
     license='MIT',
     author="guangrei",
     author_email="myawn@pm.me",
     description="python module to check indonesia holiday calendar (include sunday)",
     long_description=long_description,
```

