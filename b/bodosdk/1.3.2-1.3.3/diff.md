# Comparing `tmp/bodosdk-1.3.2.tar.gz` & `tmp/bodosdk-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodosdk-1.3.2.tar", last modified: Wed May 17 14:40:47 2023, max compression
+gzip compressed data, was "bodosdk-1.3.3.tar", last modified: Tue May 30 20:55:17 2023, max compression
```

## Comparing `bodosdk-1.3.2.tar` & `bodosdk-1.3.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:47.969244 bodosdk-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-05-17 14:40:41.000000 bodosdk-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-17 14:40:41.000000 bodosdk-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    36149 2023-05-17 14:40:47.969244 bodosdk-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    35454 2023-05-17 14:40:41.000000 bodosdk-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:47.969244 bodosdk-1.3.2/bodosdk/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-17 14:40:47.969244 bodosdk-1.3.2/bodosdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:47.965243 bodosdk-1.3.2/bodosdk/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     8160 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    13828 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/request_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:47.969244 bodosdk-1.3.2/bodosdk/client/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6724 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    12094 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/client/workspace.py
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:47.969244 bodosdk-1.3.2/bodosdk/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1429 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3729 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    14489 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/job.py
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-05-17 14:40:41.000000 bodosdk-1.3.2/bodosdk/models/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 14:40:47.965243 bodosdk-1.3.2/bodosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    36149 2023-05-17 14:40:47.000000 bodosdk-1.3.2/bodosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-05-17 14:40:47.000000 bodosdk-1.3.2/bodosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 14:40:47.000000 bodosdk-1.3.2/bodosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-17 14:40:47.000000 bodosdk-1.3.2/bodosdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-17 14:40:47.000000 bodosdk-1.3.2/bodosdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-17 14:40:47.969244 bodosdk-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-05-17 14:40:41.000000 bodosdk-1.3.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    80044 2023-05-17 14:40:41.000000 bodosdk-1.3.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:17.471089 bodosdk-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-05-30 20:55:09.000000 bodosdk-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-30 20:55:09.000000 bodosdk-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    50452 2023-05-30 20:55:17.471089 bodosdk-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    49757 2023-05-30 20:55:09.000000 bodosdk-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:17.471089 bodosdk-1.3.3/bodosdk/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-30 20:55:17.471089 bodosdk-1.3.3/bodosdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:17.467089 bodosdk-1.3.3/bodosdk/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8160 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14676 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/request_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:17.467089 bodosdk-1.3.3/bodosdk/client/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6724 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13203 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/client/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:17.471089 bodosdk-1.3.3/bodosdk/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1411 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3729 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14785 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-05-30 20:55:09.000000 bodosdk-1.3.3/bodosdk/models/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:55:17.463089 bodosdk-1.3.3/bodosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    50452 2023-05-30 20:55:17.000000 bodosdk-1.3.3/bodosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-05-30 20:55:17.000000 bodosdk-1.3.3/bodosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 20:55:17.000000 bodosdk-1.3.3/bodosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-30 20:55:17.000000 bodosdk-1.3.3/bodosdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-30 20:55:17.000000 bodosdk-1.3.3/bodosdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-30 20:55:17.471089 bodosdk-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-05-30 20:55:09.000000 bodosdk-1.3.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    80044 2023-05-30 20:55:09.000000 bodosdk-1.3.3/versioneer.py
```

### Comparing `bodosdk-1.3.2/LICENSE` & `bodosdk-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/PKG-INFO` & `bodosdk-1.3.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 1.3.2
+Version: 1.3.3
 Summary: Bodo Platform SDK
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -73,22 +73,30 @@
 )
 client = get_bodo_client(keys, print_logs=True)
 ```
 
 ### Job resource<a id="job-resource"></a> 
 Module responsible for managing jobs in workspace.
 
-- [create job](#create-job)
-- [list jobs](#list-jobs)
-- [get job](#get-job)
-- [remove job](#remove-job)
-- [get execution info](#get-execution)
-- [waiter](#job-waiter)
 
-#### Create job<a id="create-job"></a>
+
+- [Bodo Platform Jobs](#bodo-platform-jobs)
+  - [create job](#create-job)
+  - [list jobs](#list-jobs)
+  - [get job](#get-job)
+  - [remove job](#remove-job)
+  - [get execution info](#get-execution)
+  - [waiter](#job-waiter)
+- [Bodo Platform Batch Jobs](#bodo-platform-batch-jobs)
+
+<br/>
+
+#### Bodo Platform Jobs<a id="bodo-platform-jobs"></a>
+
+##### Create job<a id="create-job"></a>
 
 `BodoClient.job.create(job: JobDefinition)`
 
 Creates a job to be executed on cluster. You can either create job dedicated cluster by providing its definition or
 provide existing cluster uuid. Job dedicated clusters will be removed as soon as job execution will finish, if you provide 
 uuid of existing one, cluster will remain.
 
@@ -258,15 +266,15 @@
     retries=0,
     retries_delay=0,
     retry_on_timeout=False
 )
 
 client.job.create(job_definition)
 ```
-#### List jobs<a id="list-jobs"></a>
+##### List jobs<a id="list-jobs"></a>
 
 `BodoClient.job.list()`
 
 Returns list of all jobs defined in workspace. 
 
 **Example:**
 
@@ -279,15 +287,15 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 jobs: List[JobResponse] = client.job.list()
 ```
 
-#### Get job<a id="get-job"></a>
+##### Get job<a id="get-job"></a>
 
 `BodoClient.job.get(job_uuid)`
 
 Returns specific job in workspace. Example:
 
 ```python
 from bodosdk.models import WorkspaceKeys, JobResponse
@@ -297,15 +305,15 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 job: JobResponse = client.job.get('8c32aec5-7181-45cc-9e17-8aff35fd269e')
 ```
 
-#### Remove job<a id="remove-job"></a>
+##### Remove job<a id="remove-job"></a>
 
 `BodoClient.job.delete(job_uuid)`
 
 Removes specific job from workspace. Example:
 
 ```python
 from bodosdk.models import WorkspaceKeys
@@ -315,15 +323,15 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 client.job.remove('8c32aec5-7181-45cc-9e17-8aff35fd269e')
 ```
 
-#### Get execution<a id="get-execution"></a>
+##### Get execution<a id="get-execution"></a>
 
 `BodoClient.job.get_job_executions(job_uuid)`
 
 Gets all executions info for specific job. Result it's a list with one element (in future we might extend it)
 
 ```python
 from bodosdk.models import WorkspaceKeys, JobExecution
@@ -334,15 +342,15 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 executions: List[JobExecution] = client.job.get_job_executions('8c32aec5-7181-45cc-9e17-8aff35fd269e')
 ```
 
-#### Job waiter<a id="job-waiter"></a>
+##### Job waiter<a id="job-waiter"></a>
 
 `BodoClient.job.get_waiter()`
 
 Get waiter object, which can be used to wait till job finish. Waiter has following method
 
 ```python3
 from typing import Callable
