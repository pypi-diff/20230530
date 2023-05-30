# Comparing `tmp/bohrium-sdk-0.0.9.tar.gz` & `tmp/bohrium-sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.0.9.tar", last modified: Fri May 19 02:01:02 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.1.0.tar", last modified: Tue May 30 07:09:32 2023, max compression
```

## Comparing `bohrium-sdk-0.0.9.tar` & `bohrium-sdk-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-19 02:01:02.775052 bohrium-sdk-0.0.9/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-19 02:01:02.774707 bohrium-sdk-0.0.9/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.0.9/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-19 02:01:02.771121 bohrium-sdk-0.0.9/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-05-19 02:01:02.000000 bohrium-sdk-0.0.9/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      319 2023-05-19 02:01:02.000000 bohrium-sdk-0.0.9/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-19 02:01:02.000000 bohrium-sdk-0.0.9/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-19 02:01:02.000000 bohrium-sdk-0.0.9/bohrium_sdk.egg-info/entry_points.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-05-19 02:01:02.000000 bohrium-sdk-0.0.9/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-19 02:01:02.774448 bohrium-sdk-0.0.9/bohriumsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.0.9/bohriumsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     3901 2023-05-19 02:00:50.000000 bohrium-sdk-0.0.9/bohriumsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:16.000000 bohrium-sdk-0.0.9/bohriumsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     3465 2023-05-19 01:48:37.000000 bohrium-sdk-0.0.9/bohriumsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1608 2023-05-19 01:47:21.000000 bohrium-sdk-0.0.9/bohriumsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-16 08:22:51.000000 bohrium-sdk-0.0.9/bohriumsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-19 02:01:02.775254 bohrium-sdk-0.0.9/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      499 2023-05-19 02:00:47.000000 bohrium-sdk-0.0.9/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:09:32.685542 bohrium-sdk-0.1.0/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      206 2023-05-30 07:09:32.685274 bohrium-sdk-0.1.0/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.1.0/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:09:32.677835 bohrium-sdk-0.1.0/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      206 2023-05-30 07:09:32.000000 bohrium-sdk-0.1.0/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      459 2023-05-30 07:09:32.000000 bohrium-sdk-0.1.0/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-05-30 07:09:32.000000 bohrium-sdk-0.1.0/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-05-30 07:09:32.000000 bohrium-sdk-0.1.0/bohrium_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-05-30 07:09:32.000000 bohrium-sdk-0.1.0/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:09:32.683641 bohrium-sdk-0.1.0/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.1.0/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.1.0/bohriumsdk/__main__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     6531 2023-05-30 01:45:26.000000 bohrium-sdk-0.1.0/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1970 2023-05-30 07:06:19.000000 bohrium-sdk-0.1.0/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     3766 2023-05-30 07:06:03.000000 bohrium-sdk-0.1.0/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.1.0/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2209 2023-05-30 07:06:47.000000 bohrium-sdk-0.1.0/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2835 2023-05-30 07:06:55.000000 bohrium-sdk-0.1.0/bohriumsdk/storage.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-05-30 07:09:32.684677 bohrium-sdk-0.1.0/bohriumsdk/test/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.1.0/bohriumsdk/test/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.1.0/bohriumsdk/test/test_node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2369 2023-05-30 01:45:00.000000 bohrium-sdk-0.1.0/bohriumsdk/test.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     3120 2023-05-30 07:07:00.000000 bohrium-sdk-0.1.0/bohriumsdk/util.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-05-30 07:09:32.685594 bohrium-sdk-0.1.0/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      502 2023-05-30 01:46:18.000000 bohrium-sdk-0.1.0/setup.py
```

### Comparing `bohrium-sdk-0.0.9/bohriumsdk/job.py` & `bohrium-sdk-0.1.0/bohriumsdk/job.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import requests
-import client
+from bohriumsdk.client import Client
 import humps
 
 class Job:
-    def __init__(self, client):
+    def __init__(
+            self, 
+            client: Client = None
+        ) -> None:
         self.client = client
 
     def list_by_page(self, job_group_id, status=None, page=1, per_page=50):
         params = {
             'groupId': job_group_id,
             'page': page,
             'pageSize': per_page
         }
         if status:
             params['status'] = status
         # print(self.client.access_key)
-        params['accessKey'] = self.client.accesskey
+        params['accessKey'] = self.client.access_key
         data = self.client.get(f'/openapi/v1/job/list', params=params)
         return data
     
 
     def list_by_number(self, job_group_id, number, status=None):
         if status is None:
             status = []
@@ -52,15 +55,15 @@
         return data
     
     def log(self, job_id):
         data = self.client.get(f'/openapi/v1/job/{job_id}/log', params=self.client.params)
         return data
 
     def insert(self, **kwargs):
