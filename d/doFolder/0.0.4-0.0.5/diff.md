# Comparing `tmp/doFolder-0.0.4.tar.gz` & `tmp/doFolder-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doFolder-0.0.4.tar", last modified: Sun May 28 09:02:09 2023, max compression
+gzip compressed data, was "doFolder-0.0.5.tar", last modified: Tue May 30 18:05:58 2023, max compression
```

## Comparing `doFolder-0.0.4.tar` & `doFolder-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 09:02:09.217024 doFolder-0.0.4/
--rw-rw-rw-   0        0        0     3260 2023-05-28 09:02:09.217024 doFolder-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2535 2023-05-28 08:47:54.000000 doFolder-0.0.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-28 09:02:09.151024 doFolder-0.0.4/doFolder/
--rw-rw-rw-   0        0        0      569 2023-05-26 13:44:53.000000 doFolder-0.0.4/doFolder/__init__.py
--rw-rw-rw-   0        0        0    10825 2023-05-28 09:01:39.000000 doFolder-0.0.4/doFolder/compare.py
--rw-rw-rw-   0        0        0    19027 2023-05-28 08:57:56.000000 doFolder-0.0.4/doFolder/main.py
--rw-rw-rw-   0        0        0    13319 2023-05-28 09:02:05.000000 doFolder-0.0.4/doFolder/terminal.py
-drwxrwxrwx   0        0        0        0 2023-05-28 09:02:09.214024 doFolder-0.0.4/doFolder.egg-info/
--rw-rw-rw-   0        0        0     3260 2023-05-28 09:02:09.000000 doFolder-0.0.4/doFolder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-28 09:02:09.000000 doFolder-0.0.4/doFolder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 09:02:09.000000 doFolder-0.0.4/doFolder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-28 09:02:09.000000 doFolder-0.0.4/doFolder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-05-28 09:02:09.000000 doFolder-0.0.4/doFolder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 09:02:09.000000 doFolder-0.0.4/doFolder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 09:02:09.218025 doFolder-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1196 2023-05-28 08:38:02.000000 doFolder-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:05:58.527872 doFolder-0.0.5/
+-rw-rw-rw-   0        0        0     3349 2023-05-30 18:05:58.527872 doFolder-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2624 2023-05-30 18:05:13.000000 doFolder-0.0.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 18:05:58.516871 doFolder-0.0.5/doFolder/
+-rw-rw-rw-   0        0        0      569 2023-05-26 13:44:53.000000 doFolder-0.0.5/doFolder/__init__.py
+-rw-rw-rw-   0        0        0    10825 2023-05-28 09:01:39.000000 doFolder-0.0.5/doFolder/compare.py
+-rw-rw-rw-   0        0        0    19828 2023-05-30 17:53:26.000000 doFolder-0.0.5/doFolder/main.py
+-rw-rw-rw-   0        0        0    13825 2023-05-28 09:04:58.000000 doFolder-0.0.5/doFolder/terminal.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:05:58.525872 doFolder-0.0.5/doFolder.egg-info/
+-rw-rw-rw-   0        0        0     3349 2023-05-30 18:05:58.000000 doFolder-0.0.5/doFolder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-30 18:05:58.000000 doFolder-0.0.5/doFolder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 18:05:58.000000 doFolder-0.0.5/doFolder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-30 18:05:58.000000 doFolder-0.0.5/doFolder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-05-30 18:05:58.000000 doFolder-0.0.5/doFolder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 18:05:58.000000 doFolder-0.0.5/doFolder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 18:05:58.528872 doFolder-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-05-30 18:05:25.000000 doFolder-0.0.5/setup.py
```

### Comparing `doFolder-0.0.4/PKG-INFO` & `doFolder-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.4
+Version: 0.0.5
 Summary: download files quickly
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
@@ -49,14 +49,16 @@
    -  *方法* ``hasFolder,hasFile`` 是否包括某个文件/文件夹,参数为
       ``str``\ 时默认匹配 ``.name``\ 属性
    -  *方法* ``remove,copy,move`` 文件夹操作
    -  *方法* ``search`` 搜索文件夹的内容
 
       -  *参数* ``condition`` 搜索条件:``List[UnformattedMatching]``
       -  *参数* ``aim`` 目标: ``"file"|"folder"|"both"``
