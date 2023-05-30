# Comparing `tmp/SecuriPy-1.0.5.tar.gz` & `tmp/SecuriPy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecuriPy-1.0.5.tar", last modified: Mon May 29 17:32:27 2023, max compression
+gzip compressed data, was "SecuriPy-1.0.6.tar", last modified: Tue May 30 07:14:15 2023, max compression
```

## Comparing `SecuriPy-1.0.5.tar` & `SecuriPy-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 17:32:27.832889 SecuriPy-1.0.5/
--rw-rw-rw-   0        0        0     3594 2023-05-29 17:32:27.828902 SecuriPy-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2998 2023-05-27 06:04:44.000000 SecuriPy-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 17:32:27.823913 SecuriPy-1.0.5/SecuriPy.egg-info/
--rw-rw-rw-   0        0        0     3594 2023-05-29 17:32:27.000000 SecuriPy-1.0.5/SecuriPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-05-29 17:32:27.000000 SecuriPy-1.0.5/SecuriPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 17:32:27.000000 SecuriPy-1.0.5/SecuriPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 17:32:27.000000 SecuriPy-1.0.5/SecuriPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1643 2023-05-29 17:28:25.000000 SecuriPy-1.0.5/SecuriPy.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 17:32:27.832889 SecuriPy-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      879 2023-05-29 17:28:54.000000 SecuriPy-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:14:15.271223 SecuriPy-1.0.6/
+-rw-rw-rw-   0        0        0     3594 2023-05-30 07:14:15.269221 SecuriPy-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2998 2023-05-27 06:04:44.000000 SecuriPy-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 07:14:15.265296 SecuriPy-1.0.6/SecuriPy.egg-info/
+-rw-rw-rw-   0        0        0     3594 2023-05-30 07:14:14.000000 SecuriPy-1.0.6/SecuriPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-05-30 07:14:14.000000 SecuriPy-1.0.6/SecuriPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 07:14:14.000000 SecuriPy-1.0.6/SecuriPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 07:14:14.000000 SecuriPy-1.0.6/SecuriPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4665 2023-05-30 07:13:27.000000 SecuriPy-1.0.6/SecuriPy.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 07:14:15.271223 SecuriPy-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-05-30 07:13:54.000000 SecuriPy-1.0.6/setup.py
```

### Comparing `SecuriPy-1.0.5/PKG-INFO` & `SecuriPy-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-1.0.5/README.md` & `SecuriPy-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `SecuriPy-1.0.5/SecuriPy.egg-info/PKG-INFO` & `SecuriPy-1.0.6/SecuriPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-1.0.5/setup.py` & `SecuriPy-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SecuriPy",
-    version="1.0.5",
+    version="1.0.6",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Encrypter and Decrypter of Readable messages Using Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/SecuriPy",
     project_urls={
```

