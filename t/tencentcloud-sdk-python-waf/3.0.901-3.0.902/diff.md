# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.901.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.901.tar", last modified: Mon May 29 02:41:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.902.tar", last modified: Tue May 30 00:37:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.901.tar` & `tencentcloud-sdk-python-waf-3.0.902.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)    46563 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   180125 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:41:26.000000 tencentcloud-sdk-python-waf-3.0.901/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)    46563 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   180770 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:37:19.000000 tencentcloud-sdk-python-waf-3.0.902/tencentcloud_sdk_python_waf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-waf-3.0.901/README.rst` & `tencentcloud-sdk-python-waf-3.0.902/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.901/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.902/tencentcloud/waf/v20180125/waf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.901/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.902/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.901/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.902/tencentcloud/waf/v20180125/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4770,30 +4770,34 @@
         :type EndTime: str
         :param QueryString: Lucene语法
         :type QueryString: str
         :param TaskName: 任务名称
         :type TaskName: str
         :param Sort: 默认为desc，可以取值desc和asc
         :type Sort: str
+        :param Count: 下载的日志条数
+        :type Count: int
         """
         self.Domain = None
         self.StartTime = None
         self.EndTime = None
         self.QueryString = None
         self.TaskName = None
         self.Sort = None
+        self.Count = None
 
 
     def _deserialize(self, params):
         self.Domain = params.get("Domain")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.QueryString = params.get("QueryString")
         self.TaskName = params.get("TaskName")
         self.Sort = params.get("Sort")
+        self.Count = params.get("Count")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4833,28 +4837,32 @@
         :type ValidTime: str
         :param RenewFlag: 是否自动续费，1：自动续费，0：不自动续费
         :type RenewFlag: int
         :param Count: 套餐购买个数
         :type Count: int
         :param Region: 套餐购买地域，clb-waf暂时没有用到
         :type Region: str
+        :param BillingItem: 计费项
+        :type BillingItem: str
         """
         self.ResourceIds = None
         self.ValidTime = None
         self.RenewFlag = None
         self.Count = None
         self.Region = None
+        self.BillingItem = None
 
 
     def _deserialize(self, params):
         self.ResourceIds = params.get("ResourceIds")
         self.ValidTime = params.get("ValidTime")
         self.RenewFlag = params.get("RenewFlag")
         self.Count = params.get("Count")
         self.Region = params.get("Region")
+        self.BillingItem = params.get("BillingItem")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4935,46 +4943,51 @@
 class SearchAccessLogRequest(AbstractModel):
     """SearchAccessLog请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TopicId: 客户要查询的日志主题ID，每个客户都有对应的一个主题
+        :param TopicId: 客户要查询的日志主题ID，每个客户都有对应的一个主题，新版本此字段填空字符串
         :type TopicId: str
         :param From: 要查询的日志的起始时间，Unix时间戳，单位ms
         :type From: int
         :param To: 要查询的日志的结束时间，Unix时间戳，单位ms
         :type To: int
         :param Query: 查询语句，语句长度最大为4096
         :type Query: str
         :param Limit: 单次查询返回的日志条数，最大值为100
         :type Limit: int
-        :param Context: 加载更多日志时使用，透传上次返回的Context值，获取后续的日志内容
+        :param Context: 加载更多日志时使用，透传上次返回的Context值，获取后续的日志内容。
+新版本此字段填空填
         :type Context: str
         :param Sort: 日志接口是否按时间排序返回；可选值：asc(升序)、desc(降序)，默认为 desc
         :type Sort: str
+        :param Page: 第几页，从0开始。新版本接口字段
+        :type Page: int
         """
         self.TopicId = None
         self.From = None
         self.To = None
         self.Query = None
         self.Limit = None
         self.Context = None
         self.Sort = None
+        self.Page = None
 
 
     def _deserialize(self, params):
         self.TopicId = params.get("TopicId")
         self.From = params.get("From")
         self.To = params.get("To")
         self.Query = params.get("Query")
         self.Limit = params.get("Limit")
         self.Context = params.get("Context")
         self.Sort = params.get("Sort")
+        self.Page = params.get("Page")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5054,32 +5067,36 @@
         :type Context: str
         :param QueryString: Lucene语法
         :type QueryString: str
         :param Count: 查询的数量，默认10条，最多100条
         :type Count: int
         :param Sort: 默认为desc，可以取值desc和asc
         :type Sort: str
+        :param Page: 第几页，从0开始
+        :type Page: int
         """
         self.Domain = None
         self.StartTime = None
         self.EndTime = None
         self.Context = None
         self.QueryString = None
         self.Count = None
         self.Sort = None
+        self.Page = None
 
 
     def _deserialize(self, params):
         self.Domain = params.get("Domain")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.Context = params.get("Context")
         self.QueryString = params.get("QueryString")
         self.Count = params.get("Count")
         self.Sort = params.get("Sort")
+        self.Page = params.get("Page")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-waf-3.0.901/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.902/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-waf-3.0.901/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.902/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.901/setup.py` & `tencentcloud-sdk-python-waf-3.0.902/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.901/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.902/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