+      -  *参数* ``threaded`` 是否线程化 ``bool``
+      -  *参数* ``threaded`` 最大线程数:``int``
       -  *返回* 搜索结果:``SearchResult``
 
 -  ``File`` 指一个文件
 
    -  *参数* ``path`` 文件路径:``str|doFolder.Path``
    -  *方法* ``remove,copy,move`` 文件操作
    -  *属性* ``mode,ino,dev,uid,gid...`` 参见 ``os.stat``
@@ -81,15 +83,15 @@
       -  *返回* 比较结果:``CompareResult``
 
 命令行使用
 ~~~~~~~~~~
 
 .. code:: bash
 
-   compare Folder1 Folder2 [-c ignore|hash|content|size] [-t [-n num]]
+   compare Folder1 Folder2 [-c ] [-t [-n num]]
 
 具体作用参见
 
 .. code:: bash
 
    compare -h
```

### Comparing `doFolder-0.0.4/README.rst` & `doFolder-0.0.5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,16 @@
    -  *方法* ``hasFolder,hasFile`` 是否包括某个文件/文件夹,参数为
       ``str``\ 时默认匹配 ``.name``\ 属性
    -  *方法* ``remove,copy,move`` 文件夹操作
    -  *方法* ``search`` 搜索文件夹的内容
 
       -  *参数* ``condition`` 搜索条件:``List[UnformattedMatching]``
       -  *参数* ``aim`` 目标: ``"file"|"folder"|"both"``
+      -  *参数* ``threaded`` 是否线程化 ``bool``
+      -  *参数* ``threaded`` 最大线程数:``int``
       -  *返回* 搜索结果:``SearchResult``
 
 -  ``File`` 指一个文件
 
    -  *参数* ``path`` 文件路径:``str|doFolder.Path``
    -  *方法* ``remove,copy,move`` 文件操作
    -  *属性* ``mode,ino,dev,uid,gid...`` 参见 ``os.stat``
@@ -60,15 +62,15 @@
       -  *返回* 比较结果:``CompareResult``
 
 命令行使用
 ~~~~~~~~~~
 
 .. code:: bash
 
-   compare Folder1 Folder2 [-c ignore|hash|content|size] [-t [-n num]]
+   compare Folder1 Folder2 [-c ] [-t [-n num]]
 
 具体作用参见
 
 .. code:: bash
 
    compare -h
```

### Comparing `doFolder-0.0.4/doFolder/__init__.py` & `doFolder-0.0.5/doFolder/__init__.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.4/doFolder/compare.py` & `doFolder-0.0.5/doFolder/compare.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.4/doFolder/main.py` & `doFolder-0.0.5/doFolder/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 import re
 from typing import Any,Union,Callable,Literal,List,Tuple,Iterable,TypeVar,Generic,Protocol
 import shutil
 import copy
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler,FileSystemEvent,FileSystemMovedEvent,EVENT_TYPE_CREATED,EVENT_TYPE_DELETED,EVENT_TYPE_MOVED,EVENT_TYPE_MODIFIED
 import hashlib
+import logging
+from concurrent.futures import ThreadPoolExecutor
 
 __all__=["File","Folder","Path"]
 
 pathTester=re.compile(r"^(?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+)/(?:[^/\\\*\?]+/?)*$")
 driverFinder=re.compile(r"^((?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+))/(?:[^/\\\*\?]+/?)*$")
 pathFinder=re.compile(r"^(?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+)(/(?:[^/\\\*\?]+/?)*)$")
 SearchCondition=Union[str,re.Pattern[str],Callable[[Union["File","Folder"]],bool]]
@@ -260,22 +262,24 @@
         if type(path)!=Path:
             path=Path(path)
         self.onlisten=onlisten
         self.path=path
         self.parent=parent
         self.scaned=scan
         self.scan=scan
