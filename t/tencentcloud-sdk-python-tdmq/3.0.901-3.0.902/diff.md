# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.901.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.901.tar", last modified: Mon May 29 02:38:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.902.tar", last modified: Tue May 30 00:33:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.901.tar` & `tencentcloud-sdk-python-tdmq-3.0.902.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)   103763 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10117 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   384305 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:38:02.000000 tencentcloud-sdk-python-tdmq-3.0.901/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)   103763 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10117 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   384546 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:33:47.000000 tencentcloud-sdk-python-tdmq-3.0.902/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.901/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.902/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud/tdmq/v20200217/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8326,23 +8326,27 @@
         :param Version: 集群版本
         :type Version: str
         :param NodeDistribution: 节点分布情况
 注意：此字段可能返回 null，表示取不到有效值。
         :type NodeDistribution: list of InstanceNodeDistribution
         :param MaxStorage: 最大储存容量，单位：MB
         :type MaxStorage: int
+        :param CanEditRoute: 是否可以修改路由
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CanEditRoute: bool
         """
         self.ClusterId = None
         self.ClusterName = None
         self.Remark = None
         self.CreateTime = None
         self.Status = None
         self.Version = None
         self.NodeDistribution = None
         self.MaxStorage = None
+        self.CanEditRoute = None
 
 
     def _deserialize(self, params):
         self.ClusterId = params.get("ClusterId")
         self.ClusterName = params.get("ClusterName")
         self.Remark = params.get("Remark")
         self.CreateTime = params.get("CreateTime")
@@ -8351,14 +8355,15 @@
         if params.get("NodeDistribution") is not None:
             self.NodeDistribution = []
             for item in params.get("NodeDistribution"):
                 obj = InstanceNodeDistribution()
                 obj._deserialize(item)
                 self.NodeDistribution.append(obj)
         self.MaxStorage = params.get("MaxStorage")
+        self.CanEditRoute = params.get("CanEditRoute")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.901/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.902/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.901/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.902/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.901/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.902/setup.py`

 * *Files identical despite different names*

