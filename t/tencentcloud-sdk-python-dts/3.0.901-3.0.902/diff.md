# Comparing `tmp/tencentcloud-sdk-python-dts-3.0.901.tar.gz` & `tmp/tencentcloud-sdk-python-dts-3.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dts-3.0.901.tar", last modified: Mon May 29 02:26:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dts-3.0.902.tar", last modified: Tue May 30 00:22:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dts-3.0.901.tar` & `tencentcloud-sdk-python-dts-3.0.902.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20211206/
--rw-r--r--   0 root         (0) root         (0)    43091 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20211206/dts_client.py
--rw-r--r--   0 root         (0) root         (0)     6952 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20211206/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20211206/__init__.py
--rw-r--r--   0 root         (0) root         (0)   210144 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20211206/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20180330/
--rw-r--r--   0 root         (0) root         (0)    24761 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20180330/dts_client.py
--rw-r--r--   0 root         (0) root         (0)     5619 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20180330/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20180330/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79091 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20180330/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud_sdk_python_dts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud_sdk_python_dts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud_sdk_python_dts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud_sdk_python_dts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/tencentcloud_sdk_python_dts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:26:39.000000 tencentcloud-sdk-python-dts-3.0.901/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:22:19.000000 tencentcloud-sdk-python-dts-3.0.902/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-30 00:22:18.000000 tencentcloud-sdk-python-dts-3.0.902/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:22:19.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:22:19.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:22:19.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20211206/
+-rw-r--r--   0 root         (0) root         (0)    47170 2023-05-30 00:22:18.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20211206/dts_client.py
+-rw-r--r--   0 root         (0) root         (0)     6952 2023-05-30 00:22:18.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20211206/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:22:18.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20211206/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   218875 2023-05-30 00:22:18.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20211206/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:22:18.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:22:19.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20180330/
+-rw-r--r--   0 root         (0) root         (0)    24761 2023-05-30 00:22:18.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20180330/dts_client.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2023-05-30 00:22:18.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20180330/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:22:18.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20180330/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79091 2023-05-30 00:22:18.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20180330/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-30 00:22:18.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:22:19.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud_sdk_python_dts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:22:19.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud_sdk_python_dts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-30 00:22:19.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud_sdk_python_dts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:22:19.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud_sdk_python_dts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:22:19.000000 tencentcloud-sdk-python-dts-3.0.902/tencentcloud_sdk_python_dts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-30 00:22:19.000000 tencentcloud-sdk-python-dts-3.0.902/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-30 00:22:18.000000 tencentcloud-sdk-python-dts-3.0.902/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-30 00:22:19.000000 tencentcloud-sdk-python-dts-3.0.902/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dts-3.0.901/README.rst` & `tencentcloud-sdk-python-dts-3.0.902/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20211206/dts_client.py` & `tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20211206/dts_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateModifyCheckSyncJob(self, request):
+        """在修改同步任务的配置后、通过该接口校验当前任务是否支持修改对象操作
+
+        :param request: Request instance for CreateModifyCheckSyncJob.
+        :type request: :class:`tencentcloud.dts.v20211206.models.CreateModifyCheckSyncJobRequest`
+        :rtype: :class:`tencentcloud.dts.v20211206.models.CreateModifyCheckSyncJobResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateModifyCheckSyncJob", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateModifyCheckSyncJobResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateSyncJob(self, request):
         """创建一个同步任务
 
         :param request: Request instance for CreateSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.CreateSyncJobRequest`
         :rtype: :class:`tencentcloud.dts.v20211206.models.CreateSyncJobResponse`
 
@@ -419,14 +442,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeModifyCheckSyncJobResult(self, request):
+        """在创建修改对象的校验任务后、通过该接口查看校验任务的结果
+
+        :param request: Request instance for DescribeModifyCheckSyncJobResult.
+        :type request: :class:`tencentcloud.dts.v20211206.models.DescribeModifyCheckSyncJobResultRequest`
+        :rtype: :class:`tencentcloud.dts.v20211206.models.DescribeModifyCheckSyncJobResultResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeModifyCheckSyncJobResult", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeModifyCheckSyncJobResultResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeSyncJobs(self, request):
         """查询同步任务信息
 
         :param request: Request instance for DescribeSyncJobs.
         :type request: :class:`tencentcloud.dts.v20211206.models.DescribeSyncJobsRequest`
         :rtype: :class:`tencentcloud.dts.v20211206.models.DescribeSyncJobsResponse`
 
@@ -649,14 +695,38 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifySyncJobConfig(self, request):
+        """该接口支持在同步任务启动后修改任务的配置
+        修改同步配置的完整流程：修改同步任务配置->创建修改同步任务配置的校验任务->查询修改配置的校验任务的结果->启动修改配置任务
+
+        :param request: Request instance for ModifySyncJobConfig.
+        :type request: :class:`tencentcloud.dts.v20211206.models.ModifySyncJobConfigRequest`
+        :rtype: :class:`tencentcloud.dts.v20211206.models.ModifySyncJobConfigResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifySyncJobConfig", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifySyncJobConfigResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def PauseMigrateJob(self, request):
         """暂停一个迁移任务。
 
         :param request: Request instance for PauseMigrateJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.PauseMigrateJobRequest`
         :rtype: :class:`tencentcloud.dts.v20211206.models.PauseMigrateJobResponse`
 