+        self.logger=logging.getLogger(self.name)
         if self.onlisten:
             self.event_handler = _FolderUpdateHeader(self)
             self.observer = Observer()
             self.observer.schedule(self.event_handler, path=path, recursive=True)
             self.observer.start()
         if scan:
             self.refresh()
     def refresh(self):
+        self.logger.debug("refresh folder contents")
         """Rebuild all of this folder object"""
         self.scaned=True
         self.dir:List[str]=os.listdir(self.path)
         self.files:FileList = FileList([])
         self.subfolder:FolderList=FolderList([])
         for i in self.dir:
             newPath=self.path.add(i)
@@ -313,14 +317,15 @@
         if len(path)>1:
             nextFolder=self[path[0]]
             if type(nextFolder)==Folder:
                 nextFolder._update(path[1:],eventType,eventTarget,isDirectory)
                 return
             else:
                 raise FolderOrFileNotFoundError(f"Directory \"{self.path}\" does not contain folder \"{path[0]}\"")
+        self.logger.debug(f"file content update.{eventType}")
         name=path[0]
         if eventType==EVENT_TYPE_CREATED:
             if isDirectory:self.subfolder.append(Folder(eventTarget,parent=self))
             else:self.files.append(File(eventTarget,parent=self))
         if eventType==EVENT_TYPE_DELETED:
             target=self[name]
             if type(target)==Folder:self.subfolder.remove(target)
@@ -372,18 +377,21 @@
         if  rootPosition=="first":
             callback(self)
         for item in self.subfolder:
             item.forEachFolder(callback,rootPosition)
         if rootPosition=="last":
             callback(self)
     def remove(self)->None:
+        self.logger.info("Removing folder")
         shutil.rmtree(self.path)
     def move(self,path:str)->None:
+        self.logger.info(f"Moving folder to {path}")
         shutil.move(self.path,path)
     def copy(self,path:str)->None:
+        self.logger.info(f"Copying folder to {path}")
         shutil.copytree(self.path, path)
     def hasSubfolder(self,name:str)->bool:
         """
         Whether to include a subfolder
         :param name:folder name
         """
         for i in self.subfolder:
