# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.901.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.901.tar", last modified: Mon May 29 02:27:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.902.tar", last modified: Tue May 30 00:23:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.901.tar` & `tencentcloud-sdk-python-ess-3.0.902.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    51121 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23810 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223871 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    51121 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23981 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223871 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:23:14.000000 tencentcloud-sdk-python-ess-3.0.902/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.901/README.rst` & `tencentcloud-sdk-python-ess-3.0.902/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.901/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.902/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 
 # 签署流程已有关联文档，请检查参数修改后重试。
 FAILEDOPERATION_FLOWHASDOCUMENT = 'FailedOperation.FlowHasDocument'
 
 # 流程未找到关联的电子文件信息，请检查操作步骤，检查参数，并在修改后重试。
 FAILEDOPERATION_FLOWHASNODOCUMENT = 'FailedOperation.FlowHasNoDocument'
 
+# 当前无可用的许可
+FAILEDOPERATION_LICENSENOQUOTA = 'FailedOperation.LicenseNoQuota'
+
 # 签署审核未通过，请先完成审核。
 FAILEDOPERATION_NOSIGNREVIEWPASS = 'FailedOperation.NoSignReviewPass'
 
 # 未找到集团子企业相关用户信息，请检查用户相关参数
 FAILEDOPERATION_NOTFOUNDSHADOWUSER = 'FailedOperation.NotFoundShadowUser'
 
 # 企业经营状态与工商局信息不符。
@@ -259,14 +262,17 @@
 
 # 不合法的用户名称，请修改后重试。
 INVALIDPARAMETER_NAME = 'InvalidParameter.Name'
 
 # 不支持的通知类型，请检查并联系客服处理。
 INVALIDPARAMETER_NOTIFYTYPE = 'InvalidParameter.NotifyType'
 
+# 参数Offset不正确
+INVALIDPARAMETER_OFFSET = 'InvalidParameter.Offset'
+
 # 不合法的企业名称，请修改后重试。
 INVALIDPARAMETER_ORGANIZATIONNAME = 'InvalidParameter.OrganizationName'
 
 # 参数错误。
 INVALIDPARAMETER_PARAMERROR = 'InvalidParameter.ParamError'
 
 # 个人静默签Tag未设置，请检查后重试。
```

### Comparing `tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.902/tencentcloud/ess/v20201111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.901/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.902/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.901/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.902/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.901/setup.py` & `tencentcloud-sdk-python-ess-3.0.902/setup.py`

 * *Files identical despite different names*

