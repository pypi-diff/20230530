# Comparing `tmp/jms-storage-0.0.46.tar.gz` & `tmp/jms-storage-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jms-storage-0.0.46.tar", last modified: Tue May 30 07:04:30 2023, max compression
+gzip compressed data, was "dist/jms-storage-0.0.9.tar", last modified: Thu Mar  8 16:18:39 2018, max compression
```

## Comparing `jms-storage-0.0.46.tar` & `jms-storage-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,17 @@
-drwxr-xr-x   0 bryan      (501) staff       (20)        0 2023-05-30 07:04:30.814204 jms-storage-0.0.46/
--rw-r--r--   0 bryan      (501) staff       (20)      653 2023-05-30 07:04:30.814097 jms-storage-0.0.46/PKG-INFO
--rw-r--r--   0 bryan      (501) staff       (20)       25 2023-02-17 09:38:33.000000 jms-storage-0.0.46/README.md
-drwxr-xr-x   0 bryan      (501) staff       (20)        0 2023-05-30 07:04:30.813296 jms-storage-0.0.46/jms_storage/
--rw-r--r--   0 bryan      (501) staff       (20)     1331 2023-05-30 07:02:49.000000 jms-storage-0.0.46/jms_storage/__init__.py
--rw-r--r--   0 bryan      (501) staff       (20)     1721 2023-02-17 09:38:33.000000 jms-storage-0.0.46/jms_storage/azure.py
--rw-r--r--   0 bryan      (501) staff       (20)     1134 2023-02-17 10:04:03.000000 jms-storage-0.0.46/jms_storage/base.py
--rw-r--r--   0 bryan      (501) staff       (20)     1936 2023-02-17 09:38:33.000000 jms-storage-0.0.46/jms_storage/ceph.py
--rw-r--r--   0 bryan      (501) staff       (20)     5372 2023-02-17 10:04:03.000000 jms-storage-0.0.46/jms_storage/es.py
--rw-r--r--   0 bryan      (501) staff       (20)     3494 2023-02-17 09:38:33.000000 jms-storage-0.0.46/jms_storage/ftp.py
--rw-r--r--   0 bryan      (501) staff       (20)     1375 2023-02-17 10:04:03.000000 jms-storage-0.0.46/jms_storage/jms.py
--rw-r--r--   0 bryan      (501) staff       (20)     1705 2023-02-17 09:38:33.000000 jms-storage-0.0.46/jms_storage/multi.py
--rw-r--r--   0 bryan      (501) staff       (20)     2385 2023-02-17 09:38:33.000000 jms-storage-0.0.46/jms_storage/obs.py
--rw-r--r--   0 bryan      (501) staff       (20)     1621 2023-02-17 09:38:33.000000 jms-storage-0.0.46/jms_storage/oss.py
--rw-r--r--   0 bryan      (501) staff       (20)     2235 2023-02-17 09:38:33.000000 jms-storage-0.0.46/jms_storage/s3.py
--rw-r--r--   0 bryan      (501) staff       (20)     1725 2023-02-17 09:38:33.000000 jms-storage-0.0.46/jms_storage/storage_test.py
-drwxr-xr-x   0 bryan      (501) staff       (20)        0 2023-05-30 07:04:30.813911 jms-storage-0.0.46/jms_storage.egg-info/
--rw-r--r--   0 bryan      (501) staff       (20)      653 2023-05-30 07:04:30.000000 jms-storage-0.0.46/jms_storage.egg-info/PKG-INFO
--rw-r--r--   0 bryan      (501) staff       (20)      455 2023-05-30 07:04:30.000000 jms-storage-0.0.46/jms_storage.egg-info/SOURCES.txt
--rw-r--r--   0 bryan      (501) staff       (20)        1 2023-05-30 07:04:30.000000 jms-storage-0.0.46/jms_storage.egg-info/dependency_links.txt
--rw-r--r--   0 bryan      (501) staff       (20)      301 2023-05-30 07:04:30.000000 jms-storage-0.0.46/jms_storage.egg-info/requires.txt
--rw-r--r--   0 bryan      (501) staff       (20)       12 2023-05-30 07:04:30.000000 jms-storage-0.0.46/jms_storage.egg-info/top_level.txt
--rw-r--r--   0 bryan      (501) staff       (20)      301 2023-05-30 07:02:42.000000 jms-storage-0.0.46/requirements.txt
--rw-r--r--   0 bryan      (501) staff       (20)       38 2023-05-30 07:04:30.814244 jms-storage-0.0.46/setup.cfg
--rw-r--r--   0 bryan      (501) staff       (20)     1462 2023-02-17 09:38:33.000000 jms-storage-0.0.46/setup.py
+drwxr-xr-x   0 liuzheng   (501) staff       (20)        0 2018-03-08 16:18:39.000000 jms-storage-0.0.9/
+-rw-r--r--   0 liuzheng   (501) staff       (20)      354 2018-03-08 16:18:39.000000 jms-storage-0.0.9/PKG-INFO
+drwxr-xr-x   0 liuzheng   (501) staff       (20)        0 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage.egg-info/
+-rw-r--r--   0 liuzheng   (501) staff       (20)      354 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage.egg-info/PKG-INFO
+-rw-r--r--   0 liuzheng   (501) staff       (20)      302 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 liuzheng   (501) staff       (20)      213 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage.egg-info/requires.txt
+-rw-r--r--   0 liuzheng   (501) staff       (20)       12 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage.egg-info/top_level.txt
+-rw-r--r--   0 liuzheng   (501) staff       (20)        1 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 liuzheng   (501) staff       (20)       25 2018-03-08 10:08:10.000000 jms-storage-0.0.9/README.md
+-rw-r--r--   0 liuzheng   (501) staff       (20)     1111 2018-03-08 14:51:32.000000 jms-storage-0.0.9/setup.py
+-rw-r--r--   0 liuzheng   (501) staff       (20)       38 2018-03-08 16:18:39.000000 jms-storage-0.0.9/setup.cfg
+drwxr-xr-x   0 liuzheng   (501) staff       (20)        0 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage/
+-rw-r--r--   0 liuzheng   (501) staff       (20)     4078 2018-01-23 10:44:05.000000 jms-storage-0.0.9/jms_storage/elasticsearch.py
+-rw-r--r--   0 liuzheng   (501) staff       (20)     1172 2018-03-08 16:05:21.000000 jms-storage-0.0.9/jms_storage/ali.py
+-rw-r--r--   0 liuzheng   (501) staff       (20)      372 2018-03-08 16:18:23.000000 jms-storage-0.0.9/jms_storage/__init__.py
+-rw-r--r--   0 liuzheng   (501) staff       (20)     1674 2018-03-08 16:05:21.000000 jms-storage-0.0.9/jms_storage/aws.py
+-rw-r--r--   0 liuzheng   (501) staff       (20)      636 2018-03-08 16:05:21.000000 jms-storage-0.0.9/jms_storage/jms.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `jms-storage-0.0.46/jms_storage/ceph.py` & `jms-storage-0.0.9/jms_storage/aws.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,52 @@
 # -*- coding: utf-8 -*-
 #
+import boto3
 
-import os
-import boto
-import boto.s3.connection
-
-from .base import ObjectStorage
-
-
-class CEPHStorage(ObjectStorage):
 
+class aws:
     def __init__(self, config):
-        self.bucket = config.get("BUCKET", None)
-        self.region = config.get("REGION", None)
-        self.access_key = config.get("ACCESS_KEY", None)
-        self.secret_key = config.get("SECRET_KEY", None)
-        self.hostname = config.get("HOSTNAME", None)
-        self.port = config.get("PORT", 7480)
-
-        if self.hostname and self.access_key and self.secret_key:
-            self.conn = boto.connect_s3(
-                aws_access_key_id=self.access_key,
-                aws_secret_access_key=self.secret_key,
-                host=self.hostname,
-                port=self.port,
-                is_secure=False,
-                calling_format=boto.s3.connection.OrdinaryCallingFormat(),
-            )
+        self.BUCKET = config.get("BUCKET", "jumpserver")
+        self.REGION = config.get("REGION", None)
+        self.ACCESS_KEY = config.get("ACCESS_KEY", None)
+        self.SECRET_KEY = config.get("SECRET_KEY", None)
+        if self.ACCESS_KEY and self.REGION and self.SECRET_KEY:
+            self.client = boto3.client('s3',
+                                        region_name=self.REGION,
+                                        aws_access_key_id=self.ACCESS_KEY,
+                                        aws_secret_access_key=self.SECRET_KEY)
+        else:
+            self.client = boto3.client('s3')
 
-        try:
-            self.client = self.conn.get_bucket(bucket_name=self.bucket)
-        except Exception:
-            self.client = None
+    def type(self):
+        return 's3'
 
-    def upload(self, src, target):
+    def upload_file(self, filepath, remote_path):
         try:
-            key = self.client.new_key(target)
-            key.set_contents_from_filename(src)
-            return True, None
-        except Exception as e:
-            return False, e
+            self.client.upload_file(filepath, self.BUCKET, remote_path)
+            return True
+        except:
+            return False
 
-    def download(self, src, target):
+    def check_file(self, remote_path):
         try:
-            os.makedirs(os.path.dirname(target), 0o755, exist_ok=True)
-            key = self.client.get_key(src)
-            key.get_contents_to_filename(target)
-            return True, None
-        except Exception as e:
-            return False, e
+            self.client.head_object(Bucket=self.BUCKET, Key=remote_path)
+            return True
+        except:
+            return False
 
-    def delete(self, path):
+    def download_file(self, remote_path, locale_path):
         try:
-            self.client.delete_key(path)
-            return True, None
-        except Exception as e:
-            return False, e
+            self.client.download_file(self.BUCKET, remote_path, locale_path)
+            return True
+        except:
+            return False
 
-    def exists(self, path):
+    def generate_presigned_url(self, path, expire=3600):
         try:
-            return self.client.get_key(path)
-        except Exception:
+            return self.client.generate_presigned_url(
+                ClientMethod='get_object',
+                Params={'Bucket': self.BUCKET, 'Key': path},
+                ExpiresIn=expire,
+                HttpMethod='GET')
+        except:
             return False
-
-    @property
-    def type(self):
-        return 'ceph'
```

