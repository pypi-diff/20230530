# Comparing `tmp/dms-collector-2.0.2.tar.gz` & `tmp/dms-collector-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dms-collector-2.0.2.tar", last modified: Wed Aug 31 22:18:25 2022, max compression
+gzip compressed data, was "dms-collector-2.0.3.tar", last modified: Tue May 30 09:19:10 2023, max compression
```

## Comparing `dms-collector-2.0.2.tar` & `dms-collector-2.0.3.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2022-08-31 22:18:25.836713 dms-collector-2.0.2/
--rw-r--r--   0 tomas      (501) staff       (20)     5634 2022-08-31 22:18:25.836576 dms-collector-2.0.2/PKG-INFO
--rw-r--r--   0 tomas      (501) staff       (20)     4445 2022-08-31 16:12:57.000000 dms-collector-2.0.2/README.md
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2022-08-31 22:18:25.834944 dms-collector-2.0.2/bin/
--rwxr-xr-x   0 tomas      (501) staff       (20)      106 2022-08-31 16:12:57.000000 dms-collector-2.0.2/bin/dms-collector
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2022-08-31 22:18:25.835569 dms-collector-2.0.2/dms_collector/
--rw-r--r--   0 tomas      (501) staff       (20)      242 2022-08-31 22:15:31.000000 dms-collector-2.0.2/dms_collector/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)     7170 2022-08-31 16:12:57.000000 dms-collector-2.0.2/dms_collector/__main__.py
--rw-r--r--   0 tomas      (501) staff       (20)     9365 2022-08-31 22:15:31.000000 dms-collector-2.0.2/dms_collector/dms.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2022-08-31 22:18:25.836395 dms-collector-2.0.2/dms_collector.egg-info/
--rw-r--r--   0 tomas      (501) staff       (20)     5634 2022-08-31 22:18:25.000000 dms-collector-2.0.2/dms_collector.egg-info/PKG-INFO
--rw-r--r--   0 tomas      (501) staff       (20)      293 2022-08-31 22:18:25.000000 dms-collector-2.0.2/dms_collector.egg-info/SOURCES.txt
--rw-r--r--   0 tomas      (501) staff       (20)        1 2022-08-31 22:18:25.000000 dms-collector-2.0.2/dms_collector.egg-info/dependency_links.txt
--rw-r--r--   0 tomas      (501) staff       (20)       33 2022-08-31 22:18:25.000000 dms-collector-2.0.2/dms_collector.egg-info/requires.txt
--rw-r--r--   0 tomas      (501) staff       (20)       14 2022-08-31 22:18:25.000000 dms-collector-2.0.2/dms_collector.egg-info/top_level.txt
--rw-r--r--   0 tomas      (501) staff       (20)       38 2022-08-31 22:18:25.836759 dms-collector-2.0.2/setup.cfg
--rw-r--r--   0 tomas      (501) staff       (20)     1768 2022-08-31 16:12:57.000000 dms-collector-2.0.2/setup.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-30 09:19:10.756715 dms-collector-2.0.3/
+-rw-r--r--   0 tomas      (501) staff       (20)       94 2023-05-30 08:10:10.000000 dms-collector-2.0.3/.gitignore
+-rw-r--r--   0 tomas      (501) staff       (20)      282 2023-05-30 08:44:09.000000 dms-collector-2.0.3/CHANGELOG.md
+-rw-r--r--   0 tomas      (501) staff       (20)      361 2022-01-12 13:39:26.000000 dms-collector-2.0.3/Makefile
+-rw-r--r--   0 tomas      (501) staff       (20)     5007 2023-05-30 09:19:10.756582 dms-collector-2.0.3/PKG-INFO
+-rw-r--r--   0 tomas      (501) staff       (20)     4445 2022-01-12 10:46:25.000000 dms-collector-2.0.3/README.md
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-30 09:19:10.754882 dms-collector-2.0.3/bin/
+-rwxr-xr-x   0 tomas      (501) staff       (20)      106 2022-01-07 20:33:00.000000 dms-collector-2.0.3/bin/dms-collector
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-30 09:19:10.755622 dms-collector-2.0.3/dms_collector/
+-rw-r--r--   0 tomas      (501) staff       (20)      451 2023-05-30 08:20:03.000000 dms-collector-2.0.3/dms_collector/__init__.py
+-rw-r--r--   0 tomas      (501) staff       (20)     7628 2023-05-30 09:15:26.000000 dms-collector-2.0.3/dms_collector/__main__.py
+-rw-r--r--   0 tomas      (501) staff       (20)    10164 2023-05-30 08:49:00.000000 dms-collector-2.0.3/dms_collector/dms.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-30 09:19:10.756377 dms-collector-2.0.3/dms_collector.egg-info/
+-rw-r--r--   0 tomas      (501) staff       (20)     5007 2023-05-30 09:19:10.000000 dms-collector-2.0.3/dms_collector.egg-info/PKG-INFO
+-rw-r--r--   0 tomas      (501) staff       (20)      326 2023-05-30 09:19:10.000000 dms-collector-2.0.3/dms_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 tomas      (501) staff       (20)        1 2023-05-30 09:19:10.000000 dms-collector-2.0.3/dms_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 tomas      (501) staff       (20)       54 2023-05-30 09:19:10.000000 dms-collector-2.0.3/dms_collector.egg-info/requires.txt
+-rw-r--r--   0 tomas      (501) staff       (20)       14 2023-05-30 09:19:10.000000 dms-collector-2.0.3/dms_collector.egg-info/top_level.txt
+-rw-r--r--   0 tomas      (501) staff       (20)       38 2023-05-30 09:19:10.756753 dms-collector-2.0.3/setup.cfg
+-rw-r--r--   0 tomas      (501) staff       (20)     1818 2023-05-30 08:12:41.000000 dms-collector-2.0.3/setup.py
```

### Comparing `dms-collector-2.0.2/PKG-INFO` & `dms-collector-2.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,97 @@
 Metadata-Version: 2.1
 Name: dms-collector
