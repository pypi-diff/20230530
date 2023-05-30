# Comparing `tmp/pycontext-lib-1.0.0.tar.gz` & `tmp/pycontext-lib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycontext-lib-1.0.0.tar", last modified: Mon May 29 17:19:05 2023, max compression
+gzip compressed data, was "pycontext-lib-1.0.1.tar", last modified: Tue May 30 02:17:31 2023, max compression
```

## Comparing `pycontext-lib-1.0.0.tar` & `pycontext-lib-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 17:19:05.333530 pycontext-lib-1.0.0/
--rw-rw-rw-   0        0        0     1100 2023-05-29 17:14:53.000000 pycontext-lib-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1937 2023-05-29 17:19:05.332466 pycontext-lib-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      137 2023-05-29 17:18:43.000000 pycontext-lib-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 17:19:05.314171 pycontext-lib-1.0.0/context/
--rw-rw-rw-   0        0        0     5251 2022-11-23 02:38:19.000000 pycontext-lib-1.0.0/context/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 17:19:05.329937 pycontext-lib-1.0.0/pycontext_lib.egg-info/
--rw-rw-rw-   0        0        0     1937 2023-05-29 17:19:05.000000 pycontext-lib-1.0.0/pycontext_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-05-29 17:19:05.000000 pycontext-lib-1.0.0/pycontext_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 17:19:05.000000 pycontext-lib-1.0.0/pycontext_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-05-29 17:19:05.000000 pycontext-lib-1.0.0/pycontext_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-05-29 17:19:05.000000 pycontext-lib-1.0.0/pycontext_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      724 2023-05-29 17:18:21.000000 pycontext-lib-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 17:19:05.333530 pycontext-lib-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 02:17:31.444363 pycontext-lib-1.0.1/
+-rw-rw-rw-   0        0        0     1100 2023-05-29 17:14:53.000000 pycontext-lib-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1967 2023-05-30 02:17:31.443357 pycontext-lib-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      137 2023-05-29 17:18:43.000000 pycontext-lib-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 02:17:31.419617 pycontext-lib-1.0.1/context/
+-rw-rw-rw-   0        0        0     5251 2022-11-23 02:38:19.000000 pycontext-lib-1.0.1/context/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:17:31.440218 pycontext-lib-1.0.1/pycontext_lib.egg-info/
+-rw-rw-rw-   0        0        0     1967 2023-05-30 02:17:31.000000 pycontext-lib-1.0.1/pycontext_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-05-30 02:17:31.000000 pycontext-lib-1.0.1/pycontext_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 02:17:31.000000 pycontext-lib-1.0.1/pycontext_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-05-30 02:17:31.000000 pycontext-lib-1.0.1/pycontext_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 02:17:31.000000 pycontext-lib-1.0.1/pycontext_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      762 2023-05-30 02:17:17.000000 pycontext-lib-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 02:17:31.445585 pycontext-lib-1.0.1/setup.cfg
```

### Comparing `pycontext-lib-1.0.0/LICENSE` & `pycontext-lib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycontext-lib-1.0.0/PKG-INFO` & `pycontext-lib-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycontext-lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Lots of properties that help with program context!
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://github.com/User0332/pycontext
+Keywords: context,properties
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pycontext-lib-1.0.0/context/__init__.py` & `pycontext-lib-1.0.1/context/__init__.py`

 * *Files identical despite different names*

### Comparing `pycontext-lib-1.0.0/pycontext_lib.egg-info/PKG-INFO` & `pycontext-lib-1.0.1/pycontext_lib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycontext-lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Lots of properties that help with program context!
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://github.com/User0332/pycontext
+Keywords: context,properties
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pycontext-lib-1.0.0/pyproject.toml` & `pycontext-lib-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pycontext-lib"
-version = "1.0.0"
+version = "1.0.1"
 description = "Lots of properties that help with program context!"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3",
     "Operating System :: OS Independent"
 ]
 requires-python = ">= 3.9"
+keywords = ["context", "properties"]
 
 [project.urls]
 Homepage = "https://github.com/User0332/pycontext"
 
 [project.scripts]
 webpy = "webpy.__main__:main"
 webpy-framework = "webpy.__main__:main"
```

