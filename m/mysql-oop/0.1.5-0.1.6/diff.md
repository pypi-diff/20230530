# Comparing `tmp/mysql-oop-0.1.5.tar.gz` & `tmp/mysql-oop-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-oop-0.1.5.tar", last modified: Tue May 30 10:41:33 2023, max compression
+gzip compressed data, was "mysql-oop-0.1.6.tar", last modified: Tue May 30 13:02:41 2023, max compression
```

## Comparing `mysql-oop-0.1.5.tar` & `mysql-oop-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 10:41:33.698450 mysql-oop-0.1.5/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1084 2023-05-28 08:47:28.000000 mysql-oop-0.1.5/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-30 10:41:33.698450 mysql-oop-0.1.5/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-05-29 08:33:20.000000 mysql-oop-0.1.5/README.md
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      157 2023-05-29 11:46:25.000000 mysql-oop-0.1.5/pyproject.toml
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      608 2023-05-30 10:41:33.698450 mysql-oop-0.1.5/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 10:41:33.694450 mysql-oop-0.1.5/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 10:41:33.698450 mysql-oop-0.1.5/src/mysql_oop.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-30 10:41:33.000000 mysql-oop-0.1.5/src/mysql_oop.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-05-30 10:41:33.000000 mysql-oop-0.1.5/src/mysql_oop.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-30 10:41:33.000000 mysql-oop-0.1.5/src/mysql_oop.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-30 10:41:33.000000 mysql-oop-0.1.5/src/mysql_oop.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 10:41:33.698450 mysql-oop-0.1.5/src/mysqloop/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      331 2023-05-30 10:23:10.000000 mysql-oop-0.1.5/src/mysqloop/BuildAttrs.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2522 2023-05-30 10:25:57.000000 mysql-oop-0.1.5/src/mysqloop/Model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      153 2023-05-29 08:53:58.000000 mysql-oop-0.1.5/src/mysqloop/Users.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       98 2023-05-30 03:42:13.000000 mysql-oop-0.1.5/src/mysqloop/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    15335 2023-05-30 07:46:13.000000 mysql-oop-0.1.5/src/mysqloop/mysqloop.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 13:02:41.112139 mysql-oop-0.1.6/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1084 2023-05-28 08:47:28.000000 mysql-oop-0.1.6/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-30 13:02:41.112139 mysql-oop-0.1.6/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-05-29 08:33:20.000000 mysql-oop-0.1.6/README.md
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      157 2023-05-29 11:46:25.000000 mysql-oop-0.1.6/pyproject.toml
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      608 2023-05-30 13:02:41.112139 mysql-oop-0.1.6/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 13:02:41.108139 mysql-oop-0.1.6/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 13:02:41.112139 mysql-oop-0.1.6/src/mysql_oop.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-30 13:02:41.000000 mysql-oop-0.1.6/src/mysql_oop.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-05-30 13:02:41.000000 mysql-oop-0.1.6/src/mysql_oop.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-30 13:02:41.000000 mysql-oop-0.1.6/src/mysql_oop.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-30 13:02:41.000000 mysql-oop-0.1.6/src/mysql_oop.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 13:02:41.112139 mysql-oop-0.1.6/src/mysqloop/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      331 2023-05-30 10:23:10.000000 mysql-oop-0.1.6/src/mysqloop/BuildAttrs.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2737 2023-05-30 13:01:23.000000 mysql-oop-0.1.6/src/mysqloop/Model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      153 2023-05-29 08:53:58.000000 mysql-oop-0.1.6/src/mysqloop/Users.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       98 2023-05-30 03:42:13.000000 mysql-oop-0.1.6/src/mysqloop/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    15335 2023-05-30 07:46:13.000000 mysql-oop-0.1.6/src/mysqloop/mysqloop.py
```

### Comparing `mysql-oop-0.1.5/LICENSE` & `mysql-oop-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-oop-0.1.5/PKG-INFO` & `mysql-oop-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-oop
-Version: 0.1.5
+Version: 0.1.6
 Summary: python mysql OOP class
 Home-page: https://github.com/hahadu/mysql-py-oop
 Author: hahadu
 Author-email: mhyzhu@163.com
 Project-URL: Bug Tracker, https://github.com/hahadu/mysql-py-oop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mysql-oop-0.1.5/README.md` & `mysql-oop-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mysql-oop-0.1.5/setup.cfg` & `mysql-oop-0.1.6/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mysql-oop
-version = 0.1.5
+version = 0.1.6
 author = hahadu
 author_email = mhyzhu@163.com
 description = python mysql OOP class
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hahadu/mysql-py-oop
 project_urls =
```

### Comparing `mysql-oop-0.1.5/src/mysql_oop.egg-info/PKG-INFO` & `mysql-oop-0.1.6/src/mysql_oop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-oop
-Version: 0.1.5
+Version: 0.1.6
 Summary: python mysql OOP class
 Home-page: https://github.com/hahadu/mysql-py-oop
 Author: hahadu
 Author-email: mhyzhu@163.com
 Project-URL: Bug Tracker, https://github.com/hahadu/mysql-py-oop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mysql-oop-0.1.5/src/mysqloop/Model.py` & `mysql-oop-0.1.6/src/mysqloop/Model.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,29 +50,36 @@
     def updateOrCreate(self, attributes, values: dict):
 
         if self.where(attributes).exists():
             return self.where(attributes).update(values)
         else:
             return self.create(attributes.update(values))
 
-    def save(self):
-
-        attrs = {}
-        for attr_column in vars(self).keys():
-            if attr_column[:1] != "_":
-                attrs.update({attr_column: self.__dict__[attr_column]})
+    def save(self, data: dict = None):
+        if data is not None:
+            attrs = data
+        else:
+            attrs = {}
+            for attr_column in vars(self).keys():
+                if attr_column[:1] != "_":
+                    attrs.update({attr_column: self.__dict__[attr_column]})
         return self.create(attrs)
 
     def get(self, columns="*"):
-        attrList = []
         datas = super().select(columns=columns)
+        data_list = []
         for data in datas:
             attrs = BuildAttrs()
 
             for item in data:
-                # print(data[item])
-                # print(item)
                 setattr(attrs, item, data[item])
-            print(attrs.toJson())
-            #print(attrs.id)
+            data_list.append(attrs)
 
-        print(datas)
+        return data_list
+        
+    def find(self, columns="*"):
+        data = super().find()
+        attrs = BuildAttrs()
+        for item in data:
+            setattr(attrs, item, data[item])
+        return attrs
+
```

### Comparing `mysql-oop-0.1.5/src/mysqloop/mysqloop.py` & `mysql-oop-0.1.6/src/mysqloop/mysqloop.py`

 * *Files identical despite different names*

