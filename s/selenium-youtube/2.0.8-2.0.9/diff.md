# Comparing `tmp/selenium_youtube-2.0.8.tar.gz` & `tmp/selenium_youtube-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/selenium_youtube-2.0.8.tar", last modified: Sun Oct 24 09:08:14 2021, max compression
+gzip compressed data, was "dist/selenium_youtube-2.0.9.tar", last modified: Sun Oct 24 09:09:52 2021, max compression
```

## Comparing `selenium_youtube-2.0.8.tar` & `selenium_youtube-2.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2021-10-24 09:08:14.000000 selenium_youtube-2.0.8/
--rw-r--r--   0 kristofk (334975650) 1198310432     1079 2021-09-15 21:11:45.000000 selenium_youtube-2.0.8/LICENSE
--rw-r--r--   0 kristofk (334975650) 1198310432     3036 2021-10-24 09:08:14.000000 selenium_youtube-2.0.8/PKG-INFO
--rw-r--r--   0 kristofk (334975650) 1198310432     2322 2021-10-24 09:08:07.000000 selenium_youtube-2.0.8/README.md
-drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2021-10-24 09:08:14.000000 selenium_youtube-2.0.8/selenium_youtube/
--rw-r--r--   0 kristofk (334975650) 1198310432      281 2021-09-15 21:11:45.000000 selenium_youtube-2.0.8/selenium_youtube/__init__.py
-drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2021-10-24 09:08:14.000000 selenium_youtube-2.0.8/selenium_youtube/enums/
--rw-r--r--   0 kristofk (334975650) 1198310432        0 2021-09-15 21:11:45.000000 selenium_youtube-2.0.8/selenium_youtube/enums/__init__.py
--rw-r--r--   0 kristofk (334975650) 1198310432      759 2021-09-15 21:11:45.000000 selenium_youtube-2.0.8/selenium_youtube/enums/analytics_period.py
--rw-r--r--   0 kristofk (334975650) 1198310432      752 2021-09-15 21:11:45.000000 selenium_youtube-2.0.8/selenium_youtube/enums/analytics_tab.py
--rw-r--r--   0 kristofk (334975650) 1198310432     1699 2021-09-15 21:11:45.000000 selenium_youtube-2.0.8/selenium_youtube/enums/upload_status.py
--rw-r--r--   0 kristofk (334975650) 1198310432      674 2021-09-15 21:11:45.000000 selenium_youtube-2.0.8/selenium_youtube/enums/visibility.py
--rw-r--r--   0 kristofk (334975650) 1198310432    31039 2021-10-24 09:07:37.000000 selenium_youtube-2.0.8/selenium_youtube/youtube.py
-drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2021-10-24 09:08:14.000000 selenium_youtube-2.0.8/selenium_youtube.egg-info/
--rw-r--r--   0 kristofk (334975650) 1198310432     3036 2021-10-24 09:08:14.000000 selenium_youtube-2.0.8/selenium_youtube.egg-info/PKG-INFO
--rw-r--r--   0 kristofk (334975650) 1198310432      477 2021-10-24 09:08:14.000000 selenium_youtube-2.0.8/selenium_youtube.egg-info/SOURCES.txt
--rw-r--r--   0 kristofk (334975650) 1198310432        1 2021-10-24 09:08:14.000000 selenium_youtube-2.0.8/selenium_youtube.egg-info/dependency_links.txt
--rw-r--r--   0 kristofk (334975650) 1198310432      190 2021-10-24 09:08:14.000000 selenium_youtube-2.0.8/selenium_youtube.egg-info/requires.txt
--rw-r--r--   0 kristofk (334975650) 1198310432       17 2021-10-24 09:08:14.000000 selenium_youtube-2.0.8/selenium_youtube.egg-info/top_level.txt
--rw-r--r--   0 kristofk (334975650) 1198310432       38 2021-10-24 09:08:14.000000 selenium_youtube-2.0.8/setup.cfg
--rw-r--r--   0 kristofk (334975650) 1198310432     1315 2021-10-24 09:08:07.000000 selenium_youtube-2.0.8/setup.py
+drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2021-10-24 09:09:52.000000 selenium_youtube-2.0.9/
+-rw-r--r--   0 kristofk (334975650) 1198310432     1079 2021-09-15 21:11:45.000000 selenium_youtube-2.0.9/LICENSE
+-rw-r--r--   0 kristofk (334975650) 1198310432     3036 2021-10-24 09:09:52.000000 selenium_youtube-2.0.9/PKG-INFO
+-rw-r--r--   0 kristofk (334975650) 1198310432     2322 2021-10-24 09:09:48.000000 selenium_youtube-2.0.9/README.md
+drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2021-10-24 09:09:52.000000 selenium_youtube-2.0.9/selenium_youtube/
+-rw-r--r--   0 kristofk (334975650) 1198310432      281 2021-09-15 21:11:45.000000 selenium_youtube-2.0.9/selenium_youtube/__init__.py
+drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2021-10-24 09:09:52.000000 selenium_youtube-2.0.9/selenium_youtube/enums/
+-rw-r--r--   0 kristofk (334975650) 1198310432        0 2021-09-15 21:11:45.000000 selenium_youtube-2.0.9/selenium_youtube/enums/__init__.py
+-rw-r--r--   0 kristofk (334975650) 1198310432      759 2021-09-15 21:11:45.000000 selenium_youtube-2.0.9/selenium_youtube/enums/analytics_period.py
+-rw-r--r--   0 kristofk (334975650) 1198310432      752 2021-09-15 21:11:45.000000 selenium_youtube-2.0.9/selenium_youtube/enums/analytics_tab.py
+-rw-r--r--   0 kristofk (334975650) 1198310432     1699 2021-09-15 21:11:45.000000 selenium_youtube-2.0.9/selenium_youtube/enums/upload_status.py
+-rw-r--r--   0 kristofk (334975650) 1198310432      674 2021-09-15 21:11:45.000000 selenium_youtube-2.0.9/selenium_youtube/enums/visibility.py
+-rw-r--r--   0 kristofk (334975650) 1198310432    31039 2021-10-24 09:07:37.000000 selenium_youtube-2.0.9/selenium_youtube/youtube.py
+drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2021-10-24 09:09:52.000000 selenium_youtube-2.0.9/selenium_youtube.egg-info/
+-rw-r--r--   0 kristofk (334975650) 1198310432     3036 2021-10-24 09:09:52.000000 selenium_youtube-2.0.9/selenium_youtube.egg-info/PKG-INFO
+-rw-r--r--   0 kristofk (334975650) 1198310432      477 2021-10-24 09:09:52.000000 selenium_youtube-2.0.9/selenium_youtube.egg-info/SOURCES.txt
+-rw-r--r--   0 kristofk (334975650) 1198310432        1 2021-10-24 09:09:52.000000 selenium_youtube-2.0.9/selenium_youtube.egg-info/dependency_links.txt
+-rw-r--r--   0 kristofk (334975650) 1198310432      190 2021-10-24 09:09:52.000000 selenium_youtube-2.0.9/selenium_youtube.egg-info/requires.txt
+-rw-r--r--   0 kristofk (334975650) 1198310432       17 2021-10-24 09:09:52.000000 selenium_youtube-2.0.9/selenium_youtube.egg-info/top_level.txt
+-rw-r--r--   0 kristofk (334975650) 1198310432       38 2021-10-24 09:09:52.000000 selenium_youtube-2.0.9/setup.cfg
+-rw-r--r--   0 kristofk (334975650) 1198310432     1315 2021-10-24 09:09:48.000000 selenium_youtube-2.0.9/setup.py
```

### Comparing `selenium_youtube-2.0.8/LICENSE` & `selenium_youtube-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_youtube-2.0.8/PKG-INFO` & `selenium_youtube-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_youtube
-Version: 2.0.8
+Version: 2.0.9
 Summary: selenium_youtube
 Home-page: https://github.com/kkristof200/selenium_youtube
 Author: Kovács Kristóf-Attila & Péntek Zsolt
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `selenium_youtube-2.0.8/README.md` & `selenium_youtube-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `selenium_youtube-2.0.8/selenium_youtube/enums/analytics_period.py` & `selenium_youtube-2.0.9/selenium_youtube/enums/analytics_period.py`

 * *Files identical despite different names*

### Comparing `selenium_youtube-2.0.8/selenium_youtube/enums/analytics_tab.py` & `selenium_youtube-2.0.9/selenium_youtube/enums/analytics_tab.py`

 * *Files identical despite different names*

### Comparing `selenium_youtube-2.0.8/selenium_youtube/enums/upload_status.py` & `selenium_youtube-2.0.9/selenium_youtube/enums/upload_status.py`

 * *Files identical despite different names*

### Comparing `selenium_youtube-2.0.8/selenium_youtube/enums/visibility.py` & `selenium_youtube-2.0.9/selenium_youtube/enums/visibility.py`

 * *Files identical despite different names*

### Comparing `selenium_youtube-2.0.8/selenium_youtube/youtube.py` & `selenium_youtube-2.0.9/selenium_youtube/youtube.py`

 * *Files identical despite different names*

### Comparing `selenium_youtube-2.0.8/selenium_youtube.egg-info/PKG-INFO` & `selenium_youtube-2.0.9/selenium_youtube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-youtube
-Version: 2.0.8
+Version: 2.0.9
 Summary: selenium_youtube
 Home-page: https://github.com/kkristof200/selenium_youtube
 Author: Kovács Kristóf-Attila & Péntek Zsolt
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `selenium_youtube-2.0.8/setup.py` & `selenium_youtube-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,30 @@
     with open(readme_path, 'r') as f:
         long_description = f.read()
 else:
     long_description = 'selenium_youtube'
 
 setuptools.setup(
     name='selenium_youtube',
-    version='2.0.8',
+    version='2.0.9',
     author="Kovács Kristóf-Attila & Péntek Zsolt",
     description='selenium_youtube',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/kkristof200/selenium_youtube",
     packages=setuptools.find_packages(),
     install_requires=[
         'beautifulsoup4>=4.10.0',
         'kcu>=0.0.71',
         'kstopit>=0.0.10',
         'kyoutubescraper>=0.0.2',
         'noraise>=0.0.16',
         'selenium>=4.0.0b4',
         'selenium-browser>=0.0.12',
-        'selenium-firefox>=2.0.8',
+        'selenium-firefox>=2.0.7',
         'selenium-uploader-account>=0.2.1'
     ],
     classifiers=[
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

