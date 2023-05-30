# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.901.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.901.tar", last modified: Mon May 29 02:24:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.902.tar", last modified: Tue May 30 00:20:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.901.tar` & `tencentcloud-sdk-python-cvm-3.0.902.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud/cvm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)   119300 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)    42926 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   430455 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud/cvm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:24:37.000000 tencentcloud-sdk-python-cvm-3.0.901/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud/cvm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   119300 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)    43023 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   430455 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud/cvm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:20:28.000000 tencentcloud-sdk-python-cvm-3.0.902/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.901/README.rst` & `tencentcloud-sdk-python-cvm-3.0.902/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.901/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.902/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.901/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.902/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,17 @@
 
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
 # 最多指定一个参数。
 INVALIDPARAMETER_ATMOSTONE = 'InvalidParameter.AtMostOne'
 
+# 不支持参数CdcId。
+INVALIDPARAMETER_CDCNOTSUPPORTED = 'InvalidParameter.CdcNotSupported'
+
 # DataDiskIds不应该传入RootDisk的Id。
 INVALIDPARAMETER_DATADISKIDCONTAINSROOTDISK = 'InvalidParameter.DataDiskIdContainsRootDisk'
 
 # 指定的数据盘不属于指定的实例。
 INVALIDPARAMETER_DATADISKNOTBELONGSPECIFIEDINSTANCE = 'InvalidParameter.DataDiskNotBelongSpecifiedInstance'
 
 # 只能包含一个系统盘快照。
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.901/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.902/tencentcloud/cvm/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.901/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.902/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.901'
+__version__ = '3.0.902'
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.901/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.902/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.901/setup.py` & `tencentcloud-sdk-python-cvm-3.0.902/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.901/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.902/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

