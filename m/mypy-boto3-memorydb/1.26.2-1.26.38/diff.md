# Comparing `tmp/mypy-boto3-memorydb-1.26.2.tar.gz` & `tmp/mypy-boto3-memorydb-1.26.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-memorydb-1.26.2.tar", last modified: Thu Nov  3 19:33:03 2022, max compression
+gzip compressed data, was "mypy-boto3-memorydb-1.26.38.tar", last modified: Tue Dec 27 20:32:14 2022, max compression
```

## Comparing `mypy-boto3-memorydb-1.26.2.tar` & `mypy-boto3-memorydb-1.26.38.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:33:03.735172 mypy-boto3-memorydb-1.26.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-03 19:32:34.000000 mypy-boto3-memorydb-1.26.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15669 2022-11-03 19:33:03.731172 mypy-boto3-memorydb-1.26.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14230 2022-11-03 19:32:34.000000 mypy-boto3-memorydb-1.26.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:33:03.731172 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-11-03 19:32:34.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-11-03 19:32:34.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-11-03 19:32:34.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27885 2022-11-03 19:32:34.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    27844 2022-11-03 19:32:34.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7779 2022-11-03 19:32:34.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7777 2022-11-03 19:32:34.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 19:32:34.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    32704 2022-11-03 19:32:35.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    32673 2022-11-03 19:32:34.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-03 19:32:34.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:33:03.731172 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15669 2022-11-03 19:33:03.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-11-03 19:33:03.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 19:33:03.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 19:33:03.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-03 19:33:03.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-03 19:33:03.000000 mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-03 19:33:03.735172 mypy-boto3-memorydb-1.26.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-11-03 19:32:34.000000 mypy-boto3-memorydb-1.26.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 20:32:14.245875 mypy-boto3-memorydb-1.26.38/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19683 2022-12-27 20:32:14.245875 mypy-boto3-memorydb-1.26.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18192 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 20:32:14.245875 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36305 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36248 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9903 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15150 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41309 2022-12-27 20:32:03.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41274 2022-12-27 20:32:03.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 20:32:14.245875 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19683 2022-12-27 20:32:14.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2022-12-27 20:32:14.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 20:32:14.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 20:32:14.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-27 20:32:14.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-27 20:32:14.000000 mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-27 20:32:14.245875 mypy-boto3-memorydb-1.26.38/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2022-12-27 20:32:02.000000 mypy-boto3-memorydb-1.26.38/setup.py
```

### Comparing `mypy-boto3-memorydb-1.26.2/LICENSE` & `mypy-boto3-memorydb-1.26.38/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.26.2/PKG-INFO` & `mypy-boto3-memorydb-1.26.38/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-memorydb
-Version: 1.26.2
-Summary: Type annotations for boto3.MemoryDB 1.26.2 service generated with mypy-boto3-builder 7.11.10
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 memorydb type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-memorydb"></a>
 
 # mypy-boto3-memorydb
 
 [![PyPI - mypy-boto3-memorydb](https://img.shields.io/pypi/v/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-memorydb?color=blue)](https://pypistats.org/packages/mypy-boto3-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MemoryDB 1.26.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[boto3.MemoryDB 1.26.38](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-memorydb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -71,14 +40,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -265,33 +235,106 @@
 from mypy_boto3_memorydb import MemoryDBClient
 
 client: MemoryDBClient = Session().client("memorydb")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_memorydb.paginator` module contains type annotations for all
+paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_memorydb import MemoryDBClient
+from mypy_boto3_memorydb.paginator import (
+    DescribeACLsPaginator,
+    DescribeClustersPaginator,
+    DescribeEngineVersionsPaginator,
+    DescribeEventsPaginator,
+    DescribeParameterGroupsPaginator,
+    DescribeParametersPaginator,
+    DescribeReservedNodesPaginator,
+    DescribeReservedNodesOfferingsPaginator,
+    DescribeServiceUpdatesPaginator,
+    DescribeSnapshotsPaginator,
+    DescribeSubnetGroupsPaginator,
+    DescribeUsersPaginator,
+)
+
+client: MemoryDBClient = Session().client("memorydb")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+describe_acls_paginator: DescribeACLsPaginator = client.get_paginator("describe_acls")
+describe_clusters_paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")
+describe_engine_versions_paginator: DescribeEngineVersionsPaginator = client.get_paginator(
+    "describe_engine_versions"
+)
+describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
+describe_parameter_groups_paginator: DescribeParameterGroupsPaginator = client.get_paginator(
+    "describe_parameter_groups"
+)
+describe_parameters_paginator: DescribeParametersPaginator = client.get_paginator(
+    "describe_parameters"
+)
+describe_reserved_nodes_paginator: DescribeReservedNodesPaginator = client.get_paginator(
+    "describe_reserved_nodes"
+)
+describe_reserved_nodes_offerings_paginator: DescribeReservedNodesOfferingsPaginator = (
+    client.get_paginator("describe_reserved_nodes_offerings")
+)
+describe_service_updates_paginator: DescribeServiceUpdatesPaginator = client.get_paginator(
+    "describe_service_updates"
+)
+describe_snapshots_paginator: DescribeSnapshotsPaginator = client.get_paginator(
+    "describe_snapshots"
+)
+describe_subnet_groups_paginator: DescribeSubnetGroupsPaginator = client.get_paginator(
+    "describe_subnet_groups"
+)
+describe_users_paginator: DescribeUsersPaginator = client.get_paginator("describe_users")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_memorydb.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_memorydb.literals import (
     AZStatusType,
     AuthenticationTypeType,
     DataTieringStatusType,
+    DescribeACLsPaginatorName,
+    DescribeClustersPaginatorName,
+    DescribeEngineVersionsPaginatorName,
+    DescribeEventsPaginatorName,
+    DescribeParameterGroupsPaginatorName,
+    DescribeParametersPaginatorName,
+    DescribeReservedNodesOfferingsPaginatorName,
+    DescribeReservedNodesPaginatorName,
+    DescribeServiceUpdatesPaginatorName,
+    DescribeSnapshotsPaginatorName,
+    DescribeSubnetGroupsPaginatorName,
+    DescribeUsersPaginatorName,
     InputAuthenticationTypeType,
     ServiceUpdateStatusType,
     ServiceUpdateTypeType,
     SourceTypeType,
     MemoryDBServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
     RegionName,
 )
 
 
 def check_value(value: AZStatusType) -> bool:
     ...
 ```
@@ -320,32 +363,36 @@
     ParameterGroupTypeDef,
     DeleteACLRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     DescribeACLsRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeEngineVersionsRequestRequestTypeDef,
     EngineVersionInfoTypeDef,
     DescribeEventsRequestRequestTypeDef,
     EventTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
     DescribeParametersRequestRequestTypeDef,
     ParameterTypeDef,
+    DescribeReservedNodesOfferingsRequestRequestTypeDef,
+    DescribeReservedNodesRequestRequestTypeDef,
     DescribeServiceUpdatesRequestRequestTypeDef,
     ServiceUpdateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     FilterTypeDef,
     FailoverShardRequestRequestTypeDef,
     ListAllowedNodeTypeUpdatesRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ParameterNameValueTypeDef,
+    RecurringChargeTypeDef,
     ReplicaConfigurationRequestTypeDef,
     ResetParameterGroupRequestRequestTypeDef,
     SlotMigrationTypeDef,
     ShardConfigurationRequestTypeDef,
     ShardConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateACLRequestRequestTypeDef,
@@ -361,41 +408,59 @@
     CreateACLRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     ListTagsResponseTypeDef,
+    PurchaseReservedNodesOfferingRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TagResourceResponseTypeDef,
     UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DeleteParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     ResetParameterGroupResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
+    DescribeACLsRequestDescribeACLsPaginateTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
+    DescribeParametersRequestDescribeParametersPaginateTypeDef,
+    DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef,
+    DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef,
+    DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef,
+    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
+    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeEngineVersionsResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParametersResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
+    ReservedNodeTypeDef,
+    ReservedNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     UpdateClusterRequestRequestTypeDef,
     ShardDetailTypeDef,
     CreateACLResponseTypeDef,
     DeleteACLResponseTypeDef,
     DescribeACLsResponseTypeDef,
     UpdateACLResponseTypeDef,
     CreateUserResponseTypeDef,
     DeleteUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     UpdateUserResponseTypeDef,
     SubnetGroupTypeDef,
     ShardTypeDef,
+    DescribeReservedNodesResponseTypeDef,
+    PurchaseReservedNodesOfferingResponseTypeDef,
+    DescribeReservedNodesOfferingsResponseTypeDef,
     ClusterPendingUpdatesTypeDef,
     ClusterConfigurationTypeDef,
     CreateSubnetGroupResponseTypeDef,
     DeleteSubnetGroupResponseTypeDef,
     DescribeSubnetGroupsResponseTypeDef,
     UpdateSubnetGroupResponseTypeDef,
     ClusterTypeDef,
```

### Comparing `mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/__main__.py` & `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MemoryDB 1.26.2\nVersion:         1.26.2\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.MemoryDB 1.26.38\nVersion:         1.26.38\nBuilder version:"
+        " 7.12.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.2")
+    print("1.26.38")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/client.py` & `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,20 +9,35 @@
     from boto3.session import Session
     from mypy_boto3_memorydb.client import MemoryDBClient
 
     session = Session()
     client: MemoryDBClient = session.client("memorydb")
     ```
 """
+import sys
 from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ServiceUpdateStatusType, SourceTypeType
+from .paginator import (
+    DescribeACLsPaginator,
+    DescribeClustersPaginator,
+    DescribeEngineVersionsPaginator,
+    DescribeEventsPaginator,
+    DescribeParameterGroupsPaginator,
+    DescribeParametersPaginator,
+    DescribeReservedNodesOfferingsPaginator,
+    DescribeReservedNodesPaginator,
+    DescribeServiceUpdatesPaginator,
+    DescribeSnapshotsPaginator,
+    DescribeSubnetGroupsPaginator,
+    DescribeUsersPaginator,
+)
 from .type_defs import (
     AuthenticationModeTypeDef,
     BatchUpdateClusterResponseTypeDef,
     CopySnapshotResponseTypeDef,
     CreateACLResponseTypeDef,
     CreateClusterResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
@@ -37,37 +52,46 @@
     DeleteUserResponseTypeDef,
     DescribeACLsResponseTypeDef,
     DescribeClustersResponseTypeDef,
     DescribeEngineVersionsResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     DescribeParametersResponseTypeDef,
+    DescribeReservedNodesOfferingsResponseTypeDef,
+    DescribeReservedNodesResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
     DescribeSnapshotsResponseTypeDef,
     DescribeSubnetGroupsResponseTypeDef,
     DescribeUsersResponseTypeDef,
     FailoverShardResponseTypeDef,
     FilterTypeDef,
     ListAllowedNodeTypeUpdatesResponseTypeDef,
     ListTagsResponseTypeDef,
     ParameterNameValueTypeDef,
+    PurchaseReservedNodesOfferingResponseTypeDef,
     ReplicaConfigurationRequestTypeDef,
     ResetParameterGroupResponseTypeDef,
     ServiceUpdateRequestTypeDef,
     ShardConfigurationRequestTypeDef,
     TagResourceResponseTypeDef,
     TagTypeDef,
     UntagResourceResponseTypeDef,
     UpdateACLResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     UpdateSubnetGroupResponseTypeDef,
     UpdateUserResponseTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
+
 __all__ = ("MemoryDBClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -102,14 +126,18 @@
     InvalidVPCNetworkStateFault: Type[BotocoreClientError]
     NoOperationFault: Type[BotocoreClientError]
     NodeQuotaForClusterExceededFault: Type[BotocoreClientError]
     NodeQuotaForCustomerExceededFault: Type[BotocoreClientError]
     ParameterGroupAlreadyExistsFault: Type[BotocoreClientError]
     ParameterGroupNotFoundFault: Type[BotocoreClientError]
     ParameterGroupQuotaExceededFault: Type[BotocoreClientError]
+    ReservedNodeAlreadyExistsFault: Type[BotocoreClientError]
+    ReservedNodeNotFoundFault: Type[BotocoreClientError]
+    ReservedNodeQuotaExceededFault: Type[BotocoreClientError]
+    ReservedNodesOfferingNotFoundFault: Type[BotocoreClientError]
     ServiceLinkedRoleNotFoundFault: Type[BotocoreClientError]
     ServiceUpdateNotFoundFault: Type[BotocoreClientError]
     ShardNotFoundFault: Type[BotocoreClientError]
     ShardsPerClusterQuotaExceededFault: Type[BotocoreClientError]
     SnapshotAlreadyExistsFault: Type[BotocoreClientError]
     SnapshotNotFoundFault: Type[BotocoreClientError]
     SnapshotQuotaExceededFault: Type[BotocoreClientError]
@@ -419,14 +447,50 @@
         """
         Returns the detailed parameter list for a particular parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_parameters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#describe_parameters)
         """
 
+    def describe_reserved_nodes(
+        self,
+        *,
+        ReservationId: str = ...,
+        ReservedNodesOfferingId: str = ...,
+        NodeType: str = ...,
+        Duration: str = ...,
+        OfferingType: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeReservedNodesResponseTypeDef:
+        """
+        Returns information about reserved nodes for this account, or about a specified
+        reserved node.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_reserved_nodes)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#describe_reserved_nodes)
+        """
+
+    def describe_reserved_nodes_offerings(
+        self,
+        *,
+        ReservedNodesOfferingId: str = ...,
+        NodeType: str = ...,
+        Duration: str = ...,
+        OfferingType: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeReservedNodesOfferingsResponseTypeDef:
+        """
+        Lists available reserved node offerings.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_reserved_nodes_offerings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#describe_reserved_nodes_offerings)
+        """
+
     def describe_service_updates(
         self,
         *,
         ServiceUpdateName: str = ...,
         ClusterNames: Sequence[str] = ...,
         Status: Sequence[ServiceUpdateStatusType] = ...,
         MaxResults: int = ...,
@@ -519,14 +583,29 @@
         """
         Lists all tags currently on a named resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.list_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#list_tags)
         """
 
+    def purchase_reserved_nodes_offering(
+        self,
+        *,
+        ReservedNodesOfferingId: str,
+        ReservationId: str = ...,
+        NodeCount: int = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> PurchaseReservedNodesOfferingResponseTypeDef:
+        """
+        Allows you to purchase a reserved node offering.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.purchase_reserved_nodes_offering)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#purchase_reserved_nodes_offering)
+        """
+
     def reset_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         AllParameters: bool = ...,
         ParameterNames: Sequence[str] = ...
     ) -> ResetParameterGroupResponseTypeDef:
@@ -627,7 +706,109 @@
     ) -> UpdateUserResponseTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.update_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#update_user)
         """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["describe_acls"]) -> DescribeACLsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_clusters"]
+    ) -> DescribeClustersPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_engine_versions"]
+    ) -> DescribeEngineVersionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["describe_events"]) -> DescribeEventsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_parameter_groups"]
+    ) -> DescribeParameterGroupsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_parameters"]
+    ) -> DescribeParametersPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_reserved_nodes"]
+    ) -> DescribeReservedNodesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_reserved_nodes_offerings"]
+    ) -> DescribeReservedNodesOfferingsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_service_updates"]
+    ) -> DescribeServiceUpdatesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_snapshots"]
+    ) -> DescribeSnapshotsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_subnet_groups"]
+    ) -> DescribeSubnetGroupsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["describe_users"]) -> DescribeUsersPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/client.pyi` & `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/client.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -9,20 +9,35 @@
     from boto3.session import Session
     from mypy_boto3_memorydb.client import MemoryDBClient
 
     session = Session()
     client: MemoryDBClient = session.client("memorydb")
     ```
 """
+import sys
 from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ServiceUpdateStatusType, SourceTypeType
+from .paginator import (
+    DescribeACLsPaginator,
+    DescribeClustersPaginator,
+    DescribeEngineVersionsPaginator,
+    DescribeEventsPaginator,
+    DescribeParameterGroupsPaginator,
+    DescribeParametersPaginator,
+    DescribeReservedNodesOfferingsPaginator,
+    DescribeReservedNodesPaginator,
+    DescribeServiceUpdatesPaginator,
+    DescribeSnapshotsPaginator,
+    DescribeSubnetGroupsPaginator,
+    DescribeUsersPaginator,
+)
 from .type_defs import (
     AuthenticationModeTypeDef,
     BatchUpdateClusterResponseTypeDef,
     CopySnapshotResponseTypeDef,
     CreateACLResponseTypeDef,
     CreateClusterResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
@@ -37,37 +52,45 @@
     DeleteUserResponseTypeDef,
     DescribeACLsResponseTypeDef,
     DescribeClustersResponseTypeDef,
     DescribeEngineVersionsResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     DescribeParametersResponseTypeDef,
+    DescribeReservedNodesOfferingsResponseTypeDef,
+    DescribeReservedNodesResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
     DescribeSnapshotsResponseTypeDef,
     DescribeSubnetGroupsResponseTypeDef,
     DescribeUsersResponseTypeDef,
     FailoverShardResponseTypeDef,
     FilterTypeDef,
     ListAllowedNodeTypeUpdatesResponseTypeDef,
     ListTagsResponseTypeDef,
     ParameterNameValueTypeDef,
+    PurchaseReservedNodesOfferingResponseTypeDef,
     ReplicaConfigurationRequestTypeDef,
     ResetParameterGroupResponseTypeDef,
     ServiceUpdateRequestTypeDef,
     ShardConfigurationRequestTypeDef,
     TagResourceResponseTypeDef,
     TagTypeDef,
     UntagResourceResponseTypeDef,
     UpdateACLResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     UpdateSubnetGroupResponseTypeDef,
     UpdateUserResponseTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 __all__ = ("MemoryDBClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
@@ -100,14 +123,18 @@
     InvalidVPCNetworkStateFault: Type[BotocoreClientError]
     NoOperationFault: Type[BotocoreClientError]
     NodeQuotaForClusterExceededFault: Type[BotocoreClientError]
     NodeQuotaForCustomerExceededFault: Type[BotocoreClientError]
     ParameterGroupAlreadyExistsFault: Type[BotocoreClientError]
     ParameterGroupNotFoundFault: Type[BotocoreClientError]
     ParameterGroupQuotaExceededFault: Type[BotocoreClientError]
+    ReservedNodeAlreadyExistsFault: Type[BotocoreClientError]
+    ReservedNodeNotFoundFault: Type[BotocoreClientError]
+    ReservedNodeQuotaExceededFault: Type[BotocoreClientError]
+    ReservedNodesOfferingNotFoundFault: Type[BotocoreClientError]
     ServiceLinkedRoleNotFoundFault: Type[BotocoreClientError]
     ServiceUpdateNotFoundFault: Type[BotocoreClientError]
     ShardNotFoundFault: Type[BotocoreClientError]
     ShardsPerClusterQuotaExceededFault: Type[BotocoreClientError]
     SnapshotAlreadyExistsFault: Type[BotocoreClientError]
     SnapshotNotFoundFault: Type[BotocoreClientError]
     SnapshotQuotaExceededFault: Type[BotocoreClientError]
@@ -393,14 +420,48 @@
     ) -> DescribeParametersResponseTypeDef:
         """
         Returns the detailed parameter list for a particular parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_parameters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#describe_parameters)
         """
+    def describe_reserved_nodes(
+        self,
+        *,
+        ReservationId: str = ...,
+        ReservedNodesOfferingId: str = ...,
+        NodeType: str = ...,
+        Duration: str = ...,
+        OfferingType: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeReservedNodesResponseTypeDef:
+        """
+        Returns information about reserved nodes for this account, or about a specified
+        reserved node.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_reserved_nodes)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#describe_reserved_nodes)
+        """
+    def describe_reserved_nodes_offerings(
+        self,
+        *,
+        ReservedNodesOfferingId: str = ...,
+        NodeType: str = ...,
+        Duration: str = ...,
+        OfferingType: str = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> DescribeReservedNodesOfferingsResponseTypeDef:
+        """
+        Lists available reserved node offerings.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_reserved_nodes_offerings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#describe_reserved_nodes_offerings)
+        """
     def describe_service_updates(
         self,
         *,
         ServiceUpdateName: str = ...,
         ClusterNames: Sequence[str] = ...,
         Status: Sequence[ServiceUpdateStatusType] = ...,
         MaxResults: int = ...,
@@ -485,14 +546,28 @@
     def list_tags(self, *, ResourceArn: str) -> ListTagsResponseTypeDef:
         """
         Lists all tags currently on a named resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.list_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#list_tags)
         """
+    def purchase_reserved_nodes_offering(
+        self,
+        *,
+        ReservedNodesOfferingId: str,
+        ReservationId: str = ...,
+        NodeCount: int = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> PurchaseReservedNodesOfferingResponseTypeDef:
+        """
+        Allows you to purchase a reserved node offering.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.purchase_reserved_nodes_offering)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#purchase_reserved_nodes_offering)
+        """
     def reset_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         AllParameters: bool = ...,
         ParameterNames: Sequence[str] = ...
     ) -> ResetParameterGroupResponseTypeDef:
@@ -586,7 +661,97 @@
     ) -> UpdateUserResponseTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.update_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#update_user)
         """
