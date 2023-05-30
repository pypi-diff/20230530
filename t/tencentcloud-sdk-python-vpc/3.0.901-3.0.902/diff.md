# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.901.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.901.tar", last modified: Mon May 29 02:41:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.902.tar", last modified: Tue May 30 00:37:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.901.tar` & `tencentcloud-sdk-python-vpc-3.0.902.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   332331 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    41601 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   851805 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:41:13.000000 tencentcloud-sdk-python-vpc-3.0.901/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   332331 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    41624 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   851805 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:37:05.000000 tencentcloud-sdk-python-vpc-3.0.902/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.901/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.902/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.901/README.rst` & `tencentcloud-sdk-python-vpc-3.0.902/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.901/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.902/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.901/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.902/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,23 +142,23 @@
 
 # 该地址不可与此实例申请。
 INVALIDPARAMETERVALUE_ADDRESSNOTAPPLICABLE = 'InvalidParameterValue.AddressNotApplicable'
 
 # 该地址不是CalcIP。
 INVALIDPARAMETERVALUE_ADDRESSNOTCALCIP = 'InvalidParameterValue.AddressNotCalcIP'
 
-# 该地址不是EIP。
-INVALIDPARAMETERVALUE_ADDRESSNOTEIP = 'InvalidParameterValue.AddressNotEIP'
-
 # 未找到该地址。
 INVALIDPARAMETERVALUE_ADDRESSNOTFOUND = 'InvalidParameterValue.AddressNotFound'
 
 # 该IPv6地址已经发布。
 INVALIDPARAMETERVALUE_ADDRESSPUBLISHED = 'InvalidParameterValue.AddressPublished'
 
+# 当前IP地址类型不正确。
+INVALIDPARAMETERVALUE_ADDRESSTYPECONFLICT = 'InvalidParameterValue.AddressTypeConflict'
+
 # 带宽超出限制。
 INVALIDPARAMETERVALUE_BANDWIDTHOUTOFRANGE = 'InvalidParameterValue.BandwidthOutOfRange'
 
 # 带宽包ID不正确。
 INVALIDPARAMETERVALUE_BANDWIDTHPACKAGEIDMALFORMED = 'InvalidParameterValue.BandwidthPackageIdMalformed'
 
 # 该带宽包正在被使用。
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.901/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.902/tencentcloud/vpc/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.901/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.902/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.901/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.902/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.901/setup.py` & `tencentcloud-sdk-python-vpc-3.0.902/setup.py`

 * *Files identical despite different names*

