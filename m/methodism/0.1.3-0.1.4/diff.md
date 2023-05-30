# Comparing `tmp/methodism-0.1.3.tar.gz` & `tmp/methodism-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodism-0.1.3.tar", last modified: Tue May 30 07:31:42 2023, max compression
+gzip compressed data, was "methodism-0.1.4.tar", last modified: Tue May 30 07:54:23 2023, max compression
```

## Comparing `methodism-0.1.3.tar` & `methodism-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 07:31:42.282046 methodism-0.1.3/
--rw-rw-rw-   0        0        0     3953 2023-05-30 07:31:42.283024 methodism-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3471 2023-05-30 06:58:48.000000 methodism-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 07:31:42.265024 methodism-0.1.3/methodism/
--rw-rw-rw-   0        0        0      449 2023-05-30 07:21:18.000000 methodism-0.1.3/methodism/__init__.py
--rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.1.3/methodism/costumizing.py
--rw-rw-rw-   0        0        0      856 2023-05-30 07:16:02.000000 methodism-0.1.3/methodism/decors.py
--rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.1.3/methodism/error_messages.py
--rw-rw-rw-   0        0        0     2192 2023-05-29 07:11:47.000000 methodism-0.1.3/methodism/helper.py
--rw-rw-rw-   0        0        0     6883 2023-05-30 07:31:07.000000 methodism-0.1.3/methodism/main.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:31:42.281022 methodism-0.1.3/methodism.egg-info/
--rw-rw-rw-   0        0        0     3953 2023-05-30 07:31:42.000000 methodism-0.1.3/methodism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-30 07:31:42.000000 methodism-0.1.3/methodism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 07:31:42.000000 methodism-0.1.3/methodism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 07:31:42.000000 methodism-0.1.3/methodism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      603 2023-05-30 07:31:07.000000 methodism-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      546 2023-05-30 07:31:42.289025 methodism-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 07:54:23.194344 methodism-0.1.4/
+-rw-rw-rw-   0        0        0     4356 2023-05-30 07:54:23.194344 methodism-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3874 2023-05-30 07:51:57.000000 methodism-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 07:54:23.194344 methodism-0.1.4/methodism/
+-rw-rw-rw-   0        0        0      449 2023-05-30 07:21:18.000000 methodism-0.1.4/methodism/__init__.py
+-rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.1.4/methodism/costumizing.py
+-rw-rw-rw-   0        0        0      856 2023-05-30 07:16:02.000000 methodism-0.1.4/methodism/decors.py
+-rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.1.4/methodism/error_messages.py
+-rw-rw-rw-   0        0        0     2192 2023-05-29 07:11:47.000000 methodism-0.1.4/methodism/helper.py
+-rw-rw-rw-   0        0        0     6906 2023-05-30 07:48:34.000000 methodism-0.1.4/methodism/main.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:54:23.194344 methodism-0.1.4/methodism.egg-info/
+-rw-rw-rw-   0        0        0     4356 2023-05-30 07:54:23.000000 methodism-0.1.4/methodism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-30 07:54:23.000000 methodism-0.1.4/methodism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 07:54:23.000000 methodism-0.1.4/methodism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 07:54:23.000000 methodism-0.1.4/methodism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      603 2023-05-30 07:52:09.000000 methodism-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      546 2023-05-30 07:54:23.210244 methodism-0.1.4/setup.cfg
```

### Comparing `methodism-0.1.3/PKG-INFO` & `methodism-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: methodism
-Version: 0.1.3
-Summary: Help to build APIs Faster
-Home-page: https://github.com/xudoyberdi123/Methodism
-Author: xudikk
-Author-email: xudikk <xudikk.1@gmail.com>
-Project-URL: Homepage, https://github.com/xudikk/Methodism
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Methodism
 Methodism sizga djangoda API larni tezroq yaratish va tez ishlatish imkoni beradi.  
 ***Egamberdiyav Xudoyberdi Tomonidan Yaratilgan***
 
 ```
     pip install methodism
 ```
@@ -92,21 +78,30 @@
     auth_headers = "Authorization"
     token_class = Token
     not_auth_methods = [] # ro'yxatdan o'tish shart bo'lmagan kutubxonalarni qo'shib qo'ying
     
     
     """ Misol uchun yozgan funksiyangiz:
         def sizni_funksiyangiz(request, params):
-            return "select columns from your_table"       
+            return "select columns from your_table", True  # natija bitta bo'sa True ko'p bo'lsa False Qo'yiladi      
         
         siz yozgan har qanday ostki chiziqli yoki oddiy chiziqli funksiyalar nuqta orqali avtomatik ajratiladi!
         not_auth_methods = ['sizni.funksiyangiz']
      """
