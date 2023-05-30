# Comparing `tmp/tencentcloud-sdk-python-mps-3.0.901.tar.gz` & `tmp/tencentcloud-sdk-python-mps-3.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.901.tar", last modified: Mon May 29 02:32:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.902.tar", last modified: Tue May 30 00:28:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mps-3.0.901.tar` & `tencentcloud-sdk-python-mps-3.0.902.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud/mps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud/mps/v20190612/
--rw-r--r--   0 root         (0) root         (0)    89755 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud/mps/v20190612/mps_client.py
--rw-r--r--   0 root         (0) root         (0)    13373 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud/mps/v20190612/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud/mps/v20190612/__init__.py
--rw-r--r--   0 root         (0) root         (0)   805650 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud/mps/v20190612/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud/mps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud_sdk_python_mps.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/tencentcloud_sdk_python_mps.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:32:28.000000 tencentcloud-sdk-python-mps-3.0.901/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:28:06.000000 tencentcloud-sdk-python-mps-3.0.902/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:28:05.000000 tencentcloud-sdk-python-mps-3.0.902/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:28:06.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:28:05.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:28:06.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud/mps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:28:06.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud/mps/v20190612/
+-rw-r--r--   0 root         (0) root         (0)    89746 2023-05-30 00:28:05.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud/mps/v20190612/mps_client.py
+-rw-r--r--   0 root         (0) root         (0)    13373 2023-05-30 00:28:05.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud/mps/v20190612/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:28:05.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud/mps/v20190612/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   814885 2023-05-30 00:28:05.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud/mps/v20190612/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:28:05.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud/mps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:28:06.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud_sdk_python_mps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:28:06.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-30 00:28:06.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:28:06.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:28:06.000000 tencentcloud-sdk-python-mps-3.0.902/tencentcloud_sdk_python_mps.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:28:06.000000 tencentcloud-sdk-python-mps-3.0.902/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:28:05.000000 tencentcloud-sdk-python-mps-3.0.902/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:28:06.000000 tencentcloud-sdk-python-mps-3.0.902/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mps-3.0.901/README.rst` & `tencentcloud-sdk-python-mps-3.0.902/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.901/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mps-3.0.902/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mps-3.0.901/tencentcloud/mps/v20190612/mps_client.py` & `tencentcloud-sdk-python-mps-3.0.902/tencentcloud/mps/v20190612/mps_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1919,15 +1919,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ParseLiveStreamProcessNotification(self, request):
         """从 CMQ 获取到消息后，从消息的 msgBody 字段中解析出 MPS 直播流处理事件通知的内容。
-        该接口不用于发起网络调用，而是用来帮助生成各个语言平台的 SDK，您可以参考 SDK 的中解析函数的实现事件通知的解析。
+        该接口不用于发起网络调用，而是用来帮助生成各个语言平台的 SDK，您可以参考 SDK 中的解析实现事件通知的解析。
 
         :param request: Request instance for ParseLiveStreamProcessNotification.
         :type request: :class:`tencentcloud.mps.v20190612.models.ParseLiveStreamProcessNotificationRequest`
         :rtype: :class:`tencentcloud.mps.v20190612.models.ParseLiveStreamProcessNotificationResponse`
 
         """
         try:
@@ -1943,15 +1943,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ParseNotification(self, request):
         """从 CMQ 获取到消息后，从消息的 msgBody 字段中解析出 MPS 事件通知的内容。
-        该接口不用于发起网络调用，而是用来帮助生成各个语言平台的 SDK，您可以参考 SDK 的中解析函数的实现事件通知的解析。
+        该接口不用于发起网络调用，而是用来帮助生成各个语言平台的 SDK，您可以参考 SDK 中的解析函数，实现事件通知的解析。
 
         :param request: Request instance for ParseNotification.
         :type request: :class:`tencentcloud.mps.v20190612.models.ParseNotificationRequest`
         :rtype: :class:`tencentcloud.mps.v20190612.models.ParseNotificationResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-mps-3.0.901/tencentcloud/mps/v20190612/errorcodes.py` & `tencentcloud-sdk-python-mps-3.0.902/tencentcloud/mps/v20190612/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.901/tencentcloud/mps/v20190612/models.py` & `tencentcloud-sdk-python-mps-3.0.902/tencentcloud/mps/v20190612/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9993,14 +9993,64 @@
             for item in params.get("WorkflowInfoSet"):
                 obj = WorkflowInfo()
                 obj._deserialize(item)
                 self.WorkflowInfoSet.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DiagnoseResult(AbstractModel):
+    """诊断结果项。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Category: 诊断出的异常类别。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Category: str
+        :param Type: 诊断出的具体异常类型。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Type: str
+        :param Timestamp: 诊断出异常开始的PTS时间戳。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Timestamp: float
+        :param Description: 诊断出的异常描述。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param DateTime: 诊断到异常的北京时间，采用 ISO 日期格式。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DateTime: str
+        :param SeverityLevel: 诊断出的异常级别。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SeverityLevel: str
+        """
+        self.Category = None
+        self.Type = None
+        self.Timestamp = None
+        self.Description = None
+        self.DateTime = None
+        self.SeverityLevel = None
+
+
+    def _deserialize(self, params):
+        self.Category = params.get("Category")
+        self.Type = params.get("Type")
+        self.Timestamp = params.get("Timestamp")
+        self.Description = params.get("Description")
+        self.DateTime = params.get("DateTime")
+        self.SeverityLevel = params.get("SeverityLevel")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DisableScheduleRequest(AbstractModel):
     """DisableSchedule请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -11814,14 +11864,120 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class LiveStreamAiAnalysisResultInfo(AbstractModel):
