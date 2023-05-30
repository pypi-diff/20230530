# Comparing `tmp/alibabacloud_fc-open20210406_py2-2.0.8.tar.gz` & `tmp/alibabacloud_fc-open20210406_py2-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_fc-open20210406_py2-2.0.8.tar", last modified: Tue Apr 11 06:50:12 2023, max compression
+gzip compressed data, was "dist/alibabacloud_fc-open20210406_py2-2.0.9.tar", last modified: Tue May 30 06:47:45 2023, max compression
```

## Comparing `alibabacloud_fc-open20210406_py2-2.0.8.tar` & `alibabacloud_fc-open20210406_py2-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:50:12.000000 alibabacloud_fc-open20210406_py2-2.0.8/
--rw-r--r--   0 root         (0) root         (0)     1915 2023-04-11 06:50:11.000000 alibabacloud_fc-open20210406_py2-2.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-04-11 06:50:11.000000 alibabacloud_fc-open20210406_py2-2.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-11 06:50:11.000000 alibabacloud_fc-open20210406_py2-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2496 2023-04-11 06:50:12.000000 alibabacloud_fc-open20210406_py2-2.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2023-04-11 06:50:11.000000 alibabacloud_fc-open20210406_py2-2.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-11 06:50:11.000000 alibabacloud_fc-open20210406_py2-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:50:12.000000 alibabacloud_fc-open20210406_py2-2.0.8/alibabacloud_fc_open20210406/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 06:50:11.000000 alibabacloud_fc-open20210406_py2-2.0.8/alibabacloud_fc_open20210406/__init__.py
--rw-r--r--   0 root         (0) root         (0)   154478 2023-04-11 06:50:11.000000 alibabacloud_fc-open20210406_py2-2.0.8/alibabacloud_fc_open20210406/client.py
--rw-r--r--   0 root         (0) root         (0)   601030 2023-04-11 06:50:11.000000 alibabacloud_fc-open20210406_py2-2.0.8/alibabacloud_fc_open20210406/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:50:12.000000 alibabacloud_fc-open20210406_py2-2.0.8/alibabacloud_fc_open20210406_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2496 2023-04-11 06:50:12.000000 alibabacloud_fc-open20210406_py2-2.0.8/alibabacloud_fc_open20210406_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-04-11 06:50:12.000000 alibabacloud_fc-open20210406_py2-2.0.8/alibabacloud_fc_open20210406_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 06:50:12.000000 alibabacloud_fc-open20210406_py2-2.0.8/alibabacloud_fc_open20210406_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      286 2023-04-11 06:50:12.000000 alibabacloud_fc-open20210406_py2-2.0.8/alibabacloud_fc_open20210406_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 06:50:12.000000 alibabacloud_fc-open20210406_py2-2.0.8/alibabacloud_fc_open20210406_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 06:50:12.000000 alibabacloud_fc-open20210406_py2-2.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3063 2023-04-11 06:50:11.000000 alibabacloud_fc-open20210406_py2-2.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/alibabacloud_fc_open20210406/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/alibabacloud_fc_open20210406/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   151171 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/alibabacloud_fc_open20210406/client.py
+-rw-r--r--   0 root         (0) root         (0)   592911 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/alibabacloud_fc_open20210406/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/alibabacloud_fc_open20210406_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/alibabacloud_fc_open20210406_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/alibabacloud_fc_open20210406_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/alibabacloud_fc_open20210406_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      286 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/alibabacloud_fc_open20210406_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/alibabacloud_fc_open20210406_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3063 2023-05-30 06:47:45.000000 alibabacloud_fc-open20210406_py2-2.0.9/setup.py
```

### Comparing `alibabacloud_fc-open20210406_py2-2.0.8/ChangeLog.md` & `alibabacloud_fc-open20210406_py2-2.0.9/ChangeLog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-04-11 Version: 2.0.8
+- Fix http invocation with sts credentials.
+
 2023-03-28 Version: 2.0.6
 - Change policyItem type.
 
 2023-03-01 Version: 2.0.5
 - Support NAS with TLS.
 
 2023-02-09 Version: 2.0.4
```

### Comparing `alibabacloud_fc-open20210406_py2-2.0.8/LICENSE` & `alibabacloud_fc-open20210406_py2-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc-open20210406_py2-2.0.8/PKG-INFO` & `alibabacloud_fc-open20210406_py2-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_fc-open20210406_py2
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud FC-Open (20210406) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc-open20210406_py2-2.0.8/README-CN.md` & `alibabacloud_fc-open20210406_py2-2.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc-open20210406_py2-2.0.8/README.md` & `alibabacloud_fc-open20210406_py2-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc-open20210406_py2-2.0.8/alibabacloud_fc_open20210406/client.py` & `alibabacloud_fc-open20210406_py2-2.0.9/alibabacloud_fc_open20210406/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1027,26 +1027,14 @@
 
     def get_function(self, service_name, function_name, request):
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.GetFunctionHeaders()
         return self.get_function_with_options(service_name, function_name, request, headers, runtime)
 
     def get_function_async_invoke_config_with_options(self, service_name, function_name, request, headers, runtime):
-        """
-        StatefulAsyncInvocation indicates whether the asynchronous task feature is enabled. If the value of StatefulAsyncInvocation is true, the asynchronous task feature is enabled. All asynchronous invocations change to asynchronous task mode.
-        
-
-        @param request: GetFunctionAsyncInvokeConfigRequest
-
-        @param headers: GetFunctionAsyncInvokeConfigHeaders
-
-        @param runtime: runtime options for this request RuntimeOptions
-
-        @return: GetFunctionAsyncInvokeConfigResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.qualifier):
             query['qualifier'] = request.qualifier
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -1073,22 +1061,14 @@
         )
         return TeaCore.from_map(
             fc__open_20210406_models.GetFunctionAsyncInvokeConfigResponse(),
             self.call_api(params, req, runtime)
         )
 
     def get_function_async_invoke_config(self, service_name, function_name, request):
-        """
-        StatefulAsyncInvocation indicates whether the asynchronous task feature is enabled. If the value of StatefulAsyncInvocation is true, the asynchronous task feature is enabled. All asynchronous invocations change to asynchronous task mode.
-        
-
-        @param request: GetFunctionAsyncInvokeConfigRequest
-
-        @return: GetFunctionAsyncInvokeConfigResponse
-        """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.GetFunctionAsyncInvokeConfigHeaders()
         return self.get_function_async_invoke_config_with_options(service_name, function_name, request, headers, runtime)
 
     def get_function_code_with_options(self, service_name, function_name, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
@@ -1316,15 +1296,15 @@
     def get_service(self, service_name, request):
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.GetServiceHeaders()
         return self.get_service_with_options(service_name, request, headers, runtime)
 
     def get_stateful_async_invocation_with_options(self, service_name, function_name, invocation_id, request, headers, runtime):
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The version or alias of the service to which the asynchronous task belongs.
         
 
         @param request: GetStatefulAsyncInvocationRequest
 
         @param headers: GetStatefulAsyncInvocationHeaders
 
         @param runtime: runtime options for this request RuntimeOptions
@@ -1368,15 +1348,15 @@
         return TeaCore.from_map(
             fc__open_20210406_models.GetStatefulAsyncInvocationResponse(),
             self.call_api(params, req, runtime)
         )
 
     def get_stateful_async_invocation(self, service_name, function_name, invocation_id, request):
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The version or alias of the service to which the asynchronous task belongs.
         
 
         @param request: GetStatefulAsyncInvocationRequest
 
         @return: GetStatefulAsyncInvocationResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1432,14 +1412,16 @@
             real_headers['X-Fc-Account-Id'] = UtilClient.to_jsonstring(headers.x_fc_account_id)
         if not UtilClient.is_unset(headers.x_fc_date):
             real_headers['X-Fc-Date'] = UtilClient.to_jsonstring(headers.x_fc_date)
         if not UtilClient.is_unset(headers.x_fc_invocation_type):
             real_headers['X-Fc-Invocation-Type'] = UtilClient.to_jsonstring(headers.x_fc_invocation_type)
         if not UtilClient.is_unset(headers.x_fc_log_type):
             real_headers['X-Fc-Log-Type'] = UtilClient.to_jsonstring(headers.x_fc_log_type)
+        if not UtilClient.is_unset(headers.x_fc_stateful_async_invocation_enable):
+            real_headers['X-Fc-Stateful-Async-Invocation-Enable'] = UtilClient.to_jsonstring(headers.x_fc_stateful_async_invocation_enable)
         if not UtilClient.is_unset(headers.x_fc_stateful_async_invocation_id):
             real_headers['X-Fc-Stateful-Async-Invocation-Id'] = UtilClient.to_jsonstring(headers.x_fc_stateful_async_invocation_id)
         if not UtilClient.is_unset(headers.x_fc_trace_id):
             real_headers['X-Fc-Trace-Id'] = UtilClient.to_jsonstring(headers.x_fc_trace_id)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             query=OpenApiUtilClient.query(query),
@@ -1592,26 +1574,14 @@
 
     def list_event_sources(self, service_name, function_name, request):
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.ListEventSourcesHeaders()
         return self.list_event_sources_with_options(service_name, function_name, request, headers, runtime)
 
     def list_function_async_invoke_configs_with_options(self, service_name, function_name, request, headers, runtime):
-        """
-        StatefulAsyncInvocation indicates whether the asynchronous task feature is enabled. If StatefulAsyncInvocation is set to true, the asynchronous task is enabled. All asynchronous invocations to the function corresponding to this configuration change to asynchronous task mode.
-        
-
-        @param request: ListFunctionAsyncInvokeConfigsRequest
-
-        @param headers: ListFunctionAsyncInvokeConfigsHeaders
-
-        @param runtime: runtime options for this request RuntimeOptions
-
-        @return: ListFunctionAsyncInvokeConfigsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.limit):
             query['limit'] = request.limit
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
         real_headers = {}
