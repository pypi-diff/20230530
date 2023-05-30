# Comparing `tmp/pathml-2.1.0.tar.gz` & `tmp/pathml-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathml-2.1.0.tar", last modified: Fri Apr 22 21:23:37 2022, max compression
+gzip compressed data, was "pathml-2.1.1.tar", last modified: Tue May 30 03:02:00 2023, max compression
```

## Comparing `pathml-2.1.0.tar` & `pathml-2.1.1.tar`

### file list

```diff
@@ -1,45 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-22 21:23:37.339622 pathml-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (116)    18092 2022-04-22 21:23:27.000000 pathml-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     8855 2022-04-22 21:23:37.339622 pathml-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7658 2022-04-22 21:23:27.000000 pathml-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-22 21:23:37.335621 pathml-2.1.0/pathml/
--rw-r--r--   0 runner    (1001) docker     (116)      271 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3155 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/_logging.py
--rw-r--r--   0 runner    (1001) docker     (116)      124 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-22 21:23:37.339622 pathml-2.1.0/pathml/core/
--rw-r--r--   0 runner    (1001) docker     (116)      464 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    14207 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/core/h5managers.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3284 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/core/masks.py
--rw-r--r--   0 runner    (1001) docker     (116)    38800 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/core/slide_backends.py
--rw-r--r--   0 runner    (1001) docker     (116)    25941 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/core/slide_data.py
--rw-r--r--   0 runner    (1001) docker     (116)     3178 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/core/slide_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)     5225 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/core/slide_types.py
--rw-r--r--   0 runner    (1001) docker     (116)     7182 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/core/tile.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2945 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/core/tiles.py
--rw-r--r--   0 runner    (1001) docker     (116)     2983 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-22 21:23:37.339622 pathml-2.1.0/pathml/datasets/
--rw-r--r--   0 runner    (1001) docker     (116)      184 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      598 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/datasets/base_data_module.py
--rw-r--r--   0 runner    (1001) docker     (116)     5142 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/datasets/deepfocus.py
--rw-r--r--   0 runner    (1001) docker     (116)    16383 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/datasets/pannuke.py
--rw-r--r--   0 runner    (1001) docker     (116)     1204 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-22 21:23:37.339622 pathml-2.1.0/pathml/ml/
--rw-r--r--   0 runner    (1001) docker     (116)      210 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3117 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/ml/dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)    34076 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/ml/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (116)     6392 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/ml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-22 21:23:37.339622 pathml-2.1.0/pathml/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (116)      599 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1722 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/preprocessing/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (116)     3920 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/preprocessing/tiling.py
--rw-r--r--   0 runner    (1001) docker     (116)    64111 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/preprocessing/transforms.py
--rw-r--r--   0 runner    (1001) docker     (116)    11258 2022-04-22 21:23:27.000000 pathml-2.1.0/pathml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-22 21:23:37.335621 pathml-2.1.0/pathml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8855 2022-04-22 21:23:36.000000 pathml-2.1.0/pathml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      869 2022-04-22 21:23:37.000000 pathml-2.1.0/pathml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-22 21:23:36.000000 pathml-2.1.0/pathml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      210 2022-04-22 21:23:37.000000 pathml-2.1.0/pathml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-04-22 21:23:37.000000 pathml-2.1.0/pathml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      212 2022-04-22 21:23:27.000000 pathml-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-04-22 21:23:37.339622 pathml-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1936 2022-04-22 21:23:27.000000 pathml-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:02:00.300094 pathml-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-30 03:01:51.000000 pathml-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-05-30 03:02:00.300094 pathml-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-05-30 03:01:51.000000 pathml-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:02:00.292094 pathml-2.1.1/pathml/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:02:00.296094 pathml-2.1.1/pathml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14050 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/core/h5managers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3212 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/core/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38827 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/core/slide_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26275 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/core/slide_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/core/slide_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/core/slide_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/core/tile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2871 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/core/tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:02:00.296094 pathml-2.1.1/pathml/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/datasets/base_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/datasets/deepfocus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/datasets/pannuke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:02:00.296094 pathml-2.1.1/pathml/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/ml/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34101 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/ml/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/ml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:02:00.296094 pathml-2.1.1/pathml/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/preprocessing/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/preprocessing/tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64160 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/preprocessing/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-05-30 03:01:51.000000 pathml-2.1.1/pathml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:02:00.292094 pathml-2.1.1/pathml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-05-30 03:02:00.000000 pathml-2.1.1/pathml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-30 03:02:00.000000 pathml-2.1.1/pathml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 03:02:00.000000 pathml-2.1.1/pathml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-30 03:02:00.000000 pathml-2.1.1/pathml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 03:02:00.000000 pathml-2.1.1/pathml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-30 03:01:51.000000 pathml-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 03:02:00.300094 pathml-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-30 03:01:51.000000 pathml-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:02:00.300094 pathml-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-30 03:01:51.000000 pathml-2.1.1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-30 03:01:51.000000 pathml-2.1.1/tests/test_manuscript_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-30 03:01:51.000000 pathml-2.1.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-30 03:01:51.000000 pathml-2.1.1/tests/test_version.py
```

### Comparing `pathml-2.1.0/LICENSE` & `pathml-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pathml-2.1.0/PKG-INFO` & `pathml-2.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,31 @@
-Metadata-Version: 2.1
-Name: pathml
-Version: 2.1.0
-Summary: Tools for computational pathology
-Author: Jacob Rosenthal, Ryan Carelli et al.
-Author-email: PathML@dfci.harvard.edu
-License: UNKNOWN
-Project-URL: Documentation, https://pathml.readthedocs.io/en/stable
-Project-URL: Source Code, https://github.com/Dana-Farber-AIOS/pathml
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Framework :: Sphinx
-Classifier: Framework :: Pytest
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/logo.png width="300"> 
-
-<img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/overview.png width="750">
+🤖🔬 **PathML: Tools for computational pathology**
 