+    @overload
+    def get_paginator(self, operation_name: Literal["describe_acls"]) -> DescribeACLsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_clusters"]
+    ) -> DescribeClustersPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_engine_versions"]
+    ) -> DescribeEngineVersionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(self, operation_name: Literal["describe_events"]) -> DescribeEventsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_parameter_groups"]
+    ) -> DescribeParameterGroupsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_parameters"]
+    ) -> DescribeParametersPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_reserved_nodes"]
+    ) -> DescribeReservedNodesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_reserved_nodes_offerings"]
+    ) -> DescribeReservedNodesOfferingsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_service_updates"]
+    ) -> DescribeServiceUpdatesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_snapshots"]
+    ) -> DescribeSnapshotsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
+        self, operation_name: Literal["describe_subnet_groups"]
+    ) -> DescribeSubnetGroupsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(self, operation_name: Literal["describe_users"]) -> DescribeUsersPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/literals.py` & `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/literals.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,28 +19,53 @@
     from typing_extensions import Literal
 
 
 __all__ = (
     "AZStatusType",
     "AuthenticationTypeType",
     "DataTieringStatusType",
+    "DescribeACLsPaginatorName",
+    "DescribeClustersPaginatorName",
+    "DescribeEngineVersionsPaginatorName",
+    "DescribeEventsPaginatorName",
+    "DescribeParameterGroupsPaginatorName",
+    "DescribeParametersPaginatorName",
+    "DescribeReservedNodesOfferingsPaginatorName",
+    "DescribeReservedNodesPaginatorName",
+    "DescribeServiceUpdatesPaginatorName",
+    "DescribeSnapshotsPaginatorName",
+    "DescribeSubnetGroupsPaginatorName",
+    "DescribeUsersPaginatorName",
     "InputAuthenticationTypeType",
     "ServiceUpdateStatusType",
     "ServiceUpdateTypeType",
     "SourceTypeType",
     "MemoryDBServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
     "RegionName",
 )
 
 
 AZStatusType = Literal["multiaz", "singleaz"]
 AuthenticationTypeType = Literal["no-password", "password"]
 DataTieringStatusType = Literal["false", "true"]
