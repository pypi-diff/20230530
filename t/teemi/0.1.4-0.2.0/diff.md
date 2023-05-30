# Comparing `tmp/teemi-0.1.4.tar.gz` & `tmp/teemi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teemi-0.1.4.tar", last modified: Tue May  9 07:33:09 2023, max compression
+gzip compressed data, was "teemi-0.2.0.tar", last modified: Tue May 30 12:37:19 2023, max compression
```

## Comparing `teemi-0.1.4.tar` & `teemi-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.938116 teemi-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-09 07:31:59.000000 teemi-0.1.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-09 07:31:59.000000 teemi-0.1.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-09 07:31:59.000000 teemi-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 07:31:59.000000 teemi-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-05-09 07:33:09.938116 teemi-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10602 2023-05-09 07:31:59.000000 teemi-0.1.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-09 07:33:09.938116 teemi-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-09 07:31:59.000000 teemi-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.938116 teemi-0.1.4/teemi/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 07:33:09.938116 teemi-0.1.4/teemi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.934116 teemi-0.1.4/teemi/build/
--rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/build/PCR.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30079 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/build/containers_wells_picklists.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/build/robot_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/build/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.938116 teemi-0.1.4/teemi/design/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/design/cloning.py
--rw-r--r--   0 runner    (1001) docker     (123)    24971 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/design/combinatorial_design.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/design/fetch_sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/design/retrieve_gene_homologs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/design/teselagen_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.938116 teemi-0.1.4/teemi/learn/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/learn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/learn/auto_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/learn/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.938116 teemi-0.1.4/teemi/lims/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/lims/benchling_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/lims/csv_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.938116 teemi-0.1.4/teemi/test/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/test/genotyping.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-05-09 07:31:59.000000 teemi-0.1.4/teemi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:33:09.934116 teemi-0.1.4/teemi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 07:33:09.000000 teemi-0.1.4/teemi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-09 07:31:59.000000 teemi-0.1.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.976055 teemi-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-30 12:36:14.000000 teemi-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-30 12:36:14.000000 teemi-0.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-30 12:36:14.000000 teemi-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 12:36:14.000000 teemi-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-05-30 12:37:19.976055 teemi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10602 2023-05-30 12:36:14.000000 teemi-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-30 12:37:19.976055 teemi-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-30 12:36:15.000000 teemi-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.976055 teemi-0.2.0/teemi/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 12:37:19.976055 teemi-0.2.0/teemi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.972056 teemi-0.2.0/teemi/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/build/PCR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30079 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/build/containers_wells_picklists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/build/robot_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/build/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.972056 teemi-0.2.0/teemi/design/
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/CRISPRsequencecutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24971 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/combinatorial_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/fetch_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/retrieve_gene_homologs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/sequence_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/design/teselagen_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.976055 teemi-0.2.0/teemi/learn/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/learn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/learn/auto_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22443 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/learn/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.976055 teemi-0.2.0/teemi/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/lims/benchling_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/lims/csv_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.976055 teemi-0.2.0/teemi/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/test/data_wrangling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/test/genotyping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-05-30 12:36:15.000000 teemi-0.2.0/teemi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:37:19.972056 teemi-0.2.0/teemi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 12:37:19.000000 teemi-0.2.0/teemi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-30 12:36:15.000000 teemi-0.2.0/versioneer.py
```

### Comparing `teemi-0.1.4/LICENSE` & `teemi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/PKG-INFO` & `teemi-0.2.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: teemi
-Version: 0.1.4
-Summary: A Python package for constructing microbial strains
-Home-page: https://github.com/hiyama341/teemi
-Author: Lucas Levassor
-Author-email: lucaslevassor@gmail.com
-License: MIT license
-Keywords: teemi
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 .. image:: https://raw.githubusercontent.com/hiyama341/teemi/main/pictures/teemi_logo.svg
   :width: 400
   :alt: teemi logo 
 
 teemi: a python package designed to make HT strain construction reproducible and FAIR
 -------------------------------------------------------------------------------------
 
@@ -331,16 +309,8 @@
 -------
 - This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
