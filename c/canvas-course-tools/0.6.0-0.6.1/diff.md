# Comparing `tmp/canvas_course_tools-0.6.0.tar.gz` & `tmp/canvas_course_tools-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvas_course_tools-0.6.0.tar", max compression
+gzip compressed data, was "canvas_course_tools-0.6.1.tar", max compression
```

## Comparing `canvas_course_tools-0.6.0.tar` & `canvas_course_tools-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35129 2021-04-16 18:11:54.000000 canvas_course_tools-0.6.0/LICENSE
--rw-r--r--   0        0        0     1149 2023-02-21 16:38:48.000000 canvas_course_tools-0.6.0/README.md
--rw-r--r--   0        0        0     1181 2023-05-26 18:46:18.162541 canvas_course_tools-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      171 2023-05-28 14:30:27.596828 canvas_course_tools-0.6.0/src/canvas_course_tools/__init__.py
--rw-r--r--   0        0        0     6014 2023-05-26 16:34:41.489772 canvas_course_tools-0.6.0/src/canvas_course_tools/canvas_tasks.py
--rw-r--r--   0        0        0      925 2023-05-24 12:22:29.497305 canvas_course_tools-0.6.0/src/canvas_course_tools/cli.py
--rw-r--r--   0        0        0     1407 2023-02-20 18:42:01.000000 canvas_course_tools-0.6.0/src/canvas_course_tools/configfile.py
--rw-r--r--   0        0        0     4274 2023-05-24 12:28:18.600764 canvas_course_tools-0.6.0/src/canvas_course_tools/courses.py
--rw-r--r--   0        0        0     1366 2023-05-26 10:35:52.897835 canvas_course_tools-0.6.0/src/canvas_course_tools/datatypes.py
--rw-r--r--   0        0        0     2405 2023-03-06 20:34:05.114028 canvas_course_tools-0.6.0/src/canvas_course_tools/group_lists.py
--rw-r--r--   0        0        0     4066 2023-05-26 16:30:06.266271 canvas_course_tools-0.6.0/src/canvas_course_tools/groups.py
--rw-r--r--   0        0        0     1824 2023-03-06 12:04:47.022815 canvas_course_tools-0.6.0/src/canvas_course_tools/servers.py
--rw-r--r--   0        0        0     2102 2023-05-26 18:35:54.857315 canvas_course_tools-0.6.0/src/canvas_course_tools/students.py
--rwxr-xr-x   0        0        0     1171 2023-05-24 09:46:37.435270 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/exam.tex
--rwxr-xr-x   0        0        0      945 2023-02-21 10:44:19.000000 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/peer-feedback.tex
--rwxr-xr-x   0        0        0     1391 2023-05-26 18:44:58.002544 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/photos.tex
--rwxr-xr-x   0        0        0     1024 2023-02-21 10:48:56.000000 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/signatures.tex
--rwxr-xr-x   0        0        0      630 2023-02-21 14:27:49.000000 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/student-list-pairs.tex
--rwxr-xr-x   0        0        0      546 2023-02-21 14:27:59.000000 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/student-list.tex
--rw-r--r--   0        0        0      245 2023-03-06 20:40:35.976728 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/student-list.txt
--rw-r--r--   0        0        0      379 2023-03-06 15:35:56.420385 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/template-info.toml
--rw-r--r--   0        0        0     7076 2023-05-24 12:40:34.346462 canvas_course_tools-0.6.0/src/canvas_course_tools/templates.py
--rw-r--r--   0        0        0      836 2023-05-26 16:21:14.865830 canvas_course_tools-0.6.0/src/canvas_course_tools/utils.py
--rw-r--r--   0        0        0     2495 1970-01-01 00:00:00.000000 canvas_course_tools-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35129 2021-04-16 18:11:54.000000 canvas_course_tools-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1149 2023-02-21 16:38:48.000000 canvas_course_tools-0.6.1/README.md
+-rw-r--r--   0        0        0     1182 2023-05-30 09:37:25.530028 canvas_course_tools-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      171 2023-05-28 14:30:27.596828 canvas_course_tools-0.6.1/src/canvas_course_tools/__init__.py
+-rw-r--r--   0        0        0     6014 2023-05-26 16:34:41.489772 canvas_course_tools-0.6.1/src/canvas_course_tools/canvas_tasks.py
+-rw-r--r--   0        0        0      925 2023-05-24 12:22:29.497305 canvas_course_tools-0.6.1/src/canvas_course_tools/cli.py
+-rw-r--r--   0        0        0     1407 2023-02-20 18:42:01.000000 canvas_course_tools-0.6.1/src/canvas_course_tools/configfile.py
+-rw-r--r--   0        0        0     4274 2023-05-24 12:28:18.600764 canvas_course_tools-0.6.1/src/canvas_course_tools/courses.py
+-rw-r--r--   0        0        0     1366 2023-05-26 10:35:52.897835 canvas_course_tools-0.6.1/src/canvas_course_tools/datatypes.py
+-rw-r--r--   0        0        0     2405 2023-03-06 20:34:05.114028 canvas_course_tools-0.6.1/src/canvas_course_tools/group_lists.py
+-rw-r--r--   0        0        0     4066 2023-05-26 16:30:06.266271 canvas_course_tools-0.6.1/src/canvas_course_tools/groups.py
+-rw-r--r--   0        0        0     1824 2023-03-06 12:04:47.022815 canvas_course_tools-0.6.1/src/canvas_course_tools/servers.py
+-rw-r--r--   0        0        0     2102 2023-05-26 18:35:54.857315 canvas_course_tools-0.6.1/src/canvas_course_tools/students.py
+-rwxr-xr-x   0        0        0     1171 2023-05-24 09:46:37.435270 canvas_course_tools-0.6.1/src/canvas_course_tools/templates/exam.tex
+-rwxr-xr-x   0        0        0      945 2023-02-21 10:44:19.000000 canvas_course_tools-0.6.1/src/canvas_course_tools/templates/peer-feedback.tex
+-rwxr-xr-x   0        0        0     1391 2023-05-26 18:44:58.002544 canvas_course_tools-0.6.1/src/canvas_course_tools/templates/photos.tex
+-rwxr-xr-x   0        0        0     1024 2023-02-21 10:48:56.000000 canvas_course_tools-0.6.1/src/canvas_course_tools/templates/signatures.tex
+-rwxr-xr-x   0        0        0      630 2023-02-21 14:27:49.000000 canvas_course_tools-0.6.1/src/canvas_course_tools/templates/student-list-pairs.tex
+-rwxr-xr-x   0        0        0      546 2023-02-21 14:27:59.000000 canvas_course_tools-0.6.1/src/canvas_course_tools/templates/student-list.tex
+-rw-r--r--   0        0        0      245 2023-03-06 20:40:35.976728 canvas_course_tools-0.6.1/src/canvas_course_tools/templates/student-list.txt
+-rw-r--r--   0        0        0      379 2023-03-06 15:35:56.420385 canvas_course_tools-0.6.1/src/canvas_course_tools/templates/template-info.toml
+-rw-r--r--   0        0        0     7076 2023-05-24 12:40:34.346462 canvas_course_tools-0.6.1/src/canvas_course_tools/templates.py
+-rw-r--r--   0        0        0      836 2023-05-26 16:21:14.865830 canvas_course_tools-0.6.1/src/canvas_course_tools/utils.py
+-rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 canvas_course_tools-0.6.1/PKG-INFO
```

### Comparing `canvas_course_tools-0.6.0/LICENSE` & `canvas_course_tools-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/README.md` & `canvas_course_tools-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/pyproject.toml` & `canvas_course_tools-0.6.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "canvas-course-tools"
-version = "0.6.0"
+version = "0.6.1"
 homepage = "https://github.com/davidfokkema/canvas-course-tools"
 description = "Canvas course tools"
 authors = ["David Fokkema <d.b.r.a.fokkema@vu.nl>"]
 readme = "README.md"
 packages = [{include = "canvas_course_tools", from = "src"}]
 license = "GPL-3.0-or-later"
 classifiers = [
@@ -20,15 +20,15 @@
 ]
 
 
 [tool.poetry.scripts]
 canvas = "canvas_course_tools.cli:cli"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 click = "^8.1.3"
 appdirs = "^1.4.4"
 rich = "^13.3.5"
 canvasapi = "^3.1.0"
 python-dateutil = "^2.8.1"
 rich-click = "^1.5.2"
 jinja2 = "^3.1.2"
