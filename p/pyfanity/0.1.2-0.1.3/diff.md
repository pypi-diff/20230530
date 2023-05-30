# Comparing `tmp/pyfanity-0.1.2.tar.gz` & `tmp/pyfanity-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfanity-0.1.2.tar", max compression
+gzip compressed data, was "pyfanity-0.1.3.tar", max compression
```

## Comparing `pyfanity-0.1.2.tar` & `pyfanity-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0     1086 2023-05-05 06:59:53.587619 pyfanity-0.1.2/LICENSE
--rw-r--r--   0        0        0      447 2023-05-06 00:59:15.034621 pyfanity-0.1.2/pyfanity/__init__.py
--rw-r--r--   0        0        0       63 2023-05-05 22:11:06.255231 pyfanity-0.1.2/pyfanity/example.py
--rw-r--r--   0        0        0      954 2023-05-06 01:08:24.402629 pyfanity-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      174 2023-05-05 06:26:08.923618 pyfanity-0.1.2/README.md
--rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 pyfanity-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-05-05 06:59:53.587619 pyfanity-0.1.3/LICENSE
+-rw-r--r--   0        0        0      475 2023-05-06 07:30:51.703415 pyfanity-0.1.3/pyfanity/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-06 06:07:00.027615 pyfanity-0.1.3/pyfanity/falseprofanities.py
+-rw-r--r--   0        0        0      989 2023-05-08 22:20:24.930730 pyfanity-0.1.3/pyfanity/profanities.py
+-rw-r--r--   0        0        0     2920 2023-05-30 20:57:21.135725 pyfanity-0.1.3/pyfanity/pyfanity.py
+-rw-r--r--   0        0        0      623 2023-05-08 22:20:24.931729 pyfanity-0.1.3/pyfanity/replacements.py
+-rw-r--r--   0        0        0      180 2023-05-08 22:40:47.968363 pyfanity-0.1.3/pyfanity/test.py
+-rw-r--r--   0        0        0       96 2023-05-08 22:42:54.960878 pyfanity-0.1.3/pyfanity/testing.py
+-rw-r--r--   0        0        0      998 2023-05-30 21:09:36.575548 pyfanity-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-05-05 06:26:08.923618 pyfanity-0.1.3/README.md
+-rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 pyfanity-0.1.3/PKG-INFO
```

### Comparing `pyfanity-0.1.2/LICENSE` & `pyfanity-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfanity-0.1.2/pyproject.toml` & `pyfanity-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "pyfanity"
-version = "0.1.2"
+version = "0.1.3"
 description = "A simple and light weight profanity filter package."
-authors = ["bourrasque <stampixel@pm.me>"]
+authors = ["bourrasque <stampixel@pm.me>", "Blueblitz135 <aidanleung135@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "pyfanity"}]
+packages = [{ include = "pyfanity" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `pyfanity-0.1.2/PKG-INFO` & `pyfanity-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfanity
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple and light weight profanity filter package.
 License: MIT
 Keywords: feed,reader,tutorial
 Author: bourrasque
 Author-email: stampixel@pm.me
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -15,18 +15,14 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 
 # Example Package
 
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
```

