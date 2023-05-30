# Comparing `tmp/software_mentions_client-0.1.6.tar.gz` & `tmp/software_mentions_client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "software_mentions_client-0.1.6.tar", last modified: Tue Mar  7 19:02:22 2023, max compression
+gzip compressed data, was "software_mentions_client-0.1.7.tar", last modified: Tue May 30 14:16:17 2023, max compression
```

## Comparing `software_mentions_client-0.1.6.tar` & `software_mentions_client-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-03-07 19:02:22.219028 software_mentions_client-0.1.6/
--rwxrwxr-x   0 lopez     (1000) lopez     (1000)    11184 2023-03-07 10:52:06.000000 software_mentions_client-0.1.6/LICENSE
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      112 2023-03-07 19:00:06.000000 software_mentions_client-0.1.6/MANIFEST.in
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     7106 2023-03-07 19:02:22.219028 software_mentions_client-0.1.6/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     6548 2023-03-07 18:35:07.000000 software_mentions_client-0.1.6/Readme.md
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      504 2023-03-07 18:31:51.000000 software_mentions_client-0.1.6/config.json
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       33 2021-08-08 01:18:57.000000 software_mentions_client-0.1.6/requirements.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-03-07 19:02:22.219028 software_mentions_client-0.1.6/setup.cfg
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      898 2023-03-07 19:01:14.000000 software_mentions_client-0.1.6/setup.py
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-03-07 19:02:22.219028 software_mentions_client-0.1.6/software_mentions_client/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     2908 2022-02-17 14:19:32.000000 software_mentions_client-0.1.6/software_mentions_client/S3.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2022-02-17 14:19:32.000000 software_mentions_client-0.1.6/software_mentions_client/__init__.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    35651 2023-03-07 18:38:07.000000 software_mentions_client-0.1.6/software_mentions_client/client.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     3620 2022-02-17 14:19:32.000000 software_mentions_client-0.1.6/software_mentions_client/consistency_check.py
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-03-07 19:02:22.219028 software_mentions_client-0.1.6/software_mentions_client/resources/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     3605 2021-08-30 13:06:10.000000 software_mentions_client-0.1.6/software_mentions_client/resources/covid_blacklist.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     3191 2021-08-08 01:18:57.000000 software_mentions_client-0.1.6/software_mentions_client/resources/stopwords_en.txt
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-03-07 19:02:22.219028 software_mentions_client-0.1.6/software_mentions_client.egg-info/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     7106 2023-03-07 19:02:22.000000 software_mentions_client-0.1.6/software_mentions_client.egg-info/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      562 2023-03-07 19:02:22.000000 software_mentions_client-0.1.6/software_mentions_client.egg-info/SOURCES.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-03-07 19:02:22.000000 software_mentions_client-0.1.6/software_mentions_client.egg-info/dependency_links.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       34 2023-03-07 19:02:22.000000 software_mentions_client-0.1.6/software_mentions_client.egg-info/requires.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       25 2023-03-07 19:02:22.000000 software_mentions_client-0.1.6/software_mentions_client.egg-info/top_level.txt
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-05-30 14:16:17.021753 software_mentions_client-0.1.7/
+-rwxrwxr-x   0 lopez     (1000) lopez     (1000)    11184 2023-03-07 10:52:06.000000 software_mentions_client-0.1.7/LICENSE
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      112 2023-03-07 19:00:06.000000 software_mentions_client-0.1.7/MANIFEST.in
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     7215 2023-05-30 14:16:17.021753 software_mentions_client-0.1.7/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     6694 2023-05-22 13:05:07.000000 software_mentions_client-0.1.7/Readme.md
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      504 2023-03-07 18:31:51.000000 software_mentions_client-0.1.7/config.json
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       33 2023-05-30 14:14:03.000000 software_mentions_client-0.1.7/requirements.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-05-30 14:16:17.021753 software_mentions_client-0.1.7/setup.cfg
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      921 2023-05-30 14:14:40.000000 software_mentions_client-0.1.7/setup.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-05-30 14:16:17.021753 software_mentions_client-0.1.7/software_mentions_client/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     2908 2022-02-17 14:19:32.000000 software_mentions_client-0.1.7/software_mentions_client/S3.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2022-02-17 14:19:32.000000 software_mentions_client-0.1.7/software_mentions_client/__init__.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    52167 2023-05-30 13:10:19.000000 software_mentions_client-0.1.7/software_mentions_client/client.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     3620 2022-02-17 14:19:32.000000 software_mentions_client-0.1.7/software_mentions_client/consistency_check.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-05-30 14:16:17.021753 software_mentions_client-0.1.7/software_mentions_client/resources/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     3605 2021-08-30 13:06:10.000000 software_mentions_client-0.1.7/software_mentions_client/resources/covid_blacklist.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     3191 2021-08-08 01:18:57.000000 software_mentions_client-0.1.7/software_mentions_client/resources/stopwords_en.txt
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-05-30 14:16:17.021753 software_mentions_client-0.1.7/software_mentions_client.egg-info/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     7215 2023-05-30 14:16:16.000000 software_mentions_client-0.1.7/software_mentions_client.egg-info/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      562 2023-05-30 14:16:16.000000 software_mentions_client-0.1.7/software_mentions_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-05-30 14:16:16.000000 software_mentions_client-0.1.7/software_mentions_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       34 2023-05-30 14:16:16.000000 software_mentions_client-0.1.7/software_mentions_client.egg-info/requires.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       25 2023-05-30 14:16:16.000000 software_mentions_client-0.1.7/software_mentions_client.egg-info/top_level.txt
```

### Comparing `software_mentions_client-0.1.6/LICENSE` & `software_mentions_client-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.6/PKG-INFO` & `software_mentions_client-0.1.7/Readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: software_mentions_client
-Version: 0.1.6
-Summary: A client for extracting software mentions in scholar publications
-Home-page: https://github.com/kermitt2/software_mentions_client
-Author: Patrice Lopez
-Author-email: patrice.lopez@science-miner.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.5
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Softcite software mention recognizer client
 
 [![PyPI version](https://badge.fury.io/py/software_mentions_client.svg)](https://badge.fury.io/py/software_mentions_client)
 [![License](http://img.shields.io/:license-apache-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)
 
 Python client for using the Softcite software mention recognition service. It can be applied to 
 
@@ -59,45 +43,45 @@
 > python3 -m pip install -e .
 ```
 
 
 ## Usage and options
 
 ```
-usage: python3 -m software_mentions_client.client [-h] [--repo-in REPO_IN] [--file-in FILE_IN]
-                                  [--file-out FILE_OUT]
-                                  [--data-path DATA_PATH] [--config CONFIG]
-                                  [--reprocess] [--reset] [--load]
-                                  [--diagnostic] [--scorched-earth]
+usage: client.py [-h] [--repo-in REPO_IN] [--file-in FILE_IN] [--file-out FILE_OUT]
+                 [--data-path DATA_PATH] [--config CONFIG] [--reprocess] [--reset] [--load]
+                 [--diagnostic-mongo] [--diagnostic-files] [--scorched-earth]
 
 Softcite software mention recognizer client
 
 optional arguments:
   -h, --help            show this help message and exit
-  --repo-in REPO_IN     path to a directory of PDF files to be processed by
-                        the Softcite software mention recognizer
-  --file-in FILE_IN     a single PDF input file to be processed by the
-                        Softcite software mention recognizer
-  --file-out FILE_OUT   path to a single output the software mentions in JSON
-                        format, extracted from the PDF file-in
+  --repo-in REPO_IN     path to a directory of PDF files to be processed by the Softcite
+                        software mention recognizer
+  --file-in FILE_IN     a single PDF input file to be processed by the Softcite software
+                        mention recognizer
+  --file-out FILE_OUT   path to a single output the software mentions in JSON format, extracted
+                        from the PDF file-in
   --data-path DATA_PATH
-                        path to the resource files created/harvested by
-                        biblio-glutton-harvester
+                        path to the resource files created/harvested by biblio-glutton-
+                        harvester
   --config CONFIG       path to the config file, default is ./config.json
   --reprocess           reprocessed failed PDF
-  --reset               ignore previous processing states and re-init the
-                        annotation process from the beginning
-  --load                load json files into the MongoDB instance, the --repo-
-                        in parameter must indicate the path to the directory
-                        of resulting json files to be loaded
-  --diagnostic          perform a full count of annotations and diagnostic
-                        using MongoDB regarding the harvesting and
-                        transformation process
-  --scorched-earth      remove a PDF file after its successful processing in
-                        order to save storage space, careful with this!
+  --reset               ignore previous processing states and re-init the annotation process
+                        from the beginning
+  --load                load json files into the MongoDB instance, the --repo-in or --data-path
+                        parameter must indicate the path to the directory of resulting json
+                        files to be loaded, --dump must indicate the path to the json dump file
+                        of document metadata
+  --diagnostic-mongo    perform a full count of annotations and diagnostic using MongoDB
+                        regarding the harvesting and annotation process
+  --diagnostic-files    perform a full count of annotations and diagnostic using repository
+                        files regarding the harvesting and annotation process
+  --scorched-earth      remove a PDF file after its sucessful processing in order to save
+                        storage space, careful with this!
 ```
 
 The logs are written by default in a file `./client.log`, but the location of the logs can be changed in the configuration file (default `./config.json`).
 
 ### Processing local PDF files
 
 For processing a single file., the resulting json being written as file at the indicated output path:
@@ -143,9 +127,7 @@
 ## License and contact
 
 Distributed under [Apache 2.0 license](http://www.apache.org/licenses/LICENSE-2.0). The dependencies used in the project are either themselves also distributed under Apache 2.0 license or distributed under a compatible license. 
 
 If you contribute to Softcite software mention recognizer client project, you agree to share your contribution following these licenses. 
 
 Main author and contact: Patrice Lopez (<patrice.lopez@science-miner.com>)
-
-
```

### Comparing `software_mentions_client-0.1.6/Readme.md` & `software_mentions_client-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: software_mentions_client
+Version: 0.1.7
+Summary: A client for extracting software mentions in scholar publications
+Home-page: https://github.com/kermitt2/software_mentions_client
+Author: Patrice Lopez
+Author-email: patrice.lopez@science-miner.com
+Classifier: Programming Language :: Python :: 3.5
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Softcite software mention recognizer client
 
 [![PyPI version](https://badge.fury.io/py/software_mentions_client.svg)](https://badge.fury.io/py/software_mentions_client)
 [![License](http://img.shields.io/:license-apache-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)
 
 Python client for using the Softcite software mention recognition service. It can be applied to 
 
@@ -43,45 +57,45 @@
 > python3 -m pip install -e .
 ```
 
 
 ## Usage and options
 
 ```
-usage: python3 -m software_mentions_client.client [-h] [--repo-in REPO_IN] [--file-in FILE_IN]
-                                  [--file-out FILE_OUT]
-                                  [--data-path DATA_PATH] [--config CONFIG]
-                                  [--reprocess] [--reset] [--load]
-                                  [--diagnostic] [--scorched-earth]
+usage: client.py [-h] [--repo-in REPO_IN] [--file-in FILE_IN] [--file-out FILE_OUT]
+                 [--data-path DATA_PATH] [--config CONFIG] [--reprocess] [--reset] [--load]
+                 [--diagnostic-mongo] [--diagnostic-files] [--scorched-earth]
 
 Softcite software mention recognizer client
 
 optional arguments:
   -h, --help            show this help message and exit
-  --repo-in REPO_IN     path to a directory of PDF files to be processed by
-                        the Softcite software mention recognizer
-  --file-in FILE_IN     a single PDF input file to be processed by the
-                        Softcite software mention recognizer
-  --file-out FILE_OUT   path to a single output the software mentions in JSON
-                        format, extracted from the PDF file-in
+  --repo-in REPO_IN     path to a directory of PDF files to be processed by the Softcite
+                        software mention recognizer
+  --file-in FILE_IN     a single PDF input file to be processed by the Softcite software
+                        mention recognizer
+  --file-out FILE_OUT   path to a single output the software mentions in JSON format, extracted
+                        from the PDF file-in
   --data-path DATA_PATH
-                        path to the resource files created/harvested by
-                        biblio-glutton-harvester
+                        path to the resource files created/harvested by biblio-glutton-
+                        harvester
   --config CONFIG       path to the config file, default is ./config.json
   --reprocess           reprocessed failed PDF
-  --reset               ignore previous processing states and re-init the
-                        annotation process from the beginning
-  --load                load json files into the MongoDB instance, the --repo-
-                        in parameter must indicate the path to the directory
-                        of resulting json files to be loaded
-  --diagnostic          perform a full count of annotations and diagnostic
-                        using MongoDB regarding the harvesting and
-                        transformation process
-  --scorched-earth      remove a PDF file after its successful processing in
-                        order to save storage space, careful with this!
+  --reset               ignore previous processing states and re-init the annotation process
+                        from the beginning
+  --load                load json files into the MongoDB instance, the --repo-in or --data-path
+                        parameter must indicate the path to the directory of resulting json
+                        files to be loaded, --dump must indicate the path to the json dump file
+                        of document metadata
+  --diagnostic-mongo    perform a full count of annotations and diagnostic using MongoDB
+                        regarding the harvesting and annotation process
+  --diagnostic-files    perform a full count of annotations and diagnostic using repository
+                        files regarding the harvesting and annotation process
+  --scorched-earth      remove a PDF file after its sucessful processing in order to save
+                        storage space, careful with this!
 ```
 
 The logs are written by default in a file `./client.log`, but the location of the logs can be changed in the configuration file (default `./config.json`).
 
 ### Processing local PDF files
 
 For processing a single file., the resulting json being written as file at the indicated output path:
```

### Comparing `software_mentions_client-0.1.6/setup.py` & `software_mentions_client-0.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt', 'r') as f:
     reqs = f.readlines()
 
 setup(
     name="software_mentions_client",
-    version="0.1.6",
+    version="0.1.7",
     author="Patrice Lopez",
     author_email="patrice.lopez@science-miner.com",
     description="A client for extracting software mentions in scholar publications",
     long_description=open("Readme.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url='https://github.com/kermitt2/software_mentions_client',
-    packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
+    packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests", "my_config*", "*.log"]),
     python_requires='>=3.5',
     install_requires=reqs,
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3.5",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
```

### Comparing `software_mentions_client-0.1.6/software_mentions_client/S3.py` & `software_mentions_client-0.1.7/software_mentions_client/S3.py`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.6/software_mentions_client/client.py` & `software_mentions_client-0.1.7/software_mentions_client/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import shutil
 import json
 import pickle
 import lmdb
 import argparse
 import time
 import datetime
-from article_dataset_builder.S3 import S3
+import software_mentions_client.S3
 import concurrent.futures
 import requests
 import pymongo
 from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor, as_completed
 import hashlib
 import copyreg
 import types
@@ -25,14 +25,16 @@
 import pkgutil
 
 map_size = 100 * 1024 * 1024 * 1024 
 
 # default endpoint
 endpoint_pdf = 'service/annotateSoftwarePDF'
 endpoint_txt = 'service/annotateSoftwareText'
+endpoint_xml = 'service/annotateSoftwareXML'
+endpoint_tei = 'service/annotateSoftwareTEI'
 
 # default logging settings
 logging.basicConfig(filename='client.log', filemode='w', level=logging.DEBUG)
 
 class software_mentions_client(object):
     """
     Python client for using the Softcite software mention service. 
@@ -120,34 +122,38 @@
         envFilePath = os.path.join(self.config["data_path"], 'entries_software')
         self.env_software = lmdb.open(envFilePath, map_size=map_size)
 
         #envFilePath = os.path.join(self.config["data_path"], 'fail_software')
         #self.env_fail_software = lmdb.open(envFilePath, map_size=map_size)
 
     def annotate_directory(self, directory, force=False):
-        # recursive directory walk for all pdf documents
+        '''
+        recursive directory walk for processing in parallel all PDF and XML documents
+        '''
         pdf_files = []
         out_files = []
         full_records = []
         nb_total = 0
         start_time = time.time()
 
         print("\n")
-        sys.stdout.write("\rtotal process: " + str(nb_total) + " - accumulated runtime: 0 s - 0 PDF/s")
+        sys.stdout.write("\rtotal process: " + str(nb_total) + " - accumulated runtime: 0 s - 0 files/s")
         sys.stdout.flush()
 
         for root, directories, filenames in os.walk(directory):
             for filename in filenames:
-                if filename.endswith(".pdf") or filename.endswith(".PDF") or filename.endswith(".pdf.gz"):
+                if filename.endswith(".pdf") or filename.endswith(".PDF") or filename.endswith(".pdf.gz") or filename.endswith(".xml"):
                     if filename.endswith(".pdf"):
                         filename_json = filename.replace(".pdf", ".software.json")
                     elif filename.endswith(".pdf.gz"):
                         filename_json = filename.replace(".pdf.gz", ".software.json")
                     elif filename.endswith(".PDF"):
                         filename_json = filename.replace(".PDF", ".software.json")
+                    elif filename.endswith(".xml"):
+                        filename_json = filename.replace(".xml", ".software.json")
 
                     sha1 = getSHA1(os.path.join(root,filename))
 
                     # if the json file already exists and not force, we skip 
                     if os.path.isfile(os.path.join(root, filename_json)) and not force:
                         # check that this id is considered in the lmdb keeping track of the process
                         with self.env_software.begin() as txn:
@@ -173,25 +179,29 @@
                     if len(pdf_files) == self.config["batch_size"]:
                         self.annotate_batch(pdf_files, out_files, full_records)
                         nb_total += len(pdf_files)
                         pdf_files = []
                         out_files = []
                         full_records = []
                         runtime = round(time.time() - start_time, 3)
-                        sys.stdout.write("\rtotal process: " + str(nb_total) + " - accumulated runtime: " + str(runtime) + " s - " + str(round(nb_total/runtime, 2)) + " PDF/s  ")
+                        sys.stdout.write("\rtotal process: " + str(nb_total) + " - accumulated runtime: " + str(runtime) + " s - " + str(round(nb_total/runtime, 2)) + " files/s  ")
                         sys.stdout.flush()
+
         # last batch
         if len(pdf_files) > 0:
             self.annotate_batch(pdf_files, out_files, full_records)
             nb_total += len(pdf_files)
             runtime = round(time.time() - start_time, 3)
-            sys.stdout.write("\rtotal process: " + str(nb_total) + " - accumulated runtime: " + str(runtime) + " s - " + str(round(nb_total/runtime, 2)) + " PDF/s  ")
+            sys.stdout.write("\rtotal process: " + str(nb_total) + " - accumulated runtime: " + str(runtime) + " s - " + str(round(nb_total/runtime, 2)) + " files/s  ")
             sys.stdout.flush()
 
     def annotate_collection(self, data_path, force=False):
+        '''
+        Annotate a collection harvested by biblio_glutton_harvester or article_dataset_builder, only PDF for the moment
+        '''
         # init lmdb transactions
         # open in read mode
         envFilePath = os.path.join(data_path, 'entries')
         self.env = lmdb.open(envFilePath, map_size=map_size)
 
         with self.env.begin(write=True) as txn:
             nb_total = txn.stat()['entries']
@@ -200,15 +210,15 @@
         # iterate over the entries in lmdb
         pdf_files = []
         out_files = []
         full_records = []
         nb_total = 0
         start_time = time.time()
 
-        sys.stdout.write("\rtotal process: " + str(nb_total) + " - accumulated runtime: 0 s - 0 PDF/s")
+        sys.stdout.write("\rtotal process: " + str(nb_total) + " - accumulated runtime: 0 s - 0 files/s")
         sys.stdout.flush()
 
         with self.env.begin(write=True) as txn:
             cursor = txn.cursor()
             for key, value in cursor:
                 local_entry = _deserialize_pickle(value)
                 local_entry["id"] = key.decode(encoding='UTF-8');
@@ -238,71 +248,141 @@
                 if len(pdf_files) == self.config["batch_size"]:
                     self.annotate_batch(pdf_files, out_files, full_records)
                     nb_total += len(pdf_files)
                     pdf_files = []
                     out_files = []
                     full_records = []
                     runtime = round(time.time() - start_time, 3)
-                    sys.stdout.write("\rtotal process: " + str(nb_total) + " - accumulated runtime: " + str(runtime) + " s - " + str(round(nb_total/runtime, 2)) + " PDF/s  ")
+                    sys.stdout.write("\rtotal process: " + str(nb_total) + " - accumulated runtime: " + str(runtime) + " s - " + str(round(nb_total/runtime, 2)) + " files/s  ")
                     sys.stdout.flush()
 
         # last batch
         if len(pdf_files) > 0:
             self.annotate_batch(pdf_files, out_files, full_records)
             runtime = round(time.time() - start_time, 3)
-            sys.stdout.write("\rtotal process: " + str(nb_total) + " - accumulated runtime: " + str(runtime) + " s - " + str(round(nb_total/runtime, 2)) + " PDF/s  ")
+            sys.stdout.write("\rtotal process: " + str(nb_total) + " - accumulated runtime: " + str(runtime) + " s - " + str(round(nb_total/runtime, 2)) + " files/s  ")
             sys.stdout.flush()
 
     def annotate_batch(self, pdf_files, out_files=None, full_records=None):
         # process a provided list of PDF
         with ThreadPoolExecutor(max_workers=self.config["concurrency"]) as executor:
             #with ProcessPoolExecutor(max_workers=self.config["concurrency"]) as executor:
             # note: ProcessPoolExecutor will not work due to env objects that can't be serailized (e.g. LMDB variables)
             # client is not cpu bounded but io bounded, so normally it's still okay with threads and GIL
             executor.map(self.annotate, pdf_files, out_files, full_records, timeout=self.config["timeout"])
 
-    def reprocess_failed(self):
+    def reprocess_failed(self, directory):
         """
         we reprocess only files which have led to a failure of the service, we don't reprocess documents
         where no software mention has been found 
         """
         pdf_files = []
         out_files = []
         full_records = []
         i = 0
         nb_total = 0
-        with self.env_software.begin() as txn:
-            cursor = txn.cursor()
-            for key, value in cursor:
-                nb_total += 1
-                result = value.decode(encoding='UTF-8')
-                local_id = key.decode(encoding='UTF-8')
-                if result == "False":
-                    # reprocess
-                    logging.info("reprocess " + local_id)
-                    pdf_files.append(os.path.join(data_path, generateStoragePath(local_id), local_id, local_id+".pdf"))
-                    out_files.append(os.path.join(data_path, generateStoragePath(local_id), local_id, local_id+".software.json"))
-                    # get the full record from the data_path env
-                    json_file = os.path.join(data_path, generateStoragePath(local_id), local_id, local_id+".json")
-                    if os.path.isfile(json_file):
-                        with open(json_file) as f:
-                            full_record = json.load(f)
-                        full_records.append(full_record)
-                    i += 1
-
-            if i == self.config["batch_size"]:
-                self.annotate_batch(pdf_files, out_files, full_records)
-                pdf_files = []
-                out_files = []
-                full_records = []
-                i = 0
+        start_time = time.time()
+        if directory == None:
+            with self.env_software.begin() as txn:
+                cursor = txn.cursor()
+                for key, value in cursor:
+                    nb_total += 1
+                    result = value.decode(encoding='UTF-8')
+                    local_id = key.decode(encoding='UTF-8')
+                    if result == "False":
+                        # reprocess
+                        logging.info("reprocess " + local_id)
+
+                        input_file = os.path.join(data_path, generateStoragePath(local_id), local_id, local_id+".pdf")
+                        if os.path.exists(input_file):
+                            pdf_files.append(input_file)
+                        else:
+                            input_file = os.path.join(data_path, generateStoragePath(local_id), local_id, local_id+".tei.xml")
+                        if os.path.exists(input_file):
+                            pdf_files.append(input_file)
+                        else:
+                            input_file = os.path.join(data_path, generateStoragePath(local_id), local_id, local_id+".xml")
+                        if os.path.exists(input_file):
+                            pdf_files.append(input_file)
+                        # note: pdf.gz might be missing
+
+                        out_files.append(os.path.join(data_path, generateStoragePath(local_id), local_id, local_id+".software.json"))
+                        # get the full record from the data_path env
+                        json_file = os.path.join(data_path, generateStoragePath(local_id), local_id, local_id+".json")
+                        if os.path.isfile(json_file):
+                            with open(json_file) as f:
+                                full_record = json.load(f)
+                            full_records.append(full_record)
+                        i += 1
 
-        # last batch
+                    if i == self.config["batch_size"]:
+                        self.annotate_batch(pdf_files, out_files, full_records)
+                        nb_total += len(pdf_files)
+                        pdf_files = []
+                        out_files = []
+                        full_records = []
+                        i = 0
+                        sys.stdout.write("\rtotal reprocess: " + str(nb_total) + " - accumulated runtime: " + str(runtime) + " s - " + str(round(nb_total/runtime, 2)) + " files/s  ")
+                        sys.stdout.flush()
+        else:
+            for root, directories, filenames in os.walk(directory):
+                for filename in filenames:
+                    if filename.endswith(".pdf") or filename.endswith(".PDF") or filename.endswith(".pdf.gz") or filename.endswith(".xml"):
+                        if filename.endswith(".pdf"):
+                            filename_json = filename.replace(".pdf", ".software.json")
+                        elif filename.endswith(".pdf.gz"):
+                            filename_json = filename.replace(".pdf.gz", ".software.json")
+                        elif filename.endswith(".PDF"):
+                            filename_json = filename.replace(".PDF", ".software.json")
+                        elif filename.endswith(".xml"):
+                            filename_json = filename.replace(".xml", ".software.json")
+
+                        # if the json file already exists, we skip 
+                        if os.path.isfile(os.path.join(root, filename_json)):
+                            continue
+
+                        sha1 = getSHA1(os.path.join(root,filename))
+
+                        pdf_files.append(os.path.join(root,filename))
+                        out_files.append(os.path.join(root, filename_json))
+
+                        json_file = os.path.join(root, filename.replace(".xml", ".json"))
+                        if os.path.isfile(json_file):
+                            with open(json_file) as f:
+                                full_record = json.load(f)
+                            if full_record["id"] == sha1:
+                                full_records.append(full_record)
+                            else:
+                                record = {}
+                                record["id"] = sha1
+                                full_records.append(record)
+                        else:
+                            record = {}
+                            record["id"] = sha1
+                            full_records.append(record)
+                        i += 1
+
+                    if i == self.config["batch_size"]:
+                        self.annotate_batch(pdf_files, out_files, full_records)
+                        nb_total += len(pdf_files)
+                        pdf_files = []
+                        out_files = []
+                        full_records = []
+                        i = 0
+                        runtime = round(time.time() - start_time, 3)
+                        sys.stdout.write("\rtotal reprocess: " + str(nb_total) + " - accumulated runtime: " + str(runtime) + " s - " + str(round(nb_total/runtime, 2)) + " files/s  ")
+                        sys.stdout.flush()
+
+        # last batch for every cases
         if len(pdf_files) > 0:
             self.annotate_batch(pdf_files, out_files, full_records)
+            nb_total += len(pdf_files)
+            runtime = round(time.time() - start_time, 3)
+            sys.stdout.write("\rtotal reprocess: " + str(nb_total) + " - accumulated runtime: " + str(runtime) + " s - " + str(round(nb_total/runtime, 2)) + " files/s  ")
+            sys.stdout.flush()
 
         logging.info("re-processed: " + str(nb_total) + " entries")
 
     def reset(self):
         """
         Remove the local lmdb keeping track of the state of advancement of the annotation and
         of the failed entries
@@ -323,15 +403,15 @@
         if self.mongo_db == None:
             return
 
         failed = 0
         for root, directories, filenames in os.walk(directory):
             for filename in filenames: 
                 if filename.endswith(".software.json"):
-                    #print(os.path.join(root,filename))
+                    print(os.path.join(root,filename))
                     the_json = open(os.path.join(root,filename)).read()
                     try:
                         jsonObject = json.loads(the_json)
                     except:
                         print("the json parsing of the following file failed: ", os.path.join(root,filename))
                         continue
 
@@ -376,27 +456,37 @@
                                 failed += 1
                         else:
                             failed += 1
 
         print("number of glutton metadata lookup failed:", failed)
 
     def annotate(self, file_in, file_out, full_record):
+        url = self.config["software_mention_url"]
+        if not url.endswith("/"):
+            url += "/"
         try:
             if file_in.endswith('.pdf.gz'):
                 the_file = {'input': gzip.open(file_in, 'rb')}
-            else:
+                url += endpoint_pdf
+            elif file_in.endswith('.pdf') or file_in.endswith('.PDF'):
+                the_file = {'input': open(file_in, 'rb')}
+                url += endpoint_pdf
+            elif file_in.endswith('.tei.xml'):
                 the_file = {'input': open(file_in, 'rb')}
+                url += endpoint_tei
+            elif file_in.endswith('.xml'):
+                the_file = {'input': open(file_in, 'rb')}
+                # check if we have an XML file or a TEI file to select the best endpoint
+                if _is_tei(file_in):
+                    url += endpoint_tei
+                else:
+                    url += endpoint_xml
         except:
             logging.exception("input file appears invalid: " + file_in)
             return
-
-        url = self.config["software_mention_url"]
-        if not url.endswith("/"):
-            url += "/"
-        url += endpoint_pdf
         
         jsonObject = None
         try:
             response = requests.post(url, files=the_file, data = {'disambiguate': 1}, timeout=self.config["timeout"])
             if response.status_code == 503:
                 logging.info('service overloaded, sleep ' + str(self.config['sleep_time']) + ' seconds')
                 time.sleep(self.config['sleep_time'])
@@ -475,17 +565,19 @@
         if self.scorched_earth and jsonObject is not None:
             # processed is done, remove local PDF file
             try:
                 os.remove(file_in) 
             except:
                 logging.exception("Error while deleting file " + file_in)
 
-    def diagnostic(self, full_diagnostic=False):
+    def diagnostic(self, full_diagnostic_mongo=False, full_diagnostic_files=False, directory=None):
         """
-        Print a report on failures stored during the harvesting process
+        Print a report on annotation produced during the processing. If annotations are loaded
+        in MongoDB, use full_diagnostic_mongo=True to take advantage of mongodb queries.
+        Otherwise, the statistics will be produced using the files, which will be much slower. 
         """
         nb_total = 0
         nb_fail = 0
         nb_success = 0  
 
         with self.env_software.begin() as txn:
             cursor = txn.cursor()
@@ -501,15 +593,15 @@
         print("total entries:", nb_total)
         print("---")
         print("total successfully processed:", nb_success)
         print("---")
         print("total failed:", nb_fail)
         print("---")
 
-        if full_diagnostic:
+        if full_diagnostic_mongo:
             # check mongodb access - if mongodb is not used or available, we don't go further
             if self.mongo_db is None:
                 if "mongo_host" in self.config and len(self.config["mongo_host"].strip())>0:
                     mongo_client = pymongo.MongoClient(self.config["mongo_host"], int(self.config["mongo_port"]))
                     self.mongo_db = mongo_client[self.config["mongo_db"]]
 
             if self.mongo_db is None:
@@ -549,14 +641,217 @@
 
             result = self.mongo_db.references.find( {"tei": {"$regex": "PMID"}} )
             print("\t  * with PMID:", result.count())  
 
             result = self.mongo_db.references.find( {"tei": {"$regex": "PMC"}} )
             print("\t  * with PMC ID:", result.count())  
             print("---")
+        elif full_diagnostic_files:
+            # in this mode, we go through the produced json files to retrieve information
+            # this is slower but applies without loading annotations to mongodb
+
+            # for software
+            nb_ref = 0
+            nb_ref_marker = 0
+            nb_ref_with_doi = 0
+            nb_ref_with_pmid = 0
+            nb_ref_with_pmcid = 0
+
+            nb_software = 0
+            nb_publisher = 0
+            nb_url = 0
+            nb_version = 0
+            nb_language = 0
+            nb_environment = 0
+            nb_component = 0
+            nb_implicit = 0
+
+            nb_software_mention_with_ref = 0
+
+            nb_documents = 0
+            nb_documents_with_software = 0
+            nbSoftwareFiles = 0
+
+            # for datasets
+            nb_dataset_ref = 0
+            nb_dataset_ref_marker = 0
+            nb_dataset_ref_with_doi = 0
+            nb_dataset_ref_with_pmid = 0
+            nb_dataset_ref_with_pmcid = 0
+
+            nb_dataset_implicit = 0
+            nb_dataset_name = 0
+            nb_data_device = 0
+            nb_dataset_publisher = 0
+            nb_dataset_url = 0
+            nb_dataset_version = 0
+           
+            nb_dataset_mention_with_ref = 0
+
+            nb_dataset_documents = 0
+            nb_documents_with_dataset = 0
+            nbDatasetFiles = 0
+
+            for root, directories, filenames in os.walk(directory):
+                
+                for filename in filenames: 
+                    if filename.endswith(".software.json"):
+                        nb_documents += 1
+                        #print(os.path.join(root,filename))
+                        the_json = open(os.path.join(root,filename)).read()
+                        try:
+                            jsonObject = json.loads(the_json)
+                        except:
+                            print("the json parsing of the following file failed: ", os.path.join(root,filename))
+                            continue
+
+                        nbSoftwareFiles += 1
+
+                        if nbSoftwareFiles % 100 == 0:
+                            sys.stdout.write("\rFiles visited: %i" % nbSoftwareFiles)
+                            sys.stdout.flush()
+
+                        if "mentions" in jsonObject and len(jsonObject["mentions"])>0:
+                            nb_documents_with_software += 1
+
+                        for mention in jsonObject["mentions"]:
+                            if "type" in mention:
+                                if mention["type"] == "software":
+                                    nb_software += 1
+                            if "software-type" in mention:
+                                if mention["software-type"] == "environment":
+                                    nb_environment += 1
+                                elif mention["software-type"] == "implicit":
+                                    nb_implicit += 1
+                                elif mention["software-type"] == "component":
+                                    nb_component += 1
+
+                            if "publisher" in mention:
+                                nb_publisher += 1
+                            if "version" in mention:
+                                nb_version += 1
+                            if "language" in mention:
+                                nb_language += 1
+                            if "url" in mention:
+                                nb_url += 1
+
+                            if "references" in mention:
+                                nb_ref_marker += len(mention["references"])
+                                nb_software_mention_with_ref += 1
+
+                        if "references" in jsonObject and len(jsonObject["references"])>0:
+                            nb_ref += len(jsonObject["references"])
+
+                            # like with mongodb queries, we can use simple matching to count PID in full references
+                            for reference in jsonObject["references"]:
+                                if "tei" in reference:
+                                    reference_xml = reference["tei"]
+                                    if "DOI" in reference_xml:
+                                        nb_ref_with_doi += 1
+                                    if "PMID" in reference_xml:
+                                        nb_ref_with_pmid += 1
+                                    if "PMCID" in reference_xml:
+                                        nb_ref_with_pmcid += 1
+
+                    elif filename.endswith(".dataset.json"):
+                        nb_dataset_documents += 1
+                        #print(os.path.join(root,filename))
+                        the_json = open(os.path.join(root,filename)).read()
+                        try:
+                            jsonObject = json.loads(the_json)
+                        except:
+                            print("the json parsing of the following file failed: ", os.path.join(root,filename))
+                            continue
+
+                        nbDatasetFiles += 1
+
+                        if nbDatasetFiles % 100 == 0:
+                            sys.stdout.write("\rFiles visited: %i" % nbDatasetFiles)
+                            sys.stdout.flush()
+
+                        if "mentions" in jsonObject and len(jsonObject["mentions"])>0:
+                            nb_documents_with_dataset += 1
+
+                        for mention in jsonObject["mentions"]:
+                            if "type" in mention:
+                                if mention["type"] == "dataset-implicit":
+                                    nb_dataset_implicit += 1
+                                elif mention["type"] == "dataset-name":
+                                    nb_dataset_name += 1
+                            
+                            if mention["type"] == "data-device" or "data-device" in mention:
+                                nb_data_device += 1
+
+                            if "publisher" in mention:
+                                nb_dataset_publisher += 1
+                            if "version" in mention:
+                                nb_dataset_version += 1
+                            if "url" in mention:
+                                nb_dataset_url += 1
+
+                            if "references" in mention:
+                                nb_dataset_ref_marker += len(mention["references"])
+                                nb_dataset_mention_with_ref += 1
+
+                        if "references" in jsonObject and len(jsonObject["references"])>0:
+                            
+                            nb_dataset_ref += len(jsonObject["references"])
+
+                            # like with mongodb queries, we can use simple matching to count PID in full references
+                            for reference in jsonObject["references"]:
+                                if "tei" in reference:
+                                    reference_xml = reference["tei"]
+                                    if "DOI" in reference_xml:
+                                        nb_dataset_ref_with_doi += 1
+                                    if "PMID" in reference_xml:
+                                        nb_dataset_ref_with_pmid += 1
+                                    if "PMCID" in reference_xml:
+                                        nb_dataset_ref_with_pmcid += 1
+
+            # report results
+            if nb_documents > 0:
+                print("\n\n--- SOFTWARE MENTIONS ---") 
+                print("JSON files - number of documents: ", nb_documents)
+                print("JSON files - number of documents with at least one software mention: ", nb_documents_with_software)
+                print("JSON files - number of software mentions: ", nb_software)
+                nb_standalone = nb_software - (nb_environment + nb_component + nb_implicit)
+                print("\t     -> subtype standalone:", nb_standalone)
+                print("\t     -> subtype environment:", nb_environment)
+                print("\t     -> subtype component:", nb_component)
+                print("\t     -> subtype implicit:", nb_implicit)
+                print("\t     * with software name:", nb_software)
+                print("\t     * with version:", nb_version)
+                print("\t     * with publisher:", nb_publisher)
+                print("\t     * with url:", nb_url) 
+                print("\t     * with programming language:", nb_language) 
+                print("\t     * mentions with at least one reference", nb_software_mention_with_ref) 
+                print("---") 
+                print("JSON files - number of bibliographical reference markers: ", nb_ref_marker)
+                print("JSON files - number of bibliographical references: ", nb_ref)
+                print("\t      * with DOI:", nb_ref_with_doi)  
+                print("\t      * with PMID:", nb_ref_with_pmid)  
+                print("\t      * with PMC ID:", nb_ref_with_pmcid)  
+                print("---")              
+
+            if nb_dataset_documents > 0:
+                print("\n\n--- DATASET MENTIONS ---") 
+                print("JSON files - number of documents: ", nb_dataset_documents)
+                print("JSON files - number of documents with at least one dataset mention: ", nb_documents_with_dataset)
+                print("JSON files - number of named dataset mentions: ", nb_dataset_name)
+                print("JSON files - number of implicit dataset mentions: ", nb_dataset_implicit)
+                print("JSON files - number of data device mentions: ", nb_data_device)
+                print("\t     * with url:", nb_dataset_url) 
+                print("\t     * mentions with at least one reference", nb_dataset_mention_with_ref) 
+                print("---") 
+                print("JSON files - number of bibliographical reference markers: ", nb_dataset_ref_marker)
+                print("JSON files - number of bibliographical references: ", nb_dataset_ref)
+                print("\t      * with DOI:", nb_dataset_ref_with_doi)  
+                print("\t      * with PMID:", nb_dataset_ref_with_pmid)  
+                print("\t      * with PMC ID:", nb_dataset_ref_with_pmcid)  
+                print("---") 
 
     def _insert_mongo(self, jsonObject):
         if self.mongo_db is None:
             mongo_client = pymongo.MongoClient(self.config["mongo_host"], int(self.config["mongo_port"]))
             self.mongo_db = mongo_client[self.config["mongo_db"]]
 
         if self.mongo_db is None:
@@ -675,14 +970,25 @@
     if not isinstance(d, (dict, list)):
         return d
     if isinstance(d, list):
         return [_clean_json(v) for v in d]
     return {k: _clean_json(v) for k, v in d.items()
             if not k.startswith("$") }
 
+def _is_tei(the_file):
+    # based on the header content of the file, check if we have a TEI XML file
+    with open(the_file) as f:
+        n = 5
+        while n>=0:
+            first_line = f.readline().strip('\n')
+            if "<TEI " in first_line or "<tei " in first_line or "<teiCorpus " in first_line:
+                return True
+            n -= 1
+    return False
+
 BUF_SIZE = 65536    
 
 def getSHA1(the_file):
     sha1 = hashlib.sha1()
 
     with open(the_file, 'rb') as f:
         while True:
@@ -700,65 +1006,67 @@
     parser.add_argument("--file-out", default=None, help="path to a single output the software mentions in JSON format, extracted from the PDF file-in") 
     parser.add_argument("--data-path", default=None, help="path to the resource files created/harvested by biblio-glutton-harvester") 
     parser.add_argument("--config", default="./config.json", help="path to the config file, default is ./config.json") 
     parser.add_argument("--reprocess", action="store_true", help="reprocessed failed PDF") 
     parser.add_argument("--reset", action="store_true", help="ignore previous processing states and re-init the annotation process from the beginning") 
     parser.add_argument("--load", action="store_true", help="load json files into the MongoDB instance, the --repo-in or --data-path parameter must indicate the path "
         +"to the directory of resulting json files to be loaded, --dump must indicate the path to the json dump file of document metadata") 
-    parser.add_argument("--diagnostic", action="store_true", help="perform a full count of annotations and diagnostic using MongoDB "  
-        +"regarding the harvesting and transformation process") 
+    parser.add_argument("--diagnostic-mongo", action="store_true", help="perform a full count of annotations and diagnostic using MongoDB "  
+        +"regarding the harvesting and annotation process") 
+    parser.add_argument("--diagnostic-files", action="store_true", help="perform a full count of annotations and diagnostic using repository files "  
+        +"regarding the harvesting and annotation process") 
     parser.add_argument("--scorched-earth", action="store_true", help="remove a PDF file after its sucessful processing in order to save storage space" 
         +", careful with this!") 
 
     args = parser.parse_args()
 
     data_path = args.data_path
     config_path = args.config
     reprocess = args.reprocess
     reset = args.reset
     file_in = args.file_in
     file_out = args.file_out
     repo_in = args.repo_in
     load_mongo = args.load
-    full_diagnostic = args.diagnostic
+    full_diagnostic_mongo = args.diagnostic_mongo
+    full_diagnostic_files = args.diagnostic_files
     scorched_earth = args.scorched_earth
 
     client = software_mentions_client(config_path=config_path)
 
-    if not load_mongo and not full_diagnostic and not client.service_isalive():
+    if not load_mongo and not full_diagnostic_mongo and not full_diagnostic_files and not client.service_isalive():
         sys.exit("Softcite software mention service not available, leaving...")
 
     force = False
     if reset:
         client.reset()
         force = True
 
     if scorched_earth:
         client.scorched_earth = True
 
     if load_mongo:
-        if data_path is None:
-            data_path = client.config["data_path"] 
         # check a mongodb server is specified in the config
         if client.config["mongo_host"] is None:
             sys.exit("the mongodb server where to load the json files is not indicated in the config file, leaving...")
-        if repo_in is None and data_path is None: 
-            sys.exit("the repo_in where to find the PDF files to be processed is not indicated, leaving...")
-        if data_path is not None:
-            client.load_mongo(data_path)
-        elif repo_in is not None:
+
+        if repo_in is not None:
             client.load_mongo(repo_in)
+        elif data_path is None and len(client.config["data_path"])>0:
+            data_path = client.config["data_path"] 
+            if repo_in is None and (data_path is None or len(client.config["data_path"])==0): 
+                sys.exit("the repo_in where to find the PDF files to be processed is not indicated, leaving...")
+            if data_path is not None:
+                client.load_mongo(data_path)
+        
     elif reprocess:
-        client.reprocess_failed()
-    elif repo_in is not None: 
+        client.reprocess_failed(repo_in)
+    elif repo_in is not None and not full_diagnostic_files: 
         client.annotate_directory(repo_in, force)
     elif file_in is not None:
         client.annotate(file_in, file_out, None)
     elif data_path is not None: 
         client.annotate_collection(data_path, force)
 
-    if not full_diagnostic:
-        client.diagnostic(full_diagnostic=False)
-    else:
-        client.diagnostic(full_diagnostic=True)
+    client.diagnostic(full_diagnostic_mongo=full_diagnostic_mongo, full_diagnostic_files=full_diagnostic_files, directory=repo_in)
```

### Comparing `software_mentions_client-0.1.6/software_mentions_client/consistency_check.py` & `software_mentions_client-0.1.7/software_mentions_client/consistency_check.py`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.6/software_mentions_client/resources/covid_blacklist.txt` & `software_mentions_client-0.1.7/software_mentions_client/resources/covid_blacklist.txt`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.6/software_mentions_client/resources/stopwords_en.txt` & `software_mentions_client-0.1.7/software_mentions_client/resources/stopwords_en.txt`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.6/software_mentions_client.egg-info/PKG-INFO` & `software_mentions_client-0.1.7/software_mentions_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: software-mentions-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: A client for extracting software mentions in scholar publications
 Home-page: https://github.com/kermitt2/software_mentions_client
 Author: Patrice Lopez
 Author-email: patrice.lopez@science-miner.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -59,45 +57,45 @@
 > python3 -m pip install -e .
 ```
 
 
 ## Usage and options
 
 ```
-usage: python3 -m software_mentions_client.client [-h] [--repo-in REPO_IN] [--file-in FILE_IN]
-                                  [--file-out FILE_OUT]
-                                  [--data-path DATA_PATH] [--config CONFIG]
-                                  [--reprocess] [--reset] [--load]
-                                  [--diagnostic] [--scorched-earth]
+usage: client.py [-h] [--repo-in REPO_IN] [--file-in FILE_IN] [--file-out FILE_OUT]
+                 [--data-path DATA_PATH] [--config CONFIG] [--reprocess] [--reset] [--load]
+                 [--diagnostic-mongo] [--diagnostic-files] [--scorched-earth]
 
 Softcite software mention recognizer client
 
 optional arguments:
   -h, --help            show this help message and exit
-  --repo-in REPO_IN     path to a directory of PDF files to be processed by
-                        the Softcite software mention recognizer
-  --file-in FILE_IN     a single PDF input file to be processed by the
-                        Softcite software mention recognizer
-  --file-out FILE_OUT   path to a single output the software mentions in JSON
-                        format, extracted from the PDF file-in
+  --repo-in REPO_IN     path to a directory of PDF files to be processed by the Softcite
+                        software mention recognizer
+  --file-in FILE_IN     a single PDF input file to be processed by the Softcite software
+                        mention recognizer
+  --file-out FILE_OUT   path to a single output the software mentions in JSON format, extracted
+                        from the PDF file-in
   --data-path DATA_PATH
-                        path to the resource files created/harvested by
-                        biblio-glutton-harvester
+                        path to the resource files created/harvested by biblio-glutton-
+                        harvester
   --config CONFIG       path to the config file, default is ./config.json
   --reprocess           reprocessed failed PDF
-  --reset               ignore previous processing states and re-init the
-                        annotation process from the beginning
-  --load                load json files into the MongoDB instance, the --repo-
-                        in parameter must indicate the path to the directory
-                        of resulting json files to be loaded
-  --diagnostic          perform a full count of annotations and diagnostic
-                        using MongoDB regarding the harvesting and
-                        transformation process
-  --scorched-earth      remove a PDF file after its successful processing in
-                        order to save storage space, careful with this!
+  --reset               ignore previous processing states and re-init the annotation process
+                        from the beginning
+  --load                load json files into the MongoDB instance, the --repo-in or --data-path
+                        parameter must indicate the path to the directory of resulting json
+                        files to be loaded, --dump must indicate the path to the json dump file
+                        of document metadata
+  --diagnostic-mongo    perform a full count of annotations and diagnostic using MongoDB
+                        regarding the harvesting and annotation process
+  --diagnostic-files    perform a full count of annotations and diagnostic using repository
+                        files regarding the harvesting and annotation process
+  --scorched-earth      remove a PDF file after its sucessful processing in order to save
+                        storage space, careful with this!
 ```
 
 The logs are written by default in a file `./client.log`, but the location of the logs can be changed in the configuration file (default `./config.json`).
 
 ### Processing local PDF files
 
 For processing a single file., the resulting json being written as file at the indicated output path:
@@ -143,9 +141,7 @@
 ## License and contact
 
 Distributed under [Apache 2.0 license](http://www.apache.org/licenses/LICENSE-2.0). The dependencies used in the project are either themselves also distributed under Apache 2.0 license or distributed under a compatible license. 
 
 If you contribute to Softcite software mention recognizer client project, you agree to share your contribution following these licenses. 
 
 Main author and contact: Patrice Lopez (<patrice.lopez@science-miner.com>)
-
-
```

### Comparing `software_mentions_client-0.1.6/software_mentions_client.egg-info/SOURCES.txt` & `software_mentions_client-0.1.7/software_mentions_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

