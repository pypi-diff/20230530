# Comparing `tmp/PyParallelPipe-0.0.1.tar.gz` & `tmp/PyParallelPipe-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyParallelPipe-0.0.1.tar", last modified: Tue May 30 05:01:03 2023, max compression
+gzip compressed data, was "PyParallelPipe-1.0.0.tar", last modified: Tue May 30 05:13:29 2023, max compression
```

## Comparing `PyParallelPipe-0.0.1.tar` & `PyParallelPipe-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:01:03.923429 PyParallelPipe-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 05:00:47.000000 PyParallelPipe-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14672 2023-05-30 05:01:03.923429 PyParallelPipe-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:01:03.919429 PyParallelPipe-0.0.1/ParallelPipe/
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-30 05:00:47.000000 PyParallelPipe-0.0.1/ParallelPipe/Buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-30 05:00:47.000000 PyParallelPipe-0.0.1/ParallelPipe/Pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-30 05:00:47.000000 PyParallelPipe-0.0.1/ParallelPipe/Stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-30 05:00:47.000000 PyParallelPipe-0.0.1/ParallelPipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:01:03.923429 PyParallelPipe-0.0.1/PyParallelPipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14672 2023-05-30 05:01:03.000000 PyParallelPipe-0.0.1/PyParallelPipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-30 05:01:03.000000 PyParallelPipe-0.0.1/PyParallelPipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 05:01:03.000000 PyParallelPipe-0.0.1/PyParallelPipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 05:01:03.000000 PyParallelPipe-0.0.1/PyParallelPipe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14044 2023-05-30 05:00:47.000000 PyParallelPipe-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 05:00:47.000000 PyParallelPipe-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-30 05:01:03.923429 PyParallelPipe-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:13:29.436624 PyParallelPipe-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-05-30 05:13:29.436624 PyParallelPipe-1.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:13:29.432624 PyParallelPipe-1.0.0/ParallelPipe/
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/ParallelPipe/Buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/ParallelPipe/Pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/ParallelPipe/Stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/ParallelPipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:13:29.436624 PyParallelPipe-1.0.0/PyParallelPipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-05-30 05:13:29.000000 PyParallelPipe-1.0.0/PyParallelPipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-30 05:13:29.000000 PyParallelPipe-1.0.0/PyParallelPipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 05:13:29.000000 PyParallelPipe-1.0.0/PyParallelPipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 05:13:29.000000 PyParallelPipe-1.0.0/PyParallelPipe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 05:13:08.000000 PyParallelPipe-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-30 05:13:29.436624 PyParallelPipe-1.0.0/setup.cfg
```

### Comparing `PyParallelPipe-0.0.1/LICENSE` & `PyParallelPipe-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyParallelPipe-0.0.1/PKG-INFO` & `PyParallelPipe-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyParallelPipe
-Version: 0.0.1
+Version: 1.0.0
 Summary: Using this ParallelPipe library, it is very fast and easy to build parallel acceleration for multi-stage tasks, including deep learning. This code library does not require any dependencies and consists of pure Python code.
 Home-page: https://github.com/gongpx20069/ParallelPipe
 Author: PayShown
 Author-email: pxgong19@fudan.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,20 +15,27 @@
 <h2 align="center">Python Parallel Pipeline Architecture (ParallelPipe)</h2>
 <p align="center">
 Language: <a href="https://github.com/gongpx20069/ParallelPipe#readme" target="_blank" rel="noopener noreferrer">English</a>
   | <a href="https://github.com/gongpx20069/ParallelPipe#readme" target="_blank" rel="noopener noreferrer">中文</a>
 </p>
 
 -------------------------
+
+## Write in advance
+
+You can install this package using the following command:
+
+```pip install PyParallelPipe```
+
 ### 1. Overview
 In deep learning, many tasks in practical business scenarios are multi-stage and decomposable. Taking behavior recognition as an example, when performing behavior recognition using RGB video streams, we can divide the overall workflow into four steps: data collection, object recognition, object tracking, and behavior classification, as shown in Figure 1. If these four steps are executed sequentially, it would consume a significant amount of time. However, if these four steps can run simultaneously, it often enables real-time processing in practical applications, overcoming the time-consuming nature of sequential execution.
 
 The design principles of the framework are: **decoupling, reusability, readability, and high performance**.
 
