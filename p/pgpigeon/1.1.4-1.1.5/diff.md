# Comparing `tmp/pgpigeon-1.1.4.tar.gz` & `tmp/pgpigeon-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\CBRE\Code Community Contributions\packages\python\pypigeon\dist\tmprwc51z8k\pgpigeon-1.1.4.tar", last modified: Thu Aug 18 10:08:50 2022, max compression
+gzip compressed data, was "pgpigeon-1.1.5.tar", last modified: Tue May 30 12:15:28 2023, max compression
```

## Comparing `pgpigeon-1.1.4.tar` & `pgpigeon-1.1.5.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-08-18 10:08:50.777965 pgpigeon-1.1.4/
--rw-rw-rw-   0        0        0     1093 2022-08-16 08:03:08.000000 pgpigeon-1.1.4/LICENSE
--rw-rw-rw-   0        0        0    15317 2022-08-18 10:08:50.775963 pgpigeon-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    13416 2022-08-16 20:32:52.000000 pgpigeon-1.1.4/README.md
--rw-rw-rw-   0        0        0     1043 2022-08-16 19:41:48.000000 pgpigeon-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-18 10:08:50.778966 pgpigeon-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-08-16 19:41:48.000000 pgpigeon-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-18 10:08:50.555905 pgpigeon-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2022-08-18 10:08:50.696965 pgpigeon-1.1.4/src/pgpigeon/
--rw-rw-rw-   0        0        0       21 2022-08-18 10:05:31.000000 pgpigeon-1.1.4/src/pgpigeon/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-18 10:08:50.768963 pgpigeon-1.1.4/src/pgpigeon/commands/
--rw-rw-rw-   0        0        0        0 2022-08-16 08:03:08.000000 pgpigeon-1.1.4/src/pgpigeon/commands/__init__.py
--rw-rw-rw-   0        0        0     1314 2022-08-16 08:03:08.000000 pgpigeon-1.1.4/src/pgpigeon/commands/configure.py
--rw-rw-rw-   0        0        0     1069 2022-08-16 08:03:08.000000 pgpigeon-1.1.4/src/pgpigeon/commands/create_scripts.py
--rw-rw-rw-   0        0        0     1071 2022-08-16 08:03:08.000000 pgpigeon-1.1.4/src/pgpigeon/commands/create_triggers.py
--rw-rw-rw-   0        0        0     1911 2022-08-16 08:03:08.000000 pgpigeon-1.1.4/src/pgpigeon/commands/sample_code.py
--rw-rw-rw-   0        0        0     3187 2022-08-16 21:25:33.000000 pgpigeon-1.1.4/src/pgpigeon/common.py
--rw-rw-rw-   0        0        0     8931 2022-08-16 19:41:48.000000 pgpigeon-1.1.4/src/pgpigeon/constants.py
--rw-rw-rw-   0        0        0      911 2022-08-16 19:41:48.000000 pgpigeon-1.1.4/src/pgpigeon/context_models.py
--rw-rw-rw-   0        0        0      584 2022-08-16 08:03:08.000000 pgpigeon-1.1.4/src/pgpigeon/interpreter.py
--rw-rw-rw-   0        0        0      239 2022-08-16 08:03:08.000000 pgpigeon-1.1.4/src/pgpigeon/modules.py
--rw-rw-rw-   0        0        0     3668 2022-08-18 10:05:16.000000 pgpigeon-1.1.4/src/pgpigeon/pgnest.py
--rw-rw-rw-   0        0        0     2550 2022-08-16 20:26:27.000000 pgpigeon-1.1.4/src/pgpigeon/pgpigeon.py
--rw-rw-rw-   0        0        0     2023 2022-08-16 20:22:11.000000 pgpigeon-1.1.4/src/pgpigeon/pgscript.py
--rw-rw-rw-   0        0        0      892 2022-08-16 08:03:08.000000 pgpigeon-1.1.4/src/pgpigeon/pigeon_cli.py
-drwxrwxrwx   0        0        0        0 2022-08-18 10:08:50.733964 pgpigeon-1.1.4/src/pgpigeon.egg-info/
--rw-rw-rw-   0        0        0    15317 2022-08-18 10:08:50.000000 pgpigeon-1.1.4/src/pgpigeon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2022-08-18 10:08:50.000000 pgpigeon-1.1.4/src/pgpigeon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-18 10:08:50.000000 pgpigeon-1.1.4/src/pgpigeon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2022-08-18 10:08:50.000000 pgpigeon-1.1.4/src/pgpigeon.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2022-08-18 10:08:50.000000 pgpigeon-1.1.4/src/pgpigeon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-18 10:08:50.000000 pgpigeon-1.1.4/src/pgpigeon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 12:15:28.348079 pgpigeon-1.1.5/
+-rw-rw-rw-   0        0        0     1093 2022-08-08 18:42:03.000000 pgpigeon-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0    15395 2023-05-30 12:15:28.346977 pgpigeon-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    13494 2023-05-30 12:05:32.000000 pgpigeon-1.1.5/README.md
+-rw-rw-rw-   0        0        0     1043 2023-05-30 12:03:07.000000 pgpigeon-1.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 12:15:28.349156 pgpigeon-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-08-16 18:16:30.000000 pgpigeon-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:15:28.273011 pgpigeon-1.1.5/src/
+-rw-rw-rw-   0        0        0        0 2022-08-14 11:26:26.000000 pgpigeon-1.1.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:15:28.292091 pgpigeon-1.1.5/src/pgpigeon/
+-rw-rw-rw-   0        0        0       21 2023-05-30 12:13:25.000000 pgpigeon-1.1.5/src/pgpigeon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:15:28.344824 pgpigeon-1.1.5/src/pgpigeon/commands/
+-rw-rw-rw-   0        0        0        0 2022-08-14 11:26:26.000000 pgpigeon-1.1.5/src/pgpigeon/commands/__init__.py
+-rw-rw-rw-   0        0        0     1314 2022-08-15 20:55:12.000000 pgpigeon-1.1.5/src/pgpigeon/commands/configure.py
+-rw-rw-rw-   0        0        0     1069 2022-08-15 20:55:39.000000 pgpigeon-1.1.5/src/pgpigeon/commands/create_scripts.py
+-rw-rw-rw-   0        0        0     1071 2022-08-15 20:56:03.000000 pgpigeon-1.1.5/src/pgpigeon/commands/create_triggers.py
+-rw-rw-rw-   0        0        0     1911 2022-08-15 20:56:33.000000 pgpigeon-1.1.5/src/pgpigeon/commands/sample_code.py
+-rw-rw-rw-   0        0        0     3187 2023-05-30 12:03:32.000000 pgpigeon-1.1.5/src/pgpigeon/common.py
+-rw-rw-rw-   0        0        0     8931 2022-08-16 19:18:14.000000 pgpigeon-1.1.5/src/pgpigeon/constants.py
+-rw-rw-rw-   0        0        0      911 2022-08-16 18:42:27.000000 pgpigeon-1.1.5/src/pgpigeon/context_models.py
+-rw-rw-rw-   0        0        0      584 2022-08-14 11:26:26.000000 pgpigeon-1.1.5/src/pgpigeon/interpreter.py
+-rw-rw-rw-   0        0        0      239 2022-08-14 11:26:26.000000 pgpigeon-1.1.5/src/pgpigeon/modules.py
+-rw-rw-rw-   0        0        0     3668 2023-05-30 12:03:32.000000 pgpigeon-1.1.5/src/pgpigeon/pgnest.py
+-rw-rw-rw-   0        0        0     2550 2023-05-30 12:03:32.000000 pgpigeon-1.1.5/src/pgpigeon/pgpigeon.py
+-rw-rw-rw-   0        0        0     2023 2023-05-30 12:03:33.000000 pgpigeon-1.1.5/src/pgpigeon/pgscript.py
+-rw-rw-rw-   0        0        0      892 2022-08-15 20:57:39.000000 pgpigeon-1.1.5/src/pgpigeon/pigeon_cli.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:15:28.331807 pgpigeon-1.1.5/src/pgpigeon.egg-info/
+-rw-rw-rw-   0        0        0    15395 2023-05-30 12:15:28.000000 pgpigeon-1.1.5/src/pgpigeon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2023-05-30 12:15:28.000000 pgpigeon-1.1.5/src/pgpigeon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 12:15:28.000000 pgpigeon-1.1.5/src/pgpigeon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-30 12:15:28.000000 pgpigeon-1.1.5/src/pgpigeon.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-05-30 12:15:28.000000 pgpigeon-1.1.5/src/pgpigeon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 12:15:28.000000 pgpigeon-1.1.5/src/pgpigeon.egg-info/top_level.txt
```

### Comparing `pgpigeon-1.1.4/LICENSE` & `pgpigeon-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pgpigeon-1.1.4/PKG-INFO` & `pgpigeon-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgpigeon
-Version: 1.1.4
+Version: 1.1.5
 Summary: This package help to implement realtime db notifications.
 Author-email: Dinesh Kushwaha <2kush.dinesh@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Dinesh Kushwaha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,26 +39,27 @@
 
 <p align="center"> This package will help to capture realtime postgreSQL table notification in python scripts.
     <br> 
 </p>
 
 ## 📝 Table of Contents
 