@@ -408,14 +416,512 @@
     print(f'Waiter timeout for {job_uuid}')
     return job_uuid
 
 
 result = waiter.wait('8c32aec5-7181-45cc-9e17-8aff35fd269e', on_timeout=timeout_callback, timeout=1)
 ```
 
+
+<br/>
+
+#### Bodo Platform Batch Jobs <a id="bodo-platform-batch-jobs"></a>
+
+##### Create batch job definition 
+
+`BodoClient.job.create_batch_job_definition(job_definition: CreateBatchJobDefinition)`
+
+Creates batch job definition in the given workspace. 
+
+- **Example 1: Create batch job definition for a workspace source script**
+
+    ```python
+    from bodosdk.models import WorkspaceKeys, CreateBatchJobDefinition, BatchJobDefinition
+    from bodosdk.client import get_bodo_client
+    from bodosdk.models.job import CreateBatchJobDefinition, JobConfig, JobSource, JobSourceType, SourceCodeType, \
+        WorkspaceDef, RetryStrategy
+  
+    keys = WorkspaceKeys(
+      client_id='XYZ',
+      secret_key='XYZ'
+    )
+    client = get_bodo_client(keys)
+    
+    workspace_source_def = JobSource(
+        type=JobSourceType.WORKSPACE,
+        definition=WorkspaceDef(
+            path="Example-path/batch-job-defs",
+        ),
+    )
+    
+    retry_strategy = RetryStrategy(
+        num_retries=1,
+        retry_on_timeout=False,
+        delay_between_retries=2,
+    )
+    
+    jobConfig = JobConfig(
+        source=workspace_source_def,
+        source_code_type=SourceCodeType.PYTHON,
+        sourceLocation="test.py",
+        args=None,
+        retry_strategy=retry_strategy,
+        timeout=10000,
+        env_vars=None,
+    )
+    
+    createBatchJobDef = CreateBatchJobDefinition(
+        name="test-job",
+        config=jobConfig,
+        description="test-batch-job-description-attempt",
+        cluster_config={
+            "bodoVersion": "2023.1.3",
+            "instance_type": "c5.2xlarge",
+            "workers_quantity": 2,
+            "accelerated_networking": False,
+        }, )
+    
+    jobdef = client.job.create_batch_job_definition(createBatchJobDef)
+    ```
+  
+
+- **Example 2: Create batch job definition for a git source script**
+
+  ```python
+  from bodosdk.models import WorkspaceKeys, CreateBatchJobDefinition, BatchJobDefinition
+  from bodosdk.client import get_bodo_client
+  from bodosdk.models.job import CreateBatchJobDefinition, JobConfig, JobSource, JobSourceType, SourceCodeType, \
+      WorkspaceDef, RetryStrategy
+    
+  keys = WorkspaceKeys(
+    client_id='XYZ',
+    secret_key='XYZ'
+  )
+  client = get_bodo_client(keys)
+    
+  git_source_def = JobSource(
+      type=JobSourceType.GIT,
+      definition=GitDef(
+          repo_url='https://github.com/Bodo-inc/Bodo-examples.git',
+          username='XYZ',
+          token='XYZ'
+      ),
+  )
+    
+  retry_strategy = RetryStrategy(
+      num_retries=1,
+      retry_on_timeout=False,
+      delay_between_retries=2,
+  )
+    
+  jobConfig = JobConfig(
+      source=git_source_def,
+      source_code_type=SourceCodeType.PYTHON,
+      sourceLocation="test.py",
+      args=None,
+      retry_strategy=retry_strategy,
+      timeout=10000,
+      env_vars=None,
+  )
+    
+  createBatchJobDef = CreateBatchJobDefinition(
+      name="test-job",
+      config=jobConfig,
+      description="test-batch-job-description-attempt",
+      cluster_config={
+          "bodoVersion": "2023.1.3",
+          "instance_type": "c5.2xlarge",
+          "workers_quantity": 2,
+          "accelerated_networking": False,
+      }, )
+    
+  jobdef = client.job.create_batch_job_definition(createBatchJobDef)  
+  ```
+  
+
+<br/>
+
+#####  List batch job definitions 
+
+`BodoClient.job.list_batch_job_definitions()`
+
+Lists all batch job definitions in the given workspace.
+
+**Example:**
+```python
+from typing import List
+
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobdefs: List[BatchJobDefinitionResponse] = client.job.list_batch_job_definitions()
+```
+
+
+<br/>
+
+#####  Get batch job definition by id
+
+`BodoClient.job.get_batch_job_definition(job_definition_id: str)`
+
+Gets specific batch job definition by id.
+
+**Example:**
+```python
+from typing import List
+
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobdef: BatchJobDefinitionResponse = client.job.get_batch_job_definition('04412S5b-300e-42db-84d4-5f22f7506594')
+```  
+
+<br/>
+
+##### Get batch job definition by name
+
+`BodoClient.job.get_batch_job_definition_by_name(name: str)`
+
+Gets specific batch job definition by id.
+
+**Example:**
+```python
+from typing import List
+
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobdef: BatchJobDefinitionResponse = client.job.get_batch_job_definition('04412S5b-300e-42db-84d4-5f22f7506594')
+```  
+  
+
+<br/>
+
+#####  Remove batch job definition 
+
+`BodoClient.job.remove_batch_job_definition(job_definition_id: str)`
+
+Removes specific batch job definition by id.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+client.job.remove_batch_job_definition('04412S5b-300e-42db-84d4-5f22f7506594')
+```
+
+
+<br/>
+
+#####  Submit a batch job run 
+
+`BodoClient.job.submit_batch_job_run(job_run: CreateJobRun)`
+
+Submits a job run for a given batch job definition.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+client.job.submit_batch_job_run(CreateJobRun(batchJobDefinitionUUID='04412S5b-300e-42db-84d4-5f22f7506594', clusterUUID='12936Q5z-109d-89yi-23c4-3d91u1219823'))
+```
+
+
+#####  List batch job runs 
+
+`BodoClient.job.list_batch_job_runs()`
+
+| Parameter         | Type                | Description                              | Required          |
+|-------------------|---------------------|------------------------------------------|-------------------|
+| `batch_job_id`    | `List[str]`         | List of Ids of the batch job definitions | No                |
+| `status`          | `List[JobRunStatus]`| List of Job Run Statuses                 | No                |
+| `cluster_id`      | `List[str]`         | List of Ids of the clusters              | No                |
+
+Lists all batch job runs in the given workspace filtered by given parameters.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobruns = client.job.list_batch_job_runs(status=[JobRunStatus.FAILED], cluster_id=['ba62e653-312a-490e-9457-71d7bc096959'])
+```
+
+<br/>
+
+##### List batch job runs by batch job name
+
+`BodoClient.job.list_batch_job_runs_by_names()`
+
+| Parameter            | Type                | Description                              | Required          |
+|----------------------|---------------------|------------------------------------------|-------------------|
+| `batch_job_names`    | `List[str]`         | List of Ids of the batch job definitions | No                |
+| `status`             | `List[JobRunStatus]`| List of Job Run Statuses                 | No                |
+| `cluster_id`         | `List[str]`         | List of Ids of the clusters              | No                |
+
+
+Lists all batch job runs in the given workspace filtered by given parameters.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobruns = client.job.list_batch_job_runs_by_names(batch_job_names=['production-job-1'], status=[JobRunStatus.FAILED], cluster_id=['ba62e653-312a-490e-9457-71d7bc096959'])
+```
+
+<br/>
+
+#####  Get batch job run 
+
+
+`BodoClient.job.get_batch_job_run(job_run_id: str)`
+
+Gets specific batch job run by id.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobrun = client.job.get_batch_job_run('04412S5b-300e-42db-84d4-5f22f7506594')
+```
+
+
+<br/>
+
+#####  Cancel batch job run 
+
+
+`BodoClient.job.cancel_batch_job_run(job_run_id: str)`
+
+
+Cancels specific batch job run by id.
+
+
+**Example:**
+
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+client.job.cancel_batch_job_run('04412S5b-300e-42db-84d4-5f22f7506594')
+```
+
+
+
+<br/>
+
+#####  Check batch job run status 
+
+`BodoClient.job.check_job_run_status(job_run_id: str)`
+
+Checks status of specific batch job run by id.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+status = client.job.check_job_run_status('04412S5b-300e-42db-84d4-5f22f7506594')
+```
+
+
+<br/>
+
+#####  Submit SQL job run {#sql-job-run}
+
+`BodoClient.job.submit_sql_job_run(sql_job_details: CreateSQLJobRun)`
+
+Submits a SQL query as a job run. 
+
+!!! note
+    This needs a database [catalog][catalog] to be configured in the workspace.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+
+jobrun = client.job.submit_sql_job_run(CreateSQLJobRun(
+            clusterUUID=cluster.uuid,
+            catalog="SNOWFLAKE_CATALOG",
+            sqlQueryText="SELECT * FROM PUBLIC.TABLE LIMIT 10"))
+```
+
+<br/>
+
+##### Job Run waiter<a id="job-waiter"></a>
+
+`BodoClient.job.get_waiter()`
+
+Returns a waiter object that waits until the job run uuid specified finishes.
+To wait for job run to be finished, invoke the waiter.wait() function,
+which can take the following parameters.
+
+```python3
+from typing import Callable
+def wait(
+        self,
+        uuid,
+        on_success: Callable = None,
+        on_failure: Callable = None,
+        on_timeout: Callable = None,
+        check_period=10,
+        timeout=None
+):
+  pass
+```
+
+By default returns job model if no callbacks is provided. There is option to pass callable objects as following
+parameters:
+
+- `on_success` - will be executed on succes, job object passed as argument
+- `on_failure` - will be executed on failure, job object passed as argument
+- `on_timeout` - will be executed on timeout, job_uuid passed as argument
+
+Other options are:
+
+- `check_period` - seconds between status checks
+- `timeout` - threshold in seconds after which Timeout error will be raised, `None` means no timeout
+
+**Example 1. Success/Failure callbacks:**
+```python
+from bodosdk.models import WorkspaceKeys, CreateJobRun
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id='XYZ',
+    secret_key='XYZ'
+)
+client = get_bodo_client(keys)
+input_job = CreateJobRun(clusterUUID='<cluster-uuid>', batchJobDefinitionUUID='<batch-job-definition-uuid>')
+job_run = client.job.submit_batch_job_run(input_job)
+
+waiter = client.job.get_job_run_waiter()
+
+def success_callback(job):
+    print("in success callback", job.status)
+
+def failure_callback(job):
+    print('in failure callback', job.status)
+
+result = waiter.wait(job_run.uuid, on_success=success_callback, on_failure=failure_callback)
+```
+
+**Example 2. Timeout callback:**
+```python
+from bodosdk.models import WorkspaceKeys, CreateJobRun
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id='XYZ',
+    secret_key='XYZ'
+)
+client = get_bodo_client(keys)
+input_job = CreateJobRun(clusterUUID='<cluster-uuid>', batchJobDefinitionUUID='<batch-job-definition-uuid>')
+job_run = client.job.submit_batch_job_run(input_job)
+
+waiter = client.job.get_job_run_waiter()
+
+def timeout_callback(job_uuid):
+    print(f'Waiter timeout for {job_uuid}')
+    return job_uuid
+
+
+result = waiter.wait(job_run.status, on_timeout=timeout_callback, timeout=1)
+```
+
+
 ### Cluster resource<a id="cluster-resource"></a>
 Module responsible for managing clusters in workspace.
 
 - [get available instance types](#available-instance-types)
 - [get available images](#available-images)
 - [create cluster](#create-cluster)
 - [list clusters](#list-clusters)
```

