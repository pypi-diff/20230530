# Comparing `tmp/aixlab.cn-0.1.1.tar.gz` & `tmp/aixlab.cn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixlab.cn-0.1.1.tar", last modified: Sat May  6 03:25:20 2023, max compression
+gzip compressed data, was "aixlab.cn-0.1.2.tar", last modified: Tue May 30 03:03:15 2023, max compression
```

## Comparing `aixlab.cn-0.1.1.tar` & `aixlab.cn-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 03:25:20.320842 aixlab.cn-0.1.1/
--rw-rw-rw-   0        0        0      201 2023-05-06 03:25:20.319849 aixlab.cn-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-06 03:25:20.319849 aixlab.cn-0.1.1/aixlab.cn.egg-info/
--rw-rw-rw-   0        0        0      201 2023-05-06 03:25:20.000000 aixlab.cn-0.1.1/aixlab.cn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-05-06 03:25:20.000000 aixlab.cn-0.1.1/aixlab.cn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 03:25:20.000000 aixlab.cn-0.1.1/aixlab.cn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-05-06 03:25:20.000000 aixlab.cn-0.1.1/aixlab.cn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 03:25:20.000000 aixlab.cn-0.1.1/aixlab.cn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 03:25:20.320842 aixlab.cn-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      529 2023-05-06 03:25:08.000000 aixlab.cn-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:03:15.014545 aixlab.cn-0.1.2/
+-rw-rw-rw-   0        0        0      201 2023-05-30 03:03:15.013546 aixlab.cn-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 03:03:15.012544 aixlab.cn-0.1.2/aixlab.cn.egg-info/
+-rw-rw-rw-   0        0        0      201 2023-05-30 03:03:14.000000 aixlab.cn-0.1.2/aixlab.cn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-05-30 03:03:14.000000 aixlab.cn-0.1.2/aixlab.cn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 03:03:14.000000 aixlab.cn-0.1.2/aixlab.cn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2023-05-30 03:03:14.000000 aixlab.cn-0.1.2/aixlab.cn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 03:03:14.000000 aixlab.cn-0.1.2/aixlab.cn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 03:03:15.014545 aixlab.cn-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      542 2023-05-30 03:02:56.000000 aixlab.cn-0.1.2/setup.py
```

### Comparing `aixlab.cn-0.1.1/setup.py` & `aixlab.cn-0.1.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aixlab.cn',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'opencv-contrib-python', 
         'Flask' ,
         'scipy',
         'matplotlib==3.2.2' ,
         'flask-cors',
-        'torch==1.6.0+cpu', 
-        'torchvision==0.7.0+cpu '
+        'torch==1.8.0', 
+        'torchvision==0.10.0',
+        'requests'
     ],
     author='Xu Ziyi',
     author_email='759946140@qq.com',
     description='Support for aixlab.cn',
     url='https://github.com/xuzycuan/aixlab.cn',
     license='MIT'
 )
```