+
 ```
 
+### funksiya taxmianan shunaqa yozilishi shart!
+```python
+def funk(request, params):
+    return "select colums from your_table", False
+# sql zaprosga istalgancha uzunlik mumkin, funk 2ta qiymat strda->sql va ikkinchisi Bool typiga ega bo'lishi kerak
+# True -> agar natija bitta bo'lsa
+# False -> agar natija bittadan ko'p bo'lsa
+```
 
 ## [GitHub](https://github.com/xudikk/Methodism) Manba 
 ## [PyPi](https://pypi.org/project/methodism/) Manba
 
 # Happy Time. Enjoy IT ;)
 
 ###### if you can't understand contact with [programmer](https://t.me/xudikk)
```

### Comparing `methodism-0.1.3/methodism/costumizing.py` & `methodism-0.1.4/methodism/costumizing.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.3/methodism/decors.py` & `methodism-0.1.4/methodism/decors.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.3/methodism/error_messages.py` & `methodism-0.1.4/methodism/error_messages.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.3/methodism/helper.py` & `methodism-0.1.4/methodism/helper.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.3/methodism/main.py` & `methodism-0.1.4/methodism/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #  Created by Xudoyberdi Egamberdiyev
 #
 #  Please contact before making any changes
 #
 #  Tashkent, Uzbekistan
 from contextlib import closing
 
-from django.db import connections
+from django.db import connection
 from rest_framework.authtoken.models import Token
 from rest_framework.response import Response
-from rest_framework.permissions import AllowAny
 
 from re import compile as re_compile
 
 from methodism.costumizing import CustomGenericAPIView
 from methodism.decors import method_and_params_checker
 from methodism.error_messages import MESSAGE
 from methodism.helper import custom_response, exception_data, dictfetchone, dictfetchall
@@ -87,15 +86,15 @@
         not_auth_methods -> Ro'yxatdan o'tish talab qilinmaydigan funksiyalarni ko'rsating | list ko'rinishida
 
         Methodism sql zaproslarni spiga aylantirib beruvchi class!
 
         EXP:
             def your_funk(request, params):
                 # return "sql zapros"
-                return "select colums from your_table"
+                return "select colums from your_table", True  # True-returns one, False-returns many
 
 
         in methodism your_funk == your.funk
 
         DIQQAT !!!  BearerAuth yoki TokenAuthentication classlaridan foydalanish mumkin emas!!!
         """
 
@@ -131,19 +130,19 @@
             return Response(custom_response(False, method=method, message=MESSAGE['UndefinedError'],
                                             data=exception_data(e)))
         funk = map(funk, [requests], [params])
 
         # sql code larini ishlatish uchun!
         try:
             sql = list(funk)[0]
-            with closing(connections.cursor()) as cursor:
+            with closing(connection.cursor()) as cursor:
                 try:
                     cursor.execute(sql[0])
                     result = dictfetchone(cursor) if sql[1] else dictfetchall(cursor)
-                    response = Response(result)
+                    response = Response(custom_response(True, data=result))
                 except Exception as e:
                     response = Response(custom_response(False, method=method, message=MESSAGE['UndefinedError'],
                                                         data=exception_data(e)))
             response.data.update({'method': method})
 
         except Exception as e:
             response = Response(custom_response(False, method=method, message=MESSAGE['UndefinedError'],
```

### Comparing `methodism-0.1.3/methodism.egg-info/PKG-INFO` & `methodism-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.1.3
+Version: 0.1.4
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -92,21 +92,30 @@
     auth_headers = "Authorization"
     token_class = Token
     not_auth_methods = [] # ro'yxatdan o'tish shart bo'lmagan kutubxonalarni qo'shib qo'ying
     
     
     """ Misol uchun yozgan funksiyangiz:
         def sizni_funksiyangiz(request, params):
-            return "select columns from your_table"       
+            return "select columns from your_table", True  # natija bitta bo'sa True ko'p bo'lsa False Qo'yiladi      
         
         siz yozgan har qanday ostki chiziqli yoki oddiy chiziqli funksiyalar nuqta orqali avtomatik ajratiladi!
         not_auth_methods = ['sizni.funksiyangiz']
      """
+
 ```
 
+### funksiya taxmianan shunaqa yozilishi shart!
+```python
+def funk(request, params):
+    return "select colums from your_table", False
+# sql zaprosga istalgancha uzunlik mumkin, funk 2ta qiymat strda->sql va ikkinchisi Bool typiga ega bo'lishi kerak
+# True -> agar natija bitta bo'lsa
+# False -> agar natija bittadan ko'p bo'lsa
+```
 
 ## [GitHub](https://github.com/xudikk/Methodism) Manba 
 ## [PyPi](https://pypi.org/project/methodism/) Manba
 
 # Happy Time. Enjoy IT ;)
 
 ###### if you can't understand contact with [programmer](https://t.me/xudikk)
```

### Comparing `methodism-0.1.3/pyproject.toml` & `methodism-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "djangorestframework>=3.14.0",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "methodism"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="xudikk", email="xudikk.1@gmail.com" },
 ]
 description = "Help to build APIs Faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `methodism-0.1.3/setup.cfg` & `methodism-0.1.4/setup.cfg`

 * *Files identical despite different names*

