# Comparing `tmp/pymg-1.0.0.tar.gz` & `tmp/pymg-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymg-1.0.0.tar", last modified: Sun May  7 08:38:32 2023, max compression
+gzip compressed data, was "pymg-2.0.1.tar", last modified: Tue May 30 15:16:58 2023, max compression
```

## Comparing `pymg-1.0.0.tar` & `pymg-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,16 @@
-drwxr-xr-x   0 mimseyedi   (501) staff       (20)        0 2023-05-07 08:38:32.662390 pymg-1.0.0/
--rw-r--r--   0 mimseyedi   (501) staff       (20)    35129 2023-05-03 19:17:09.000000 pymg-1.0.0/LICENSE
--rw-r--r--   0 mimseyedi   (501) staff       (20)       67 2023-05-07 08:31:31.000000 pymg-1.0.0/MANIFEST.in
--rw-r--r--   0 mimseyedi   (501) staff       (20)     3254 2023-05-07 08:38:32.662285 pymg-1.0.0/PKG-INFO
--rw-r--r--   0 mimseyedi   (501) staff       (20)     2625 2023-05-07 06:55:27.000000 pymg-1.0.0/README.md
-drwxr-xr-x   0 mimseyedi   (501) staff       (20)        0 2023-05-07 08:38:32.661238 pymg-1.0.0/pymg/
--rw-r--r--   0 mimseyedi   (501) staff       (20)        0 2023-05-03 19:21:55.000000 pymg-1.0.0/pymg/__init__.py
--rw-r--r--   0 mimseyedi   (501) staff       (20)    14555 2023-05-07 06:46:14.000000 pymg-1.0.0/pymg/pymg.py
-drwxr-xr-x   0 mimseyedi   (501) staff       (20)        0 2023-05-07 08:38:32.662140 pymg-1.0.0/pymg/template/
--rw-r--r--   0 mimseyedi   (501) staff       (20)     4099 2023-05-06 13:17:32.000000 pymg-1.0.0/pymg/template/FOOTER.json
--rw-r--r--   0 mimseyedi   (501) staff       (20)       26 2023-05-06 08:18:40.000000 pymg-1.0.0/pymg/template/HEADER.json
-drwxr-xr-x   0 mimseyedi   (501) staff       (20)        0 2023-05-07 08:38:32.661922 pymg-1.0.0/pymg.egg-info/
--rw-r--r--   0 mimseyedi   (501) staff       (20)     3254 2023-05-07 08:38:32.000000 pymg-1.0.0/pymg.egg-info/PKG-INFO
--rw-r--r--   0 mimseyedi   (501) staff       (20)      290 2023-05-07 08:38:32.000000 pymg-1.0.0/pymg.egg-info/SOURCES.txt
--rw-r--r--   0 mimseyedi   (501) staff       (20)       15 2023-05-07 08:38:32.000000 pymg-1.0.0/pymg.egg-info/dependency_links.txt
--rw-r--r--   0 mimseyedi   (501) staff       (20)       40 2023-05-07 08:38:32.000000 pymg-1.0.0/pymg.egg-info/entry_points.txt
--rw-r--r--   0 mimseyedi   (501) staff       (20)       15 2023-05-07 08:38:32.000000 pymg-1.0.0/pymg.egg-info/requires.txt
--rw-r--r--   0 mimseyedi   (501) staff       (20)        5 2023-05-07 08:38:32.000000 pymg-1.0.0/pymg.egg-info/top_level.txt
--rw-r--r--   0 mimseyedi   (501) staff       (20)       38 2023-05-07 08:38:32.662422 pymg-1.0.0/setup.cfg
--rw-r--r--   0 mimseyedi   (501) staff       (20)     1166 2023-05-07 08:33:26.000000 pymg-1.0.0/setup.py
+drwxr-xr-x   0 mimseyedi   (501) staff       (20)        0 2023-05-30 15:16:58.813490 pymg-2.0.1/
+-rw-r--r--   0 mimseyedi   (501) staff       (20)    35129 2023-05-03 19:17:09.000000 pymg-2.0.1/LICENSE
+-rw-r--r--   0 mimseyedi   (501) staff       (20)     1656 2023-05-30 15:16:58.813385 pymg-2.0.1/PKG-INFO
+-rw-r--r--   0 mimseyedi   (501) staff       (20)      985 2023-05-30 15:13:59.000000 pymg-2.0.1/README.md
+drwxr-xr-x   0 mimseyedi   (501) staff       (20)        0 2023-05-30 15:16:58.812559 pymg-2.0.1/pymg/
+-rw-r--r--   0 mimseyedi   (501) staff       (20)        0 2023-05-03 19:21:55.000000 pymg-2.0.1/pymg/__init__.py
+-rw-r--r--   0 mimseyedi   (501) staff       (20)    44032 2023-05-30 14:42:00.000000 pymg-2.0.1/pymg/pymg.py
+drwxr-xr-x   0 mimseyedi   (501) staff       (20)        0 2023-05-30 15:16:58.813249 pymg-2.0.1/pymg.egg-info/
+-rw-r--r--   0 mimseyedi   (501) staff       (20)     1656 2023-05-30 15:16:58.000000 pymg-2.0.1/pymg.egg-info/PKG-INFO
+-rw-r--r--   0 mimseyedi   (501) staff       (20)      226 2023-05-30 15:16:58.000000 pymg-2.0.1/pymg.egg-info/SOURCES.txt
+-rw-r--r--   0 mimseyedi   (501) staff       (20)       20 2023-05-30 15:16:58.000000 pymg-2.0.1/pymg.egg-info/dependency_links.txt
+-rw-r--r--   0 mimseyedi   (501) staff       (20)       40 2023-05-30 15:16:58.000000 pymg-2.0.1/pymg.egg-info/entry_points.txt
+-rw-r--r--   0 mimseyedi   (501) staff       (20)       20 2023-05-30 15:16:58.000000 pymg-2.0.1/pymg.egg-info/requires.txt
+-rw-r--r--   0 mimseyedi   (501) staff       (20)        5 2023-05-30 15:16:58.000000 pymg-2.0.1/pymg.egg-info/top_level.txt
+-rw-r--r--   0 mimseyedi   (501) staff       (20)       38 2023-05-30 15:16:58.813530 pymg-2.0.1/setup.cfg
+-rw-r--r--   0 mimseyedi   (501) staff       (20)     1193 2023-05-30 15:16:37.000000 pymg-2.0.1/setup.py
```

### Comparing `pymg-1.0.0/LICENSE` & `pymg-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymg-1.0.0/setup.py` & `pymg-2.0.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 
 HERE = Path(__file__).parent
 README = (HERE / "README.md").read_text()
-install_requires = ['click', 'requests']
-dependency_links = ['click', 'requests']
+install_requires = ['rich', 'click', 'requests']
+dependency_links = ['rich', 'click', 'requests']
 
 
 setup (
  name = 'pymg',
- description = 'pymg is a CLI tool that can interpret Python files and display errors in a more optimized and more readable way.',
- version = '1.0.0',
+ description = 'pymg is a CLI tool that can interpret Python files by the Python interpreter and display the error message in a more readable way if an exception occurs.',
+ version = '2.0.1',
  packages = find_packages(),
- include_package_data = True,
  install_requires = install_requires,
  python_requires='>=3.11',
  entry_points='''
         [console_scripts]
         pymg=pymg.pymg:main
     ''',
  author="mimseyedi",
```

