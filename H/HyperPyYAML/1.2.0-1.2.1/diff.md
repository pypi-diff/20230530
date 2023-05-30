# Comparing `tmp/HyperPyYAML-1.2.0.tar.gz` & `tmp/HyperPyYAML-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HyperPyYAML-1.2.0.tar", last modified: Fri Mar 31 13:28:27 2023, max compression
+gzip compressed data, was "HyperPyYAML-1.2.1.tar", last modified: Tue May 30 14:03:24 2023, max compression
```

## Comparing `HyperPyYAML-1.2.0.tar` & `HyperPyYAML-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pplantinga  (1000) pplantinga  (1000)        0 2023-03-31 13:28:27.907717 HyperPyYAML-1.2.0/
-drwxr-xr-x   0 pplantinga  (1000) pplantinga  (1000)        0 2023-03-31 13:28:27.904384 HyperPyYAML-1.2.0/HyperPyYAML.egg-info/
--rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)     7582 2023-03-31 13:28:27.000000 HyperPyYAML-1.2.0/HyperPyYAML.egg-info/PKG-INFO
--rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)      268 2023-03-31 13:28:27.000000 HyperPyYAML-1.2.0/HyperPyYAML.egg-info/SOURCES.txt
--rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)        1 2023-03-31 13:28:27.000000 HyperPyYAML-1.2.0/HyperPyYAML.egg-info/dependency_links.txt
--rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)       32 2023-03-31 13:28:27.000000 HyperPyYAML-1.2.0/HyperPyYAML.egg-info/requires.txt
--rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)       12 2023-03-31 13:28:27.000000 HyperPyYAML-1.2.0/HyperPyYAML.egg-info/top_level.txt
--rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)    11357 2022-04-18 14:42:12.000000 HyperPyYAML-1.2.0/LICENSE
--rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)     7582 2023-03-31 13:28:27.907717 HyperPyYAML-1.2.0/PKG-INFO
--rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)     7163 2023-03-31 13:01:54.000000 HyperPyYAML-1.2.0/README.md
-drwxr-xr-x   0 pplantinga  (1000) pplantinga  (1000)        0 2023-03-31 13:28:27.904384 HyperPyYAML-1.2.0/hyperpyyaml/
--rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)      581 2022-04-18 14:42:12.000000 HyperPyYAML-1.2.0/hyperpyyaml/__init__.py
--rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)    24585 2023-03-31 13:10:57.000000 HyperPyYAML-1.2.0/hyperpyyaml/core.py
--rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)       38 2023-03-31 13:28:27.907717 HyperPyYAML-1.2.0/setup.cfg
--rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)      696 2023-03-31 13:11:53.000000 HyperPyYAML-1.2.0/setup.py
-drwxr-xr-x   0 pplantinga  (1000) pplantinga  (1000)        0 2023-03-31 13:28:27.904384 HyperPyYAML-1.2.0/tests/
--rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)     7529 2023-03-31 13:10:57.000000 HyperPyYAML-1.2.0/tests/test_hyperyaml.py
+drwxr-xr-x   0 pplantinga  (1000) pplantinga  (1000)        0 2023-05-30 14:03:24.646307 HyperPyYAML-1.2.1/
+drwxr-xr-x   0 pplantinga  (1000) pplantinga  (1000)        0 2023-05-30 14:03:24.642973 HyperPyYAML-1.2.1/HyperPyYAML.egg-info/
+-rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)     7582 2023-05-30 14:03:24.000000 HyperPyYAML-1.2.1/HyperPyYAML.egg-info/PKG-INFO
+-rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)      268 2023-05-30 14:03:24.000000 HyperPyYAML-1.2.1/HyperPyYAML.egg-info/SOURCES.txt
+-rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)        1 2023-05-30 14:03:24.000000 HyperPyYAML-1.2.1/HyperPyYAML.egg-info/dependency_links.txt
+-rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)       42 2023-05-30 14:03:24.000000 HyperPyYAML-1.2.1/HyperPyYAML.egg-info/requires.txt
+-rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)       12 2023-05-30 14:03:24.000000 HyperPyYAML-1.2.1/HyperPyYAML.egg-info/top_level.txt
+-rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)    11357 2022-04-18 14:42:12.000000 HyperPyYAML-1.2.1/LICENSE
+-rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)     7582 2023-05-30 14:03:24.646307 HyperPyYAML-1.2.1/PKG-INFO
+-rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)     7163 2023-03-31 13:01:54.000000 HyperPyYAML-1.2.1/README.md
+drwxr-xr-x   0 pplantinga  (1000) pplantinga  (1000)        0 2023-05-30 14:03:24.642973 HyperPyYAML-1.2.1/hyperpyyaml/
+-rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)      581 2022-04-18 14:42:12.000000 HyperPyYAML-1.2.1/hyperpyyaml/__init__.py
+-rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)    24585 2023-03-31 13:10:57.000000 HyperPyYAML-1.2.1/hyperpyyaml/core.py
+-rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)       38 2023-05-30 14:03:24.646307 HyperPyYAML-1.2.1/setup.cfg
+-rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)      707 2023-05-30 13:58:48.000000 HyperPyYAML-1.2.1/setup.py
+drwxr-xr-x   0 pplantinga  (1000) pplantinga  (1000)        0 2023-05-30 14:03:24.642973 HyperPyYAML-1.2.1/tests/
+-rw-r--r--   0 pplantinga  (1000) pplantinga  (1000)     7529 2023-03-31 13:10:57.000000 HyperPyYAML-1.2.1/tests/test_hyperyaml.py
```

### Comparing `HyperPyYAML-1.2.0/HyperPyYAML.egg-info/PKG-INFO` & `HyperPyYAML-1.2.1/HyperPyYAML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperPyYAML
-Version: 1.2.0
+Version: 1.2.1
 Summary: Extensions to YAML syntax for better python interaction
 Home-page: https://github.com/speechbrain/HyperPyYAML
 Author: Peter Plantinga, Aku Rouhe
 Author-email: speechbrain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `HyperPyYAML-1.2.0/LICENSE` & `HyperPyYAML-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HyperPyYAML-1.2.0/PKG-INFO` & `HyperPyYAML-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperPyYAML
-Version: 1.2.0
+Version: 1.2.1
 Summary: Extensions to YAML syntax for better python interaction
 Home-page: https://github.com/speechbrain/HyperPyYAML
 Author: Peter Plantinga, Aku Rouhe
 Author-email: speechbrain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `HyperPyYAML-1.2.0/README.md` & `HyperPyYAML-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `HyperPyYAML-1.2.0/hyperpyyaml/__init__.py` & `HyperPyYAML-1.2.1/hyperpyyaml/__init__.py`

 * *Files identical despite different names*

### Comparing `HyperPyYAML-1.2.0/hyperpyyaml/core.py` & `HyperPyYAML-1.2.1/hyperpyyaml/core.py`

 * *Files identical despite different names*

### Comparing `HyperPyYAML-1.2.0/setup.py` & `HyperPyYAML-1.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import setuptools
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="HyperPyYAML",
-    version="1.2.0",
+    version="1.2.1",
     description="Extensions to YAML syntax for better python interaction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/speechbrain/HyperPyYAML",
     author="Peter Plantinga, Aku Rouhe",
     author_email="speechbrain@gmail.com",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
     ],
     packages=["hyperpyyaml"],
-    install_requires=["pyyaml>=5.1", "ruamel.yaml>=0.17.8"],
+    install_requires=["pyyaml>=5.1", "ruamel.yaml>=0.17.8, <=0.17.28"],
 )
```

### Comparing `HyperPyYAML-1.2.0/tests/test_hyperyaml.py` & `HyperPyYAML-1.2.1/tests/test_hyperyaml.py`

 * *Files identical despite different names*