### Comparing `bodosdk-1.3.2/README.md` & `bodosdk-1.3.3/bodosdk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: bodosdk
+Version: 1.3.3
+Summary: Bodo Platform SDK
+Home-page: https://github.com/Bodo-inc/bodo-sdk
+Author: Bodo, Inc.
+Author-email: noreply@bodo.ai
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Bodo Platform SDK
 
 A simple SDK for Bodo Cloud Platform.
 
 List of contents:
 
 - [Getting Started](#getting-started)
@@ -52,22 +73,30 @@
 )
 client = get_bodo_client(keys, print_logs=True)
 ```
 
 ### Job resource<a id="job-resource"></a> 
 Module responsible for managing jobs in workspace.
 
-- [create job](#create-job)
-- [list jobs](#list-jobs)
-- [get job](#get-job)
-- [remove job](#remove-job)
-- [get execution info](#get-execution)
-- [waiter](#job-waiter)
 
-#### Create job<a id="create-job"></a>
+
+- [Bodo Platform Jobs](#bodo-platform-jobs)
+  - [create job](#create-job)
+  - [list jobs](#list-jobs)
+  - [get job](#get-job)
+  - [remove job](#remove-job)
+  - [get execution info](#get-execution)
+  - [waiter](#job-waiter)
+- [Bodo Platform Batch Jobs](#bodo-platform-batch-jobs)
+
+<br/>
+
+#### Bodo Platform Jobs<a id="bodo-platform-jobs"></a>
+
+##### Create job<a id="create-job"></a>
 
 `BodoClient.job.create(job: JobDefinition)`
 
 Creates a job to be executed on cluster. You can either create job dedicated cluster by providing its definition or
 provide existing cluster uuid. Job dedicated clusters will be removed as soon as job execution will finish, if you provide 
 uuid of existing one, cluster will remain.
 
@@ -237,15 +266,15 @@
     retries=0,
     retries_delay=0,
     retry_on_timeout=False
 )
 
 client.job.create(job_definition)
 ```
-#### List jobs<a id="list-jobs"></a>
+##### List jobs<a id="list-jobs"></a>
 
 `BodoClient.job.list()`
 
 Returns list of all jobs defined in workspace. 
 
 **Example:**
 
@@ -258,15 +287,15 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 jobs: List[JobResponse] = client.job.list()
 ```
 
-#### Get job<a id="get-job"></a>
+##### Get job<a id="get-job"></a>
 
 `BodoClient.job.get(job_uuid)`
 
 Returns specific job in workspace. Example:
 
 ```python
 from bodosdk.models import WorkspaceKeys, JobResponse
@@ -276,15 +305,15 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 job: JobResponse = client.job.get('8c32aec5-7181-45cc-9e17-8aff35fd269e')
 ```
 
-#### Remove job<a id="remove-job"></a>
+##### Remove job<a id="remove-job"></a>
 
 `BodoClient.job.delete(job_uuid)`
 
 Removes specific job from workspace. Example:
 
 ```python
 from bodosdk.models import WorkspaceKeys
@@ -294,15 +323,15 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 client.job.remove('8c32aec5-7181-45cc-9e17-8aff35fd269e')
 ```
 
-#### Get execution<a id="get-execution"></a>
+##### Get execution<a id="get-execution"></a>
 
 `BodoClient.job.get_job_executions(job_uuid)`
 
 Gets all executions info for specific job. Result it's a list with one element (in future we might extend it)
 
 ```python
 from bodosdk.models import WorkspaceKeys, JobExecution
@@ -313,15 +342,15 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 executions: List[JobExecution] = client.job.get_job_executions('8c32aec5-7181-45cc-9e17-8aff35fd269e')
 ```
 
-#### Job waiter<a id="job-waiter"></a>
+##### Job waiter<a id="job-waiter"></a>
 
 `BodoClient.job.get_waiter()`
 
 Get waiter object, which can be used to wait till job finish. Waiter has following method
 
 ```python3
 from typing import Callable
