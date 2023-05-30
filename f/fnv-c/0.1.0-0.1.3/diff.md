# Comparing `tmp/fnv-c-0.1.0.tar.gz` & `tmp/fnv-c-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnv-c-0.1.0.tar", last modified: Tue May 30 13:31:08 2023, max compression
+gzip compressed data, was "dist/fnv-c-0.1.3.tar", last modified: Tue May 30 14:58:32 2023, max compression
```

## Comparing `fnv-c-0.1.0.tar` & `fnv-c-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxr-xr-x   0 fab        (501) staff       (20)        0 2023-05-30 13:31:08.592281 fnv-c-0.1.0/
--rw-r--r--   0 fab        (501) staff       (20)     1069 2023-05-23 16:00:33.000000 fnv-c-0.1.0/LICENSE
--rw-r--r--   0 fab        (501) staff       (20)      411 2023-05-30 13:31:08.592141 fnv-c-0.1.0/PKG-INFO
--rw-r--r--   0 fab        (501) staff       (20)     1216 2023-05-30 08:00:24.000000 fnv-c-0.1.0/README.md
-drwxr-xr-x   0 fab        (501) staff       (20)        0 2023-05-30 13:31:08.590619 fnv-c-0.1.0/fnv_c/
--rw-r--r--   0 fab        (501) staff       (20)      935 2023-05-30 07:38:03.000000 fnv-c-0.1.0/fnv_c/__init__.py
-drwxr-xr-x   0 fab        (501) staff       (20)        0 2023-05-30 13:31:08.591549 fnv-c-0.1.0/fnv_c/ext/
--rw-r--r--   0 fab        (501) staff       (20)        0 2023-05-23 16:00:33.000000 fnv-c-0.1.0/fnv_c/ext/__init__.py
--rw-r--r--   0 fab        (501) staff       (20)      465 2023-05-24 08:37:58.000000 fnv-c-0.1.0/fnv_c/ext/build.py
--rw-r--r--   0 fab        (501) staff       (20)     1682 2023-05-30 07:38:03.000000 fnv-c-0.1.0/fnv_c/ext/fnv.c
-drwxr-xr-x   0 fab        (501) staff       (20)        0 2023-05-30 13:31:08.591261 fnv-c-0.1.0/fnv_c.egg-info/
--rw-r--r--   0 fab        (501) staff       (20)      411 2023-05-30 13:31:08.000000 fnv-c-0.1.0/fnv_c.egg-info/PKG-INFO
--rw-r--r--   0 fab        (501) staff       (20)      280 2023-05-30 13:31:08.000000 fnv-c-0.1.0/fnv_c.egg-info/SOURCES.txt
--rw-r--r--   0 fab        (501) staff       (20)        1 2023-05-30 13:31:08.000000 fnv-c-0.1.0/fnv_c.egg-info/dependency_links.txt
--rw-r--r--   0 fab        (501) staff       (20)       12 2023-05-30 13:31:08.000000 fnv-c-0.1.0/fnv_c.egg-info/requires.txt
--rw-r--r--   0 fab        (501) staff       (20)        6 2023-05-30 13:31:08.000000 fnv-c-0.1.0/fnv_c.egg-info/top_level.txt
--rw-r--r--   0 fab        (501) staff       (20)      240 2023-05-23 16:00:33.000000 fnv-c-0.1.0/pyproject.toml
--rw-r--r--   0 fab        (501) staff       (20)       38 2023-05-30 13:31:08.592315 fnv-c-0.1.0/setup.cfg
--rw-r--r--   0 fab        (501) staff       (20)      657 2023-05-24 08:39:25.000000 fnv-c-0.1.0/setup.py
-drwxr-xr-x   0 fab        (501) staff       (20)        0 2023-05-30 13:31:08.591843 fnv-c-0.1.0/tests/
--rw-r--r--   0 fab        (501) staff       (20)      451 2023-05-24 08:30:53.000000 fnv-c-0.1.0/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:32.000000 fnv-c-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-30 14:58:32.000000 fnv-c-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-30 14:58:21.000000 fnv-c-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-30 14:58:21.000000 fnv-c-0.1.3/fnv_c/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:21.000000 fnv-c-0.1.3/fnv_c/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 14:58:21.000000 fnv-c-0.1.3/fnv_c/ext/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-30 14:58:21.000000 fnv-c-0.1.3/fnv_c/ext/fnv.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 14:58:32.000000 fnv-c-0.1.3/fnv_c.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 14:58:21.000000 fnv-c-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:58:32.000000 fnv-c-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-30 14:58:32.000000 fnv-c-0.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `fnv-c-0.1.0/README.md` & `fnv-c-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fnv-c-0.1.0/fnv_c/__init__.py` & `fnv-c-0.1.3/fnv_c/__init__.py`

 * *Files identical despite different names*

### Comparing `fnv-c-0.1.0/fnv_c/ext/fnv.c` & `fnv-c-0.1.3/fnv_c/ext/fnv.c`

 * *Files identical despite different names*

