# Comparing `tmp/tencentcloud-sdk-python-ssl-3.0.901.tar.gz` & `tmp/tencentcloud-sdk-python-ssl-3.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.901.tar", last modified: Mon May 29 02:35:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.902.tar", last modified: Tue May 30 00:31:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssl-3.0.901.tar` & `tencentcloud-sdk-python-ssl-3.0.902.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud/ssl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud/ssl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud/ssl/v20191205/
--rw-r--r--   0 root         (0) root         (0)     8810 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud/ssl/v20191205/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud/ssl/v20191205/__init__.py
--rw-r--r--   0 root         (0) root         (0)   217643 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud/ssl/v20191205/models.py
--rw-r--r--   0 root         (0) root         (0)    48579 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud/ssl/v20191205/ssl_client.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud_sdk_python_ssl.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:35:47.000000 tencentcloud-sdk-python-ssl-3.0.901/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:31:33.000000 tencentcloud-sdk-python-ssl-3.0.902/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud/ssl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud/ssl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud/ssl/v20191205/
+-rw-r--r--   0 root         (0) root         (0)     8810 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud/ssl/v20191205/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud/ssl/v20191205/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   217801 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud/ssl/v20191205/models.py
+-rw-r--r--   0 root         (0) root         (0)    48579 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud/ssl/v20191205/ssl_client.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:31:33.000000 tencentcloud-sdk-python-ssl-3.0.902/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:31:33.000000 tencentcloud-sdk-python-ssl-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:31:33.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud_sdk_python_ssl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:31:32.000000 tencentcloud-sdk-python-ssl-3.0.902/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.901/README.rst` & `tencentcloud-sdk-python-ssl-3.0.902/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.901/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssl-3.0.902/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssl-3.0.901/tencentcloud/ssl/v20191205/errorcodes.py` & `tencentcloud-sdk-python-ssl-3.0.902/tencentcloud/ssl/v20191205/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.901/tencentcloud/ssl/v20191205/models.py` & `tencentcloud-sdk-python-ssl-3.0.902/tencentcloud/ssl/v20191205/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -771,20 +771,24 @@
 
     """
 
     def __init__(self):
         r"""
         :param CertificateId: 证书 ID。
         :type CertificateId: str
+        :param VerifyType: 域名验证方式
+        :type VerifyType: str
         """
         self.CertificateId = None
+        self.VerifyType = None
 
 
     def _deserialize(self, params):
         self.CertificateId = params.get("CertificateId")
+        self.VerifyType = params.get("VerifyType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.901/tencentcloud/ssl/v20191205/ssl_client.py` & `tencentcloud-sdk-python-ssl-3.0.902/tencentcloud/ssl/v20191205/ssl_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.901/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.902/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.901/setup.py` & `tencentcloud-sdk-python-ssl-3.0.902/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.901/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.902/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```
