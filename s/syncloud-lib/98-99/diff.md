# Comparing `tmp/syncloud-lib-98.tar.gz` & `tmp/syncloud-lib-99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/syncloud-lib-98.tar", last modified: Tue Jan 15 21:11:17 2019, max compression
+gzip compressed data, was "dist/syncloud-lib-99.tar", last modified: Sat Jan 26 09:08:25 2019, max compression
```

## Comparing `syncloud-lib-98.tar` & `syncloud-lib-99.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-15 21:11:17.000000 syncloud-lib-98/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-15 21:11:17.000000 syncloud-lib-98/syncloud_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1399 2019-01-15 21:11:17.000000 syncloud-lib-98/syncloud_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-01-15 21:11:17.000000 syncloud-lib-98/syncloud_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2019-01-15 21:11:17.000000 syncloud-lib-98/syncloud_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2019-01-15 21:11:17.000000 syncloud-lib-98/syncloud_lib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      235 2019-01-15 21:11:17.000000 syncloud-lib-98/syncloud_lib.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-15 21:11:17.000000 syncloud-lib-98/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-15 21:11:17.000000 syncloud-lib-98/test/json/
--rw-r--r--   0 root         (0) root         (0)     6747 2019-01-15 21:11:04.000000 syncloud-lib-98/test/json/test_convertible.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-15 21:11:17.000000 syncloud-lib-98/test/application/
--rw-r--r--   0 root         (0) root         (0)      104 2019-01-15 21:11:04.000000 syncloud-lib-98/test/application/test_paths.py
--rw-r--r--   0 root         (0) root         (0)       88 2019-01-15 21:11:04.000000 syncloud-lib-98/test/application/test_service.py
--rw-r--r--   0 root         (0) root         (0)      101 2019-01-15 21:11:04.000000 syncloud-lib-98/test/application/test_connection.py
--rw-r--r--   0 root         (0) root         (0)       89 2019-01-15 21:11:04.000000 syncloud-lib-98/test/application/test_urls.py
--rw-r--r--   0 root         (0) root         (0)       93 2019-01-15 21:11:04.000000 syncloud-lib-98/test/application/test_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-15 21:11:17.000000 syncloud-lib-98/test/integration/
--rw-r--r--   0 root         (0) root         (0)       83 2019-01-15 21:11:04.000000 syncloud-lib-98/test/integration/test_ssh.py
--rw-r--r--   0 root         (0) root         (0)      433 2019-01-15 21:11:04.000000 syncloud-lib-98/test/integration/test_hosts.py
--rw-r--r--   0 root         (0) root         (0)       95 2019-01-15 21:11:04.000000 syncloud-lib-98/test/integration/test_installer.py
--rw-r--r--   0 root         (0) root         (0)       96 2019-01-15 21:11:04.000000 syncloud-lib-98/test/integration/test_loop.py
--rw-r--r--   0 root         (0) root         (0)       78 2019-01-15 21:11:04.000000 syncloud-lib-98/test/test_gen.py
--rw-r--r--   0 root         (0) root         (0)       74 2019-01-15 21:11:04.000000 syncloud-lib-98/test/test_linux.py
--rw-r--r--   0 root         (0) root         (0)     1254 2019-01-15 21:11:04.000000 syncloud-lib-98/test/test_logger.py
--rw-r--r--   0 root         (0) root         (0)       71 2019-01-15 21:11:04.000000 syncloud-lib-98/test/test_fs.py
--rw-r--r--   0 root         (0) root         (0)       38 2019-01-15 21:11:17.000000 syncloud-lib-98/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-15 21:11:17.000000 syncloud-lib-98/syncloudlib/
--rw-r--r--   0 root         (0) root         (0)        0 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-15 21:11:17.000000 syncloud-lib-98/syncloudlib/json/
--rw-r--r--   0 root         (0) root         (0)        0 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/json/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3240 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/json/convertible.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-15 21:11:17.000000 syncloud-lib-98/syncloudlib/application/
--rw-r--r--   0 root         (0) root         (0)     1561 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/application/connection.py
--rw-r--r--   0 root         (0) root         (0)        0 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/application/__init__.py
--rw-r--r--   0 root         (0) root         (0)      254 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/application/ports.py
--rw-r--r--   0 root         (0) root         (0)      275 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/application/urls.py
--rw-r--r--   0 root         (0) root         (0)       84 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/application/users.py
--rw-r--r--   0 root         (0) root         (0)      199 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/application/paths.py
--rw-r--r--   0 root         (0) root         (0)      244 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/application/storage.py
--rw-r--r--   0 root         (0) root         (0)      131 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/application/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-15 21:11:17.000000 syncloud-lib-98/syncloudlib/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1591 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/integration/ssh.py
--rw-r--r--   0 root         (0) root         (0)     2124 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/integration/device.py
--rw-r--r--   0 root         (0) root         (0)     4003 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/integration/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1467 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/integration/screenshots.py
--rw-r--r--   0 root         (0) root         (0)     2474 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/integration/installer.py
--rw-r--r--   0 root         (0) root         (0)     1585 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/integration/loop.py
--rw-r--r--   0 root         (0) root         (0)      305 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/integration/hosts.py
--rw-r--r--   0 root         (0) root         (0)     1776 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/logger.py
--rw-r--r--   0 root         (0) root         (0)      501 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/linux.py
--rw-r--r--   0 root         (0) root         (0)      172 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/error.py
--rw-r--r--   0 root         (0) root         (0)     1833 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/gen.py
--rw-r--r--   0 root         (0) root         (0)      804 2019-01-15 21:11:04.000000 syncloud-lib-98/syncloudlib/fs.py
--rw-r--r--   0 root         (0) root         (0)    35142 2019-01-15 21:11:04.000000 syncloud-lib-98/LICENSE
--rw-r--r--   0 root         (0) root         (0)      742 2019-01-15 21:11:04.000000 syncloud-lib-98/setup.py
--rw-r--r--   0 root         (0) root         (0)      182 2019-01-15 21:11:04.000000 syncloud-lib-98/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-15 21:11:17.000000 syncloud-lib-98/bin/
--rwxr-xr-x   0 root         (0) root         (0)      452 2019-01-15 21:11:04.000000 syncloud-lib-98/bin/syncloud-upload.sh
--rwxr-xr-x   0 root         (0) root         (0)      505 2019-01-15 21:11:04.000000 syncloud-lib-98/bin/syncloud-upload-artifact.sh
--rw-r--r--   0 root         (0) root         (0)      235 2019-01-15 21:11:17.000000 syncloud-lib-98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        3 2019-01-15 21:11:06.000000 syncloud-lib-98/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-26 09:08:25.000000 syncloud-lib-99/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-26 09:08:25.000000 syncloud-lib-99/syncloud_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1399 2019-01-26 09:08:24.000000 syncloud-lib-99/syncloud_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-01-26 09:08:24.000000 syncloud-lib-99/syncloud_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2019-01-26 09:08:24.000000 syncloud-lib-99/syncloud_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2019-01-26 09:08:24.000000 syncloud-lib-99/syncloud_lib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      235 2019-01-26 09:08:24.000000 syncloud-lib-99/syncloud_lib.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-26 09:08:25.000000 syncloud-lib-99/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-26 09:08:25.000000 syncloud-lib-99/test/json/
+-rw-r--r--   0 root         (0) root         (0)     6747 2019-01-26 09:08:10.000000 syncloud-lib-99/test/json/test_convertible.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-26 09:08:25.000000 syncloud-lib-99/test/application/
+-rw-r--r--   0 root         (0) root         (0)      104 2019-01-26 09:08:10.000000 syncloud-lib-99/test/application/test_paths.py
+-rw-r--r--   0 root         (0) root         (0)       88 2019-01-26 09:08:10.000000 syncloud-lib-99/test/application/test_service.py
+-rw-r--r--   0 root         (0) root         (0)      101 2019-01-26 09:08:10.000000 syncloud-lib-99/test/application/test_connection.py
+-rw-r--r--   0 root         (0) root         (0)       89 2019-01-26 09:08:10.000000 syncloud-lib-99/test/application/test_urls.py
+-rw-r--r--   0 root         (0) root         (0)       93 2019-01-26 09:08:10.000000 syncloud-lib-99/test/application/test_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-26 09:08:25.000000 syncloud-lib-99/test/integration/
+-rw-r--r--   0 root         (0) root         (0)       83 2019-01-26 09:08:10.000000 syncloud-lib-99/test/integration/test_ssh.py
+-rw-r--r--   0 root         (0) root         (0)      433 2019-01-26 09:08:10.000000 syncloud-lib-99/test/integration/test_hosts.py
+-rw-r--r--   0 root         (0) root         (0)       95 2019-01-26 09:08:10.000000 syncloud-lib-99/test/integration/test_installer.py
+-rw-r--r--   0 root         (0) root         (0)       96 2019-01-26 09:08:10.000000 syncloud-lib-99/test/integration/test_loop.py
+-rw-r--r--   0 root         (0) root         (0)       78 2019-01-26 09:08:10.000000 syncloud-lib-99/test/test_gen.py
+-rw-r--r--   0 root         (0) root         (0)       74 2019-01-26 09:08:10.000000 syncloud-lib-99/test/test_linux.py
+-rw-r--r--   0 root         (0) root         (0)     1254 2019-01-26 09:08:10.000000 syncloud-lib-99/test/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)       71 2019-01-26 09:08:10.000000 syncloud-lib-99/test/test_fs.py
+-rw-r--r--   0 root         (0) root         (0)       38 2019-01-26 09:08:25.000000 syncloud-lib-99/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-26 09:08:25.000000 syncloud-lib-99/syncloudlib/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-26 09:08:25.000000 syncloud-lib-99/syncloudlib/json/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/json/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3240 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/json/convertible.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-26 09:08:25.000000 syncloud-lib-99/syncloudlib/application/
+-rw-r--r--   0 root         (0) root         (0)     1561 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/application/connection.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/application/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      254 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/application/ports.py
+-rw-r--r--   0 root         (0) root         (0)      275 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/application/urls.py
+-rw-r--r--   0 root         (0) root         (0)       84 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/application/users.py
+-rw-r--r--   0 root         (0) root         (0)      199 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/application/paths.py
+-rw-r--r--   0 root         (0) root         (0)      244 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/application/storage.py
+-rw-r--r--   0 root         (0) root         (0)      131 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/application/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-26 09:08:25.000000 syncloud-lib-99/syncloudlib/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/integration/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/integration/device.py
+-rw-r--r--   0 root         (0) root         (0)     4003 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/integration/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/integration/screenshots.py
+-rw-r--r--   0 root         (0) root         (0)     2558 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/integration/installer.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/integration/loop.py
+-rw-r--r--   0 root         (0) root         (0)      305 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/integration/hosts.py
+-rw-r--r--   0 root         (0) root         (0)     1776 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/logger.py
+-rw-r--r--   0 root         (0) root         (0)      501 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/linux.py
+-rw-r--r--   0 root         (0) root         (0)      172 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/error.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/gen.py
+-rw-r--r--   0 root         (0) root         (0)      804 2019-01-26 09:08:10.000000 syncloud-lib-99/syncloudlib/fs.py
+-rw-r--r--   0 root         (0) root         (0)    35142 2019-01-26 09:08:10.000000 syncloud-lib-99/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      742 2019-01-26 09:08:10.000000 syncloud-lib-99/setup.py
+-rw-r--r--   0 root         (0) root         (0)      182 2019-01-26 09:08:10.000000 syncloud-lib-99/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-01-26 09:08:25.000000 syncloud-lib-99/bin/
+-rwxr-xr-x   0 root         (0) root         (0)      452 2019-01-26 09:08:10.000000 syncloud-lib-99/bin/syncloud-upload.sh
+-rwxr-xr-x   0 root         (0) root         (0)      505 2019-01-26 09:08:10.000000 syncloud-lib-99/bin/syncloud-upload-artifact.sh
+-rw-r--r--   0 root         (0) root         (0)      235 2019-01-26 09:08:25.000000 syncloud-lib-99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        3 2019-01-26 09:08:12.000000 syncloud-lib-99/version
```

### Comparing `syncloud-lib-98/syncloud_lib.egg-info/SOURCES.txt` & `syncloud-lib-99/syncloud_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/test/json/test_convertible.py` & `syncloud-lib-99/test/json/test_convertible.py`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/test/test_logger.py` & `syncloud-lib-99/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/syncloudlib/json/convertible.py` & `syncloud-lib-99/syncloudlib/json/convertible.py`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/syncloudlib/application/connection.py` & `syncloud-lib-99/syncloudlib/application/connection.py`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/syncloudlib/integration/ssh.py` & `syncloud-lib-99/syncloudlib/integration/ssh.py`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/syncloudlib/integration/device.py` & `syncloud-lib-99/syncloudlib/integration/device.py`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/syncloudlib/integration/conftest.py` & `syncloud-lib-99/syncloudlib/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/syncloudlib/integration/screenshots.py` & `syncloud-lib-99/syncloudlib/integration/screenshots.py`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/syncloudlib/integration/installer.py` & `syncloud-lib-99/syncloudlib/integration/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,27 +38,28 @@
 
 
 def wait_for_platform_web(host):
     print(check_output('while ! nc -w 1 -z {0} 81; do sleep 1; done'.format(host), shell=True))
     print(check_output('while ! nc -w 1 -z {0} 80; do sleep 1; done'.format(host), shell=True))
 
 