+[![Downloads](https://pepy.tech/badge/pathml)](https://pepy.tech/project/pathml)
 [![Documentation Status](https://readthedocs.org/projects/pathml/badge/?version=latest)](https://pathml.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/gh/Dana-Farber-AIOS/pathml/branch/master/graph/badge.svg?token=UHSQPTM28Y)](https://codecov.io/gh/Dana-Farber-AIOS/pathml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://img.shields.io/pypi/v/pathml)](https://pypi.org/project/pathml/)
-[![Downloads](https://pepy.tech/badge/pathml)](https://pepy.tech/project/pathml)
-[![codecov](https://codecov.io/gh/Dana-Farber-AIOS/pathml/branch/master/graph/badge.svg?token=UHSQPTM28Y)](https://codecov.io/gh/Dana-Farber-AIOS/pathml)
+
+⭐ **PathML objective is to lower the barrier to entry to digital pathology**
+
+Imaging datasets in cancer research are growing exponentially in both quantity and information density. These massive datasets may enable derivation of insights for cancer research and clinical care, but only if researchers are equipped with the tools to leverage advanced computational analysis approaches such as machine learning and artificial intelligence. In this work, we highlight three themes to guide development of such computational tools: scalability, standardization, and ease of use. We then apply these principles to develop PathML, a general-purpose research toolkit for computational pathology. We describe the design of the PathML framework and demonstrate applications in diverse use cases. 
+
+🚀 **The fastest way to get started?**
+
+    docker pull pathml/pathml && docker run -it -p 8888:8888 pathml/pathml
 
 | Branch | Test status   |
 | ------ | ------------- |
 | master | ![tests](https://github.com/Dana-Farber-AIOS/pathml/actions/workflows/tests-conda.yml/badge.svg?branch=master) |
 | dev    | ![tests](https://github.com/Dana-Farber-AIOS/pathml/actions/workflows/tests-conda.yml/badge.svg?branch=dev) |
 
-An open-source toolkit for computational pathology and machine learning.
+<img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/logo.png width="300"> 
+
+<img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/overview.png width="750">
 
 **View [documentation](https://pathml.readthedocs.io/en/latest/)**
 
 :construction: the `dev` branch is under active development, with experimental features, bug fixes, and refactors that may happen at any time! 
 Stable versions are available as tagged releases on GitHub, or as versioned releases on PyPI
 
 # Installation
@@ -115,14 +96,16 @@
 pip install -e .
 ````
 
 ## Installation option 3: Docker
 
 First, download or build the PathML Docker container:
 
+![pathml-docker-installation](https://user-images.githubusercontent.com/25375373/191053363-477497a1-9804-48f3-91f9-767dc7f859ed.gif)
+
 - Option A: download PathML container from Docker Hub
    ````
    docker pull pathml/pathml:latest
    ````
   Optionally specify a tag for a particular version, e.g. `docker pull pathml/pathml:2.0.2`. To view possible tags, 
   please refer to the [PathML DockerHub page](https://hub.docker.com/r/pathml/pathml).
   
@@ -146,14 +129,31 @@
 
 Note that the docker container requires extra configurations to use with GPU.  
 Note that these instructions assume that there are no other processes using port 8888.
 
 Please refer to the `Docker run` [documentation](https://docs.docker.com/engine/reference/run/) for further instructions
 on accessing the container, e.g. for mounting volumes to access files on a local machine from within the container.
 
+## Option 4: Google Colab
+
+To get PathML running in a Colab environment:
+
+````
+!pip install openslide-python
+!apt-get install openslide-tools
+!apt-get install openjdk-8-jdk-headless -qq > /dev/null
+os.environ["JAVA_HOME"] = "/usr/lib/jvm/java-8-openjdk-amd64"
+!update-alternatives --set java /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java
+!java -version
+!pip install pathml
+````
+
+*Thanks to all of our open-source collaborators for helping maintain these installation instructions!*  
+*Please open an issue for any bugs or other problems during installation process.*
+
 ## CUDA
 
 To use GPU acceleration for model training or other tasks, you must install CUDA. 
 This guide should work, but for the most up-to-date instructions, refer to the [official PyTorch installation instructions](https://pytorch.org/get-started/locally/).
 
 Check the version of CUDA:
 ````
@@ -212,30 +212,52 @@
 * Sharing trained model parameters
 * Sharing ``PathML`` with colleagues, students, etc.
 
 See [contributing](https://github.com/Dana-Farber-AIOS/pathml/blob/master/CONTRIBUTING.rst) for more details.
 
 # Citing
 
-If you use `PathML` in your work, please cite our paper:
+If you use `PathML` please cite:
+
+- [**J. Rosenthal et al., "Building tools for machine learning and artificial intelligence in cancer research: best practices and a case study with the PathML toolkit for computational pathology." Molecular Cancer Research, 2022.**](https://doi.org/10.1158/1541-7786.MCR-21-0665)
+
+So far, PathML was used in the following manuscripts: 
 
-Rosenthal J, Carelli R, Omar M, Brundage D, Halbert E, Nyman J, Hari SN, Van Allen EM, Marchionni L, Umeton R, Loda M. 
-Building tools for machine learning and artificial intelligence in cancer research: best practices and a case study 
-with the PathML toolkit for computational pathology. *Molecular Cancer Research*, 2021. 
-DOI: [10.1158/1541-7786.MCR-21-0665](https://doi.org/10.1158/1541-7786.MCR-21-0665)
+- [J. Linares et al. **Molecular Cell** 2021](https://www.cell.com/molecular-cell/fulltext/S1097-2765(21)00729-2)
+- [A. Shmatko et al. **Nature Cancer** 2022](https://www.nature.com/articles/s43018-022-00436-4)
+- [J. Pocock et al. **Nature Communications Medicine** 2022](https://www.nature.com/articles/s43856-022-00186-5)
+- [S. Orsulic et al. **Frontiers in Oncology** 2022](https://www.frontiersin.org/articles/10.3389/fonc.2022.924945/full)
+- [D. Brundage et al. **arXiv** 2022](https://arxiv.org/abs/2203.13888)
+- [A. Marcolini et al. **SoftwareX** 2022](https://www.sciencedirect.com/science/article/pii/S2352711022001558)
+- [M. Rahman et al. **Bioengineering** 2022](https://www.mdpi.com/2306-5354/9/8/335)
+- [C. Lama et al. **bioRxiv** 2022](https://www.biorxiv.org/content/10.1101/2022.09.28.509751v1.full)
+- the list continues [**here 🔗 for 2023 and onwards**](https://scholar.google.com/scholar?oi=bibs&hl=en&cites=1157052756975292108)
+
+# Users
+
+<table style="border: 0px !important;"><tr><td>This is where in the world our most enthusiastic supporters are located:
+   <br/><br/>
+<img src="https://user-images.githubusercontent.com/25375373/208137141-e450aa86-8433-415a-9cc7-c4274139bdc2.png" width="500px">
+   </td><td>   
+and this is where they work:
+   <br/><br/>
+<img src="https://user-images.githubusercontent.com/25375373/208137644-f73c86d0-c5c7-4094-80d9-ea11e0edbdc5.png" width="400px">
+</td>                                                                                                                             
+</tr>
+</table>
+
+Source: https://ossinsight.io/analyze/Dana-Farber-AIOS/pathml#people
 
 # License
 
 The GNU GPL v2 version of PathML is made available via Open Source licensing. 
 The user is free to use, modify, and distribute under the terms of the GNU General Public License version 2.
 
 Commercial license options are available also.
 
 # Contact
 
 Questions? Comments? Suggestions? Get in touch!
 
-[PathML@dfci.harvard.edu](mailto:PathML@dfci.harvard.edu)
+[pathml@dfci.harvard.edu](mailto:pathml@dfci.harvard.edu)
 
 <img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/dfci_cornell_joint_logos.png width="750"> 
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pathml-2.1.0/README.md` & `pathml-2.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,56 @@
-<img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/logo.png width="300"> 
+Metadata-Version: 2.1
+Name: pathml
+Version: 2.1.1
+Summary: Tools for computational pathology
+Author: Jacob Rosenthal, Ryan Carelli et al.
+Author-email: PathML@dfci.harvard.edu
+Project-URL: Documentation, https://pathml.readthedocs.io/en/stable
+Project-URL: Source Code, https://github.com/Dana-Farber-AIOS/pathml
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Framework :: Sphinx
+Classifier: Framework :: Pytest
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-<img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/overview.png width="750">
+🤖🔬 **PathML: Tools for computational pathology**
 
+[![Downloads](https://pepy.tech/badge/pathml)](https://pepy.tech/project/pathml)
 [![Documentation Status](https://readthedocs.org/projects/pathml/badge/?version=latest)](https://pathml.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/gh/Dana-Farber-AIOS/pathml/branch/master/graph/badge.svg?token=UHSQPTM28Y)](https://codecov.io/gh/Dana-Farber-AIOS/pathml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://img.shields.io/pypi/v/pathml)](https://pypi.org/project/pathml/)
-[![Downloads](https://pepy.tech/badge/pathml)](https://pepy.tech/project/pathml)
-[![codecov](https://codecov.io/gh/Dana-Farber-AIOS/pathml/branch/master/graph/badge.svg?token=UHSQPTM28Y)](https://codecov.io/gh/Dana-Farber-AIOS/pathml)
+
+⭐ **PathML objective is to lower the barrier to entry to digital pathology**
+
+Imaging datasets in cancer research are growing exponentially in both quantity and information density. These massive datasets may enable derivation of insights for cancer research and clinical care, but only if researchers are equipped with the tools to leverage advanced computational analysis approaches such as machine learning and artificial intelligence. In this work, we highlight three themes to guide development of such computational tools: scalability, standardization, and ease of use. We then apply these principles to develop PathML, a general-purpose research toolkit for computational pathology. We describe the design of the PathML framework and demonstrate applications in diverse use cases. 
+
+🚀 **The fastest way to get started?**
+
+    docker pull pathml/pathml && docker run -it -p 8888:8888 pathml/pathml
 
 | Branch | Test status   |
 | ------ | ------------- |
 | master | ![tests](https://github.com/Dana-Farber-AIOS/pathml/actions/workflows/tests-conda.yml/badge.svg?branch=master) |
 | dev    | ![tests](https://github.com/Dana-Farber-AIOS/pathml/actions/workflows/tests-conda.yml/badge.svg?branch=dev) |
 
-An open-source toolkit for computational pathology and machine learning.
+<img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/logo.png width="300"> 
+
+<img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/overview.png width="750">
 
 **View [documentation](https://pathml.readthedocs.io/en/latest/)**
 
 :construction: the `dev` branch is under active development, with experimental features, bug fixes, and refactors that may happen at any time! 
 Stable versions are available as tagged releases on GitHub, or as versioned releases on PyPI
 
 # Installation
@@ -88,14 +121,16 @@
 pip install -e .
 ````
 
 ## Installation option 3: Docker
 
 First, download or build the PathML Docker container:
 
+![pathml-docker-installation](https://user-images.githubusercontent.com/25375373/191053363-477497a1-9804-48f3-91f9-767dc7f859ed.gif)
+
 - Option A: download PathML container from Docker Hub
    ````
    docker pull pathml/pathml:latest
    ````
   Optionally specify a tag for a particular version, e.g. `docker pull pathml/pathml:2.0.2`. To view possible tags, 
   please refer to the [PathML DockerHub page](https://hub.docker.com/r/pathml/pathml).
   
@@ -119,14 +154,31 @@
 
 Note that the docker container requires extra configurations to use with GPU.  
 Note that these instructions assume that there are no other processes using port 8888.
 
 Please refer to the `Docker run` [documentation](https://docs.docker.com/engine/reference/run/) for further instructions
 on accessing the container, e.g. for mounting volumes to access files on a local machine from within the container.
 
+## Option 4: Google Colab
+
+To get PathML running in a Colab environment:
+
+````
+!pip install openslide-python
+!apt-get install openslide-tools
+!apt-get install openjdk-8-jdk-headless -qq > /dev/null
+os.environ["JAVA_HOME"] = "/usr/lib/jvm/java-8-openjdk-amd64"
+!update-alternatives --set java /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java
+!java -version
+!pip install pathml
+````
+
+*Thanks to all of our open-source collaborators for helping maintain these installation instructions!*  
+*Please open an issue for any bugs or other problems during installation process.*
+
 ## CUDA
 
 To use GPU acceleration for model training or other tasks, you must install CUDA. 
 This guide should work, but for the most up-to-date instructions, refer to the [official PyTorch installation instructions](https://pytorch.org/get-started/locally/).
 
 Check the version of CUDA:
 ````
@@ -185,28 +237,52 @@
 * Sharing trained model parameters
 * Sharing ``PathML`` with colleagues, students, etc.
 
 See [contributing](https://github.com/Dana-Farber-AIOS/pathml/blob/master/CONTRIBUTING.rst) for more details.
 
 # Citing
 
-If you use `PathML` in your work, please cite our paper:
+If you use `PathML` please cite:
+
+- [**J. Rosenthal et al., "Building tools for machine learning and artificial intelligence in cancer research: best practices and a case study with the PathML toolkit for computational pathology." Molecular Cancer Research, 2022.**](https://doi.org/10.1158/1541-7786.MCR-21-0665)
+
+So far, PathML was used in the following manuscripts: 
+
+- [J. Linares et al. **Molecular Cell** 2021](https://www.cell.com/molecular-cell/fulltext/S1097-2765(21)00729-2)
+- [A. Shmatko et al. **Nature Cancer** 2022](https://www.nature.com/articles/s43018-022-00436-4)
+- [J. Pocock et al. **Nature Communications Medicine** 2022](https://www.nature.com/articles/s43856-022-00186-5)
+- [S. Orsulic et al. **Frontiers in Oncology** 2022](https://www.frontiersin.org/articles/10.3389/fonc.2022.924945/full)
+- [D. Brundage et al. **arXiv** 2022](https://arxiv.org/abs/2203.13888)
+- [A. Marcolini et al. **SoftwareX** 2022](https://www.sciencedirect.com/science/article/pii/S2352711022001558)
+- [M. Rahman et al. **Bioengineering** 2022](https://www.mdpi.com/2306-5354/9/8/335)
+- [C. Lama et al. **bioRxiv** 2022](https://www.biorxiv.org/content/10.1101/2022.09.28.509751v1.full)
+- the list continues [**here 🔗 for 2023 and onwards**](https://scholar.google.com/scholar?oi=bibs&hl=en&cites=1157052756975292108)
+
+# Users
+
+<table style="border: 0px !important;"><tr><td>This is where in the world our most enthusiastic supporters are located:
+   <br/><br/>
+<img src="https://user-images.githubusercontent.com/25375373/208137141-e450aa86-8433-415a-9cc7-c4274139bdc2.png" width="500px">
+   </td><td>   
+and this is where they work:
+   <br/><br/>
+<img src="https://user-images.githubusercontent.com/25375373/208137644-f73c86d0-c5c7-4094-80d9-ea11e0edbdc5.png" width="400px">
+</td>                                                                                                                             
+</tr>
+</table>
 
-Rosenthal J, Carelli R, Omar M, Brundage D, Halbert E, Nyman J, Hari SN, Van Allen EM, Marchionni L, Umeton R, Loda M. 
-Building tools for machine learning and artificial intelligence in cancer research: best practices and a case study 
-with the PathML toolkit for computational pathology. *Molecular Cancer Research*, 2021. 
-DOI: [10.1158/1541-7786.MCR-21-0665](https://doi.org/10.1158/1541-7786.MCR-21-0665)
+Source: https://ossinsight.io/analyze/Dana-Farber-AIOS/pathml#people
 
 # License
 
 The GNU GPL v2 version of PathML is made available via Open Source licensing. 
 The user is free to use, modify, and distribute under the terms of the GNU General Public License version 2.
 
 Commercial license options are available also.
 
 # Contact
 
 Questions? Comments? Suggestions? Get in touch!
 
-[PathML@dfci.harvard.edu](mailto:PathML@dfci.harvard.edu)
+[pathml@dfci.harvard.edu](mailto:pathml@dfci.harvard.edu)
 
 <img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/dfci_cornell_joint_logos.png width="750">
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pathml-2.1.0/pathml/_logging.py` & `pathml-2.1.1/pathml/_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
-from loguru import logger
 import functools
 import sys
 
+from loguru import logger
+
 
 class PathMLLogger:
     """
     Convenience methods for turning on or off and configuring logging for PathML.
     Note that this can also be achieved by interfacing with loguru directly
 
     Example::
```

### Comparing `pathml-2.1.0/pathml/core/h5managers.py` & `pathml-2.1.1/pathml/core/h5managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
-import itertools
 import os
 import tempfile
-from collections import OrderedDict
 
 import anndata
-from loguru import logger
 import h5py
 import numpy as np
+from loguru import logger
+
 import pathml.core
 import pathml.core.masks
 import pathml.core.tile
 from pathml.core.utils import readcounts
 
 
 class h5pathManager:
@@ -31,57 +30,57 @@
         self.h5reference = path
         # create temporary file for slidedata.counts
         self.countspath = tempfile.TemporaryDirectory()
         self.counts = anndata.AnnData()
         if h5path:
             assert (
                 not slidedata
-            ), f"if creating h5pathmanager from h5path, slidedata should not be required"
+            ), "if creating h5pathmanager from h5path, slidedata should not be required"
             assert check_valid_h5path_format(
                 h5path
-            ), f"h5path must conform to .h5path standard, see documentation"
+            ), "h5path must conform to .h5path standard, see documentation"
             # copy h5path into self.h5
             for ds in h5path.keys():
                 if ds in ["fields", "masks", "tiles"]:
                     h5path.copy(ds, self.h5)
                 if ds in ["counts"]:
                     h5path.copy(ds, self.h5)
                     if h5path["counts"].keys():
                         self.counts = readcounts(h5path["counts"])
                         self.counts.filename = (
                             str(self.countspath.name) + "/tmpfile.h5ad"
                         )
 
         else:
-            assert slidedata, f"must pass slidedata object to create h5path"
+            assert slidedata, "must pass slidedata object to create h5path"
             # initialize h5path file hierarchy
             # fields
             fieldsgroup = self.h5.create_group("fields")
             # name, shape, labels
             fieldsgroup.attrs["name"] = slidedata.name
             fieldsgroup.attrs["shape"] = slidedata.slide.get_image_shape()
-            labelsgroup = self.h5["fields"].create_group("labels")
+            self.h5["fields"].create_group("labels")
             if slidedata.labels:
                 for key, label in slidedata.labels.items():
                     self.h5["fields/labels"].attrs[key] = label
             # slidetype
-            slidetypegroup = self.h5["fields"].create_group("slide_type")
+            self.h5["fields"].create_group("slide_type")
             if slidedata.slide_type:
                 for key, val in slidedata.slide_type.asdict().items():
                     self.h5["fields/slide_type"].attrs[key] = val
             # tiles
             tilesgroup = self.h5.create_group("tiles")
             # initialize tile_shape with zeros
             tilesgroup.attrs["tile_shape"] = b"(0, 0)"
             # initialize stride with 0
             tilesgroup.attrs["tile_stride"] = b"(0, 0)"
             # masks
-            masksgroup = self.h5.create_group("masks")
+            self.h5.create_group("masks")
             # counts
-            countsgroup = self.h5.create_group("counts")
+            self.h5.create_group("counts")
 
         slide_type_dict = {
             key: val for key, val in self.h5["fields/slide_type"].attrs.items()
         }
         self.slide_type = pathml.core.slide_types.SlideType(**slide_type_dict)
 
     def __repr__(self):
@@ -146,15 +145,15 @@
             and self.h5["tiles"].attrs["tile_shape"] == b"(0, 0)"
         ):
             self.h5["tiles"].attrs["tile_shape"] = str(tile.image.shape).encode("utf-8")
 
         if tile.masks:
             # create a group to hold tile-level masks
             if "masks" not in self.h5["tiles"][str(tile.coords)].keys():
-                masksgroup = self.h5["tiles"][str(tile.coords)].create_group("masks")
+                self.h5["tiles"][str(tile.coords)].create_group("masks")
 
             # add tile-level masks
             for key, mask in tile.masks.items():
                 self.h5["tiles"][str(tile.coords)]["masks"].create_dataset(
                     str(key),
                     data=mask,
                     dtype="float16",
@@ -164,15 +163,15 @@
         self.h5["tiles"][str(tile.coords)].attrs["coords"] = (
             str(tile.coords) if tile.coords else 0
         )
         # add name
         self.h5["tiles"][str(tile.coords)].attrs["name"] = (
             str(tile.name) if tile.name else 0
         )
-        tilelabelsgroup = self.h5["tiles"][str(tile.coords)].create_group("labels")
+        self.h5["tiles"][str(tile.coords)].create_group("labels")
         if tile.labels:
             for key, val in tile.labels.items():
                 self.h5["tiles"][str(tile.coords)]["labels"].attrs[key] = val
         if tile.counts:
             # cannot concatenate on disk, read into RAM, concatenate, write back to disk
             if self.counts:
                 self.counts = self.counts.to_memory()
@@ -194,15 +193,15 @@
         Args:
             item(int, str, tuple): key or index of tile to be retrieved
 
         Returns:
             Tile(pathml.core.tile.Tile)
         """
         if isinstance(item, bool):
-            raise KeyError(f"invalid key, pass str or tuple")
+            raise KeyError("invalid key, pass str or tuple")
         if isinstance(item, (str, tuple)):
             item = str(item)
             if item not in self.h5["tiles"].keys():
                 raise KeyError(f"key {item} does not exist")
         elif isinstance(item, int):
             if item > len(self.h5["tiles"].keys()) - 1:
                 raise IndexError(
@@ -242,15 +241,15 @@
         )
 
     def remove_tile(self, key):
         """
         Remove tile from self.h5 by key.
         """
         if not isinstance(key, (str, tuple)):
-            raise KeyError(f"key must be str or tuple, check valid keys in repr")
+            raise KeyError("key must be str or tuple, check valid keys in repr")
         if str(key) not in self.h5["tiles"].keys():
             raise KeyError(f"key {key} is not in Tiles")
         del self.h5["tiles"][str(key)]
 
     def add_mask(self, key, mask):
         """
         Add mask to h5.
@@ -266,15 +265,15 @@
             )
         if not isinstance(key, str):
             raise ValueError(f"invalid type {type(key)}, key must be of type str")
         if key in self.h5["masks"].keys():
             raise ValueError(
                 f"key {key} already exists in 'masks'. Cannot add. Must update to modify existing mask."
             )
-        newmask = self.h5["masks"].create_dataset(key, data=mask)
+        self.h5["masks"].create_dataset(key, data=mask)
 
     def update_mask(self, key, mask):
         """
         Update a mask.
 
         Args:
             key(str): key indicating mask to be updated
@@ -336,15 +335,15 @@
             key(str): key indicating mask to be removed
         """
         if not isinstance(key, str):
             raise KeyError(
                 f"masks keys must be of type(str) but key was passed of type {type(key)}"
             )
         if key not in self.h5["masks"].keys():
-            raise KeyError(f"key is not in Masks")
+            raise KeyError("key is not in Masks")
         del self.h5["masks"][key]
 
     def get_slidetype(self):
         slide_type_dict = {
             key: val for key, val in self.h5["fields/slide_type"].items()
         }
         return pathml.core.slide_types.SlideType(**slide_type_dict)
```

### Comparing `pathml-2.1.0/pathml/core/masks.py` & `pathml-2.1.1/pathml/core/masks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
-import numpy as np
-import os
-from pathlib import Path
-from collections import OrderedDict
-import h5py
 import reprlib
-from loguru import logger
+from collections import OrderedDict
+
+import numpy as np
 
 import pathml.core.h5managers
 
 
 class Masks:
     """
     Object wrapping a dict of masks.
```

### Comparing `pathml-2.1.0/pathml/core/slide_backends.py` & `pathml-2.1.1/pathml/core/slide_backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
 from io import BytesIO
-from typing import Tuple
 
 import numpy as np
 import openslide
-from loguru import logger
-import pathml.core
-import pathml.core.tile
 from javabridge.jutil import JavaException
-from pathml.utils import pil_to_rgb
+from loguru import logger
 from PIL import Image
 from pydicom.dataset import Dataset
 from pydicom.encaps import get_frame_offsets
 from pydicom.filebase import DicomFile
 from pydicom.filereader import data_element_offset_to_value, dcmread
 from pydicom.tag import SequenceDelimiterTag, TupleTag
 from pydicom.uid import UID
 from scipy.ndimage import zoom
 
+import pathml.core
+import pathml.core.tile
+from pathml.utils import pil_to_rgb
+
 try:
     import bioformats
     import javabridge
     from bioformats.metadatatools import createOMEXMLMetadata
 except ImportError:
     logger.exception("Unable to import bioformats, javabridge")
     raise Exception(
-        f"Installation of PathML not complete. Please install openjdk8, bioformats, and javabridge:\nconda install openjdk==8.0.152\npip install javabridge==1.0.19 python-bioformats==4.0.0\nFor detailed installation instructions, please see https://github.com/Dana-Farber-AIOS/pathml/"
+        "Installation of PathML not complete. Please install openjdk8, bioformats, and javabridge:\nconda install openjdk==8.0.152\npip install javabridge==1.0.19 python-bioformats==4.0.0\nFor detailed installation instructions, please see https://github.com/Dana-Farber-AIOS/pathml/"
     )
 
 
 class SlideBackend:
     """base class for backends that interface with slides on disk"""
 
     def extract_region(self, location, size, level, **kwargs):
@@ -326,15 +326,16 @@
             ome_pixeltype = (
                 bioformats.OMEXML(self.metadata).image().Pixels.get_PixelType()
             )
             logger.info(f"Using pixel dtype found in OME metadata: {ome_pixeltype}")
             try:
                 self.pixel_dtype = pixel_dtype_map[ome_pixeltype]
                 logger.info(f"Found corresponding dtype: {self.pixel_dtype}")
-            except:
+            # TODO: change to specific exception
+            except Exception:
                 logger.exception("datatype from metadata not found in pixel_dtype_map")
                 raise Exception(
                     f"pixel type '{ome_pixeltype}' detected from OME metadata not recognized."
                 )
 
     def __repr__(self):
         return f"BioFormatsBackend('{self.filename}')"
@@ -407,15 +408,15 @@
             and len(size) < 3
             and all([isinstance(x, int) for x in size])
         ):
             raise ValueError(
                 f"input size {size} invalid. Must be a tuple of integer coordinates of len<2"
             )
         if series_as_channels:
-            logger.info(f"using series_as_channels=True")
+            logger.info("using series_as_channels=True")
             if level != 0:
                 logger.exception(
                     f"When series_as_channels=True, must use level=0. Input 'level={level}' invalid."
                 )
                 raise ValueError(
                     f"Multi-level images not supported with series_as_channels=True. Input 'level={level}' invalid. Use 'level=0'."
                 )
@@ -486,15 +487,15 @@
             # scale array before converting: https://github.com/Dana-Farber-AIOS/pathml/issues/271
             # first scale to [0-1]
             array_scaled = array / (2 ** (8 * self.pixel_dtype.itemsize))
             logger.info(
                 f"Scaling image to [0, 1] by dividing by {(2 ** (8 * self.pixel_dtype.itemsize))}"
             )
             # then scale to [0-255] and convert to 8 bit
-            array_scaled = array_scaled * 2 ** 8
+            array_scaled = array_scaled * 2**8
             return array_scaled.astype(np.uint8)
 
     def get_thumbnail(self, size=None):
         """
         Get a thumbnail of the image. Since there is no default thumbnail for multiparametric, volumetric
         images, this function supports downsampling of all image dimensions.
 
@@ -503,28 +504,28 @@
         Returns:
             np.ndarray: RGB thumbnail image
         Example:
             Get 1000x1000 thumbnail of 7 channel fluorescent image.
             shape = data.slide.get_image_shape()
             thumb = data.slide.get_thumbnail(size=(1000,1000, shape[2], shape[3], shape[4]))
         """
-        assert isinstance(size, (tuple, type(None))), f"Size must be a tuple of ints."
+        assert isinstance(size, (tuple, type(None))), "Size must be a tuple of ints."
         if size is not None:
             if len(size) != len(self.shape):
                 size = size + self.shape[len(size) :]
         if self.shape[0] * self.shape[1] * self.shape[2] * self.shape[3] > 2147483647:
             raise Exception(
                 f"Java arrays allocate maximum 32 bits (~2GB). Image size is {self.imsize}"
             )
         array = self.extract_region(location=(0, 0), size=self.shape[:2])
         if size is not None:
             ratio = tuple([x / y for x, y in zip(size, self.shape)])
             assert (
                 ratio[3] == 1
-            ), f"cannot interpolate between fluor channels, resampling doesn't apply, fix size[3]"
+            ), "cannot interpolate between fluor channels, resampling doesn't apply, fix size[3]"
             image_array = zoom(array, ratio)
         return image_array
 
     def generate_tiles(self, shape=3000, stride=None, pad=False, level=0, **kwargs):
         """
         Generator over tiles.
 
@@ -764,15 +765,15 @@
             size (Union[int, Tuple[int, int]]): Size of each tile. May be a tuple of (height, width) or a
                 single integer, in which case square tiles of that size are generated.
                 Must be the same as the frame size.
 
         Returns:
             np.ndarray: image at the specified region
         """
-        assert level == 0 or level is None, f"dicom does not support levels"
+        assert level == 0 or level is None, "dicom does not support levels"
         # check inputs first
         # check location
         if isinstance(location, tuple):
             frame_ix = self._coords_to_index(location)
         elif isinstance(location, int):
             frame_ix = location
         else:
@@ -883,15 +884,15 @@
             pad (bool): How to handle tiles on the edges. If ``True``, these edge tiles will be zero-padded
                 and yielded with the other chunks. If ``False``, incomplete edge chunks will be ignored.
                 Defaults to ``False``.
 
         Yields:
             pathml.core.tile.Tile: Extracted Tile object
         """
-        assert level == 0 or level is None, f"dicom does not support levels"
+        assert level == 0 or level is None, "dicom does not support levels"
         for i in range(self.n_frames):
 
             if not pad:
                 # skip frame if it's in the last column
                 if i % self.n_cols == (self.n_cols - 1):
                     continue
                 # skip frame if it's in the last row
```

### Comparing `pathml-2.1.0/pathml/core/slide_data.py` & `pathml-2.1.1/pathml/core/slide_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 """
 
 import os
 import reprlib
 from pathlib import Path
 
 import anndata
-from loguru import logger
 import dask.distributed
 import h5py
 import matplotlib.pyplot as plt
 import numpy as np
+from loguru import logger
+
 import pathml.core
 import pathml.preprocessing.pipeline
 from pathml.core.slide_types import SlideType
 
 
 def infer_backend(path):
     """
@@ -209,15 +210,16 @@
         if self._filepath:
             out.append(f"filepath='{self._filepath}'")
         if self.backend:
             out.append(f"backend={repr(self.backend)}")
         out.append(f"image shape: {self.shape}")
         try:
             nlevels = self.slide.level_count
-        except:
+        # TODO: change to specific exception
+        except Exception:
             nlevels = 1
         out.append(f"number of levels: {nlevels}")
         out.append(repr(self.tiles))
         out.append(repr(self.masks))
         if self.tiles:
             out.append(f"tile_shape={eval(self.tiles.tile_shape)}")
         if self.labels:
@@ -225,15 +227,15 @@
                 f"{len(self.labels)} labels: {reprlib.repr(list(self.labels.keys()))}"
             )
         else:
             out.append("labels=None")
         if self.counts:
             out.append(f"counts matrix of shape {self.counts.shape}")
         else:
-            out.append(f"counts=None")
+            out.append("counts=None")
 
         out = ",\n\t".join(out)
         out += ")"
         return out
 
     def run(
         self,
@@ -275,15 +277,15 @@
         ), f"pipeline is of type {type(pipeline)} but must be of type pathml.preprocessing.pipeline.Pipeline"
         assert self.slide is not None, "cannot run pipeline because self.slide is None"
 
         if len(self.tiles) != 0:
             # in this case, tiles already exist
             if not overwrite_existing_tiles:
                 raise Exception(
-                    f"Slide already has tiles. Running the pipeline will overwrite the existing tiles. Use overwrite_existing_tiles=True to force overwriting existing tiles."
+                    "Slide already has tiles. Running the pipeline will overwrite the existing tiles. Use overwrite_existing_tiles=True to force overwriting existing tiles."
                 )
             else:
                 # delete all existing tiles
                 for tile_key in self.tiles.keys:
                     self.tiles.remove(tile_key)
 
         # TODO: be careful here since we are modifying h5 outside of h5manager
@@ -375,14 +377,20 @@
                 single integer, in which case square tiles of that size are generated.
             *args: positional arguments passed through to ``extract_region()`` method of the backend.
             **kwargs: keyword arguments passed through to ``extract_region()`` method of the backend.
 
         Returns:
             np.ndarray: image at the specified region
         """
+        if self.slide is None:
+            raise ValueError(
+                "Cannot call `.extract_region()` because no slide is specified. "
+                "If already tiled, access `.tiles` directly instead"
+            )
+
         return self.slide.extract_region(location, size, *args, **kwargs)
 
     def generate_tiles(self, shape=3000, stride=None, pad=False, **kwargs):
         """
         Generator over Tile objects containing regions of the image.
         Calls ``generate_tiles()`` method of the backend.
         Tries to add the corresponding slide-level masks to each tile, if possible.
@@ -438,18 +446,19 @@
         Not supported by all backends.
 
         Args:
             ax: matplotlib axis object on which to plot the thumbnail. Optional.
         """
         try:
             thumbnail = self.slide.get_thumbnail(size=(500, 500))
-        except:
+        # TODO: change to specific exception
+        except Exception:
             if not self.slide:
                 raise NotImplementedError(
-                    f"Plotting only supported via backend, but SlideData has no backend."
+                    "Plotting only supported via backend, but SlideData has no backend."
                 )
             else:
                 raise NotImplementedError(
                     f"plotting not supported for slide_backend={self.slide.__class__.__name__}"
                 )
         if ax is None:
             ax = plt.gca()
@@ -467,15 +476,15 @@
         if self.tiles.h5manager:
             assert value is None or isinstance(
                 value, anndata.AnnData
             ), f"cannot set counts with obj of type {type(value)}. Must be Anndata"
             self.tiles.h5manager.counts = value
         else:
             raise AttributeError(
-                f"cannot assign counts slidedata contains no tiles, first generate tiles"
+                "cannot assign counts slidedata contains no tiles, first generate tiles"
             )
 
     def write(self, path):
         """
         Write contents to disk in h5path format.
 
         Args:
```

### Comparing `pathml-2.1.0/pathml/core/slide_dataset.py` & `pathml-2.1.1/pathml/core/slide_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
 import reprlib
 from pathlib import Path
-from loguru import logger
 
 import dask.distributed
-from torch.utils.data import ConcatDataset
+from loguru import logger
 
 
 class SlideDataset:
     """
     Container for a dataset of WSIs
 
     Args:
@@ -84,10 +83,10 @@
         for i, slide in enumerate(self.slides):
             if filenames:
                 slide_path = d / (filenames[i] + ".h5path")
             elif slide.name:
                 slide_path = d / (slide.name + ".h5path")
             else:
                 raise ValueError(
-                    f"slide does not have a .name attribute. Must supply a 'filenames' argument."
+                    "slide does not have a .name attribute. Must supply a 'filenames' argument."
                 )
             slide.write(slide_path)
```

### Comparing `pathml-2.1.0/pathml/core/slide_types.py` & `pathml-2.1.1/pathml/core/slide_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
-from loguru import logger
 
 
 class SlideType:
     """
     SlideType objects define types based on a set of image parameters.
 
     Args:
```

### Comparing `pathml-2.1.0/pathml/core/tile.py` & `pathml-2.1.1/pathml/core/tile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
-import numpy as np
-import anndata
+import reprlib
 from collections import OrderedDict
-import matplotlib.pyplot as plt
+
+import anndata
 import h5py
-import reprlib
-from loguru import logger
+import matplotlib.pyplot as plt
+import numpy as np
 
 import pathml.core.masks
 
 
 class Tile:
     """
     Object representing a tile extracted from an image. Holds the array for the tile, as well as the (i,j)
@@ -149,15 +149,15 @@
                 f"{len(self.masks)} masks: {reprlib.repr(list(self.masks.keys()))}"
             )
         else:
             out.append("masks=None")
         if self.counts:
             out.append(f"counts matrix of shape {self.counts.shape}")
         else:
-            out.append(f"counts=None")
+            out.append("counts=None")
         out = ",\n\t".join(out)
         out += ")"
         return out
 
     def plot(self, ax=None):
         """
         View the tile image, using matplotlib.
```

### Comparing `pathml-2.1.0/pathml/core/tiles.py` & `pathml-2.1.1/pathml/core/tiles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
-import os
 import reprlib
 from collections import OrderedDict
-from pathlib import Path
-from loguru import logger
 
-import h5py
 import pathml.core.h5managers
 import pathml.core.masks
 import pathml.core.tile
 
 
 class Tiles:
     """
@@ -35,15 +31,15 @@
             tiledictionary = {}
             for tile in tiles:
                 if not isinstance(tile, pathml.core.Tile):
                     raise ValueError(
                         f"Tiles expects a list of type Tile but was given {type(tile)}"
                     )
                 if tile.coords is None:
-                    raise ValueError(f"tiles must contain valid coords")
+                    raise ValueError("tiles must contain valid coords")
                 coords = tile.coords
                 tiledictionary[coords] = tile
             self._tiles = OrderedDict(tiledictionary)
 
             # add tiles in _tiles to h5manager
             for key, val in self._tiles.items():
                 self.h5manager.add_tile(val)
```

### Comparing `pathml-2.1.0/pathml/core/utils.py` & `pathml-2.1.1/pathml/core/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
-import ast
 import tempfile
-from collections import OrderedDict
-from dataclasses import asdict
-from loguru import logger
+
 import anndata
 import h5py
 import numpy as np
-import pathml.core.slide_backends
-import pathml.core.slide_data
 
 
 # TODO: Fletcher32 checksum?
 def writedataframeh5(h5, name, df):
     """
     Write dataframe as h5 dataset.
 
     Args:
         h5(h5py.Dataset): root of h5 object that df will be written into
         name(str): name of dataset to be created
         df(pd.DataFrame): dataframe to be written
     """
-    dataset = h5.create_dataset(
+    h5.create_dataset(
         str(name),
         data=df,
         chunks=True,
         compression="gzip",
         compression_opts=5,
         shuffle=True,
     )
```

### Comparing `pathml-2.1.0/pathml/datasets/base_data_module.py` & `pathml-2.1.1/pathml/datasets/base_data_module.py`

 * *Files identical despite different names*

### Comparing `pathml-2.1.0/pathml/datasets/deepfocus.py` & `pathml-2.1.1/pathml/datasets/deepfocus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
 import hashlib
 import os
-from loguru import logger
 from pathlib import Path
 
 import h5py
+from loguru import logger
+from torch.utils.data import DataLoader, Dataset
+
 from pathml.datasets.base_data_module import BaseDataModule
 from pathml.utils import download_from_url
-from torch.utils.data import DataLoader, Dataset
 
 
 class DeepFocusDataModule(BaseDataModule):
     """
     DataModule for the DeepFocus dataset. The DeepFocus dataset comprises four slides from different patients,
     each with four different stains (H&E, Ki67, CD21, and CD10) for a total of 16 whole-slide images.
     For each slide, a region of interest (ROI) of approx 6mm^2 was scanned at 40x magnification with
@@ -43,15 +44,15 @@
     ):
         self.data_dir = Path(data_dir)
         if download:
             self._download_deepfocus(self.data_dir)
         else:
             assert (
                 self._check_integrity()
-            ), f"download is False but data directory does not exist or md5 checksum failed"
+            ), "download is False but data directory does not exist or md5 checksum failed"
         self.shuffle = shuffle
         self.transforms = transforms
         self.batch_size = batch_size
 
     @property
     def train_dataloader(self):
         return DataLoader(
```

### Comparing `pathml-2.1.0/pathml/datasets/pannuke.py` & `pathml-2.1.1/pathml/datasets/pannuke.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 """
 
 import os
 import re
 import shutil
 import zipfile
 from pathlib import Path
-from warnings import warn
 
 import cv2
 import numpy as np
-from loguru import logger
 import torch
 import torch.utils.data as data
+from loguru import logger
+
 from pathml.datasets.base_data_module import BaseDataModule
 from pathml.datasets.utils import pannuke_multiclass_mask_to_nucleus_mask
 from pathml.ml.hovernet import compute_hv_map
 from pathml.utils import download_from_url
 
 
 class PanNukeDataset(data.Dataset):
```

### Comparing `pathml-2.1.0/pathml/datasets/utils.py` & `pathml-2.1.1/pathml/datasets/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
 import numpy as np
-from loguru import logger
+
 
 def pannuke_multiclass_mask_to_nucleus_mask(multiclass_mask):
     """
     Convert multiclass mask from PanNuke to a single channel nucleus mask.
     Assumes each pixel is assigned to one and only one class. Sums across channels, except the last mask channel
     which indicates background pixels in PanNuke.
     Operates on a single mask.
```

### Comparing `pathml-2.1.0/pathml/ml/dataset.py` & `pathml-2.1.1/pathml/ml/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
-from loguru import logger
 import h5py
 import numpy as np
 import torch
 
 
 class TileDataset(torch.utils.data.Dataset):
     """
@@ -48,15 +47,15 @@
         return self.dataset_len
 
     def __getitem__(self, ix):
         if self.h5 is None:
             self.h5 = h5py.File(self.file_path, "r")
 
         k = self.tile_keys[ix]
-        ### this part copied from h5manager.get_tile()
+        # this part copied from h5manager.get_tile()
         tile_image = self.h5["tiles"][str(k)]["array"][:]
 
         # get corresponding masks if there are masks
         if "masks" in self.h5["tiles"][str(k)].keys():
             masks = {
                 mask: self.h5["tiles"][str(k)]["masks"][mask][:]
                 for mask in self.h5["tiles"][str(k)]["masks"]
```

### Comparing `pathml-2.1.0/pathml/ml/hovernet.py` & `pathml-2.1.1/pathml/ml/hovernet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
-import torch
-from torch import nn
-from torch.nn import functional as F
-import numpy as np
 import cv2
-from loguru import logger
-from skimage.segmentation import watershed
-from scipy.ndimage.morphology import binary_fill_holes
 import matplotlib.pyplot as plt
+import numpy as np
+import torch
+from loguru import logger
 from matplotlib.colors import TABLEAU_COLORS
-from warnings import warn
+from scipy.ndimage.morphology import binary_fill_holes
+from skimage.segmentation import watershed
+from torch import nn
+from torch.nn import functional as F
 
-from pathml.utils import segmentation_lines
 from pathml.ml.utils import center_crop_im_batch, dice_loss, get_sobel_kernels
+from pathml.utils import segmentation_lines
 
 
 class _BatchNormRelu(nn.Module):
     """BatchNorm + Relu layer"""
 
     def __init__(self, n_channels):
         super(_BatchNormRelu, self).__init__()
@@ -427,15 +426,16 @@
 
     out = np.zeros((2, mask.shape[0], mask.shape[1]))
     # each individual nucleus is indexed with a different number
     inst_list = list(np.unique(mask))
 
     try:
         inst_list.remove(0)  # 0 is background
-    except:
+    # TODO: change to specific exception
+    except Exception:
         logger.warning(
             "No pixels with 0 label. This means that there are no background pixels. This may indicate a problem. Ignore this warning if this is expected/intended."
         )
 
     for inst_id in inst_list:
         # get the mask for the nucleus
         inst_map = mask == inst_id
```

### Comparing `pathml-2.1.0/pathml/ml/utils.py` & `pathml-2.1.1/pathml/ml/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
+import numpy as np
+
 # Utilities for ML module
 import torch
 from torch.nn import functional as F
-import numpy as np
-from loguru import logger
 
 
 def center_crop_im_batch(batch, dims, batch_order="BCHW"):
     """
     Center crop images in a batch.
 
     Args:
@@ -39,15 +39,15 @@
         crop_r = dims[1] - crop_l
 
         if batch_order == "BHWC":
             batch_cropped = batch[:, crop_t:-crop_b, crop_l:-crop_r, :]
         elif batch_order == "BCHW":
             batch_cropped = batch[:, :, crop_t:-crop_b, crop_l:-crop_r]
         else:
-            raise Exception(f"Input batch order not valid")
+            raise Exception("Input batch order not valid")
 
     return batch_cropped
 
 
 def dice_loss(true, logits, eps=1e-3):
     """
     Computes the Sørensen–Dice loss.
@@ -156,15 +156,15 @@
     """
     targets = transform.additional_targets
     n_targets = len(targets)
 
     # make sure that everything is correct so that transform is correctly applied
     assert all(
         [v == "mask" for v in targets.values()]
-    ), f"error all values in transform.additional_targets must be 'mask'."
+    ), "error all values in transform.additional_targets must be 'mask'."
 
     def transform_out(*args, **kwargs):
         mask = kwargs.pop("mask")
         assert mask.ndim == 3, f"input mask shape {mask.shape} must be 3-dimensions ()"
         assert (
             mask.shape[0] == n_targets
         ), f"input mask shape {mask.shape} doesn't match additional_targets {transform.additional_targets}"
```

### Comparing `pathml-2.1.0/pathml/preprocessing/__init__.py` & `pathml-2.1.1/pathml/preprocessing/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
 from .pipeline import Pipeline
 from .transforms import (
+    AdaptiveHistogramEqualization,
     BinaryThreshold,
     BoxBlur,
+    CollapseRunsCODEX,
+    CollapseRunsVectra,
     ForegroundDetection,
     GaussianBlur,
+    HistogramEqualization,
+    LabelArtifactTileHE,
+    LabelWhiteSpaceHE,
     MedianBlur,
-    MorphOpen,
     MorphClose,
+    MorphOpen,
     NucleusDetectionHE,
+    QuantifyMIF,
+    RescaleIntensity,
+    SegmentMIF,
     StainNormalizationHE,
     SuperpixelInterpolation,
     TissueDetectionHE,
-    LabelArtifactTileHE,
-    LabelWhiteSpaceHE,
-    SegmentMIF,
-    QuantifyMIF,
-    CollapseRunsVectra,
-    CollapseRunsCODEX,
-    RescaleIntensity,
-    HistogramEqualization,
-    AdaptiveHistogramEqualization,
 )
```

### Comparing `pathml-2.1.0/pathml/preprocessing/pipeline.py` & `pathml-2.1.1/pathml/preprocessing/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
 import pickle
-from loguru import logger
 
 import pathml.core.tile
 from pathml.preprocessing.transforms import Transform
 
 
 class Pipeline(Transform):
     """
@@ -18,25 +17,25 @@
         transform_sequence (list): sequence of transforms to be consecutively applied.
             List of `pathml.core.Transform` objects
     """
 
     def __init__(self, transform_sequence=None):
         assert transform_sequence is None or all(
             [isinstance(t, Transform) for t in transform_sequence]
-        ), (f"All elements in input list must be of" f" type pathml.core.Transform")
+        ), "All elements in input list must be of type pathml.core.Transform"
         self.transforms = transform_sequence
 
     def __len__(self):
         return len(self.transforms)
 
     def __repr__(self):
         if self.transforms is None:
             return "Pipeline()"
         else:
-            out = f"Pipeline([\n"
+            out = "Pipeline([\n"
             for t in self.transforms:
                 out += f"\t{repr(t)},\n"
             out += "])"
             return out
 
     def apply(self, tile):
         # this function has side effects
```

### Comparing `pathml-2.1.0/pathml/preprocessing/tiling.py` & `pathml-2.1.1/pathml/preprocessing/tiling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
 import numpy as np
-from loguru import logger
 
 
 def extract_tiles(arr, tile_size, stride=None):
     """
     Extract tiles from an array. Allows user to specify stride between tiles.
     Based on original implementation in ``sklearn.feature_extraction.image_ref._extract_patches``
     Incomplete tiles on the edge are dropped (TO DO: fix this (zero padding?))
```

### Comparing `pathml-2.1.0/pathml/preprocessing/transforms.py` & `pathml-2.1.1/pathml/preprocessing/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 Copyright 2021, Dana-Farber Cancer Institute and Weill Cornell Medicine
 License: GNU GPL 2.0
 """
 
 import os
-from warnings import warn
 
-from loguru import logger
 import anndata
 import cv2
 import numpy as np
 import pandas as pd
+from loguru import logger
+from skimage import restoration
+from skimage.exposure import equalize_adapthist, equalize_hist, rescale_intensity
+from skimage.measure import regionprops_table
+
 import pathml.core
 import pathml.core.slide_data
 from pathml.utils import (
     RGB_to_GREY,
     RGB_to_HSI,
     RGB_to_HSV,
     RGB_to_OD,
     normalize_matrix_cols,
 )
-from skimage import restoration
-from skimage.exposure import equalize_adapthist, equalize_hist, rescale_intensity
-from skimage.measure import regionprops_table
+
 
 # Base class
 class Transform:
     """
     Base class for all Transforms.
     Each transform must operate on a Tile.
     """
@@ -643,18 +644,18 @@
         ], f"Error: input stain estimation method {stain_estimation_method} must be one of 'macenko' or 'vahadane'"
         assert (
             0 <= background_intensity <= 255
         ), f"Error: input background intensity {background_intensity} must be an integer between 0 and 255"
 
         if stain_estimation_method.lower() == "vahadane":
             try:
-                import spams
+                import spams  # noqa: F401
             except (ImportError, ModuleNotFoundError):
                 raise Exception(
-                    f"Vahadane method requires `spams` package to be installed"
+                    "Vahadane method requires `spams` package to be installed"
                 )
 
         self.target = target.lower()
         self.stain_estimation_method = stain_estimation_method.lower()
         self.optical_density_threshold = optical_density_threshold
         self.sparsity_regularizer = sparsity_regularizer
         self.angular_percentile = angular_percentile
@@ -739,15 +740,15 @@
 
         Args:
             image (np.ndarray): RGB image
         """
         try:
             import spams
         except (ImportError, ModuleNotFoundError):
-            raise Exception(f"Vahadane method requires `spams` package to be installed")
+            raise Exception("Vahadane method requires `spams` package to be installed")
         # convert to Optical Density (OD) space
         image_OD = RGB_to_OD(image)
         # reshape to (M*N)x3
         image_OD = image_OD.reshape(-1, 3)
         # drop pixels with low OD
         OD = image_OD[np.all(image_OD > self.optical_density_threshold, axis=1)]
 
@@ -843,15 +844,15 @@
             image (np.ndarray): RGB image
             stain_matrix (np.ndarray): matrix of H and E stain vectors in optical density (OD) space.
                 Stain_matrix is (3, 2) and first column corresponds to hematoxylin by convention.
         """
         try:
             import spams
         except (ImportError, ModuleNotFoundError):
-            raise Exception(f"Vahadane method requires `spams` package to be installed")
+            raise Exception("Vahadane method requires `spams` package to be installed")
         image_OD = RGB_to_OD(image).reshape(-1, 3)
 
         # Get concentrations of each stain at each pixel
         # image_ref.T = S @ C.T
         #   image_ref.T is 3x(M*N)
         #   stain matrix S is 3x2
         #   concentration matrix C.T is 2x(M*N)
@@ -1226,15 +1227,15 @@
         assert psf is None or isinstance(
             psf, np.ndarray
         ), f"psf must be None or an np.ndarray. input psf is type {type(psf)}"
         self.psf = psf
         if psfparameters:
             assert (
                 psf is None
-            ), f"you passed an empirical psf, cannot simultaneously use theoretical psf"
+            ), "you passed an empirical psf, cannot simultaneously use theoretical psf"
         self.psfparameters = psfparameters
         self.iterations = iterations
 
     def __repr__(self):
         return (
             f"DeconvolveMIF(psf={'empirical' if self.psf else self.psfparameters}, iterations={self.self.iterations}, "
             f"gpu={self.gpu})"
@@ -1314,46 +1315,46 @@
         image_resolution=0.5,
         preprocess_kwargs=None,
         postprocess_kwargs_nuclear=None,
         postprocess_kwargs_whole_cell=None,
     ):
         assert isinstance(
             nuclear_channel, int
-        ), f"nuclear_channel must be an int indicating index"
+        ), "nuclear_channel must be an int indicating index"
         assert isinstance(
             cytoplasm_channel, int
-        ), f"cytoplasm_channel must be an int indicating index"
+        ), "cytoplasm_channel must be an int indicating index"
         self.nuclear_channel = nuclear_channel
         self.cytoplasm_channel = cytoplasm_channel
         self.image_resolution = image_resolution
         self.preprocess_kwargs = preprocess_kwargs if preprocess_kwargs else {}
         self.postprocess_kwargs_nuclear = (
             postprocess_kwargs_nuclear if postprocess_kwargs_nuclear else {}
         )
         self.postprocess_kwargs_whole_cell = (
             postprocess_kwargs_whole_cell if postprocess_kwargs_whole_cell else {}
         )
 
         if model.lower() == "mesmer":
             try:
-                from deepcell.applications import Mesmer
+                from deepcell.applications import Mesmer  # noqa: F401
             except ImportError:
                 logger.warning(
                     "The Mesmer model in SegmentMIF requires extra libraries to be installed.\nYou can install these via pip using:\npip install deepcell"
                 )
                 raise ImportError(
-                    f"The Mesmer model in SegmentMIF requires deepcell to be installed"
+                    "The Mesmer model in SegmentMIF requires deepcell to be installed"
                 ) from None
             self.model = model.lower()
         elif model.lower() == "cellpose":
             """from cellpose import models
             self.model = models.Cellpose(gpu=self.gpu, model_type='cyto')"""
-            raise NotImplementedError(f"Cellpose model not currently supported")
+            raise NotImplementedError("Cellpose model not currently supported")
         else:
-            raise ValueError(f"currently only supports mesmer model")
+            raise ValueError("currently only supports mesmer model")
 
     def __repr__(self):
         return (
             f"SegmentMIF(model={self.model}, image_resolution={self.image_resolution})"
         )
 
     def F(self, image):
@@ -1487,15 +1488,16 @@
         counts.layers["min_intensity"] = min_intensities
         max_intensities = pd.DataFrame()
         for i in range(img.shape[-1]):
             max_intensities[i] = countsdataframe[f"max_intensity-{i}"]
         counts.layers["max_intensity"] = max_intensities
         try:
             counts.obsm["spatial"] = np.array(counts.obs[["x", "y"]])
-        except:
+        # TODO: change to specific exception
+        except Exception:
             logger.warning("did not log coordinates in obsm")
         return counts
 
     def apply(self, tile):
         assert isinstance(
             tile, pathml.core.tile.Tile
         ), f"tile is type {type(tile)} but must be pathml.core.tile.Tile"
@@ -1518,15 +1520,15 @@
     For compatibility with transforms, tiles need to have their shape collapsed to (x, y, c)
     """
 
     def __init__(self):
         pass
 
     def __repr__(self):
-        return f"CollapseRunsVectra()"
+        return "CollapseRunsVectra()"
 
     def F(self, image):
         image = np.squeeze(image)
         return image
 
     def apply(self, tile):
         assert isinstance(
```

### Comparing `pathml-2.1.0/pathml/utils.py` & `pathml-2.1.1/pathml/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             shutil.copyfileobj(response, out_file)
 
 
 def parse_file_size(fs):
     """
     Parse a file size string into bytes.
     """
-    units = {"B": 1, "KB": 10 ** 3, "MB": 10 ** 6, "GB": 10 ** 9, "TB": 10 ** 12}
+    units = {"B": 1, "KB": 10**3, "MB": 10**6, "GB": 10**9, "TB": 10**12}
     number, unit = [s.strip() for s in fs.split()]
     return int(float(number) * units[unit.upper()])
 
 
 def upsample_array(arr, factor):
     """
     Upsample array by a factor. Each element in input array will become a CxC block in the upsampled array, where
```

### Comparing `pathml-2.1.0/pathml.egg-info/PKG-INFO` & `pathml-2.1.1/pathml.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pathml
-Version: 2.1.0
+Version: 2.1.1
 Summary: Tools for computational pathology
 Author: Jacob Rosenthal, Ryan Carelli et al.
 Author-email: PathML@dfci.harvard.edu
-License: UNKNOWN
 Project-URL: Documentation, https://pathml.readthedocs.io/en/stable
 Project-URL: Source Code, https://github.com/Dana-Farber-AIOS/pathml
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Framework :: Sphinx
@@ -21,30 +19,38 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/logo.png width="300"> 
-
-<img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/overview.png width="750">
+🤖🔬 **PathML: Tools for computational pathology**
 
+[![Downloads](https://pepy.tech/badge/pathml)](https://pepy.tech/project/pathml)
 [![Documentation Status](https://readthedocs.org/projects/pathml/badge/?version=latest)](https://pathml.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/gh/Dana-Farber-AIOS/pathml/branch/master/graph/badge.svg?token=UHSQPTM28Y)](https://codecov.io/gh/Dana-Farber-AIOS/pathml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://img.shields.io/pypi/v/pathml)](https://pypi.org/project/pathml/)
-[![Downloads](https://pepy.tech/badge/pathml)](https://pepy.tech/project/pathml)
-[![codecov](https://codecov.io/gh/Dana-Farber-AIOS/pathml/branch/master/graph/badge.svg?token=UHSQPTM28Y)](https://codecov.io/gh/Dana-Farber-AIOS/pathml)
+
+⭐ **PathML objective is to lower the barrier to entry to digital pathology**
+
+Imaging datasets in cancer research are growing exponentially in both quantity and information density. These massive datasets may enable derivation of insights for cancer research and clinical care, but only if researchers are equipped with the tools to leverage advanced computational analysis approaches such as machine learning and artificial intelligence. In this work, we highlight three themes to guide development of such computational tools: scalability, standardization, and ease of use. We then apply these principles to develop PathML, a general-purpose research toolkit for computational pathology. We describe the design of the PathML framework and demonstrate applications in diverse use cases. 
+
+🚀 **The fastest way to get started?**
+
+    docker pull pathml/pathml && docker run -it -p 8888:8888 pathml/pathml
 
 | Branch | Test status   |
 | ------ | ------------- |
 | master | ![tests](https://github.com/Dana-Farber-AIOS/pathml/actions/workflows/tests-conda.yml/badge.svg?branch=master) |
 | dev    | ![tests](https://github.com/Dana-Farber-AIOS/pathml/actions/workflows/tests-conda.yml/badge.svg?branch=dev) |
 
-An open-source toolkit for computational pathology and machine learning.
+<img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/logo.png width="300"> 
+
+<img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/overview.png width="750">
 
 **View [documentation](https://pathml.readthedocs.io/en/latest/)**
 
 :construction: the `dev` branch is under active development, with experimental features, bug fixes, and refactors that may happen at any time! 
 Stable versions are available as tagged releases on GitHub, or as versioned releases on PyPI
 
 # Installation
@@ -115,14 +121,16 @@
 pip install -e .
 ````
 
 ## Installation option 3: Docker
 
 First, download or build the PathML Docker container:
 
+![pathml-docker-installation](https://user-images.githubusercontent.com/25375373/191053363-477497a1-9804-48f3-91f9-767dc7f859ed.gif)
+
 - Option A: download PathML container from Docker Hub
    ````
    docker pull pathml/pathml:latest
    ````
   Optionally specify a tag for a particular version, e.g. `docker pull pathml/pathml:2.0.2`. To view possible tags, 
   please refer to the [PathML DockerHub page](https://hub.docker.com/r/pathml/pathml).
   
@@ -146,14 +154,31 @@
 
 Note that the docker container requires extra configurations to use with GPU.  
 Note that these instructions assume that there are no other processes using port 8888.
 
 Please refer to the `Docker run` [documentation](https://docs.docker.com/engine/reference/run/) for further instructions
 on accessing the container, e.g. for mounting volumes to access files on a local machine from within the container.
 
+## Option 4: Google Colab
+
+To get PathML running in a Colab environment:
+
+````
+!pip install openslide-python
+!apt-get install openslide-tools
+!apt-get install openjdk-8-jdk-headless -qq > /dev/null
+os.environ["JAVA_HOME"] = "/usr/lib/jvm/java-8-openjdk-amd64"
+!update-alternatives --set java /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java
+!java -version
+!pip install pathml
+````
+
+*Thanks to all of our open-source collaborators for helping maintain these installation instructions!*  
+*Please open an issue for any bugs or other problems during installation process.*
+
 ## CUDA
 
 To use GPU acceleration for model training or other tasks, you must install CUDA. 
 This guide should work, but for the most up-to-date instructions, refer to the [official PyTorch installation instructions](https://pytorch.org/get-started/locally/).
 
 Check the version of CUDA:
 ````
@@ -212,30 +237,52 @@
 * Sharing trained model parameters
 * Sharing ``PathML`` with colleagues, students, etc.
 
 See [contributing](https://github.com/Dana-Farber-AIOS/pathml/blob/master/CONTRIBUTING.rst) for more details.
 
 # Citing
 
-If you use `PathML` in your work, please cite our paper:
+If you use `PathML` please cite:
+
+- [**J. Rosenthal et al., "Building tools for machine learning and artificial intelligence in cancer research: best practices and a case study with the PathML toolkit for computational pathology." Molecular Cancer Research, 2022.**](https://doi.org/10.1158/1541-7786.MCR-21-0665)
+
+So far, PathML was used in the following manuscripts: 
 
-Rosenthal J, Carelli R, Omar M, Brundage D, Halbert E, Nyman J, Hari SN, Van Allen EM, Marchionni L, Umeton R, Loda M. 
-Building tools for machine learning and artificial intelligence in cancer research: best practices and a case study 
-with the PathML toolkit for computational pathology. *Molecular Cancer Research*, 2021. 
-DOI: [10.1158/1541-7786.MCR-21-0665](https://doi.org/10.1158/1541-7786.MCR-21-0665)
+- [J. Linares et al. **Molecular Cell** 2021](https://www.cell.com/molecular-cell/fulltext/S1097-2765(21)00729-2)
+- [A. Shmatko et al. **Nature Cancer** 2022](https://www.nature.com/articles/s43018-022-00436-4)
+- [J. Pocock et al. **Nature Communications Medicine** 2022](https://www.nature.com/articles/s43856-022-00186-5)
+- [S. Orsulic et al. **Frontiers in Oncology** 2022](https://www.frontiersin.org/articles/10.3389/fonc.2022.924945/full)
+- [D. Brundage et al. **arXiv** 2022](https://arxiv.org/abs/2203.13888)
+- [A. Marcolini et al. **SoftwareX** 2022](https://www.sciencedirect.com/science/article/pii/S2352711022001558)
+- [M. Rahman et al. **Bioengineering** 2022](https://www.mdpi.com/2306-5354/9/8/335)
+- [C. Lama et al. **bioRxiv** 2022](https://www.biorxiv.org/content/10.1101/2022.09.28.509751v1.full)
+- the list continues [**here 🔗 for 2023 and onwards**](https://scholar.google.com/scholar?oi=bibs&hl=en&cites=1157052756975292108)
+
+# Users
+
+<table style="border: 0px !important;"><tr><td>This is where in the world our most enthusiastic supporters are located:
+   <br/><br/>
+<img src="https://user-images.githubusercontent.com/25375373/208137141-e450aa86-8433-415a-9cc7-c4274139bdc2.png" width="500px">
+   </td><td>   
+and this is where they work:
+   <br/><br/>
+<img src="https://user-images.githubusercontent.com/25375373/208137644-f73c86d0-c5c7-4094-80d9-ea11e0edbdc5.png" width="400px">
+</td>                                                                                                                             
+</tr>
+</table>
+
+Source: https://ossinsight.io/analyze/Dana-Farber-AIOS/pathml#people
 
 # License
 
 The GNU GPL v2 version of PathML is made available via Open Source licensing. 
 The user is free to use, modify, and distribute under the terms of the GNU General Public License version 2.
 
 Commercial license options are available also.
 
 # Contact
 
 Questions? Comments? Suggestions? Get in touch!
 
-[PathML@dfci.harvard.edu](mailto:PathML@dfci.harvard.edu)
+[pathml@dfci.harvard.edu](mailto:pathml@dfci.harvard.edu)
 
 <img src=https://raw.githubusercontent.com/Dana-Farber-AIOS/pathml/master/docs/source/_static/images/dfci_cornell_joint_logos.png width="750"> 
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pathml-2.1.0/pathml.egg-info/SOURCES.txt` & `pathml-2.1.1/pathml.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,8 +29,12 @@
 pathml/ml/__init__.py
 pathml/ml/dataset.py
 pathml/ml/hovernet.py
 pathml/ml/utils.py
 pathml/preprocessing/__init__.py
 pathml/preprocessing/pipeline.py
 pathml/preprocessing/tiling.py
-pathml/preprocessing/transforms.py
+pathml/preprocessing/transforms.py
+tests/test_logging.py
+tests/test_manuscript_urls.py
+tests/test_utils.py
+tests/test_version.py
```

### Comparing `pathml-2.1.0/setup.py` & `pathml-2.1.1/setup.py`

 * *Files identical despite different names*

