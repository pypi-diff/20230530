# Comparing `tmp/O365-2.0.8.tar.gz` & `tmp/O365-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\O365-2.0.8.tar", last modified: Wed Apr 15 21:59:55 2020, max compression
+gzip compressed data, was "dist\O365-2.0.9.tar", last modified: Tue Apr 21 09:18:00 2020, max compression
```

## Comparing `O365-2.0.8.tar` & `O365-2.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2020-04-15 21:59:55.000000 O365-2.0.8/
-drwxrwxrwx   0        0        0        0 2020-04-15 21:59:55.000000 O365-2.0.8/O365/
--rw-rw-rw-   0        0        0      400 2019-08-29 10:59:11.000000 O365-2.0.8/O365/__init__.py
--rw-rw-rw-   0        0        0       25 2020-04-15 21:56:10.000000 O365-2.0.8/O365/__version__.py
--rw-rw-rw-   0        0        0    10845 2020-04-03 08:09:22.000000 O365-2.0.8/O365/account.py
--rw-rw-rw-   0        0        0    33113 2019-11-11 21:01:27.000000 O365-2.0.8/O365/address_book.py
--rw-rw-rw-   0        0        0    71694 2019-12-21 23:16:22.000000 O365-2.0.8/O365/calendar.py
--rw-rw-rw-   0        0        0     7202 2020-04-03 08:09:22.000000 O365-2.0.8/O365/category.py
--rw-rw-rw-   0        0        0    39334 2020-04-03 08:09:22.000000 O365-2.0.8/O365/connection.py
--rw-rw-rw-   0        0        0    12963 2019-11-05 21:45:28.000000 O365-2.0.8/O365/directory.py
--rw-rw-rw-   0        0        0    70081 2020-04-15 21:49:45.000000 O365-2.0.8/O365/drive.py
--rw-rw-rw-   0        0        0    68752 2020-04-03 08:09:22.000000 O365-2.0.8/O365/excel.py
--rw-rw-rw-   0        0        0    21994 2019-11-05 21:45:27.000000 O365-2.0.8/O365/mailbox.py
--rw-rw-rw-   0        0        0    38397 2020-04-03 08:09:22.000000 O365-2.0.8/O365/message.py
--rw-rw-rw-   0        0        0     5114 2019-11-05 21:45:27.000000 O365-2.0.8/O365/planner.py
--rw-rw-rw-   0        0        0    24733 2019-11-05 21:45:28.000000 O365-2.0.8/O365/sharepoint.py
--rw-rw-rw-   0        0        0    10623 2020-04-15 21:59:06.000000 O365-2.0.8/O365/teams.py
-drwxrwxrwx   0        0        0        0 2020-04-15 21:59:55.000000 O365-2.0.8/O365/utils/
--rw-rw-rw-   0        0        0      528 2019-03-10 16:35:20.000000 O365-2.0.8/O365/utils/__init__.py
--rw-rw-rw-   0        0        0    19218 2019-11-05 21:45:27.000000 O365-2.0.8/O365/utils/attachment.py
--rw-rw-rw-   0        0        0     3519 2019-01-03 10:53:23.000000 O365-2.0.8/O365/utils/decorators.py
--rw-rw-rw-   0        0        0    11230 2020-04-03 08:09:22.000000 O365-2.0.8/O365/utils/token.py
--rw-rw-rw-   0        0        0    42635 2020-04-15 21:49:45.000000 O365-2.0.8/O365/utils/utils.py
--rw-rw-rw-   0        0        0    30629 2019-12-13 21:43:39.000000 O365-2.0.8/O365/utils/windows_tz.py
-drwxrwxrwx   0        0        0        0 2020-04-15 21:59:55.000000 O365-2.0.8/O365.egg-info/
--rw-rw-rw-   0        0        0    70880 2020-04-15 21:59:53.000000 O365-2.0.8/O365.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2020-04-15 21:59:53.000000 O365-2.0.8/O365.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-04-15 21:59:53.000000 O365-2.0.8/O365.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2020-04-15 21:59:53.000000 O365-2.0.8/O365.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2020-04-15 21:59:53.000000 O365-2.0.8/O365.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    70880 2020-04-15 21:59:55.000000 O365-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    59369 2020-04-03 08:09:22.000000 O365-2.0.8/README.md
--rw-rw-rw-   0        0        0       42 2020-04-15 21:59:55.000000 O365-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1757 2020-04-15 21:56:10.000000 O365-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-04-21 09:18:00.000000 O365-2.0.9/
+drwxrwxrwx   0        0        0        0 2020-04-21 09:17:59.000000 O365-2.0.9/O365/
+-rw-rw-rw-   0        0        0    10845 2020-04-15 07:46:10.000000 O365-2.0.9/O365/account.py
+-rw-rw-rw-   0        0        0    33113 2019-11-08 12:24:21.000000 O365-2.0.9/O365/address_book.py
+-rw-rw-rw-   0        0        0    71694 2020-02-06 15:11:09.000000 O365-2.0.9/O365/calendar.py
+-rw-rw-rw-   0        0        0     7202 2020-02-06 15:13:26.000000 O365-2.0.9/O365/category.py
+-rw-rw-rw-   0        0        0    39334 2020-02-19 17:13:04.000000 O365-2.0.9/O365/connection.py
+-rw-rw-rw-   0        0        0    12963 2019-11-08 11:04:05.000000 O365-2.0.9/O365/directory.py
+-rw-rw-rw-   0        0        0    70081 2020-04-21 09:05:30.000000 O365-2.0.9/O365/drive.py
+-rw-rw-rw-   0        0        0    68752 2020-02-06 15:11:09.000000 O365-2.0.9/O365/excel.py
+-rw-rw-rw-   0        0        0    21994 2019-11-08 11:04:05.000000 O365-2.0.9/O365/mailbox.py
+-rw-rw-rw-   0        0        0    38397 2020-02-06 15:28:27.000000 O365-2.0.9/O365/message.py
+-rw-rw-rw-   0        0        0     5114 2019-11-08 11:04:05.000000 O365-2.0.9/O365/planner.py
+-rw-rw-rw-   0        0        0    24140 2020-04-21 09:03:59.000000 O365-2.0.9/O365/sharepoint.py
+-rw-rw-rw-   0        0        0    10623 2020-04-21 09:05:30.000000 O365-2.0.9/O365/teams.py
+drwxrwxrwx   0        0        0        0 2020-04-21 09:18:00.000000 O365-2.0.9/O365/utils/
+-rw-rw-rw-   0        0        0    19218 2019-11-08 11:04:05.000000 O365-2.0.9/O365/utils/attachment.py
+-rw-rw-rw-   0        0        0     3519 2018-12-19 08:58:56.000000 O365-2.0.9/O365/utils/decorators.py
+-rw-rw-rw-   0        0        0    11230 2020-02-06 15:11:09.000000 O365-2.0.9/O365/utils/token.py
+-rw-rw-rw-   0        0        0    42635 2020-04-21 09:05:30.000000 O365-2.0.9/O365/utils/utils.py
+-rw-rw-rw-   0        0        0    30629 2019-12-05 12:38:40.000000 O365-2.0.9/O365/utils/windows_tz.py
+-rw-rw-rw-   0        0        0      528 2019-03-04 13:55:14.000000 O365-2.0.9/O365/utils/__init__.py
+-rw-rw-rw-   0        0        0      400 2019-08-02 07:57:31.000000 O365-2.0.9/O365/__init__.py
+-rw-rw-rw-   0        0        0       23 2020-04-21 09:17:11.000000 O365-2.0.9/O365/__version__.py
+drwxrwxrwx   0        0        0        0 2020-04-21 09:17:59.000000 O365-2.0.9/O365.egg-info/
+-rw-rw-rw-   0        0        0        1 2020-04-21 09:17:58.000000 O365-2.0.9/O365.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    70880 2020-04-21 09:17:58.000000 O365-2.0.9/O365.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2020-04-21 09:17:58.000000 O365-2.0.9/O365.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      549 2020-04-21 09:17:58.000000 O365-2.0.9/O365.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        5 2020-04-21 09:17:58.000000 O365-2.0.9/O365.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    70880 2020-04-21 09:18:00.000000 O365-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    59369 2020-02-06 15:11:09.000000 O365-2.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2020-04-21 09:18:00.000000 O365-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1757 2020-04-21 09:17:11.000000 O365-2.0.9/setup.py
```

### Comparing `O365-2.0.8/O365/account.py` & `O365-2.0.9/O365/account.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/address_book.py` & `O365-2.0.9/O365/address_book.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/calendar.py` & `O365-2.0.9/O365/calendar.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/category.py` & `O365-2.0.9/O365/category.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/connection.py` & `O365-2.0.9/O365/connection.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/directory.py` & `O365-2.0.9/O365/directory.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/drive.py` & `O365-2.0.9/O365/drive.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/excel.py` & `O365-2.0.9/O365/excel.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/mailbox.py` & `O365-2.0.9/O365/mailbox.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/message.py` & `O365-2.0.9/O365/message.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/planner.py` & `O365-2.0.9/O365/planner.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/sharepoint.py` & `O365-2.0.9/O365/sharepoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,31 +450,21 @@
         """ Returns a Document Library (a Drive instance)
 
         :param drive_id: the drive_id to be retrieved.
         :rtype: Drive
         """
         return self.site_storage.get_drive(drive_id=drive_id)
 
