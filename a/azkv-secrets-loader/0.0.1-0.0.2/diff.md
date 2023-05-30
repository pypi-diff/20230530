# Comparing `tmp/azkv-secrets-loader-0.0.1.tar.gz` & `tmp/azkv-secrets-loader-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azkv-secrets-loader-0.0.1.tar", last modified: Tue May 30 21:35:53 2023, max compression
+gzip compressed data, was "azkv-secrets-loader-0.0.2.tar", last modified: Tue May 30 21:38:56 2023, max compression
```

## Comparing `azkv-secrets-loader-0.0.1.tar` & `azkv-secrets-loader-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 21:35:53.670069 azkv-secrets-loader-0.0.1/
--rw-rw-rw-   0        0        0      558 2023-05-30 21:35:53.668820 azkv-secrets-loader-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-30 16:51:04.000000 azkv-secrets-loader-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 21:35:53.665084 azkv-secrets-loader-0.0.1/azkv_secrets_loader.egg-info/
--rw-rw-rw-   0        0        0      558 2023-05-30 21:35:53.000000 azkv-secrets-loader-0.0.1/azkv_secrets_loader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-05-30 21:35:53.000000 azkv-secrets-loader-0.0.1/azkv_secrets_loader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 21:35:53.000000 azkv-secrets-loader-0.0.1/azkv_secrets_loader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-30 21:35:53.000000 azkv-secrets-loader-0.0.1/azkv_secrets_loader.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 21:35:53.000000 azkv-secrets-loader-0.0.1/azkv_secrets_loader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 21:35:53.670069 azkv-secrets-loader-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-05-30 21:35:27.000000 azkv-secrets-loader-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 21:38:56.009380 azkv-secrets-loader-0.0.2/
+-rw-rw-rw-   0        0        0      558 2023-05-30 21:38:56.009380 azkv-secrets-loader-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-30 16:51:04.000000 azkv-secrets-loader-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 21:38:56.008617 azkv-secrets-loader-0.0.2/azkv_secrets_loader.egg-info/
+-rw-rw-rw-   0        0        0      558 2023-05-30 21:38:55.000000 azkv-secrets-loader-0.0.2/azkv_secrets_loader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-05-30 21:38:55.000000 azkv-secrets-loader-0.0.2/azkv_secrets_loader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 21:38:55.000000 azkv-secrets-loader-0.0.2/azkv_secrets_loader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-30 21:38:55.000000 azkv-secrets-loader-0.0.2/azkv_secrets_loader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 21:38:55.000000 azkv-secrets-loader-0.0.2/azkv_secrets_loader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 21:38:56.009380 azkv-secrets-loader-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1007 2023-05-30 21:38:43.000000 azkv-secrets-loader-0.0.2/setup.py
```

### Comparing `azkv-secrets-loader-0.0.1/PKG-INFO` & `azkv-secrets-loader-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azkv-secrets-loader
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for loading Azure Key Vault Secrets.
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: azure,api,keyvault
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `azkv-secrets-loader-0.0.1/azkv_secrets_loader.egg-info/PKG-INFO` & `azkv-secrets-loader-0.0.2/azkv_secrets_loader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azkv-secrets-loader
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for loading Azure Key Vault Secrets.
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: azure,api,keyvault
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `azkv-secrets-loader-0.0.1/setup.py` & `azkv-secrets-loader-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A package for loading Azure Key Vault Secrets.'
 LONG_DESCRIPTION = 'A package for loading Azure Key Vault Secrets.'
 
 # Setting up
 setup(
     name="azkv-secrets-loader",
     version=VERSION,
     author="Richard",
     author_email="<rich_swainson@hotmail.co.uk>",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[
-        'azure-identity' 
-        'azure-keyvault-secrets'
+        'azure-identity' ,
+        'azure-keyvault-secrets',
         'azure-core'
     ],
     keywords=['azure', 'api', 'keyvault'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