+DescribeACLsPaginatorName = Literal["describe_acls"]
+DescribeClustersPaginatorName = Literal["describe_clusters"]
+DescribeEngineVersionsPaginatorName = Literal["describe_engine_versions"]
+DescribeEventsPaginatorName = Literal["describe_events"]
+DescribeParameterGroupsPaginatorName = Literal["describe_parameter_groups"]
+DescribeParametersPaginatorName = Literal["describe_parameters"]
+DescribeReservedNodesOfferingsPaginatorName = Literal["describe_reserved_nodes_offerings"]
+DescribeReservedNodesPaginatorName = Literal["describe_reserved_nodes"]
+DescribeServiceUpdatesPaginatorName = Literal["describe_service_updates"]
+DescribeSnapshotsPaginatorName = Literal["describe_snapshots"]
+DescribeSubnetGroupsPaginatorName = Literal["describe_subnet_groups"]
+DescribeUsersPaginatorName = Literal["describe_users"]
 InputAuthenticationTypeType = Literal["password"]
 ServiceUpdateStatusType = Literal["available", "complete", "in-progress", "scheduled"]
 ServiceUpdateTypeType = Literal["security-update"]
 SourceTypeType = Literal["acl", "cluster", "node", "parameter-group", "subnet-group", "user"]
 MemoryDBServiceName = Literal["memorydb"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -62,14 +87,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -79,27 +105,29 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -128,14 +156,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -183,14 +212,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -206,25 +236,27 @@
     "kafkaconnect",
     "kendra",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -256,28 +288,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -286,14 +322,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -304,38 +341,44 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
@@ -370,25 +413,41 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal[
+    "describe_acls",
+    "describe_clusters",
+    "describe_engine_versions",
+    "describe_events",
+    "describe_parameter_groups",
+    "describe_parameters",
+    "describe_reserved_nodes",
+    "describe_reserved_nodes_offerings",
+    "describe_service_updates",
+    "describe_snapshots",
+    "describe_subnet_groups",
+    "describe_users",
+]
 RegionName = Literal[
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
+    "eu-south-1",
     "eu-west-1",
     "eu-west-2",
+    "eu-west-3",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb/literals.pyi` & `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb/literals.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -18,27 +18,52 @@
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AZStatusType",
     "AuthenticationTypeType",
     "DataTieringStatusType",
+    "DescribeACLsPaginatorName",
+    "DescribeClustersPaginatorName",
+    "DescribeEngineVersionsPaginatorName",
+    "DescribeEventsPaginatorName",
+    "DescribeParameterGroupsPaginatorName",
+    "DescribeParametersPaginatorName",
+    "DescribeReservedNodesOfferingsPaginatorName",
+    "DescribeReservedNodesPaginatorName",
+    "DescribeServiceUpdatesPaginatorName",
+    "DescribeSnapshotsPaginatorName",
+    "DescribeSubnetGroupsPaginatorName",
+    "DescribeUsersPaginatorName",
     "InputAuthenticationTypeType",
     "ServiceUpdateStatusType",
     "ServiceUpdateTypeType",
     "SourceTypeType",
     "MemoryDBServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
     "RegionName",
 )
 
 AZStatusType = Literal["multiaz", "singleaz"]
 AuthenticationTypeType = Literal["no-password", "password"]
 DataTieringStatusType = Literal["false", "true"]
+DescribeACLsPaginatorName = Literal["describe_acls"]
+DescribeClustersPaginatorName = Literal["describe_clusters"]
+DescribeEngineVersionsPaginatorName = Literal["describe_engine_versions"]
+DescribeEventsPaginatorName = Literal["describe_events"]
+DescribeParameterGroupsPaginatorName = Literal["describe_parameter_groups"]
+DescribeParametersPaginatorName = Literal["describe_parameters"]
+DescribeReservedNodesOfferingsPaginatorName = Literal["describe_reserved_nodes_offerings"]
+DescribeReservedNodesPaginatorName = Literal["describe_reserved_nodes"]
+DescribeServiceUpdatesPaginatorName = Literal["describe_service_updates"]
+DescribeSnapshotsPaginatorName = Literal["describe_snapshots"]
+DescribeSubnetGroupsPaginatorName = Literal["describe_subnet_groups"]
+DescribeUsersPaginatorName = Literal["describe_users"]
 InputAuthenticationTypeType = Literal["password"]
 ServiceUpdateStatusType = Literal["available", "complete", "in-progress", "scheduled"]
 ServiceUpdateTypeType = Literal["security-update"]
 SourceTypeType = Literal["acl", "cluster", "node", "parameter-group", "subnet-group", "user"]
 MemoryDBServiceName = Literal["memorydb"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -60,14 +85,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -77,27 +103,29 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -126,14 +154,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -181,14 +210,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -204,25 +234,27 @@
     "kafkaconnect",
     "kendra",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -254,28 +286,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -284,14 +320,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -302,38 +339,44 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
@@ -368,25 +411,41 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal[
+    "describe_acls",
+    "describe_clusters",
+    "describe_engine_versions",
+    "describe_events",
+    "describe_parameter_groups",
+    "describe_parameters",
+    "describe_reserved_nodes",
+    "describe_reserved_nodes_offerings",
+    "describe_service_updates",
+    "describe_snapshots",
+    "describe_subnet_groups",
+    "describe_users",
+]
 RegionName = Literal[
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
+    "eu-south-1",
     "eu-west-1",
     "eu-west-2",
+    "eu-west-3",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb.egg-info/PKG-INFO` & `mypy-boto3-memorydb-1.26.38/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-memorydb
-Version: 1.26.2
-Summary: Type annotations for boto3.MemoryDB 1.26.2 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.38
+Summary: Type annotations for boto3.MemoryDB 1.26.38 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-memorydb?color=blue)](https://pypistats.org/packages/mypy-boto3-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MemoryDB 1.26.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[boto3.MemoryDB 1.26.38](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-memorydb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -71,14 +72,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -265,33 +267,106 @@
 from mypy_boto3_memorydb import MemoryDBClient
 
 client: MemoryDBClient = Session().client("memorydb")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_memorydb.paginator` module contains type annotations for all
+paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_memorydb import MemoryDBClient
+from mypy_boto3_memorydb.paginator import (
+    DescribeACLsPaginator,
+    DescribeClustersPaginator,
+    DescribeEngineVersionsPaginator,
+    DescribeEventsPaginator,
+    DescribeParameterGroupsPaginator,
+    DescribeParametersPaginator,
+    DescribeReservedNodesPaginator,
+    DescribeReservedNodesOfferingsPaginator,
+    DescribeServiceUpdatesPaginator,
+    DescribeSnapshotsPaginator,
+    DescribeSubnetGroupsPaginator,
+    DescribeUsersPaginator,
+)
+
+client: MemoryDBClient = Session().client("memorydb")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+describe_acls_paginator: DescribeACLsPaginator = client.get_paginator("describe_acls")
+describe_clusters_paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")
+describe_engine_versions_paginator: DescribeEngineVersionsPaginator = client.get_paginator(
+    "describe_engine_versions"
+)
+describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
+describe_parameter_groups_paginator: DescribeParameterGroupsPaginator = client.get_paginator(
+    "describe_parameter_groups"
+)
+describe_parameters_paginator: DescribeParametersPaginator = client.get_paginator(
+    "describe_parameters"
+)
+describe_reserved_nodes_paginator: DescribeReservedNodesPaginator = client.get_paginator(
+    "describe_reserved_nodes"
+)
+describe_reserved_nodes_offerings_paginator: DescribeReservedNodesOfferingsPaginator = (
+    client.get_paginator("describe_reserved_nodes_offerings")
+)
+describe_service_updates_paginator: DescribeServiceUpdatesPaginator = client.get_paginator(
+    "describe_service_updates"
+)
+describe_snapshots_paginator: DescribeSnapshotsPaginator = client.get_paginator(
+    "describe_snapshots"
+)
+describe_subnet_groups_paginator: DescribeSubnetGroupsPaginator = client.get_paginator(
+    "describe_subnet_groups"
+)
+describe_users_paginator: DescribeUsersPaginator = client.get_paginator("describe_users")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_memorydb.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_memorydb.literals import (
     AZStatusType,
     AuthenticationTypeType,
     DataTieringStatusType,
+    DescribeACLsPaginatorName,
+    DescribeClustersPaginatorName,
+    DescribeEngineVersionsPaginatorName,
+    DescribeEventsPaginatorName,
+    DescribeParameterGroupsPaginatorName,
+    DescribeParametersPaginatorName,
+    DescribeReservedNodesOfferingsPaginatorName,
+    DescribeReservedNodesPaginatorName,
+    DescribeServiceUpdatesPaginatorName,
+    DescribeSnapshotsPaginatorName,
+    DescribeSubnetGroupsPaginatorName,
+    DescribeUsersPaginatorName,
     InputAuthenticationTypeType,
     ServiceUpdateStatusType,
     ServiceUpdateTypeType,
     SourceTypeType,
     MemoryDBServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
     RegionName,
 )
 
 
 def check_value(value: AZStatusType) -> bool:
     ...
 ```
@@ -320,32 +395,36 @@
     ParameterGroupTypeDef,
     DeleteACLRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     DescribeACLsRequestRequestTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeEngineVersionsRequestRequestTypeDef,
     EngineVersionInfoTypeDef,
     DescribeEventsRequestRequestTypeDef,
     EventTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
     DescribeParametersRequestRequestTypeDef,
     ParameterTypeDef,
+    DescribeReservedNodesOfferingsRequestRequestTypeDef,
+    DescribeReservedNodesRequestRequestTypeDef,
     DescribeServiceUpdatesRequestRequestTypeDef,
     ServiceUpdateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     FilterTypeDef,
     FailoverShardRequestRequestTypeDef,
     ListAllowedNodeTypeUpdatesRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ParameterNameValueTypeDef,
+    RecurringChargeTypeDef,
     ReplicaConfigurationRequestTypeDef,
     ResetParameterGroupRequestRequestTypeDef,
     SlotMigrationTypeDef,
     ShardConfigurationRequestTypeDef,
     ShardConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateACLRequestRequestTypeDef,
@@ -361,41 +440,59 @@
     CreateACLRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     ListTagsResponseTypeDef,
+    PurchaseReservedNodesOfferingRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TagResourceResponseTypeDef,
     UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DeleteParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     ResetParameterGroupResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
+    DescribeACLsRequestDescribeACLsPaginateTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
+    DescribeParametersRequestDescribeParametersPaginateTypeDef,
+    DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef,
+    DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef,
+    DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef,
+    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
+    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeEngineVersionsResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParametersResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
+    ReservedNodeTypeDef,
+    ReservedNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     UpdateClusterRequestRequestTypeDef,
     ShardDetailTypeDef,
     CreateACLResponseTypeDef,
     DeleteACLResponseTypeDef,
     DescribeACLsResponseTypeDef,
     UpdateACLResponseTypeDef,
     CreateUserResponseTypeDef,
     DeleteUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     UpdateUserResponseTypeDef,
     SubnetGroupTypeDef,
     ShardTypeDef,
+    DescribeReservedNodesResponseTypeDef,
+    PurchaseReservedNodesOfferingResponseTypeDef,
+    DescribeReservedNodesOfferingsResponseTypeDef,
     ClusterPendingUpdatesTypeDef,
     ClusterConfigurationTypeDef,
     CreateSubnetGroupResponseTypeDef,
     DeleteSubnetGroupResponseTypeDef,
     DescribeSubnetGroupsResponseTypeDef,
     UpdateSubnetGroupResponseTypeDef,
     ClusterTypeDef,
```

### Comparing `mypy-boto3-memorydb-1.26.2/mypy_boto3_memorydb.egg-info/SOURCES.txt` & `mypy-boto3-memorydb-1.26.38/mypy_boto3_memorydb.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 mypy_boto3_memorydb/__init__.py
 mypy_boto3_memorydb/__init__.pyi
 mypy_boto3_memorydb/__main__.py
 mypy_boto3_memorydb/client.py
 mypy_boto3_memorydb/client.pyi
 mypy_boto3_memorydb/literals.py
 mypy_boto3_memorydb/literals.pyi
+mypy_boto3_memorydb/paginator.py
+mypy_boto3_memorydb/paginator.pyi
 mypy_boto3_memorydb/py.typed
 mypy_boto3_memorydb/type_defs.py
 mypy_boto3_memorydb/type_defs.pyi
 mypy_boto3_memorydb/version.py
 mypy_boto3_memorydb.egg-info/PKG-INFO
 mypy_boto3_memorydb.egg-info/SOURCES.txt
 mypy_boto3_memorydb.egg-info/dependency_links.txt
```

### Comparing `mypy-boto3-memorydb-1.26.2/setup.py` & `mypy-boto3-memorydb-1.26.38/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-memorydb",
-    version="1.26.2",
+    version="1.26.38",
     packages=["mypy_boto3_memorydb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MemoryDB 1.26.2 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.MemoryDB 1.26.38 service generated with mypy-boto3-builder"
+        " 7.12.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 memorydb type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_memorydb": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_memorydb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