-![pipeline_zh](docs/pipeline_zh.png)
+[![pipeline_zh](docs/pipeline_zh.png)](https://github.com/gongpx20069/ParallelPipe/blob/main/docs/pipeline_zh.png)
 
 #### 1.1 Environment Requirements
 This framework can run in a Python 3.5+ environment without requiring any additional Python dependencies.
 
 #### 1.2 Python Dependencies
 To avoid the Global Interpreter Lock (GIL) in Python for multithreading, we plan to use the following built-in Python libraries:
 
@@ -194,21 +201,27 @@
 P.put("Something Stage one can process.")
 ```
 
 You can add inputs to the pipeline using the `put` function as needed. The pipeline will automatically distribute the inputs to the appropriate stages for processing.
 
 --------------------------------
 
+## 简单安装
+
+你可以使用如下命令安装本Python包：
+
+```pip install PyParallelPipe```
+
 ### 1. 概述
 
 在深度学习中，很多实际业务场景中的任务是多阶段的，可拆解的任务。如图1，以行为识别为例，在使用RGB视频流进行行为识别时，我们可以将整体工作流分为四个步骤（数据采集、目标识别、目标追踪、行为分类）。如果四个步骤串行运行，则会占用大量的时间。如果四个步骤可以同时运行，往往可以使串行占用大量时间的方法在实际业务中实时进行。
 
 框架设计宗旨为：**解耦，可复用，易理解，高性能。**
 
-![pipeline_zh](docs/pipeline_zh.png)
+[![pipeline_zh](docs/pipeline_zh.png)](https://github.com/gongpx20069/ParallelPipe/blob/main/docs/pipeline_zh.png)
 
 #### 1.1 使用环境
 
 本框架可以在python3.5+的环境中运行，无需额外的Python依赖包。
 
 #### 1.2 Python依赖
```

### Comparing `PyParallelPipe-0.0.1/ParallelPipe/Buffer.py` & `PyParallelPipe-1.0.0/ParallelPipe/Buffer.py`

 * *Files identical despite different names*

### Comparing `PyParallelPipe-0.0.1/ParallelPipe/Pipeline.py` & `PyParallelPipe-1.0.0/ParallelPipe/Pipeline.py`

 * *Files identical despite different names*

### Comparing `PyParallelPipe-0.0.1/ParallelPipe/Stage.py` & `PyParallelPipe-1.0.0/ParallelPipe/Stage.py`

 * *Files identical despite different names*

### Comparing `PyParallelPipe-0.0.1/PyParallelPipe.egg-info/PKG-INFO` & `PyParallelPipe-1.0.0/PyParallelPipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyParallelPipe
-Version: 0.0.1
+Version: 1.0.0
 Summary: Using this ParallelPipe library, it is very fast and easy to build parallel acceleration for multi-stage tasks, including deep learning. This code library does not require any dependencies and consists of pure Python code.
 Home-page: https://github.com/gongpx20069/ParallelPipe
 Author: PayShown
 Author-email: pxgong19@fudan.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,20 +15,27 @@
 <h2 align="center">Python Parallel Pipeline Architecture (ParallelPipe)</h2>
 <p align="center">
 Language: <a href="https://github.com/gongpx20069/ParallelPipe#readme" target="_blank" rel="noopener noreferrer">English</a>
   | <a href="https://github.com/gongpx20069/ParallelPipe#readme" target="_blank" rel="noopener noreferrer">中文</a>
 </p>
 
 -------------------------
+
+## Write in advance
+
+You can install this package using the following command:
+
+```pip install PyParallelPipe```
+
 ### 1. Overview
 In deep learning, many tasks in practical business scenarios are multi-stage and decomposable. Taking behavior recognition as an example, when performing behavior recognition using RGB video streams, we can divide the overall workflow into four steps: data collection, object recognition, object tracking, and behavior classification, as shown in Figure 1. If these four steps are executed sequentially, it would consume a significant amount of time. However, if these four steps can run simultaneously, it often enables real-time processing in practical applications, overcoming the time-consuming nature of sequential execution.
 
 The design principles of the framework are: **decoupling, reusability, readability, and high performance**.
 
-![pipeline_zh](docs/pipeline_zh.png)
+[![pipeline_zh](docs/pipeline_zh.png)](https://github.com/gongpx20069/ParallelPipe/blob/main/docs/pipeline_zh.png)
 
 #### 1.1 Environment Requirements
 This framework can run in a Python 3.5+ environment without requiring any additional Python dependencies.
 
 #### 1.2 Python Dependencies
 To avoid the Global Interpreter Lock (GIL) in Python for multithreading, we plan to use the following built-in Python libraries:
 
@@ -194,21 +201,27 @@
 P.put("Something Stage one can process.")
 ```
 
 You can add inputs to the pipeline using the `put` function as needed. The pipeline will automatically distribute the inputs to the appropriate stages for processing.
 
 --------------------------------
 
+## 简单安装
+
+你可以使用如下命令安装本Python包：
+
+```pip install PyParallelPipe```
+
 ### 1. 概述
 
 在深度学习中，很多实际业务场景中的任务是多阶段的，可拆解的任务。如图1，以行为识别为例，在使用RGB视频流进行行为识别时，我们可以将整体工作流分为四个步骤（数据采集、目标识别、目标追踪、行为分类）。如果四个步骤串行运行，则会占用大量的时间。如果四个步骤可以同时运行，往往可以使串行占用大量时间的方法在实际业务中实时进行。
 
 框架设计宗旨为：**解耦，可复用，易理解，高性能。**
 
-![pipeline_zh](docs/pipeline_zh.png)
+[![pipeline_zh](docs/pipeline_zh.png)](https://github.com/gongpx20069/ParallelPipe/blob/main/docs/pipeline_zh.png)
 
 #### 1.1 使用环境
 
 本框架可以在python3.5+的环境中运行，无需额外的Python依赖包。
 
 #### 1.2 Python依赖
```

### Comparing `PyParallelPipe-0.0.1/README.md` & `PyParallelPipe-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 <h2 align="center">Python Parallel Pipeline Architecture (ParallelPipe)</h2>
 <p align="center">
 Language: <a href="https://github.com/gongpx20069/ParallelPipe#readme" target="_blank" rel="noopener noreferrer">English</a>
   | <a href="https://github.com/gongpx20069/ParallelPipe#readme" target="_blank" rel="noopener noreferrer">中文</a>
 </p>
 
 -------------------------
+
+## Write in advance
+
+You can install this package using the following command:
+
+```pip install PyParallelPipe```
+
 ### 1. Overview
 In deep learning, many tasks in practical business scenarios are multi-stage and decomposable. Taking behavior recognition as an example, when performing behavior recognition using RGB video streams, we can divide the overall workflow into four steps: data collection, object recognition, object tracking, and behavior classification, as shown in Figure 1. If these four steps are executed sequentially, it would consume a significant amount of time. However, if these four steps can run simultaneously, it often enables real-time processing in practical applications, overcoming the time-consuming nature of sequential execution.
 
 The design principles of the framework are: **decoupling, reusability, readability, and high performance**.
 
-![pipeline_zh](docs/pipeline_zh.png)
+[![pipeline_zh](docs/pipeline_zh.png)](https://github.com/gongpx20069/ParallelPipe/blob/main/docs/pipeline_zh.png)
 
 #### 1.1 Environment Requirements
 This framework can run in a Python 3.5+ environment without requiring any additional Python dependencies.
 
 #### 1.2 Python Dependencies
 To avoid the Global Interpreter Lock (GIL) in Python for multithreading, we plan to use the following built-in Python libraries:
 
@@ -180,21 +187,27 @@
 P.put("Something Stage one can process.")
 ```
 
 You can add inputs to the pipeline using the `put` function as needed. The pipeline will automatically distribute the inputs to the appropriate stages for processing.
 
 --------------------------------
 
+## 简单安装
+
+你可以使用如下命令安装本Python包：
+
+```pip install PyParallelPipe```
+
 ### 1. 概述
 
 在深度学习中，很多实际业务场景中的任务是多阶段的，可拆解的任务。如图1，以行为识别为例，在使用RGB视频流进行行为识别时，我们可以将整体工作流分为四个步骤（数据采集、目标识别、目标追踪、行为分类）。如果四个步骤串行运行，则会占用大量的时间。如果四个步骤可以同时运行，往往可以使串行占用大量时间的方法在实际业务中实时进行。
 
 框架设计宗旨为：**解耦，可复用，易理解，高性能。**
 
-![pipeline_zh](docs/pipeline_zh.png)
+[![pipeline_zh](docs/pipeline_zh.png)](https://github.com/gongpx20069/ParallelPipe/blob/main/docs/pipeline_zh.png)
 
 #### 1.1 使用环境
 
 本框架可以在python3.5+的环境中运行，无需额外的Python依赖包。
 
 #### 1.2 Python依赖
```

### Comparing `PyParallelPipe-0.0.1/setup.cfg` & `PyParallelPipe-1.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PyParallelPipe
-version = 0.0.1
+version = 1.0.0
 author = PayShown
 author_email = pxgong19@fudan.edu.cn
 description = Using this ParallelPipe library, it is very fast and easy to build parallel acceleration for multi-stage tasks, including deep learning. This code library does not require any dependencies and consists of pure Python code.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/gongpx20069/ParallelPipe
 classifiers =
```

