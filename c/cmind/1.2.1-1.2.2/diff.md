# Comparing `tmp/cmind-1.2.1.tar.gz` & `tmp/cmind-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-1.2.1.tar", last modified: Fri May 26 16:31:24 2023, max compression
+gzip compressed data, was "cmind-1.2.2.tar", last modified: Tue May 30 19:25:32 2023, max compression
```

## Comparing `cmind-1.2.1.tar` & `cmind-1.2.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.816393 cmind-1.2.1/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6042 2023-05-26 16:31:24.816393 cmind-1.2.1/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     5112 2023-05-25 12:13:31.000000 cmind-1.2.1/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.806393 cmind-1.2.1/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-05-26 16:24:59.000000 cmind-1.2.1/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4908 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    46002 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4213 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    24428 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9326 2023-05-26 16:24:59.000000 cmind-1.2.1/cmind/index.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.806393 cmind-1.2.1/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.806393 cmind-1.2.1/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.816393 cmind-1.2.1/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1858 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.816393 cmind-1.2.1/cmind/repo/automation/ck/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1020 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/ck/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/ck/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/ck/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.816393 cmind-1.2.1/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1032 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.816393 cmind-1.2.1/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.816393 cmind-1.2.1/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8771 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    31178 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    18709 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    41400 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.806393 cmind-1.2.1/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6042 2023-05-26 16:31:24.000000 cmind-1.2.1/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1222 2023-05-26 16:31:24.000000 cmind-1.2.1/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-26 16:31:24.000000 cmind-1.2.1/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       60 2023-05-26 16:31:24.000000 cmind-1.2.1/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-25 12:15:08.000000 cmind-1.2.1/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-05-26 16:31:24.000000 cmind-1.2.1/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-05-26 16:31:24.000000 cmind-1.2.1/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-05-26 16:31:24.816393 cmind-1.2.1/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2668 2023-05-25 12:13:31.000000 cmind-1.2.1/setup.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.316357 cmind-1.2.2/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6057 2023-05-30 19:25:32.316357 cmind-1.2.2/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     5127 2023-05-30 19:25:20.000000 cmind-1.2.2/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.306357 cmind-1.2.2/cmind/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-05-30 19:25:20.000000 cmind-1.2.2/cmind/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/__main__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4908 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/artifact.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    46002 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/automation.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4213 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/cli.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/config.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    24428 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/core.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9326 2023-05-26 16:24:59.000000 cmind-1.2.2/cmind/index.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/net.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.306357 cmind-1.2.2/cmind/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.296357 cmind-1.2.2/cmind/repo/automation/
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.306357 cmind-1.2.2/cmind/repo/automation/automation/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2023-05-30 19:25:20.000000 cmind-1.2.2/cmind/repo/automation/automation/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/automation/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/automation/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/automation/module_dummy.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/automation/module_misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/automation/template_list_of_automations.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.306357 cmind-1.2.2/cmind/repo/automation/ck/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2023-05-30 19:25:20.000000 cmind-1.2.2/cmind/repo/automation/ck/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/ck/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/ck/module.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.316357 cmind-1.2.2/cmind/repo/automation/core/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2023-05-30 19:25:20.000000 cmind-1.2.2/cmind/repo/automation/core/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/core/_cm.json
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.316357 cmind-1.2.2/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/core/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/core/module_misc.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.316357 cmind-1.2.2/cmind/repo/automation/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9508 2023-05-30 19:25:20.000000 cmind-1.2.2/cmind/repo/automation/repo/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/repo/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    31060 2023-05-30 19:25:20.000000 cmind-1.2.2/cmind/repo/automation/repo/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/cmr.yaml
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    18709 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repos.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    41400 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/utils.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.306357 cmind-1.2.2/cmind.egg-info/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6057 2023-05-30 19:25:32.000000 cmind-1.2.2/cmind.egg-info/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1222 2023-05-30 19:25:32.000000 cmind-1.2.2/cmind.egg-info/SOURCES.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-30 19:25:32.000000 cmind-1.2.2/cmind.egg-info/dependency_links.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       60 2023-05-30 19:25:32.000000 cmind-1.2.2/cmind.egg-info/entry_points.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-25 12:15:08.000000 cmind-1.2.2/cmind.egg-info/not-zip-safe
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-05-30 19:25:32.000000 cmind-1.2.2/cmind.egg-info/requires.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-05-30 19:25:32.000000 cmind-1.2.2/cmind.egg-info/top_level.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-05-30 19:25:32.316357 cmind-1.2.2/setup.cfg
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2668 2023-05-25 12:13:31.000000 cmind-1.2.2/setup.py
```

### Comparing `cmind-1.2.1/PKG-INFO` & `cmind-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 1.2.1
+Version: 1.2.2
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck/tree/master/cm
 Author: Grigori Fursin
 Author-email: grigori@octoml.ai
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
         [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
@@ -32,15 +32,15 @@
         Is helps to solve the "dependency hell" for ML and AI systems while automatically generating 
         unified README files and synthesize unified containers with a common API.
         It is also used to automate [reproducibility initiatives and artifact evaluation at AI, ML and Systems conferences](https://cTuning.org/ae)
         while reducing all the tedious, manual, repetitive, and ad-hoc efforts to reproduce research projects and validate them in production.
         
         CM powers the [Collective Knowledge platform (MLCommons CK playground)](https://access.cKnowledge.org)
         to aggregate [reproducible experiments](https://access.cknowledge.org/playground/?action=experiments),
-        connect academia and industry to [organize reproducibility and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
+        connect academia and industry to [organize reproducibility, replicability and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
         and help developers and users select Pareto-optimal end-to-end applications and systems based on their requirements and constraints
         (cost, performance, power consumption, accuracy, etc).
         
         See a few real-world examples of using the CM scripting language:
         - [README to reproduce published IPOL'22 paper](cm-mlops/script/app-ipol-reproducibility-2022-439)
         - [README to reproduce MLPerf RetinaNet inference benchmark at Student Cluster Competition'22](docs/tutorials/sc22-scc-mlperf.md)
         - [Auto-generated READMEs to reproduce official MLPerf BERT inference benchmark v3.0 submission with a model from the Hugging Face Zoo](https://github.com/mlcommons/submissions_inference_3.0/tree/main/open/cTuning/code/huggingface-bert/README.md)
```

### Comparing `cmind-1.2.1/README.md` & `cmind-1.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 Is helps to solve the "dependency hell" for ML and AI systems while automatically generating 
 unified README files and synthesize unified containers with a common API.
 It is also used to automate [reproducibility initiatives and artifact evaluation at AI, ML and Systems conferences](https://cTuning.org/ae)
 while reducing all the tedious, manual, repetitive, and ad-hoc efforts to reproduce research projects and validate them in production.
 
 CM powers the [Collective Knowledge platform (MLCommons CK playground)](https://access.cKnowledge.org)
 to aggregate [reproducible experiments](https://access.cknowledge.org/playground/?action=experiments),
-connect academia and industry to [organize reproducibility and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
+connect academia and industry to [organize reproducibility, replicability and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
 and help developers and users select Pareto-optimal end-to-end applications and systems based on their requirements and constraints
 (cost, performance, power consumption, accuracy, etc).
 
 See a few real-world examples of using the CM scripting language:
 - [README to reproduce published IPOL'22 paper](cm-mlops/script/app-ipol-reproducibility-2022-439)
 - [README to reproduce MLPerf RetinaNet inference benchmark at Student Cluster Competition'22](docs/tutorials/sc22-scc-mlperf.md)
 - [Auto-generated READMEs to reproduce official MLPerf BERT inference benchmark v3.0 submission with a model from the Hugging Face Zoo](https://github.com/mlcommons/submissions_inference_3.0/tree/main/open/cTuning/code/huggingface-bert/README.md)
```

### Comparing `cmind-1.2.1/cmind/artifact.py` & `cmind-1.2.2/cmind/artifact.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/automation.py` & `cmind-1.2.2/cmind/automation.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/cli.py` & `cmind-1.2.2/cmind/cli.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/config.py` & `cmind-1.2.2/cmind/config.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/core.py` & `cmind-1.2.2/cmind/core.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/index.py` & `cmind-1.2.2/cmind/index.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/net.py` & `cmind-1.2.2/cmind/net.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/repo/automation/automation/README.md` & `cmind-1.2.2/cmind/repo/automation/automation/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,67 @@
 *This README is automatically generated - don't edit! Use `README-extra.md` for extra notes!*
 
 ### Automation actions
 
+#### print_input
+
+  * CM CLI: ```cm print_input automation``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L15))
+  * CM CLI with UID: ```cm print_input automation,bbeb15d8f0a944a4``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L15))
+  * CM Python API:
+    ```python
+    import cmind
+
+    r=cm.access({
+                 'action':'print_input'
+                 'automation':'automation,bbeb15d8f0a944a4'
+                 'out':'con'
+    ```
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L15)
+    ```python
+                })
+    if r['return']>0:
+        print(r['error'])
+    ```
+
 #### add
 
-  * CM CLI: ```cm add automation``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L15))
-  * CM CLI with UID: ```cm add automation,bbeb15d8f0a944a4``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L15))
+  * CM CLI: ```cm add automation``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L39))
+  * CM CLI with UID: ```cm add automation,bbeb15d8f0a944a4``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L39))
   * CM Python API:
     ```python
     import cmind
 
     r=cm.access({
                  'action':'add'
                  'automation':'automation,bbeb15d8f0a944a4'
                  'out':'con'
     ```
-    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L15)
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L39)
     ```python
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 #### doc
 
-  * CM CLI: ```cm doc automation``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L87))
-  * CM CLI with UID: ```cm doc automation,bbeb15d8f0a944a4``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L87))
+  * CM CLI: ```cm doc automation``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L111))
+  * CM CLI with UID: ```cm doc automation,bbeb15d8f0a944a4``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L111))
   * CM Python API:
     ```python
     import cmind
 
     r=cm.access({
                  'action':'doc'
                  'automation':'automation,bbeb15d8f0a944a4'
                  'out':'con'
     ```
-    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L87)
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/automation/module.py#L111)
     ```python
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 ### Maintainers
 
-* [Open MLCommons taskforce on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/mlperf-education-workgroup.md)
+* [Open MLCommons taskforce on automation and reproducibility](https://cKnowledge.org/mlcommons-taskforce)
```

### Comparing `cmind-1.2.1/cmind/repo/automation/automation/module.py` & `cmind-1.2.2/cmind/repo/automation/automation/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/repo/automation/automation/module_dummy.py` & `cmind-1.2.2/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/repo/automation/automation/module_misc.py` & `cmind-1.2.2/cmind/repo/automation/automation/module_misc.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/repo/automation/ck/README.md` & `cmind-1.2.2/cmind/repo/automation/ck/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,8 +20,8 @@
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 ### Maintainers
 
-* [Open MLCommons taskforce on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/mlperf-education-workgroup.md)
+* [Open MLCommons taskforce on automation and reproducibility](https://cKnowledge.org/mlcommons-taskforce)
```

### Comparing `cmind-1.2.1/cmind/repo/automation/ck/module.py` & `cmind-1.2.2/cmind/repo/automation/ck/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/repo/automation/core/README.md` & `cmind-1.2.2/cmind/repo/automation/core/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,8 +20,8 @@
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 ### Maintainers
 
-* [Open MLCommons taskforce on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/mlperf-education-workgroup.md)
+* [Open MLCommons taskforce on automation and reproducibility](https://cKnowledge.org/mlcommons-taskforce)
```

### Comparing `cmind-1.2.1/cmind/repo/automation/core/module.py` & `cmind-1.2.2/cmind/repo/automation/core/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/repo/automation/repo/README.md` & `cmind-1.2.2/cmind/repo/automation/repo/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,208 +20,228 @@
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 #### search
 
-  * CM CLI: ```cm search repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L93))
-  * CM CLI with UID: ```cm search repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L93))
+  * CM CLI: ```cm search repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L98))
+  * CM CLI with UID: ```cm search repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L98))
   * CM Python API:
     ```python
     import cmind
 
     r=cm.access({
                  'action':'search'
                  'automation':'repo,55c3e27e8a140e48'
                  'out':'con'
     ```
-    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L93)
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L98)
     ```python
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 #### update
 
-  * CM CLI: ```cm update repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L172))
-  * CM CLI with UID: ```cm update repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L172))
+  * CM CLI: ```cm update repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L177))
+  * CM CLI with UID: ```cm update repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L177))
   * CM Python API:
     ```python
     import cmind
 
     r=cm.access({
                  'action':'update'
                  'automation':'repo,55c3e27e8a140e48'
                  'out':'con'
     ```
-    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L172)
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L177)
     ```python
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 #### delete
 
-  * CM CLI: ```cm delete repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L209))
-  * CM CLI with UID: ```cm delete repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L209))
+  * CM CLI: ```cm delete repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L214))
+  * CM CLI with UID: ```cm delete repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L214))
   * CM Python API:
     ```python
     import cmind
 
     r=cm.access({
                  'action':'delete'
                  'automation':'repo,55c3e27e8a140e48'
                  'out':'con'
     ```
