# Comparing `tmp/tencentcloud-sdk-python-yinsuda-3.0.901.tar.gz` & `tmp/tencentcloud-sdk-python-yinsuda-3.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-yinsuda-3.0.901.tar", last modified: Mon May 29 02:41:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-yinsuda-3.0.902.tar", last modified: Tue May 30 00:37:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-yinsuda-3.0.901.tar` & `tencentcloud-sdk-python-yinsuda-3.0.902.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud_sdk_python_yinsuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud_sdk_python_yinsuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud_sdk_python_yinsuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud_sdk_python_yinsuda.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud/yinsuda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud/yinsuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud/yinsuda/v20220527/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud/yinsuda/v20220527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud/yinsuda/v20220527/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72966 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud/yinsuda/v20220527/models.py
--rw-r--r--   0 root         (0) root         (0)    15889 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud/yinsuda/v20220527/yinsuda_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.901/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:45.000000 tencentcloud-sdk-python-yinsuda-3.0.902/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:45.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud_sdk_python_yinsuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:37:45.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud_sdk_python_yinsuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-30 00:37:45.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud_sdk_python_yinsuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-30 00:37:45.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:37:45.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud_sdk_python_yinsuda.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-30 00:37:44.000000 tencentcloud-sdk-python-yinsuda-3.0.902/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:45.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:45.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud/yinsuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:37:44.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud/yinsuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:45.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud/yinsuda/v20220527/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-05-30 00:37:44.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud/yinsuda/v20220527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:37:44.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud/yinsuda/v20220527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72966 2023-05-30 00:37:44.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud/yinsuda/v20220527/models.py
+-rw-r--r--   0 root         (0) root         (0)    15889 2023-05-30 00:37:44.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud/yinsuda/v20220527/yinsuda_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:37:44.000000 tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-30 00:37:45.000000 tencentcloud-sdk-python-yinsuda-3.0.902/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-30 00:37:44.000000 tencentcloud-sdk-python-yinsuda-3.0.902/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:37:45.000000 tencentcloud-sdk-python-yinsuda-3.0.902/setup.cfg
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO` & `tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yinsuda
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Yinsuda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.901/README.rst` & `tencentcloud-sdk-python-yinsuda-3.0.902/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud/yinsuda/v20220527/errorcodes.py` & `tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud/yinsuda/v20220527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud/yinsuda/v20220527/models.py` & `tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud/yinsuda/v20220527/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud/yinsuda/v20220527/yinsuda_client.py` & `tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud/yinsuda/v20220527/yinsuda_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.901/tencentcloud/__init__.py` & `tencentcloud-sdk-python-yinsuda-3.0.902/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.901/PKG-INFO` & `tencentcloud-sdk-python-yinsuda-3.0.902/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yinsuda
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Yinsuda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.901/setup.py` & `tencentcloud-sdk-python-yinsuda-3.0.902/setup.py`

 * *Files identical despite different names*

