# Comparing `tmp/tencentcloud-sdk-python-billing-3.0.901.tar.gz` & `tmp/tencentcloud-sdk-python-billing-3.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.901.tar", last modified: Mon May 29 02:19:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.902.tar", last modified: Tue May 30 00:15:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-billing-3.0.901.tar` & `tencentcloud-sdk-python-billing-3.0.902.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud/billing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud/billing/v20180709/
--rw-r--r--   0 root         (0) root         (0)     2904 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud/billing/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud/billing/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155292 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud/billing/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)    20134 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud/billing/v20180709/billing_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud_sdk_python_billing.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/tencentcloud_sdk_python_billing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:19:33.000000 tencentcloud-sdk-python-billing-3.0.901/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud/billing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud/billing/v20180709/
+-rw-r--r--   0 root         (0) root         (0)     2904 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud/billing/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud/billing/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155292 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud/billing/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)    20134 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud/billing/v20180709/billing_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud_sdk_python_billing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/tencentcloud_sdk_python_billing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:15:50.000000 tencentcloud-sdk-python-billing-3.0.902/setup.cfg
```

### Comparing `tencentcloud-sdk-python-billing-3.0.901/README.rst` & `tencentcloud-sdk-python-billing-3.0.902/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.901/tencentcloud/__init__.py` & `tencentcloud-sdk-python-billing-3.0.902/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-billing-3.0.901/tencentcloud/billing/v20180709/errorcodes.py` & `tencentcloud-sdk-python-billing-3.0.902/tencentcloud/billing/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.901/tencentcloud/billing/v20180709/models.py` & `tencentcloud-sdk-python-billing-3.0.902/tencentcloud/billing/v20180709/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.901/tencentcloud/billing/v20180709/billing_client.py` & `tencentcloud-sdk-python-billing-3.0.902/tencentcloud/billing/v20180709/billing_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.901/tencentcloud_sdk_python_billing.egg-info/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.902/tencentcloud_sdk_python_billing.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.901/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.902/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.901/setup.py` & `tencentcloud-sdk-python-billing-3.0.902/setup.py`

 * *Files identical despite different names*