-- [About](#about)
-- [Getting Started](#getting_started)
-- [Authors](#authors)
+- [📝 Table of Contents](#-table-of-contents)
+- [🧐 About ](#-about-)
+- [🏁 Getting Started ](#-getting-started-)
+- [✍️ Authors ](#️-authors-)
 
 ## 🧐 About <a name = "about"></a>
 
 This package can be used for capture PostgreSQL database table event at real time in python scripts.
 
 ## 🏁 Getting Started <a name = "getting_started"></a>
 - Dependancy & prerequisite 
     - Python >=3.6 should be installed.
-    - "psycopg2==2.9.3"
+    - "psycopg2>=2.9.3"
 
 - To Start experimenting this package you need to install it.
 
 - [Step - 1]
 ```
 
     pip install pgpigeon
```

### Comparing `pgpigeon-1.1.4/README.md` & `pgpigeon-1.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 <p align="center"> This package will help to capture realtime postgreSQL table notification in python scripts.
     <br> 
 </p>
 
 ## 📝 Table of Contents
 
-- [About](#about)
-- [Getting Started](#getting_started)
-- [Authors](#authors)
+- [📝 Table of Contents](#-table-of-contents)
+- [🧐 About ](#-about-)
+- [🏁 Getting Started ](#-getting-started-)
+- [✍️ Authors ](#️-authors-)
 
 ## 🧐 About <a name = "about"></a>
 
 This package can be used for capture PostgreSQL database table event at real time in python scripts.
 
 ## 🏁 Getting Started <a name = "getting_started"></a>
 - Dependancy & prerequisite 
     - Python >=3.6 should be installed.
-    - "psycopg2==2.9.3"
+    - "psycopg2>=2.9.3"
 
 - To Start experimenting this package you need to install it.
 
 - [Step - 1]
 ```
 
     pip install pgpigeon
```

### Comparing `pgpigeon-1.1.4/pyproject.toml` & `pgpigeon-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 keywords = ["python", "postgresql", "realtime", "notification","pg_notify","channel"]
 requires-python = ">=3.6"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
-dependencies = ["psycopg2==2.9.3"]
+dependencies = ["psycopg2>=2.9.3"]
 
 [tool.setuptools.dynamic]
 version = {attr = "pgpigeon.__version__"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `pgpigeon-1.1.4/src/pgpigeon/commands/configure.py` & `pgpigeon-1.1.5/src/pgpigeon/commands/configure.py`

 * *Files identical despite different names*

### Comparing `pgpigeon-1.1.4/src/pgpigeon/commands/create_scripts.py` & `pgpigeon-1.1.5/src/pgpigeon/commands/create_scripts.py`

 * *Files identical despite different names*

### Comparing `pgpigeon-1.1.4/src/pgpigeon/commands/create_triggers.py` & `pgpigeon-1.1.5/src/pgpigeon/commands/create_triggers.py`

 * *Files identical despite different names*

### Comparing `pgpigeon-1.1.4/src/pgpigeon/commands/sample_code.py` & `pgpigeon-1.1.5/src/pgpigeon/commands/sample_code.py`

 * *Files identical despite different names*

### Comparing `pgpigeon-1.1.4/src/pgpigeon/common.py` & `pgpigeon-1.1.5/src/pgpigeon/common.py`

 * *Files identical despite different names*

### Comparing `pgpigeon-1.1.4/src/pgpigeon/constants.py` & `pgpigeon-1.1.5/src/pgpigeon/constants.py`

 * *Files identical despite different names*

### Comparing `pgpigeon-1.1.4/src/pgpigeon/context_models.py` & `pgpigeon-1.1.5/src/pgpigeon/context_models.py`

 * *Files identical despite different names*

### Comparing `pgpigeon-1.1.4/src/pgpigeon/interpreter.py` & `pgpigeon-1.1.5/src/pgpigeon/interpreter.py`

 * *Files identical despite different names*

### Comparing `pgpigeon-1.1.4/src/pgpigeon/pgnest.py` & `pgpigeon-1.1.5/src/pgpigeon/pgnest.py`

 * *Files identical despite different names*

### Comparing `pgpigeon-1.1.4/src/pgpigeon/pgpigeon.py` & `pgpigeon-1.1.5/src/pgpigeon/pgpigeon.py`

 * *Files identical despite different names*

### Comparing `pgpigeon-1.1.4/src/pgpigeon/pgscript.py` & `pgpigeon-1.1.5/src/pgpigeon/pgscript.py`

 * *Files identical despite different names*

### Comparing `pgpigeon-1.1.4/src/pgpigeon/pigeon_cli.py` & `pgpigeon-1.1.5/src/pgpigeon/pigeon_cli.py`

 * *Files identical despite different names*

### Comparing `pgpigeon-1.1.4/src/pgpigeon.egg-info/PKG-INFO` & `pgpigeon-1.1.5/src/pgpigeon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgpigeon
-Version: 1.1.4
+Version: 1.1.5
 Summary: This package help to implement realtime db notifications.
 Author-email: Dinesh Kushwaha <2kush.dinesh@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Dinesh Kushwaha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,26 +39,27 @@
 
 <p align="center"> This package will help to capture realtime postgreSQL table notification in python scripts.
     <br> 
 </p>
 
 ## 📝 Table of Contents
 
-- [About](#about)
-- [Getting Started](#getting_started)
-- [Authors](#authors)
+- [📝 Table of Contents](#-table-of-contents)
+- [🧐 About ](#-about-)
+- [🏁 Getting Started ](#-getting-started-)
+- [✍️ Authors ](#️-authors-)
 
 ## 🧐 About <a name = "about"></a>
 
 This package can be used for capture PostgreSQL database table event at real time in python scripts.
 
 ## 🏁 Getting Started <a name = "getting_started"></a>
 - Dependancy & prerequisite 
     - Python >=3.6 should be installed.
-    - "psycopg2==2.9.3"
+    - "psycopg2>=2.9.3"
 
 - To Start experimenting this package you need to install it.
 
 - [Step - 1]
 ```
 
     pip install pgpigeon
```

### Comparing `pgpigeon-1.1.4/src/pgpigeon.egg-info/SOURCES.txt` & `pgpigeon-1.1.5/src/pgpigeon.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+src/__init__.py
 src/pgpigeon/__init__.py
 src/pgpigeon/common.py
 src/pgpigeon/constants.py
 src/pgpigeon/context_models.py
 src/pgpigeon/interpreter.py
 src/pgpigeon/modules.py
 src/pgpigeon/pgnest.py
```

