# Comparing `tmp/async-payok-0.1.5.tar.gz` & `tmp/async-payok-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-payok-0.1.5.tar", last modified: Tue May 30 07:18:13 2023, max compression
+gzip compressed data, was "async-payok-0.1.6.tar", last modified: Tue May 30 07:21:17 2023, max compression
```

## Comparing `async-payok-0.1.5.tar` & `async-payok-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 07:18:13.086274 async-payok-0.1.5/
--rw-rw-rw-   0        0        0     1278 2023-05-30 07:18:13.099675 async-payok-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      881 2023-05-30 07:18:00.000000 async-payok-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 07:18:13.051206 async-payok-0.1.5/async_payok/
--rw-rw-rw-   0        0        0      128 2023-05-27 05:54:41.000000 async-payok-0.1.5/async_payok/__init__.py
--rw-rw-rw-   0        0        0       25 2022-08-16 03:10:02.000000 async-payok-0.1.5/async_payok/__version__.py
--rw-rw-rw-   0        0        0     5874 2023-05-30 06:41:39.000000 async-payok-0.1.5/async_payok/asyncpayok.py
--rw-rw-rw-   0        0        0      138 2023-05-27 05:32:01.000000 async-payok-0.1.5/async_payok/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:18:13.085275 async-payok-0.1.5/async_payok/models/
--rw-rw-rw-   0        0        0      145 2023-05-27 05:54:41.000000 async-payok-0.1.5/async_payok/models/__init__.py
--rw-rw-rw-   0        0        0      162 2023-05-27 06:44:41.000000 async-payok-0.1.5/async_payok/models/balance.py
--rw-rw-rw-   0        0        0      199 2023-05-27 06:55:47.000000 async-payok-0.1.5/async_payok/models/enums.py
--rw-rw-rw-   0        0        0      496 2023-05-27 05:46:47.000000 async-payok-0.1.5/async_payok/models/invoice.py
--rw-rw-rw-   0        0        0      317 2023-05-27 06:55:47.000000 async-payok-0.1.5/async_payok/models/methods.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:18:13.081856 async-payok-0.1.5/async_payok.egg-info/
--rw-rw-rw-   0        0        0     1278 2023-05-30 07:18:12.000000 async-payok-0.1.5/async_payok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-05-30 07:18:13.000000 async-payok-0.1.5/async_payok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 07:18:12.000000 async-payok-0.1.5/async_payok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-30 07:18:12.000000 async-payok-0.1.5/async_payok.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2023-05-30 07:18:12.000000 async-payok-0.1.5/async_payok.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-30 07:18:12.000000 async-payok-0.1.5/async_payok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 07:18:13.100679 async-payok-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      929 2023-05-30 07:18:00.000000 async-payok-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:21:17.357699 async-payok-0.1.6/
+-rw-rw-rw-   0        0        0     1278 2023-05-30 07:21:17.414860 async-payok-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2023-05-30 07:21:04.000000 async-payok-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 07:21:17.347675 async-payok-0.1.6/async_payok/
+-rw-rw-rw-   0        0        0      128 2023-05-27 05:54:41.000000 async-payok-0.1.6/async_payok/__init__.py
+-rw-rw-rw-   0        0        0       25 2022-08-16 03:10:02.000000 async-payok-0.1.6/async_payok/__version__.py
+-rw-rw-rw-   0        0        0     5874 2023-05-30 06:41:39.000000 async-payok-0.1.6/async_payok/asyncpayok.py
+-rw-rw-rw-   0        0        0      138 2023-05-27 05:32:01.000000 async-payok-0.1.6/async_payok/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:21:17.356698 async-payok-0.1.6/async_payok/models/
+-rw-rw-rw-   0        0        0      145 2023-05-27 05:54:41.000000 async-payok-0.1.6/async_payok/models/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-05-27 06:44:41.000000 async-payok-0.1.6/async_payok/models/balance.py
+-rw-rw-rw-   0        0        0      199 2023-05-27 06:55:47.000000 async-payok-0.1.6/async_payok/models/enums.py
+-rw-rw-rw-   0        0        0      496 2023-05-27 05:46:47.000000 async-payok-0.1.6/async_payok/models/invoice.py
+-rw-rw-rw-   0        0        0      317 2023-05-27 06:55:47.000000 async-payok-0.1.6/async_payok/models/methods.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:21:17.353031 async-payok-0.1.6/async_payok.egg-info/
+-rw-rw-rw-   0        0        0     1278 2023-05-30 07:21:17.000000 async-payok-0.1.6/async_payok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-05-30 07:21:17.000000 async-payok-0.1.6/async_payok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 07:21:17.000000 async-payok-0.1.6/async_payok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-30 07:18:12.000000 async-payok-0.1.6/async_payok.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2023-05-30 07:21:17.000000 async-payok-0.1.6/async_payok.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-30 07:21:17.000000 async-payok-0.1.6/async_payok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 07:21:17.415861 async-payok-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      929 2023-05-30 07:21:04.000000 async-payok-0.1.6/setup.py
```

### Comparing `async-payok-0.1.5/PKG-INFO` & `async-payok-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-payok
-Version: 0.1.5
+Version: 0.1.6
 Summary: Asynchronous module for working with the Payok API
 Author: VoXDoX
 Author-email: 1voxdox1@gmail.com
 Project-URL: TG Channel, https://t.me/AsyncModules
 Project-URL: Github, https://github.com/VoXDoX/async-payok
 Keywords: payok,payok api,asyncpayok,aiopayok
 Requires-Python: >=3.7
