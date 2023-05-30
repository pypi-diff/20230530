# Comparing `tmp/pythttp-0.0.7.tar.gz` & `tmp/pythttp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.0.7.tar", last modified: Mon May 22 10:28:32 2023, max compression
+gzip compressed data, was "pythttp-0.0.8.tar", last modified: Tue May 30 16:11:44 2023, max compression
```

## Comparing `pythttp-0.0.7.tar` & `pythttp-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 10:28:32.386756 pythttp-0.0.7/
--rw-rw-rw-   0        0        0     1093 2023-05-22 10:28:32.385753 pythttp-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.0.7/README.md
--rw-rw-rw-   0        0        0      419 2023-05-22 10:28:29.000000 pythttp-0.0.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-22 10:28:32.374119 pythttp-0.0.7/pythttp/
--rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.0.7/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     6611 2023-05-22 10:25:00.000000 pythttp-0.0.7/pythttp/Protocol.py
--rw-rw-rw-   0        0        0     2732 2023-05-17 09:20:38.000000 pythttp-0.0.7/pythttp/Structure.py
--rw-rw-rw-   0        0        0     2997 2023-05-22 10:27:50.000000 pythttp-0.0.7/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      108 2023-05-22 10:13:49.000000 pythttp-0.0.7/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:28:32.385753 pythttp-0.0.7/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-05-22 10:28:32.000000 pythttp-0.0.7/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-22 10:28:32.000000 pythttp-0.0.7/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 10:28:32.000000 pythttp-0.0.7/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 10:28:32.000000 pythttp-0.0.7/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 10:28:32.386756 pythttp-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-05-22 10:28:19.000000 pythttp-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:11:44.978352 pythttp-0.0.8/
+-rw-rw-rw-   0        0        0     1093 2023-05-30 16:11:44.977271 pythttp-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.0.8/README.md
+-rw-rw-rw-   0        0        0      419 2023-05-30 16:11:39.000000 pythttp-0.0.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-30 16:11:44.964744 pythttp-0.0.8/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.0.8/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     6620 2023-05-30 15:45:53.000000 pythttp-0.0.8/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0     2732 2023-05-17 09:20:38.000000 pythttp-0.0.8/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     3037 2023-05-30 15:45:28.000000 pythttp-0.0.8/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      108 2023-05-22 10:13:49.000000 pythttp-0.0.8/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:11:44.977271 pythttp-0.0.8/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-05-30 16:11:44.000000 pythttp-0.0.8/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-30 16:11:44.000000 pythttp-0.0.8/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 16:11:44.000000 pythttp-0.0.8/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 16:11:44.000000 pythttp-0.0.8/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 16:11:44.978352 pythttp-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-05-30 16:11:33.000000 pythttp-0.0.8/setup.py
```

### Comparing `pythttp-0.0.7/PKG-INFO` & `pythttp-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.7/README.md` & `pythttp-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.7/pythttp/Log_Manager.py` & `pythttp-0.0.8/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.7/pythttp/Protocol.py` & `pythttp-0.0.8/pythttp/Protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             self.s.close()
 
     def start_web_server(self):
         self.bind_address()
         self.listen()
         while True:
             user_info=self.accept_connection()
-            self.Thread.Create_Thread(target=self.handle_request_thread,args=user_info)[1].start()
+            self.Thread.ThreadConstructor(target=self.handle_request_thread,args=user_info)[1].start()
     
     def handle_request_thread(self, client_socket, client_address):
         socket_and_address = [(client_socket,), client_address]
         thread_name, thread = self.assign_user_thread(socket_and_address)
         thread.start()
         thread.join()
         first_line = thread.result[0]
@@ -45,15 +45,15 @@
             file_name=thread.result[1][1].split('"')[3]
             self.ImgFileUpload(thread.result[2],f'{file_name}')
             query=self.HandleFileRequest(self.DB.ServerDB['Img'][file_name])
         else:
             return 'This communication is not HTTP protocol'
         self.send_response(query, socket_and_address)
         self.Thread.find_stopped_thread()
