# Comparing `tmp/cdk-pgstac-4.0.0.tar.gz` & `tmp/cdk-pgstac-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-pgstac-4.0.0.tar", last modified: Tue Apr 25 14:43:16 2023, max compression
+gzip compressed data, was "cdk-pgstac-4.1.0.tar", last modified: Tue May 30 00:10:54 2023, max compression
```

## Comparing `cdk-pgstac-4.0.0.tar` & `cdk-pgstac-4.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/src/cdk_pgstac/
--rw-r--r--   0 runner    (1001) docker     (123)   123992 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/src/cdk_pgstac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/src/cdk_pgstac/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/src/cdk_pgstac/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   160948 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/src/cdk_pgstac/_jsii/cdk-pgstac@4.0.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:43:05.000000 cdk-pgstac-4.0.0/src/cdk_pgstac/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:16.476083 cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-25 14:43:15.000000 cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-25 14:43:16.000000 cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:43:15.000000 cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 14:43:16.000000 cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 14:43:16.000000 cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/src/cdk_pgstac/
+-rw-r--r--   0 runner    (1001) docker     (123)   124828 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/src/cdk_pgstac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/src/cdk_pgstac/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/src/cdk_pgstac/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161106 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/src/cdk_pgstac/_jsii/cdk-pgstac@4.1.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:10:45.000000 cdk-pgstac-4.1.0/src/cdk_pgstac/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:10:54.343108 cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-30 00:10:53.000000 cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-30 00:10:54.000000 cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:10:53.000000 cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 00:10:54.000000 cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 00:10:54.000000 cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/top_level.txt
```

### Comparing `cdk-pgstac-4.0.0/LICENSE` & `cdk-pgstac-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-pgstac-4.0.0/PKG-INFO` & `cdk-pgstac-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pgstac
-Version: 4.0.0
+Version: 4.1.0
 Summary: A set of constructs deploying pgSTAC with CDK
 Home-page: https://github.com/developmentseed/cdk-pgstac.git
 Author: Anthony Lukach<anthony@developmentseed.org>
 License: ISC
 Project-URL: Source, https://github.com/developmentseed/cdk-pgstac.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-pgstac-4.0.0/README.md` & `cdk-pgstac-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-pgstac-4.0.0/setup.py` & `cdk-pgstac-4.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-pgstac",
-    "version": "4.0.0",
+    "version": "4.1.0",
     "description": "A set of constructs deploying pgSTAC with CDK",
     "license": "ISC",
     "url": "https://github.com/developmentseed/cdk-pgstac.git",
     "long_description_content_type": "text/markdown",
     "author": "Anthony Lukach<anthony@developmentseed.org>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_pgstac",
         "cdk_pgstac._jsii"
     ],
     "package_data": {
         "cdk_pgstac._jsii": [
-            "cdk-pgstac@4.0.0.jsii.tgz"
+            "cdk-pgstac@4.1.0.jsii.tgz"
         ],
         "cdk_pgstac": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-pgstac-4.0.0/src/cdk_pgstac/__init__.py` & `cdk-pgstac-4.1.0/src/cdk_pgstac/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 import aws_cdk
 import aws_cdk.aws_apigateway
 import aws_cdk.aws_dynamodb
 import aws_cdk.aws_ec2
 import aws_cdk.aws_iam
 import aws_cdk.aws_kms
+import aws_cdk.aws_lambda_python_alpha
 import aws_cdk.aws_logs
 import aws_cdk.aws_rds
 import aws_cdk.aws_s3
 import aws_cdk.aws_secretsmanager
 import constructs
 
 
@@ -170,23 +171,23 @@
 
     **Setting up an SSH tunnel**
 
     In your ``~/.ssh/config`` file, add an entry like::
 
        Host db-tunnel
        Hostname {the-bastion-host-address}
-       LocalForward 54322 {the-db-hostname}:5432
+       LocalForward 9999 {the-db-hostname}:5432
 
     Then a tunnel can be opened via::
 
        ssh -N db-tunnel
 
     And a connection to the DB can be made via::
 
-       psql -h 127.0.0.1 -p 5433 -U {username} -d {database}
+       psql -h 127.0.0.1 -p 9999 -U {username} -d {database}
 
     **Handling ``REMOTE HOST IDENTIFICATION HAS CHANGED!`` error**
 
     If you've redeployed a bastion host that you've previously connected to, you may see an error like::
 
     :stability: experimental
     ::
@@ -838,14 +839,34 @@
     @jsii.member(jsii_name="url")
     def url(self) -> builtins.str:
         '''
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "url"))
 
+    @builtins.property
+    @jsii.member(jsii_name="stacApiLambdaFunction")
+    def stac_api_lambda_function(
+        self,
+    ) -> aws_cdk.aws_lambda_python_alpha.PythonFunction:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(aws_cdk.aws_lambda_python_alpha.PythonFunction, jsii.get(self, "stacApiLambdaFunction"))
+
+    @stac_api_lambda_function.setter
+    def stac_api_lambda_function(
+        self,
+        value: aws_cdk.aws_lambda_python_alpha.PythonFunction,
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(PgStacApiLambda, "stac_api_lambda_function").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "stacApiLambdaFunction", value)
+
 
 @jsii.data_type(
     jsii_type="cdk-pgstac.PgStacApiLambdaProps",
     jsii_struct_bases=[],
     name_mapping={
         "db": "db",
         "db_secret": "dbSecret",
```

### Comparing `cdk-pgstac-4.0.0/src/cdk_pgstac.egg-info/PKG-INFO` & `cdk-pgstac-4.1.0/src/cdk_pgstac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pgstac
-Version: 4.0.0
+Version: 4.1.0
 Summary: A set of constructs deploying pgSTAC with CDK
 Home-page: https://github.com/developmentseed/cdk-pgstac.git
 Author: Anthony Lukach<anthony@developmentseed.org>
 License: ISC
 Project-URL: Source, https://github.com/developmentseed/cdk-pgstac.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

