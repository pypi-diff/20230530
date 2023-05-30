# Comparing `tmp/methodism-0.0.63.tar.gz` & `tmp/methodism-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodism-0.0.63.tar", last modified: Mon May 15 09:18:53 2023, max compression
+gzip compressed data, was "methodism-0.1.0.tar", last modified: Tue May 30 07:16:33 2023, max compression
```

## Comparing `methodism-0.0.63.tar` & `methodism-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:18:53.643958 methodism-0.0.63/
--rw-rw-rw-   0        0        0     2917 2023-05-15 09:18:53.643958 methodism-0.0.63/PKG-INFO
--rw-rw-rw-   0        0        0     2434 2023-04-28 10:28:06.000000 methodism-0.0.63/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 09:18:53.623492 methodism-0.0.63/methodism/
--rw-rw-rw-   0        0        0        0 2023-04-26 06:59:17.000000 methodism-0.0.63/methodism/__init__.py
--rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.0.63/methodism/costumizing.py
--rw-rw-rw-   0        0        0      772 2023-04-28 13:17:15.000000 methodism-0.0.63/methodism/decors.py
--rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.0.63/methodism/error_messages.py
--rw-rw-rw-   0        0        0     1296 2023-05-15 09:16:13.000000 methodism-0.0.63/methodism/helper.py
--rw-rw-rw-   0        0        0     3294 2023-04-28 10:28:06.000000 methodism-0.0.63/methodism/main.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:18:53.643958 methodism-0.0.63/methodism.egg-info/
--rw-rw-rw-   0        0        0     2917 2023-05-15 09:18:53.000000 methodism-0.0.63/methodism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-15 09:18:53.000000 methodism-0.0.63/methodism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:18:53.000000 methodism-0.0.63/methodism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-15 09:18:53.000000 methodism-0.0.63/methodism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      604 2023-05-15 09:18:18.000000 methodism-0.0.63/pyproject.toml
--rw-rw-rw-   0        0        0      546 2023-05-15 09:18:53.643958 methodism-0.0.63/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 07:16:33.296627 methodism-0.1.0/
+-rw-rw-rw-   0        0        0     3953 2023-05-30 07:16:33.296627 methodism-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3471 2023-05-30 06:58:48.000000 methodism-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 07:16:33.281012 methodism-0.1.0/methodism/
+-rw-rw-rw-   0        0        0      399 2023-05-29 07:36:13.000000 methodism-0.1.0/methodism/__init__.py
+-rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.1.0/methodism/costumizing.py
+-rw-rw-rw-   0        0        0      856 2023-05-30 07:16:02.000000 methodism-0.1.0/methodism/decors.py
+-rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.1.0/methodism/error_messages.py
+-rw-rw-rw-   0        0        0     2192 2023-05-29 07:11:47.000000 methodism-0.1.0/methodism/helper.py
+-rw-rw-rw-   0        0        0     6883 2023-05-30 06:51:39.000000 methodism-0.1.0/methodism/main.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:16:33.296627 methodism-0.1.0/methodism.egg-info/
+-rw-rw-rw-   0        0        0     3953 2023-05-30 07:16:33.000000 methodism-0.1.0/methodism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-30 07:16:33.000000 methodism-0.1.0/methodism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 07:16:33.000000 methodism-0.1.0/methodism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 07:16:33.000000 methodism-0.1.0/methodism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      603 2023-05-30 06:43:18.000000 methodism-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      546 2023-05-30 07:16:33.296627 methodism-0.1.0/setup.cfg
```

### Comparing `methodism-0.0.63/PKG-INFO` & `methodism-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,12 @@
-Metadata-Version: 2.1
-Name: methodism
-Version: 0.0.63
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
 