@@ -387,14 +416,512 @@
     print(f'Waiter timeout for {job_uuid}')
     return job_uuid
 
 
 result = waiter.wait('8c32aec5-7181-45cc-9e17-8aff35fd269e', on_timeout=timeout_callback, timeout=1)
 ```
 
+
+<br/>
+
+#### Bodo Platform Batch Jobs <a id="bodo-platform-batch-jobs"></a>
+
+##### Create batch job definition 
+
+`BodoClient.job.create_batch_job_definition(job_definition: CreateBatchJobDefinition)`
+
+Creates batch job definition in the given workspace. 
+
+- **Example 1: Create batch job definition for a workspace source script**
+
+    ```python
+    from bodosdk.models import WorkspaceKeys, CreateBatchJobDefinition, BatchJobDefinition
+    from bodosdk.client import get_bodo_client
+    from bodosdk.models.job import CreateBatchJobDefinition, JobConfig, JobSource, JobSourceType, SourceCodeType, \
+        WorkspaceDef, RetryStrategy
+  
+    keys = WorkspaceKeys(
+      client_id='XYZ',
+      secret_key='XYZ'
+    )
+    client = get_bodo_client(keys)
+    
+    workspace_source_def = JobSource(
+        type=JobSourceType.WORKSPACE,
+        definition=WorkspaceDef(
+            path="Example-path/batch-job-defs",
+        ),
+    )
+    
+    retry_strategy = RetryStrategy(
+        num_retries=1,
+        retry_on_timeout=False,
+        delay_between_retries=2,
+    )
+    
+    jobConfig = JobConfig(
+        source=workspace_source_def,
+        source_code_type=SourceCodeType.PYTHON,
+        sourceLocation="test.py",
+        args=None,
+        retry_strategy=retry_strategy,
+        timeout=10000,
+        env_vars=None,
+    )
+    
+    createBatchJobDef = CreateBatchJobDefinition(
+        name="test-job",
+        config=jobConfig,
+        description="test-batch-job-description-attempt",
+        cluster_config={
+            "bodoVersion": "2023.1.3",
+            "instance_type": "c5.2xlarge",
+            "workers_quantity": 2,
+            "accelerated_networking": False,
+        }, )
+    
+    jobdef = client.job.create_batch_job_definition(createBatchJobDef)
+    ```
+  
+
+- **Example 2: Create batch job definition for a git source script**
+
+  ```python
+  from bodosdk.models import WorkspaceKeys, CreateBatchJobDefinition, BatchJobDefinition
+  from bodosdk.client import get_bodo_client
+  from bodosdk.models.job import CreateBatchJobDefinition, JobConfig, JobSource, JobSourceType, SourceCodeType, \
+      WorkspaceDef, RetryStrategy
+    
+  keys = WorkspaceKeys(
+    client_id='XYZ',
+    secret_key='XYZ'
+  )
+  client = get_bodo_client(keys)
+    
+  git_source_def = JobSource(
+      type=JobSourceType.GIT,
+      definition=GitDef(
+          repo_url='https://github.com/Bodo-inc/Bodo-examples.git',
+          username='XYZ',
+          token='XYZ'
+      ),
+  )
+    
+  retry_strategy = RetryStrategy(
+      num_retries=1,
+      retry_on_timeout=False,
+      delay_between_retries=2,
+  )
+    
+  jobConfig = JobConfig(
+      source=git_source_def,
+      source_code_type=SourceCodeType.PYTHON,
+      sourceLocation="test.py",
+      args=None,
+      retry_strategy=retry_strategy,
+      timeout=10000,
+      env_vars=None,
+  )
+    
+  createBatchJobDef = CreateBatchJobDefinition(
+      name="test-job",
+      config=jobConfig,
+      description="test-batch-job-description-attempt",
+      cluster_config={
+          "bodoVersion": "2023.1.3",
+          "instance_type": "c5.2xlarge",
+          "workers_quantity": 2,
+          "accelerated_networking": False,
+      }, )
+    
+  jobdef = client.job.create_batch_job_definition(createBatchJobDef)  
+  ```
+  
+
+<br/>
+
+#####  List batch job definitions 
+
+`BodoClient.job.list_batch_job_definitions()`
+
+Lists all batch job definitions in the given workspace.
+
+**Example:**
+```python
+from typing import List
+
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobdefs: List[BatchJobDefinitionResponse] = client.job.list_batch_job_definitions()
+```
+
+
+<br/>
+
+#####  Get batch job definition by id
+
+`BodoClient.job.get_batch_job_definition(job_definition_id: str)`
+
+Gets specific batch job definition by id.
+
+**Example:**
+```python
+from typing import List
+
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobdef: BatchJobDefinitionResponse = client.job.get_batch_job_definition('04412S5b-300e-42db-84d4-5f22f7506594')
+```  
+
+<br/>
+
+##### Get batch job definition by name
+
+`BodoClient.job.get_batch_job_definition_by_name(name: str)`
+
+Gets specific batch job definition by id.
+
+**Example:**
+```python
+from typing import List
+
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobdef: BatchJobDefinitionResponse = client.job.get_batch_job_definition('04412S5b-300e-42db-84d4-5f22f7506594')
+```  
+  
+
+<br/>
+
+#####  Remove batch job definition 
+
+`BodoClient.job.remove_batch_job_definition(job_definition_id: str)`
+
+Removes specific batch job definition by id.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+client.job.remove_batch_job_definition('04412S5b-300e-42db-84d4-5f22f7506594')
+```
+
+
+<br/>
+
+#####  Submit a batch job run 
+
+`BodoClient.job.submit_batch_job_run(job_run: CreateJobRun)`
+
+Submits a job run for a given batch job definition.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+client.job.submit_batch_job_run(CreateJobRun(batchJobDefinitionUUID='04412S5b-300e-42db-84d4-5f22f7506594', clusterUUID='12936Q5z-109d-89yi-23c4-3d91u1219823'))
+```
+
+
+#####  List batch job runs 
+
+`BodoClient.job.list_batch_job_runs()`
+
+| Parameter         | Type                | Description                              | Required          |
+|-------------------|---------------------|------------------------------------------|-------------------|
+| `batch_job_id`    | `List[str]`         | List of Ids of the batch job definitions | No                |
+| `status`          | `List[JobRunStatus]`| List of Job Run Statuses                 | No                |
+| `cluster_id`      | `List[str]`         | List of Ids of the clusters              | No                |
+
+Lists all batch job runs in the given workspace filtered by given parameters.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobruns = client.job.list_batch_job_runs(status=[JobRunStatus.FAILED], cluster_id=['ba62e653-312a-490e-9457-71d7bc096959'])
+```
+
+<br/>
+
+##### List batch job runs by batch job name
+
+`BodoClient.job.list_batch_job_runs_by_names()`
+
+| Parameter            | Type                | Description                              | Required          |
+|----------------------|---------------------|------------------------------------------|-------------------|
+| `batch_job_names`    | `List[str]`         | List of Ids of the batch job definitions | No                |
+| `status`             | `List[JobRunStatus]`| List of Job Run Statuses                 | No                |
+| `cluster_id`         | `List[str]`         | List of Ids of the clusters              | No                |
+
+
+Lists all batch job runs in the given workspace filtered by given parameters.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobruns = client.job.list_batch_job_runs_by_names(batch_job_names=['production-job-1'], status=[JobRunStatus.FAILED], cluster_id=['ba62e653-312a-490e-9457-71d7bc096959'])
+```
+
+<br/>
+
+#####  Get batch job run 
+
+
+`BodoClient.job.get_batch_job_run(job_run_id: str)`
+
+Gets specific batch job run by id.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobrun = client.job.get_batch_job_run('04412S5b-300e-42db-84d4-5f22f7506594')
+```
+
+
+<br/>
+
+#####  Cancel batch job run 
+
+
+`BodoClient.job.cancel_batch_job_run(job_run_id: str)`
+
+
+Cancels specific batch job run by id.
+
+
+**Example:**
+
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+client.job.cancel_batch_job_run('04412S5b-300e-42db-84d4-5f22f7506594')
+```
+
+
+
+<br/>
+
+#####  Check batch job run status 
+
+`BodoClient.job.check_job_run_status(job_run_id: str)`
+
+Checks status of specific batch job run by id.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+status = client.job.check_job_run_status('04412S5b-300e-42db-84d4-5f22f7506594')
+```
+
+
+<br/>
+
+#####  Submit SQL job run {#sql-job-run}
+
+`BodoClient.job.submit_sql_job_run(sql_job_details: CreateSQLJobRun)`
+
+Submits a SQL query as a job run. 
+
+!!! note
+    This needs a database [catalog][catalog] to be configured in the workspace.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+
+jobrun = client.job.submit_sql_job_run(CreateSQLJobRun(
+            clusterUUID=cluster.uuid,
+            catalog="SNOWFLAKE_CATALOG",
+            sqlQueryText="SELECT * FROM PUBLIC.TABLE LIMIT 10"))
+```
+
+<br/>
+
+##### Job Run waiter<a id="job-waiter"></a>
+
+`BodoClient.job.get_waiter()`
+
+Returns a waiter object that waits until the job run uuid specified finishes.
+To wait for job run to be finished, invoke the waiter.wait() function,
+which can take the following parameters.
+
+```python3
+from typing import Callable
+def wait(
+        self,
+        uuid,
+        on_success: Callable = None,
+        on_failure: Callable = None,
+        on_timeout: Callable = None,
+        check_period=10,
+        timeout=None
+):
+  pass
+```
+
+By default returns job model if no callbacks is provided. There is option to pass callable objects as following
+parameters:
+
+- `on_success` - will be executed on succes, job object passed as argument
+- `on_failure` - will be executed on failure, job object passed as argument
+- `on_timeout` - will be executed on timeout, job_uuid passed as argument
+
+Other options are:
+
+- `check_period` - seconds between status checks
+- `timeout` - threshold in seconds after which Timeout error will be raised, `None` means no timeout
+
+**Example 1. Success/Failure callbacks:**
+```python
+from bodosdk.models import WorkspaceKeys, CreateJobRun
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id='XYZ',
+    secret_key='XYZ'
+)
+client = get_bodo_client(keys)
+input_job = CreateJobRun(clusterUUID='<cluster-uuid>', batchJobDefinitionUUID='<batch-job-definition-uuid>')
+job_run = client.job.submit_batch_job_run(input_job)
+
+waiter = client.job.get_job_run_waiter()
+
+def success_callback(job):
+    print("in success callback", job.status)
+
+def failure_callback(job):
+    print('in failure callback', job.status)
+
+result = waiter.wait(job_run.uuid, on_success=success_callback, on_failure=failure_callback)
+```
+
+**Example 2. Timeout callback:**
+```python
+from bodosdk.models import WorkspaceKeys, CreateJobRun
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id='XYZ',
+    secret_key='XYZ'
+)
+client = get_bodo_client(keys)
+input_job = CreateJobRun(clusterUUID='<cluster-uuid>', batchJobDefinitionUUID='<batch-job-definition-uuid>')
+job_run = client.job.submit_batch_job_run(input_job)
+
+waiter = client.job.get_job_run_waiter()
+
+def timeout_callback(job_uuid):
+    print(f'Waiter timeout for {job_uuid}')
+    return job_uuid
+
+
+result = waiter.wait(job_run.status, on_timeout=timeout_callback, timeout=1)
+```
+
+
 ### Cluster resource<a id="cluster-resource"></a>
 Module responsible for managing clusters in workspace.
 
 - [get available instance types](#available-instance-types)
 - [get available images](#available-images)
 - [create cluster](#create-cluster)
 - [list clusters](#list-clusters)
@@ -1327,7 +1854,9 @@
 keys = WorkspaceKeys(
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 secret_info: SecretInfo = client.secrets.remove("<secret-uuid>")
 ```
