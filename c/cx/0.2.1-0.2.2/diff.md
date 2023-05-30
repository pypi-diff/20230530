# Comparing `tmp/cx-0.2.1.tar.gz` & `tmp/cx-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cx-0.2.1.tar", last modified: Thu Feb 25 11:59:10 2021, max compression
+gzip compressed data, was "cx-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cx-0.2.1.tar` & `cx-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      772 2021-02-25 11:58:58.674776 cx-0.2.1/.github/workflows/package.yml
--rw-r--r--   0        0        0      736 2021-02-25 11:58:58.674776 cx-0.2.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       65 2021-02-25 11:58:58.674776 cx-0.2.1/.gitignore
--rw-r--r--   0        0        0    16725 2021-02-25 11:58:58.674776 cx-0.2.1/LICENSE
--rw-r--r--   0        0        0     2732 2021-02-25 11:58:58.674776 cx-0.2.1/README.rst
--rw-r--r--   0        0        0      101 2021-02-25 11:58:58.674776 cx-0.2.1/cx/__init__.py
--rw-r--r--   0        0        0      833 2021-02-25 11:58:58.674776 cx-0.2.1/cx/cli.py
--rw-r--r--   0        0        0      465 2021-02-25 11:58:58.674776 cx-0.2.1/cx/clockwise.py
--rw-r--r--   0        0        0     2631 2021-02-25 11:58:58.674776 cx-0.2.1/cx/main.py
--rw-r--r--   0        0        0     1569 2021-02-25 11:58:58.678776 cx-0.2.1/cx/test.py
--rw-r--r--   0        0        0     1393 2021-02-25 11:58:58.678776 cx-0.2.1/cx/view_vectors.py
--rw-r--r--   0        0        0     1283 2021-02-25 11:58:58.678776 cx-0.2.1/example/boundary.txt
--rwxr-xr-x   0        0        0      193 2021-02-25 11:58:58.678776 cx-0.2.1/example/example.sh
--rw-r--r--   0        0        0      826 2021-02-25 11:58:58.678776 cx-0.2.1/example/islands.txt
--rw-r--r--   0        0        0     2667 2021-02-25 11:58:58.678776 cx-0.2.1/example/output/boundary.txt
--rw-r--r--   0        0        0     1648 2021-02-25 11:58:58.678776 cx-0.2.1/example/output/islands.txt
--rw-r--r--   0        0        0      435 2021-02-25 11:58:58.678776 cx-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       18 2021-02-25 11:58:58.678776 cx-0.2.1/requirements.txt
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 cx-0.2.1/setup.py
--rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 cx-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      815 2023-05-30 14:51:11.480442 cx-0.2.2/.github/workflows/package.yml
+-rw-r--r--   0        0        0      738 2023-05-30 14:51:11.480442 cx-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0       65 2023-05-30 14:51:11.480442 cx-0.2.2/.gitignore
+-rw-r--r--   0        0        0    16725 2023-05-30 14:51:11.484442 cx-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2732 2023-05-30 14:51:11.484442 cx-0.2.2/README.rst
+-rw-r--r--   0        0        0      101 2023-05-30 14:51:11.484442 cx-0.2.2/cx/__init__.py
+-rw-r--r--   0        0        0      833 2023-05-30 14:51:11.484442 cx-0.2.2/cx/cli.py
+-rw-r--r--   0        0        0      465 2023-05-30 14:51:11.484442 cx-0.2.2/cx/clockwise.py
+-rw-r--r--   0        0        0     2631 2023-05-30 14:51:11.484442 cx-0.2.2/cx/main.py
+-rw-r--r--   0        0        0     1569 2023-05-30 14:51:11.484442 cx-0.2.2/cx/test.py
+-rw-r--r--   0        0        0     1393 2023-05-30 14:51:11.484442 cx-0.2.2/cx/view_vectors.py
+-rw-r--r--   0        0        0     1283 2023-05-30 14:51:11.484442 cx-0.2.2/example/boundary.txt
+-rwxr-xr-x   0        0        0      193 2023-05-30 14:51:11.484442 cx-0.2.2/example/example.sh
+-rw-r--r--   0        0        0      826 2023-05-30 14:51:11.484442 cx-0.2.2/example/islands.txt
+-rw-r--r--   0        0        0     2667 2023-05-30 14:51:11.484442 cx-0.2.2/example/output/boundary.txt
+-rw-r--r--   0        0        0     1648 2023-05-30 14:51:11.484442 cx-0.2.2/example/output/islands.txt
+-rw-r--r--   0        0        0      435 2023-05-30 14:51:11.484442 cx-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-05-30 14:51:11.484442 cx-0.2.2/requirements.txt
+-rw-r--r--   0        0        0     3130 1970-01-01 00:00:00.000000 cx-0.2.2/PKG-INFO
```

### Comparing `cx-0.2.1/.github/workflows/package.yml` & `cx-0.2.2/.github/workflows/package.yml`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 on:
   release:
     types: [created]
 
 jobs:
   build:
-
+    permissions: write-all
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: [3.6]
+        python-version: ["3.8", "3.9", "3.10"]
         os: [ubuntu-latest]
 
     steps:
     - name: Switch branch
       uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
```

### Comparing `cx-0.2.1/.github/workflows/test.yml` & `cx-0.2.2/.github/workflows/test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: [3.6, 3.7, 3.8, 3.9]
+        python-version: ["3.8", "3.9", "3.10"]
         os: [ubuntu-latest, macOS-latest, windows-latest]
 
     steps:
     - name: Checkout
       uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
```

### Comparing `cx-0.2.1/LICENSE` & `cx-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cx-0.2.1/README.rst` & `cx-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `cx-0.2.1/cx/cli.py` & `cx-0.2.2/cx/cli.py`

 * *Files identical despite different names*

### Comparing `cx-0.2.1/cx/main.py` & `cx-0.2.2/cx/main.py`

 * *Files identical despite different names*

### Comparing `cx-0.2.1/cx/test.py` & `cx-0.2.2/cx/test.py`

 * *Files identical despite different names*

### Comparing `cx-0.2.1/cx/view_vectors.py` & `cx-0.2.2/cx/view_vectors.py`

 * *Files identical despite different names*

### Comparing `cx-0.2.1/example/boundary.txt` & `cx-0.2.2/example/boundary.txt`

 * *Files identical despite different names*

### Comparing `cx-0.2.1/example/islands.txt` & `cx-0.2.2/example/islands.txt`

 * *Files identical despite different names*

### Comparing `cx-0.2.1/example/output/boundary.txt` & `cx-0.2.2/example/output/boundary.txt`

 * *Files identical despite different names*

### Comparing `cx-0.2.1/example/output/islands.txt` & `cx-0.2.2/example/output/islands.txt`

 * *Files identical despite different names*

