# Comparing `tmp/jixn_utils-0.0.2.tar.gz` & `tmp/jixn_utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jixn_utils-0.0.2.tar", last modified: Sat May  6 06:55:53 2023, max compression
+gzip compressed data, was "jixn_utils-0.0.3.tar", last modified: Tue May 30 07:53:25 2023, max compression
```

## Comparing `jixn_utils-0.0.2.tar` & `jixn_utils-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 06:55:53.271077 jixn_utils-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-05-06 06:29:33.000000 jixn_utils-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      419 2023-05-06 06:55:53.270079 jixn_utils-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-05-06 06:27:28.000000 jixn_utils-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 06:55:53.264078 jixn_utils-0.0.2/jixn_utils/
--rw-rw-rw-   0        0        0     2452 2023-04-20 03:16:10.000000 jixn_utils-0.0.2/jixn_utils/GetConfig.py
--rw-rw-rw-   0        0        0     3607 2023-03-10 07:58:55.000000 jixn_utils-0.0.2/jixn_utils/JudgeFile.py
--rw-rw-rw-   0        0        0        0 2023-05-06 06:24:35.000000 jixn_utils-0.0.2/jixn_utils/__init__.py
--rw-rw-rw-   0        0        0     8397 2023-05-06 06:22:15.000000 jixn_utils-0.0.2/jixn_utils/dbmysql.py
--rw-rw-rw-   0        0        0     3201 2023-03-21 07:10:32.000000 jixn_utils-0.0.2/jixn_utils/gen_guid.py
--rw-rw-rw-   0        0        0     9259 2023-04-20 03:16:10.000000 jixn_utils-0.0.2/jixn_utils/jixn_parser.py
--rw-rw-rw-   0        0        0    91465 2023-04-20 03:16:10.000000 jixn_utils-0.0.2/jixn_utils/jixn_parser_嵌套类型.py
--rw-rw-rw-   0        0        0    37882 2023-04-20 03:16:10.000000 jixn_utils-0.0.2/jixn_utils/jixn_utils.py
--rw-rw-rw-   0        0        0     2716 2023-04-20 03:16:10.000000 jixn_utils-0.0.2/jixn_utils/sendnews.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:55:53.268077 jixn_utils-0.0.2/jixn_utils.egg-info/
--rw-rw-rw-   0        0        0      419 2023-05-06 06:55:53.000000 jixn_utils-0.0.2/jixn_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-05-06 06:55:53.000000 jixn_utils-0.0.2/jixn_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 06:55:53.000000 jixn_utils-0.0.2/jixn_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 06:55:53.000000 jixn_utils-0.0.2/jixn_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 06:55:53.271077 jixn_utils-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1136 2023-05-06 06:55:46.000000 jixn_utils-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:53:25.022288 jixn_utils-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-05-06 06:29:33.000000 jixn_utils-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      419 2023-05-30 07:53:25.021287 jixn_utils-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-05-06 06:27:28.000000 jixn_utils-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 07:53:25.014285 jixn_utils-0.0.3/jixn_utils/
+-rw-rw-rw-   0        0        0     2452 2023-04-20 03:16:10.000000 jixn_utils-0.0.3/jixn_utils/GetConfig.py
+-rw-rw-rw-   0        0        0     3607 2023-03-10 07:58:55.000000 jixn_utils-0.0.3/jixn_utils/JudgeFile.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 06:24:35.000000 jixn_utils-0.0.3/jixn_utils/__init__.py
+-rw-rw-rw-   0        0        0     8524 2023-05-30 07:52:03.000000 jixn_utils-0.0.3/jixn_utils/dbmysql.py
+-rw-rw-rw-   0        0        0     3201 2023-03-21 07:10:32.000000 jixn_utils-0.0.3/jixn_utils/gen_guid.py
+-rw-rw-rw-   0        0        0     9259 2023-04-20 03:16:10.000000 jixn_utils-0.0.3/jixn_utils/jixn_parser.py
+-rw-rw-rw-   0        0        0    91465 2023-04-20 03:16:10.000000 jixn_utils-0.0.3/jixn_utils/jixn_parser_嵌套类型.py
+-rw-rw-rw-   0        0        0    37882 2023-04-20 03:16:10.000000 jixn_utils-0.0.3/jixn_utils/jixn_utils.py
+-rw-rw-rw-   0        0        0     2716 2023-04-20 03:16:10.000000 jixn_utils-0.0.3/jixn_utils/sendnews.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:53:25.019286 jixn_utils-0.0.3/jixn_utils.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-05-30 07:53:24.000000 jixn_utils-0.0.3/jixn_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-05-30 07:53:24.000000 jixn_utils-0.0.3/jixn_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 07:53:24.000000 jixn_utils-0.0.3/jixn_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-30 07:53:24.000000 jixn_utils-0.0.3/jixn_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 07:53:25.023288 jixn_utils-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1136 2023-05-30 07:53:21.000000 jixn_utils-0.0.3/setup.py
```

### Comparing `jixn_utils-0.0.2/LICENSE.txt` & `jixn_utils-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.2/jixn_utils/GetConfig.py` & `jixn_utils-0.0.3/jixn_utils/GetConfig.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.2/jixn_utils/JudgeFile.py` & `jixn_utils-0.0.3/jixn_utils/JudgeFile.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.2/jixn_utils/dbmysql.py` & `jixn_utils-0.0.3/jixn_utils/dbmysql.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # author:吉祥鸟
 # datetime:2018/10/22 14:41
 # software: PyCharm
 import time