### Comparing `jms-storage-0.0.46/jms_storage/jms.py` & `jms-storage-0.0.9/jms_storage/ali.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,39 @@
 # -*- coding: utf-8 -*-
 #
-import os
-from .base import ObjectStorage, LogStorage
+import oss2
 
 
-class JMSReplayStorage(ObjectStorage):
+class ali:
     def __init__(self, config):
-        self.client = config.get("SERVICE")
+        self.ENDPOINT = config.get("ENDPOINT", None)
+        self.BUCKET = config.get("BUCKET", None)
+        self.ACCESS_KEY = config.get("ACCESS_KEY", None)
+        self.SECRET_KEY = config.get("SECRET_KEY", None)
+        if self.ACCESS_KEY and self.SECRET_KEY:
+            self.auth = oss2.Auth(self.ACCESS_KEY, self.SECRET_KEY)
+        else:
+            self.auth = None
+        if self.auth and self.ENDPOINT and self.BUCKET:
+            self.client = oss2.Bucket(self.auth, self.ENDPOINT, self.BUCKET)
+        else:
+            self.client = None
 
-    def upload(self, src, target):
-        session_id = os.path.basename(target).split('.')[0]
-        ok = self.client.push_session_replay(src, session_id)
-        return ok, None
-
-    def delete(self, path):
-        return False, Exception("Not support not")
-
-    def exists(self, path):
-        return False
-
-    def download(self, src, target):
-        return False, Exception("Not support not")
-
-    @property
     def type(self):
