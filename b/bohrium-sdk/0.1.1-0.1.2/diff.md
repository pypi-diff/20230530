# Comparing `tmp/bohrium-sdk-0.1.1.tar.gz` & `tmp/bohrium-sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.1.1.tar", last modified: Tue May 30 07:14:33 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.1.2.tar", last modified: Tue May 30 07:19:45 2023, max compression
```

## Comparing `bohrium-sdk-0.1.1.tar` & `bohrium-sdk-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:14:33.683892 bohrium-sdk-0.1.1/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-30 07:14:33.683622 bohrium-sdk-0.1.1/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.1.1/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:14:33.670118 bohrium-sdk-0.1.1/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-30 07:14:33.000000 bohrium-sdk-0.1.1/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      459 2023-05-30 07:14:33.000000 bohrium-sdk-0.1.1/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-30 07:14:33.000000 bohrium-sdk-0.1.1/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-30 07:14:33.000000 bohrium-sdk-0.1.1/bohrium_sdk.egg-info/entry_points.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-05-30 07:14:33.000000 bohrium-sdk-0.1.1/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:14:33.682366 bohrium-sdk-0.1.1/bohriumsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.1.1/bohriumsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.1.1/bohriumsdk/__main__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     6220 2023-05-30 07:14:12.000000 bohrium-sdk-0.1.1/bohriumsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1970 2023-05-30 07:06:19.000000 bohrium-sdk-0.1.1/bohriumsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     3766 2023-05-30 07:06:03.000000 bohrium-sdk-0.1.1/bohriumsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.1.1/bohriumsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2209 2023-05-30 07:06:47.000000 bohrium-sdk-0.1.1/bohriumsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2835 2023-05-30 07:06:55.000000 bohrium-sdk-0.1.1/bohriumsdk/storage.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:14:33.682933 bohrium-sdk-0.1.1/bohriumsdk/test/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.1.1/bohriumsdk/test/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.1.1/bohriumsdk/test/test_node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2369 2023-05-30 01:45:00.000000 bohrium-sdk-0.1.1/bohriumsdk/test.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     3120 2023-05-30 07:07:00.000000 bohrium-sdk-0.1.1/bohriumsdk/util.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-30 07:14:33.683950 bohrium-sdk-0.1.1/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      501 2023-05-30 07:14:29.000000 bohrium-sdk-0.1.1/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:19:45.748698 bohrium-sdk-0.1.2/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-30 07:19:45.748464 bohrium-sdk-0.1.2/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.1.2/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:19:45.740161 bohrium-sdk-0.1.2/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-30 07:19:45.000000 bohrium-sdk-0.1.2/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      459 2023-05-30 07:19:45.000000 bohrium-sdk-0.1.2/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-30 07:19:45.000000 bohrium-sdk-0.1.2/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-30 07:19:45.000000 bohrium-sdk-0.1.2/bohrium_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-05-30 07:19:45.000000 bohrium-sdk-0.1.2/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:19:45.747247 bohrium-sdk-0.1.2/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.1.2/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.1.2/bohriumsdk/__main__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     6220 2023-05-30 07:14:12.000000 bohrium-sdk-0.1.2/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1970 2023-05-30 07:06:19.000000 bohrium-sdk-0.1.2/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     3766 2023-05-30 07:06:03.000000 bohrium-sdk-0.1.2/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.1.2/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2209 2023-05-30 07:06:47.000000 bohrium-sdk-0.1.2/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2835 2023-05-30 07:06:55.000000 bohrium-sdk-0.1.2/bohriumsdk/storage.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:19:45.748009 bohrium-sdk-0.1.2/bohriumsdk/test/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.1.2/bohriumsdk/test/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.1.2/bohriumsdk/test/test_node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2369 2023-05-30 01:45:00.000000 bohrium-sdk-0.1.2/bohriumsdk/test.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     3159 2023-05-30 07:19:31.000000 bohrium-sdk-0.1.2/bohriumsdk/util.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-30 07:19:45.748759 bohrium-sdk-0.1.2/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      501 2023-05-30 07:19:42.000000 bohrium-sdk-0.1.2/setup.py
```

### Comparing `bohrium-sdk-0.1.1/bohriumsdk/client.py` & `bohrium-sdk-0.1.2/bohriumsdk/client.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.1/bohriumsdk/image.py` & `bohrium-sdk-0.1.2/bohriumsdk/image.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.1/bohriumsdk/job.py` & `bohrium-sdk-0.1.2/bohriumsdk/job.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.1/bohriumsdk/node.py` & `bohrium-sdk-0.1.2/bohriumsdk/node.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.1/bohriumsdk/project.py` & `bohrium-sdk-0.1.2/bohriumsdk/project.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.1/bohriumsdk/storage.py` & `bohrium-sdk-0.1.2/bohriumsdk/storage.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.1/bohriumsdk/test.py` & `bohrium-sdk-0.1.2/bohriumsdk/test.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.1/bohriumsdk/util.py` & `bohrium-sdk-0.1.2/bohriumsdk/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
     def nice_print_table(
             self,
             headers: list = [],
             items: list = []
         ) -> None:
 
-        table = Table()
+        table = Table(show_header=True, header_style="bold magenta", expand=True)
         for header in headers:
-            table.add_column(header, style="bold blue")
+            table.add_column(header)
         
         for row in items:
             table.add_row(*[str(item) for item in row])
 
         print(table)
 
 if __name__ == '__main__':
```