-```python
+```
     pip install methodism
 ```
 ## About
 Ushbu Kutubxona Egamberdiyev Xudoyberdi Tomonidan yaratilgan bo'lib tog'ridan tog'ri django 
 kutubxonasi ustiga qurulgan. Bu sizga API lar yozganda uni tez ishlatish va tezroq API yozish imkoni beradi.
 Avtomatik tarzda siz yozgan funksiyani method ga aylantirgan holatda api hosil qiladi
 
@@ -47,21 +33,21 @@
 
 Yuklab olib bo'lgach O'zingizga  `views.py` faylida kerakli bo'lgan classni yozing va uni `urls.py` ga ulang,
 class ga esa `methodism/main.py` dagi `METHODIZM` classidan vorislik bering.  
 ### Example in `views.py`
 
 
 ```python
-from methodism.main import METHODIZM
+from methodism.main import METHODISM
 
 # agar bundan foydalansangiz settings.INSTALLED_APPS ga 'rest_framework.authtoken' ni qo'shib qo'ying
 from rest_framework.authtoken.models import Token 
 
 
-class YourClass(METHODIZM):
+class YourClass(METHODISM):
 
     file = '__main__'
     token_key = "Bearer"
     auth_headers = "Authorization"
     token_class = Token
     not_auth_methods = [] # ro'yxatdan o'tish shart bo'lmagan kutubxonalarni qo'shib qo'ying
     
@@ -72,14 +58,42 @@
         methodizm:
             salom.dunyo
         
         siz yozgan har qanday ostki chiziqli yoki oddiy chiziqli funksiyalar nuqta orqali avtomatik ajratiladi!
         not_auth_methods = ['salom.dunyo']
      """
 ```
+# Navbatdagi class SqlAPIMethodism
+
+```python
+from methodism.main import SqlAPIMethodism
+
+# agar bundan foydalansangiz settings.INSTALLED_APPS ga 'rest_framework.authtoken' ni qo'shib qo'ying
+from rest_framework.authtoken.models import Token 
+# import your funksitions located file
+
+class YourClass(SqlAPIMethodism):
+
+    file = "__main__"  # funksiyalar joylashgan fileni hech qanday qo'shimchalarsiz tanishitiring
+    token_key = "Bearer"
+    auth_headers = "Authorization"
+    token_class = Token
+    not_auth_methods = [] # ro'yxatdan o'tish shart bo'lmagan kutubxonalarni qo'shib qo'ying
+    
+    
+    """ Misol uchun yozgan funksiyangiz:
+        def sizni_funksiyangiz(request, params):
+            return "select columns from your_table"       
+        
+        siz yozgan har qanday ostki chiziqli yoki oddiy chiziqli funksiyalar nuqta orqali avtomatik ajratiladi!
+        not_auth_methods = ['sizni.funksiyangiz']
+     """
+```
+
 
 ## [GitHub](https://github.com/xudikk/Methodism) Manba 
 ## [PyPi](https://pypi.org/project/methodism/) Manba
 
 # Happy Time. Enjoy IT ;)
 
+###### if you can't understand contact with [programmer](https://t.me/xudikk)
```

### Comparing `methodism-0.0.63/README.md` & `methodism-0.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,26 @@
+Metadata-Version: 2.1
+Name: methodism
+Version: 0.1.0
+Summary: Help to build APIs Faster
+Home-page: https://github.com/xudoyberdi123/Methodism
+Author: xudikk
+Author-email: xudikk <xudikk.1@gmail.com>
+Project-URL: Homepage, https://github.com/xudikk/Methodism
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # Methodism
 Methodism sizga djangoda API larni tezroq yaratish va tez ishlatish imkoni beradi.  
 ***Egamberdiyav Xudoyberdi Tomonidan Yaratilgan***
 
-```python
+```
     pip install methodism
 ```
 ## About
 Ushbu Kutubxona Egamberdiyev Xudoyberdi Tomonidan yaratilgan bo'lib tog'ridan tog'ri django 
 kutubxonasi ustiga qurulgan. Bu sizga API lar yozganda uni tez ishlatish va tezroq API yozish imkoni beradi.
 Avtomatik tarzda siz yozgan funksiyani method ga aylantirgan holatda api hosil qiladi
 
@@ -33,21 +47,21 @@
 
 Yuklab olib bo'lgach O'zingizga  `views.py` faylida kerakli bo'lgan classni yozing va uni `urls.py` ga ulang,
 class ga esa `methodism/main.py` dagi `METHODIZM` classidan vorislik bering.  
 ### Example in `views.py`
 
 
 ```python
-from methodism.main import METHODIZM
+from methodism.main import METHODISM
 
 # agar bundan foydalansangiz settings.INSTALLED_APPS ga 'rest_framework.authtoken' ni qo'shib qo'ying
 from rest_framework.authtoken.models import Token 
 
 
-class YourClass(METHODIZM):
+class YourClass(METHODISM):
 
     file = '__main__'
     token_key = "Bearer"
     auth_headers = "Authorization"
     token_class = Token
     not_auth_methods = [] # ro'yxatdan o'tish shart bo'lmagan kutubxonalarni qo'shib qo'ying
     
@@ -58,14 +72,42 @@
         methodizm:
             salom.dunyo
         
         siz yozgan har qanday ostki chiziqli yoki oddiy chiziqli funksiyalar nuqta orqali avtomatik ajratiladi!
         not_auth_methods = ['salom.dunyo']
      """
 ```
+# Navbatdagi class SqlAPIMethodism
+
+```python
+from methodism.main import SqlAPIMethodism
+
+# agar bundan foydalansangiz settings.INSTALLED_APPS ga 'rest_framework.authtoken' ni qo'shib qo'ying
+from rest_framework.authtoken.models import Token 
+# import your funksitions located file
+
+class YourClass(SqlAPIMethodism):
+
+    file = "__main__"  # funksiyalar joylashgan fileni hech qanday qo'shimchalarsiz tanishitiring
+    token_key = "Bearer"
+    auth_headers = "Authorization"
+    token_class = Token
+    not_auth_methods = [] # ro'yxatdan o'tish shart bo'lmagan kutubxonalarni qo'shib qo'ying
+    
+    
+    """ Misol uchun yozgan funksiyangiz:
+        def sizni_funksiyangiz(request, params):
+            return "select columns from your_table"       
+        
+        siz yozgan har qanday ostki chiziqli yoki oddiy chiziqli funksiyalar nuqta orqali avtomatik ajratiladi!
+        not_auth_methods = ['sizni.funksiyangiz']
+     """
+```
+
 
 ## [GitHub](https://github.com/xudikk/Methodism) Manba 
 ## [PyPi](https://pypi.org/project/methodism/) Manba
 
 # Happy Time. Enjoy IT ;)
 
+###### if you can't understand contact with [programmer](https://t.me/xudikk)
```