+    """直播流分析结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ResultSet: 直播分析子任务结果，暂时只支持直播拆条。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResultSet: list of LiveStreamAiAnalysisResultItem
+        """
+        self.ResultSet = None
+
+
+    def _deserialize(self, params):
+        if params.get("ResultSet") is not None:
+            self.ResultSet = []
+            for item in params.get("ResultSet"):
+                obj = LiveStreamAiAnalysisResultItem()
+                obj._deserialize(item)
+                self.ResultSet.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class LiveStreamAiAnalysisResultItem(AbstractModel):
+    """直播流 AI 分析结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Type: 结果的类型，取值范围：
+<li>SegmentRecognition：拆条。</li>
+        :type Type: str
+        :param SegmentResultSet: 拆条结果，当 Type 为
+SegmentRecognition 时有效。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SegmentResultSet: list of SegmentRecognitionItem
+        """
+        self.Type = None
+        self.SegmentResultSet = None
+
+
+    def _deserialize(self, params):
+        self.Type = params.get("Type")
+        if params.get("SegmentResultSet") is not None:
+            self.SegmentResultSet = []
+            for item in params.get("SegmentResultSet"):
+                obj = SegmentRecognitionItem()
+                obj._deserialize(item)
+                self.SegmentResultSet.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class LiveStreamAiQualityControlResultInfo(AbstractModel):
+    """直播流质检结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param QualityControlResults: 质检结果列表。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QualityControlResults: list of QualityControlResult
+        :param DiagnoseResults: 格式诊断结果列表。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DiagnoseResults: list of DiagnoseResult
+        """
+        self.QualityControlResults = None
+        self.DiagnoseResults = None
+
+
+    def _deserialize(self, params):
+        if params.get("QualityControlResults") is not None:
+            self.QualityControlResults = []
+            for item in params.get("QualityControlResults"):
+                obj = QualityControlResult()
+                obj._deserialize(item)
+                self.QualityControlResults.append(obj)
+        if params.get("DiagnoseResults") is not None:
+            self.DiagnoseResults = []
+            for item in params.get("DiagnoseResults"):
+                obj = DiagnoseResult()
+                obj._deserialize(item)
+                self.DiagnoseResults.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class LiveStreamAiRecognitionResultInfo(AbstractModel):
     """直播流 AI 识别结果
 
     """
 
     def __init__(self):
         r"""
@@ -12262,26 +12418,41 @@
         :type Text: str
         :param StartPtsTime: 识别片段起始的 PTS 时间，单位：秒。
         :type StartPtsTime: float
         :param EndPtsTime: 识别片段终止的 PTS 时间，单位：秒。
         :type EndPtsTime: float
         :param Confidence: 识别片段置信度。取值：0~100。
         :type Confidence: float
+        :param StartTime: 识别开始UTC时间。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StartTime: str
+        :param EndTime: 识别结束UTC时间。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EndTime: str
+        :param SteadyState: 稳态标记。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SteadyState: bool
         """
         self.Text = None
         self.StartPtsTime = None
         self.EndPtsTime = None
         self.Confidence = None
+        self.StartTime = None
+        self.EndTime = None
+        self.SteadyState = None
 
 
     def _deserialize(self, params):
         self.Text = params.get("Text")
         self.StartPtsTime = params.get("StartPtsTime")
         self.EndPtsTime = params.get("EndPtsTime")
         self.Confidence = params.get("Confidence")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.SteadyState = params.get("SteadyState")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -12583,28 +12754,43 @@
         :type StartPtsTime: float
         :param EndPtsTime: 翻译片段终止的 PTS 时间，单位：秒。
         :type EndPtsTime: float
         :param Confidence: 翻译片段置信度。取值：0~100。
         :type Confidence: float
         :param Trans: 翻译文本。
         :type Trans: str