@@ -900,14 +970,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def StartModifySyncJob(self, request):
+        """在查询修改对象的校验任务的结果中的status为success后、通过该接口开始修改配置流程
+
+        :param request: Request instance for StartModifySyncJob.
+        :type request: :class:`tencentcloud.dts.v20211206.models.StartModifySyncJobRequest`
+        :rtype: :class:`tencentcloud.dts.v20211206.models.StartModifySyncJobResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StartModifySyncJob", params, headers=headers)
+            response = json.loads(body)
+            model = models.StartModifySyncJobResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def StartSyncJob(self, request):
         """启动同步任务
 
         :param request: Request instance for StartSyncJob.
         :type request: :class:`tencentcloud.dts.v20211206.models.StartSyncJobRequest`
```

### Comparing `tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20211206/errorcodes.py` & `tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20211206/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20211206/models.py` & `tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20211206/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1084,14 +1084,55 @@
 
 
     def _deserialize(self, params):
         self.JobIds = params.get("JobIds")
         self.RequestId = params.get("RequestId")
 
 
+class CreateModifyCheckSyncJobRequest(AbstractModel):
+    """CreateModifyCheckSyncJob请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param JobId: 同步任务id
+        :type JobId: str
+        """
+        self.JobId = None
+
+
+    def _deserialize(self, params):
+        self.JobId = params.get("JobId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateModifyCheckSyncJobResponse(AbstractModel):
+    """CreateModifyCheckSyncJob返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class CreateSyncJobRequest(AbstractModel):
     """CreateSyncJob请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2415,14 +2456,84 @@
             for item in params.get("JobList"):
                 obj = JobItem()
                 obj._deserialize(item)
                 self.JobList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeModifyCheckSyncJobResultRequest(AbstractModel):
+    """DescribeModifyCheckSyncJobResult请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param JobId: 同步任务id
+        :type JobId: str
+        """
+        self.JobId = None
+
+
+    def _deserialize(self, params):
+        self.JobId = params.get("JobId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeModifyCheckSyncJobResultResponse(AbstractModel):
+    """DescribeModifyCheckSyncJobResult返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Status: 校验任务执行状态，如：notStarted(未开始)、running(校验中)、failed(校验任务失败)、success(任务成功)
+        :type Status: str
+        :param StepCount: 校验的步骤总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StepCount: int
+        :param StepCur: 当前所在步骤
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StepCur: int
+        :param Progress: 总体进度，范围为[0,100]	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Progress: int
+        :param StepInfos: 步骤详细信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StepInfos: list of StepInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Status = None
+        self.StepCount = None
+        self.StepCur = None
+        self.Progress = None
+        self.StepInfos = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Status = params.get("Status")
+        self.StepCount = params.get("StepCount")
+        self.StepCur = params.get("StepCur")
+        self.Progress = params.get("Progress")
+        if params.get("StepInfos") is not None:
+            self.StepInfos = []
+            for item in params.get("StepInfos"):
+                obj = StepInfo()
+                obj._deserialize(item)
+                self.StepInfos.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeSyncJobsRequest(AbstractModel):
     """DescribeSyncJobs请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2763,14 +2874,61 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DynamicOptions(AbstractModel):
+    """数据同步中的选项
+
+    """
+
+    def __init__(self):
+        r"""
+        :param OpTypes: 所要同步的DML和DDL的选项，Insert(插入操作)、Update(更新操作)、Delete(删除操作)、DDL(结构同步)，PartialDDL(自定义,和DdlOptions一起起作用 )；必填、dts会用该值覆盖原有的值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OpTypes: list of str
+        :param DdlOptions: DDL同步选项，具体描述要同步那些DDL; 当OpTypes取值PartialDDL时、字段不能为空；必填、dts会用该值覆盖原有的值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DdlOptions: list of DdlOption
+        :param ConflictHandleType: 冲突处理选项，ReportError(报错)、Ignore(忽略)、Cover(覆盖)、ConditionCover(条件覆盖); 目前目标端为kafka的链路不支持修改该配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ConflictHandleType: str
+        :param ConflictHandleOption: 冲突处理的详细选项，如条件覆盖中的条件行和条件操作；不能部分更新该选项的内部字段；有更新时、需要全量更新该字段
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ConflictHandleOption: :class:`tencentcloud.dts.v20211206.models.ConflictHandleOption`
+        """
+        self.OpTypes = None
+        self.DdlOptions = None
+        self.ConflictHandleType = None
+        self.ConflictHandleOption = None
+
+
+    def _deserialize(self, params):
+        self.OpTypes = params.get("OpTypes")
+        if params.get("DdlOptions") is not None:
+            self.DdlOptions = []
+            for item in params.get("DdlOptions"):
+                obj = DdlOption()
+                obj._deserialize(item)
+                self.DdlOptions.append(obj)
+        self.ConflictHandleType = params.get("ConflictHandleType")
+        if params.get("ConflictHandleOption") is not None:
+            self.ConflictHandleOption = ConflictHandleOption()
+            self.ConflictHandleOption._deserialize(params.get("ConflictHandleOption"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class Endpoint(AbstractModel):
     """数据同步中的描述源端和目的端的信息
 
     """
 
     def __init__(self):
         r"""
@@ -3712,14 +3870,67 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ModifySyncJobConfigRequest(AbstractModel):
+    """ModifySyncJobConfig请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param JobId: 同步任务id
+        :type JobId: str
+        :param DynamicObjects: 修改后的同步对象
+        :type DynamicObjects: :class:`tencentcloud.dts.v20211206.models.Objects`
+        :param DynamicOptions: 修改后的同步任务选项
+        :type DynamicOptions: :class:`tencentcloud.dts.v20211206.models.DynamicOptions`
+        """
+        self.JobId = None
+        self.DynamicObjects = None
+        self.DynamicOptions = None
+
+
+    def _deserialize(self, params):
+        self.JobId = params.get("JobId")
+        if params.get("DynamicObjects") is not None:
+            self.DynamicObjects = Objects()
+            self.DynamicObjects._deserialize(params.get("DynamicObjects"))
+        if params.get("DynamicOptions") is not None:
+            self.DynamicOptions = DynamicOptions()
+            self.DynamicOptions._deserialize(params.get("DynamicOptions"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifySyncJobConfigResponse(AbstractModel):
+    """ModifySyncJobConfig返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class Objects(AbstractModel):
     """同步的数据库对对象描述
 
     """
 
     def __init__(self):
         r"""
@@ -4515,14 +4726,55 @@
 
     """
 
     def __init__(self):
         r"""
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class StartModifySyncJobRequest(AbstractModel):
+    """StartModifySyncJob请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param JobId: 同步任务id
+        :type JobId: str
+        """
+        self.JobId = None
+
+
+    def _deserialize(self, params):
+        self.JobId = params.get("JobId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class StartModifySyncJobResponse(AbstractModel):
+    """StartModifySyncJob返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20180330/dts_client.py` & `tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20180330/dts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20180330/errorcodes.py` & `tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20180330/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.901/tencentcloud/dts/v20180330/models.py` & `tencentcloud-sdk-python-dts-3.0.902/tencentcloud/dts/v20180330/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.901/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dts-3.0.902/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dts-3.0.901/tencentcloud_sdk_python_dts.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dts-3.0.902/tencentcloud_sdk_python_dts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.901/tencentcloud_sdk_python_dts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dts-3.0.902/tencentcloud_sdk_python_dts.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dts
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Dts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dts-3.0.901/PKG-INFO` & `tencentcloud-sdk-python-dts-3.0.902/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dts
-Version: 3.0.901
+Version: 3.0.902
 Summary: Tencent Cloud Dts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dts-3.0.901/setup.py` & `tencentcloud-sdk-python-dts-3.0.902/setup.py`

 * *Files identical despite different names*

