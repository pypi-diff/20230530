# Comparing `tmp/scanimage-tiff-reader-1.4.1.tar.gz` & `tmp/scanimage-tiff-reader-1.4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\scanimage-tiff-reader-1.4.1.tar", last modified: Wed Feb 13 16:03:01 2019, max compression
+gzip compressed data, was "C:\Gitlab\scanimagetiffreader-python\dist\.tmp-i325r66q\scanimage-tiff-reader-1.4.1.3.tar", last modified: Tue May 30 14:58:52 2023, max compression
```

## Comparing `scanimage-tiff-reader-1.4.1.tar` & `scanimage-tiff-reader-1.4.1.3.tar`

### file list

```diff
@@ -1,37 +1,30 @@
-drwxrwxrwx   0        0        0        0 2019-02-13 16:03:01.000000 scanimage-tiff-reader-1.4.1/
--rw-rw-rw-   0        0        0      576 2018-10-05 13:37:22.000000 scanimage-tiff-reader-1.4.1/LICENSE
--rw-rw-rw-   0        0        0      119 2018-10-09 19:54:23.000000 scanimage-tiff-reader-1.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3274 2019-02-13 16:03:01.000000 scanimage-tiff-reader-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2076 2019-02-13 14:33:27.000000 scanimage-tiff-reader-1.4.1/README.rst
--rw-rw-rw-   0        0        0       42 2019-02-13 16:03:01.000000 scanimage-tiff-reader-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1640 2019-02-13 16:02:17.000000 scanimage-tiff-reader-1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2019-02-13 16:03:00.000000 scanimage-tiff-reader-1.4.1/src/
--rw-rw-rw-   0        0        0       48 2018-10-10 16:41:11.000000 scanimage-tiff-reader-1.4.1/src/.gitignore
-drwxrwxrwx   0        0        0        0 2019-02-13 16:03:00.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/
--rw-rw-rw-   0        0        0    13401 2019-02-13 15:54:49.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/__init__.py
--rw-rw-rw-   0        0        0    14605 2018-10-16 17:50:47.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/__init__.pyc
-drwxrwxrwx   0        0        0        0 2019-02-13 16:03:00.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/__pycache__/
--rw-rw-rw-   0        0        0    12324 2018-10-10 16:32:28.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0    12853 2019-02-13 15:54:52.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/__pycache__/__init__.cpython-37.pyc
-drwxrwxrwx   0        0        0        0 2019-02-13 16:03:00.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/
--rw-rw-rw-   0        0        0      708 2018-10-05 20:02:00.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/README.md
-drwxrwxrwx   0        0        0        0 2019-02-13 16:02:58.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/
-drwxrwxrwx   0        0        0        0 2019-02-13 16:03:00.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/lib/
--rw-rw-rw-   0        0        0   379788 2019-02-13 15:46:27.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/lib/libScanImageTiffReaderAPI.so
-drwxrwxrwx   0        0        0        0 2019-02-13 16:02:58.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/
-drwxrwxrwx   0        0        0        0 2019-02-13 16:03:00.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/lib/
--rw-rw-rw-   0        0        0  2409728 2019-02-13 15:46:16.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/lib/libScanImageTiffReaderAPI.so
-drwxrwxrwx   0        0        0        0 2019-02-13 16:03:00.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/
-drwxrwxrwx   0        0        0        0 2019-02-13 16:03:00.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/lib/
--rw-rw-rw-   0        0        0   538112 2019-02-13 15:46:40.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/lib/ScanImageTiffReaderAPI.dll
--rw-rw-rw-   0        0        0      919 2019-02-13 15:51:25.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/__init__.py
--rw-rw-rw-   0        0        0     1198 2018-10-16 17:50:48.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/__init__.pyc
-drwxrwxrwx   0        0        0        0 2019-02-13 16:03:00.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/__pycache__/
--rw-rw-rw-   0        0        0      954 2018-10-10 15:17:04.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      955 2019-02-13 15:54:09.000000 scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/__pycache__/__init__.cpython-37.pyc
-drwxrwxrwx   0        0        0        0 2019-02-13 16:03:01.000000 scanimage-tiff-reader-1.4.1/src/scanimage_tiff_reader.egg-info/
--rw-rw-rw-   0        0        0     3274 2019-02-13 16:02:57.000000 scanimage-tiff-reader-1.4.1/src/scanimage_tiff_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2019-02-13 16:02:57.000000 scanimage-tiff-reader-1.4.1/src/scanimage_tiff_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-02-13 16:02:57.000000 scanimage-tiff-reader-1.4.1/src/scanimage_tiff_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2019-02-13 16:02:57.000000 scanimage-tiff-reader-1.4.1/src/scanimage_tiff_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2019-02-13 16:02:57.000000 scanimage-tiff-reader-1.4.1/src/scanimage_tiff_reader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/
+-rw-rw-rw-   0        0        0      570 2023-05-16 20:53:57.000000 scanimage-tiff-reader-1.4.1.3/LICENSE
+-rw-rw-rw-   0        0        0      119 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3779 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2076 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/README.rst
+-rw-rw-rw-   0        0        0     1330 2023-05-19 19:23:47.000000 scanimage-tiff-reader-1.4.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       69 2023-05-19 18:45:13.000000 scanimage-tiff-reader-1.4.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/
+-rw-rw-rw-   0        0        0    13401 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/
+-rw-rw-rw-   0        0        0      708 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/
+drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/lib/
+-rw-rw-rw-   0        0        0   379788 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/lib/libScanImageTiffReaderAPI.so
+drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/
+drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/lib/
+-rw-rw-rw-   0        0        0  2409728 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/lib/libScanImageTiffReaderAPI.so
+drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/
+drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/lib/
+-rw-rw-rw-   0        0        0   538112 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/lib/ScanImageTiffReaderAPI.dll
+-rw-rw-rw-   0        0        0      919 2023-05-10 16:52:17.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/
+-rw-rw-rw-   0        0        0     3779 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/top_level.txt
```

### Comparing `scanimage-tiff-reader-1.4.1/README.rst` & `scanimage-tiff-reader-1.4.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/__init__.py` & `scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/__init__.py`

 * *Files identical despite different names*

### Comparing `scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/README.md` & `scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/README.md`

 * *Files identical despite different names*

### Comparing `scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/lib/libScanImageTiffReaderAPI.so` & `scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/lib/libScanImageTiffReaderAPI.so`

 * *Files identical despite different names*

### Comparing `scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/lib/libScanImageTiffReaderAPI.so` & `scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/lib/libScanImageTiffReaderAPI.so`

 * *Files identical despite different names*

### Comparing `scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/lib/ScanImageTiffReaderAPI.dll` & `scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/lib/ScanImageTiffReaderAPI.dll`

 * *Files identical despite different names*

### Comparing `scanimage-tiff-reader-1.4.1/src/ScanImageTiffReader/external/__init__.py` & `scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/__init__.py`

 * *Files identical despite different names*