-        return 'jms'
-
+        return 'oss'
 
-class JMSCommandStorage(LogStorage):
-    def __init__(self, config):
-        self.client = config.get("SERVICE")
-        if not self.client:
-            raise Exception("Not found app service")
-
-    def save(self, command):
-        return self.client.push_session_command([command])
-
-    def bulk_save(self, command_set, raise_on_error=True):
-        return self.client.push_session_command(command_set)
-
-    def filter(self, date_from=None, date_to=None,
-               user=None, asset=None, account=None,
-               input=None, session=None):
-        pass
-
-    def count(self, date_from=None, date_to=None,
-              user=None, asset=None, account=None,
-              input=None, session=None):
-        pass
+    def upload_file(self, filepath, remote_path):
+        try:
+            self.client.put_object_from_file(remote_path, filepath)
+            return True
+        except:
+            return False
+
+    def check_file(self, remote_path):
+        return self.client.object_exists(remote_path)
+
+    def download_file(self, remote_path, locale_path):
+        try:
+            self.client.get_object_to_file(remote_path, locale_path)
+            return True
+        except:
+            return False
```

### Comparing `jms-storage-0.0.46/setup.py` & `jms-storage-0.0.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 #!/usr/bin/env python
 # coding: utf-8
 # Copyright (c) 2018
+# Gmail:liuzheng712
+#
+
+
 import re
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
@@ -14,35 +18,25 @@
 
 if not version:
     raise RuntimeError('Cannot find version information')
 
 with open('README.md', 'rb') as f:
     readme = f.read().decode('utf-8')
 
-with open('requirements.txt', 'r') as f:
-    requirements = [x.strip() for x in f.readlines()]
+with open('jms_storage.egg-info/requires.txt', 'r') as requirements_file:
+    requirements = [x.strip() for x in requirements_file.readlines()]
 
 setup(
     name='jms-storage',
     version=version,
-    keywords=['jumpserver', 'storage', 'oss', 's3', 'elasticsearch'],
+    keywords=['jumpserver', 'storage', 'oss', 's3', 'aws'],
     description='Jumpserver storage python sdk tools',
     long_description=readme,
     license='MIT Licence',
     url='http://www.jumpserver.org/',
     author='Jumpserver team',
-    author_email='support@fit2cloud.com',
+    author_email='liuzheng712@gmail.com',
     packages=['jms_storage'],
-    data_files=[('requirements', ['requirements.txt'])],
     include_package_data=True,
     install_requires=requirements,
     platforms='any',
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6'
-    ]
 )
```

