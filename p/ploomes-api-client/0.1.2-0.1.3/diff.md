# Comparing `tmp/ploomes-api-client-0.1.2.tar.gz` & `tmp/ploomes-api-client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomes-api-client-0.1.2.tar", last modified: Fri May 26 18:49:42 2023, max compression
+gzip compressed data, was "ploomes-api-client-0.1.3.tar", last modified: Tue May 30 15:36:34 2023, max compression
```

## Comparing `ploomes-api-client-0.1.2.tar` & `ploomes-api-client-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-26 18:49:42.584521 ploomes-api-client-0.1.2/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.2/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-26 18:49:42.584363 ploomes-api-client-0.1.2/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     1137 2023-05-26 14:13:51.000000 ploomes-api-client-0.1.2/README.md
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-26 18:49:42.583297 ploomes-api-client-0.1.2/ploomes_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-26 18:49:42.000000 ploomes-api-client-0.1.2/ploomes_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-05-26 18:49:42.000000 ploomes-api-client-0.1.2/ploomes_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-05-26 18:49:42.000000 ploomes-api-client-0.1.2/ploomes_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-05-26 18:49:42.000000 ploomes-api-client-0.1.2/ploomes_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-05-26 18:49:42.000000 ploomes-api-client-0.1.2/ploomes_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-26 18:49:42.583691 ploomes-api-client-0.1.2/ploomes_client/
--rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-26 18:47:42.000000 ploomes-api-client-0.1.2/ploomes_client/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)    22820 2023-05-26 18:41:36.000000 ploomes-api-client-0.1.2/ploomes_client/ploomes_client.py
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-05-26 18:49:42.584576 ploomes-api-client-0.1.2/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-05-26 18:48:32.000000 ploomes-api-client-0.1.2/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-30 15:36:34.776379 ploomes-api-client-0.1.3/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.3/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-30 15:36:34.776217 ploomes-api-client-0.1.3/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1137 2023-05-26 14:13:51.000000 ploomes-api-client-0.1.3/README.md
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-30 15:36:34.775336 ploomes-api-client-0.1.3/ploomes_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-30 15:36:34.000000 ploomes-api-client-0.1.3/ploomes_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-05-30 15:36:34.000000 ploomes-api-client-0.1.3/ploomes_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-05-30 15:36:34.000000 ploomes-api-client-0.1.3/ploomes_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-05-30 15:36:34.000000 ploomes-api-client-0.1.3/ploomes_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-05-30 15:36:34.000000 ploomes-api-client-0.1.3/ploomes_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-30 15:36:34.775660 ploomes-api-client-0.1.3/ploomes_client/
+-rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-26 18:47:42.000000 ploomes-api-client-0.1.3/ploomes_client/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)    22837 2023-05-30 15:35:09.000000 ploomes-api-client-0.1.3/ploomes_client/ploomes_client.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-05-30 15:36:34.776435 ploomes-api-client-0.1.3/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-05-30 15:36:33.000000 ploomes-api-client-0.1.3/setup.py
```

### Comparing `ploomes-api-client-0.1.2/LICENSE` & `ploomes-api-client-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.1.2/PKG-INFO` & `ploomes-api-client-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # Ploomes API Python Client
```

### Comparing `ploomes-api-client-0.1.2/README.md` & `ploomes-api-client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.1.2/ploomes_api_client.egg-info/PKG-INFO` & `ploomes-api-client-0.1.3/ploomes_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # Ploomes API Python Client
```

### Comparing `ploomes-api-client-0.1.2/ploomes_client/ploomes_client.py` & `ploomes-api-client-0.1.3/ploomes_client/ploomes_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         return None
 
     @retry
     @sleep_and_retry
     @limits(calls=MAX_REQUESTS_PER_SECOND, period=1)
     def get_contacts(self, filter):
         response = []
-        url = f"{self.host}/Contacts?$top=300&$orderby=Id+desc,CNPJ&$expand=Phones&$filter={filter}"
+        url = f"{self.host}/Contacts?$top=300&$orderby=Id+desc,CNPJ&$expand=OtherProperties,Phones&$filter={filter}"
         while url:
             r = requests.get(url, headers=self.headers)
             data = r.json()
             if data.get('value'):
                 response += data["value"]
             url = data.get("@odata.nextLink")
         return response
@@ -620,14 +620,15 @@
         r = requests.post(
             f"{self.host}/InteractionRecords", data=payload, headers=self.headers
         )
         response = r.json()
         return response
 
 
+
 def get_file_url(url):
     filename = url.split("/")[-1]  # get the filename from the URL
     if "." not in filename:  # if there's no extension
         return url  # return the original URL
     else:
         # return the URL up to the query string, if present
         return url.split("?")[0]
```

### Comparing `ploomes-api-client-0.1.2/setup.py` & `ploomes-api-client-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ploomes-api-client',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),   
     url='https://github.com/victorfigueredo/ploomes-api-client',
     author='Victor Figueredo',
     author_email='cto@filterfeed.com.br',
     description='Python client for the Ploomes API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