-- teemis logo was made by Jonas Krogh Fischer. Check out his `website <http://jkfischerproductions.com/kea/portfolio/index.html>`__. 
-
-History
--------
-
-0.1.0 (2023-01-02)
-------------------
-
-* First release on PyPI.
+- teemis logo was made by Jonas Krogh Fischer. Check out his `website <http://jkfischerproductions.com/kea/portfolio/index.html>`__.
```

### Comparing `teemi-0.1.4/README.rst` & `teemi-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,316 +1,354 @@
-.. image:: https://raw.githubusercontent.com/hiyama341/teemi/main/pictures/teemi_logo.svg
-  :width: 400
-  :alt: teemi logo 
-
-teemi: a python package designed to make HT strain construction reproducible and FAIR
--------------------------------------------------------------------------------------
-
-.. summary-start
-
-.. image:: https://badge.fury.io/py/teemi.svg
-        :target: https://badge.fury.io/py/teemi
-
-.. image:: https://github.com/hiyama341/teemi/actions/workflows/main.yml/badge.svg
-        :target: https://github.com/hiyama341/teemi/actions
-
-.. image:: https://readthedocs.org/projects/teemi/badge/?version=latest
-        :target: https://teemi.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-.. image:: https://img.shields.io/github/license/hiyama341/teemi
-        :target: https://github.com/hiyama341/teemi/blob/main/LICENSE
-
-.. image:: https://img.shields.io/pypi/pyversions/teemi.svg
-        :target: https://pypi.org/project/teemi/
-        :alt: Supported Python Versions
-
-.. image:: https://codecov.io/gh/hiyama341/teemi/branch/main/graph/badge.svg?token=P4457QACUY 
-        :target: https://codecov.io/gh/hiyama341/teemi
-
-.. image:: https://img.shields.io/badge/code%20style-black-black
-        :target: https://black.readthedocs.io/en/stable/
-
-.. image:: https://img.shields.io/github/last-commit/hiyama341/teemi
-
-
-
-What is teemi?
-~~~~~~~~~~~~~~
-
-**teemi**, named after the Greek goddess of fairness, is a python package designed
-to make microbial strain construction reproducible and FAIR (Findable, Accessible, 
-Interoperable, and Reusable). With teemi, you can simulate all steps of 
-a strain construction cycle, from generating genetic parts to designing 
-a combinatorial library and keeping track of samples through a commercial
-Benchling API and a low-level CSV file database. 
-This tool can be used in literate programming to 
-increase efficiency and speed in metabolic engineering tasks. 
-To try teemi, visit our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__.
-
-
-teemi not only simplifies the strain construction process but also offers the 
-flexibility to adapt to different experimental workflows through its open-source
-Python platform. This allows for efficient automation of repetitive tasks and
-a faster pace in metabolic engineering.
-
-Our demonstration of teemi in a complex machine learning-guided
-metabolic engineering task showcases its efficiency 
-and speed by debottlenecking a crucial step in the strictosidine pathway. 
-This highlights the versatility and usefulness of this tool in various  
-biological applications. 
-
-Curious about how you can build strains easier and faster with teemi? 
-Head over to our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__
-and give it a try.
-
-Please cite our paper (in preparation - link tba) if you've used teemi in a scientific publication.
-
-.. summary-end
-
-
-Features
---------
-
-* Combinatorial library generation
-* HT cloning and transformation workflows
-* Flowbot One instructions
-* CSV-based LIMS system as well as integration to Benchling
-* Genotyping of microbial strains
-* Advanced Machine Learning of biological datasets with the AutoML `H2O <https://docs.h2o.ai/h2o/latest-stable/h2o-docs/automl.html>`__
-* Workflows for selecting enzyme homologs
-* Promoter selection workflows from RNA-seq datasets
-* Data analysis of large LC-MS datasets along with workflows for analysis
-
-
-Getting started
-~~~~~~~~~~~~~~~
-To get started with making microbial strains in an HT manner please follow the steps below: 
-
-1. Install teemi. You will find the necessary information below for installation.
-
-2. Check out our `notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__ for inspiration to make HT strain construction with teemi.
-
-3. You can start making your own workflows by importing teemi into either Google colab or Jupyter lab/notebooks.
-
-
-Colab notebooks
----------------
-As a proof of concept we show how teemi and literate programming can be used to streamline bioengineering workflows.
-These workflows should serve as a guide or a help to build your own workflows and thereby harnessing the power of literate programming with teemi. 
-
-Specifically, in this study we present how teemi and literate programming to build simulation-guided, iterative,
-and evolution-guided laboratory workflows for optimizing strictosidine production in yeast.
-
-Below you can find all the notebooks developed in this work. 
-Just click the Google colab badge to start the workflows. 
-
-Strictosidine case : First DBTL cycle
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-**DESIGN:**
-
-..  |Notebook 00| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 00
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/00_1_DESIGN_Homologs.ipynb 
-
-..  |Notebook 01| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 01
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/01_1_DESIGN_Promoters.ipynb
-
-..  |Notebook 02| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 02
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/02_1_DESIGN_Combinatorial_library.ipynb
-    
-
-00. Automatically fetch homologs from NCBI from a query in a standardizable and repeatable way 
-
-|Notebook 00| 
-
-
-01. Promoters can be selected from RNAseq data and fetched from online database with various quality measurements implemented 
-
-|Notebook 01|
-
-
-
-02. Combinatorial libraries can be generated with the DesignAssembly class along with robot executable intructions 
-
-|Notebook 02| 
-
-
-
-
-**BUILD:**
-
-..  |Notebook 03| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 03
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/03_1_BUILD_USER_gRNA_plasmid.ipynb
-
-
-..  |Notebook 04| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 04
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/04_1_BUILD_Background_strain.ipynb
-
-
-..  |Notebook 05| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 05
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/05_1_BUILD_CombinatorialLibrary_AllStrains.ipynb
-
-
-03. Assembly of a CRISPR plasmid with USER cloning 
-
-|Notebook 03|
-
-04. Construction of the background strain by K/O of G8H and CPR 
-
-|Notebook 04|
-
-05. First combinatorial library was generated for 1280 possible combinations 
-
-|Notebook 05| 
-
-
-
-**TEST:**
-
-
-..  |Notebook 06| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 06
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/06_1_TEST_LibraryCharacterisation.ipynb
-
-
-06. Data processing of LC-MS data and genotyping of the generated strains 
-
-|Notebook 06|  
-
-
-**LEARN:**
-
-..  |Notebook 07| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 07
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/07_1_LEARN_DataAnalysis.ipynb
-
-
-07. Use AutoML to predict the best combinations for a targeted second round of library construction 
-
-|Notebook 07|
-
-
-
-Strictosidine case : Second DBTL cycle
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-
-
-**DESIGN:**
-
-..  |Notebook 08| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 08
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_BUILD_Library2.ipynb
-
-08. Results from the ML can be translated into making a targeted library of strains 
-
-|Notebook 08| 
-
-
-
-**BUILD:**
-
-
-..  |Notebook 09| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 09
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_2_BUILD_CombinatorialLibrary.ipynb
-
-
-09. Shows the construction of a targeted library of strains 
-
-|Notebook 09| 
-
-
-
-
-**TEST:**
-
-..  |Notebook 10| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 10
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/10_2_TEST_Library_Characterization.ipynb
-
-
-
-10. Data processing of LC-MS data like in notebook 6 
-
-|Notebook 10|
-
-
-
-
-**LEARN:**
-
-..  |Notebook 11| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 11
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/11_2_LEARN_DataAnalysisML.ipynb
-
-
-11. Second ML cycle of ML showing how the model increased performance and saturation of best performing strains 
-
-|Notebook 11| 
-
-
-
-Installation
-~~~~~~~~~~~~
-
-.. installation-start
-
-Use pip to install teemi from `PyPI <https://pypi.org/project/teemi/>`__.
-
-::
-
-    $ pip install teemi
-
-
-If you want to develop or if you cloned the repository from our `GitHub <https://github.com/hiyama341/teemi/>`__
-you can install teemi in the following way.
-
-::
-
-    $ pip install -e <path-to-teemi-repo>  
-
-
-You might need to run these commands with administrative
-privileges if you're not using a virtual environment (using ``sudo`` for example).
-Please check the `documentation <https://teemi.readthedocs.io/en/latest/installation.html#>`__
-for further details.
-
-.. installation-end
-
-Documentation and Examples
-~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Documentation is available on through numerous Google Colab notebooks with
-examples on how to use teemi and how we use these notebooks for strain
-construnction. The Colab notebooks can be found here 
-`teemi.notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__. 
-
-* Documentation: https://teemi.readthedocs.io.
-
-
-Contributions
-~~~~~~~~~~~~~
-
-Contributions are very welcome! Check our `guidelines <https://teemi.readthedocs.io/en/latest/contributing.html>`__ for instructions how to contribute.
-
-
-License
-~~~~~~~
-* Free software: MIT license
-
-Credits
--------
-- This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-
-- teemis logo was made by Jonas Krogh Fischer. Check out his `website <http://jkfischerproductions.com/kea/portfolio/index.html>`__. 
+Metadata-Version: 1.2
+Name: teemi
+Version: 0.2.0
+Summary: A Python package for constructing microbial strains
+Home-page: https://github.com/hiyama341/teemi
+Author: Lucas Levassor
+Author-email: lucaslevassor@gmail.com
+License: MIT license
+Description: .. image:: https://raw.githubusercontent.com/hiyama341/teemi/main/pictures/teemi_logo.svg
+          :width: 400
+          :alt: teemi logo 
+        
+        teemi: a python package designed to make HT strain construction reproducible and FAIR
+        -------------------------------------------------------------------------------------
+        
+        .. summary-start
+        
+        .. image:: https://badge.fury.io/py/teemi.svg
+                :target: https://badge.fury.io/py/teemi
+        
+        .. image:: https://github.com/hiyama341/teemi/actions/workflows/main.yml/badge.svg
+                :target: https://github.com/hiyama341/teemi/actions
+        
+        .. image:: https://readthedocs.org/projects/teemi/badge/?version=latest
+                :target: https://teemi.readthedocs.io/en/latest/?version=latest
+                :alt: Documentation Status
+        
+        .. image:: https://img.shields.io/github/license/hiyama341/teemi
+                :target: https://github.com/hiyama341/teemi/blob/main/LICENSE
+        
+        .. image:: https://img.shields.io/pypi/pyversions/teemi.svg
+                :target: https://pypi.org/project/teemi/
+                :alt: Supported Python Versions
+        
+        .. image:: https://codecov.io/gh/hiyama341/teemi/branch/main/graph/badge.svg?token=P4457QACUY 
+                :target: https://codecov.io/gh/hiyama341/teemi
+        
+        .. image:: https://img.shields.io/badge/code%20style-black-black
+                :target: https://black.readthedocs.io/en/stable/
+        
+        .. image:: https://img.shields.io/github/last-commit/hiyama341/teemi
+        
+        
+        
+        What is teemi?
+        ~~~~~~~~~~~~~~
+        
+        **teemi**, named after the Greek goddess of fairness, is a python package designed
+        to make microbial strain construction reproducible and FAIR (Findable, Accessible, 
+        Interoperable, and Reusable). With teemi, you can simulate all steps of 
+        a strain construction cycle, from generating genetic parts to designing 
+        a combinatorial library and keeping track of samples through a commercial
+        Benchling API and a low-level CSV file database. 
+        This tool can be used in literate programming to 
+        increase efficiency and speed in metabolic engineering tasks. 
+        To try teemi, visit our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__.
+        
+        
+        teemi not only simplifies the strain construction process but also offers the 
+        flexibility to adapt to different experimental workflows through its open-source
+        Python platform. This allows for efficient automation of repetitive tasks and
+        a faster pace in metabolic engineering.
+        
+        Our demonstration of teemi in a complex machine learning-guided
+        metabolic engineering task showcases its efficiency 
+        and speed by debottlenecking a crucial step in the strictosidine pathway. 
+        This highlights the versatility and usefulness of this tool in various  
+        biological applications. 
+        
+        Curious about how you can build strains easier and faster with teemi? 
+        Head over to our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__
+        and give it a try.
+        
+        Please cite our paper (in preparation - link tba) if you've used teemi in a scientific publication.
+        
+        .. summary-end
+        
+        
+        Features
+        --------
+        
+        * Combinatorial library generation
+        * HT cloning and transformation workflows
+        * Flowbot One instructions
+        * CSV-based LIMS system as well as integration to Benchling
+        * Genotyping of microbial strains
+        * Advanced Machine Learning of biological datasets with the AutoML `H2O <https://docs.h2o.ai/h2o/latest-stable/h2o-docs/automl.html>`__
+        * Workflows for selecting enzyme homologs
+        * Promoter selection workflows from RNA-seq datasets
+        * Data analysis of large LC-MS datasets along with workflows for analysis
+        
+        
+        Getting started
+        ~~~~~~~~~~~~~~~
+        To get started with making microbial strains in an HT manner please follow the steps below: 
+        
+        1. Install teemi. You will find the necessary information below for installation.
+        
+        2. Check out our `notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__ for inspiration to make HT strain construction with teemi.
+        
+        3. You can start making your own workflows by importing teemi into either Google colab or Jupyter lab/notebooks.
+        
+        
+        Colab notebooks
+        ---------------
+        As a proof of concept we show how teemi and literate programming can be used to streamline bioengineering workflows.
+        These workflows should serve as a guide or a help to build your own workflows and thereby harnessing the power of literate programming with teemi. 
+        
+        Specifically, in this study we present how teemi and literate programming to build simulation-guided, iterative,
+        and evolution-guided laboratory workflows for optimizing strictosidine production in yeast.
+        
+        Below you can find all the notebooks developed in this work. 
+        Just click the Google colab badge to start the workflows. 
+        
+        Strictosidine case : First DBTL cycle
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        **DESIGN:**
+        
+        ..  |Notebook 00| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 00
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/00_1_DESIGN_Homologs.ipynb 
+        
+        ..  |Notebook 01| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 01
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/01_1_DESIGN_Promoters.ipynb
+        
+        ..  |Notebook 02| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 02
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/02_1_DESIGN_Combinatorial_library.ipynb
+            
+        
+        00. Automatically fetch homologs from NCBI from a query in a standardizable and repeatable way 
+        
+        |Notebook 00| 
+        
+        
+        01. Promoters can be selected from RNAseq data and fetched from online database with various quality measurements implemented 
+        
+        |Notebook 01|
+        
+        
+        
+        02. Combinatorial libraries can be generated with the DesignAssembly class along with robot executable intructions 
+        
+        |Notebook 02| 
+        
+        
+        
+        
+        **BUILD:**
+        
+        ..  |Notebook 03| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 03
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/03_1_BUILD_USER_gRNA_plasmid.ipynb
+        
+        
+        ..  |Notebook 04| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 04
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/04_1_BUILD_Background_strain.ipynb
+        
+        
+        ..  |Notebook 05| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 05
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/05_1_BUILD_CombinatorialLibrary_AllStrains.ipynb
+        
+        
+        03. Assembly of a CRISPR plasmid with USER cloning 
+        
+        |Notebook 03|
+        
+        04. Construction of the background strain by K/O of G8H and CPR 
+        
+        |Notebook 04|
+        
+        05. First combinatorial library was generated for 1280 possible combinations 
+        
+        |Notebook 05| 
+        
+        
+        
+        **TEST:**
+        
+        
+        ..  |Notebook 06| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 06
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/06_1_TEST_LibraryCharacterisation.ipynb
+        
+        
+        06. Data processing of LC-MS data and genotyping of the generated strains 
+        
+        |Notebook 06|  
+        
+        
+        **LEARN:**
+        
+        ..  |Notebook 07| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 07
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/07_1_LEARN_DataAnalysis.ipynb
+        
+        
+        07. Use AutoML to predict the best combinations for a targeted second round of library construction 
+        
+        |Notebook 07|
+        
+        
+        
+        Strictosidine case : Second DBTL cycle
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        
+        
+        **DESIGN:**
+        
+        ..  |Notebook 08| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 08
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_BUILD_Library2.ipynb
+        
+        08. Results from the ML can be translated into making a targeted library of strains 
+        
+        |Notebook 08| 
+        
+        
+        
+        **BUILD:**
+        
+        
+        ..  |Notebook 09| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 09
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_2_BUILD_CombinatorialLibrary.ipynb
+        
+        
+        09. Shows the construction of a targeted library of strains 
+        
+        |Notebook 09| 
+        
+        
+        
+        
+        **TEST:**
+        
+        ..  |Notebook 10| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 10
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/10_2_TEST_Library_Characterization.ipynb
+        
+        
+        
+        10. Data processing of LC-MS data like in notebook 6 
+        
+        |Notebook 10|
+        
+        
+        
+        
+        **LEARN:**
+        
+        ..  |Notebook 11| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 11
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/11_2_LEARN_DataAnalysisML.ipynb
+        
+        
+        11. Second ML cycle of ML showing how the model increased performance and saturation of best performing strains 
+        
+        |Notebook 11| 
+        
+        
+        
+        Installation
+        ~~~~~~~~~~~~
+        
+        .. installation-start
+        
+        Use pip to install teemi from `PyPI <https://pypi.org/project/teemi/>`__.
+        
+        ::
+        
+            $ pip install teemi
+        
+        
+        If you want to develop or if you cloned the repository from our `GitHub <https://github.com/hiyama341/teemi/>`__
+        you can install teemi in the following way.
+        
+        ::
+        
+            $ pip install -e <path-to-teemi-repo>  
+        
+        
+        You might need to run these commands with administrative
+        privileges if you're not using a virtual environment (using ``sudo`` for example).
+        Please check the `documentation <https://teemi.readthedocs.io/en/latest/installation.html#>`__
+        for further details.
+        
+        .. installation-end
+        
+        Documentation and Examples
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        Documentation is available on through numerous Google Colab notebooks with
+        examples on how to use teemi and how we use these notebooks for strain
+        construnction. The Colab notebooks can be found here 
+        `teemi.notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__. 
+        
+        * Documentation: https://teemi.readthedocs.io.
+        
+        
+        Contributions
+        ~~~~~~~~~~~~~
+        
+        Contributions are very welcome! Check our `guidelines <https://teemi.readthedocs.io/en/latest/contributing.html>`__ for instructions how to contribute.
+        
+        
+        License
+        ~~~~~~~
+        * Free software: MIT license
+        
+        Credits
+        -------
+        - This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+        
+        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
+        
+        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+        
+        - teemis logo was made by Jonas Krogh Fischer. Check out his `website <http://jkfischerproductions.com/kea/portfolio/index.html>`__. 
+        
+        History
+        -------
+        
+        0.1.0 (2023-01-02)
+        ------------------
+        
+        * First release on PyPI.
+        
+        
+        0.2.0 (2023-31-05)
+        ------------------
+        
+        * New submodules: CRISPRsequencecutter, sequence_finder. 
+        
+        CRISPRSequenceCutter is a dataclass that is used to cut DNA through CRISPR-cas9 double-stranded break.
+        SequenceFinder is a dataclass that finds upstream and downstream sequences from a sequence input, annotates them and saves them.
+        
+Keywords: teemi
+Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
```

### Comparing `teemi-0.1.4/setup.py` & `teemi-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/teemi/build/PCR.py` & `teemi-0.2.0/teemi/build/PCR.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/teemi/build/containers_wells_picklists.py` & `teemi-0.2.0/teemi/build/containers_wells_picklists.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/teemi/build/robot_assembly.py` & `teemi-0.2.0/teemi/build/robot_assembly.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/teemi/build/transformation.py` & `teemi-0.2.0/teemi/build/transformation.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,70 +72,67 @@
     """
     if initialOD >= 0 and time >= 0:
         return round(initialOD * 2 ** (time * td), 3)
     else:
         return "non-valid_input"
 
 
-def time_to_inculate(
-    initialOD=0.0025, td=0.4, verbose=False, transformation_time: int = 12, plot = False
-):
-
-    """Calculates when a starter culture is ready to be inoculated
-     with a transformation mixture.
+def time_to_inoculate(
+    initialOD: float, td: float, verbose: bool, transformation_time: int, target_OD: float, plot:bool=True):
+    """Calculates when a starter culture is ready to be transformed.
 
     Parameters
     ----------
     initialOD : float
+        the OD that you have you have diluted to e.g. 0.0025
     td : float
-        is doubling time
+        Doubling time - you can find this online or find experimentally.
     transformation_time : int
-        The time you want to transform
+        The time you want to transform. For example could be at 8 in the morning. 
     verbose : Bool
         Provides extra information
+    target_OD: float
+        The target optical density that needs to be reached before transformation.
+    plot : bool
+        If you want to visualize the plot
 
     Returns
     -------
-    A plot of cell growth at different td
+    A plot of cell growth at different td along with text about the transformation.
 
     Notes
     -----
     This is used to calculate when the cells should be used for transformation.
     For example:
     OD_1 = 1 * 10^7 cells / ml
-    For a succesfull S.cerevisiae transformation between 1 to 2 × 10^7 cells/ml should be used
-    Normal doupling time is between 3-6 hours
+    For a successful S.cerevisiae transformation between 1 to 2 × 10^7 cells/ml should be used
+    Normal doubling time is between 3-6 hours
 
 
     """
     if verbose:
         print("GOAL: to get enough cells in exponential phase for transformation")