### Comparing `methodism-0.0.63/methodism/costumizing.py` & `methodism-0.1.0/methodism/costumizing.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.63/methodism/decors.py` & `methodism-0.1.0/methodism/decors.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 
 from rest_framework.response import Response
 
 from methodism.error_messages import MESSAGE
 from methodism.helper import custom_response
 
 
-# asosiy decorator
+# asosiy decorator method va params kalitlarini tekshirib oluvchi funksiya
 def method_and_params_checker(funk):
     def wrapper(self, req, *args, **kwargs):
         params = req.data.get('params')
         method = req.data.get("method")
         response = {
-            not method: Response(custom_response(status=False, message=MESSAGE['MethodMust'])),
-            params is None: Response(custom_response(status=False, message=MESSAGE['ParamsMust']))
-
+            not method: Response(custom_response(status=False, method=method, message=MESSAGE['MethodMust'])),
+            params is None: Response(custom_response(status=False, method=method, message=MESSAGE['ParamsMust']))
         }
         return response.get(True) or funk(self, req, *args, **kwargs)
 
     return wrapper
```

### Comparing `methodism-0.0.63/methodism/error_messages.py` & `methodism-0.1.0/methodism/error_messages.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.63/methodism.egg-info/PKG-INFO` & `methodism-0.1.0/methodism.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.0.63
+Version: 0.1.0
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Methodism
 Methodism sizga djangoda API larni tezroq yaratish va tez ishlatish imkoni beradi.  
 ***Egamberdiyav Xudoyberdi Tomonidan Yaratilgan***
 