-def wait_for_installer(web_session, host):
+def wait_for_installer(web_session, host, attempts=200, throw_on_error=False):
     is_running = True
-    attempts = 200
     attempt = 0
     while is_running and attempt < attempts:
         try:
             response = web_session.get('https://{0}/rest/settings/sam_status'.format(host), verify=False)
             if response.status_code == 200:
                 status = json.loads(response.text)
                 is_running = status['is_running']
         except Exception, e:
             print(e.message)
-
+            if throw_on_error:
+                raise e
+            
         print("attempt: {0}/{1}".format(attempt, attempts))
         attempt += 1
         time.sleep(10)
     
     if is_running:
         raise Exception("time out waiting for thr installer")
```

### Comparing `syncloud-lib-98/syncloudlib/integration/loop.py` & `syncloud-lib-99/syncloudlib/integration/loop.py`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/syncloudlib/logger.py` & `syncloud-lib-99/syncloudlib/logger.py`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/syncloudlib/gen.py` & `syncloud-lib-99/syncloudlib/gen.py`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/syncloudlib/fs.py` & `syncloud-lib-99/syncloudlib/fs.py`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/LICENSE` & `syncloud-lib-99/LICENSE`

 * *Files identical despite different names*

### Comparing `syncloud-lib-98/setup.py` & `syncloud-lib-99/setup.py`

 * *Files identical despite different names*

