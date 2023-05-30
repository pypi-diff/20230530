# Comparing `tmp/tencentcloud-sdk-python-faceid-3.0.901.tar.gz` & `tmp/tencentcloud-sdk-python-faceid-3.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.901.tar", last modified: Mon May 29 02:27:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.902.tar", last modified: Tue May 30 00:23:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-faceid-3.0.901.tar` & `tencentcloud-sdk-python-faceid-3.0.902.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud/faceid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud/faceid/v20180301/
--rw-r--r--   0 root         (0) root         (0)    34030 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud/faceid/v20180301/faceid_client.py
--rw-r--r--   0 root         (0) root         (0)     9370 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud/faceid/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud/faceid/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)   141322 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud/faceid/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud/faceid/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud_sdk_python_faceid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:27:59.000000 tencentcloud-sdk-python-faceid-3.0.901/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:33.000000 tencentcloud-sdk-python-faceid-3.0.902/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-30 00:23:32.000000 tencentcloud-sdk-python-faceid-3.0.902/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:33.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:33.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud/faceid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:33.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud/faceid/v20180301/
+-rw-r--r--   0 root         (0) root         (0)    34030 2023-05-30 00:23:32.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud/faceid/v20180301/faceid_client.py
+-rw-r--r--   0 root         (0) root         (0)     9370 2023-05-30 00:23:32.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud/faceid/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:23:32.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud/faceid/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   141706 2023-05-30 00:23:32.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud/faceid/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:23:32.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud/faceid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:23:32.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-30 00:23:33.000000 tencentcloud-sdk-python-faceid-3.0.902/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-05-30 00:23:32.000000 tencentcloud-sdk-python-faceid-3.0.902/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:23:33.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud_sdk_python_faceid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:23:33.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-05-30 00:23:33.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-30 00:23:33.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:23:33.000000 tencentcloud-sdk-python-faceid-3.0.902/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:23:33.000000 tencentcloud-sdk-python-faceid-3.0.902/setup.cfg
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.901/README.rst` & `tencentcloud-sdk-python-faceid-3.0.902/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.901/tencentcloud/faceid/v20180301/faceid_client.py` & `tencentcloud-sdk-python-faceid-3.0.902/tencentcloud/faceid/v20180301/faceid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.901/tencentcloud/faceid/v20180301/errorcodes.py` & `tencentcloud-sdk-python-faceid-3.0.902/tencentcloud/faceid/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.901/tencentcloud/faceid/v20180301/models.py` & `tencentcloud-sdk-python-faceid-3.0.902/tencentcloud/faceid/v20180301/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1044,14 +1044,20 @@
         :type ErrCode: int
         :param ErrMsg: 本次流程最终验证结果描述。（仅描述用，文案更新时不会通知。）
 注意：此字段可能返回 null，表示取不到有效值。
         :type ErrMsg: str
         :param IdCard: 本次验证使用的身份证号。
 注意：此字段可能返回 null，表示取不到有效值。
         :type IdCard: str
+        :param UseIDType: 用户认证时使用的证件号码类型：
+0：二代身份证的证件号码
+1：港澳台居住证的证件号码
+2：其他（核验使用的证件号码非合法身份号码）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UseIDType: int
         :param Name: 本次验证使用的姓名。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Name: str
         :param OcrNation: 身份校验环节识别结果：民族。
 注意：此字段可能返回 null，表示取不到有效值。
         :type OcrNation: str
         :param OcrAddress: 身份校验环节识别结果：家庭住址。
@@ -1133,14 +1139,15 @@
         :param VisaNum: 港澳台居住证签发次数
 注意：此字段可能返回 null，表示取不到有效值。
         :type VisaNum: str
         """
         self.ErrCode = None
         self.ErrMsg = None
         self.IdCard = None
+        self.UseIDType = None
         self.Name = None
         self.OcrNation = None
         self.OcrAddress = None
         self.OcrBirth = None
         self.OcrAuthority = None
         self.OcrValidDate = None
         self.OcrName = None
@@ -1164,14 +1171,15 @@
         self.VisaNum = None
 
 
     def _deserialize(self, params):
         self.ErrCode = params.get("ErrCode")
         self.ErrMsg = params.get("ErrMsg")
         self.IdCard = params.get("IdCard")
+        self.UseIDType = params.get("UseIDType")
         self.Name = params.get("Name")
         self.OcrNation = params.get("OcrNation")
         self.OcrAddress = params.get("OcrAddress")
         self.OcrBirth = params.get("OcrBirth")
         self.OcrAuthority = params.get("OcrAuthority")
         self.OcrValidDate = params.get("OcrValidDate")
         self.OcrName = params.get("OcrName")
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.901/tencentcloud/__init__.py` & `tencentcloud-sdk-python-faceid-3.0.902/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-faceid-3.0.901/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.902/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.901/setup.py` & `tencentcloud-sdk-python-faceid-3.0.902/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.901/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.902/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