-```python
+```
     pip install methodism
 ```
 ## About
 Ushbu Kutubxona Egamberdiyev Xudoyberdi Tomonidan yaratilgan bo'lib tog'ridan tog'ri django 
 kutubxonasi ustiga qurulgan. Bu sizga API lar yozganda uni tez ishlatish va tezroq API yozish imkoni beradi.
 Avtomatik tarzda siz yozgan funksiyani method ga aylantirgan holatda api hosil qiladi
 
@@ -47,21 +47,21 @@
 
 Yuklab olib bo'lgach O'zingizga  `views.py` faylida kerakli bo'lgan classni yozing va uni `urls.py` ga ulang,
 class ga esa `methodism/main.py` dagi `METHODIZM` classidan vorislik bering.  
 ### Example in `views.py`
 
 
 ```python
-from methodism.main import METHODIZM
+from methodism.main import METHODISM
 
 # agar bundan foydalansangiz settings.INSTALLED_APPS ga 'rest_framework.authtoken' ni qo'shib qo'ying
 from rest_framework.authtoken.models import Token 
 
 
-class YourClass(METHODIZM):
+class YourClass(METHODISM):
 
     file = '__main__'
     token_key = "Bearer"
     auth_headers = "Authorization"
     token_class = Token
     not_auth_methods = [] # ro'yxatdan o'tish shart bo'lmagan kutubxonalarni qo'shib qo'ying
     
@@ -72,14 +72,42 @@
         methodizm:
             salom.dunyo
         
         siz yozgan har qanday ostki chiziqli yoki oddiy chiziqli funksiyalar nuqta orqali avtomatik ajratiladi!
         not_auth_methods = ['salom.dunyo']
      """
 ```
+# Navbatdagi class SqlAPIMethodism
+
+```python
+from methodism.main import SqlAPIMethodism
+
+# agar bundan foydalansangiz settings.INSTALLED_APPS ga 'rest_framework.authtoken' ni qo'shib qo'ying
+from rest_framework.authtoken.models import Token 
+# import your funksitions located file
+
+class YourClass(SqlAPIMethodism):
+
+    file = "__main__"  # funksiyalar joylashgan fileni hech qanday qo'shimchalarsiz tanishitiring
+    token_key = "Bearer"
+    auth_headers = "Authorization"
+    token_class = Token
+    not_auth_methods = [] # ro'yxatdan o'tish shart bo'lmagan kutubxonalarni qo'shib qo'ying
+    
+    
+    """ Misol uchun yozgan funksiyangiz:
+        def sizni_funksiyangiz(request, params):
+            return "select columns from your_table"       
+        
+        siz yozgan har qanday ostki chiziqli yoki oddiy chiziqli funksiyalar nuqta orqali avtomatik ajratiladi!
+        not_auth_methods = ['sizni.funksiyangiz']
+     """
+```
+
 
 ## [GitHub](https://github.com/xudikk/Methodism) Manba 
 ## [PyPi](https://pypi.org/project/methodism/) Manba
 
 # Happy Time. Enjoy IT ;)
 
+###### if you can't understand contact with [programmer](https://t.me/xudikk)
```

### Comparing `methodism-0.0.63/pyproject.toml` & `methodism-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "djangorestframework>=3.14.0",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "methodism"
-version = "0.0.63"
+version = "0.1.0"
 authors = [
   { name="xudikk", email="xudikk.1@gmail.com" },
 ]
 description = "Help to build APIs Faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `methodism-0.0.63/setup.cfg` & `methodism-0.1.0/setup.cfg`

 * *Files identical despite different names*