+
+
```

### Comparing `bodosdk-1.3.2/bodosdk/api/auth.py` & `bodosdk-1.3.3/bodosdk/api/auth.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/api/base.py` & `bodosdk-1.3.3/bodosdk/api/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/api/catalog.py` & `bodosdk-1.3.3/bodosdk/api/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/api/cloud_config.py` & `bodosdk-1.3.3/bodosdk/api/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/api/cluster.py` & `bodosdk-1.3.3/bodosdk/api/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/api/instance_role.py` & `bodosdk-1.3.3/bodosdk/api/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/api/job.py` & `bodosdk-1.3.3/bodosdk/api/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import logging
 from datetime import datetime
 from typing import List, Union
 from uuid import UUID
 
+import pydantic.error_wrappers
 from pydantic import validate_arguments
 
 from bodosdk.api.base import BackendApi
 from bodosdk.exc import (
     ResourceNotFound,
     ServiceUnavailable,
     UnknownError,
@@ -195,16 +197,23 @@
         resp = self._requests.get(resource_url, headers=headers)
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable
         if str(resp.status_code).startswith("4"):
             raise ResourceNotFound(resp.json()["message"])
 
         result = []
-        for json_data in resp.json():
-            result.append(BatchJobDefinitionResponse(**json_data))
+        for json_data in resp.json()["data"]:
+            try:
+                result.append(BatchJobDefinitionResponse(**json_data))
+            except pydantic.ValidationError:
+                logging.error(
+                    f"Failed to parse batch job definition for batch job id: {json_data['uuid']}"
+                )
+            except Exception as e:
+                logging.error(f"Bad Response: {e}")
         return result
 
     @validate_arguments
     def get_batch_job_definition(self, uuid: UUID) -> BatchJobDefinitionResponse:
         headers = self.get_auth_header()
         resp = self._requests.get(
             f"{self.get_resource_url()}/batch_job_def/{uuid}", headers=headers
@@ -224,15 +233,15 @@
         )
         if resp.status_code == 404:
             raise ResourceNotFound
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable
 
         # Based on DB criteria there can be only one element
-        for json_data in resp.json():
+        for json_data in resp.json()["data"]:
             return BatchJobDefinitionResponse(**json_data)
 
         raise ResourceNotFound
 
     @validate_arguments
     def update_batch_job_definition(
         self, uuid: UUID, config_override: JobConfigOverride
@@ -255,14 +264,19 @@
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable
         raise UnknownError(resp.content)
 
     # Job Run APIs
     @validate_arguments
     def create_batch_job_run(self, create_job_run: CreateJobRun) -> JobRunResponse:
+        if not create_job_run.batchJobDefinitionUUID:
+            batch_job_definition = self.get_batch_job_definition_by_name(
+                create_job_run.batchJobName
+            )
+            create_job_run.batchJobDefinitionUUID = batch_job_definition.uuid
         headers = {"Content-type": "application/json"}
         headers.update(self.get_auth_header())
         resp = self._requests.post(
             f"{self.get_resource_url()}/run/batch",
             data=create_job_run.json(by_alias=True),
             headers=headers,
         )
@@ -340,27 +354,33 @@
         self,
         job_type: List[JobRunType] = None,
         batch_job_id: Union[List[UUID], None] = None,
         status: Union[List[JobRunStatus], None] = None,
         cluster_id: Union[List[UUID], None] = None,
         started_at: Union[datetime, None] = None,
         finished_at: Union[datetime, None] = None,
-        page: int = 1,
-        page_size: int = 100,
-        order: PaginationOrder = PaginationOrder.ASC,
+        page: int = DEFAULT_PAGE,
+        page_size: int = DEFAULT_PAGE_SIZE,
+        order: PaginationOrder = DEFAULT_ORDER,
     ) -> List[JobRunResponse]:
         args = LIST_QUERY_PARAMS
         query_string_args = {
             k: v for k, v in locals().items() if k in args and v is not None
         }
         headers = self.get_auth_header()
         query_string = build_query_string(query_string_args)
         url = f"{self.get_resource_url()}/run{query_string}"
         resp = self._requests.get(url, headers=headers)
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable()
         if str(resp.status_code).startswith("4"):
             raise ResourceNotFound(resp.json()["message"])
         result = []
-        for json_data in resp.json():
-            result.append(JobRunResponse(**json_data))
+        for json_data in resp.json()["data"]:
+            try:
+                result.append(JobRunResponse(**json_data))
+            except pydantic.ValidationError:
+                logging.warning(
+                    f"Failed to parse job run response: {json_data['uuid']}"
+                )
+
         return result
```

### Comparing `bodosdk-1.3.2/bodosdk/api/request_wrapper.py` & `bodosdk-1.3.3/bodosdk/api/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/api/secret_group.py` & `bodosdk-1.3.3/bodosdk/api/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/api/secrets.py` & `bodosdk-1.3.3/bodosdk/api/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/api/workspace.py` & `bodosdk-1.3.3/bodosdk/api/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/client/base.py` & `bodosdk-1.3.3/bodosdk/client/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/client/catalog.py` & `bodosdk-1.3.3/bodosdk/client/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/client/cloud_config.py` & `bodosdk-1.3.3/bodosdk/client/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/client/cluster.py` & `bodosdk-1.3.3/bodosdk/client/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/client/instance_role.py` & `bodosdk-1.3.3/bodosdk/client/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/client/job.py` & `bodosdk-1.3.3/bodosdk/client/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,22 +20,23 @@
     CreateJobRun,
     JobRunStatus,
     CreateSQLJobRun,
 )
 
 
 class JobWaiter:
-    def __init__(self, client):
+    def __init__(self, client, job_run=False):
         """
         Object for waiting till job finishes
 
         :param client:
         :type client: JobClient
         """
         self._client = client