```

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/canvas_tasks.py` & `canvas_course_tools-0.6.1/src/canvas_course_tools/canvas_tasks.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/cli.py` & `canvas_course_tools-0.6.1/src/canvas_course_tools/cli.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/configfile.py` & `canvas_course_tools-0.6.1/src/canvas_course_tools/configfile.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/courses.py` & `canvas_course_tools-0.6.1/src/canvas_course_tools/courses.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/datatypes.py` & `canvas_course_tools-0.6.1/src/canvas_course_tools/datatypes.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/group_lists.py` & `canvas_course_tools-0.6.1/src/canvas_course_tools/group_lists.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/groups.py` & `canvas_course_tools-0.6.1/src/canvas_course_tools/groups.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/servers.py` & `canvas_course_tools-0.6.1/src/canvas_course_tools/servers.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/students.py` & `canvas_course_tools-0.6.1/src/canvas_course_tools/students.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/templates/exam.tex` & `canvas_course_tools-0.6.1/src/canvas_course_tools/templates/exam.tex`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/templates/peer-feedback.tex` & `canvas_course_tools-0.6.1/src/canvas_course_tools/templates/peer-feedback.tex`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/templates/photos.tex` & `canvas_course_tools-0.6.1/src/canvas_course_tools/templates/photos.tex`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/templates/signatures.tex` & `canvas_course_tools-0.6.1/src/canvas_course_tools/templates/signatures.tex`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/templates/student-list-pairs.tex` & `canvas_course_tools-0.6.1/src/canvas_course_tools/templates/student-list-pairs.tex`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/templates/student-list.tex` & `canvas_course_tools-0.6.1/src/canvas_course_tools/templates/student-list.tex`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/templates.py` & `canvas_course_tools-0.6.1/src/canvas_course_tools/templates.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/src/canvas_course_tools/utils.py` & `canvas_course_tools-0.6.1/src/canvas_course_tools/utils.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.6.0/PKG-INFO` & `canvas_course_tools-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: canvas-course-tools
-Version: 0.6.0
+Version: 0.6.1
 Summary: Canvas course tools
 Home-page: https://github.com/davidfokkema/canvas-course-tools
 License: GPL-3.0-or-later
 Author: David Fokkema
 Author-email: d.b.r.a.fokkema@vu.nl
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: canvasapi (>=3.1.0,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
```