@@ -1646,22 +1616,14 @@
         )
         return TeaCore.from_map(
             fc__open_20210406_models.ListFunctionAsyncInvokeConfigsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def list_function_async_invoke_configs(self, service_name, function_name, request):
-        """
-        StatefulAsyncInvocation indicates whether the asynchronous task feature is enabled. If StatefulAsyncInvocation is set to true, the asynchronous task is enabled. All asynchronous invocations to the function corresponding to this configuration change to asynchronous task mode.
-        
-
-        @param request: ListFunctionAsyncInvokeConfigsRequest
-
-        @return: ListFunctionAsyncInvokeConfigsResponse
-        """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.ListFunctionAsyncInvokeConfigsHeaders()
         return self.list_function_async_invoke_configs_with_options(service_name, function_name, request, headers, runtime)
 
     def list_functions_with_options(self, service_name, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
@@ -1707,16 +1669,16 @@
     def list_functions(self, service_name, request):
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.ListFunctionsHeaders()
         return self.list_functions_with_options(service_name, request, headers, runtime)
 
     def list_instances_with_options(self, service_name, function_name, request, headers, runtime):
         """
-        The ListInstances operation allows you to query the available instances of a function.
-        Available instances are instances that are processing requests or can be scheduled to process requests. Available instances queried by the ListInstances operation are the same as those that can be used when you call the InvokeFunction operation with the same values specified for the `serviceName`, `functionName`, and `qualifier` parameters.
+        The maximum number of resources to return. Valid values: \\[0,1000].
+        The number of returned resources is less than or equal to the specified number.
         
 
         @param request: ListInstancesRequest
 
         @param headers: ListInstancesHeaders
 
         @param runtime: runtime options for this request RuntimeOptions
@@ -1754,16 +1716,16 @@
         return TeaCore.from_map(
             fc__open_20210406_models.ListInstancesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def list_instances(self, service_name, function_name, request):
         """
-        The ListInstances operation allows you to query the available instances of a function.
-        Available instances are instances that are processing requests or can be scheduled to process requests. Available instances queried by the ListInstances operation are the same as those that can be used when you call the InvokeFunction operation with the same values specified for the `serviceName`, `functionName`, and `qualifier` parameters.
+        The maximum number of resources to return. Valid values: \\[0,1000].
+        The number of returned resources is less than or equal to the specified number.
         
 
         @param request: ListInstancesRequest
 
         @return: ListInstancesResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2079,15 +2041,15 @@
     def list_services(self, request):
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.ListServicesHeaders()
         return self.list_services_with_options(request, headers, runtime)
 
     def list_stateful_async_invocation_functions_with_options(self, request, headers, runtime):
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The metadata of the service and function to which the asynchronous task belongs.
         
 
         @param request: ListStatefulAsyncInvocationFunctionsRequest
 
         @param headers: ListStatefulAsyncInvocationFunctionsHeaders
 
         @param runtime: runtime options for this request RuntimeOptions
@@ -2127,28 +2089,28 @@
         return TeaCore.from_map(
             fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def list_stateful_async_invocation_functions(self, request):
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The metadata of the service and function to which the asynchronous task belongs.
         
 
         @param request: ListStatefulAsyncInvocationFunctionsRequest
 
         @return: ListStatefulAsyncInvocationFunctionsResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsHeaders()
         return self.list_stateful_async_invocation_functions_with_options(request, headers, runtime)
 
     def list_stateful_async_invocations_with_options(self, service_name, function_name, request, headers, runtime):
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The name of the service to which the asynchronous task belongs.
         
 
         @param request: ListStatefulAsyncInvocationsRequest
 
         @param headers: ListStatefulAsyncInvocationsHeaders
 
         @param runtime: runtime options for this request RuntimeOptions
@@ -2208,15 +2170,15 @@
         return TeaCore.from_map(
             fc__open_20210406_models.ListStatefulAsyncInvocationsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def list_stateful_async_invocations(self, service_name, function_name, request):
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The name of the service to which the asynchronous task belongs.
         
 
         @param request: ListStatefulAsyncInvocationsRequest
 
         @return: ListStatefulAsyncInvocationsResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2382,15 +2344,15 @@
     def publish_service_version(self, service_name, request):
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.PublishServiceVersionHeaders()
         return self.publish_service_version_with_options(service_name, request, headers, runtime)
 
     def put_function_async_invoke_config_with_options(self, service_name, function_name, request, headers, runtime):
         """
-        StatefulAsyncInvocation specifies the configurations of the asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The maximum validity period of messages.
         
 
         @param request: PutFunctionAsyncInvokeConfigRequest
 
         @param headers: PutFunctionAsyncInvokeConfigHeaders
 
         @param runtime: runtime options for this request RuntimeOptions
@@ -2438,15 +2400,15 @@
         return TeaCore.from_map(
             fc__open_20210406_models.PutFunctionAsyncInvokeConfigResponse(),
             self.call_api(params, req, runtime)
         )
 
     def put_function_async_invoke_config(self, service_name, function_name, request):
         """
-        StatefulAsyncInvocation specifies the configurations of the asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The maximum validity period of messages.
         
 
         @param request: PutFunctionAsyncInvokeConfigRequest
 
         @return: PutFunctionAsyncInvokeConfigResponse
         """
         runtime = util_models.RuntimeOptions()
```

### Comparing `alibabacloud_fc-open20210406_py2-2.0.8/alibabacloud_fc_open20210406/models.py` & `alibabacloud_fc-open20210406_py2-2.0.9/alibabacloud_fc_open20210406/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -2891,20 +2891,20 @@
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class CreateAliasRequest(TeaModel):
     def __init__(self, additional_version_weight=None, alias_name=None, description=None, resolve_policy=None,
                  route_policy=None, version_id=None):
-        # The canary release version to which the alias points and the weight of the canary release version.
+        # The additional version to which the alias points and the weight of the additional version.
         # 
-        # *   The canary release version takes effect only when the function is invoked.
+        # *   The additional version takes effect only when the function is invoked.
         # *   The value consists of a version number and a specific weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
         self.additional_version_weight = additional_version_weight  # type: dict[str, float]
-        # The name of the alias.  The name contains only letters, digits, hyphens (-), and underscores (\_). The name must be 1 to 128 characters in length and cannot start with a digit or hyphen (-).  The name cannot be **LATEST**.
+        # The name of the alias. The name can contain letters, digits, underscores (\_), and hyphens (-) only. The name cannot start with a digit or a hyphen (-). The name must be 1 to 128 characters in length. The name cannot be set to **LATEST**\
         self.alias_name = alias_name  # type: str
         # The description of the alias.
         self.description = description  # type: str
         # The canary release mode. Valid values:
         # 
         # *   **Random**: random canary release. This is the default value.
         # *   **Content**: rule-based canary release.
@@ -2955,17 +2955,17 @@
             self.version_id = m.get('versionId')
         return self
 
 
 class CreateAliasResponseBody(TeaModel):
     def __init__(self, additional_version_weight=None, alias_name=None, created_time=None, description=None,
                  last_modified_time=None, version_id=None):
-        # The canary release version to which the alias points and the weight of the canary release version.
+        # The additional version to which the alias points and the weight of the additional version.
         # 
-        # *   The canary release version takes effect only when the function is invoked.
+        # *   The additional version takes effect only when the function is invoked.
         # *   The value consists of a version number and a specific weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
         self.additional_version_weight = additional_version_weight  # type: dict[str, float]
         # The name of the alias.
         self.alias_name = alias_name  # type: str
         # The time when the alias was created.
         self.created_time = created_time  # type: str
         # The description of the alias.
@@ -3301,21 +3301,17 @@
         return self
 
 
 class CreateFunctionHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_code_checksum=None, x_fc_date=None,
                  x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The CRC-64 value of the function code package.
         self.x_fc_code_checksum = x_fc_code_checksum  # type: str
-        # The time on which the function is invoked. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the request. The value is the same as that of the requestId parameter in the response.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateFunctionHeaders, self).to_map()
@@ -3352,69 +3348,36 @@
 
 class CreateFunctionRequest(TeaModel):
     def __init__(self, ca_port=None, code=None, cpu=None, custom_container_config=None, custom_dns=None,
                  custom_health_check_config=None, custom_runtime_config=None, description=None, disk_size=None, environment_variables=None,
                  function_name=None, gpu_memory_size=None, handler=None, initialization_timeout=None, initializer=None,
                  instance_concurrency=None, instance_lifecycle_config=None, instance_soft_concurrency=None, instance_type=None,
                  layers=None, memory_size=None, runtime=None, timeout=None):
-        # The port on which the HTTP server listens for the custom runtime or custom container runtime.
         self.ca_port = ca_port  # type: int
-        # The code of the function. The code must be packaged into a ZIP file. Choose **code** or **customContainerConfig** for the function.
         self.code = code  # type: Code
-        # The number of vCPUs of the function. The value must be a multiple of 0.05.
         self.cpu = cpu  # type: float
-        # The configurations of the custom container runtime. After you configure the custom container runtime, Function Compute can execute the function in a container created from a custom image. Choose **code** or **customContainerConfig** for the function.
         self.custom_container_config = custom_container_config  # type: CustomContainerConfig
-        # The custom Domain Name System (DNS) configurations of the function.
         self.custom_dns = custom_dns  # type: CustomDNS
-        # The custom health check configurations of the function. This parameter is applicable to only custom runtimes and custom containers.
         self.custom_health_check_config = custom_health_check_config  # type: CustomHealthCheckConfig
-        # The configurations of the custom runtime.
         self.custom_runtime_config = custom_runtime_config  # type: CustomRuntimeConfig
-        # The description of the function.
         self.description = description  # type: str
-        # The disk size of the function. Unit: MB. Valid values: 512 and 10240.
         self.disk_size = disk_size  # type: int
-        # The environment variables that you configured for the function. You can obtain the values of the environment variables from the function. For more information, see [Overview](~~69777~~).
         self.environment_variables = environment_variables  # type: dict[str, str]
-        # The name of the function. The name can contain letters, digits, underscores (\_), and hyphens (-) only. The name cannot start with a digit or a hyphen (-). The name must be 1 to 64 characters in length.
         self.function_name = function_name  # type: str
-        # The GPU memory capacity for the function. Unit: MB. The value must be a multiple of 1,024.
         self.gpu_memory_size = gpu_memory_size  # type: int
-        # The handler of the function. The format varies based on the programming language. For more information, see [Function handlers](~~157704~~).
         self.handler = handler  # type: str
-        # The timeout period for the execution of the Initializer hook. Unit: seconds. Default value: 3. Valid values: 1 to 300. When this period expires, the execution of the Initializer hook is terminated.
         self.initialization_timeout = initialization_timeout  # type: int
-        # The handler of the Initializer hook. For more information, see [Initializer hooks](~~157704~~).
         self.initializer = initializer  # type: str
-        # The number of requests that can be concurrently processed by a single instance.
         self.instance_concurrency = instance_concurrency  # type: int
-        # The lifecycle configurations of the instance.
         self.instance_lifecycle_config = instance_lifecycle_config  # type: InstanceLifecycleConfig
-        # The soft concurrency of the instance. You can use this parameter to implement graceful scale-up of instances. If the number of concurrent requests on an instance is greater than the value of soft concurrency, an instance scale-up is triggered. For example, if your instance requires a long time to start, you can specify a suitable soft concurrency to start the instance in advance.
-        # 
-        # The value must be less than or equal to that of the **instanceConcurrency** parameter.
         self.instance_soft_concurrency = instance_soft_concurrency  # type: int
-        # The instance type of the function. Valid values:
-        # 
-        # *   **e1**: elastic instance
-        # *   **c1**: performance instance
-        # *   **fc.gpu.tesla.1**: GPU-accelerated instance (Tesla T4)
-        # *   **fc.gpu.ampere.1**: GPU-accelerated instance (Ampere A10)
-        # *   **g1**: same as **fc.gpu.tesla.1**\
         self.instance_type = instance_type  # type: str
-        # The information about layers.
-        # 
-        # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name as a layer with a larger subscript.
         self.layers = layers  # type: list[str]
-        # The memory size for the function. Unit: MB. The value must be a multiple of 64. The memory size varies based on the function instance type. For more information, see [Instance types](~~179379~~).
         self.memory_size = memory_size  # type: int
-        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom** and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
         self.runtime = runtime  # type: str
-        # The timeout period for the execution of the function. Unit: seconds. Default value: 3. Minimum value: 1. When the period ends, the execution of the function is terminated.
         self.timeout = timeout  # type: int
 
     def validate(self):
         if self.code:
             self.code.validate()
         if self.custom_container_config:
             self.custom_container_config.validate()
@@ -3541,77 +3504,40 @@
 class CreateFunctionResponseBody(TeaModel):
     def __init__(self, ca_port=None, code_checksum=None, code_size=None, cpu=None, created_time=None,
                  custom_container_config=None, custom_dns=None, custom_health_check_config=None, custom_runtime_config=None,
                  description=None, disk_size=None, environment_variables=None, function_id=None, function_name=None,
                  gpu_memory_size=None, handler=None, initialization_timeout=None, initializer=None, instance_concurrency=None,
                  instance_lifecycle_config=None, instance_soft_concurrency=None, instance_type=None, last_modified_time=None, layers=None,
                  memory_size=None, runtime=None, timeout=None):
-        # The port on which the HTTP server listens for the custom runtime or custom container runtime.
         self.ca_port = ca_port  # type: int
-        # The CRC-64 value of the function code package.
         self.code_checksum = code_checksum  # type: str
-        # The size of the function code package that is returned by the system. Unit: bytes.
         self.code_size = code_size  # type: long
-        # The number of vCPUs of the function. The value is a multiple of 0.05.
         self.cpu = cpu  # type: float
-        # The time when the function was created.
         self.created_time = created_time  # type: str
-        # The configurations of the custom container runtime. After you configure the custom container runtime, Function Compute can execute the function in a container created from a custom image.
         self.custom_container_config = custom_container_config  # type: CustomContainerConfig
-        # The custom DNS configurations of the function.
         self.custom_dns = custom_dns  # type: CustomDNS
-        # The custom health check configuration of the function. This parameter is applicable only to custom runtimes and custom containers.
         self.custom_health_check_config = custom_health_check_config  # type: CustomHealthCheckConfig
-        # The configurations of the custom runtime.
         self.custom_runtime_config = custom_runtime_config  # type: CustomRuntimeConfig
-        # The description of the function.
         self.description = description  # type: str
-        # The disk size of the function. Unit: MB. Valid values: 512 and 10240.
         self.disk_size = disk_size  # type: int
-        # The environment variables that are configured for the function. You can obtain the values of the environment variables from the function. For more information, see [Environment variables](~~69777~~).
         self.environment_variables = environment_variables  # type: dict[str, str]
-        # The unique ID that is generated by the system for the function.
         self.function_id = function_id  # type: str
-        # The name of the function.
         self.function_name = function_name  # type: str
-        # The GPU memory capacity for the function. Unit: MB. The value is a multiple of 1,024.
         self.gpu_memory_size = gpu_memory_size  # type: int
-        # The handler of the function.
         self.handler = handler  # type: str
-        # The timeout period for the execution of the Initializer hook. Unit: seconds. Default value: 3. Minimum value: 1. When the period ends, the execution of the Initializer hook is terminated.
         self.initialization_timeout = initialization_timeout  # type: int
-        # The handler of the Initializer hook. The format is determined by the programming language.
         self.initializer = initializer  # type: str
-        # The number of requests that can be concurrently processed by a single instance.
         self.instance_concurrency = instance_concurrency  # type: int
-        # The lifecycle configurations of the instance.
         self.instance_lifecycle_config = instance_lifecycle_config  # type: InstanceLifecycleConfig
-        # The soft concurrency of the instance. You can use this parameter to implement graceful scale-up of instances. If the number of concurrent requests on an instance is greater than the value of soft concurrency, an instance scale-up is triggered. For example, if your instance requires a long time to start, you can specify a suitable soft concurrency to start the instance in advance.
-        # 
-        # The value must be less than or equal to that of the **instanceConcurrency** parameter.
         self.instance_soft_concurrency = instance_soft_concurrency  # type: int
-        # The instance type of the function. Valid values:
-        # 
-        # *   **e1**: elastic instance
-        # *   **c1**: performance instance
-        # *   **fc.gpu.tesla.1**: GPU-accelerated instance (Tesla T4)
-        # *   **fc.gpu.ampere.1**: GPU-accelerated instance (Ampere A10)
-        # *   **g1**: same as **fc.gpu.tesla.1**\
         self.instance_type = instance_type  # type: str
-        # The time when the function was last modified.
         self.last_modified_time = last_modified_time  # type: str
-        # An array that consists of the information of layers.
-        # 
-        # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name as a layer with a larger subscript.
         self.layers = layers  # type: list[str]
-        # The memory size that is configured for the function. Unit: MB.
         self.memory_size = memory_size  # type: int
-        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom** and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
         self.runtime = runtime  # type: str
-        # The timeout period for the execution of the function. Unit: seconds. Default value: 60. Valid values: 1 to 600. When this period expires, the execution of the function is terminated.
         self.timeout = timeout  # type: int
 
     def validate(self):
         if self.custom_container_config:
             self.custom_container_config.validate()
         if self.custom_dns:
             self.custom_dns.validate()
@@ -3786,19 +3712,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateLayerVersionHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # The description of the layer.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The checksum of the layer code package.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the invocation request of Function Compute.
+        # The information about the layer code package.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateLayerVersionHeaders, self).to_map()
@@ -3827,19 +3753,19 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class CreateLayerVersionRequest(TeaModel):
     def __init__(self, code=None, compatible_runtime=None, description=None):
-        # The code of the layer.
+        # The name of the layer.
         self.code = code  # type: Code
-        # The list of runtime environments that are supported by the layer.
+        # The name of the runtime. Valid values: **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **php7.2**, **go1**, **dotnetcore2.1** and **custom**.
         self.compatible_runtime = compatible_runtime  # type: list[str]
-        # The description of the layer.
+        # The name of the layer.
         self.description = description  # type: str
 
     def validate(self):
         if self.code:
             self.code.validate()
 
     def to_map(self):
@@ -3867,33 +3793,32 @@
             self.description = m.get('description')
         return self
 
 
 class CreateLayerVersionResponseBody(TeaModel):
     def __init__(self, acl=None, arn=None, code=None, code_checksum=None, codesize=None, compatible_runtime=None,
                  create_time=None, description=None, layer_name=None, version=None):
-        # The access mode of the layer.
+        # Creates a layer version.
         self.acl = acl  # type: int
-        # The name of the layer.
         self.arn = arn  # type: str
-        # The information about the layer code package.
+        # The access mode of the layer.
         self.code = code  # type: OutputCodeLocation
-        # The checksum of the layer code package.
+        # Example 1
         self.code_checksum = code_checksum  # type: str
         # The size of the layer code package. Unit: Byte.
         self.codesize = codesize  # type: long
-        # The list of runtime environments that are supported by the layer.
+        # Luoni
         self.compatible_runtime = compatible_runtime  # type: list[str]
-        # The time when the layer version was created. The time follows the **yyyy-MM-ddTHH:mm:ssZ** format.
+        # Creates a layer version.
         self.create_time = create_time  # type: str
-        # The description of the layer version.
-        self.description = description  # type: str
         # The name of the layer.
+        self.description = description  # type: str
+        # The list of runtime environments that are supported by the layer.
         self.layer_name = layer_name  # type: str
-        # The version of the layer.
+        # The time when the layer version was created. The time follows the **yyyy-MM-ddTHH:mm:ssZ** format.
         self.version = version  # type: int
 
     def validate(self):
         if self.code:
             self.code.validate()
 
     def to_map(self):
@@ -4276,19 +4201,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateTriggerHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
-        self.x_fc_account_id = x_fc_account_id  # type: str
         # The time when the request is initiated on the client. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
-        self.x_fc_date = x_fc_date  # type: str
+        self.x_fc_account_id = x_fc_account_id  # type: str
         # The custom request ID.
+        self.x_fc_date = x_fc_date  # type: str
+        # The ETag that is used to modify the trigger. This parameter is used to ensure that the modified trigger is consistent with the trigger to be modified.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateTriggerHeaders, self).to_map()
@@ -4318,43 +4243,43 @@
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class CreateTriggerRequest(TeaModel):
     def __init__(self, description=None, invocation_role=None, qualifier=None, source_arn=None, trigger_config=None,
                  trigger_name=None, trigger_type=None):
-        # The description of the trigger.
+        # The ID of your Alibaba Cloud account.
         self.description = description  # type: str
-        # The role that is used by the event source such as OSS to invoke the function. For more information, see [Overview](~~53102~~).
-        self.invocation_role = invocation_role  # type: str
         # The version or alias of the service.
-        self.qualifier = qualifier  # type: str
+        self.invocation_role = invocation_role  # type: str
         # The Alibaba Cloud Resource Name (ARN) of the event source for the trigger.
-        self.source_arn = source_arn  # type: str
+        self.qualifier = qualifier  # type: str
         # The configurations of the trigger. The configurations vary based on the trigger type. For more information about the format, see the following topics:
         # 
         # * OSS trigger: [OSSTriggerConfig](~~struct:OSSTriggerConfig~~).
         # * Log Service trigger: [LogTriggerConfig](~~struct:LogTriggerConfig~~).
         # * Time trigger: [TimeTriggerConfig](~~struct:LogTriggerConfig~~).
         # * HTTP trigger: [HTTPTriggerConfig](~~struct:HTTPTriggerConfig~~).
         # * Tablestore trigger: Specify the **SourceArn** parameter and leave this parameter empty.
         # * Alibaba Cloud CDN event trigger: [CDNEventsTriggerConfig](~~struct:CDNEventsTriggerConfig~~).
         # * MNS topic trigger: [MnsTopicTriggerConfig](~~struct:MnsTopicTriggerConfig~~).
-        self.trigger_config = trigger_config  # type: str
+        self.source_arn = source_arn  # type: str
         # The name of the trigger. The name contains only letters, digits, hyphens (-), and underscores (\_). The name must be 1 to 128 characters in length and cannot start with a digit or hyphen (-).
-        self.trigger_name = trigger_name  # type: str
+        self.trigger_config = trigger_config  # type: str
         # The type of the trigger. Valid values:
         # 
         # *   **oss**: OSS event trigger. For more information, see [Overview](~~62922~~).
         # *   **log**: Log Service trigger. For more information, see [Overview](~~84386~~).
         # *   **timer**: time trigger. For more information, see [Overview](~~68172~~).
         # *   **http**: HTTP trigger. For more information, see [Overview](~~71229~~).
         # *   **tablestore**: Tablestore trigger. For more information, see [Overview](~~100092~~).
         # *   **cdn_events**: CDN event trigger. For more information, see [Overview](~~73333~~).
         # *   **mns_topic**: MNS topic trigger. For more information, see [Overview](~~97032~~).
+        self.trigger_name = trigger_name  # type: str
+        # The description of the trigger.
         self.trigger_type = trigger_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateTriggerRequest, self).to_map()
@@ -4397,39 +4322,38 @@
         return self
 
 
 class CreateTriggerResponseBody(TeaModel):
     def __init__(self, created_time=None, description=None, domain_name=None, invocation_role=None,
                  last_modified_time=None, qualifier=None, source_arn=None, trigger_config=None, trigger_id=None, trigger_name=None,
                  trigger_type=None, url_internet=None, url_intranet=None):
-        # The time when the trigger was created.
+        # The ARN of the RAM role that is used by the event source to invoke the function.
         self.created_time = created_time  # type: str
-        # The description of the trigger.
+        # The unique ID of the trigger.
         self.description = description  # type: str
-        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
+        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
         self.domain_name = domain_name  # type: str
-        # The ARN of the RAM role that is used by the event source to invoke the function.
-        self.invocation_role = invocation_role  # type: str
         # The time when the trigger was last modified.
-        self.last_modified_time = last_modified_time  # type: str
+        self.invocation_role = invocation_role  # type: str
         # The version of the service.
-        self.qualifier = qualifier  # type: str
+        self.last_modified_time = last_modified_time  # type: str
         # The ARN of the event source.
-        self.source_arn = source_arn  # type: str
+        self.qualifier = qualifier  # type: str
         # The configurations of the trigger. The configurations vary based on the trigger type.
+        self.source_arn = source_arn  # type: str
+        # The name of the trigger. The name contains only letters, digits, hyphens (-), and underscores (\_). The name must be 1 to 128 characters in length and cannot start with a digit or hyphen (-).
         self.trigger_config = trigger_config  # type: str
-        # The unique ID of the trigger.
+        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
         self.trigger_id = trigger_id  # type: str
-        # The name of the trigger. The name contains only letters, digits, hyphens (-), and underscores (\_). The name must be 1 to 128 characters in length and cannot start with a digit or hyphen (-).
-        self.trigger_name = trigger_name  # type: str
         # The trigger type, such as **oss**, **log**, **tablestore**, **timer**, **http**, **cdn_events**, and **mns_topic**.
+        self.trigger_name = trigger_name  # type: str
+        # The description of the trigger.
         self.trigger_type = trigger_type  # type: str
-        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
-        self.url_internet = url_internet  # type: str
         # The private endpoint. In a VPC, you can access HTTP triggers by using HTTP or HTTPS.
+        self.url_internet = url_internet  # type: str
         self.url_intranet = url_intranet  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateTriggerResponseBody, self).to_map()
@@ -4534,19 +4458,18 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateVpcBindingHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # Binds a VPC.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # {"name":"CreateVpcBinding","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/services/{serviceName}/bindings","deprecated":0,"method":"POST","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"serviceName\",\"position\":\"Path\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"A short description of struct\",\"description\":\"The name of the service. \",\"example\":\"demo-service\"},{\"name\":\"body\",\"position\":\"Body\",\"style\":\"json\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Object\",\"params\":[{\"name\":\"vpcId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of the VPC to be bound. \",\"example\":\"v-xxxx\"}],\"description\":\"The structure of the request. \"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. Specify the time in the yyyy-mm-ddhh:mm:ss format. \",\"example\":\"2022-01-0112:00:00\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The custom request ID. \",\"example\":\"asdf****\"}]","response_headers":"[]","response":"{}","body_style":"json","errors":"{}"}
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateVpcBindingHeaders, self).to_map()
@@ -4575,15 +4498,15 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class CreateVpcBindingRequest(TeaModel):
     def __init__(self, vpc_id=None):
-        # The ID of the VPC to be bound.
+        # Example 1
         self.vpc_id = vpc_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateVpcBindingRequest, self).to_map()
@@ -4631,23 +4554,20 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class DeleteAliasHeaders(TeaModel):
     def __init__(self, common_headers=None, if_match=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # If the ETag specified in the request matches the ETag value of the object, OSS transmits the object and returns 200 OK. If the ETag specified in the request does not match the ETag value of the object, OSS returns 412 Precondition Failed. 
-        # The ETag value of a resource is used to check whether the resource has changed. You can check data integrity by using the ETag value. 
-        # Default value: null
+        # {"name":"DeleteAlias","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/services/{serviceName}/aliases/{aliasName}","deprecated":0,"method":"DELETE","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"serviceName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the service.\",\"description\":\"The name of the service.\",\"example\":\"demo-service\"},{\"name\":\"aliasName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the alias.\",\"description\":\"The name of the alias.\",\"example\":\"test\"},{\"name\":\"If-Match\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"If the ETag specified in the request matches the ETag value of the object, OSS transmits the object and returns 200 OK. If the ETag specified in the request does not match the ETag value of the object, OSS returns 412 Precondition Failed. \\nThe ETag value of a resource is used to check whether the resource has changed. You can check data integrity by using the ETag value. \\nDefault value: null\",\"example\":\"e19d5cd5af0378da05f63f891c7467af\"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. \",\"example\":\"2020-12-1210:00:00\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The trace ID of the invocation request of Function Compute. \",\"example\":\"r9s89isisi****\"}]","response_headers":"[]","response":"{}","errors":"{}"}
         self.if_match = if_match  # type: str
-        # The ID of your Alibaba Cloud account.
+        # 139490
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Xiaoqi
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteAliasHeaders, self).to_map()
@@ -4711,19 +4631,18 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class DeleteCustomDomainHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # 150868
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Xiawan
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteCustomDomainHeaders, self).to_map()
@@ -4783,21 +4702,19 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class DeleteFunctionHeaders(TeaModel):
     def __init__(self, common_headers=None, if_match=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ETag value of the resource. This value is used to ensure that the modified resource is consistent with the resource to be modified. The ETag value is returned in the responses of the CREATE, GET, and UPDATE operations.
+        # $.parameters[8].schema.description
         self.if_match = if_match  # type: str
-        # The ID of your Alibaba Cloud account.
+        # {"name":"DeleteFunction","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/services/{serviceName}/functions/{functionName}","deprecated":0,"method":"DELETE","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"If-Match\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The ETag value of the resource. This value is used to ensure that the modified resource is consistent with the resource to be modified. The ETag value is returned in the responses of the CREATE, GET, and UPDATE operations.\",\"description\":\"The ETag value of the resource. This value is used to ensure that the modified resource is consistent with the resource to be modified. The ETag value is returned in the responses of the CREATE, GET, and UPDATE operations. \",\"example\":\"e19d5cd5af0378da05f63f891c7467af\"},{\"name\":\"serviceName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the service.\",\"description\":\"The name of the service. \",\"example\":\"demoService\"},{\"name\":\"functionName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the function.\",\"description\":\"The name of the function. \",\"example\":\"demoFunction\"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The start time when the function is invoked. Specify the time in the yyyy-mm-ddhh:mm:ss format. \",\"example\":\"2022-01-01 12:00:00\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The trace ID of the request for Function Compute API. The value is the same as that of the requestId parameter in the response. \",\"example\":\"test-trace-id\"}]","response_headers":"[]","response":"{}","errors":"{}"}
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the request for Function Compute API. The value is the same as that of the requestId parameter in the response.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteFunctionHeaders, self).to_map()
@@ -4861,19 +4778,18 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class DeleteFunctionAsyncInvokeConfigHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # {"name":"DeleteFunctionAsyncInvokeConfig","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/services/{serviceName}/functions/{functionName}/async-invoke-config","deprecated":0,"method":"DELETE","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"serviceName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the service.\",\"description\":\"The name of the service. \",\"example\":\"demo-service\"},{\"name\":\"functionName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the function.\",\"description\":\"The name of the function. \",\"example\":\"helloworld\"},{\"name\":\"qualifier\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The qualifier.\",\"description\":\"The qualifier. \",\"example\":\"test\"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. \",\"example\":\"None\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The trace ID of the invocation request of Function Compute.\",\"example\":\"asdf*****\"}]","response_headers":"[]","response":"{}","errors":"{}"}
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Jianyi
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteFunctionAsyncInvokeConfigHeaders, self).to_map()
@@ -4902,15 +4818,15 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class DeleteFunctionAsyncInvokeConfigRequest(TeaModel):
     def __init__(self, qualifier=None):
-        # The qualifier.
+        # Deletes the asynchronous invocation configurations of a function in a service.
         self.qualifier = qualifier  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteFunctionAsyncInvokeConfigRequest, self).to_map()
@@ -4958,21 +4874,19 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class DeleteFunctionOnDemandConfigHeaders(TeaModel):
     def __init__(self, common_headers=None, if_match=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # If the ETag specified in the request matches the ETag value of the OndemandConfig, FC returns 200 OK. If the ETag specified in the request does not match the ETag value of the object, FC returns 412 Precondition Failed.
+        # Xiaoqi
         self.if_match = if_match  # type: str
-        # The ID of your Alibaba Cloud account.
+        # 65332
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The start time when the function is invoked. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the request for Function Compute API, which is also the unique ID of the request.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteFunctionOnDemandConfigHeaders, self).to_map()
@@ -5005,15 +4919,15 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class DeleteFunctionOnDemandConfigRequest(TeaModel):
     def __init__(self, qualifier=None):
-        # The alias of the service or LATEST.
+        # Deletes the on-demand configuration of a function.
         self.qualifier = qualifier  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteFunctionOnDemandConfigRequest, self).to_map()
@@ -5061,19 +4975,18 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class DeleteLayerVersionHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # 320124
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Luoni
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the request for Function Compute API.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteLayerVersionHeaders, self).to_map()
@@ -5133,21 +5046,19 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class DeleteServiceHeaders(TeaModel):
     def __init__(self, common_headers=None, if_match=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ETag value of the service. This value is used to ensure that the modified service is consistent with the service to be modified. The ETag value is returned in the responses of the [CreateService](~~175256~~), [UpdateService](~~188167~~), and [GetService](~~189225~~) operations.
+        # Examples
         self.if_match = if_match  # type: str
-        # The ID of your Alibaba Cloud account.
+        # Liuxia
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteServiceHeaders, self).to_map()
@@ -5211,19 +5122,17 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class DeleteServiceVersionHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # Xiaoqi
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteServiceVersionHeaders, self).to_map()
@@ -5283,21 +5192,17 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class DeleteTriggerHeaders(TeaModel):
     def __init__(self, common_headers=None, if_match=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # This parameter is used to ensure that the modified resource is consistent with the resource to be modified. You can obtain the parameter value from the responses of [CreateTrigger](~~415729~~), [GetTrigger](~~415732~~), and [UpdateTrigger](~~415731~~) operations.
         self.if_match = if_match  # type: str
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when the request is initiated on the client. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteTriggerHeaders, self).to_map()
@@ -5361,19 +5266,18 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class DeleteVpcBindingHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # Deletes a bound VPC.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # {"name":"DeleteVpcBinding","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/services/{serviceName}/bindings/{vpcId}","deprecated":0,"method":"DELETE","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"serviceName\",\"position\":\"Path\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The name of the service. \",\"example\":\"demoService\"},{\"name\":\"vpcId\",\"position\":\"Path\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of the VPC to be unbound. \",\"example\":\"vpc-xxxx\"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. Specify the time in the yyyy-mm-ddhh:mm:ss format. \",\"example\":\"2022-01-0112:00:00\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The custom request ID. \",\"example\":\"asdf****\"}]","response_headers":"[]","response":"{}","errors":"{}"}
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteVpcBindingHeaders, self).to_map()
@@ -5433,19 +5337,16 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class DeregisterEventSourceHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeregisterEventSourceHeaders, self).to_map()
@@ -5474,15 +5375,14 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class DeregisterEventSourceRequest(TeaModel):
     def __init__(self, qualifier=None):
-        # The version or alias of the service.
         self.qualifier = qualifier  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeregisterEventSourceRequest, self).to_map()
@@ -5532,17 +5432,17 @@
 
 
 class GetAccountSettingsHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Example 1
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
+        # Queries available zones within the current account.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetAccountSettingsHeaders, self).to_map()
@@ -5571,17 +5471,16 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class GetAccountSettingsResponseBody(TeaModel):
     def __init__(self, available_azs=None, default_role=None):
-        # The list of zones.
+        # Liuxia
         self.available_azs = available_azs  # type: list[str]
-        # The default RAM role.
         self.default_role = default_role  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetAccountSettingsResponseBody, self).to_map()
@@ -5644,15 +5543,15 @@
 
 
 class GetAliasHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The start time when the function is invoked. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The time on which the function is invoked. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date  # type: str
         # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
@@ -5684,33 +5583,33 @@
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class GetAliasResponseBody(TeaModel):
     def __init__(self, additional_version_weight=None, alias_name=None, created_time=None, description=None,
                  last_modified_time=None, resolve_policy=None, route_policy=None, version_id=None):
-        # The canary release version to which the alias points and the weight of the canary release version. 
+        # The additional version to which the alias points and the weight of the additional version.
         # 
-        # - The canary release version takes effect only when the function is invoked. 
-        # - The value consists of a version number and the corresponding weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
+        # *   The additional version takes effect only when the function is invoked.
+        # *   The value consists of a version number and a specific weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
         self.additional_version_weight = additional_version_weight  # type: dict[str, float]
         # The name of the alias.
         self.alias_name = alias_name  # type: str
         # The time when the alias was created.
         self.created_time = created_time  # type: str
         # The description of the alias.
         self.description = description  # type: str
         # The time when the alias was last modified.
         self.last_modified_time = last_modified_time  # type: str
         # The canary release mode. Valid values:
         # 
-        # - **Random**: random canary release. This is the default value.
-        # - **Content**: rule-based canary release.
+        # *   **Random**: random canary release. This is the default value.
+        # *   **Content**: rule-based canary release.
         self.resolve_policy = resolve_policy  # type: str
-        # Canary release rule. The traffic that meets the conditions of the canary release rule is diverted to the canary release instances.
+        # The canary release rule. Traffic that meets the canary release rule is routed to the canary release instance.
         self.route_policy = route_policy  # type: RoutePolicy
         # The version to which the alias points.
         self.version_id = version_id  # type: str
 
     def validate(self):
         if self.route_policy:
             self.route_policy.validate()
@@ -5975,19 +5874,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetFunctionHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # The custom request ID.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time on which the function is invoked. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
+        # The value that is used to ensure that the modified function is consistent with the function that is expected to be modified.
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
+        # The definition of the function.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetFunctionHeaders, self).to_map()
@@ -6016,15 +5915,15 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class GetFunctionRequest(TeaModel):
     def __init__(self, qualifier=None):
-        # The version or alias of the service.
+        # The ID of your Alibaba Cloud account.
         self.qualifier = qualifier  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetFunctionRequest, self).to_map()
@@ -6046,85 +5945,81 @@
 class GetFunctionResponseBody(TeaModel):
     def __init__(self, ca_port=None, code_checksum=None, code_size=None, cpu=None, created_time=None,
                  custom_container_config=None, custom_dns=None, custom_health_check_config=None, custom_runtime_config=None,
                  description=None, disk_size=None, environment_variables=None, function_id=None, function_name=None,
                  gpu_memory_size=None, handler=None, initialization_timeout=None, initializer=None, instance_concurrency=None,
                  instance_lifecycle_config=None, instance_soft_concurrency=None, instance_type=None, last_modified_time=None, layers=None,
                  layers_arn_v2=None, memory_size=None, runtime=None, timeout=None):
-        # The port on which the HTTP server listens for the custom runtime or custom container runtime.
+        # The list of layers (ARN V1 version).
+        # 
+        # > If multiple layers exist, the layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file with the same name in the layer with a larger subscript. >
+        # 
+        # **\
+        # 
+        # **Warning:** This parameter is to be deprecated. Use layersArnV2.
         self.ca_port = ca_port  # type: int
-        # The CRC-64 value of the function code package.
+        # The time when the function was created.
         self.code_checksum = code_checksum  # type: str
-        # The size of the function code package. Unit: byte.
+        # The description of the function.
         self.code_size = code_size  # type: long
-        # The number of vCPUs of the function. The value must be a multiple of 0.05.
+        # The GPU memory capacity for the function. Unit: MB. The memory capacity must be a multiple of 1024 MB.
         self.cpu = cpu  # type: float
-        # The time when the function was created.
+        # The environment variables that are configured for the function. You can obtain the values of the environment variables from the function. For more information, see [Environment variables](~~69777~~).
         self.created_time = created_time  # type: str
-        # The configurations of the custom container runtime. After you configure the custom container runtime, Function Compute can execute the function in a container created from a custom image.
+        # The name of the layer resource (ARN V1 version).
         self.custom_container_config = custom_container_config  # type: CustomContainerConfigInfo
-        # The custom DNS configurations of the function.
-        self.custom_dns = custom_dns  # type: CustomDNS
         # The custom health check configuration of the function. This parameter is applicable only to custom runtimes and custom containers.
+        self.custom_dns = custom_dns  # type: CustomDNS
+        # The name of the layer resource (ARN V2 version).
         self.custom_health_check_config = custom_health_check_config  # type: CustomHealthCheckConfig
-        # The configurations of the custom runtime.
+        # The list of layers (ARN V2 version).
+        # 
+        # > If multiple layers exist, the layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name and a larger subscript in the layer.
         self.custom_runtime_config = custom_runtime_config  # type: CustomRuntimeConfig
-        # The description of the function.
+        # The environment variables that you configured for the function.
         self.description = description  # type: str
-        # The disk size of the function. Unit: MB. Valid values: 512 and 10240.
         self.disk_size = disk_size  # type: int
-        # The environment variables that are configured for the function. You can obtain the values of the environment variables from the function. For more information, see [Environment variables](~~69777~~).
-        self.environment_variables = environment_variables  # type: dict[str, str]
         # The ID that is generated by the system for the function. Each function ID is unique in Function Compute.
+        self.environment_variables = environment_variables  # type: dict[str, str]
+        # The handler of the function. For more information, see [Function handler](~~157704~~).
         self.function_id = function_id  # type: str
-        # The name of the function.
+        # The time when the function was last modified.
         self.function_name = function_name  # type: str
-        # The GPU memory capacity for the function. Unit: MB. The memory capacity must be a multiple of 1024 MB.
         self.gpu_memory_size = gpu_memory_size  # type: int
-        # The handler of the function. For more information, see [Function handler](~~157704~~).
+        # The memory size for the function. Unit: MB. The memory size must be a multiple of 64 MB. The memory size varies based on the function instance type. For more information, see [Instance types](~~179379~~).
         self.handler = handler  # type: str
-        # The timeout period for the execution of the initializer function. Unit: seconds. Default value: 3. Valid values: 1 to 300. When this period ends, the execution of the initializer function is terminated.
+        # The port on which the HTTP server listens for the custom runtime or custom container runtime.
         self.initialization_timeout = initialization_timeout  # type: int
-        # The handler of the initializer function. The format of the value is determined by the programming language that you use. For more information, see [Initializer function](~~157704~~).
+        # The configurations of the custom container runtime. After you configure the custom container runtime, Function Compute can execute the function in a container created from a custom image.
         self.initializer = initializer  # type: str
-        # The number of requests that can be concurrently processed by a single instance.
-        self.instance_concurrency = instance_concurrency  # type: int
-        # The lifecycle configurations of the instance.
-        self.instance_lifecycle_config = instance_lifecycle_config  # type: InstanceLifecycleConfig
-        # The soft concurrency of the instance. You can use this parameter to implement graceful scale-up of instances. If the number of concurrent requests on an instance is greater than the number of the soft concurrency, the instance scale-up is triggered. For example, if your instance requires a long time to start, you can specify a suitable soft concurrency to start the instance in advance.
-        # 
-        # The value must be less than or equal to that of the **instanceConcurrency** parameter.
-        self.instance_soft_concurrency = instance_soft_concurrency  # type: int
         # The instance type of the function. Valid values:
         # 
         # *   **e1**: elastic instance
         # *   **c1**: performance instance
         # *   **fc.gpu.tesla.1**: GPU-accelerated instances (Tesla T4)
         # *   **fc.gpu.ampere.1**: GPU-accelerated instances (Ampere A10)
         # *   **g1**: same fc.gpu.tesla.1
+        self.instance_concurrency = instance_concurrency  # type: int
+        # The configurations of the custom runtime.
+        self.instance_lifecycle_config = instance_lifecycle_config  # type: InstanceLifecycleConfig
+        # The lifecycle configurations of the instance.
+        self.instance_soft_concurrency = instance_soft_concurrency  # type: int
+        # The custom DNS configurations of the function.
         self.instance_type = instance_type  # type: str
-        # The time when the function was last modified.
+        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore2.1**, **custom**, and **custom-container**.
         self.last_modified_time = last_modified_time  # type: str
-        # The list of layers (ARN V1 version).
-        # 
-        # > If multiple layers exist, the layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file with the same name in the layer with a larger subscript. >
-        # 
-        # **\
-        # 
-        # **Warning:** This parameter is to be deprecated. Use layersArnV2.
+        # The number of requests that can be concurrently processed by a single instance.
         self.layers = layers  # type: list[str]
-        # The list of layers (ARN V2 version).
-        # 
-        # > If multiple layers exist, the layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name and a larger subscript in the layer.
+        # The number of vCPUs of the function. The value must be a multiple of 0.05.
         self.layers_arn_v2 = layers_arn_v2  # type: list[str]
-        # The memory size for the function. Unit: MB. The memory size must be a multiple of 64 MB. The memory size varies based on the function instance type. For more information, see [Instance types](~~179379~~).
+        # The timeout period for the execution of the function. Unit: seconds. Default value: 60. Valid values: 1 to 600. When this period expires, the execution of the function is terminated.
         self.memory_size = memory_size  # type: int
-        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore2.1**, **custom**, and **custom-container**.
+        # The timeout period for the execution of the initializer function. Unit: seconds. Default value: 3. Valid values: 1 to 300. When this period ends, the execution of the initializer function is terminated.
         self.runtime = runtime  # type: str
-        # The timeout period for the execution of the function. Unit: seconds. Default value: 60. Valid values: 1 to 600. When this period expires, the execution of the function is terminated.
+        # The handler of the initializer function. The format of the value is determined by the programming language that you use. For more information, see [Initializer function](~~157704~~).
         self.timeout = timeout  # type: int
 
     def validate(self):
         if self.custom_container_config:
             self.custom_container_config.validate()
         if self.custom_dns:
             self.custom_dns.validate()
@@ -6303,19 +6198,16 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetFunctionAsyncInvokeConfigHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when the Function Compute is called. The format is **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetFunctionAsyncInvokeConfigHeaders, self).to_map()
@@ -6344,15 +6236,14 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class GetFunctionAsyncInvokeConfigRequest(TeaModel):
     def __init__(self, qualifier=None):
-        # The qualifier.
         self.qualifier = qualifier  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetFunctionAsyncInvokeConfigRequest, self).to_map()
@@ -6370,34 +6261,22 @@
             self.qualifier = m.get('qualifier')
         return self
 
 
 class GetFunctionAsyncInvokeConfigResponseBody(TeaModel):
     def __init__(self, created_time=None, destination_config=None, function=None, last_modified_time=None,
                  max_async_event_age_in_seconds=None, max_async_retry_attempts=None, qualifier=None, service=None, stateful_invocation=None):
-        # The time when the desktop group was created.
         self.created_time = created_time  # type: str
-        # The configuration structure of the destination for asynchronous invocations.
         self.destination_config = destination_config  # type: DestinationConfig
-        # The name of the function.
         self.function = function  # type: str
-        # The time when the configuration was last modified.
         self.last_modified_time = last_modified_time  # type: str
-        # The maximum validity period of a message.
         self.max_async_event_age_in_seconds = max_async_event_age_in_seconds  # type: long
-        # The maximum number of retries allowed after an asynchronous invocation fails.
         self.max_async_retry_attempts = max_async_retry_attempts  # type: long
-        # The version or alias of the service to which the function belongs.
         self.qualifier = qualifier  # type: str
-        # The name of the service.
         self.service = service  # type: str
-        # Indicates whether the asynchronous task feature is enabled.
-        # 
-        # *   **true**: The asynchronous task feature is enabled.
-        # *   **false**: The asynchronous task feature is disabled.
         self.stateful_invocation = stateful_invocation  # type: bool
 
     def validate(self):
         if self.destination_config:
             self.destination_config.validate()
 
     def to_map(self):
@@ -6488,19 +6367,16 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetFunctionCodeHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time on which the function is invoked. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetFunctionCodeHeaders, self).to_map()
@@ -6529,15 +6405,14 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class GetFunctionCodeRequest(TeaModel):
     def __init__(self, qualifier=None):
-        # The version or alias of the service.
         self.qualifier = qualifier  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetFunctionCodeRequest, self).to_map()
@@ -6554,17 +6429,15 @@
         if m.get('qualifier') is not None:
             self.qualifier = m.get('qualifier')
         return self
 
 
 class GetFunctionCodeResponseBody(TeaModel):
     def __init__(self, checksum=None, url=None):
-        # The CRC-64 value of the function code package.
         self.checksum = checksum  # type: str
-        # The URL of the function code package.
         self.url = url  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetFunctionCodeResponseBody, self).to_map()
@@ -6762,19 +6635,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetLayerVersionHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # This parameter is returned only when the information about a specific layer version is queried.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The location of the layer code.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the request for Function Compute API.
+        # The structure of the layer code.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetLayerVersionHeaders, self).to_map()
@@ -7028,19 +6901,22 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetResourceTagsHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # The Alibaba Cloud Resource Name (ARN) of the resource. 
+        # > **Note:** You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource. You can manage tags only for services for top level resources.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The tag dictionary. Valid values:
+        # - **key**: the key of the tag. 
+        # - **value**: the value of the tag.
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
+        # Example 1
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetResourceTagsHeaders, self).to_map()
@@ -7069,17 +6945,16 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class GetResourceTagsRequest(TeaModel):
     def __init__(self, resource_arn=None):
-        # The Alibaba Cloud Resource Name (ARN) of the resource. 
-        # 
-        # > You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource. You can manage tags only for services for top level resources.
+        # The ARN of the resource. 
+        # > **Note:** You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource.
         self.resource_arn = resource_arn  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetResourceTagsRequest, self).to_map()
@@ -7096,19 +6971,16 @@
         if m.get('resourceArn') is not None:
             self.resource_arn = m.get('resourceArn')
         return self
 
 
 class GetResourceTagsResponseBody(TeaModel):
     def __init__(self, resource_arn=None, tags=None):
-        # The ARN of the resource. 
-        # 
-        # > You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource.
+        # 147258
         self.resource_arn = resource_arn  # type: str
-        # The tag dictionary.
         self.tags = tags  # type: dict[str, str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetResourceTagsResponseBody, self).to_map()
@@ -7389,31 +7261,25 @@
         return self
 
 
 class GetStatefulAsyncInvocationHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_code_checksum=None, x_fc_date=None,
                  x_fc_invocation_type=None, x_fc_log_type=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # The list of events that trigger the asynchronous task.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The CRC-64 value of the function code package. This value is used to check data integrity. The value is automatically calculated by the tool.
+        # The structure of the asynchronous task.
         self.x_fc_code_checksum = x_fc_code_checksum  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Alibaba Cloud provides SDKs for multiple programming languages to help you integrate Alibaba Cloud services by using APIs. We recommend that you use an SDK to call API operations. This frees you from manual signature verification.
         self.x_fc_date = x_fc_date  # type: str
-        # The invocation method. 
-        # 
-        # - **Sync**: synchronous invocation 
-        # - **Async**: asynchronous invocation
+        # StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
         self.x_fc_invocation_type = x_fc_invocation_type  # type: str
-        # The method used to return logs. Valid values: 
-        # 
-        # - **Tail**: returns the last 4 KB of logs that are generated for the current request. 
-        # - **None**: does not return logs for the current request. This is the default value.
+        # The latest version of Function Compute API.
         self.x_fc_log_type = x_fc_log_type  # type: str
-        # The trace ID of the invocation request of Function Compute.
+        # You can search for API operations, call and debug API operations online, and dynamically generate executable sample code for SDKs.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetStatefulAsyncInvocationHeaders, self).to_map()
@@ -7454,15 +7320,15 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class GetStatefulAsyncInvocationRequest(TeaModel):
     def __init__(self, qualifier=None):
-        # The version or alias of the service to which the asynchronous task belongs.
+        # The ID of the instance that is used to run the asynchronous task.
         self.qualifier = qualifier  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetStatefulAsyncInvocationRequest, self).to_map()
@@ -7519,19 +7385,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetTriggerHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
-        self.x_fc_account_id = x_fc_account_id  # type: str
         # The time when the request is initiated on the client. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
-        self.x_fc_date = x_fc_date  # type: str
+        self.x_fc_account_id = x_fc_account_id  # type: str
         # The custom request ID.
+        self.x_fc_date = x_fc_date  # type: str
+        # The ETag that is used to modify the trigger. This parameter is used to ensure that the modified trigger is consistent with the trigger to be modified.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetTriggerHeaders, self).to_map()
@@ -7562,47 +7428,46 @@
         return self
 
 
 class GetTriggerResponseBody(TeaModel):
     def __init__(self, created_time=None, description=None, domain_name=None, invocation_role=None,
                  last_modified_time=None, qualifier=None, source_arn=None, trigger_config=None, trigger_id=None, trigger_name=None,
                  trigger_type=None, url_internet=None, url_intranet=None):
-        # The time when the trigger was created.
+        # The ARN of the RAM role that is used by the event source to invoke the function.
         self.created_time = created_time  # type: str
-        # The description of the trigger.
+        # The unique ID of the trigger.
         self.description = description  # type: str
-        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
+        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
         self.domain_name = domain_name  # type: str
-        # The ARN of the RAM role that is used by the event source to invoke the function.
-        self.invocation_role = invocation_role  # type: str
         # The time when the trigger was last modified.
-        self.last_modified_time = last_modified_time  # type: str
+        self.invocation_role = invocation_role  # type: str
         # The version or alias of the service.
-        self.qualifier = qualifier  # type: str
+        self.last_modified_time = last_modified_time  # type: str
         # The ARN of the event source.
-        self.source_arn = source_arn  # type: str
+        self.qualifier = qualifier  # type: str
         # The configurations of the trigger. The configurations vary based on the trigger type. For more information about the format, see the following topics:
         # 
         # *   OSS trigger: [OSSTriggerConfig](~~struct:OSSTriggerConfig~~).
         # *   Log Service trigger: [LogTriggerConfig](~~struct:LogTriggerConfig~~).
         # *   Time trigger: [TimeTriggerConfig](~~struct:TimeTriggerConfig~~).
         # *   HTTP trigger: [HTTPTriggerConfig](~~struct:HTTPTriggerConfig~~).
         # *   Tablestore trigger: Specify the **SourceArn** parameter and leave this parameter empty.
         # *   Alibaba Cloud CDN event trigger: [CDNEventsTriggerConfig](~~struct:CDNEventsTriggerConfig~~).
         # *   MNS topic trigger: [MnsTopicTriggerConfig](~~struct:MnsTopicTriggerConfig~~).
+        self.source_arn = source_arn  # type: str
+        # The name of the trigger.
         self.trigger_config = trigger_config  # type: str
-        # The unique ID of the trigger.
+        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
         self.trigger_id = trigger_id  # type: str
-        # The name of the trigger.
-        self.trigger_name = trigger_name  # type: str
         # The trigger type, such as **oss**, **log**, **tablestore**, **timer**, **http**, **cdn_events**, and **mns_topic**.
+        self.trigger_name = trigger_name  # type: str
+        # The description of the trigger.
         self.trigger_type = trigger_type  # type: str
-        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
-        self.url_internet = url_internet  # type: str
         # The private endpoint. In a VPC, you can access HTTP triggers by using HTTP or HTTPS.
+        self.url_internet = url_internet  # type: str
         self.url_intranet = url_intranet  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetTriggerResponseBody, self).to_map()
@@ -7706,15 +7571,16 @@
             temp_model = GetTriggerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class InvokeFunctionHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_invocation_type=None,
-                 x_fc_log_type=None, x_fc_stateful_async_invocation_id=None, x_fc_trace_id=None):
+                 x_fc_log_type=None, x_fc_stateful_async_invocation_enable=None, x_fc_stateful_async_invocation_id=None,
+                 x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
         # The time when the function is invoked. The format is **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date  # type: str
         # The method used to invoke the function. Valid values:
         # 
@@ -7722,14 +7588,15 @@
         # *   **Async**: asynchronous
         self.x_fc_invocation_type = x_fc_invocation_type  # type: str
         # The method used to return logs. Valid values:
         # 
         # *   **Tail**: returns the last 4 KB of logs that are generated for the current request.
         # *   **None**: No logs are returned for the current request. Default value: None.
         self.x_fc_log_type = x_fc_log_type  # type: str
+        self.x_fc_stateful_async_invocation_enable = x_fc_stateful_async_invocation_enable  # type: str
         # The ID of the asynchronous task. You must enable the asynchronous task feature in advance.
         # 
         # > When you use an SDK to invoke a function, we recommend that you specify a business-related ID to facilitate subsequent operations. For example, you can use the video name as the invocation ID for a video-processing function. This way, you can use the ID to check whether the video is processed or terminate the processing of the video. The ID must start with a letter or an underscore (\_) and can contain letters, digits, underscores (\_), and hyphens (-). The ID can be up to 128 characters in length. If you do not specify the ID of the asynchronous invocation, Function Compute automatically generates an ID.
         self.x_fc_stateful_async_invocation_id = x_fc_stateful_async_invocation_id  # type: str
         # The trace ID of the request for Function Compute API. The value is the same as that of the **requestId** parameter in the response.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
@@ -7748,14 +7615,16 @@
             result['X-Fc-Account-Id'] = self.x_fc_account_id
         if self.x_fc_date is not None:
             result['X-Fc-Date'] = self.x_fc_date
         if self.x_fc_invocation_type is not None:
             result['X-Fc-Invocation-Type'] = self.x_fc_invocation_type
         if self.x_fc_log_type is not None:
             result['X-Fc-Log-Type'] = self.x_fc_log_type
+        if self.x_fc_stateful_async_invocation_enable is not None:
+            result['X-Fc-Stateful-Async-Invocation-Enable'] = self.x_fc_stateful_async_invocation_enable
         if self.x_fc_stateful_async_invocation_id is not None:
             result['X-Fc-Stateful-Async-Invocation-Id'] = self.x_fc_stateful_async_invocation_id
         if self.x_fc_trace_id is not None:
             result['X-Fc-Trace-Id'] = self.x_fc_trace_id
         return result
 
     def from_map(self, m=None):
@@ -7766,14 +7635,16 @@
             self.x_fc_account_id = m.get('X-Fc-Account-Id')
         if m.get('X-Fc-Date') is not None:
             self.x_fc_date = m.get('X-Fc-Date')
         if m.get('X-Fc-Invocation-Type') is not None:
             self.x_fc_invocation_type = m.get('X-Fc-Invocation-Type')
         if m.get('X-Fc-Log-Type') is not None:
             self.x_fc_log_type = m.get('X-Fc-Log-Type')
+        if m.get('X-Fc-Stateful-Async-Invocation-Enable') is not None:
+            self.x_fc_stateful_async_invocation_enable = m.get('X-Fc-Stateful-Async-Invocation-Enable')
         if m.get('X-Fc-Stateful-Async-Invocation-Id') is not None:
             self.x_fc_stateful_async_invocation_id = m.get('X-Fc-Stateful-Async-Invocation-Id')
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
@@ -7845,15 +7716,15 @@
 
 
 class ListAliasesHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The start time when the function is invoked. Specify the time in the yyyy-mm-ddhh:mm:ss format.
+        # The time on which the function is invoked. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date  # type: str
         # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
@@ -7884,21 +7755,21 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class ListAliasesRequest(TeaModel):
     def __init__(self, limit=None, next_token=None, prefix=None, start_key=None):
-        # The maximum number of resources to return.
+        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
         self.limit = limit  # type: int
-        # The token used to obtain more results.
+        # The token required to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
         self.next_token = next_token  # type: str
-        # The prefix.
+        # The prefix that the names of returned resources must contain.
         self.prefix = prefix  # type: str
-        # The starting position of the result list.
+        # The starting position of the result list. The returned resources are sorted in alphabetical order, and the resources that include and follow the resource specified by the startKey parameter are returned.
         self.start_key = start_key  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListAliasesRequest, self).to_map()
@@ -7928,25 +7799,33 @@
             self.start_key = m.get('startKey')
         return self
 
 
 class ListAliasesResponseBodyAliases(TeaModel):
     def __init__(self, additional_version_weight=None, alias_name=None, created_time=None, description=None,
                  last_modified_time=None, resolve_policy=None, route_policy=None, version_id=None):
-        # The weight of the canary release version.
+        # The additional version to which the alias points and the weight of the additional version.
+        # 
+        # *   The additional version takes effect only when the function is invoked.
+        # *   The value consists of a version number and a specific weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
         self.additional_version_weight = additional_version_weight  # type: dict[str, float]
         # The name of the alias.
         self.alias_name = alias_name  # type: str
-        # The creation time.
+        # The time when the ConfigMaps were created.
         self.created_time = created_time  # type: str
         # The description of the alias.
         self.description = description  # type: str
-        # The last update time.
+        # The time at which the system parameter was last modified.
         self.last_modified_time = last_modified_time  # type: str
+        # The canary release mode. Valid values:
+        # 
+        # *   **Random**: random canary release. This is the default value.
+        # *   **Content**: rule-based canary release.
         self.resolve_policy = resolve_policy  # type: str
+        # The canary release rule. Traffic that meets the canary release rule is routed to the canary release instance.
         self.route_policy = route_policy  # type: RoutePolicy
         # The ID of the version.
         self.version_id = version_id  # type: str
 
     def validate(self):
         if self.route_policy:
             self.route_policy.validate()
@@ -8332,19 +8211,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListEventSourcesHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # $.parameters[7].schema.enumValueTitles
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # $.parameters[8].schema.description
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the invocation request of Function Compute.
+        # $.parameters[8].schema.example
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListEventSourcesHeaders, self).to_map()
@@ -8373,15 +8252,15 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class ListEventSourcesRequest(TeaModel):
     def __init__(self, qualifier=None):
-        # The version or alias of the service.
+        # $.parameters[7].schema.example
         self.qualifier = qualifier  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListEventSourcesRequest, self).to_map()
@@ -8398,17 +8277,16 @@
         if m.get('qualifier') is not None:
             self.qualifier = m.get('qualifier')
         return self
 
 
 class ListEventSourcesResponseBodyEventSources(TeaModel):
     def __init__(self, created_time=None, source_arn=None):
-        # The time when the event source was created.
         self.created_time = created_time  # type: str
-        # The ARN of the event source.
+        # Jianyi
         self.source_arn = source_arn  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListEventSourcesResponseBodyEventSources, self).to_map()
@@ -8429,15 +8307,15 @@
         if m.get('sourceArn') is not None:
             self.source_arn = m.get('sourceArn')
         return self
 
 
 class ListEventSourcesResponseBody(TeaModel):
     def __init__(self, event_sources=None):
-        # The information about event sources.
+        # Queries all the event sources of a function.
         self.event_sources = event_sources  # type: list[ListEventSourcesResponseBodyEventSources]
 
     def validate(self):
         if self.event_sources:
             for k in self.event_sources:
                 if k:
                     k.validate()
@@ -8503,31 +8381,19 @@
         return self
 
 
 class ListFunctionAsyncInvokeConfigsHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_code_checksum=None, x_fc_date=None,
                  x_fc_invocation_type=None, x_fc_log_type=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The CRC-64 value of the function code package. This value is used to check data integrity. The value is automatically calculated by the tool.
         self.x_fc_code_checksum = x_fc_code_checksum  # type: str
-        # The time when the Function Compute is called. The format is **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date  # type: str
-        # The invocation method.
-        # 
-        # *   **Sync**: synchronous
-        # *   **Async**: asynchronous
         self.x_fc_invocation_type = x_fc_invocation_type  # type: str
-        # The method used to return logs. Valid values:
-        # 
-        # *   **Tail**: returns the last 4 KB of logs that are generated for the current request.
-        # *   **None**: No logs are returned for the current request. Default value: None.
         self.x_fc_log_type = x_fc_log_type  # type: str
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListFunctionAsyncInvokeConfigsHeaders, self).to_map()
@@ -8568,17 +8434,15 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class ListFunctionAsyncInvokeConfigsRequest(TeaModel):
     def __init__(self, limit=None, next_token=None):
-        # The maximum number of resources to return.
         self.limit = limit  # type: int
-        # The token required to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
         self.next_token = next_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListFunctionAsyncInvokeConfigsRequest, self).to_map()
@@ -8600,36 +8464,22 @@
             self.next_token = m.get('nextToken')
         return self
 
 
 class ListFunctionAsyncInvokeConfigsResponseBodyConfigs(TeaModel):
     def __init__(self, created_time=None, destination_config=None, function=None, last_modified_time=None,
                  max_async_event_age_in_seconds=None, max_async_retry_attempts=None, qualifier=None, service=None, stateful_invocation=None):
-        # The time when the desktop group was created.
         self.created_time = created_time  # type: str
-        # The configuration structure of the destination for asynchronous invocations. If you have not configured this parameter, this parameter is null.
         self.destination_config = destination_config  # type: DestinationConfig
-        # The name of the function.
         self.function = function  # type: str
-        # The time when the configuration was last modified.
         self.last_modified_time = last_modified_time  # type: str
-        # The maximum validity period of a message. If you have not configured this parameter, this parameter is null.
         self.max_async_event_age_in_seconds = max_async_event_age_in_seconds  # type: long
-        # The maximum number of retries allowed after an asynchronous invocation fails. If you have not configured this parameter, this parameter is null.
         self.max_async_retry_attempts = max_async_retry_attempts  # type: long
-        # The version or alias of the service.
         self.qualifier = qualifier  # type: str
-        # The name of the service.
         self.service = service  # type: str
-        # Indicates whether the asynchronous task feature is enabled.
-        # 
-        # *   **true**: The asynchronous task feature is enabled.
-        # *   **false**: The asynchronous task feature is disabled.
-        # 
-        # If you have not configured this parameter, this parameter is null.
         self.stateful_invocation = stateful_invocation  # type: bool
 
     def validate(self):
         if self.destination_config:
             self.destination_config.validate()
 
     def to_map(self):
@@ -8680,17 +8530,15 @@
         if m.get('statefulInvocation') is not None:
             self.stateful_invocation = m.get('statefulInvocation')
         return self
 
 
 class ListFunctionAsyncInvokeConfigsResponseBody(TeaModel):
     def __init__(self, configs=None, next_token=None):
-        # The list of asynchronous invocation configurations.
         self.configs = configs  # type: list[ListFunctionAsyncInvokeConfigsResponseBodyConfigs]
-        # The token used to obtain more results.
         self.next_token = next_token  # type: str
 
     def validate(self):
         if self.configs:
             for k in self.configs:
                 if k:
                     k.validate()
@@ -8910,15 +8758,15 @@
         self.last_modified_time = last_modified_time  # type: str
         # The information about layers.
         # 
         # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name as a layer with a larger subscript.
         self.layers = layers  # type: list[str]
         # The memory size that is configured for the function. Unit: MB.
         self.memory_size = memory_size  # type: int
-        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom** and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
+        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.10**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom.debian10**, **custom**, and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
         self.runtime = runtime  # type: str
         # The timeout period for the execution of the function. Unit: seconds. Default value: 60. Valid values: 1 to 600. When this period expires, the execution of the function is terminated.
         self.timeout = timeout  # type: int
 
     def validate(self):
         if self.custom_container_config:
             self.custom_container_config.validate()
@@ -9120,15 +8968,15 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListInstancesHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # Queries the available instances of a function.
         self.x_fc_account_id = x_fc_account_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListInstancesHeaders, self).to_map()
@@ -9149,21 +8997,19 @@
         if m.get('X-Fc-Account-Id') is not None:
             self.x_fc_account_id = m.get('X-Fc-Account-Id')
         return self
 
 
 class ListInstancesRequest(TeaModel):
     def __init__(self, instance_ids=None, limit=None, qualifier=None):
-        # The IDs of the instance.
+        # The name of the service.
         self.instance_ids = instance_ids  # type: list[str]
-        # The maximum number of resources to return. Valid values: \[0,1000].
-        # 
-        # The number of returned resources is less than or equal to the specified number.
+        # The ID of your Alibaba Cloud account.
         self.limit = limit  # type: int
-        # The version or alias.
+        # The ID of the instance.
         self.qualifier = qualifier  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListInstancesRequest, self).to_map()
@@ -9188,17 +9034,15 @@
         if m.get('qualifier') is not None:
             self.qualifier = m.get('qualifier')
         return self
 
 
 class ListInstancesResponseBodyInstances(TeaModel):
     def __init__(self, instance_id=None, version_id=None):
-        # The ID of the instance.
         self.instance_id = instance_id  # type: str
-        # The version of the service to which the instance belongs. If the instance belongs to the LATEST alias, 0 is returned as the version.
         self.version_id = version_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListInstancesResponseBodyInstances, self).to_map()
@@ -9219,15 +9063,15 @@
         if m.get('versionId') is not None:
             self.version_id = m.get('versionId')
         return self
 
 
 class ListInstancesResponseBody(TeaModel):
     def __init__(self, instances=None):
-        # The information about instances.
+        # 210234
         self.instances = instances  # type: list[ListInstancesResponseBodyInstances]
 
     def validate(self):
         if self.instances:
             for k in self.instances:
                 if k:
                     k.validate()
@@ -9443,19 +9287,16 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListLayersHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when the function is invoked. The format is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the request for Function Compute API.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListLayersHeaders, self).to_map()
@@ -9484,25 +9325,19 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class ListLayersRequest(TeaModel):
     def __init__(self, limit=None, next_token=None, official=None, prefix=None, public=None, start_key=None):
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned configurations is less than or equal to the specified number.
         self.limit = limit  # type: int
-        # The token required to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
         self.next_token = next_token  # type: str
-        # Specifies whether to obtain the official public layer. When the official parameter is set to true, the public field does not take effect. The default value is false.
         self.official = official  # type: bool
-        # The name prefix of the layer. The names of returned resources must contain the prefix. If the name prefix is a, the names of returned resources must start with a.
         self.prefix = prefix  # type: str
-        # Specifies whether to obtain only the common layer. Default value: false.
         self.public = public  # type: bool
-        # The name of the start layer. The returned layers are sorted in alphabetical order, and the layers that include and follow the layer specified by the startKey parameter are returned.
         self.start_key = start_key  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListLayersRequest, self).to_map()
@@ -9539,17 +9374,15 @@
         if m.get('startKey') is not None:
             self.start_key = m.get('startKey')
         return self
 
 
 class ListLayersResponseBody(TeaModel):
     def __init__(self, layers=None, next_token=None):
-        # The information about layers.
         self.layers = layers  # type: list[Layer]
-        # The name of the start layer for the next query, which is also the token used to obtain more results.
         self.next_token = next_token  # type: str
 
     def validate(self):
         if self.layers:
             for k in self.layers:
                 if k:
                     k.validate()
@@ -9618,19 +9451,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListOnDemandConfigsHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # $.parameters[8].schema.description
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # $.parameters[8].schema.example
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the invocation request of Function Compute.
+        # $.parameters[8].schema.enumValueTitles
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListOnDemandConfigsHeaders, self).to_map()
@@ -9659,21 +9492,21 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class ListOnDemandConfigsRequest(TeaModel):
     def __init__(self, limit=None, next_token=None, prefix=None, start_key=None):
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
+        # The time when Function Compute API is called.
         self.limit = limit  # type: int
-        # The token used to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
+        # The ID of your Alibaba Cloud account.
         self.next_token = next_token  # type: str
-        # The prefix that the names of returned resources must contain. If the name prefix is a, the names of returned resources must start with a.
+        # The returned data.
         self.prefix = prefix  # type: str
-        # The returned resources are sorted in alphabetical order, and the resources that include and follow the resource specified by the startKey parameter are returned.
+        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
         self.start_key = start_key  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListOnDemandConfigsRequest, self).to_map()
@@ -9702,17 +9535,17 @@
         if m.get('startKey') is not None:
             self.start_key = m.get('startKey')
         return self
 
 
 class ListOnDemandConfigsResponseBody(TeaModel):
     def __init__(self, configs=None, next_token=None):
-        # The information about the provisioned configuration.
+        # $.parameters[9].schema.enumValueTitles
         self.configs = configs  # type: list[OnDemandConfig]
-        # The token used to obtain more results. If this parameter is left empty, all the results are returned.
+        # {"name":"ListOnDemandConfigs","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/on-demand-configs","deprecated":0,"method":"GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"prefix\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The prefix that the names of returned resources must contain. If the name prefix is a, the names of returned resources must start with a. \",\"description\":\"The prefix that the names of returned resources must contain. If the name prefix is a, the names of returned resources must start with a. \",\"example\":\"prefix_text\"},{\"name\":\"startKey\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The returned resources are sorted in alphabetical order, and the resources that include and follow the resource specified by the startKey parameter are returned. \",\"description\":\"The returned resources are sorted in alphabetical order, and the resources that include and follow the resource specified by the startKey parameter are returned. \",\"example\":\"nextservice\"},{\"name\":\"nextToken\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The token used to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call. \",\"description\":\"The token used to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call. \",\"example\":\"8bj81uI8n****\"},{\"name\":\"limit\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number. \",\"description\":\"The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number. \",\"example\":\"20\"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. \",\"example\":\"2020-12-1210:00:00\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The trace ID of the invocation request of Function Compute. \",\"example\":\"rid281s******\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"configs\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Array\",\"subType\":\"Object\",\"example\":\"[{\"maximumInstanceCount\": 10, \"resource\": \"services/serviceName-bb7f36eb-7f1b-4c42-8f64-401b32ecbf31.aliasName/functions/functionName\"}]\",\"description\":\"The information about the on-demand configuration. \",\"children\":[{\"name\":\"resource\",\"required\":false,\"checkBlank\":false,\"visibility\":\"public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The details of the function.\",\"description\":\"The description of the resource. \",\"example\":\"123#serviceName#alias#functionName\"},{\"name\":\"maximumInstanceCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"todo\",\"description\":\"The maximum number of on-demand instances. \",\"example\":\"10\"}],\"title\":\"The information about the provisioned configuration.\"},{\"name\":\"nextToken\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The token used to obtain more results. If this parameter is left empty, all the results are returned. \",\"description\":\"The token used to obtain more results. If this parameter is left empty, all the results are returned. \",\"example\":\"next_token\"}],\"title\":\"Schema of Response\",\"description\":\"The returned data. \"}","errors":"{}"}
         self.next_token = next_token  # type: str
 
     def validate(self):
         if self.configs:
             for k in self.configs:
                 if k:
                     k.validate()
@@ -9781,19 +9614,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListProvisionConfigsHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # The actual number of provisioned instances.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Specifies whether to always allocate CPU to a function instance.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the invocation request of Function Compute.
+        # The configurations of scheduled auto scaling.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListProvisionConfigsHeaders, self).to_map()
@@ -9822,21 +9655,21 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class ListProvisionConfigsRequest(TeaModel):
     def __init__(self, limit=None, next_token=None, qualifier=None, service_name=None):
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
+        # Queries provisioned instances.
         self.limit = limit  # type: long
-        # The token used to obtain more results. You do not need to provide this parameter in the first call. The tokens for subsequent queries are obtained from the returned results.
+        # Alibaba Cloud provides SDKs for multiple programming languages to help you integrate Alibaba Cloud services by using APIs. We recommend that you use an SDK to call API operations. This frees you from manual signature verification.
         self.next_token = next_token  # type: str
-        # The qualifier of the service to which resources belong. The qualifier must be aliasName and used together with the serviceName parameter.
+        # The token used to obtain more results.
         self.qualifier = qualifier  # type: str
-        # The name of the service to which resources belong.
+        # It is a tool used to manage and configure Alibaba Cloud resources. After simple installation and configuration, you can use Alibaba Cloud CLI to manage multiple Alibaba Cloud services and migrate your data and business to the cloud with ease.
         self.service_name = service_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListProvisionConfigsRequest, self).to_map()
@@ -9866,27 +9699,31 @@
             self.service_name = m.get('serviceName')
         return self
 
 
 class ListProvisionConfigsResponseBodyProvisionConfigs(TeaModel):
     def __init__(self, always_allocate_cpu=None, current=None, current_error=None, resource=None,
                  scheduled_actions=None, target=None, target_tracking_policies=None):
-        # Specifies whether to always allocate CPU to a function instance.
         self.always_allocate_cpu = always_allocate_cpu  # type: bool
-        # The actual number of provisioned instances.
+        # The expected number of provisioned instances.
         self.current = current  # type: long
-        # The error message returned if a provisioned instance fails to be created.
+        # 139490
         self.current_error = current_error  # type: str
-        # The description of the resource.
+        # Details about the scheduled scaling policy. You can use the scheduled scaling policy to flexibly configure provisioned instances. You can specify the number of provisioned instances to the desired value at the scheduled time. This way, the number of provisioned instances can meet the concurrency requirements of your business.
         self.resource = resource  # type: str
-        # The configurations of scheduled auto scaling.
+        # The ID of your Alibaba Cloud account.
         self.scheduled_actions = scheduled_actions  # type: list[ScheduledActions]
-        # The expected number of provisioned instances.
+        # The configuration of metric-based auto scaling. Provisioned instances are scaled in or out every minute based on the concurrency utilization of provisioned instances. 
+        # 
+        # - If the metric value exceeds the value of the metricTarget parameter, the system scales out provisioned instances based on a progressive policy to make the metric value closer to the value of the metricTarget parameter. 
+        # - When the metric value is smaller than the value of the metricTarget parameter, the system scales in provisioned instances based on a conservative policy to make the metric value close to the value of the metricTarget parameter. 
+        # 
+        # After you specify the maximum and minimum numbers of provisioned instances, the system scales in or out provisioned instances within the range from the minimum number to the maximum number. If the number of provisioned instances is beyond the range, the scaling stops.
         self.target = target  # type: long
-        # The configurations of metric-based auto scaling.
+        # Example 1
         self.target_tracking_policies = target_tracking_policies  # type: list[TargetTrackingPolicies]
 
     def validate(self):
         if self.scheduled_actions:
             for k in self.scheduled_actions:
                 if k:
                     k.validate()
@@ -9944,17 +9781,17 @@
                 temp_model = TargetTrackingPolicies()
                 self.target_tracking_policies.append(temp_model.from_map(k))
         return self
 
 
 class ListProvisionConfigsResponseBody(TeaModel):
     def __init__(self, next_token=None, provision_configs=None):
-        # The token used to obtain more results.
+        # The qualifier of the service to which resources belong. The qualifier must be aliasName and used together with the serviceName parameter.
         self.next_token = next_token  # type: str
-        # The information about provisioned instances.
+        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.provision_configs = provision_configs  # type: list[ListProvisionConfigsResponseBodyProvisionConfigs]
 
     def validate(self):
         if self.provision_configs:
             for k in self.provision_configs:
                 if k:
                     k.validate()
@@ -10023,19 +9860,16 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListReservedCapacitiesHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when the Function Compute API is called. The format is **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListReservedCapacitiesHeaders, self).to_map()
@@ -10064,17 +9898,15 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class ListReservedCapacitiesRequest(TeaModel):
     def __init__(self, limit=None, next_token=None):
-        # The maximum number of resources to return. Valid values: \[1, 100].
         self.limit = limit  # type: str
-        # The token that determines the start point of the query.
         self.next_token = next_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListReservedCapacitiesRequest, self).to_map()
@@ -10095,17 +9927,15 @@
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         return self
 
 
 class ListReservedCapacitiesResponseBody(TeaModel):
     def __init__(self, next_token=None, reserved_capacities=None):
-        # The token used to obtain more results.
         self.next_token = next_token  # type: str
-        # The information about subscription instances.
         self.reserved_capacities = reserved_capacities  # type: list[OpenReservedCapacity]
 
     def validate(self):
         if self.reserved_capacities:
             for k in self.reserved_capacities:
                 if k:
                     k.validate()
@@ -10178,15 +10008,15 @@
 class ListServiceVersionsHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
         # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the invocation request of Function Compute.
+        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListServiceVersionsHeaders, self).to_map()
@@ -10215,23 +10045,21 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class ListServiceVersionsRequest(TeaModel):
     def __init__(self, direction=None, limit=None, next_token=None, start_key=None):
-        # The order in which the returned versions are sorted. Valid values:
-        #   - **FORWARD**: in ascending order. 
-        #   - **BACKWARD**: in descending order. This is the default value.
+        # The name of the service.
         self.direction = direction  # type: str
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
-        self.limit = limit  # type: int
         # The token used to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
+        self.limit = limit  # type: int
+        # The description of the service version.
         self.next_token = next_token  # type: str
-        # The starting position of the result list. The returned resources are sorted based on the version number, and the resources that include and follow the resource specified by the startKey parameter are returned.
+        # The time when the service version was created.
         self.start_key = start_key  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListServiceVersionsRequest, self).to_map()
@@ -10260,21 +10088,20 @@
         if m.get('startKey') is not None:
             self.start_key = m.get('startKey')
         return self
 
 
 class ListServiceVersionsResponseBodyVersions(TeaModel):
     def __init__(self, created_time=None, description=None, last_modified_time=None, version_id=None):
-        # The time when the service version was created.
+        # $.parameters[10].schema.enumValueTitles
         self.created_time = created_time  # type: str
-        # The description of the service version.
+        # Queries all the versions of a service.
         self.description = description  # type: str
-        # The time when the service version was last modified.
+        # Xiaoqi
         self.last_modified_time = last_modified_time  # type: str
-        # The version of the service.
         self.version_id = version_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListServiceVersionsResponseBodyVersions, self).to_map()
@@ -10303,21 +10130,19 @@
         if m.get('versionId') is not None:
             self.version_id = m.get('versionId')
         return self
 
 
 class ListServiceVersionsResponseBody(TeaModel):
     def __init__(self, direction=None, next_token=None, versions=None):
-        # The order in which the returned versions are sorted. Valid values:
-        #   - **FORWARD**: in ascending order. 
-        #   - **BACKWARD**: in descending order. This is the default value.
+        # The information about the version.
         self.direction = direction  # type: str
-        # The token used to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
+        # $.parameters[9].schema.description
         self.next_token = next_token  # type: str
-        # The list of versions.
+        # $.parameters[9].schema.enumValueTitles
         self.versions = versions  # type: list[ListServiceVersionsResponseBodyVersions]
 
     def validate(self):
         if self.versions:
             for k in self.versions:
                 if k:
                     k.validate()
@@ -10666,19 +10491,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListStatefulAsyncInvocationFunctionsHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # It is a tool used to manage and configure Alibaba Cloud resources. After simple installation and configuration, you can use Alibaba Cloud CLI to manage multiple Alibaba Cloud services and migrate your data and business to the cloud with ease.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The token used to obtain more results. If this parameter is left empty, all the results are returned.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the request for Function Compute API.
+        # The details of returned data.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListStatefulAsyncInvocationFunctionsHeaders, self).to_map()
@@ -10707,17 +10532,17 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class ListStatefulAsyncInvocationFunctionsRequest(TeaModel):
     def __init__(self, limit=None, next_token=None):
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
+        # The latest version of Function Compute API.
         self.limit = limit  # type: int
-        # The starting position of the query. If this parameter is left empty, the query starts from the beginning. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
+        # Alibaba Cloud provides SDKs for multiple programming languages to help you integrate Alibaba Cloud services by using APIs. We recommend that you use an SDK to call API operations. This frees you from manual signature verification.
         self.next_token = next_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListStatefulAsyncInvocationFunctionsRequest, self).to_map()
@@ -10738,17 +10563,17 @@
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         return self
 
 
 class ListStatefulAsyncInvocationFunctionsResponseBody(TeaModel):
     def __init__(self, data=None, next_token=None):
-        # The details of returned data.
+        # The trace ID of the request for Function Compute API.
         self.data = data  # type: list[AsyncConfigMeta]
-        # The token used to obtain more results. If this parameter is left empty, all the results are returned.
+        # 2022-01-28 18:04:38
         self.next_token = next_token  # type: str
 
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
@@ -10818,31 +10643,28 @@
         return self
 
 
 class ListStatefulAsyncInvocationsHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_code_checksum=None, x_fc_date=None,
                  x_fc_invocation_type=None, x_fc_log_type=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # It is a tool used to manage and configure Alibaba Cloud resources. After simple installation and configuration, you can use Alibaba Cloud CLI to manage multiple Alibaba Cloud services and migrate your data and business to the cloud with ease.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The CRC-64 value of the function code package. This value is used to check data integrity. The value is automatically calculated by the tool.
+        # Alibaba Cloud CLI
         self.x_fc_code_checksum = x_fc_code_checksum  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
-        self.x_fc_date = x_fc_date  # type: str
-        # The invocation method. 
+        # - **true**: returns the invocationPayload parameter in the response. 
+        # - **false**: does not return the invocationPayload parameter in the response. 
         # 
-        # - **Sync**: synchronous invocation 
-        # - **Async**: asynchronous invocation
+        # > The `invocationPayload` parameter indicates the input parameters of an asynchronous task.
+        self.x_fc_date = x_fc_date  # type: str
+        # The token used to obtain more results. If this parameter is left empty, all the results are returned.
         self.x_fc_invocation_type = x_fc_invocation_type  # type: str
-        # The method used to return logs. Valid values: 
-        # 
-        # - **Tail**: returns the last 4 KB of logs that are generated for the current request. 
-        # - **None**: does not return logs for the current request. This is the default value.
+        # The time when Function Compute API is called.
         self.x_fc_log_type = x_fc_log_type  # type: str
-        # The trace ID of the invocation request of Function Compute.
+        # The CRC-64 value of the function code package. This value is used to check data integrity. The value is automatically calculated by the tool.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListStatefulAsyncInvocationsHeaders, self).to_map()
@@ -10884,47 +10706,31 @@
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class ListStatefulAsyncInvocationsRequest(TeaModel):
     def __init__(self, include_payload=None, invocation_id_prefix=None, limit=None, next_token=None, qualifier=None,
                  sort_order_by_time=None, started_time_begin=None, started_time_end=None, status=None):
-        # - **true**: returns the invocationPayload parameter in the response. 
-        # - **false**: does not return the invocationPayload parameter in the response. 
-        # 
-        # > The `invocationPayload` parameter indicates the input parameters of an asynchronous task.
+        # You can search for API operations, call and debug API operations online, and dynamically generate executable sample code for SDKs.
         self.include_payload = include_payload  # type: bool
-        # The name prefix of the asynchronous invocation. The names of returned resources must contain the prefix. For example, if invocationidPrefix is set to job, the names of returned resources must start with job.
+        # Alibaba Cloud provides SDKs for multiple programming languages to help you integrate Alibaba Cloud services by using APIs. We recommend that you use an SDK to call API operations. This frees you from manual signature verification.
         self.invocation_id_prefix = invocation_id_prefix  # type: str
-        # The maximum number of asynchronous invocations to return. Valid values: [1, 100]. Default value: 50.
+        # The list of events that trigger the asynchronous task.
         self.limit = limit  # type: int
-        # The token used to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
+        # The ID of the instance that is used to run the asynchronous task.
         self.next_token = next_token  # type: str
-        # The version or alias of the service to which the asynchronous task belongs.
+        # The number of retries after the asynchronous task fails.
         self.qualifier = qualifier  # type: str
-        # The order in which the returned asynchronous invocations are sorted. Valid values:
-        # 
-        # - **asc**: in ascending order 
-        # - **desc**: in descending order
+        # StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
         self.sort_order_by_time = sort_order_by_time  # type: str
-        # The start time of the asynchronous task.
+        # The structure of the asynchronous task.
         self.started_time_begin = started_time_begin  # type: long
-        # The end time of the asynchronous task.
+        # The latest version of Function Compute API.
         self.started_time_end = started_time_end  # type: long
-        # The status of the asynchronous task. 
-        # 
-        # - **Enqueued**: The asynchronous invocation is enqueued and is waiting to be executed. 
-        # - **Succeeded**: The invocation is successful. 
-        # - **Failed**: The invocation fails. 
-        # - **Running**: The invocation is being executed. 
-        # - **Stopped**: The invocation is terminated. 
-        # - **Stopping**: The invocation is being terminated. 
-        # - **Invalid**: The invocation is invalid and not executed due to specific reasons. For example, the function is deleted. 
-        # - **Expired**: The maximum validity period of messages is specified for asynchronous invocation. The invocation is discarded and not executed because the specified maximum validity period of messages expires. 
-        # - **Retrying**: The asynchronous invocation is being retried due to an execution error.
+        # The request ID of the asynchronous task.
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListStatefulAsyncInvocationsRequest, self).to_map()
@@ -10973,17 +10779,17 @@
         if m.get('status') is not None:
             self.status = m.get('status')
         return self
 
 
 class ListStatefulAsyncInvocationsResponseBody(TeaModel):
     def __init__(self, invocations=None, next_token=None):
-        # The information about asynchronous tasks.
+        # The version or alias of the service to which the asynchronous task belongs.
         self.invocations = invocations  # type: list[StatefulAsyncInvocation]
-        # The token used to obtain more results. If this parameter is left empty, all the results are returned.
+        # The returned data.
         self.next_token = next_token  # type: str
 
     def validate(self):
         if self.invocations:
             for k in self.invocations:
                 if k:
                     k.validate()
@@ -11052,19 +10858,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListTaggedResourcesHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # Queries all tagged services.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # {"name":"ListTaggedResources","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/tags","deprecated":0,"method":"GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"nextToken\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The token used to obtain more results. You do not need to provide this parameter in the first call. The tokens for subsequent queries are obtained from the returned results. \",\"example\":\"a-service\"},{\"name\":\"limit\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"description\":\"The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number. \",\"example\":\"20\"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. Specify the time in the yyyy-mm-ddhh:mm:ss format. \",\"example\":\"2022-01-01 12:00:00\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The custom request ID. \",\"example\":\"my-test-trace-id\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"nextToken\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The token used to obtain more results. You do not need to provide this parameter in the first call. The tokens for subsequent queries are obtained from the returned results. \",\"example\":\"a-service\"},{\"name\":\"resources\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Array\",\"subType\":\"Object\",\"children\":[{\"name\":\"resourceArn\",\"required\":false,\"checkBlank\":false,\"visibility\":\"public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"resourceArn\",\"description\":\"The Alibaba Cloud Resource Name (ARN). \\n> You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource. You can manage tags only for services for top level resources. \",\"example\":\"acs:fc:cn-shanghai:188077086902****:services/demo\"},{\"name\":\"tags\",\"required\":false,\"checkBlank\":false,\"visibility\":\"public\",\"deprecated\":false,\"type\":\"Map\",\"keyType\":\"String\",\"value\":{\"type\":\"String\",\"required\":false,\"checkBlank\":false,\"visibility\":\"public\",\"deprecated\":false,\"description\":\"The tag dictionary. A tag consists of the following parameters:\\n  - **key**: the key of the tag. \\n  - **value**: the value of the tag. \",\"example\":\"{\\\"k1\\\":\\\"v1\\\" , \\\"k2\\\":\\\"v2\\\"}\"},\"title\":\"tags\",\"description\":\"The tag dictionary. \"}],\"description\":\"The information about tagged services.\"}],\"title\":\"Schema of Response\",\"description\":\"Schema of Response\"}","errors":"{}"}
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
+        # 147258
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTaggedResourcesHeaders, self).to_map()
@@ -11093,15 +10899,15 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class ListTaggedResourcesRequest(TeaModel):
     def __init__(self, limit=None, next_token=None):
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
+        # Example 1
         self.limit = limit  # type: int
         # The token used to obtain more results. You do not need to provide this parameter in the first call. The tokens for subsequent queries are obtained from the returned results.
         self.next_token = next_token  # type: str
 
     def validate(self):
         pass
 
@@ -11124,17 +10930,15 @@
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         return self
 
 
 class ListTaggedResourcesResponseBody(TeaModel):
     def __init__(self, next_token=None, resources=None):
-        # The token used to obtain more results. You do not need to provide this parameter in the first call. The tokens for subsequent queries are obtained from the returned results.
         self.next_token = next_token  # type: str
-        # The information about tagged services.
         self.resources = resources  # type: list[Resource]
 
     def validate(self):
         if self.resources:
             for k in self.resources:
                 if k:
                     k.validate()
@@ -11203,19 +11007,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListTriggersHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
-        self.x_fc_account_id = x_fc_account_id  # type: str
         # The time when the request is initiated on the client. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
-        self.x_fc_date = x_fc_date  # type: str
+        self.x_fc_account_id = x_fc_account_id  # type: str
         # The custom request ID.
+        self.x_fc_date = x_fc_date  # type: str
+        # The returned data.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTriggersHeaders, self).to_map()
@@ -11244,21 +11048,21 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class ListTriggersRequest(TeaModel):
     def __init__(self, limit=None, next_token=None, prefix=None, start_key=None):
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
-        self.limit = limit  # type: int
         # The token required to obtain more results. You do not need to provide this parameter in the first call. The tokens for subsequent queries are obtained from the returned results.
-        self.next_token = next_token  # type: str
+        self.limit = limit  # type: int
         # The prefix that the names of returned resources must contain.
-        self.prefix = prefix  # type: str
+        self.next_token = next_token  # type: str
         # The returned resources are sorted in alphabetical order, and the resources that include and follow the resource specified by the startKey parameter are returned.
+        self.prefix = prefix  # type: str
+        # The ID of your Alibaba Cloud account.
         self.start_key = start_key  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTriggersRequest, self).to_map()
@@ -11289,47 +11093,46 @@
         return self
 
 
 class ListTriggersResponseBodyTriggers(TeaModel):
     def __init__(self, created_time=None, description=None, domain_name=None, invocation_role=None,
                  last_modified_time=None, qualifier=None, source_arn=None, trigger_config=None, trigger_id=None, trigger_name=None,
                  trigger_type=None, url_internet=None, url_intranet=None):
-        # The time when the trigger was created.
+        # The ARN of the RAM role that is used by the event source to invoke the function.
         self.created_time = created_time  # type: str
-        # The description of the trigger.
+        # The unique ID of the trigger.
         self.description = description  # type: str
-        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
+        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
         self.domain_name = domain_name  # type: str
-        # The ARN of the RAM role that is used by the event source to invoke the function.
-        self.invocation_role = invocation_role  # type: str
         # The time when the trigger was last modified.
-        self.last_modified_time = last_modified_time  # type: str
+        self.invocation_role = invocation_role  # type: str
         # The version or alias of the service.
-        self.qualifier = qualifier  # type: str
+        self.last_modified_time = last_modified_time  # type: str
         # The ARN of the event source.
-        self.source_arn = source_arn  # type: str
+        self.qualifier = qualifier  # type: str
         # The configurations of the trigger. The configurations vary based on the trigger type. For more information about the format, see the following topics:
         # 
         # *   OSS trigger: [OSSTriggerConfig](~~struct:OSSTriggerConfig~~).
         # *   Log Service trigger: [LogTriggerConfig](~~struct:LogTriggerConfig~~).
         # *   Time trigger: [TimeTriggerConfig](~~struct:TimeTriggerConfig~~).
         # *   HTTP trigger: [HTTPTriggerConfig](~~struct:HTTPTriggerConfig~~).
         # *   Tablestore trigger: Specify the **SourceArn** parameter and leave this parameter empty.
         # *   Alibaba Cloud CDN event trigger: [CDNEventsTriggerConfig](~~struct:CDNEventsTriggerConfig~~).
         # *   MNS topic trigger: [MnsTopicTriggerConfig](~~struct:MnsTopicTriggerConfig~~).
+        self.source_arn = source_arn  # type: str
+        # The name of the trigger.
         self.trigger_config = trigger_config  # type: str
-        # The unique ID of the trigger.
+        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
         self.trigger_id = trigger_id  # type: str
-        # The name of the trigger.
-        self.trigger_name = trigger_name  # type: str
         # The trigger type, such as **oss**, **log**, **tablestore**, **timer**, **http**, **cdn\_events**, and **mns\_topic**.
+        self.trigger_name = trigger_name  # type: str
+        # The description of the trigger.
         self.trigger_type = trigger_type  # type: str
-        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
-        self.url_internet = url_internet  # type: str
         # The private endpoint. In a VPC, you can access HTTP triggers by using HTTP or HTTPS.
+        self.url_internet = url_internet  # type: str
         self.url_intranet = url_intranet  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTriggersResponseBodyTriggers, self).to_map()
@@ -11394,17 +11197,17 @@
         if m.get('urlIntranet') is not None:
             self.url_intranet = m.get('urlIntranet')
         return self
 
 
 class ListTriggersResponseBody(TeaModel):
     def __init__(self, next_token=None, triggers=None):
-        # The token used to obtain more results. If this parameter is left empty, all the results are returned.
-        self.next_token = next_token  # type: str
         # The information about triggers.
+        self.next_token = next_token  # type: str
+        # The details of the trigger.
         self.triggers = triggers  # type: list[ListTriggersResponseBodyTriggers]
 
     def validate(self):
         if self.triggers:
             for k in self.triggers:
                 if k:
                     k.validate()
@@ -11473,19 +11276,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListVpcBindingsHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # The time when Function Compute API is called. Specify the time in the yyyy-mm-ddhh:mm:ss format.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Example 1
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
+        # Queries the list of VPCs.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListVpcBindingsHeaders, self).to_map()
@@ -11514,15 +11317,14 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class ListVpcBindingsResponseBody(TeaModel):
     def __init__(self, vpc_ids=None):
-        # The IDs of bound VPCs.
         self.vpc_ids = vpc_ids  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListVpcBindingsResponseBody, self).to_map()
@@ -11585,15 +11387,15 @@
         self.common_headers = common_headers  # type: dict[str, str]
         # The ETag value of the service. This value is used to ensure that the modified service is consistent with the service to be modified. The ETag value is returned in the responses of the [CreateService](~~175256~~), [UpdateService](~~188167~~), and [GetService](~~189225~~) operations.
         self.if_match = if_match  # type: str
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
         # The start time when the function is invoked. Specify the time in the yyyy-mm-ddhh:mm:ss format.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the invocation request of Function Compute.
+        # 2020-12-1210:00:00
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PublishServiceVersionHeaders, self).to_map()
@@ -11651,21 +11453,21 @@
         if m.get('description') is not None:
             self.description = m.get('description')
         return self
 
 
 class PublishServiceVersionResponseBody(TeaModel):
     def __init__(self, created_time=None, description=None, last_modified_time=None, version_id=None):
-        # The time when the service version was created.
+        # The returned data.
         self.created_time = created_time  # type: str
-        # The description of the service version.
+        # The creation time.
         self.description = description  # type: str
-        # The time when the service version was last modified.
+        # The description of the service version.
         self.last_modified_time = last_modified_time  # type: str
-        # The version of the service.
+        # The last update time.
         self.version_id = version_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PublishServiceVersionResponseBody, self).to_map()
@@ -11734,19 +11536,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PutFunctionAsyncInvokeConfigHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # The name of the service.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The creation time.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the invocation request of Function Compute.
+        # The maximum number of retries allowed after an asynchronous invocation fails. Default value: 3. Valid values: 0 to 8.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PutFunctionAsyncInvokeConfigHeaders, self).to_map()
@@ -11776,26 +11578,23 @@
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class PutFunctionAsyncInvokeConfigRequest(TeaModel):
     def __init__(self, destination_config=None, max_async_event_age_in_seconds=None,
                  max_async_retry_attempts=None, stateful_invocation=None, qualifier=None):
-        # The configuration structure of the destination for asynchronous invocation.
+        # You can search for API operations, call and debug API operations online, and dynamically generate executable sample code for SDKs.
         self.destination_config = destination_config  # type: DestinationConfig
-        # The maximum validity period of messages. Valid values: 1 to 2592000. Unit: seconds.
+        # Alibaba Cloud CLI
         self.max_async_event_age_in_seconds = max_async_event_age_in_seconds  # type: long
-        # The maximum number of retries allowed after an asynchronous invocation fails. Default value: 3. Valid values: 0 to 8.
+        # The information about the asynchronous invocation configuration.
         self.max_async_retry_attempts = max_async_retry_attempts  # type: long
-        # Specifies whether to enable the asynchronous task feature. 
-        # 
-        # - **true**: enables the asynchronous task feature. 
-        # - **false**: does not enable the asynchronous task feature.
-        self.stateful_invocation = stateful_invocation  # type: bool
         # The version or alias of the service.
+        self.stateful_invocation = stateful_invocation  # type: bool
+        # The latest version of Function Compute API.
         self.qualifier = qualifier  # type: str
 
     def validate(self):
         if self.destination_config:
             self.destination_config.validate()
 
     def to_map(self):
@@ -11831,34 +11630,37 @@
             self.qualifier = m.get('qualifier')
         return self
 
 
 class PutFunctionAsyncInvokeConfigResponseBody(TeaModel):
     def __init__(self, created_time=None, destination_config=None, function=None, last_modified_time=None,
                  max_async_event_age_in_seconds=None, max_async_retry_attempts=None, qualifier=None, service=None, stateful_invocation=None):
-        # The creation time.
+        # Sat, 14 Jul 2017 07:02:38 GMT
         self.created_time = created_time  # type: str
-        # The configuration structure of the destination for asynchronous invocation.
+        # The trace ID of the invocation request of Function Compute.
         self.destination_config = destination_config  # type: DestinationConfig
         # The name of the function.
         self.function = function  # type: str
-        # The time when the configuration was last modified.
+        # The configuration structure of the destination for asynchronous invocation.
         self.last_modified_time = last_modified_time  # type: str
-        # The maximum validity period of messages.
+        # Specifies whether to enable the asynchronous task feature. 
+        # 
+        # - **true**: enables the asynchronous task feature. 
+        # - **false**: does not enable the asynchronous task feature.
         self.max_async_event_age_in_seconds = max_async_event_age_in_seconds  # type: long
-        # The maximum number of retries allowed after an asynchronous invocation fails.
+        # The ID of your Alibaba Cloud account.
         self.max_async_retry_attempts = max_async_retry_attempts  # type: long
-        # The qualifier.
-        self.qualifier = qualifier  # type: str
-        # The name of the service.
-        self.service = service  # type: str
         # Specifies whether to enable the asynchronous task feature. 
         # 
         # - **true**: enables the asynchronous task feature. 
         # - **false**: does not enable the asynchronous task feature.
+        self.qualifier = qualifier  # type: str
+        # Creates or modifies an asynchronous invocation configuration for a function.
+        self.service = service  # type: str
+        # Jianyi
         self.stateful_invocation = stateful_invocation  # type: bool
 
     def validate(self):
         if self.destination_config:
             self.destination_config.validate()
 
     def to_map(self):
@@ -11949,21 +11751,21 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PutFunctionOnDemandConfigHeaders(TeaModel):
     def __init__(self, common_headers=None, if_match=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # If the ETag specified in the request matches the ETag value of the OndemandConfig, FC returns 200 OK. If the ETag specified in the request does not match the ETag value of the object, FC returns 412 Precondition Failed.
+        # The name of the service.
         self.if_match = if_match  # type: str
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The start time when the function is invoked. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Example 1
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the request for Function Compute API, which is also the unique ID of the request.
+        # Creates function rules.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PutFunctionOnDemandConfigHeaders, self).to_map()
@@ -11996,17 +11798,17 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class PutFunctionOnDemandConfigRequest(TeaModel):
     def __init__(self, maximum_instance_count=None, qualifier=None):
-        # The maximum number of on-demand instances. For more information, see [Instance scaling limits](~~185038~~).
+        # The maximum number of instances.
         self.maximum_instance_count = maximum_instance_count  # type: long
-        # The alias of the service or LATEST.
+        # The trace ID of the request for Function Compute API, which is also the unique ID of the request.
         self.qualifier = qualifier  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PutFunctionOnDemandConfigRequest, self).to_map()
@@ -12027,17 +11829,15 @@
         if m.get('qualifier') is not None:
             self.qualifier = m.get('qualifier')
         return self
 
 
 class PutFunctionOnDemandConfigResponseBody(TeaModel):
     def __init__(self, maximum_instance_count=None, resource=None):
-        # The maximum number of instances.
         self.maximum_instance_count = maximum_instance_count  # type: long
-        # The description of the resource.
         self.resource = resource  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PutFunctionOnDemandConfigResponseBody, self).to_map()
@@ -12098,19 +11898,16 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PutLayerACLHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when the operation is called. The format is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the request for Function Compute API.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PutLayerACLHeaders, self).to_map()
@@ -12139,18 +11936,14 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class PutLayerACLRequest(TeaModel):
     def __init__(self, public=None):
-        # Specifies whether the layer is public.
-        # 
-        # *   **true**: Public.
-        # *   **false**: Not public.
         self.public = public  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PutLayerACLRequest, self).to_map()
@@ -12419,19 +12212,17 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RegisterEventSourceHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
+        # Jianyi
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RegisterEventSourceHeaders, self).to_map()
@@ -12460,17 +12251,17 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class RegisterEventSourceRequest(TeaModel):
     def __init__(self, source_arn=None, qualifier=None):
-        # The Alibaba Cloud Resource Name (ARN) of the event source.
+        # {"name":"RegisterEventSource","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/services/{serviceName}/functions/{functionName}/event-sources","deprecated":0,"method":"POST","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"serviceName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the service.\",\"description\":\"The name of the service. \",\"example\":\"demo-service\"},{\"name\":\"functionName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the function.\",\"description\":\"The name of the function. \",\"example\":\"demo-function\"},{\"name\":\"qualifier\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The version or alias of the service.\",\"description\":\"The version or alias of the service. \",\"example\":\"LATEST\"},{\"name\":\"body\",\"position\":\"Body\",\"style\":\"json\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Object\",\"params\":[{\"name\":\"sourceArn\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The Alibaba Cloud Resource Name (ARN) of the event source.\",\"description\":\"The Alibaba Cloud Resource Name (ARN) of the event source.\",\"example\":\"acs:eventbridge:cn-shanghai:123456:eventbus/mns-test/rule/fc-test1/target/abc\"}],\"description\":\"The body of the request. \"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. \",\"example\":\"Sat, 14 Jul 2017 07:02:38 GMT\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The trace ID of the invocation request of Function Compute. \",\"example\":\"asdf****\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"sourceArn\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The Alibaba Cloud Resource Name (ARN) of the event source.\",\"description\":\"The ARN of the event source. \",\"example\":\"acs:eventbridge:cn-shanghai:123456:eventbus/mns-test/rule/fc-test1/target/abc\"},{\"name\":\"createdTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The creation time.\",\"description\":\"The time when the event source was created. \",\"example\":\"2016-08-15T16:06:05.000+0000\"}],\"title\":\"Schema of Response\",\"description\":\"The returned data. \"}","body_style":"json","errors":"{}"}
         self.source_arn = source_arn  # type: str
-        # The version or alias of the service.
+        # asdf****\
         self.qualifier = qualifier  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RegisterEventSourceRequest, self).to_map()
@@ -12491,17 +12282,15 @@
         if m.get('qualifier') is not None:
             self.qualifier = m.get('qualifier')
         return self
 
 
 class RegisterEventSourceResponseBody(TeaModel):
     def __init__(self, created_time=None, source_arn=None):
-        # The time when the event source was created.
         self.created_time = created_time  # type: str
-        # The ARN of the event source.
         self.source_arn = source_arn  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RegisterEventSourceResponseBody, self).to_map()
@@ -12562,19 +12351,16 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ReleaseGPUInstanceHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when the function is invoked. The format of the value is: EEE,d MMM yyyy HH:mm:ss GMT.
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ReleaseGPUInstanceHeaders, self).to_map()
@@ -12731,19 +12517,16 @@
             self.status_code = m.get('statusCode')
         return self
 
 
 class TagResourceHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when the function is invoked. The format is **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date  # type: str
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(TagResourceHeaders, self).to_map()
@@ -12772,19 +12555,15 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class TagResourceRequest(TeaModel):
     def __init__(self, resource_arn=None, tags=None):
-        # The ARN of the resource.
-        # 
-        # > You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource. You can manage tags only for services for top level resources.
         self.resource_arn = resource_arn  # type: str
-        # The tag dictionary.
         self.tags = tags  # type: dict[str, str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(TagResourceRequest, self).to_map()
@@ -12838,15 +12617,15 @@
 
 
 class UntagResourceHeaders(TeaModel):
     def __init__(self, common_headers=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The time when the function is invoked. The value is in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date  # type: str
         # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
@@ -12878,18 +12657,19 @@
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class UntagResourceRequest(TeaModel):
     def __init__(self, all=None, resource_arn=None, tag_keys=None):
         # Specifies whether to remove all tags. This parameter takes effect only when no tag key is specified. Valid values:
-        #   - **true**: removes all tags. 
-        #   - **false**: does not remove all tags.
+        # 
+        # *   **true**\
+        # *   **false**\
         self.all = all  # type: bool
-        # The ARN of the resource. 
+        # The Alibaba Cloud Resource Name (ARN) of the resource.
         # 
         # > You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource. You can manage tags only for services for top level resources.
         self.resource_arn = resource_arn  # type: str
         # The keys of the tags that you want to remove.
         self.tag_keys = tag_keys  # type: list[str]
 
     def validate(self):
@@ -12999,17 +12779,17 @@
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class UpdateAliasRequest(TeaModel):
     def __init__(self, additional_version_weight=None, description=None, resolve_policy=None, route_policy=None,
                  version_id=None):
-        # The canary release version to which the alias points and the weight of the canary release version.
+        # The additional version to which the alias points and the weight of the additional version.
         # 
-        # *   The canary release version takes effect only when the function is invoked.
+        # *   The additional version takes effect only when the function is invoked.
         # *   The value consists of a version number and a specific weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
         self.additional_version_weight = additional_version_weight  # type: dict[str, float]
         # The description of the alias.
         self.description = description  # type: str
         # The canary release mode. Valid values:
         # 
         # *   **Random**: random canary release. This is the default value.
@@ -13057,17 +12837,17 @@
             self.version_id = m.get('versionId')
         return self
 
 
 class UpdateAliasResponseBody(TeaModel):
     def __init__(self, additional_version_weight=None, alias_name=None, created_time=None, description=None,
                  last_modified_time=None, version_id=None):
-        # The canary release version to which the alias points and the weight of the canary release version.
+        # The additional version to which the alias points and the weight of the additional version.
         # 
-        # *   The canary release version takes effect only when the function is invoked.
+        # *   The additional version takes effect only when the function is invoked.
         # *   The value consists of a version number and a specific weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
         self.additional_version_weight = additional_version_weight  # type: dict[str, float]
         # The name of the alias.
         self.alias_name = alias_name  # type: str
         # The time when the alias was created.
         self.created_time = created_time  # type: str
         # The description of the alias.
@@ -13396,23 +13176,18 @@
         return self
 
 
 class UpdateFunctionHeaders(TeaModel):
     def __init__(self, common_headers=None, if_match=None, x_fc_account_id=None, x_fc_code_checksum=None,
                  x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # The parameter that is used to ensure that the modified resource is consistent with the resource to be modified. The value of this parameter is returned in the responses of the [CreateFunction](~~415747~~), [GetFunction](~~415750~~), and [UpdateFunction](~~415749~~) operations.
         self.if_match = if_match  # type: str
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id  # type: str
-        # The CRC-64 value of the function code package.
         self.x_fc_code_checksum = x_fc_code_checksum  # type: str
-        # The time on which the function is invoked. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date  # type: str
-        # The trace ID of the request. The value is the same as that of the requestId parameter in the response.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateFunctionHeaders, self).to_map()
@@ -13453,70 +13228,35 @@
 
 class UpdateFunctionRequest(TeaModel):
     def __init__(self, instance_concurrency=None, ca_port=None, code=None, cpu=None, custom_container_config=None,
                  custom_dns=None, custom_health_check_config=None, custom_runtime_config=None, description=None,
                  disk_size=None, environment_variables=None, gpu_memory_size=None, handler=None, initialization_timeout=None,
                  initializer=None, instance_lifecycle_config=None, instance_soft_concurrency=None, instance_type=None,
                  layers=None, memory_size=None, runtime=None, timeout=None):
-        # The number of requests that can be concurrently processed by a single instance.
         self.instance_concurrency = instance_concurrency  # type: int
-        # The port on which the HTTP server listens for the custom runtime or custom container runtime.
         self.ca_port = ca_port  # type: int
-        # The packaged code of the function. **Function code packages** can be provided with the following two methods. You must use only one of the methods in a request.
-        # 
-        # *   Specify the name of the Object Storage Service (OSS) bucket and object where the code package is stored. The names are specified in the **ossBucketName** and **ossObjectName** parameters.
-        # *   Specify the Base64-encoded content of the ZIP file by using the **zipFile** parameter.
         self.code = code  # type: Code
-        # The number of vCPUs of the function. The value must be a multiple of 0.05.
         self.cpu = cpu  # type: float
-        # The configuration of the custom container. After you configure the custom container, Function Compute can execute the function in a container created from a custom image.
         self.custom_container_config = custom_container_config  # type: CustomContainerConfig
-        # The custom DNS configurations of the function.
         self.custom_dns = custom_dns  # type: CustomDNS
-        # The custom health check configurations of the function. This parameter is applicable to only custom runtimes and custom containers.
         self.custom_health_check_config = custom_health_check_config  # type: CustomHealthCheckConfig
-        # The configurations of the custom runtime.
         self.custom_runtime_config = custom_runtime_config  # type: CustomRuntimeConfig
-        # The description of the function.
         self.description = description  # type: str
-        # The disk size of the function. Unit: MB. Valid values: 512 and 10240.
         self.disk_size = disk_size  # type: int
-        # The environment variables that are configured for the function. You can obtain the values of the environment variables from the function. For more information, see [Environment variables](~~69777~~).
         self.environment_variables = environment_variables  # type: dict[str, str]
-        # The GPU memory capacity for the function. Unit: MB. The value must be a multiple of 1,024.
         self.gpu_memory_size = gpu_memory_size  # type: int
-        # The handler of the function. The format varies based on the programming language. For more information, see [Function handlers](~~157704~~).
         self.handler = handler  # type: str
-        # The timeout period for the execution of the Initializer hook. Unit: seconds. Default value: 3. Minimum value: 1. When the period ends, the execution of the Initializer hook is terminated.
         self.initialization_timeout = initialization_timeout  # type: int
-        # The handler of the Initializer hook. The format is determined by the programming language. For more information, see [Function handlers](~~157704~~).
         self.initializer = initializer  # type: str
-        # The lifecycle configurations of the instance.
         self.instance_lifecycle_config = instance_lifecycle_config  # type: InstanceLifecycleConfig
-        # The soft concurrency of the instance. You can use this parameter to implement graceful scale-up of instances. If the number of concurrent requests on an instance is greater than the value of soft concurrency, an instance scale-up is triggered. For example, if your instance requires a long time to start, you can specify a suitable soft concurrency to start the instance in advance.
-        # 
-        # The value must be less than or equal to that of the **instanceConcurrency** parameter.
         self.instance_soft_concurrency = instance_soft_concurrency  # type: int
-        # The instance type of the function. Valid values:
-        # 
-        # *   **e1**: elastic instance
-        # *   **c1**: performance instance
-        # *   **fc.gpu.tesla.1**: GPU-accelerated instance (Tesla T4)
-        # *   **fc.gpu.ampere.1**: GPU-accelerated instance (Ampere A10)
-        # *   **g1**: same as **fc.gpu.tesla.1**\
         self.instance_type = instance_type  # type: str
-        # The information about layers.
-        # 
-        # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name as a layer with a larger subscript.
         self.layers = layers  # type: list[str]
-        # The memory size for the function. Unit: MB. The memory size must be a multiple of 64. The memory size varies based on the function instance type. For more information, see [Instance types](~~179379~~).
         self.memory_size = memory_size  # type: int
-        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom** and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
         self.runtime = runtime  # type: str
-        # The timeout period for the execution of the function. Unit: seconds. Default value: 3. Minimum value: 1. When the period ends, the execution of the function is terminated.
         self.timeout = timeout  # type: int
 
     def validate(self):
         if self.code:
             self.code.validate()
         if self.custom_container_config:
             self.custom_container_config.validate()
@@ -13639,77 +13379,40 @@
 class UpdateFunctionResponseBody(TeaModel):
     def __init__(self, ca_port=None, code_checksum=None, code_size=None, cpu=None, created_time=None,
                  custom_container_config=None, custom_dns=None, custom_health_check_config=None, custom_runtime_config=None,
                  description=None, disk_size=None, environment_variables=None, function_id=None, function_name=None,
                  gpu_memory_size=None, handler=None, initialization_timeout=None, initializer=None, instance_concurrency=None,
                  instance_lifecycle_config=None, instance_soft_concurrency=None, instance_type=None, last_modified_time=None, layers=None,
                  memory_size=None, runtime=None, timeout=None):
-        # The port on which the HTTP server listens for the custom runtime or custom container runtime.
         self.ca_port = ca_port  # type: int
-        # The CRC-64 value of the function code package.
         self.code_checksum = code_checksum  # type: str
-        # The size of the function code package that is returned by the system. Unit: bytes.
         self.code_size = code_size  # type: long
-        # The number of vCPUs of the function. The value must be a multiple of 0.05.
         self.cpu = cpu  # type: float
-        # The time when the function was created.
         self.created_time = created_time  # type: str
-        # The configurations of the custom container runtime. After you configure the custom container runtime, Function Compute can execute the function in a container created from a custom image.
         self.custom_container_config = custom_container_config  # type: CustomContainerConfig
-        # The custom DNS configurations of the function.
         self.custom_dns = custom_dns  # type: CustomDNS
-        # The custom health check configuration of the function. This parameter is applicable only to custom runtimes and custom containers.
         self.custom_health_check_config = custom_health_check_config  # type: CustomHealthCheckConfig
-        # The configurations of the custom runtime.
         self.custom_runtime_config = custom_runtime_config  # type: CustomRuntimeConfig
-        # The description of the function.
         self.description = description  # type: str
-        # The disk size of the function. Unit: MB. Valid values: 512 and 10240.
         self.disk_size = disk_size  # type: int
-        # The environment variables that are configured for the function. You can obtain the values of the environment variables from the function. For more information, see [Environment variables](~~69777~~).
         self.environment_variables = environment_variables  # type: dict[str, str]
-        # The unique ID that is generated by the system for the function.
         self.function_id = function_id  # type: str
-        # The name of the function.
         self.function_name = function_name  # type: str
-        # The GPU memory capacity for the function. Unit: MB. The value must be a multiple of 1,024.
         self.gpu_memory_size = gpu_memory_size  # type: int
-        # The handler of the function.
         self.handler = handler  # type: str
-        # The timeout period for the execution of the Initializer hook. Unit: seconds. Default value: 3. Minimum value: 1. When the period ends, the execution of the Initializer hook is terminated.
         self.initialization_timeout = initialization_timeout  # type: int
-        # The handler of the Initializer hook. The format is determined by the programming language.
         self.initializer = initializer  # type: str
-        # The number of requests that can be concurrently processed by a single instance.
         self.instance_concurrency = instance_concurrency  # type: int
-        # The lifecycle configurations of the instance.
         self.instance_lifecycle_config = instance_lifecycle_config  # type: InstanceLifecycleConfig
-        # The soft concurrency of the instance. You can use this parameter to implement graceful scale-up of instances. If the number of concurrent requests on an instance is greater than the value of soft concurrency, an instance scale-up is triggered. For example, if your instance requires a long time to start, you can specify a suitable soft concurrency to start the instance in advance.
-        # 
-        # The value must be less than or equal to that of the **instanceConcurrency** parameter.
         self.instance_soft_concurrency = instance_soft_concurrency  # type: int
-        # The instance type of the function. Valid values:
-        # 
-        # *   **e1**: elastic instance
-        # *   **c1**: performance instance
-        # *   **fc.gpu.tesla.1**: GPU-accelerated instance (Tesla T4)
-        # *   **fc.gpu.ampere.1**: GPU-accelerated instance (Ampere A10)
-        # *   **g1**: same as **fc.gpu.tesla.1**\
         self.instance_type = instance_type  # type: str
-        # The time when the function was last modified.
         self.last_modified_time = last_modified_time  # type: str
-        # An array that consists of the information of layers.
-        # 
-        # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name as a layer with a larger subscript.
         self.layers = layers  # type: list[str]
-        # The memory size that is configured for the function. Unit: MB.
         self.memory_size = memory_size  # type: int
-        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom** and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
         self.runtime = runtime  # type: str
-        # The timeout period for the execution. Unit: seconds.
         self.timeout = timeout  # type: int
 
     def validate(self):
         if self.custom_container_config:
             self.custom_container_config.validate()
         if self.custom_dns:
             self.custom_dns.validate()
@@ -14172,21 +13875,21 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateTriggerHeaders(TeaModel):
     def __init__(self, common_headers=None, if_match=None, x_fc_account_id=None, x_fc_date=None, x_fc_trace_id=None):
         self.common_headers = common_headers  # type: dict[str, str]
-        # This parameter is used to ensure that the modified resource is consistent with the resource to be modified. You can obtain the parameter value from the responses of [CreateTrigger](~~190054~~), [GetTrigger](~~190056~~), and [UpdateTrigger](~~190055~~) operations.
+        # The name of the service.
         self.if_match = if_match  # type: str
-        # The ID of your Alibaba Cloud account.
-        self.x_fc_account_id = x_fc_account_id  # type: str
         # The time when the request is initiated on the client. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
-        self.x_fc_date = x_fc_date  # type: str
+        self.x_fc_account_id = x_fc_account_id  # type: str
         # The custom request ID.
+        self.x_fc_date = x_fc_date  # type: str
+        # The ETag that is used to modify the trigger. This parameter is used to ensure that the modified trigger is consistent with the trigger to be modified.
         self.x_fc_trace_id = x_fc_trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateTriggerHeaders, self).to_map()
@@ -14219,29 +13922,29 @@
         if m.get('X-Fc-Trace-Id') is not None:
             self.x_fc_trace_id = m.get('X-Fc-Trace-Id')
         return self
 
 
 class UpdateTriggerRequest(TeaModel):
     def __init__(self, description=None, invocation_role=None, qualifier=None, trigger_config=None):
-        # The description of the trigger.
+        # The ID of your Alibaba Cloud account.
         self.description = description  # type: str
-        # The role that is used by the event source such as OSS to invoke the function. For more information, see [Overview](~~53102~~).
-        self.invocation_role = invocation_role  # type: str
         # The version or alias of the service.
-        self.qualifier = qualifier  # type: str
+        self.invocation_role = invocation_role  # type: str
         # The configurations of the trigger. The configurations vary based on the trigger type. For more information about the format, see the following topics:
         # 
         # *   OSS trigger: [OSSTriggerConfig](~~struct:OSSTriggerConfig~~).
         # *   Log Service trigger: [LogTriggerConfig](~~struct:LogTriggerConfig~~).
         # *   Time trigger: [TimeTriggerConfig](~~struct:TimeTriggerConfig~~).
         # *   HTTP trigger: [HTTPTriggerConfig](~~struct:HTTPTriggerConfig~~).
         # *   Tablestore trigger: Specify the **SourceArn** parameter and leave this parameter empty.
         # *   Alibaba Cloud CDN event trigger: [CDNEventsTriggerConfig](~~struct:CDNEventsTriggerConfig~~).
         # *   MNS topic trigger: [MnsTopicTriggerConfig](~~struct:MnsTopicTriggerConfig~~).
+        self.qualifier = qualifier  # type: str
+        # The description of the trigger.
         self.trigger_config = trigger_config  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateTriggerRequest, self).to_map()
@@ -14272,39 +13975,38 @@
         return self
 
 
 class UpdateTriggerResponseBody(TeaModel):
     def __init__(self, created_time=None, description=None, domain_name=None, invocation_role=None,
                  last_modified_time=None, qualifier=None, source_arn=None, trigger_config=None, trigger_id=None, trigger_name=None,
                  trigger_type=None, url_internet=None, url_intranet=None):
-        # The time when the audio or video file was created.
+        # The ARN of the RAM role that is used by the event source to invoke the function.
         self.created_time = created_time  # type: str
-        # The description of the trigger.
+        # The unique ID of the trigger.
         self.description = description  # type: str
-        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
+        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
         self.domain_name = domain_name  # type: str
-        # The ARN of the RAM role that is used by the event source to invoke the function.
-        self.invocation_role = invocation_role  # type: str
         # The last modification time.
-        self.last_modified_time = last_modified_time  # type: str
+        self.invocation_role = invocation_role  # type: str
         # The version or alias of the service.
-        self.qualifier = qualifier  # type: str
+        self.last_modified_time = last_modified_time  # type: str
         # The ARN of the event source.
-        self.source_arn = source_arn  # type: str
+        self.qualifier = qualifier  # type: str
         # The configurations of the trigger. The configurations vary based on the trigger type.
+        self.source_arn = source_arn  # type: str
+        # The name of the trigger.
         self.trigger_config = trigger_config  # type: str
-        # The unique ID of the trigger.
+        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
         self.trigger_id = trigger_id  # type: str
-        # The name of the trigger.
-        self.trigger_name = trigger_name  # type: str
         # The trigger type, such as **oss**, **log**, **tablestore**, **timer**, **http**, **cdn_events**, and **mns_topic**.
+        self.trigger_name = trigger_name  # type: str
+        # The description of the trigger.
         self.trigger_type = trigger_type  # type: str
-        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
-        self.url_internet = url_internet  # type: str
         # The private endpoint. In a VPC, you can access HTTP triggers by using HTTP or HTTPS.
+        self.url_internet = url_internet  # type: str
         self.url_intranet = url_intranet  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateTriggerResponseBody, self).to_map()
```

### Comparing `alibabacloud_fc-open20210406_py2-2.0.8/alibabacloud_fc_open20210406_py2.egg-info/PKG-INFO` & `alibabacloud_fc-open20210406_py2-2.0.9/alibabacloud_fc_open20210406_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-fc-open20210406-py2
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud FC-Open (20210406) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc-open20210406_py2-2.0.8/setup.py` & `alibabacloud_fc-open20210406_py2-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_fc-open20210406_py2.
 
-Created on 11/04/2023
+Created on 30/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_fc_open20210406"
 NAME = "alibabacloud_fc-open20210406_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud FC-Open (20210406) SDK Library for Python2"
```

