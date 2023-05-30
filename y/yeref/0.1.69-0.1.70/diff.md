# Comparing `tmp/yeref-0.1.69.tar.gz` & `tmp/yeref-0.1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.69.tar", last modified: Tue May 30 11:54:26 2023, max compression
+gzip compressed data, was "yeref-0.1.70.tar", last modified: Tue May 30 13:53:48 2023, max compression
```

## Comparing `yeref-0.1.69.tar` & `yeref-0.1.70.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 11:54:26.657080 yeref-0.1.69/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 11:54:26.657357 yeref-0.1.69/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-30 11:54:26.659049 yeref-0.1.69/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1372 2023-05-30 11:54:26.000000 yeref-0.1.69/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 11:54:26.646666 yeref-0.1.69/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.69/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   489276 2023-05-30 09:13:09.000000 yeref-0.1.69/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   205925 2023-05-30 11:53:26.000000 yeref-0.1.69/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 11:54:26.654743 yeref-0.1.69/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 11:54:26.000000 yeref-0.1.69/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-30 11:54:26.000000 yeref-0.1.69/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-30 11:54:26.000000 yeref-0.1.69/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-30 11:54:26.000000 yeref-0.1.69/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 13:53:48.786630 yeref-0.1.70/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 13:53:48.786772 yeref-0.1.70/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-30 13:53:48.787347 yeref-0.1.70/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1392 2023-05-30 13:53:38.000000 yeref-0.1.70/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 13:53:48.782791 yeref-0.1.70/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.70/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   489276 2023-05-30 09:13:09.000000 yeref-0.1.70/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   206005 2023-05-30 13:53:38.000000 yeref-0.1.70/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 13:53:48.786250 yeref-0.1.70/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 13:53:48.000000 yeref-0.1.70/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-30 13:53:48.000000 yeref-0.1.70/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-30 13:53:48.000000 yeref-0.1.70/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-30 13:53:48.000000 yeref-0.1.70/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.69/setup.py` & `yeref-0.1.70/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.69',
+      version='0.1.70',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,15 +39,15 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 # freey.sitner.ya
-# 
+# cejwez-nosgin-vaVfe7
 
 # python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.66-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
```

### Comparing `yeref-0.1.69/yeref/l_.py` & `yeref-0.1.70/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.69/yeref/yeref.py` & `yeref-0.1.70/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,14 +297,16 @@
             POST_USERTID       BIGINT       NOT NULL,
             
             POST_TARGET        VARCHAR,
             POST_TEXT          VARCHAR,
             POST_MEDIATYPE     VARCHAR,
             POST_FILEID        VARCHAR,
             POST_FILEIDNOTE    VARCHAR,
+            POSTB_FILEID       VARCHAR,
+            POSTB_FILEIDNOTE   VARCHAR,
             POST_FILENAME      VARCHAR,
 
             POST_TGPHLINK      VARCHAR,
             POST_ISTGPH        BOOLEAN     DEFAULT 0,
             POST_BUTTON        VARCHAR,
             POST_ISBUTTON      BOOLEAN     DEFAULT 0,
             POST_ISSPOILER     BOOLEAN     DEFAULT 0,
```