-    print("Assumed that: ")
+    print("Assumptions:")
     print(
-        "- transformation time "
-        + str(transformation_time)
-        + " (reached OD=1 the day after)"
+        f"- Transformation time: {transformation_time} (aka time when the target OD is reached)"
     )
 
-    times = list(range(0, 37))
-    ods_025_3 = [ODtime(initialOD, time, td=0.3) for time in times]
+    times = list(range(0, 30))
+    ods_025_3 = [ODtime(initialOD, time, td=td-0.1) for time in times]
     ods_025_input = [ODtime(initialOD, time, td=td) for time in times]
-    ods_025_5 = [ODtime(initialOD, time, td=0.5) for time in times]
+    ods_025_5 = [ODtime(initialOD, time, td=td+0.1) for time in times]
 
-    if plot: 
+    if plot:
         fig = plt.figure()
         ax = plt.axes()
-
-        # ax.set_xlim(lims)
-        ax.set_ylim([0, 2.2])
-        ax.plot(times, [2] * len(times), "r-", label="end of exponential phase")
-        ax.plot(times, [1] * len(times), "k-", label="target")
-        ax.plot(times, ods_025_3, label="iOD=" + str(initialOD) + ", td=0.3")
+        ax.set_ylim([0, 2.0])
+        ax.plot(times, [target_OD] * len(times), "k-", label="target")
+        ax.plot(times, ods_025_3, label="iOD=" + str(initialOD) + ", td=" + str(round(td-0.1, 1)))
         ax.plot(times, ods_025_input, label="iOD=" + str(initialOD) + ", td=" + str(td))
