# Comparing `tmp/mlops-ai-1.0.0.tar.gz` & `tmp/mlops-ai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops-ai-1.0.0.tar", last modified: Tue May 30 11:50:29 2023, max compression
+gzip compressed data, was "mlops-ai-1.0.1.tar", last modified: Tue May 30 13:02:24 2023, max compression
```

## Comparing `mlops-ai-1.0.0.tar` & `mlops-ai-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 11:50:29.534586 mlops-ai-1.0.0/
--rw-rw-rw-   0        0        0     6123 2023-05-30 11:50:29.533586 mlops-ai-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5562 2023-05-30 07:32:36.000000 mlops-ai-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 11:50:29.526586 mlops-ai-1.0.0/mlops/
--rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.0.0/mlops/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.0.0/mlops/monitoring.py
--rw-rw-rw-   0        0        0     8387 2023-05-25 19:35:05.000000 mlops-ai-1.0.0/mlops/tracking.py
-drwxrwxrwx   0        0        0        0 2023-05-30 11:50:29.532586 mlops-ai-1.0.0/mlops_ai.egg-info/
--rw-rw-rw-   0        0        0     6123 2023-05-30 11:50:29.000000 mlops-ai-1.0.0/mlops_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-30 11:50:29.000000 mlops-ai-1.0.0/mlops_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 11:50:29.000000 mlops-ai-1.0.0/mlops_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 11:50:29.000000 mlops-ai-1.0.0/mlops_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 11:50:29.000000 mlops-ai-1.0.0/mlops_ai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 11:50:29.534586 mlops-ai-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      986 2023-05-30 11:48:39.000000 mlops-ai-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:02:24.199574 mlops-ai-1.0.1/
+-rw-rw-rw-   0        0        0     6123 2023-05-30 13:02:24.199574 mlops-ai-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5562 2023-05-30 07:32:36.000000 mlops-ai-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 13:02:24.184574 mlops-ai-1.0.1/mlops/
+-rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.0.1/mlops/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:02:24.186574 mlops-ai-1.0.1/mlops/config/
+-rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.0.1/mlops/config/__init__.py
+-rw-rw-rw-   0        0        0      614 2023-05-04 07:18:08.000000 mlops-ai-1.0.1/mlops/config/config.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:02:24.189574 mlops-ai-1.0.1/mlops/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-05-09 21:55:11.000000 mlops-ai-1.0.1/mlops/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-05-09 21:55:11.000000 mlops-ai-1.0.1/mlops/exceptions/iteration.py
+-rw-rw-rw-   0        0        0      637 2023-05-17 16:50:20.000000 mlops-ai-1.0.1/mlops/exceptions/tracking.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.0.1/mlops/monitoring.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:02:24.192574 mlops-ai-1.0.1/mlops/src/
+-rw-rw-rw-   0        0        0        0 2023-05-04 07:18:08.000000 mlops-ai-1.0.1/mlops/src/__init__.py
+-rw-rw-rw-   0        0        0     1623 2023-05-25 19:35:05.000000 mlops-ai-1.0.1/mlops/src/dataset.py
+-rw-rw-rw-   0        0        0     4045 2023-05-25 19:35:05.000000 mlops-ai-1.0.1/mlops/src/iteration.py
+-rw-rw-rw-   0        0        0     8387 2023-05-25 19:35:05.000000 mlops-ai-1.0.1/mlops/tracking.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:02:24.198574 mlops-ai-1.0.1/mlops_ai.egg-info/
+-rw-rw-rw-   0        0        0     6123 2023-05-30 13:02:24.000000 mlops-ai-1.0.1/mlops_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2023-05-30 13:02:24.000000 mlops-ai-1.0.1/mlops_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 13:02:24.000000 mlops-ai-1.0.1/mlops_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 13:02:24.000000 mlops-ai-1.0.1/mlops_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 13:02:24.000000 mlops-ai-1.0.1/mlops_ai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 13:02:24.199574 mlops-ai-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1007 2023-05-30 13:02:19.000000 mlops-ai-1.0.1/setup.py
```

### Comparing `mlops-ai-1.0.0/PKG-INFO` & `mlops-ai-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops-ai
-Version: 1.0.0
+Version: 1.0.1
 Summary: Mlops-ai library for managing machine learning projects, experiments, iterations and datasets.
 Author: Kacper Pękalski, Kajetan Szal, Jędrzej Rybczyński
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mlops-ai-1.0.0/README.md` & `mlops-ai-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.0.0/mlops/tracking.py` & `mlops-ai-1.0.1/mlops/tracking.py`

 * *Files identical despite different names*

### Comparing `mlops-ai-1.0.0/mlops_ai.egg-info/PKG-INFO` & `mlops-ai-1.0.1/mlops_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops-ai
-Version: 1.0.0
+Version: 1.0.1
 Summary: Mlops-ai library for managing machine learning projects, experiments, iterations and datasets.
 Author: Kacper Pękalski, Kajetan Szal, Jędrzej Rybczyński
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mlops-ai-1.0.0/setup.py` & `mlops-ai-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import pathlib
-from setuptools import setup
+from setuptools import setup, find_packages
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE/"README.md").read_text()
 
 setup(
    name="mlops-ai",
-   version="1.0.0",
+   version="1.0.1",
    description="Mlops-ai library for managing machine learning projects, experiments, iterations and datasets.",
    long_description=README,
    long_description_content_type="text/markdown",
    URL="https://github.com/kajetsz/mlops/tree/main/library",
    author="Kacper Pękalski, Kajetan Szal, Jędrzej Rybczyński",
    license="Apache License 2.0",
    classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
 
    ],
-   packages=["mlops"],
+   packages=find_packages(),
    includepackagedata=True,
    install_requires=["requests"],
  )
```

