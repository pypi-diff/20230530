# Comparing `tmp/tencentcloud-sdk-python-live-3.0.901.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.901.tar", last modified: Mon May 29 02:31:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.902.tar", last modified: Tue May 30 00:26:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.901.tar` & `tencentcloud-sdk-python-live-3.0.902.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)   137459 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)    18117 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   431811 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:31:16.000000 tencentcloud-sdk-python-live-3.0.901/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)   137451 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)    18117 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   433012 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-30 00:26:56.000000 tencentcloud-sdk-python-live-3.0.902/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:26:57.000000 tencentcloud-sdk-python-live-3.0.902/setup.cfg
```

### Comparing `tencentcloud-sdk-python-live-3.0.901/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.902/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.901/README.rst` & `tencentcloud-sdk-python-live-3.0.902/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.901/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/live_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,16 +71,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def AddLiveWatermark(self, request):
-        """添加水印，成功返回水印 ID 后，需要调用[CreateLiveWatermarkRule](/document/product/267/32629)接口将水印 ID 绑定到流使用。
-        水印数量上限 100，超过后需要先删除，再添加。
+        """添加水印，成功返回水印 ID 后，需要调用[CreateLiveWatermarkRule](/document/product/267/32629)接口将水印 ID 绑定到流使用。 水印数量上限 100，超过后需要先删除，再添加。
 
         :param request: Request instance for AddLiveWatermark.
         :type request: :class:`tencentcloud.live.v20180801.models.AddLiveWatermarkRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.AddLiveWatermarkResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-live-3.0.901/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.901/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.902/tencentcloud/live/v20180801/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,30 +174,38 @@
         :type XPosition: int
         :param YPosition: 显示位置，Y轴偏移，单位是百分比，默认 0。
         :type YPosition: int
         :param Width: 水印宽度，占直播原始画面宽度百分比，建议高宽只设置一项，另外一项会自适应缩放，避免变形。默认原始宽度。
         :type Width: int
         :param Height: 水印高度，占直播原始画面高度百分比，建议高宽只设置一项，另外一项会自适应缩放，避免变形。默认原始高度。
         :type Height: int
+        :param BackgroundWidth: 背景水印宽度。默认宽度1920。
+        :type BackgroundWidth: int
+        :param BackgroundHeight: 背景水印高度。默认高度1080。
+        :type BackgroundHeight: int
         """
         self.PictureUrl = None
         self.WatermarkName = None
         self.XPosition = None
         self.YPosition = None
         self.Width = None
         self.Height = None
+        self.BackgroundWidth = None
+        self.BackgroundHeight = None
 
 
     def _deserialize(self, params):
         self.PictureUrl = params.get("PictureUrl")
         self.WatermarkName = params.get("WatermarkName")
         self.XPosition = params.get("XPosition")
         self.YPosition = params.get("YPosition")
         self.Width = params.get("Width")
         self.Height = params.get("Height")
+        self.BackgroundWidth = params.get("BackgroundWidth")
+        self.BackgroundHeight = params.get("BackgroundHeight")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -12203,32 +12211,40 @@
         :param WatermarkName: 水印名称。
 最长16字节。
         :type WatermarkName: str
         :param Width: 水印宽度，占直播原始画面宽度百分比，建议高宽只设置一项，另外一项会自适应缩放，避免变形。默认原始宽度。
         :type Width: int
         :param Height: 水印高度，占直播原始画面宽度百分比，建议高宽只设置一项，另外一项会自适应缩放，避免变形。默认原始高度。
         :type Height: int
+        :param BackgroundWidth: 背景水印宽度。默认宽度1920。
+        :type BackgroundWidth: int
+        :param BackgroundHeight: 背景水印高度。默认高度1080。
+        :type BackgroundHeight: int
         """
         self.WatermarkId = None
         self.PictureUrl = None
         self.XPosition = None
         self.YPosition = None
         self.WatermarkName = None
         self.Width = None
         self.Height = None
+        self.BackgroundWidth = None
+        self.BackgroundHeight = None
 
 
     def _deserialize(self, params):
         self.WatermarkId = params.get("WatermarkId")
         self.PictureUrl = params.get("PictureUrl")
         self.XPosition = params.get("XPosition")
         self.YPosition = params.get("YPosition")
         self.WatermarkName = params.get("WatermarkName")
         self.Width = params.get("Width")
         self.Height = params.get("Height")
+        self.BackgroundWidth = params.get("BackgroundWidth")
+        self.BackgroundHeight = params.get("BackgroundHeight")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -12273,36 +12289,44 @@
         :param CreateTime: 添加时间。
 注：此字段为北京时间（UTC+8时区）。
         :type CreateTime: str
         :param Width: 水印宽。
         :type Width: int
         :param Height: 水印高。
         :type Height: int
+        :param BackgroundWidth: 背景水印宽。
+        :type BackgroundWidth: int
+        :param BackgroundHeight: 背景水印高。
+        :type BackgroundHeight: int
         """
         self.WatermarkId = None
         self.PictureUrl = None
         self.XPosition = None
         self.YPosition = None
         self.WatermarkName = None
         self.Status = None
         self.CreateTime = None
         self.Width = None
         self.Height = None
+        self.BackgroundWidth = None
+        self.BackgroundHeight = None
 
 
     def _deserialize(self, params):
         self.WatermarkId = params.get("WatermarkId")
         self.PictureUrl = params.get("PictureUrl")
         self.XPosition = params.get("XPosition")
         self.YPosition = params.get("YPosition")
         self.WatermarkName = params.get("WatermarkName")
         self.Status = params.get("Status")
         self.CreateTime = params.get("CreateTime")
         self.Width = params.get("Width")
         self.Height = params.get("Height")
+        self.BackgroundWidth = params.get("BackgroundWidth")
+        self.BackgroundHeight = params.get("BackgroundHeight")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-live-3.0.901/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.902/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.901/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.902/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.901/setup.py` & `tencentcloud-sdk-python-live-3.0.902/setup.py`

 * *Files identical despite different names*

