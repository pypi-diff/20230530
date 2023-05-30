# Comparing `tmp/amhhandler-1.2.4.tar.gz` & `tmp/amhhandler-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ops/zzz/amh-handler/AmhHandler/dist/tmpnaatuhhw/amhhandler-1.2.4.tar", last modified: Wed Feb 15 11:33:13 2023, max compression
+gzip compressed data, was "/home/ops/zzz/amh-handler/AmhHandler/dist/tmpqumauvs1/amhhandler-1.2.5.tar", last modified: Tue May 30 07:26:26 2023, max compression
```

## Comparing `amhhandler-1.2.4.tar` & `amhhandler-1.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 11:33:13.000000 amhhandler-1.2.4/
--rw-r--r--   0 root         (0) root         (0)      866 2023-02-15 11:32:43.000000 amhhandler-1.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 11:33:13.000000 amhhandler-1.2.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 11:33:13.000000 amhhandler-1.2.4/src/amhhandler/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-02-15 11:32:43.000000 amhhandler-1.2.4/src/amhhandler/mysql.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-02-09 11:12:39.000000 amhhandler-1.2.4/src/amhhandler/shell.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-02-09 11:12:39.000000 amhhandler-1.2.4/src/amhhandler/drobot.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-02-09 11:12:39.000000 amhhandler-1.2.4/src/amhhandler/logger.py
--rw-r--r--   0 root         (0) root         (0)       19 2023-02-09 11:12:39.000000 amhhandler-1.2.4/src/amhhandler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 11:33:13.000000 amhhandler-1.2.4/src/amhhandler.egg-info/
--rw-r--r--   0 root         (0) root         (0)       17 2023-02-15 11:33:13.000000 amhhandler-1.2.4/src/amhhandler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-02-15 11:33:13.000000 amhhandler-1.2.4/src/amhhandler.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      355 2023-02-15 11:33:13.000000 amhhandler-1.2.4/src/amhhandler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-15 11:33:13.000000 amhhandler-1.2.4/src/amhhandler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1135 2023-02-15 11:33:13.000000 amhhandler-1.2.4/src/amhhandler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-15 11:33:13.000000 amhhandler-1.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      632 2023-02-09 11:12:39.000000 amhhandler-1.2.4/README.md
--rw-r--r--   0 root         (0) root         (0)      104 2023-02-09 11:12:39.000000 amhhandler-1.2.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1074 2023-02-09 11:12:39.000000 amhhandler-1.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1135 2023-02-15 11:33:13.000000 amhhandler-1.2.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:26:26.000000 amhhandler-1.2.5/
+-rw-r--r--   0 root         (0) root         (0)      866 2023-05-30 07:17:06.000000 amhhandler-1.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:26:26.000000 amhhandler-1.2.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:26:26.000000 amhhandler-1.2.5/src/amhhandler/
+-rw-r--r--   0 root         (0) root         (0)     1776 2023-05-30 07:17:06.000000 amhhandler-1.2.5/src/amhhandler/mysql.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-02-09 11:12:39.000000 amhhandler-1.2.5/src/amhhandler/shell.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-02-09 11:12:39.000000 amhhandler-1.2.5/src/amhhandler/drobot.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-02-09 11:12:39.000000 amhhandler-1.2.5/src/amhhandler/logger.py
+-rw-r--r--   0 root         (0) root         (0)       19 2023-02-09 11:12:39.000000 amhhandler-1.2.5/src/amhhandler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:26:26.000000 amhhandler-1.2.5/src/amhhandler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-30 07:26:26.000000 amhhandler-1.2.5/src/amhhandler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-30 07:26:26.000000 amhhandler-1.2.5/src/amhhandler.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-30 07:26:26.000000 amhhandler-1.2.5/src/amhhandler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 07:26:26.000000 amhhandler-1.2.5/src/amhhandler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      631 2023-05-30 07:26:26.000000 amhhandler-1.2.5/src/amhhandler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 07:26:26.000000 amhhandler-1.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      128 2023-05-30 07:17:06.000000 amhhandler-1.2.5/README.md
+-rw-r--r--   0 root         (0) root         (0)      104 2023-02-09 11:12:39.000000 amhhandler-1.2.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-02-09 11:12:39.000000 amhhandler-1.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      631 2023-05-30 07:26:26.000000 amhhandler-1.2.5/PKG-INFO
```

### Comparing `amhhandler-1.2.4/setup.py` & `amhhandler-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='amhhandler',       # 包名
-    version='1.2.4',         # 版本号
+    version='1.2.5',         # 版本号
     description='An even better way to work with Python.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='nbyue',
     author_email='20671413@163.com',
     url='https://gitee.com/nbyue/amh-handler',
     license="MIT",    # 开源协议
```

### Comparing `amhhandler-1.2.4/src/amhhandler/mysql.py` & `amhhandler-1.2.5/src/amhhandler/mysql.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             self.cur = self.conn.cursor()
         except Exception as e:
             sys.exit(e)
 
     def select(self, select_sql, return_type=None):
         """执行select, show 类查询，有返回值"""
         try:
-            if return_type in ("Dict", "dict", "d", "D"):
+            if return_type.lower() in ("dict", "d"):
                 self.cur = self.conn.cursor(DictCursor)
             self.cur.execute(select_sql)
             rt_tuple = self.cur.fetchall()
             return rt_tuple
         except Exception as e:
             print(e)
             return b''
```

### Comparing `amhhandler-1.2.4/src/amhhandler/shell.py` & `amhhandler-1.2.5/src/amhhandler/shell.py`

 * *Files identical despite different names*

### Comparing `amhhandler-1.2.4/src/amhhandler/drobot.py` & `amhhandler-1.2.5/src/amhhandler/drobot.py`

 * *Files identical despite different names*

### Comparing `amhhandler-1.2.4/src/amhhandler/logger.py` & `amhhandler-1.2.5/src/amhhandler/logger.py`

 * *Files identical despite different names*

### Comparing `amhhandler-1.2.4/LICENSE` & `amhhandler-1.2.5/LICENSE`

 * *Files identical despite different names*