-    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L209)
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L214)
     ```python
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 #### init
 
-  * CM CLI: ```cm init repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L262))
-  * CM CLI with UID: ```cm init repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L262))
+  * CM CLI: ```cm init repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L271))
+  * CM CLI with UID: ```cm init repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L271))
   * CM Python API:
     ```python
     import cmind
 
     r=cm.access({
                  'action':'init'
                  'automation':'repo,55c3e27e8a140e48'
                  'out':'con'
     ```
-    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L262)
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L271)
     ```python
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 #### add
 
-  * CM CLI: ```cm add repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L381))
-  * CM CLI with UID: ```cm add repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L381))
+  * CM CLI: ```cm add repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L395))
+  * CM CLI with UID: ```cm add repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L395))
   * CM Python API:
     ```python
     import cmind
 
     r=cm.access({
                  'action':'add'
                  'automation':'repo,55c3e27e8a140e48'
                  'out':'con'
     ```
-    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L381)
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L395)
     ```python
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 #### pack
 
-  * CM CLI: ```cm pack repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L389))
-  * CM CLI with UID: ```cm pack repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L389))
+  * CM CLI: ```cm pack repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L403))
+  * CM CLI with UID: ```cm pack repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L403))
   * CM Python API:
     ```python
     import cmind
 
     r=cm.access({
                  'action':'pack'
                  'automation':'repo,55c3e27e8a140e48'
                  'out':'con'
     ```
-    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L389)
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L403)
     ```python
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 #### unpack
 
-  * CM CLI: ```cm unpack repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L459))
-  * CM CLI with UID: ```cm unpack repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L459))
+  * CM CLI: ```cm unpack repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L473))
+  * CM CLI with UID: ```cm unpack repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L473))
   * CM Python API:
     ```python
     import cmind
 
     r=cm.access({
                  'action':'unpack'
                  'automation':'repo,55c3e27e8a140e48'
                  'out':'con'
     ```