-        self.Thread.clearSessionInfo(thread_name, client_address)
+        self.Thread.SessionDestructor(thread_name, client_address)
 
     def bind_address(self, address='0.0.0.0', port=80):
         external_ip = request.urlopen('https://ident.me').read().decode('utf8')  
         self.s.bind((address, port))
         self.log(f"[Server started on] ==> \033[96m{external_ip}:{port}\033[0m")
 
     def listen(self, limit=0):
@@ -78,15 +78,15 @@
             for count in range(int(self.ExtractPostBodySize(header_list)/2048)):
                 post_body+=socket[0].recv(2048)
             return 'POST',post_header,post_body
         self.log(msg=f'[{parse.unquote(header_list[0])} request from] ==> \033[33m{addres}\033[0m')
         return 'GET',header_list
 
     def assign_user_thread(self,socket_and_addres):
-        thread_name,thread = self.Thread.Create_Thread(target=self.receive,args=socket_and_addres)
+        thread_name,thread = self.Thread.ThreadConstructor(target=self.receive,args=socket_and_addres)
         self.Thread.USERS.append(socket_and_addres[1])
         self.Thread.USERS_COUNT+=1
         self.Thread.SESSIONS[thread_name]=socket_and_addres[1]
         self.Thread.user_socket_dict[socket_and_addres[1]]=socket_and_addres[0]
         return thread_name,thread
 
     def send_response(self,query,socket_and_addres):
```

### Comparing `pythttp-0.0.7/pythttp/Structure.py` & `pythttp-0.0.8/pythttp/Structure.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.7/pythttp/Thread_Manager.py` & `pythttp-0.0.8/pythttp/Thread_Manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 class Thread:
     def __init__(self):
         self.ACTIVATED_THREADS={}
         self.USERS=Thread_DataManager().USERS
         self.SESSIONS=Thread_DataManager().SESSIONS
         self.USERS_COUNT=Thread_DataManager().USERS_COUNT
+        self.user_socket_dict=Thread_DataManager().user_socket_dict
         self.THREADS_COUNT=0
-        self.user_socket_dict={}
         self.stopped_threads={}
         self.finished_users=[]
         self.log=Log().logging
 
     def display_variables(self):
         LIST_VARIABLES=f'''
                             'SESSIONS':{self.SESSIONS},
@@ -42,28 +42,28 @@
                             'user_thread_result_dict':{self.user_thread_result_dict}
                             'user_socket_dict':{self.user_socket_dict}
                             'stopped_threads':{self.stopped_threads}
                             'finished_users':{self.finished_users}
                         '''
         print(LIST_VARIABLES)
 
-    def Create_Thread(self, target, args=(), daemon=False):
+    def ThreadConstructor(self, target, args=(), daemon=False):
         thread_mutex=0
         while True:
             new_thread_name='THREAD_{}_{}'.format(target.__name__,thread_mutex)
             self.THREADS_COUNT+=1
             if new_thread_name not in self.ACTIVATED_THREADS.keys():
                 globals()[new_thread_name] = THREAD_PRESET(target=target,args=args,daemon=daemon)
                 new_thread=globals()[new_thread_name]
                 self.ACTIVATED_THREADS[new_thread_name]=new_thread
                 return new_thread_name,new_thread
             else:
                 thread_mutex+=1
 
-    def clearSessionInfo(self,thread_name,user):
+    def SessionDestructor(self,thread_name,user):
         thread=eval(thread_name)
         if (thread.is_alive()==False):
             del self.user_socket_dict[user]
             del self.finished_users[self.finished_users.index(user)]
             del self.USERS[self.USERS.index(user)]
             del self.SESSIONS[thread_name]
             self.USERS_COUNT-=1
```

### Comparing `pythttp-0.0.7/pythttp.egg-info/PKG-INFO` & `pythttp-0.0.8/pythttp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.7/setup.py` & `pythttp-0.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.0.7",
+    version="0.0.8",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=[],
```