-        must_fill = ['oss_path', 'project_id', 'machine_type', 'command', 'platform', 'image_address']
+        must_fill = ['oss_path', 'project_id', 'machine_type', 'command', 'platform', 'image_address', 'job_id', 'bohr_job_group_id']
         # must_fill = ['job_type', 'oss_path', 'project_id', 'scass_type', 'command', 'platform', 'image_name']
         for each in must_fill:
             if each not in kwargs:
                 raise ValueError(f'{each} is required when submitting job')
         camel_data = {humps.camelize(k): v for k, v in kwargs.items()}
         if not isinstance(camel_data['ossPath'], list):
             camel_data['ossPath'] = [camel_data['ossPath']]
@@ -83,12 +86,19 @@
             'projectId': project_id
         }
         if name:
             data['name'] = name
         if group_id:
             data['groupId'] = group_id
         try:
-            data = self.client.post(f'/openapi/v1/job/create', data=data, params=self.params)
+            data = self.client.post(f'/openapi/v1/job/create', data=data, params=self.client.params)
         except Exception as e:
             raise e
         return data
     
+    def get_job_token(self, job_id):
+        url = f"/openapi/v1/job/{job_id}/input/token"
+
+        data = self.client.get(url=url, params=self.client.params)
+        print(data)
+
+
```

### Comparing `bohrium-sdk-0.0.9/bohriumsdk/node.py` & `bohrium-sdk-0.1.0/bohriumsdk/image.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,67 @@
-import client
-class Node:
-    def __init__(self, client):
-        self.client = client
-        
-
-    def list_server(self, project_id):
-        self.params["projectId"] = project_id
-        data = self.client.get('/openapi/v1/node/list', params=self.client.params)
-        return data['items']
+from bohriumsdk.client import Client
+from bohriumsdk.util import Util
 
-    def stop(self, machine_id, creator_id):
-        data = self.client.post(f'/openapi/v1/node/stop/{machine_id}', data={"creatorId": creator_id}, params=self.client.params)
-        return data
+class Image(object):
+    def __init__(
+            self, 
+            client: Client = None
+        ) -> None:
+        self.client = client
 
-    def restart(self, machine_id):
-        data = self.client.post(f'/openapi/v1/node/restart/{machine_id}', params=self.client.params)
+    def list_image_by_page(
+            self, 
+            project_id: int = 1, 
+            kind=None, 
+            page=1, 
+            per_page=30
+        ) -> None:
+        params = {
+            'page': page, 
+            'pageSize': per_page, 
+            'projectId': project_id, 
+            "type": "private"
+        }
+        if kind is not None:
+            params['kind'] = kind
+        url = '/brm/v1/image/list'
+        host = "https://bohrium.dp.tech"
+        data = self.client.get(host=host, url=url, params=params)
+        #print(data)
         return data
-
-    def delete(self, machine_id, creator_id):
-        data = self.client.post(f'/openapi/v1/node/del/{machine_id}', data={"creatorId": creator_id}, params=self.client.params)
+    
+    def list_all_image(self, project_id, kind=None):
+        project_list = []
+        data = self.list_image_by_page(project_id=project_id, kind=kind)
+        total = data['total']
+        per_page = data['pageSize']
+        page_number = 0
+        while page_number * per_page < total:
+            page_number = page_number + 1
+            if page_number > 1:
+                data = self.list_image_by_page(project_id=project_id, kind=kind, page=page_number, per_page=30)
+            project_list.extend(data['items'])
+        return project_list
+
+
+    def delete(self, image_id):
+        host = "https://bohrium.test.dp.tech"
+        url = f'/brm/v1/image/del/{image_id}'
+        data = self.client.get(host=host, url=url)
+        
         return data
 
-    def create(self, image_id, disk_size, memory, cpu, gpu, project_id, name=None):
-        post_data = {
-            'imageId': image_id,
-            'diskSize': disk_size,
-            'projectId': project_id,
-            'memory': memory,
-            'cpu': cpu,
-            'gpu': gpu,
-            'name': name
-        }
-        data = self.client.post(f'/openapi/v1/node/add', data=post_data, params=self.client.params)
-        return data
+    def print_image(
+            self,
+            project_id: int = 0 
+        ) -> None:
+        data = self.list_all_image(project_id)
+        headers = ['imageName','createTime', "creatorName",  'diskSize', 'projectRole', 'status']
+        items = []
+        for row in data:
+            i = [row[k] for k in headers]
+            items.append(i)
+        Util().nice_print_table(headers=headers, items=items)
 
-    def to_dev_image(self, machine_id, image_name, comment=''):
-        post_data = {
-            'imageName': image_name,
-            'nodeId': machine_id,
-            'comment': comment
-        }
-        data = self.client.post(f'/openapi/v1/image/add', data=post_data, params=self.client.params)
-        return data
+    
 
+
```