+        :param StartTime: 翻译开始UTC时间。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StartTime: str
+        :param EndTime: 翻译结束UTC时间。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EndTime: str
+        :param SteadyState: 稳态标记。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SteadyState: bool
         """
         self.Text = None
         self.StartPtsTime = None
         self.EndPtsTime = None
         self.Confidence = None
         self.Trans = None
+        self.StartTime = None
+        self.EndTime = None
+        self.SteadyState = None
 
 
     def _deserialize(self, params):
         self.Text = params.get("Text")
         self.StartPtsTime = params.get("StartPtsTime")
         self.EndPtsTime = params.get("EndPtsTime")
         self.Confidence = params.get("Confidence")
         self.Trans = params.get("Trans")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.SteadyState = params.get("SteadyState")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -15942,26 +16128,34 @@
         :type ProcessEofInfo: :class:`tencentcloud.mps.v20190612.models.LiveStreamProcessErrorInfo`
         :param AiReviewResultInfo: 内容审核结果，当 NotificationType 为 AiReviewResult 时有效。
 注意：此字段可能返回 null，表示取不到有效值。
         :type AiReviewResultInfo: :class:`tencentcloud.mps.v20190612.models.LiveStreamAiReviewResultInfo`
         :param AiRecognitionResultInfo: 内容识别结果，当 NotificationType 为 AiRecognitionResult 时有效。
 注意：此字段可能返回 null，表示取不到有效值。
         :type AiRecognitionResultInfo: :class:`tencentcloud.mps.v20190612.models.LiveStreamAiRecognitionResultInfo`
+        :param AiAnalysisResultInfo: 内容分析结果，当 NotificationType 为 AiAnalysisResult 时有效。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AiAnalysisResultInfo: :class:`tencentcloud.mps.v20190612.models.LiveStreamAiAnalysisResultInfo`
+        :param AiQualityControlResultInfo: 媒体质检结果，当 NotificationType 为 AiQualityControlResult 时有效。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AiQualityControlResultInfo: :class:`tencentcloud.mps.v20190612.models.LiveStreamAiQualityControlResultInfo`
         :param SessionId: 用于去重的识别码，如果七天内曾有过相同的识别码的请求，则本次的请求会返回错误。最长50个字符，不带或者带空字符串表示不做去重。
         :type SessionId: str
         :param SessionContext: 来源上下文，用于透传用户请求信息，任务流状态变更回调将返回该字段值，最长1000个字符。
         :type SessionContext: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.NotificationType = None
         self.TaskId = None
         self.ProcessEofInfo = None
         self.AiReviewResultInfo = None
         self.AiRecognitionResultInfo = None
+        self.AiAnalysisResultInfo = None
+        self.AiQualityControlResultInfo = None
         self.SessionId = None
         self.SessionContext = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.NotificationType = params.get("NotificationType")
@@ -15971,14 +16165,20 @@
             self.ProcessEofInfo._deserialize(params.get("ProcessEofInfo"))
         if params.get("AiReviewResultInfo") is not None:
             self.AiReviewResultInfo = LiveStreamAiReviewResultInfo()
             self.AiReviewResultInfo._deserialize(params.get("AiReviewResultInfo"))
         if params.get("AiRecognitionResultInfo") is not None:
             self.AiRecognitionResultInfo = LiveStreamAiRecognitionResultInfo()
             self.AiRecognitionResultInfo._deserialize(params.get("AiRecognitionResultInfo"))
+        if params.get("AiAnalysisResultInfo") is not None:
+            self.AiAnalysisResultInfo = LiveStreamAiAnalysisResultInfo()
+            self.AiAnalysisResultInfo._deserialize(params.get("AiAnalysisResultInfo"))
+        if params.get("AiQualityControlResultInfo") is not None:
+            self.AiQualityControlResultInfo = LiveStreamAiQualityControlResultInfo()
+            self.AiQualityControlResultInfo._deserialize(params.get("AiQualityControlResultInfo"))
         self.SessionId = params.get("SessionId")
         self.SessionContext = params.get("SessionContext")
         self.RequestId = params.get("RequestId")
 
 
 class ParseNotificationRequest(AbstractModel):
     """ParseNotification请求参数结构体
@@ -18382,14 +18582,51 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class SegmentRecognitionItem(AbstractModel):
+    """智能拆条片段。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Confidence: 置信度。
+        :type Confidence: float
+        :param StartTimeOffset: 片段起始时间偏移。
+        :type StartTimeOffset: float
+        :param EndTimeOffset: 片段结束时间偏移。
+        :type EndTimeOffset: float
+        :param SegmentUrl: 拆条片段URL。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SegmentUrl: str
+        """
+        self.Confidence = None
+        self.StartTimeOffset = None
+        self.EndTimeOffset = None
+        self.SegmentUrl = None
+
+
+    def _deserialize(self, params):
+        self.Confidence = params.get("Confidence")
+        self.StartTimeOffset = params.get("StartTimeOffset")
+        self.EndTimeOffset = params.get("EndTimeOffset")
+        self.SegmentUrl = params.get("SegmentUrl")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class SharpEnhanceConfig(AbstractModel):
     """细节增强配置
 
     """
```

### Comparing `tencentcloud-sdk-python-mps-3.0.901/tencentcloud_sdk_python_mps.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.902/tencentcloud_sdk_python_mps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.901/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.902/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.901/setup.py` & `tencentcloud-sdk-python-mps-3.0.902/setup.py`

 * *Files identical despite different names*