-    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L459)
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L473)
     ```python
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 #### import_ck_to_cm
 
-  * CM CLI: ```cm import_ck_to_cm repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L562))
-  * CM CLI with UID: ```cm import_ck_to_cm repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L562))
+  * CM CLI: ```cm import_ck_to_cm repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L580))
+  * CM CLI with UID: ```cm import_ck_to_cm repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L580))
   * CM Python API:
     ```python
     import cmind
 
     r=cm.access({
                  'action':'import_ck_to_cm'
                  'automation':'repo,55c3e27e8a140e48'
                  'out':'con'
     ```
-    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L562)
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L580)
     ```python
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 #### convert_ck_to_cm
 
-  * CM CLI: ```cm convert_ck_to_cm repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L613))
-  * CM CLI with UID: ```cm convert_ck_to_cm repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L613))
+  * CM CLI: ```cm convert_ck_to_cm repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L631))
+  * CM CLI with UID: ```cm convert_ck_to_cm repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L631))
   * CM Python API:
     ```python
     import cmind
 
     r=cm.access({
                  'action':'convert_ck_to_cm'
                  'automation':'repo,55c3e27e8a140e48'
                  'out':'con'
     ```
-    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L613)
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L631)
     ```python
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 #### detect
 
-  * CM CLI: ```cm detect repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L667))
-  * CM CLI with UID: ```cm detect repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L667))
+  * CM CLI: ```cm detect repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L685))
+  * CM CLI with UID: ```cm detect repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L685))
   * CM Python API:
     ```python
     import cmind
 
     r=cm.access({
                  'action':'detect'
                  'automation':'repo,55c3e27e8a140e48'
                  'out':'con'
     ```
-    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L667)
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L685)
+    ```python
+                })
+    if r['return']>0:
+        print(r['error'])
+    ```
+
+#### reindex
+
+  * CM CLI: ```cm reindex repo``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L872))
+  * CM CLI with UID: ```cm reindex repo,55c3e27e8a140e48``` ([add flags (dict keys) from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L872))
+  * CM Python API:
+    ```python
+    import cmind
+
+    r=cm.access({
+                 'action':'reindex'
+                 'automation':'repo,55c3e27e8a140e48'
+                 'out':'con'
+    ```
+    [add keys from this API](https://github.com/mlcommons/ck/tree/master/cm/cmind/repo/automation/repo/module.py#L872)
     ```python
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 ### Maintainers
 
-* [Open MLCommons taskforce on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/mlperf-education-workgroup.md)
+* [Open MLCommons taskforce on automation and reproducibility](https://cKnowledge.org/mlcommons-taskforce)
```

### Comparing `cmind-1.2.1/cmind/repo/automation/repo/module.py` & `cmind-1.2.2/cmind/repo/automation/repo/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -858,18 +858,14 @@
                     print ('')
                     print ('Current directory has a CM artifact:')
 
                     print ('')
                     print ('  Artifact alias: {}'.format(artifact_meta['alias']))
                     print ('  Artifact UID:   {}'.format(artifact_meta['uid']))
 
-        if self.cmind.use_index:
-            ii = {'out':'con'} if console else {}
-            rx = self.reindex(ii)
-
         return rr
 
 
     ############################################################
     def reindex(self, i):
         """
         Reindex all CM repositories
```

### Comparing `cmind-1.2.1/cmind/repo.py` & `cmind-1.2.2/cmind/repo.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/repos.py` & `cmind-1.2.2/cmind/repos.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind/utils.py` & `cmind-1.2.2/cmind/utils.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/cmind.egg-info/PKG-INFO` & `cmind-1.2.2/cmind.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 1.2.1
+Version: 1.2.2
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck/tree/master/cm
 Author: Grigori Fursin
 Author-email: grigori@octoml.ai
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
         [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
@@ -32,15 +32,15 @@
         Is helps to solve the "dependency hell" for ML and AI systems while automatically generating 
         unified README files and synthesize unified containers with a common API.
         It is also used to automate [reproducibility initiatives and artifact evaluation at AI, ML and Systems conferences](https://cTuning.org/ae)
         while reducing all the tedious, manual, repetitive, and ad-hoc efforts to reproduce research projects and validate them in production.
         
         CM powers the [Collective Knowledge platform (MLCommons CK playground)](https://access.cKnowledge.org)
         to aggregate [reproducible experiments](https://access.cknowledge.org/playground/?action=experiments),
-        connect academia and industry to [organize reproducibility and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
+        connect academia and industry to [organize reproducibility, replicability and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
         and help developers and users select Pareto-optimal end-to-end applications and systems based on their requirements and constraints
         (cost, performance, power consumption, accuracy, etc).
         
         See a few real-world examples of using the CM scripting language:
         - [README to reproduce published IPOL'22 paper](cm-mlops/script/app-ipol-reproducibility-2022-439)
         - [README to reproduce MLPerf RetinaNet inference benchmark at Student Cluster Competition'22](docs/tutorials/sc22-scc-mlperf.md)
         - [Auto-generated READMEs to reproduce official MLPerf BERT inference benchmark v3.0 submission with a model from the Hugging Face Zoo](https://github.com/mlcommons/submissions_inference_3.0/tree/main/open/cTuning/code/huggingface-bert/README.md)
```

### Comparing `cmind-1.2.1/cmind.egg-info/SOURCES.txt` & `cmind-1.2.2/cmind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmind-1.2.1/setup.py` & `cmind-1.2.2/setup.py`

 * *Files identical despite different names*