-        ax.plot(times, ods_025_5, label="iOD=" + str(initialOD) + ", td=0.5")
+        ax.plot(times, ods_025_5, label="iOD=" + str(initialOD) + ", td=" + str(td+0.1))
 
         plt.xlabel("time, h^-1")
         plt.ylabel("OD")
         plt.legend()
         plt.show()
 
     def inoculation_time(times, ods):
@@ -144,51 +141,40 @@
             idx = A.searchsorted(target)
             idx = np.clip(idx, 1, len(A) - 1)
             left = A[idx - 1]
             right = A[idx]
             idx -= target - left < right - target
             return idx
 
-        # In how many hours will the cells have reached OD 1?
+        # In how many hours will the cells have reached the
         hours_to_OD1 = times[find_closest(np.array(ods), 1)]
-        print("Hours to OD = 1: \t" + str(hours_to_OD1) + " hours")
+        print("Hours to target OD: \t" + str(hours_to_OD1) + " hours")
 
         ### When do u need to innoculate?
-        when_to_inoculate = transformation_time - hours_to_OD1
-
-        if when_to_inoculate < 0:
-            print("Transformation time has been set to ", transformation_time)
-            print(
-                "Time of inoculation: \t"
-                + str(when_to_inoculate + 24)
-                + " (the day before)"
+        when_to_inoculate = timedelta(hours=transformation_time) - timedelta(hours=hours_to_OD1)
+        print("Transformation time has been set to ", transformation_time)
+        print("Time of inoculation: \t"
+                + str(when_to_inoculate), "(aka when to start growing the cells)"
             )
 
-        else:
-            print("Transformation time has been set to ", transformation_time)
-            print(
-                "Time of inoculation: \t" + str(when_to_inoculate) + "(the day before)"
-            )
-
-        # If i innoculate now?
-
+        # If i inoculate now?
+        from datetime import datetime
         print(
-            "\nIf you innoculate now, the cells will have reached OD= 1 by:  ",
+            "\nNB: If you inoculated now, the cells will have reached the target OD by:  ",
             datetime.now() + timedelta(hours=hours_to_OD1),
         )
 
     inoculation_time(times, ods_025_input)
 
     if verbose:
         print()
         print(
             "How to hit initialOD = 0.0025 (e.g. from colony)? Guess. Inoculate 9/10 + 1/10 'normal' colony per ~10 ml"
         )
-        print("How much volume? ~2 ml per transformation")
-
+        print("How much volume? ~2 ml per transformation.")
 
 def transformation_mix(
     reaction_names, reaction_participants, wanted_amounts, water_dna_p_reac, media=""
 ):
 
     """Makes a pandas dataframe of the parts (their location)
      that needs to be put into the transformation mixes.
@@ -211,15 +197,15 @@
     pandas.DataFrame
         with a transformation scheme showing which parts should be
         mixed for each reaction including positive and negative
         controls.
 
     Examples
     --------
-    # 1. Mention which reacion names you have
+    # 1. Mention which reaction names you have
     reaction_names = ["insert", "n.ctr", "n.ctr", "n.ctr", "p. ctr"]
 
     # 2. Add reaction reaction_participants
     reaction_participants = [[vector, gRNA1_pcr_prod,gRNA2_pcr_prod], #the insert we want
                      [vector],                                        #negative control
                      [gRNA1_pcr_prod],                                #negative control
                      [gRNA2_pcr_prod],                                #negative control
```

### Comparing `teemi-0.1.4/teemi/design/cloning.py` & `teemi-0.2.0/teemi/design/cloning.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/teemi/design/combinatorial_design.py` & `teemi-0.2.0/teemi/design/combinatorial_design.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/teemi/design/fetch_sequences.py` & `teemi-0.2.0/teemi/design/fetch_sequences.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/teemi/design/retrieve_gene_homologs.py` & `teemi-0.2.0/teemi/design/retrieve_gene_homologs.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/teemi/design/teselagen_helpers.py` & `teemi-0.2.0/teemi/design/teselagen_helpers.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/teemi/learn/auto_ml.py` & `teemi-0.2.0/teemi/learn/auto_ml.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/teemi/learn/plotting.py` & `teemi-0.2.0/teemi/learn/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,15 @@
             yerr=error_bar,
             fmt="o",
             color="black",
         )  # ms = 2)
 
     # add horisontal line
     if horisontal_line:
-        plt.axhline(y=100, color="black", linestyle="-")
+        plt.axhline(y=100, color = 'black', linestyle = 'dashed')
 
     # Title and labels
     if title is not None:
         ax.set_title(title, size=30, fontname="Helvetica")
     if x_label is not None:
         ax.set_xlabel(x_label, size=20, fontname="Helvetica")
     if y_label is not None:
@@ -298,14 +298,15 @@
     path: str = "",
     color="white",
     title=None,
     x_label=None,
     y_label=None,
     size_height: int = 10,
     size_length: int = 8,
+    legend= False
 ) -> None:
     """Plotting a horisontal_bar_plot .
 
     Parameters
     ----------
     x : list
         x coordinates
@@ -332,14 +333,21 @@
 
     # Plot
     plt.barh(x, y, edgecolor="black", color=color)  # white # '#deebf7'
 
     # Change x labels rotation
     ax.tick_params(rotation=90)
 
+    # LEGEND
+    if legend: 
+        lineOne, = ax.plot([], label='dbtl_2')
+        lineTwo, = ax.plot([], label='dbtl_1')
+        ax.legend(handles=[lineOne, lineTwo], loc='best')
+
+
     # remove gridlines
     ax.grid(False)
 
     # Title and labels
     if title is not None:
         ax.set_title(title, size=30, fontname="Helvetica")
     if x_label is not None:
@@ -348,23 +356,23 @@
         ax.set_ylabel(y_label, size=20, fontname="Helvetica")
 
     # Background
     ax.set_facecolor("white")
 
     # add horisontal line
     if vertical_line:
-        plt.axvline(x=100, color="black", linestyle="-")
+        plt.axvline(x=100, color="black", linestyle='dashed')
 
     # rotate sticks
     ax.tick_params(rotation=0)
 
-    ## adding the labels on the bar
+    # ## adding the labels on the bar
     for c in ax.containers:
         ax.bar_label(c, padding=10)
-
+    #remove spines
     ax.spines["right"].set_visible(False)
     ax.spines["top"].set_visible(False)
     ax.spines["left"].set_visible(False)
     ax.spines["bottom"].set_visible(False)
 
     # SIze matters
     fig = mpl.pyplot.gcf()
@@ -377,28 +385,32 @@
 
 
 def correlation_plot(dataframe, x: str, y: str, 
     save_pdf:bool =True, 
     path: str = "", 
     title: str = '',
     size_height: int = 10,
-    size_length: int = 10) -> None:
+    size_length: int = 10,
+    y_axis_range: list = [0,1],
+    x_axis_range: list = [0,1]) -> None:
     """Plotting a correlation_plot.
 
     Parameters
     ----------
     dataframe : pd.DataFrame
     x : str
         x coordinates
     y : str
         y coordinates
     save_pdf : bool
     path : str
     size_height : int
     size_length : int
+    x_axis_range : list
+    y_axis_range : list
 
     Returns
     -------
     correlation_plot"""
 
     # set seaborn plotting aesthetics as default
     sns.set_context("paper", font_scale=2.0, rc={"lines.linewidth": 1.5})