-Version: 2.0.2
+Version: 2.0.3
 Summary: Oracle FMW DMS Spy collector utility
 Home-page: UNKNOWN
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
 License: UNKNOWN
-Description: # $ dms-collector
-        
-        DMS is a Weblogic Dynamic Monitoring Service providing a massive amount of sensors about Weblogic and application components performance.
-        It can be accessed in a number of ways, such as Weblogic Scripting Tool (wlst), Java API or DMS Spy application. DMS Spy is used to access DMS metric tables by using a browser while it also provides endpoints to retrieve metric tables in XML format.
-        
-        dms-collector is a Python utility that retrieves DMS metrics from Weblogic DMS Spy application. It provides an API to access DMS tables' data and a CLI to query the DMS and display the data in CSV.
-        
-        ## Installation
-        
-        You can install the dms-collector with pip as follows:
-        
-        ```
-        pip install dms-collector 
-        ``` 
-        
-        ## Usage
-        
-        You can use dms-collector CLI to query the DMS Spy running at `https://wls-domain` with username `weblogic` and password `password1` by running the following command: 
-        
-        ```
-        $ dms-collector --url https://wls-domain --connect weblogic/password1 --table JVM_Memory
-        datetime,timezone,Host,Parent,ServerName,pendingFinalization_value,verbose_value,Process,JVM,Name
-        "22-01-12 11:23:30",+0100,"domain-3.oraclevnc.com","/JVM/MxBeans","AdminServer",0,"TRUE","AdminServer:7101","JVM","memory"
-        "22-01-12 11:23:30",+0100,"fmw-poc-app10.oraclevcn.com","/JVM/MxBeans","soa_server2",0,"TRUE","soa_server2:8102","JVM","memory"
-        "22-01-12 11:23:30",+0100,"fmw-poc-app10.oraclevcn.com","/JVM/MxBeans","proc15010",0,"FALSE","machine2:15010","JVM","memory"
-        "22-01-12 11:23:30",+0100,"domain-3.oraclevcn.com","/JVM/MxBeans","proc69725",0,"FALSE","machine1:69725","JVM","memory"
-        ```
-        
-        ## CLI Options
-        
-        There are many options that you can use to control, for example, a number of calls the CLI will run, a delay between calls, fields to be included or excluded or rows to be filtered out in the result. 
-        
-        For the full list of options please run `dms-collector --help`. 
-        
-        ### Filtering 
-        
-        If you want to exclude certain fields from the output, such as `Process` and `Parent`, run the following command:
-        
-        ```
-        $ dms-collector --url https://wls-domain --connect weblogic/password1 --table JVM_Memory \
-          --exclude Process,Parent
-        ```
-        
-        If you want to only return rows that match a certain criteria, such as a server name, run the following command:
-        
-        ```
-        $ dms-collector --url https://wls-domain --connect weblogic/password1 --table JVM_Memory \
-          --filter "bool(re.match(r\"WLS_SOA[0-9]+\",str(ServerName)))"
-        ```
-        
-        The `--filter` parameter accepts any valid Python expression with variable names matching table's header names. You can use all header names regardless whether they are included or excluded from the output.   
-        
-        ### Timestamp and Timezone
-        
-        The dms-collector CLI adds two columns to the CSV output, namely `datetime` and `timezone`. This is the current local time when the data is retrieved from the DMS and changes with every iteration. You can change the field names for both columns by using `--datetimefield` and `--timezonefield` respectively as well as remove them from the output by using `--exclude` option.    
-        
-        ### Delay Time
-        
-        You can specify a number of seconds the dms-collector CLI should wait between iterations by using `--delay` parameter. Since reading the data may in some situations take more time to finish, the delay time needs to be adjusted so that dms-collector always retrieves the data at the same time and the overall running time can be determined. The time adjustment is however disabled when the time to retrieve the DMS data takes more than 2/3 of the delay time. You can disable the delay time adjustment by using `--nodelayadjust` or change the 2/3 limit by `--nodelayperc`.
-        
-        ### Login
-         
-        dms-collector uses DMS Spy login form by default. If you are collecting data from a DMS Spy of an earlier version such as FMW infrastructure 11g, you need to use `--basicauth` option which uses HTTP basic authentication.
-         
-        ## Changes over previous version 1.1
-        
-        The version 2.0+ introduces the following changes:
-        
-        *  It is now possible to use `dms-collector` as a Python module which provides [DmsCollector class](https://github.com/tomvit/dms-collector/blob/v2.0/dms_collector/dms.py) that you can integrate into your Python applications. 
-        
-        * Several command-line arguments were removed such as linux pipelines and emitting the events, DMS reset and time adjustments.  
-        
-        You can still access the previous version in [1.1 branch](https://github.com/tomvit/dms-collector/tree/v1.1).
-         
-        # License
-        
-        free and free as a bird
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.5.0
+Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+
+# $ dms-collector
+
+DMS is a Weblogic Dynamic Monitoring Service providing a massive amount of sensors about Weblogic and application components performance.
+It can be accessed in a number of ways, such as Weblogic Scripting Tool (wlst), Java API or DMS Spy application. DMS Spy is used to access DMS metric tables by using a browser while it also provides endpoints to retrieve metric tables in XML format.
+
+dms-collector is a Python utility that retrieves DMS metrics from Weblogic DMS Spy application. It provides an API to access DMS tables' data and a CLI to query the DMS and display the data in CSV.
+
+## Installation
+
+You can install the dms-collector with pip as follows:
+
+```
+pip install dms-collector 
+``` 
+
+## Usage
+
+You can use dms-collector CLI to query the DMS Spy running at `https://wls-domain` with username `weblogic` and password `password1` by running the following command: 
+
+```
+$ dms-collector --url https://wls-domain --connect weblogic/password1 --table JVM_Memory
+datetime,timezone,Host,Parent,ServerName,pendingFinalization_value,verbose_value,Process,JVM,Name
+"22-01-12 11:23:30",+0100,"domain-3.oraclevnc.com","/JVM/MxBeans","AdminServer",0,"TRUE","AdminServer:7101","JVM","memory"
+"22-01-12 11:23:30",+0100,"fmw-poc-app10.oraclevcn.com","/JVM/MxBeans","soa_server2",0,"TRUE","soa_server2:8102","JVM","memory"
+"22-01-12 11:23:30",+0100,"fmw-poc-app10.oraclevcn.com","/JVM/MxBeans","proc15010",0,"FALSE","machine2:15010","JVM","memory"
+"22-01-12 11:23:30",+0100,"domain-3.oraclevcn.com","/JVM/MxBeans","proc69725",0,"FALSE","machine1:69725","JVM","memory"
+```
+
+## CLI Options
+
+There are many options that you can use to control, for example, a number of calls the CLI will run, a delay between calls, fields to be included or excluded or rows to be filtered out in the result. 
+
+For the full list of options please run `dms-collector --help`. 
+
+### Filtering 
+
+If you want to exclude certain fields from the output, such as `Process` and `Parent`, run the following command:
+
+```
+$ dms-collector --url https://wls-domain --connect weblogic/password1 --table JVM_Memory \
+  --exclude Process,Parent
+```
+
+If you want to only return rows that match a certain criteria, such as a server name, run the following command:
+
+```
+$ dms-collector --url https://wls-domain --connect weblogic/password1 --table JVM_Memory \
+  --filter "bool(re.match(r\"WLS_SOA[0-9]+\",str(ServerName)))"
+```
+
+The `--filter` parameter accepts any valid Python expression with variable names matching table's header names. You can use all header names regardless whether they are included or excluded from the output.   
+
+### Timestamp and Timezone
+
+The dms-collector CLI adds two columns to the CSV output, namely `datetime` and `timezone`. This is the current local time when the data is retrieved from the DMS and changes with every iteration. You can change the field names for both columns by using `--datetimefield` and `--timezonefield` respectively as well as remove them from the output by using `--exclude` option.    
+
+### Delay Time
+
+You can specify a number of seconds the dms-collector CLI should wait between iterations by using `--delay` parameter. Since reading the data may in some situations take more time to finish, the delay time needs to be adjusted so that dms-collector always retrieves the data at the same time and the overall running time can be determined. The time adjustment is however disabled when the time to retrieve the DMS data takes more than 2/3 of the delay time. You can disable the delay time adjustment by using `--nodelayadjust` or change the 2/3 limit by `--nodelayperc`.
+
+### Login
+ 
+dms-collector uses DMS Spy login form by default. If you are collecting data from a DMS Spy of an earlier version such as FMW infrastructure 11g, you need to use `--basicauth` option which uses HTTP basic authentication.
+ 
+## Changes over previous version 1.1
+
+The version 2.0+ introduces the following changes:
+
+*  It is now possible to use `dms-collector` as a Python module which provides [DmsCollector class](https://github.com/tomvit/dms-collector/blob/v2.0/dms_collector/dms.py) that you can integrate into your Python applications. 
+
+* Several command-line arguments were removed such as linux pipelines and emitting the events, DMS reset and time adjustments.  
+
+You can still access the previous version in [1.1 branch](https://github.com/tomvit/dms-collector/tree/v1.1).
+ 
+# License
+
+free and free as a bird
+
+
```

### Comparing `dms-collector-2.0.2/README.md` & `dms-collector-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dms-collector-2.0.2/dms_collector/dms.py` & `dms-collector-2.0.3/dms_collector/dms.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-
 import time
 import re
 import os
 
 import xml.etree.ElementTree as ET
 
 import urllib3
 import requests
 
-from dms_collector import __version__
+from importlib.metadata import version, PackageNotFoundError
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 TBML_VERSIONS = ["11.0"]
 
 # DMS REQESTS URLs
 # before changing the urls below check their param bindings as per their usage
@@ -21,241 +20,290 @@
 DMSLOGIN_URL = "%s/dms/j_security_check"
 
 # timeout to read data from dms spy
 TIMEOUT_CONNECT = 3.05
 TIMEOUT_READ = 30
 
 # HTML CLEANER RE
-CLEANR = re.compile('<.*?>|&([a-z0-9]+|#[0-9]{1,6}|#x[0-9a-f]{1,6});')
+CLEANR = re.compile("<.*?>|&([a-z0-9]+|#[0-9]{1,6}|#x[0-9a-f]{1,6});")
+
+
+def dms_version():
+    """
+    Return the version number of the package.
+    """
+    try:
+        return version("dms-collector")
+    except PackageNotFoundError as e:
+        return "unknown"
 
 
 def is_number(s):
-    '''
+    """
     Checks if the argument is a number.
-    '''
+    """
     s = str(s)
-    p = re.compile(r'^[\+\-]?[0-9]*(\.[0-9]+)?$')
-    return s != '' and p.match(s)
+    p = re.compile(r"^[\+\-]?[0-9]*(\.[0-9]+)?$")
+    return s != "" and p.match(s)
 
 
 def check_positive(value):
-    '''
+    """
     Checks if the number is a positive integer.
-    '''
+    """
     ivalue = int(value)
     if ivalue <= 0:
         raise Exception("%s is an invalid positive int value" % value)
     return ivalue
 
 
 def eval_filter(filter, tags, fields):
-    '''
+    """
     Evaluates the filter as a Python expression using tags and fields. It adds
     tags and fields to the scope of the filter evaluation.
-    '''
+    """
     try:
         for k, v in tags.items():
             if v is not None:
-                exec(k + "=\"" + v + "\"")
+                exec(k + '="' + v + '"')
         for k, v in fields.items():
             if v is not None:
                 exec(k + "=" + str(v))
         return eval(filter)
     except Exception:
         return False
 
 
 def get_tags_fields(row):
-    '''
+    """
     Retrieves tags and fields from the row dict.
-    '''
-    tags = {k: str(v).replace('\n', ' ')
-            for k, v in row.items() if not (is_number(v))}
+    """
+    tags = {k: str(v).replace("\n", " ") for k, v in row.items() if not (is_number(v))}
     fields = {k: float(v) for k, v in row.items() if is_number(v)}
     return tags, fields
 
 
 def normalize(header, preserve_orig_header):
-    '''
+    """
     Normalizes the header, i.e. replaces dots with underscores.
-    '''
+    """
     if not preserve_orig_header:
         return header.replace(".", "_")
     return header
 
 
 def int_or_float_or_str(v):
-    '''
+    """
     Converts the value to int or float. If this is not possible, then it returns
     the original value.
-    '''
+    """
     if isinstance(v, str):
         try:
             return int(v)
         except:
             try:
                 return float(v)
             except Exception:
                 return v
     else:
         return v
 
 
 def cleanhtml(html_string):
-    '''
+    """
     Removes html markup from the string.
-    '''
-    return re.sub(CLEANR, '', html_string)
+    """
+    return re.sub(CLEANR, "", html_string)
 
 
-class DmsCollector():
-    '''
+class DmsCollector:
+    """
     The main DMS collector class that allows to retrieve a DMS table from DMS Spy application.
-    '''
+    """
 
-    def __init__(self, admin_url, username=None, password=None, basic_auth=False, file_cache=None, store_to_cache=False):
-        '''
+    def __init__(
+        self,
+        admin_url,
+        username=None,
+        password=None,
+        basic_auth=False,
+        file_cache=None,
+        store_to_cache=False,
+        read_timeout=TIMEOUT_READ,
+        connect_timeout=TIMEOUT_CONNECT,
+    ):
+        """
         Create the instance of dms collector with admin server url `admin_url` and authentication details `username` and `password`.
         When you connect to the DMS Spy running on FMW 11g, then you need to set the `basic_auth` to `True`.
-        '''
+        """
         self.logged_in = False
         self.session = requests.session()
         self.admin_url = admin_url
         self.username = username
         self.password = password
         self.basic_auth = basic_auth
         self.header_cache = {}
         self.file_cache = file_cache
         self.store_to_cache = store_to_cache
+        self.read_timeout = read_timeout
+        self.connect_timeout = connect_timeout
 
     def login(self):
-        '''
+        """
         Performs login to the DMS Spy application using the login form.
-        '''
-        headers = {"User-Agent": "dms-collector/%s" % __version__}
-        logindata = {"j_username": self.username,
-                     "j_password": self.password, "j_character_encoding": "UTF-8"}
-        r = self.session.post(DMSLOGIN_URL % (
-            self.admin_url), headers=headers, data=logindata, allow_redirects=True, verify=False)
+        """
+        headers = {"User-Agent": "dms-collector/%s" % dms_version()}
+        logindata = {
+            "j_username": self.username,
+            "j_password": self.password,
+            "j_character_encoding": "UTF-8",
+        }
+        r = self.session.post(
+            DMSLOGIN_URL % (self.admin_url),
+            headers=headers,
+            data=logindata,
+            allow_redirects=True,
+            verify=False,
+            timeout=(self.connect_timeout, self.read_timeout),
+        )
         r.raise_for_status()
         if len([x.url for x in r.history]) == 1:
             raise Exception("Wrong username or password. Login failed!")
         self.logged_in = True
 
     def call(self, url):
-        '''
+        """
         Sends HTTP GET at the specified `url` of the DMS Spy application. When the basic authentication
         is enabled, the username and password are added on the request.
-        '''
+        """
         if not self.logged_in and not self.basic_auth:
             self.login()
         if self.basic_auth and self.username is not None and self.password is not None:
-            r = self.session.get(url, auth=(self.username, self.password),
-                                 timeout=(TIMEOUT_CONNECT, TIMEOUT_READ), allow_redirects=True)
+            r = self.session.get(
+                url,
+                auth=(self.username, self.password),
+                timeout=(self.connect_timeout, self.read_timeout),
+                allow_redirects=True,
+            )
         else:
-            r = self.session.get(url, timeout=(
-                TIMEOUT_CONNECT, TIMEOUT_READ), allow_redirects=True)
+            r = self.session.get(
+                url,
+                timeout=(self.connect_timeout, self.read_timeout),
+                allow_redirects=True,
+            )
         r.raise_for_status()
         return r
 
     def retrieve_data(self, url, check_tbl_version=True):
-        '''
+        """
         Retrieves and parses DMS table data as XML.
-        '''
+        """
         r = self.call(url)
 
         # remove the default namespace if it exsits
         # dmss spy deployed to wls 12c uses default namespaces in TBML whereas previous version not
         xmlstring = r.text
-        xmlstring = re.sub(r'\sxmlns="[^"]+"', '', xmlstring, count=1)
+        xmlstring = re.sub(r'\sxmlns="[^"]+"', "", xmlstring, count=1)
         root = ET.fromstring(xmlstring)
         if not (check_tbl_version):
             tbml_version = root.get("version")
             if tbml_version not in TBML_VERSIONS:
-                raise Exception("Data retrieved are of not supported tbml version %s. Supported versions are: %s"
-                                % (tbml_version, ','.join(TBML_VERSIONS)))
+                raise Exception(
+                    "Data retrieved are of not supported tbml version %s. Supported versions are: %s"
+                    % (tbml_version, ",".join(TBML_VERSIONS))
+                )
         return root, xmlstring
 
     def table_file(self, table):
         if self.file_cache is not None:
             return os.path.join(self.file_cache, table)
         else:
             return None
 
     def get_header(self, table, check_tbl_version=True):
-        '''
+        """
         Retrieves a DMS table header. If the table does not exist then it raises an error.
-        '''
+        """
         if table not in self.header_cache:
             # try to retrieve the table from the file cache and write to the file cache if enabled
             root = None
             table_file = self.table_file(table)
             if table_file is not None and os.path.exists(table_file):
                 with open(table_file, "r") as r:
                     lines = r.readlines()
                 root = ET.fromstring("\n".join(lines))
             if root is None:
-                root, xmlstring = self.retrieve_data(DMSREQUEST_HEADER % (
-                    self.admin_url, table), check_tbl_version=check_tbl_version)
+                root, xmlstring = self.retrieve_data(
+                    DMSREQUEST_HEADER % (self.admin_url, table),
+                    check_tbl_version=check_tbl_version,
+                )
                 if table_file is not None and self.store_to_cache:
                     with open(table_file, "w") as w:
                         w.writelines(xmlstring)
 
             te = root.find("./table")
             if te is None or te.get("name") != table:
                 raise Exception(f"The table '{table}' does not exist!")
             cdef = root.findall(".//columndef")
             items = {}
             for x in cdef:
                 d = x.find("description")
-                items[x.get("name")] = cleanhtml(
-                    d.text).strip() if d is not None else "n/a"
+                items[x.get("name")] = cleanhtml(d.text).strip() if d is not None else "n/a"
             self.header_cache[table] = items
         return self.header_cache[table]
 
-    def collect(self, table, check_tbl_version=True, preserve_orig_header=False, include=[], exclude=[], filter=None):
-        '''
+    def collect(
+        self,
+        table,
+        check_tbl_version=True,
+        preserve_orig_header=False,
+        include=[],
+        exclude=[],
+        filter=None,
+    ):
+        """
         Retrieves the DMS table as a list of dict where a dict represents a row with fields and values.
         The `include` parameter provides a list of fields that should be included in the result, the `exclude` parameter
         provides a list of fields that should be excluded from the result and `filter` defines a Python expression
         that is used to filter our the table rows. The expression can contain conditions with table fields.
-        '''
+        """
         start_time = time.time()
 
         header = self.get_header(table, check_tbl_version)
-        root, _ = self.retrieve_data(DMSREQUEST_DATA % (
-            self.admin_url, table), check_tbl_version=check_tbl_version)
+        root, _ = self.retrieve_data(
+            DMSREQUEST_DATA % (self.admin_url, table),
+            check_tbl_version=check_tbl_version,
+        )
 
         rows = []
         for rw in root.findall(".//row"):
             row = {}
             for key in header.keys():
-                nkey = normalize(
-                    key, preserve_orig_header=preserve_orig_header)
+                nkey = normalize(key, preserve_orig_header=preserve_orig_header)
                 if (nkey not in exclude and len(include) == 0) or nkey in include:
                     cv = rw.find("./column[@name='%s']" % key)
                     if cv is not None and cv.text is not None:
-                        if cv.text.strip() != '':
+                        if cv.text.strip() != "":
                             row[nkey] = int_or_float_or_str(cv.text.strip())
                         else:
                             row[nkey] = None
                     else:
                         row[nkey] = None
 
             output_row = True
-            if filter is not None and filter.strip() != '':
+            if filter is not None and filter.strip() != "":
                 tags, fields = get_tags_fields(row)
                 output_row = eval_filter(filter, tags, fields)
 
             if output_row is True:
                 rows.append(row)
 
         return {
             "time": time.time(),
             "table": table,
             "url": DMSREQUEST_HEADER % (self.admin_url, table),
             "include": include,
             "exclude": exclude,
             "filter": filter,
-            "query_time": time.time()-start_time,
-            "data": rows
+            "query_time": time.time() - start_time,
+            "data": rows,
         }
```

### Comparing `dms-collector-2.0.2/dms_collector.egg-info/PKG-INFO` & `dms-collector-2.0.3/dms_collector.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,97 @@
 Metadata-Version: 2.1
 Name: dms-collector
-Version: 2.0.2
+Version: 2.0.3
 Summary: Oracle FMW DMS Spy collector utility
 Home-page: UNKNOWN
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
 License: UNKNOWN
-Description: # $ dms-collector
-        
-        DMS is a Weblogic Dynamic Monitoring Service providing a massive amount of sensors about Weblogic and application components performance.
-        It can be accessed in a number of ways, such as Weblogic Scripting Tool (wlst), Java API or DMS Spy application. DMS Spy is used to access DMS metric tables by using a browser while it also provides endpoints to retrieve metric tables in XML format.
-        
-        dms-collector is a Python utility that retrieves DMS metrics from Weblogic DMS Spy application. It provides an API to access DMS tables' data and a CLI to query the DMS and display the data in CSV.
-        
-        ## Installation
-        
-        You can install the dms-collector with pip as follows:
-        
-        ```
-        pip install dms-collector 
-        ``` 
-        
-        ## Usage
-        
-        You can use dms-collector CLI to query the DMS Spy running at `https://wls-domain` with username `weblogic` and password `password1` by running the following command: 
-        
-        ```
-        $ dms-collector --url https://wls-domain --connect weblogic/password1 --table JVM_Memory
-        datetime,timezone,Host,Parent,ServerName,pendingFinalization_value,verbose_value,Process,JVM,Name
-        "22-01-12 11:23:30",+0100,"domain-3.oraclevnc.com","/JVM/MxBeans","AdminServer",0,"TRUE","AdminServer:7101","JVM","memory"
-        "22-01-12 11:23:30",+0100,"fmw-poc-app10.oraclevcn.com","/JVM/MxBeans","soa_server2",0,"TRUE","soa_server2:8102","JVM","memory"
-        "22-01-12 11:23:30",+0100,"fmw-poc-app10.oraclevcn.com","/JVM/MxBeans","proc15010",0,"FALSE","machine2:15010","JVM","memory"
-        "22-01-12 11:23:30",+0100,"domain-3.oraclevcn.com","/JVM/MxBeans","proc69725",0,"FALSE","machine1:69725","JVM","memory"
-        ```
-        
-        ## CLI Options
-        
-        There are many options that you can use to control, for example, a number of calls the CLI will run, a delay between calls, fields to be included or excluded or rows to be filtered out in the result. 
-        
-        For the full list of options please run `dms-collector --help`. 
-        
-        ### Filtering 
-        
-        If you want to exclude certain fields from the output, such as `Process` and `Parent`, run the following command:
-        
-        ```
-        $ dms-collector --url https://wls-domain --connect weblogic/password1 --table JVM_Memory \
-          --exclude Process,Parent
-        ```
-        
-        If you want to only return rows that match a certain criteria, such as a server name, run the following command:
-        
-        ```
-        $ dms-collector --url https://wls-domain --connect weblogic/password1 --table JVM_Memory \
-          --filter "bool(re.match(r\"WLS_SOA[0-9]+\",str(ServerName)))"
-        ```
-        
-        The `--filter` parameter accepts any valid Python expression with variable names matching table's header names. You can use all header names regardless whether they are included or excluded from the output.   
-        
-        ### Timestamp and Timezone
-        
-        The dms-collector CLI adds two columns to the CSV output, namely `datetime` and `timezone`. This is the current local time when the data is retrieved from the DMS and changes with every iteration. You can change the field names for both columns by using `--datetimefield` and `--timezonefield` respectively as well as remove them from the output by using `--exclude` option.    
-        
-        ### Delay Time
-        
-        You can specify a number of seconds the dms-collector CLI should wait between iterations by using `--delay` parameter. Since reading the data may in some situations take more time to finish, the delay time needs to be adjusted so that dms-collector always retrieves the data at the same time and the overall running time can be determined. The time adjustment is however disabled when the time to retrieve the DMS data takes more than 2/3 of the delay time. You can disable the delay time adjustment by using `--nodelayadjust` or change the 2/3 limit by `--nodelayperc`.
-        
-        ### Login
-         
-        dms-collector uses DMS Spy login form by default. If you are collecting data from a DMS Spy of an earlier version such as FMW infrastructure 11g, you need to use `--basicauth` option which uses HTTP basic authentication.
-         
-        ## Changes over previous version 1.1
-        
-        The version 2.0+ introduces the following changes:
-        
-        *  It is now possible to use `dms-collector` as a Python module which provides [DmsCollector class](https://github.com/tomvit/dms-collector/blob/v2.0/dms_collector/dms.py) that you can integrate into your Python applications. 
-        
-        * Several command-line arguments were removed such as linux pipelines and emitting the events, DMS reset and time adjustments.  
-        
-        You can still access the previous version in [1.1 branch](https://github.com/tomvit/dms-collector/tree/v1.1).
-         
-        # License
-        
-        free and free as a bird
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.5.0
+Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+
+# $ dms-collector
+
+DMS is a Weblogic Dynamic Monitoring Service providing a massive amount of sensors about Weblogic and application components performance.
+It can be accessed in a number of ways, such as Weblogic Scripting Tool (wlst), Java API or DMS Spy application. DMS Spy is used to access DMS metric tables by using a browser while it also provides endpoints to retrieve metric tables in XML format.
+
+dms-collector is a Python utility that retrieves DMS metrics from Weblogic DMS Spy application. It provides an API to access DMS tables' data and a CLI to query the DMS and display the data in CSV.
+
+## Installation
+
+You can install the dms-collector with pip as follows:
+
+```
+pip install dms-collector 
+``` 
+
+## Usage
+
+You can use dms-collector CLI to query the DMS Spy running at `https://wls-domain` with username `weblogic` and password `password1` by running the following command: 
+
+```
+$ dms-collector --url https://wls-domain --connect weblogic/password1 --table JVM_Memory
+datetime,timezone,Host,Parent,ServerName,pendingFinalization_value,verbose_value,Process,JVM,Name
+"22-01-12 11:23:30",+0100,"domain-3.oraclevnc.com","/JVM/MxBeans","AdminServer",0,"TRUE","AdminServer:7101","JVM","memory"
+"22-01-12 11:23:30",+0100,"fmw-poc-app10.oraclevcn.com","/JVM/MxBeans","soa_server2",0,"TRUE","soa_server2:8102","JVM","memory"
+"22-01-12 11:23:30",+0100,"fmw-poc-app10.oraclevcn.com","/JVM/MxBeans","proc15010",0,"FALSE","machine2:15010","JVM","memory"
+"22-01-12 11:23:30",+0100,"domain-3.oraclevcn.com","/JVM/MxBeans","proc69725",0,"FALSE","machine1:69725","JVM","memory"
+```
+
+## CLI Options
+
+There are many options that you can use to control, for example, a number of calls the CLI will run, a delay between calls, fields to be included or excluded or rows to be filtered out in the result. 
+
+For the full list of options please run `dms-collector --help`. 
+
+### Filtering 
+
+If you want to exclude certain fields from the output, such as `Process` and `Parent`, run the following command:
+
+```
+$ dms-collector --url https://wls-domain --connect weblogic/password1 --table JVM_Memory \
+  --exclude Process,Parent
+```
+
+If you want to only return rows that match a certain criteria, such as a server name, run the following command:
+
+```
+$ dms-collector --url https://wls-domain --connect weblogic/password1 --table JVM_Memory \
+  --filter "bool(re.match(r\"WLS_SOA[0-9]+\",str(ServerName)))"
+```
+
+The `--filter` parameter accepts any valid Python expression with variable names matching table's header names. You can use all header names regardless whether they are included or excluded from the output.   
+
+### Timestamp and Timezone
+
+The dms-collector CLI adds two columns to the CSV output, namely `datetime` and `timezone`. This is the current local time when the data is retrieved from the DMS and changes with every iteration. You can change the field names for both columns by using `--datetimefield` and `--timezonefield` respectively as well as remove them from the output by using `--exclude` option.    
+
+### Delay Time
+
+You can specify a number of seconds the dms-collector CLI should wait between iterations by using `--delay` parameter. Since reading the data may in some situations take more time to finish, the delay time needs to be adjusted so that dms-collector always retrieves the data at the same time and the overall running time can be determined. The time adjustment is however disabled when the time to retrieve the DMS data takes more than 2/3 of the delay time. You can disable the delay time adjustment by using `--nodelayadjust` or change the 2/3 limit by `--nodelayperc`.
+
+### Login
+ 
+dms-collector uses DMS Spy login form by default. If you are collecting data from a DMS Spy of an earlier version such as FMW infrastructure 11g, you need to use `--basicauth` option which uses HTTP basic authentication.
+ 
+## Changes over previous version 1.1
+
+The version 2.0+ introduces the following changes:
+
+*  It is now possible to use `dms-collector` as a Python module which provides [DmsCollector class](https://github.com/tomvit/dms-collector/blob/v2.0/dms_collector/dms.py) that you can integrate into your Python applications. 
+
+* Several command-line arguments were removed such as linux pipelines and emitting the events, DMS reset and time adjustments.  
+
+You can still access the previous version in [1.1 branch](https://github.com/tomvit/dms-collector/tree/v1.1).
+ 
+# License
+
+free and free as a bird
+
+
```

### Comparing `dms-collector-2.0.2/setup.py` & `dms-collector-2.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,50 +11,54 @@
 import sys
 import argparse
 import glob
 
 from setuptools import find_packages
 from setuptools import setup
 
+
 # read file content
 def read(*parts):
     path = os.path.join(os.path.dirname(__file__), *parts)
-    with codecs.open(path, encoding='utf-8') as fobj:
+    with codecs.open(path, encoding="utf-8") as fobj:
         return fobj.read()
 
-# finds the version of the package 
+
+# finds the version of the package
 def find_version(*file_paths):
     version_file = read(*file_paths)
-    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]",
-                              version_file, re.M)
+    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M)
     if version_match:
         return version_match.group(1)
     raise RuntimeError("Unable to find version string.")
-        
-# setup main 
+
+
+# setup main
 # required modules
-install_requires = [
-    'urllib3==1.26.8',
-    'requests==2.27.1']
+install_requires = ["urllib3>=2.0.2", "requests>=2.31.0", "setuptools_scm>=6.3.2"]
 
 setup(
-    name='dms-collector',
-    version=find_version("dms_collector", "__init__.py"),
-    description='Oracle FMW DMS Spy collector utility',
-    long_description=read('README.md'),
-    long_description_content_type='text/markdown',
-    author='Tomas Vitvar',
-    author_email='tomas@vitvar.com',
-    packages=find_packages(exclude=['tests.*', 'tests']),
+    name="dms-collector",
+    use_scm_version={
+        "root": ".",
+        "relative_to": __file__,
+        "local_scheme": "node-and-timestamp",
+    },
+    description="Oracle FMW DMS Spy collector utility",
+    long_description=read("README.md"),
+    long_description_content_type="text/markdown",
+    author="Tomas Vitvar",
+    author_email="tomas@vitvar.com",
+    packages=find_packages(exclude=["tests.*", "tests"]),
     include_package_data=True,
     install_requires=install_requires,
-    python_requires='>=3.5.0',
-    scripts=['bin/dms-collector'],
+    python_requires=">=3.6.0",
+    scripts=["bin/dms-collector"],
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Environment :: Console',
-        'Intended Audience :: Developers',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-    ]
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Console",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+    ],
 )
```