-    def list_document_libraries(self, limit=None, *, query=None, order_by=None,
-                                batch=None):
+    def list_document_libraries(self):
         """ Returns a collection of document libraries for this site
         (a collection of Drive instances)
-
-        :param int limit: max no. of items to get. Over 999 uses batch.
-        :param query: applies a OData filter to the request
-        :type query: Query or str
-        :param order_by: orders the result set based on this condition
-        :type order_by: Query or str
-        :param int batch: batch size, retrieves items in
-         batches allowing to retrieve more items than the limit.
         :return: list of items in this folder
         :rtype: list[Drive] or Pagination
         """
-        return self.site_storage.get_drives(limit=limit, query=query,
-                                            order_by=order_by, batch=batch)
+        return self.site_storage.get_drives()
 
     def get_subsites(self):
         """ Returns a list of subsites defined for this site
 
         :rtype: list[Site]
         """
         url = self.build_url(
```

### Comparing `O365-2.0.8/O365/teams.py` & `O365-2.0.9/O365/teams.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/utils/__init__.py` & `O365-2.0.9/O365/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/utils/attachment.py` & `O365-2.0.9/O365/utils/attachment.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/utils/decorators.py` & `O365-2.0.9/O365/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/utils/token.py` & `O365-2.0.9/O365/utils/token.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/utils/utils.py` & `O365-2.0.9/O365/utils/utils.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365/utils/windows_tz.py` & `O365-2.0.9/O365/utils/windows_tz.py`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/O365.egg-info/PKG-INFO` & `O365-2.0.9/O365.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: O365
-Version: 2.0.8
+Version: 2.0.9
 Summary: Microsoft Graph and Office 365 API made easy
 Home-page: https://github.com/O365/python-o365
 Author: Janscas, Roycem90, Narcolapser
 Author-email: janscas@users.noreply.github.com
 Maintainer: Janscas
 Maintainer-email: janscas@users.noreply.github.com
 License: Apache License 2.0
```

### Comparing `O365-2.0.8/O365.egg-info/SOURCES.txt` & `O365-2.0.9/O365.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/PKG-INFO` & `O365-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: O365
-Version: 2.0.8
+Version: 2.0.9
 Summary: Microsoft Graph and Office 365 API made easy
 Home-page: https://github.com/O365/python-o365
 Author: Janscas, Roycem90, Narcolapser
 Author-email: janscas@users.noreply.github.com
 Maintainer: Janscas
 Maintainer-email: janscas@users.noreply.github.com
 License: Apache License 2.0
```

### Comparing `O365-2.0.8/README.md` & `O365-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `O365-2.0.8/setup.py` & `O365-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import setup, find_packages
 
 
-VERSION = '2.0.8'
+VERSION = '2.0.9'
 
 # Available classifiers: https://pypi.org/pypi?%3Aaction=list_classifiers
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Topic :: Office/Business :: Office Suites',
```