@@ -432,14 +444,18 @@
     # add title 
     ax.set_title(title)
 
     # SIze matters
     fig = mpl.pyplot.gcf()
     fig.set_size_inches(size_height, size_length)
     
+    # change y-axis range 
+    plt.xlim(x_axis_range)
+    plt.ylim(y_axis_range)
+
 
     if save_pdf and path != "":
         plt.savefig(path + ".pdf", format="pdf", dpi=300, bbox_inches="tight")
 
     plt.show()
 
 
@@ -497,15 +513,15 @@
 
     # SIze matters
     fig = mpl.pyplot.gcf()
     fig.set_size_inches(size_length, size_height )
 
     if horisontal_line:
         # normalized line
-        ax.axhline(100)
+        ax.axhline(100, color = 'black', linestyle = 'dashed')
 
     if save_pdf == True and path != "":
         plt.savefig(path + ".pdf", format="pdf", dpi=300)
     
     plt.show()
 
 
@@ -752,15 +768,15 @@
     # Add labels and titel
     ax.set_ylabel(y_label, size = 20, fontname='Helvetica')
     ax.set_xlabel(x_label, size = 30, fontname='Helvetica')
     ax.set_title(title, size = 30, fontname='Helvetica')
     
     if axhline: 
         # add horisontal line
