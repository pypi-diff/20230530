# Comparing `tmp/pythttp-0.0.8.tar.gz` & `tmp/pythttp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.0.8.tar", last modified: Tue May 30 16:11:44 2023, max compression
+gzip compressed data, was "pythttp-0.0.9.tar", last modified: Tue May 30 16:15:22 2023, max compression
```

## Comparing `pythttp-0.0.8.tar` & `pythttp-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 16:11:44.978352 pythttp-0.0.8/
--rw-rw-rw-   0        0        0     1093 2023-05-30 16:11:44.977271 pythttp-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.0.8/README.md
--rw-rw-rw-   0        0        0      419 2023-05-30 16:11:39.000000 pythttp-0.0.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-30 16:11:44.964744 pythttp-0.0.8/pythttp/
--rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.0.8/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     6620 2023-05-30 15:45:53.000000 pythttp-0.0.8/pythttp/Protocol.py
--rw-rw-rw-   0        0        0     2732 2023-05-17 09:20:38.000000 pythttp-0.0.8/pythttp/Structure.py
--rw-rw-rw-   0        0        0     3037 2023-05-30 15:45:28.000000 pythttp-0.0.8/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      108 2023-05-22 10:13:49.000000 pythttp-0.0.8/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 16:11:44.977271 pythttp-0.0.8/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-05-30 16:11:44.000000 pythttp-0.0.8/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-30 16:11:44.000000 pythttp-0.0.8/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 16:11:44.000000 pythttp-0.0.8/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 16:11:44.000000 pythttp-0.0.8/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 16:11:44.978352 pythttp-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-05-30 16:11:33.000000 pythttp-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:15:22.041201 pythttp-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2023-05-30 16:15:22.041201 pythttp-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.0.9/README.md
+-rw-rw-rw-   0        0        0      419 2023-05-30 16:15:20.000000 pythttp-0.0.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-30 16:15:22.030090 pythttp-0.0.9/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.0.9/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     6654 2023-05-30 16:14:59.000000 pythttp-0.0.9/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0     2732 2023-05-17 09:20:38.000000 pythttp-0.0.9/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     3037 2023-05-30 15:45:28.000000 pythttp-0.0.9/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      108 2023-05-22 10:13:49.000000 pythttp-0.0.9/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:15:22.040201 pythttp-0.0.9/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-05-30 16:15:21.000000 pythttp-0.0.9/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-30 16:15:21.000000 pythttp-0.0.9/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 16:15:21.000000 pythttp-0.0.9/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 16:15:21.000000 pythttp-0.0.9/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 16:15:22.041201 pythttp-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-05-30 16:15:17.000000 pythttp-0.0.9/setup.py
```

### Comparing `pythttp-0.0.8/PKG-INFO` & `pythttp-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.8/README.md` & `pythttp-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.8/pythttp/Log_Manager.py` & `pythttp-0.0.9/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.8/pythttp/Protocol.py` & `pythttp-0.0.9/pythttp/Protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                 Response=self.HandleTextFileRequest(result)
             elif '.png' in result:
                 Response= self.HandleFileRequest(f'{result}')
             elif '/upload_from' == result:
                 Response= self.HandleTextFileRequest('/upload_from.html')
             return Response
         except FileNotFoundError:
-            with open('resource/Hello world.html','r') as arg:
+            with open('resource/Hello world.html','r',encoding='UTF-8') as arg:
                 print(f'해당 resource{result}파일을 찾을수 없습니다.')
                 Error_Response=arg.read().format(msg=f'해당 resource{result}파일을 찾을수 없습니다.').encode('utf-8')
                 return PrepareHeader()._response_headers('404 Not Found',Error_Response) + Error_Response
 
     def ExtractPostBodySize(self, header):
         content_length_header = next((header for header in header if 'Content-Length' in header), None)
         if content_length_header:
@@ -127,15 +127,15 @@
         
     def HandleFileRequest(self,img_file='/a.png'):
         with open(f'resource{img_file}', 'rb') as ImgFile:
             Response_file=ImgFile.read()
             return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file
         
     def HandleTextFileRequest(self,flie='/Hello world.html', query='아무튼 웹 서버임'):
-        with open(f'resource{flie}','r') as TextFile:
+        with open(f'resource{flie}','r',encoding='UTF-8') as TextFile:
             Response_file=TextFile.read().format(msg=query,ImgFiles='<img src="a.png" alt="적당한사진">')
         return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file.encode('utf-8')
     
     def ImgFileUpload(self,img_file,file_name):
         #self.DB.loadDB()
         with open(f'resource/ImgFileUpload/{file_name}', 'wb') as ImgFile:
             ImgFile.write(img_file)
```

### Comparing `pythttp-0.0.8/pythttp/Structure.py` & `pythttp-0.0.9/pythttp/Structure.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.8/pythttp/Thread_Manager.py` & `pythttp-0.0.9/pythttp/Thread_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.8/pythttp.egg-info/PKG-INFO` & `pythttp-0.0.9/pythttp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.8/setup.py` & `pythttp-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.0.8",
+    version="0.0.9",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=[],
```