@@ -395,32 +403,36 @@
         Whether to include a file
         :param name:file name
         """
         for i in self.files:
             if i.name==name:
                 return True
         return False
-    def search(self,condition:List[UnformattedMatching],aim:Literal["file","folder","both"]="both")->SearchResult:
+    def search(self,condition:List[UnformattedMatching],aim:Literal["file","folder","both"]="both",threaded:bool=False,threads:Union[None,int]=None)->SearchResult:
         """
         Search item in the Folder
         :param condition: search conditions which is unformatted
         str: match the files whose name == condition\n
         re.Pattern[str]: match the files whose name matches the regular expression\n
         Callable[[Union["File","Folder"]],bool]: Returns a match based on the folder or file object\n
         Tuple[str | re.Pattern[str]| Callable ,int,int|None] the condition , the Minimum repetition , Maximum repetition("None" indicates that there is no limit)
         :param aim: search type
         """
-        return self.match([_formatMatching(i) for i in condition],aim=aim)
-    def match(self,condition:List[FormatedMatching],aim:Literal["file","folder","both"]="both")->SearchResult:
+        self.logger.debug(f"Searching objects in folder.{condition}")
+        threadPool=ThreadPoolExecutor(max_workers=threads) if threaded else None
+        retsult:SearchResult=SearchResult()
+        self._match([_formatMatching(i) for i in condition],retsult,aim=aim,pool=threadPool)
+        if threadPool:threadPool.shutdown(wait=True)
+        return retsult
+    def _match(self,condition:List[FormatedMatching],retsult:SearchResult,aim:Literal["file","folder","both"]="both",pool:Union[ThreadPoolExecutor,None]=None)->None:
         """
         This is the ultimate implementation of the search behavior, but if your criteria are not formatted, consider starting with the "search" function, which will format the criteria and complete the search for you
         :param condition: search conditions which is formatted
         :param aim: search type
         """
-        retsult:SearchResult=SearchResult()
         for i in range(len(condition)):
             if aim!="folder":
                 for j in self.files:
                     if not condition[i][0](j):continue
                     restCondition=copy.deepcopy(condition)
                     restCondition[0]=(restCondition[0][0],max(restCondition[0][1]-1,0),None if restCondition[0][2]==None else max(restCondition[0][2]-1,0))
                     k=i
@@ -431,19 +443,19 @@
                     if (k==len(restCondition)):
                         retsult.append(j)
             for j in self.subfolder:
                 if not condition[i][0](j):continue
                 restCondition=copy.deepcopy(condition)
                 restCondition[0]=(restCondition[0][0],max(restCondition[0][1]-1,0),None if restCondition[0][2]==None else max(restCondition[0][2]-1,0))
                 if restCondition[0][2]!=None and restCondition[0][2]<=0:del restCondition[0]
-                retsult+=j.match(restCondition,aim=aim)
+                if pool:pool.submit(j._match,restCondition,retsult,aim,pool)
+                else:j._match(restCondition,retsult,aim,pool)
                 if aim=="file":continue
                 k=i
                 while k<len(restCondition):
                     if restCondition[k][1]!=0:
                         break
                     k+=1
                 if (k==len(restCondition)):
                     retsult.append(j)
             if condition[i][1]>0:
-                break
-        return retsult
+                break
```

### Comparing `doFolder-0.0.4/doFolder/terminal.py` & `doFolder-0.0.5/doFolder/terminal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+"""
+Copyright (c) 2023 Gou Haoming
+doFolder is licensed under Mulan PSL v2.
+You can use this software according to the terms and conditions of the Mulan PSL v2.
+You may obtain a copy of Mulan PSL v2 at:
+         http://license.coscl.org.cn/MulanPSL2
+THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND,
+EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
+MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
+See the Mulan PSL v2 for more details.
+"""
 import doFolder
 import doFolder.compare as comp
 from rich.console import Console
 from rich.table import Table,Column
 from rich.style import Style
 import datetime
 import sys
```

### Comparing `doFolder-0.0.4/doFolder.egg-info/PKG-INFO` & `doFolder-0.0.5/doFolder.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.4
+Version: 0.0.5
 Summary: download files quickly
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
@@ -49,14 +49,16 @@
    -  *方法* ``hasFolder,hasFile`` 是否包括某个文件/文件夹,参数为
       ``str``\ 时默认匹配 ``.name``\ 属性
    -  *方法* ``remove,copy,move`` 文件夹操作
    -  *方法* ``search`` 搜索文件夹的内容
 
       -  *参数* ``condition`` 搜索条件:``List[UnformattedMatching]``
       -  *参数* ``aim`` 目标: ``"file"|"folder"|"both"``
+      -  *参数* ``threaded`` 是否线程化 ``bool``
+      -  *参数* ``threaded`` 最大线程数:``int``
       -  *返回* 搜索结果:``SearchResult``
 
 -  ``File`` 指一个文件
 
    -  *参数* ``path`` 文件路径:``str|doFolder.Path``
    -  *方法* ``remove,copy,move`` 文件操作
    -  *属性* ``mode,ino,dev,uid,gid...`` 参见 ``os.stat``
@@ -81,15 +83,15 @@
       -  *返回* 比较结果:``CompareResult``
 
 命令行使用
 ~~~~~~~~~~
 
 .. code:: bash
 
-   compare Folder1 Folder2 [-c ignore|hash|content|size] [-t [-n num]]
+   compare Folder1 Folder2 [-c ] [-t [-n num]]
 
 具体作用参见
 
 .. code:: bash
 
    compare -h
```

### Comparing `doFolder-0.0.4/setup.py` & `doFolder-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 setup(
     name = 'doFolder',
-    version = '0.0.4',
+    version = '0.0.5',
     keywords = ['file',"foler","path","filesystem"],
     description = 'download files quickly',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/do-folder/",
     install_requires = [
```