-        plt.axhline(y = 100, color = 'black', linestyle = '-')
+        plt.axhline(y = 100, color = 'black', linestyle = 'dashed')
 
     # Set color 
     ax.set_facecolor("white")
 
     white_patch = mpatches.Patch(color='white', label=category_labels[0])
     black_patch = mpatches.Patch(color='black', label=category_labels[1])
     ax.legend(handles=[white_patch,black_patch ], fontsize = 20, frameon=False)
```

### Comparing `teemi-0.1.4/teemi/lims/benchling_api.py` & `teemi-0.2.0/teemi/lims/benchling_api.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/teemi/lims/csv_database.py` & `teemi-0.2.0/teemi/lims/csv_database.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/teemi/utils.py` & `teemi-0.2.0/teemi/utils.py`

 * *Files identical despite different names*

### Comparing `teemi-0.1.4/teemi.egg-info/PKG-INFO` & `teemi-0.2.0/teemi.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,346 +1,354 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: teemi
-Version: 0.1.4
+Version: 0.2.0
 Summary: A Python package for constructing microbial strains
 Home-page: https://github.com/hiyama341/teemi
 Author: Lucas Levassor
 Author-email: lucaslevassor@gmail.com
 License: MIT license
+Description: .. image:: https://raw.githubusercontent.com/hiyama341/teemi/main/pictures/teemi_logo.svg
+          :width: 400
+          :alt: teemi logo 
+        
+        teemi: a python package designed to make HT strain construction reproducible and FAIR
+        -------------------------------------------------------------------------------------
+        
+        .. summary-start
+        
+        .. image:: https://badge.fury.io/py/teemi.svg
+                :target: https://badge.fury.io/py/teemi
+        
+        .. image:: https://github.com/hiyama341/teemi/actions/workflows/main.yml/badge.svg
+                :target: https://github.com/hiyama341/teemi/actions
+        
+        .. image:: https://readthedocs.org/projects/teemi/badge/?version=latest
+                :target: https://teemi.readthedocs.io/en/latest/?version=latest
+                :alt: Documentation Status
+        
+        .. image:: https://img.shields.io/github/license/hiyama341/teemi
+                :target: https://github.com/hiyama341/teemi/blob/main/LICENSE
+        
+        .. image:: https://img.shields.io/pypi/pyversions/teemi.svg
+                :target: https://pypi.org/project/teemi/
+                :alt: Supported Python Versions
+        
+        .. image:: https://codecov.io/gh/hiyama341/teemi/branch/main/graph/badge.svg?token=P4457QACUY 
+                :target: https://codecov.io/gh/hiyama341/teemi
+        
+        .. image:: https://img.shields.io/badge/code%20style-black-black
+                :target: https://black.readthedocs.io/en/stable/
+        
+        .. image:: https://img.shields.io/github/last-commit/hiyama341/teemi
+        
+        
+        
+        What is teemi?
+        ~~~~~~~~~~~~~~
+        
+        **teemi**, named after the Greek goddess of fairness, is a python package designed
+        to make microbial strain construction reproducible and FAIR (Findable, Accessible, 
+        Interoperable, and Reusable). With teemi, you can simulate all steps of 
+        a strain construction cycle, from generating genetic parts to designing 
+        a combinatorial library and keeping track of samples through a commercial
+        Benchling API and a low-level CSV file database. 
+        This tool can be used in literate programming to 
+        increase efficiency and speed in metabolic engineering tasks. 
+        To try teemi, visit our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__.
+        
+        
+        teemi not only simplifies the strain construction process but also offers the 
+        flexibility to adapt to different experimental workflows through its open-source
+        Python platform. This allows for efficient automation of repetitive tasks and
+        a faster pace in metabolic engineering.
+        
+        Our demonstration of teemi in a complex machine learning-guided
+        metabolic engineering task showcases its efficiency 
+        and speed by debottlenecking a crucial step in the strictosidine pathway. 
+        This highlights the versatility and usefulness of this tool in various  
+        biological applications. 
+        
+        Curious about how you can build strains easier and faster with teemi? 
+        Head over to our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__
+        and give it a try.
+        
+        Please cite our paper (in preparation - link tba) if you've used teemi in a scientific publication.
+        
+        .. summary-end
+        
+        
+        Features
+        --------
+        
+        * Combinatorial library generation
+        * HT cloning and transformation workflows
+        * Flowbot One instructions
+        * CSV-based LIMS system as well as integration to Benchling
+        * Genotyping of microbial strains
+        * Advanced Machine Learning of biological datasets with the AutoML `H2O <https://docs.h2o.ai/h2o/latest-stable/h2o-docs/automl.html>`__
+        * Workflows for selecting enzyme homologs
+        * Promoter selection workflows from RNA-seq datasets
+        * Data analysis of large LC-MS datasets along with workflows for analysis
+        
+        
+        Getting started
+        ~~~~~~~~~~~~~~~
+        To get started with making microbial strains in an HT manner please follow the steps below: 
+        
+        1. Install teemi. You will find the necessary information below for installation.
+        
+        2. Check out our `notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__ for inspiration to make HT strain construction with teemi.
+        
+        3. You can start making your own workflows by importing teemi into either Google colab or Jupyter lab/notebooks.
+        
+        
+        Colab notebooks
+        ---------------
+        As a proof of concept we show how teemi and literate programming can be used to streamline bioengineering workflows.
+        These workflows should serve as a guide or a help to build your own workflows and thereby harnessing the power of literate programming with teemi. 
+        
+        Specifically, in this study we present how teemi and literate programming to build simulation-guided, iterative,
+        and evolution-guided laboratory workflows for optimizing strictosidine production in yeast.
+        
+        Below you can find all the notebooks developed in this work. 
+        Just click the Google colab badge to start the workflows. 
+        
+        Strictosidine case : First DBTL cycle
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        **DESIGN:**
+        
+        ..  |Notebook 00| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 00
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/00_1_DESIGN_Homologs.ipynb 
+        
+        ..  |Notebook 01| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 01
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/01_1_DESIGN_Promoters.ipynb
+        
+        ..  |Notebook 02| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 02
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/02_1_DESIGN_Combinatorial_library.ipynb
+            
+        
+        00. Automatically fetch homologs from NCBI from a query in a standardizable and repeatable way 
+        
+        |Notebook 00| 
+        
+        
+        01. Promoters can be selected from RNAseq data and fetched from online database with various quality measurements implemented 
+        
+        |Notebook 01|
+        
+        
+        
+        02. Combinatorial libraries can be generated with the DesignAssembly class along with robot executable intructions 
+        
+        |Notebook 02| 
+        
+        
+        
+        
+        **BUILD:**
+        
+        ..  |Notebook 03| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 03
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/03_1_BUILD_USER_gRNA_plasmid.ipynb
+        
+        
+        ..  |Notebook 04| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 04
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/04_1_BUILD_Background_strain.ipynb
+        
+        
+        ..  |Notebook 05| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 05
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/05_1_BUILD_CombinatorialLibrary_AllStrains.ipynb
+        
+        
+        03. Assembly of a CRISPR plasmid with USER cloning 
+        
+        |Notebook 03|
+        
+        04. Construction of the background strain by K/O of G8H and CPR 
+        
+        |Notebook 04|
+        
+        05. First combinatorial library was generated for 1280 possible combinations 
+        
+        |Notebook 05| 
+        
+        
+        
+        **TEST:**
+        
+        
+        ..  |Notebook 06| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 06
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/06_1_TEST_LibraryCharacterisation.ipynb
+        
+        
+        06. Data processing of LC-MS data and genotyping of the generated strains 
+        
+        |Notebook 06|  
+        
+        
+        **LEARN:**
+        
+        ..  |Notebook 07| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 07
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/07_1_LEARN_DataAnalysis.ipynb
+        
+        
+        07. Use AutoML to predict the best combinations for a targeted second round of library construction 
+        
+        |Notebook 07|
+        
+        
+        
+        Strictosidine case : Second DBTL cycle
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        
+        
+        **DESIGN:**
+        
+        ..  |Notebook 08| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 08
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_BUILD_Library2.ipynb
+        
+        08. Results from the ML can be translated into making a targeted library of strains 
+        
+        |Notebook 08| 
+        
+        
+        
+        **BUILD:**
+        
+        
+        ..  |Notebook 09| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 09
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_2_BUILD_CombinatorialLibrary.ipynb
+        
+        
+        09. Shows the construction of a targeted library of strains 
+        
+        |Notebook 09| 
+        
+        
+        
+        
+        **TEST:**
+        
+        ..  |Notebook 10| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 10
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/10_2_TEST_Library_Characterization.ipynb
+        
+        
+        
+        10. Data processing of LC-MS data like in notebook 6 
+        
+        |Notebook 10|
+        
+        
+        
+        
+        **LEARN:**
+        
+        ..  |Notebook 11| image:: https://colab.research.google.com/assets/colab-badge.svg
+            :alt: Notebook 11
+            :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/11_2_LEARN_DataAnalysisML.ipynb
+        
+        
+        11. Second ML cycle of ML showing how the model increased performance and saturation of best performing strains 
+        
+        |Notebook 11| 
+        
+        
+        
+        Installation
+        ~~~~~~~~~~~~
+        
+        .. installation-start
+        
+        Use pip to install teemi from `PyPI <https://pypi.org/project/teemi/>`__.
+        
+        ::
+        
+            $ pip install teemi
+        
+        
+        If you want to develop or if you cloned the repository from our `GitHub <https://github.com/hiyama341/teemi/>`__
+        you can install teemi in the following way.
+        
+        ::
+        
+            $ pip install -e <path-to-teemi-repo>  
+        
+        
+        You might need to run these commands with administrative
+        privileges if you're not using a virtual environment (using ``sudo`` for example).
+        Please check the `documentation <https://teemi.readthedocs.io/en/latest/installation.html#>`__
+        for further details.
+        
+        .. installation-end
+        
+        Documentation and Examples
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        Documentation is available on through numerous Google Colab notebooks with
+        examples on how to use teemi and how we use these notebooks for strain
+        construnction. The Colab notebooks can be found here 
+        `teemi.notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__. 
+        
+        * Documentation: https://teemi.readthedocs.io.
+        
+        
+        Contributions
+        ~~~~~~~~~~~~~
+        
+        Contributions are very welcome! Check our `guidelines <https://teemi.readthedocs.io/en/latest/contributing.html>`__ for instructions how to contribute.
+        
+        
+        License
+        ~~~~~~~
+        * Free software: MIT license
+        
+        Credits
+        -------
+        - This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+        
+        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
+        
+        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+        
+        - teemis logo was made by Jonas Krogh Fischer. Check out his `website <http://jkfischerproductions.com/kea/portfolio/index.html>`__. 
+        
+        History
+        -------
+        
+        0.1.0 (2023-01-02)
+        ------------------
+        
+        * First release on PyPI.
+        
+        
+        0.2.0 (2023-31-05)
+        ------------------
+        
+        * New submodules: CRISPRsequencecutter, sequence_finder. 
+        
+        CRISPRSequenceCutter is a dataclass that is used to cut DNA through CRISPR-cas9 double-stranded break.
+        SequenceFinder is a dataclass that finds upstream and downstream sequences from a sequence input, annotates them and saves them.
+        
 Keywords: teemi
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-.. image:: https://raw.githubusercontent.com/hiyama341/teemi/main/pictures/teemi_logo.svg
-  :width: 400
-  :alt: teemi logo 
-
-teemi: a python package designed to make HT strain construction reproducible and FAIR
--------------------------------------------------------------------------------------
-
-.. summary-start
-
-.. image:: https://badge.fury.io/py/teemi.svg
-        :target: https://badge.fury.io/py/teemi
-
-.. image:: https://github.com/hiyama341/teemi/actions/workflows/main.yml/badge.svg
-        :target: https://github.com/hiyama341/teemi/actions
-
-.. image:: https://readthedocs.org/projects/teemi/badge/?version=latest
-        :target: https://teemi.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-.. image:: https://img.shields.io/github/license/hiyama341/teemi
-        :target: https://github.com/hiyama341/teemi/blob/main/LICENSE
-
-.. image:: https://img.shields.io/pypi/pyversions/teemi.svg
-        :target: https://pypi.org/project/teemi/
-        :alt: Supported Python Versions
-
-.. image:: https://codecov.io/gh/hiyama341/teemi/branch/main/graph/badge.svg?token=P4457QACUY 
-        :target: https://codecov.io/gh/hiyama341/teemi
-
-.. image:: https://img.shields.io/badge/code%20style-black-black
-        :target: https://black.readthedocs.io/en/stable/
-
-.. image:: https://img.shields.io/github/last-commit/hiyama341/teemi
-
-
-
-What is teemi?
-~~~~~~~~~~~~~~
-
-**teemi**, named after the Greek goddess of fairness, is a python package designed
-to make microbial strain construction reproducible and FAIR (Findable, Accessible, 
-Interoperable, and Reusable). With teemi, you can simulate all steps of 
-a strain construction cycle, from generating genetic parts to designing 
-a combinatorial library and keeping track of samples through a commercial
-Benchling API and a low-level CSV file database. 
-This tool can be used in literate programming to 
-increase efficiency and speed in metabolic engineering tasks. 
-To try teemi, visit our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__.
-
-
-teemi not only simplifies the strain construction process but also offers the 
-flexibility to adapt to different experimental workflows through its open-source
-Python platform. This allows for efficient automation of repetitive tasks and
-a faster pace in metabolic engineering.
-
-Our demonstration of teemi in a complex machine learning-guided
-metabolic engineering task showcases its efficiency 
-and speed by debottlenecking a crucial step in the strictosidine pathway. 
-This highlights the versatility and usefulness of this tool in various  
-biological applications. 
-
-Curious about how you can build strains easier and faster with teemi? 
-Head over to our `Google Colab notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__
-and give it a try.
-
-Please cite our paper (in preparation - link tba) if you've used teemi in a scientific publication.
-
-.. summary-end
-
-
-Features
---------
-
-* Combinatorial library generation
-* HT cloning and transformation workflows
-* Flowbot One instructions
-* CSV-based LIMS system as well as integration to Benchling
-* Genotyping of microbial strains
-* Advanced Machine Learning of biological datasets with the AutoML `H2O <https://docs.h2o.ai/h2o/latest-stable/h2o-docs/automl.html>`__
-* Workflows for selecting enzyme homologs
-* Promoter selection workflows from RNA-seq datasets
-* Data analysis of large LC-MS datasets along with workflows for analysis
-
-
-Getting started
-~~~~~~~~~~~~~~~
-To get started with making microbial strains in an HT manner please follow the steps below: 
-
-1. Install teemi. You will find the necessary information below for installation.
-
-2. Check out our `notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__ for inspiration to make HT strain construction with teemi.
-
-3. You can start making your own workflows by importing teemi into either Google colab or Jupyter lab/notebooks.
-
-
-Colab notebooks
----------------
-As a proof of concept we show how teemi and literate programming can be used to streamline bioengineering workflows.
-These workflows should serve as a guide or a help to build your own workflows and thereby harnessing the power of literate programming with teemi. 
-
-Specifically, in this study we present how teemi and literate programming to build simulation-guided, iterative,
-and evolution-guided laboratory workflows for optimizing strictosidine production in yeast.
-
-Below you can find all the notebooks developed in this work. 
-Just click the Google colab badge to start the workflows. 
-
-Strictosidine case : First DBTL cycle
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-**DESIGN:**
-
-..  |Notebook 00| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 00
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/00_1_DESIGN_Homologs.ipynb 
-
-..  |Notebook 01| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 01
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/01_1_DESIGN_Promoters.ipynb
-
-..  |Notebook 02| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 02
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/02_1_DESIGN_Combinatorial_library.ipynb
-    
-
-00. Automatically fetch homologs from NCBI from a query in a standardizable and repeatable way 
-
-|Notebook 00| 
-
-
-01. Promoters can be selected from RNAseq data and fetched from online database with various quality measurements implemented 
-
-|Notebook 01|
-
-
-
-02. Combinatorial libraries can be generated with the DesignAssembly class along with robot executable intructions 
-
-|Notebook 02| 
-
-
-
-
-**BUILD:**
-
-..  |Notebook 03| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 03
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/03_1_BUILD_USER_gRNA_plasmid.ipynb
-
-
-..  |Notebook 04| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 04
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/04_1_BUILD_Background_strain.ipynb
-
-
-..  |Notebook 05| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 05
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/05_1_BUILD_CombinatorialLibrary_AllStrains.ipynb
-
-
-03. Assembly of a CRISPR plasmid with USER cloning 
-
-|Notebook 03|
-
-04. Construction of the background strain by K/O of G8H and CPR 
-
-|Notebook 04|
-
-05. First combinatorial library was generated for 1280 possible combinations 
-
-|Notebook 05| 
-
-
-
-**TEST:**
-
-
-..  |Notebook 06| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 06
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/06_1_TEST_LibraryCharacterisation.ipynb
-
-
-06. Data processing of LC-MS data and genotyping of the generated strains 
-
-|Notebook 06|  
-
-
-**LEARN:**
-
-..  |Notebook 07| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 07
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/07_1_LEARN_DataAnalysis.ipynb
-
-
-07. Use AutoML to predict the best combinations for a targeted second round of library construction 
-
-|Notebook 07|
-
-
-
-Strictosidine case : Second DBTL cycle
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-
-
-**DESIGN:**
-
-..  |Notebook 08| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 08
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_BUILD_Library2.ipynb
-
-08. Results from the ML can be translated into making a targeted library of strains 
-
-|Notebook 08| 
-
-
-
-**BUILD:**
-
-
-..  |Notebook 09| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 09
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/09_2_BUILD_CombinatorialLibrary.ipynb
-
-
-09. Shows the construction of a targeted library of strains 
-
-|Notebook 09| 
-
-
-
-
-**TEST:**
-
-..  |Notebook 10| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 10
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/10_2_TEST_Library_Characterization.ipynb
-
-
-
-10. Data processing of LC-MS data like in notebook 6 
-
-|Notebook 10|
-
-
-
-
-**LEARN:**
-
-..  |Notebook 11| image:: https://colab.research.google.com/assets/colab-badge.svg
-    :alt: Notebook 11
-    :target: https://colab.research.google.com/github/hiyama341/teemi/blob/main/colab_notebooks/11_2_LEARN_DataAnalysisML.ipynb
-
-
-11. Second ML cycle of ML showing how the model increased performance and saturation of best performing strains 
-
-|Notebook 11| 
-
-
-
-Installation
-~~~~~~~~~~~~
-
-.. installation-start
-
-Use pip to install teemi from `PyPI <https://pypi.org/project/teemi/>`__.
-
-::
-
-    $ pip install teemi
-
-
-If you want to develop or if you cloned the repository from our `GitHub <https://github.com/hiyama341/teemi/>`__
-you can install teemi in the following way.
-
-::
-
-    $ pip install -e <path-to-teemi-repo>  
-
-
-You might need to run these commands with administrative
-privileges if you're not using a virtual environment (using ``sudo`` for example).
-Please check the `documentation <https://teemi.readthedocs.io/en/latest/installation.html#>`__
-for further details.
-
-.. installation-end
-
-Documentation and Examples
-~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Documentation is available on through numerous Google Colab notebooks with
-examples on how to use teemi and how we use these notebooks for strain
-construnction. The Colab notebooks can be found here 
-`teemi.notebooks <https://github.com/hiyama341/teemi/tree/main/colab_notebooks>`__. 
-
-* Documentation: https://teemi.readthedocs.io.
-
-
-Contributions
-~~~~~~~~~~~~~
-
-Contributions are very welcome! Check our `guidelines <https://teemi.readthedocs.io/en/latest/contributing.html>`__ for instructions how to contribute.
-
-
-License
-~~~~~~~
-* Free software: MIT license
-
-Credits
--------
-- This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-
-- teemis logo was made by Jonas Krogh Fischer. Check out his `website <http://jkfischerproductions.com/kea/portfolio/index.html>`__. 
-
-History
--------
-
-0.1.0 (2023-01-02)
-------------------
-
-* First release on PyPI.
```

### Comparing `teemi-0.1.4/teemi.egg-info/SOURCES.txt` & `teemi-0.2.0/teemi.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,21 +17,24 @@
 teemi.egg-info/requires.txt
 teemi.egg-info/top_level.txt
 teemi/build/PCR.py
 teemi/build/__init__.py
 teemi/build/containers_wells_picklists.py
 teemi/build/robot_assembly.py
 teemi/build/transformation.py
+teemi/design/CRISPRsequencecutter.py
 teemi/design/__init__.py
 teemi/design/cloning.py
 teemi/design/combinatorial_design.py
 teemi/design/fetch_sequences.py
 teemi/design/retrieve_gene_homologs.py
+teemi/design/sequence_finder.py
 teemi/design/teselagen_helpers.py
 teemi/learn/__init__.py
 teemi/learn/auto_ml.py
 teemi/learn/plotting.py
 teemi/lims/__init__.py
 teemi/lims/benchling_api.py
 teemi/lims/csv_database.py
 teemi/test/__init__.py
+teemi/test/data_wrangling.py
 teemi/test/genotyping.py
```

### Comparing `teemi-0.1.4/versioneer.py` & `teemi-0.2.0/versioneer.py`

 * *Files identical despite different names*