+        self._is_job_run = job_run
 
     def wait(
         self,
         uuid,
         on_success: Callable = None,
         on_failure: Callable = None,
         on_timeout: Callable = None,
@@ -51,29 +52,51 @@
         :param on_timeout: callback to be called on failure, job uuid passed into.
         If no callback WaiterTimeout exception raised
         :param check_period: how often waiter should check
         :param timeout: how long waiter should try, None means infinity
         :return: job response or result of callbacks
         :raises WaiterTimeout: when timeout and no on_timeout callback defined
         """
-        job: JobResponse = self._client.get(uuid)
-        while job.status not in (JobStatus.FINISHED, JobStatus.FAILED):
+        job = self.get_job_by_uuid(uuid)
+        while not self.termination_condition(job, job.status):
             sleep(check_period)
             timeout = timeout - check_period if timeout else timeout
             if timeout is not None and timeout <= 0:
                 if on_timeout:
                     return on_timeout(uuid)
                 raise WaiterTimeout
-            job: JobResponse = self._client.get(uuid)
-        if job.status == JobStatus.FINISHED and on_success:
+            job = self.get_job_by_uuid(uuid)
+
+        if (job.status == JobStatus.FINISHED and on_success) or (
+            job.status == JobRunStatus.SUCCEEDED and on_success
+        ):
             return on_success(job)
-        if job.status == JobStatus.FAILED and on_failure:
+        if (job.status == JobStatus.FAILED and on_failure) or (
+            job.status == JobRunStatus.FAILED and on_failure
+        ):
             return on_failure(job)
         return job
 
+    def get_job_by_uuid(self, uuid):
+        return (
+            self._client.get_batch_job_run(uuid)
+            if self._is_job_run
+            else self._client.get(uuid)
+        )
+
+    def termination_condition(self, job, status):
+        if isinstance(status, JobRunStatus):
+            job: JobRunStatus = job
+            return job.status in (
+                JobRunStatus.FAILED,
+                JobRunStatus.SUCCEEDED,
+                JobRunStatus.CANCELLED,
+            )
+        return job.status in (JobStatus.FINISHED, JobStatus.FAILED)  # for jobs v2
+
 
 class JobClient:
     def __init__(self, api: JobApi):
         self._api = api
 
     def create(self, job_definition: JobDefinition) -> JobCreateResponse:
         """
@@ -135,20 +158,29 @@
         :rtype: List[JobExecution]
         :raises ResourceNotFound:
         """
         return self._api.get_tasks(str(uuid))
 
     def get_waiter(self) -> JobWaiter:
         """
-        Returns waiter
+        Returns waiter waiting till the job finishes, given a workspace
         :return: a helper waiting till job finishes
         :rtype: JobWaiter
         """
         return JobWaiter(client=deepcopy(self))
 
+    def get_job_run_waiter(self) -> JobWaiter:
+        """
+        Returns a waiter that waits until the job run finishes
+        Designed for V3 jobs usage
+        :return: a helper waiting till job finishes
+        :rtype: JobWaiter
+        """
+        return JobWaiter(client=deepcopy(self), job_run=True)
+
     def list_batch_job_definitions(self) -> List[BatchJobDefinitionResponse]:
         """
         List all batch job definitions in workspace
 
         :return: list of batch job definitions
         :rtype: List[BatchJobDefinition]
         """
```

### Comparing `bodosdk-1.3.2/bodosdk/client/secret_group.py` & `bodosdk-1.3.3/bodosdk/client/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/client/secrets.py` & `bodosdk-1.3.3/bodosdk/client/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/client/workspace.py` & `bodosdk-1.3.3/bodosdk/client/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/models/__init__.py` & `bodosdk-1.3.3/bodosdk/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     WorkspaceSource,
     JobCluster,
     JobExecution,
     BatchJobDefinitionResponse,
     CreateBatchJobDefinition,
     JobConfig,
     JobConfigOverride,
-    WorkspaceDef,
     SourceCodeType,
     RetryStrategy,
     JobSource,
     JobSourceType,
     CreateJobRun,
     JobRunResponse,
     JobRunStatus,
```

### Comparing `bodosdk-1.3.2/bodosdk/models/base.py` & `bodosdk-1.3.3/bodosdk/models/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/models/catalog.py` & `bodosdk-1.3.3/bodosdk/models/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/models/cloud_config.py` & `bodosdk-1.3.3/bodosdk/models/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/models/cluster.py` & `bodosdk-1.3.3/bodosdk/models/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk/models/job.py` & `bodosdk-1.3.3/bodosdk/models/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import enum
 from datetime import datetime
 from typing import Optional, Dict, Union, List
 from uuid import UUID
 
 import pydantic
-from pydantic import Field
+from pydantic import Field, root_validator
 
 from bodosdk.models.base import JobStatus, TaskStatus, CamelCaseBase
 
 
 class JobClusterDefinition(CamelCaseBase):
     instance_type: str = Field(..., alias="instanceType")
     workers_quantity: int = Field(..., alias="workersQuantity")
     accelerated_networking: bool = Field(..., alias="acceleratedNetworking")
     image_id: Optional[str] = Field(None, alias="imageId")
     bodo_version: Optional[str] = Field(None, alias="bodoVersion")
     instance_role_uuid: Optional[str] = Field(None, alias="instanceRoleUUID")
     availability_zone: Optional[str] = Field(None, alias="availabilityZone")
     aws_deployment_subnet_id: Optional[str] = Field(None, alias="awsDeploymentSubnetId")
     custom_tags: Optional[Dict[str, str]] = Field(None, alias="customTags")
+    auto_pause: Optional[int] = Field(60, alias="autoPause")
+    auto_shutdown: Optional[int] = Field(0, alias="autoShutdown")
 
 
 class JobCluster(pydantic.BaseModel):
     uuid: Union[str, UUID]
 
 
 class JobSourceType(enum.Enum):
@@ -32,32 +34,89 @@
     SQL = "SQL"
 
     def __repr__(self):
         return self.value
 
 
 class GitRepoSource(CamelCaseBase):
+    """
+    Git repository source definition.
+
+    ...
+
+    Attributes
+    ----------
+    repo_url: str
+        Git repository URL.
+
+    reference: Optional[str]
+        Git reference (branch, tag, commit hash). (Default: "")
+
+    username: str
+        Git username.
+
+    token: str
+        Git token.
+
+    """
+
     type: JobSourceType = Field(JobSourceType.GIT, const=True)
     repo_url: str = Field(..., alias="repoUrl")
     reference: Optional[str] = ""
     username: str
     token: str
 
 
 class S3Source(CamelCaseBase):
+    """
+    S3 source definition.
+
+    ...
+
+    Attributes
+    ----------
+    bucket_path: str
+        S3 bucket path.
+
+    bucket_region: str
+        S3 bucket region.
+
+    """
+
     type: JobSourceType = Field(JobSourceType.S3, const=True)
     bucket_path: str = Field(..., alias="bucketPath")
     bucket_region: str = Field(..., alias="bucketRegion")
 
 
 class WorkspaceSource(pydantic.BaseModel):
+    """
+    Workspace source definition.
+
+    ...
+
+    Attributes
+    ----------
+    path: str
+        Workspace path.
+    """
+
     type: JobSourceType = Field(JobSourceType.WORKSPACE, const=True)
     path: str
 
 
+class SQLSource(CamelCaseBase):
+    """
+    SQL source definition.
+
+    ...
+    """
+
+    type: JobSourceType = Field(JobSourceType.SQL, const=True)
+
+
 class JobDefinition(CamelCaseBase):
     name: str
     args: str
     source_config: Union[GitRepoSource, S3Source, WorkspaceSource] = Field(
         ..., alias="sourceConfig"
     )
     cluster_object: Union[JobClusterDefinition, JobCluster] = Field(
@@ -116,86 +175,14 @@
     uuid: UUID
     status: TaskStatus
     logs: str
     modify_date: datetime = Field(..., alias="modifyDate")
     created_at: datetime = Field(..., alias="createdAt")
 
 
-# New source definitions per the new API.
-class GitDef(CamelCaseBase):
-    """
-    Git repository source definition.
-
-    ...
-
-    Attributes
-    ----------
-    repo_url: str
-        Git repository URL.
-
-    reference: Optional[str]
-        Git reference (branch, tag, commit hash). (Default: "")
-
-    username: str
-        Git username.
-
-    token: str
-        Git token.
-
-    """
-
-    repo_url: str = Field(..., alias="repoUrl")
-    reference: Optional[str] = ""
-    username: Optional[str]
-    token: Optional[str]
-
-
-class S3Def(CamelCaseBase):
-    """
-    S3 source definition.
-
-    ...
-
-    Attributes
-    ----------
-    bucket_path: str
-        S3 bucket path.
-
-    bucket_region: str
-        S3 bucket region.
-
-    """
-
-    bucket_path: str = Field(..., alias="bucketPath")
-    bucket_region: str = Field(..., alias="bucketRegion")
-
-
-class WorkspaceDef(CamelCaseBase):
-    """
-    Workspace source definition.
-
-    ...
-
-    Attributes
-    ----------
-    path: str
-        Workspace path.
-    """
-
-    path: str
-
-
-class SQLDef(CamelCaseBase):
-    """
-    SQL source definition.
-
-    ...
-    """
-
-
 class JobSource(CamelCaseBase):
     """
     Job source.
 
     ...
 
     Attributes
@@ -204,15 +191,15 @@
         Job source type.
 
     definition: Union[GitDef, S3Def, WorkspaceDef]
         Job source definition.
     """
 
     type: JobSourceType
-    definition: Union[GitDef, S3Def, WorkspaceDef, SQLDef] = Field(
+    definition: Union[GitRepoSource, S3Source, WorkspaceSource, SQLSource] = Field(
         ..., alias="sourceDef"
     )
 
 
 class RetryStrategy(CamelCaseBase):
     """
     Retry strategy for a job.
@@ -529,25 +516,37 @@
 
     clusterUUID: Optional[Union[UUID, str]]
         Job cluster UUID.
 
     batchJobUUID: Optional[Union[UUID, str]]
         Batch job UUID.
 
+    batchJobName: Optional[str]
+
     batchJobDefinitionConfigOverrides: Optional[JobConfigOverride]
         Batch job definition configuration overrides.
     """
 
     type: JobRunType = JobRunType.BATCH
     clusterUUID: Optional[Union[UUID, str]]  # Todo(Ritwika): Confirm
     batchJobDefinitionUUID: Optional[Union[UUID, str]] = Field(
-        ..., alias="batchJobDefinitionUUID"
+        default=None, alias="batchJobDefinitionUUID"
     )
+    batchJobName: Optional[str] = Field(default=None, alias="batchJobName")
     batchJobDefinitionConfigOverrides: Optional[JobConfigOverride]
 
+    @root_validator(pre=True)
+    def validate_batch_job_def_id(cls, values):
+        if not ("batchJobDefinitionUUID" in values.keys()):
+            if not ("batchJobName" in values.keys()):
+                raise ValueError(
+                    "Either batchJobDefinitionUUID or batchJobName must be provided."
+                )
+        return values
+
 
 class CreateSQLJobRun(CamelCaseBase):
     """
     Create SQL job run.
 
     ...
```

### Comparing `bodosdk-1.3.2/bodosdk/models/workspace.py` & `bodosdk-1.3.3/bodosdk/models/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/bodosdk.egg-info/PKG-INFO` & `bodosdk-1.3.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: bodosdk
-Version: 1.3.2
-Summary: Bodo Platform SDK
-Home-page: https://github.com/Bodo-inc/bodo-sdk
-Author: Bodo, Inc.
-Author-email: noreply@bodo.ai
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Bodo Platform SDK
 
 A simple SDK for Bodo Cloud Platform.
 
 List of contents:
 
 - [Getting Started](#getting-started)
@@ -73,22 +52,30 @@
 )
 client = get_bodo_client(keys, print_logs=True)
 ```
 
 ### Job resource<a id="job-resource"></a> 
 Module responsible for managing jobs in workspace.
 
-- [create job](#create-job)
-- [list jobs](#list-jobs)
-- [get job](#get-job)
-- [remove job](#remove-job)
-- [get execution info](#get-execution)
-- [waiter](#job-waiter)
 
-#### Create job<a id="create-job"></a>
+
+- [Bodo Platform Jobs](#bodo-platform-jobs)
+  - [create job](#create-job)
+  - [list jobs](#list-jobs)
+  - [get job](#get-job)
+  - [remove job](#remove-job)
+  - [get execution info](#get-execution)
+  - [waiter](#job-waiter)
+- [Bodo Platform Batch Jobs](#bodo-platform-batch-jobs)
+
+<br/>
+
+#### Bodo Platform Jobs<a id="bodo-platform-jobs"></a>
+
+##### Create job<a id="create-job"></a>
 
 `BodoClient.job.create(job: JobDefinition)`
 
 Creates a job to be executed on cluster. You can either create job dedicated cluster by providing its definition or
 provide existing cluster uuid. Job dedicated clusters will be removed as soon as job execution will finish, if you provide 
 uuid of existing one, cluster will remain.
 
@@ -258,15 +245,15 @@
     retries=0,
     retries_delay=0,
     retry_on_timeout=False
 )
 
 client.job.create(job_definition)
 ```
-#### List jobs<a id="list-jobs"></a>
+##### List jobs<a id="list-jobs"></a>
 
 `BodoClient.job.list()`
 
 Returns list of all jobs defined in workspace. 
 
 **Example:**
 
@@ -279,15 +266,15 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 jobs: List[JobResponse] = client.job.list()
 ```
 
-#### Get job<a id="get-job"></a>
+##### Get job<a id="get-job"></a>
 
 `BodoClient.job.get(job_uuid)`
 
 Returns specific job in workspace. Example:
 
 ```python
 from bodosdk.models import WorkspaceKeys, JobResponse
@@ -297,15 +284,15 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 job: JobResponse = client.job.get('8c32aec5-7181-45cc-9e17-8aff35fd269e')
 ```
 
-#### Remove job<a id="remove-job"></a>
+##### Remove job<a id="remove-job"></a>
 
 `BodoClient.job.delete(job_uuid)`
 
 Removes specific job from workspace. Example:
 
 ```python
 from bodosdk.models import WorkspaceKeys
@@ -315,15 +302,15 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 client.job.remove('8c32aec5-7181-45cc-9e17-8aff35fd269e')
 ```
 
-#### Get execution<a id="get-execution"></a>
+##### Get execution<a id="get-execution"></a>
 
 `BodoClient.job.get_job_executions(job_uuid)`
 
 Gets all executions info for specific job. Result it's a list with one element (in future we might extend it)
 
 ```python
 from bodosdk.models import WorkspaceKeys, JobExecution
@@ -334,15 +321,15 @@
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 executions: List[JobExecution] = client.job.get_job_executions('8c32aec5-7181-45cc-9e17-8aff35fd269e')
 ```
 
-#### Job waiter<a id="job-waiter"></a>
+##### Job waiter<a id="job-waiter"></a>
 
 `BodoClient.job.get_waiter()`
 
 Get waiter object, which can be used to wait till job finish. Waiter has following method
 
 ```python3
 from typing import Callable
@@ -408,14 +395,512 @@
     print(f'Waiter timeout for {job_uuid}')
     return job_uuid
 
 
 result = waiter.wait('8c32aec5-7181-45cc-9e17-8aff35fd269e', on_timeout=timeout_callback, timeout=1)
 ```
 
+
+<br/>
+
+#### Bodo Platform Batch Jobs <a id="bodo-platform-batch-jobs"></a>
+
+##### Create batch job definition 
+
+`BodoClient.job.create_batch_job_definition(job_definition: CreateBatchJobDefinition)`
+
+Creates batch job definition in the given workspace. 
+
+- **Example 1: Create batch job definition for a workspace source script**
+
+    ```python
+    from bodosdk.models import WorkspaceKeys, CreateBatchJobDefinition, BatchJobDefinition
+    from bodosdk.client import get_bodo_client
+    from bodosdk.models.job import CreateBatchJobDefinition, JobConfig, JobSource, JobSourceType, SourceCodeType, \
+        WorkspaceDef, RetryStrategy
+  
+    keys = WorkspaceKeys(
+      client_id='XYZ',
+      secret_key='XYZ'
+    )
+    client = get_bodo_client(keys)
+    
+    workspace_source_def = JobSource(
+        type=JobSourceType.WORKSPACE,
+        definition=WorkspaceDef(
+            path="Example-path/batch-job-defs",
+        ),
+    )
+    
+    retry_strategy = RetryStrategy(
+        num_retries=1,
+        retry_on_timeout=False,
+        delay_between_retries=2,
+    )
+    
+    jobConfig = JobConfig(
+        source=workspace_source_def,
+        source_code_type=SourceCodeType.PYTHON,
+        sourceLocation="test.py",
+        args=None,
+        retry_strategy=retry_strategy,
+        timeout=10000,
+        env_vars=None,
+    )
+    
+    createBatchJobDef = CreateBatchJobDefinition(
+        name="test-job",
+        config=jobConfig,
+        description="test-batch-job-description-attempt",
+        cluster_config={
+            "bodoVersion": "2023.1.3",
+            "instance_type": "c5.2xlarge",
+            "workers_quantity": 2,
+            "accelerated_networking": False,
+        }, )
+    
+    jobdef = client.job.create_batch_job_definition(createBatchJobDef)
+    ```
+  
+
+- **Example 2: Create batch job definition for a git source script**
+
+  ```python
+  from bodosdk.models import WorkspaceKeys, CreateBatchJobDefinition, BatchJobDefinition
+  from bodosdk.client import get_bodo_client
+  from bodosdk.models.job import CreateBatchJobDefinition, JobConfig, JobSource, JobSourceType, SourceCodeType, \
+      WorkspaceDef, RetryStrategy
+    
+  keys = WorkspaceKeys(
+    client_id='XYZ',
+    secret_key='XYZ'
+  )
+  client = get_bodo_client(keys)
+    
+  git_source_def = JobSource(
+      type=JobSourceType.GIT,
+      definition=GitDef(
+          repo_url='https://github.com/Bodo-inc/Bodo-examples.git',
+          username='XYZ',
+          token='XYZ'
+      ),
+  )
+    
+  retry_strategy = RetryStrategy(
+      num_retries=1,
+      retry_on_timeout=False,
+      delay_between_retries=2,
+  )
+    
+  jobConfig = JobConfig(
+      source=git_source_def,
+      source_code_type=SourceCodeType.PYTHON,
+      sourceLocation="test.py",
+      args=None,
+      retry_strategy=retry_strategy,
+      timeout=10000,
+      env_vars=None,
+  )
+    
+  createBatchJobDef = CreateBatchJobDefinition(
+      name="test-job",
+      config=jobConfig,
+      description="test-batch-job-description-attempt",
+      cluster_config={
+          "bodoVersion": "2023.1.3",
+          "instance_type": "c5.2xlarge",
+          "workers_quantity": 2,
+          "accelerated_networking": False,
+      }, )
+    
+  jobdef = client.job.create_batch_job_definition(createBatchJobDef)  
+  ```
+  
+
+<br/>
+
+#####  List batch job definitions 
+
+`BodoClient.job.list_batch_job_definitions()`
+
+Lists all batch job definitions in the given workspace.
+
+**Example:**
+```python
+from typing import List
+
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobdefs: List[BatchJobDefinitionResponse] = client.job.list_batch_job_definitions()
+```
+
+
+<br/>
+
+#####  Get batch job definition by id
+
+`BodoClient.job.get_batch_job_definition(job_definition_id: str)`
+
+Gets specific batch job definition by id.
+
+**Example:**
+```python
+from typing import List
+
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobdef: BatchJobDefinitionResponse = client.job.get_batch_job_definition('04412S5b-300e-42db-84d4-5f22f7506594')
+```  
+
+<br/>
+
+##### Get batch job definition by name
+
+`BodoClient.job.get_batch_job_definition_by_name(name: str)`
+
+Gets specific batch job definition by id.
+
+**Example:**
+```python
+from typing import List
+
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobdef: BatchJobDefinitionResponse = client.job.get_batch_job_definition('04412S5b-300e-42db-84d4-5f22f7506594')
+```  
+  
+
+<br/>
+
+#####  Remove batch job definition 
+
+`BodoClient.job.remove_batch_job_definition(job_definition_id: str)`
+
+Removes specific batch job definition by id.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+client.job.remove_batch_job_definition('04412S5b-300e-42db-84d4-5f22f7506594')
+```
+
+
+<br/>
+
+#####  Submit a batch job run 
+
+`BodoClient.job.submit_batch_job_run(job_run: CreateJobRun)`
+
+Submits a job run for a given batch job definition.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+client.job.submit_batch_job_run(CreateJobRun(batchJobDefinitionUUID='04412S5b-300e-42db-84d4-5f22f7506594', clusterUUID='12936Q5z-109d-89yi-23c4-3d91u1219823'))
+```
+
+
+#####  List batch job runs 
+
+`BodoClient.job.list_batch_job_runs()`
+
+| Parameter         | Type                | Description                              | Required          |
+|-------------------|---------------------|------------------------------------------|-------------------|
+| `batch_job_id`    | `List[str]`         | List of Ids of the batch job definitions | No                |
+| `status`          | `List[JobRunStatus]`| List of Job Run Statuses                 | No                |
+| `cluster_id`      | `List[str]`         | List of Ids of the clusters              | No                |
+
+Lists all batch job runs in the given workspace filtered by given parameters.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobruns = client.job.list_batch_job_runs(status=[JobRunStatus.FAILED], cluster_id=['ba62e653-312a-490e-9457-71d7bc096959'])
+```
+
+<br/>
+
+##### List batch job runs by batch job name
+
+`BodoClient.job.list_batch_job_runs_by_names()`
+
+| Parameter            | Type                | Description                              | Required          |
+|----------------------|---------------------|------------------------------------------|-------------------|
+| `batch_job_names`    | `List[str]`         | List of Ids of the batch job definitions | No                |
+| `status`             | `List[JobRunStatus]`| List of Job Run Statuses                 | No                |
+| `cluster_id`         | `List[str]`         | List of Ids of the clusters              | No                |
+
+
+Lists all batch job runs in the given workspace filtered by given parameters.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+from bodosdk.models.job import CreateJobRun, JobSource, JobRunStatus, BatchJobDefinitionResponse
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobruns = client.job.list_batch_job_runs_by_names(batch_job_names=['production-job-1'], status=[JobRunStatus.FAILED], cluster_id=['ba62e653-312a-490e-9457-71d7bc096959'])
+```
+
+<br/>
+
+#####  Get batch job run 
+
+
+`BodoClient.job.get_batch_job_run(job_run_id: str)`
+
+Gets specific batch job run by id.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+jobrun = client.job.get_batch_job_run('04412S5b-300e-42db-84d4-5f22f7506594')
+```
+
+
+<br/>
+
+#####  Cancel batch job run 
+
+
+`BodoClient.job.cancel_batch_job_run(job_run_id: str)`
+
+
+Cancels specific batch job run by id.
+
+
+**Example:**
+
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+client.job.cancel_batch_job_run('04412S5b-300e-42db-84d4-5f22f7506594')
+```
+
+
+
+<br/>
+
+#####  Check batch job run status 
+
+`BodoClient.job.check_job_run_status(job_run_id: str)`
+
+Checks status of specific batch job run by id.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+status = client.job.check_job_run_status('04412S5b-300e-42db-84d4-5f22f7506594')
+```
+
+
+<br/>
+
+#####  Submit SQL job run {#sql-job-run}
+
+`BodoClient.job.submit_sql_job_run(sql_job_details: CreateSQLJobRun)`
+
+Submits a SQL query as a job run. 
+
+!!! note
+    This needs a database [catalog][catalog] to be configured in the workspace.
+
+**Example:**
+```python
+from bodosdk.models import PersonalKeys, WorkspaceKeys, JobConfig, SourceCodeType, RetryStrategy, JobSourceType, \
+    WorkspaceDef, CreateBatchJobDefinition
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id="XYZ",
+    secret_key="XYZ"
+)
+
+client = get_bodo_client(keys)
+
+jobrun = client.job.submit_sql_job_run(CreateSQLJobRun(
+            clusterUUID=cluster.uuid,
+            catalog="SNOWFLAKE_CATALOG",
+            sqlQueryText="SELECT * FROM PUBLIC.TABLE LIMIT 10"))
+```
+
+<br/>
+
+##### Job Run waiter<a id="job-waiter"></a>
+
+`BodoClient.job.get_waiter()`
+
+Returns a waiter object that waits until the job run uuid specified finishes.
+To wait for job run to be finished, invoke the waiter.wait() function,
+which can take the following parameters.
+
+```python3
+from typing import Callable
+def wait(
+        self,
+        uuid,
+        on_success: Callable = None,
+        on_failure: Callable = None,
+        on_timeout: Callable = None,
+        check_period=10,
+        timeout=None
+):
+  pass
+```
+
+By default returns job model if no callbacks is provided. There is option to pass callable objects as following
+parameters:
+
+- `on_success` - will be executed on succes, job object passed as argument
+- `on_failure` - will be executed on failure, job object passed as argument
+- `on_timeout` - will be executed on timeout, job_uuid passed as argument
+
+Other options are:
+
+- `check_period` - seconds between status checks
+- `timeout` - threshold in seconds after which Timeout error will be raised, `None` means no timeout
+
+**Example 1. Success/Failure callbacks:**
+```python
+from bodosdk.models import WorkspaceKeys, CreateJobRun
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id='XYZ',
+    secret_key='XYZ'
+)
+client = get_bodo_client(keys)
+input_job = CreateJobRun(clusterUUID='<cluster-uuid>', batchJobDefinitionUUID='<batch-job-definition-uuid>')
+job_run = client.job.submit_batch_job_run(input_job)
+
+waiter = client.job.get_job_run_waiter()
+
+def success_callback(job):
+    print("in success callback", job.status)
+
+def failure_callback(job):
+    print('in failure callback', job.status)
+
+result = waiter.wait(job_run.uuid, on_success=success_callback, on_failure=failure_callback)
+```
+
+**Example 2. Timeout callback:**
+```python
+from bodosdk.models import WorkspaceKeys, CreateJobRun
+from bodosdk.client import get_bodo_client
+
+keys = WorkspaceKeys(
+    client_id='XYZ',
+    secret_key='XYZ'
+)
+client = get_bodo_client(keys)
+input_job = CreateJobRun(clusterUUID='<cluster-uuid>', batchJobDefinitionUUID='<batch-job-definition-uuid>')
+job_run = client.job.submit_batch_job_run(input_job)
+
+waiter = client.job.get_job_run_waiter()
+
+def timeout_callback(job_uuid):
+    print(f'Waiter timeout for {job_uuid}')
+    return job_uuid
+
+
+result = waiter.wait(job_run.status, on_timeout=timeout_callback, timeout=1)
+```
+
+
 ### Cluster resource<a id="cluster-resource"></a>
 Module responsible for managing clusters in workspace.
 
 - [get available instance types](#available-instance-types)
 - [get available images](#available-images)
 - [create cluster](#create-cluster)
 - [list clusters](#list-clusters)
@@ -1348,9 +1833,7 @@
 keys = WorkspaceKeys(
     client_id='XYZ',
     secret_key='XYZ'
 )
 client = get_bodo_client(keys)
 secret_info: SecretInfo = client.secrets.remove("<secret-uuid>")
 ```
-
-
```

### Comparing `bodosdk-1.3.2/bodosdk.egg-info/SOURCES.txt` & `bodosdk-1.3.3/bodosdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/setup.py` & `bodosdk-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.2/versioneer.py` & `bodosdk-1.3.3/versioneer.py`

 * *Files identical despite different names*