@@ -21,16 +21,16 @@
 ```
 pip3 install async-payok
 ```
 ![изображение](https://imgur.com/OyxTv9W.jpg)
 
 
 # Information | Информация
-ENG: The current version of AsyncPayOk is 0.1.5
-RU: Актуальная версия AsyncPayOk 0.1.5
+ENG: The current version of AsyncPayOk is 0.1.6
+RU: Актуальная версия AsyncPayOk 0.1.6
 
 # Methods | Фyнкции
 ## ENG
 ```
 Asynchronous module for working with the Payok API
 
 What can?
```

### Comparing `async-payok-0.1.5/README.md` & `async-payok-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ```
 pip3 install async-payok
 ```
 ![изображение](https://imgur.com/OyxTv9W.jpg)
 
 
 # Information | Информация
-ENG: The current version of AsyncPayOk is 0.1.5
-RU: Актуальная версия AsyncPayOk 0.1.5
+ENG: The current version of AsyncPayOk is 0.1.6
+RU: Актуальная версия AsyncPayOk 0.1.6
 
 # Methods | Фyнкции
 ## ENG
 ```
 Asynchronous module for working with the Payok API
 
 What can?
```

### Comparing `async-payok-0.1.5/async_payok/asyncpayok.py` & `async-payok-0.1.6/async_payok/asyncpayok.py`

 * *Files identical despite different names*

### Comparing `async-payok-0.1.5/async_payok.egg-info/PKG-INFO` & `async-payok-0.1.6/async_payok.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-payok
-Version: 0.1.5
+Version: 0.1.6
 Summary: Asynchronous module for working with the Payok API
 Author: VoXDoX
 Author-email: 1voxdox1@gmail.com
 Project-URL: TG Channel, https://t.me/AsyncModules
 Project-URL: Github, https://github.com/VoXDoX/async-payok
 Keywords: payok,payok api,asyncpayok,aiopayok
 Requires-Python: >=3.7
@@ -21,16 +21,16 @@
 ```
 pip3 install async-payok
 ```
 ![изображение](https://imgur.com/OyxTv9W.jpg)
 
 
 # Information | Информация
-ENG: The current version of AsyncPayOk is 0.1.5
-RU: Актуальная версия AsyncPayOk 0.1.5
+ENG: The current version of AsyncPayOk is 0.1.6
+RU: Актуальная версия AsyncPayOk 0.1.6
 
 # Methods | Фyнкции
 ## ENG
 ```
 Asynchronous module for working with the Payok API
 
 What can?
```

### Comparing `async-payok-0.1.5/setup.py` & `async-payok-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 with open("README.md", "r", encoding="utf-8") as desc_long:
 	description_long = desc_long.read()
 
 
 setup(
 	name='async-payok',
-	version='0.1.5',
+	version='0.1.6',
 	description='Asynchronous module for working with the Payok API',
 	long_description=description_long,
 	packages=find_packages(),
 	long_description_content_type='text/markdown',
 	author='VoXDoX',
 	author_email='1voxdox1@gmail.com',
 	keywords=['payok', 'payok api', 'asyncpayok', 'aiopayok'],
```

