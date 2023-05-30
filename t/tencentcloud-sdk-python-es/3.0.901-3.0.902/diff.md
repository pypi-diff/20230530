# Comparing `tmp/tencentcloud-sdk-python-es-3.0.901.tar.gz` & `tmp/tencentcloud-sdk-python-es-3.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-es-3.0.901.tar", last modified: Mon May 29 02:27:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-es-3.0.902.tar", last modified: Tue May 30 00:23:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-es-3.0.901.tar` & `tencentcloud-sdk-python-es-3.0.902.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/
--rw-r--r--   0 root         (0) root         (0)      734 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud/es/v20180416/
--rw-r--r--   0 root         (0) root         (0)    35037 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud/es/v20180416/es_client.py
--rw-r--r--   0 root         (0) root         (0)     3332 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud/es/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud/es/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   177851 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud/es/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud/es/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud_sdk_python_es.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud_sdk_python_es.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud_sdk_python_es.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud_sdk_python_es.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/tencentcloud_sdk_python_es.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1004 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:27:32.000000 tencentcloud-sdk-python-es-3.0.901/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/
+-rw-r--r--   0 root         (0) root         (0)      734 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud/es/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    35037 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud/es/v20180416/es_client.py
+-rw-r--r--   0 root         (0) root         (0)     3342 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud/es/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud/es/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   177851 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud/es/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud/es/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud_sdk_python_es.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud_sdk_python_es.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud_sdk_python_es.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud_sdk_python_es.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/tencentcloud_sdk_python_es.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:23:08.000000 tencentcloud-sdk-python-es-3.0.902/setup.cfg
```

### Comparing `tencentcloud-sdk-python-es-3.0.901/README.rst` & `tencentcloud-sdk-python-es-3.0.902/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.901/tencentcloud/es/v20180416/es_client.py` & `tencentcloud-sdk-python-es-3.0.902/tencentcloud/es/v20180416/es_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.901/tencentcloud/es/v20180416/errorcodes.py` & `tencentcloud-sdk-python-es-3.0.902/tencentcloud/es/v20180416/errorcodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,21 +41,21 @@
 # 账户未绑定信用卡或paypal，无法支付。
 FAILEDOPERATION_NOPAYMENT = 'FailedOperation.NoPayment'
 
 # 用户未实名认证。
 FAILEDOPERATION_NOTAUTHENTICATED = 'FailedOperation.NotAuthenticated'
 
 # 不支持在滚动重启扩容计算资源同时扩容磁盘数量。
-FAILEDOPERATION_UNSUPPORTRESETNODETYPEANDSCALEOUTDISK = 'FailedOperation.UnsupportResetNodeTypeAndScaleoutDisk'
+FAILEDOPERATION_UNSUPPORTEDRESETNODETYPEANDSCALEOUTDISK = 'FailedOperation.UnsupportedResetNodeTypeAndScaleOutDisk'
 
 # 不支持在滚动重启缩容计算资源同时修改磁盘大小
-FAILEDOPERATION_UNSUPPORTRESETSCALEDOWNANDMODIFYDISK = 'FailedOperation.UnsupportResetScaledownAndModifyDisk'
+FAILEDOPERATION_UNSUPPORTEDRESTSCALEDOWNANDMODIFYDISK = 'FailedOperation.UnsupportedRestScaleDownAndModifyDisk'
 
 # 不支持反向调节节点配置和磁盘容量。
-FAILEDOPERATION_UNSUPPORTREVERSEREGULATIONNODETYPEANDDISK = 'FailedOperation.UnsupportReverseRegulationNodeTypeAndDisk'
+FAILEDOPERATION_UNSUPPORTEDREVERSEREGULATIONNODETYPEANDDISK = 'FailedOperation.UnsupportedReverseRegulationNodeTypeAndDisk'
 
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
```

### Comparing `tencentcloud-sdk-python-es-3.0.901/tencentcloud/es/v20180416/models.py` & `tencentcloud-sdk-python-es-3.0.902/tencentcloud/es/v20180416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.901/tencentcloud/__init__.py` & `tencentcloud-sdk-python-es-3.0.902/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-es-3.0.901/PKG-INFO` & `tencentcloud-sdk-python-es-3.0.902/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-es
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Es SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-es-3.0.901/tencentcloud_sdk_python_es.egg-info/PKG-INFO` & `tencentcloud-sdk-python-es-3.0.902/tencentcloud_sdk_python_es.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-es
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Es SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-es-3.0.901/setup.py` & `tencentcloud-sdk-python-es-3.0.902/setup.py`

 * *Files identical despite different names*