-from pprint import pprint
-
-import pymysql
-import requests
-import random
+from pathlib import Path
+import pymysql,yaml
 import warnings
 
 
 warnings.filterwarnings("ignore")
 
 """
 个人常用存储库（此库不是所有的代码都会使用）
@@ -23,14 +20,17 @@
 5.单条信息插入或更新： ————  insert_update_one()
 6.多条信息插入或更新： ————  insert_update_many()
 7.单条信息更新： ————  update_one()
 8.单条信息插入忽略：———— insert_ignore_one()
 9.多条信息插入忽略： ———— insert_ignore_many()
 """
 
+f = Path(r"config/config_db.yaml").read_text(encoding="utf-8")
+config = yaml.safe_load(f)
+print(config)
 
 def open_local_db_dict(host,user,passwd,db,port=3306,charset='utf8'):
     """
     开启本地数据库
     :param db: 数据库（默认为spider）
     :return: 创建好的数据库连接
     """
@@ -83,22 +83,26 @@
             item_values = list(item.values())
             item_values[1] = str(item_values[1])
             # print item_values
             sql = sql1 + sql2[:-1] + sql3[:-1] + sql4[:-1]
             # print(sql)
             cursor.execute(sql, item_values)
             conn.commit()
-            # print(now_time(), "数据更新成功")
         except Exception as e:
             print(now_time(), '更新数据失败，回滚',e)
             conn.rollback()
+            return False
+        else:
+            return True
     else:
         print("无数据")
+        return True
     if _type:
         conn.close()
+    return False
 
 def classification_of_dict(items):
     itemsz = {}
     for item in items:
         type_str = ""
         for key in item.keys():
             type_str += key
```

### Comparing `jixn_utils-0.0.2/jixn_utils/gen_guid.py` & `jixn_utils-0.0.3/jixn_utils/gen_guid.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.2/jixn_utils/jixn_parser.py` & `jixn_utils-0.0.3/jixn_utils/jixn_parser.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.2/jixn_utils/jixn_parser_嵌套类型.py` & `jixn_utils-0.0.3/jixn_utils/jixn_parser_嵌套类型.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.2/jixn_utils/jixn_utils.py` & `jixn_utils-0.0.3/jixn_utils/jixn_utils.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.2/jixn_utils/sendnews.py` & `jixn_utils-0.0.3/jixn_utils/sendnews.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.2/setup.py` & `jixn_utils-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jixn_utils",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.2",  # 包版本号，便于维护版本
+    version="0.0.3",  # 包版本号，便于维护版本
     author="jixn",  # 作者，可以写自己的姓名
     author_email="jixn@example.com",  # 作者联系方式，可写自己的邮箱地址
     description="一个工具包啊这",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

