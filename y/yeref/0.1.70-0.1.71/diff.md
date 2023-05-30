# Comparing `tmp/yeref-0.1.70.tar.gz` & `tmp/yeref-0.1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.70.tar", last modified: Tue May 30 13:53:48 2023, max compression
+gzip compressed data, was "yeref-0.1.71.tar", last modified: Tue May 30 14:43:03 2023, max compression
```

## Comparing `yeref-0.1.70.tar` & `yeref-0.1.71.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 13:53:48.786630 yeref-0.1.70/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 13:53:48.786772 yeref-0.1.70/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-30 13:53:48.787347 yeref-0.1.70/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1392 2023-05-30 13:53:38.000000 yeref-0.1.70/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 13:53:48.782791 yeref-0.1.70/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.70/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   489276 2023-05-30 09:13:09.000000 yeref-0.1.70/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   206005 2023-05-30 13:53:38.000000 yeref-0.1.70/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 13:53:48.786250 yeref-0.1.70/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 13:53:48.000000 yeref-0.1.70/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-30 13:53:48.000000 yeref-0.1.70/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-30 13:53:48.000000 yeref-0.1.70/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-30 13:53:48.000000 yeref-0.1.70/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 14:43:03.920371 yeref-0.1.71/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 14:43:03.920611 yeref-0.1.71/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-30 14:43:03.921854 yeref-0.1.71/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1392 2023-05-30 14:42:44.000000 yeref-0.1.71/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 14:43:03.913062 yeref-0.1.71/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.71/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   489716 2023-05-30 14:42:24.000000 yeref-0.1.71/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   206005 2023-05-30 13:53:38.000000 yeref-0.1.71/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 14:43:03.919047 yeref-0.1.71/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 14:43:03.000000 yeref-0.1.71/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-30 14:43:03.000000 yeref-0.1.71/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-30 14:43:03.000000 yeref-0.1.71/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-30 14:43:03.000000 yeref-0.1.71/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.70/setup.py` & `yeref-0.1.71/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.70',
+      version='0.1.71',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.70/yeref/l_.py` & `yeref-0.1.71/yeref/l_.py`

 * *Files 1% similar despite different names*

```diff
@@ -572,14 +572,22 @@
     'ru': "📧 <b>Готово!</b> Рассылка запланирована",
     'en': "🗝️ <b>Done!</b> Newsletter scheduled",
     'es': "🗝️ <b>Listo!</b> Boletín programado",
     'fr': "🗝️ <b>C&#x27;est fait !</b> Newsletter prévue",
     'zh': "🗝️<b>完成！</b>已安排时事通讯",
     'ar': "🗝️ <b>انتهى!</b> النشرة الإخبارية المجدولة",
 }
+l_broadcast_plan_bot = {
+    'ru': "📧 <b>Готово!</b> Рассылка запланирована в @{0}",
+    'en': "🗝️ <b>Done!</b> Newsletter scheduled",
+    'es': "🗝️ <b>Listo!</b> Boletín programado",
+    'fr': "🗝️ <b>C&#x27;est fait !</b> Newsletter prévue",
+    'zh': "🗝️<b>完成！</b>已安排时事通讯",
+    'ar': "🗝️ <b>انتهى!</b> النشرة الإخبارية المجدولة",
+}
 l_broadcast_start = {
     'ru': "📧 <b>Старт</b> рассылки..\n#длительность {0}min",
     'en': "🗝️ <b>Start</b> mailing..\n#duration {0}min",
     'es': "🗝️ <b>Empezar a</b> enviar correos..\n#duración {0}min",
     'fr': "🗝️ <b>Lancer</b> l'envoi..\n#durée {0}min",
     'zh': "🗝️<b>开始</b>邮寄..\n#duration {0}min",
     'ar': "🗝️ <b>ابدأ</b> المراسلة ..\n# مدة {0} دقيقة",
```

### Comparing `yeref-0.1.70/yeref/yeref.py` & `yeref-0.1.71/yeref/yeref.py`

 * *Files identical despite different names*

