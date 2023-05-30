# Comparing `tmp/alibabacloud_fc-open20210406-2.0.8.tar.gz` & `tmp/alibabacloud_fc-open20210406-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_fc-open20210406-2.0.8.tar", last modified: Tue Apr 11 06:50:21 2023, max compression
+gzip compressed data, was "dist/alibabacloud_fc-open20210406-2.0.9.tar", last modified: Tue May 30 06:48:08 2023, max compression
```

## Comparing `alibabacloud_fc-open20210406-2.0.8.tar` & `alibabacloud_fc-open20210406-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/
--rw-r--r--   0 root         (0) root         (0)     2205 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2352 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1034 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406/__init__.py
--rw-r--r--   0 root         (0) root         (0)   352899 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406/client.py
--rw-r--r--   0 root         (0) root         (0)   600025 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2352 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      262 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2762 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/
+-rw-r--r--   0 root         (0) root         (0)     2276 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/alibabacloud_fc_open20210406/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/alibabacloud_fc_open20210406/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   346309 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/alibabacloud_fc_open20210406/client.py
+-rw-r--r--   0 root         (0) root         (0)   591891 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/alibabacloud_fc_open20210406/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/alibabacloud_fc_open20210406.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/alibabacloud_fc_open20210406.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/alibabacloud_fc_open20210406.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/alibabacloud_fc_open20210406.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/alibabacloud_fc_open20210406.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/alibabacloud_fc_open20210406.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-05-30 06:48:08.000000 alibabacloud_fc-open20210406-2.0.9/setup.py
```

### Comparing `alibabacloud_fc-open20210406-2.0.8/ChangeLog.md` & `alibabacloud_fc-open20210406-2.0.9/ChangeLog.md`

 * *Files 10% similar despite different names*

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

### Comparing `alibabacloud_fc-open20210406-2.0.8/LICENSE` & `alibabacloud_fc-open20210406-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc-open20210406-2.0.8/PKG-INFO` & `alibabacloud_fc-open20210406-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_fc-open20210406
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud FC-Open (20210406) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc-open20210406-2.0.8/README-CN.md` & `alibabacloud_fc-open20210406-2.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc-open20210406-2.0.8/README.md` & `alibabacloud_fc-open20210406-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406/client.py` & `alibabacloud_fc-open20210406-2.0.9/alibabacloud_fc_open20210406/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2470,22 +2470,14 @@
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.GetFunctionAsyncInvokeConfigRequest,
         headers: fc__open_20210406_models.GetFunctionAsyncInvokeConfigHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.GetFunctionAsyncInvokeConfigResponse:
-        """
-        StatefulAsyncInvocation indicates whether the asynchronous task feature is enabled. If the value of StatefulAsyncInvocation is true, the asynchronous task feature is enabled. All asynchronous invocations change to asynchronous task mode.
-        
-        @param request: GetFunctionAsyncInvokeConfigRequest
-        @param headers: GetFunctionAsyncInvokeConfigHeaders
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: GetFunctionAsyncInvokeConfigResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.qualifier):
             query['qualifier'] = request.qualifier
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -2519,22 +2511,14 @@
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.GetFunctionAsyncInvokeConfigRequest,
         headers: fc__open_20210406_models.GetFunctionAsyncInvokeConfigHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.GetFunctionAsyncInvokeConfigResponse:
-        """
-        StatefulAsyncInvocation indicates whether the asynchronous task feature is enabled. If the value of StatefulAsyncInvocation is true, the asynchronous task feature is enabled. All asynchronous invocations change to asynchronous task mode.
-        
-        @param request: GetFunctionAsyncInvokeConfigRequest
-        @param headers: GetFunctionAsyncInvokeConfigHeaders
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: GetFunctionAsyncInvokeConfigResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.qualifier):
             query['qualifier'] = request.qualifier
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -2566,36 +2550,24 @@
 
     def get_function_async_invoke_config(
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.GetFunctionAsyncInvokeConfigRequest,
     ) -> fc__open_20210406_models.GetFunctionAsyncInvokeConfigResponse:
-        """
-        StatefulAsyncInvocation indicates whether the asynchronous task feature is enabled. If the value of StatefulAsyncInvocation is true, the asynchronous task feature is enabled. All asynchronous invocations change to asynchronous task mode.
-        
-        @param request: GetFunctionAsyncInvokeConfigRequest
-        @return: GetFunctionAsyncInvokeConfigResponse
-        """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.GetFunctionAsyncInvokeConfigHeaders()
         return self.get_function_async_invoke_config_with_options(service_name, function_name, request, headers, runtime)
 
     async def get_function_async_invoke_config_async(
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.GetFunctionAsyncInvokeConfigRequest,
     ) -> fc__open_20210406_models.GetFunctionAsyncInvokeConfigResponse:
-        """
-        StatefulAsyncInvocation indicates whether the asynchronous task feature is enabled. If the value of StatefulAsyncInvocation is true, the asynchronous task feature is enabled. All asynchronous invocations change to asynchronous task mode.
-        
-        @param request: GetFunctionAsyncInvokeConfigRequest
-        @return: GetFunctionAsyncInvokeConfigResponse
-        """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.GetFunctionAsyncInvokeConfigHeaders()
         return await self.get_function_async_invoke_config_with_options_async(service_name, function_name, request, headers, runtime)
 
     def get_function_code_with_options(
         self,
         service_name: str,
@@ -3188,15 +3160,15 @@
         function_name: str,
         invocation_id: str,
         request: fc__open_20210406_models.GetStatefulAsyncInvocationRequest,
         headers: fc__open_20210406_models.GetStatefulAsyncInvocationHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.GetStatefulAsyncInvocationResponse:
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The version or alias of the service to which the asynchronous task belongs.
         
         @param request: GetStatefulAsyncInvocationRequest
         @param headers: GetStatefulAsyncInvocationHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetStatefulAsyncInvocationResponse
         """
         UtilClient.validate_model(request)
@@ -3244,15 +3216,15 @@
         function_name: str,
         invocation_id: str,
         request: fc__open_20210406_models.GetStatefulAsyncInvocationRequest,
         headers: fc__open_20210406_models.GetStatefulAsyncInvocationHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.GetStatefulAsyncInvocationResponse:
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The version or alias of the service to which the asynchronous task belongs.
         
         @param request: GetStatefulAsyncInvocationRequest
         @param headers: GetStatefulAsyncInvocationHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetStatefulAsyncInvocationResponse
         """
         UtilClient.validate_model(request)
@@ -3298,15 +3270,15 @@
         self,
         service_name: str,
         function_name: str,
         invocation_id: str,
         request: fc__open_20210406_models.GetStatefulAsyncInvocationRequest,
     ) -> fc__open_20210406_models.GetStatefulAsyncInvocationResponse:
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The version or alias of the service to which the asynchronous task belongs.
         
         @param request: GetStatefulAsyncInvocationRequest
         @return: GetStatefulAsyncInvocationResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.GetStatefulAsyncInvocationHeaders()
         return self.get_stateful_async_invocation_with_options(service_name, function_name, invocation_id, request, headers, runtime)
@@ -3315,15 +3287,15 @@
         self,
         service_name: str,
         function_name: str,
         invocation_id: str,
         request: fc__open_20210406_models.GetStatefulAsyncInvocationRequest,
     ) -> fc__open_20210406_models.GetStatefulAsyncInvocationResponse:
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The version or alias of the service to which the asynchronous task belongs.
         
         @param request: GetStatefulAsyncInvocationRequest
         @return: GetStatefulAsyncInvocationResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.GetStatefulAsyncInvocationHeaders()
         return await self.get_stateful_async_invocation_with_options_async(service_name, function_name, invocation_id, request, headers, runtime)
@@ -3442,14 +3414,16 @@
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
@@ -3493,14 +3467,16 @@
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
@@ -3864,22 +3840,14 @@
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.ListFunctionAsyncInvokeConfigsRequest,
         headers: fc__open_20210406_models.ListFunctionAsyncInvokeConfigsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.ListFunctionAsyncInvokeConfigsResponse:
-        """
-        StatefulAsyncInvocation indicates whether the asynchronous task feature is enabled. If StatefulAsyncInvocation is set to true, the asynchronous task is enabled. All asynchronous invocations to the function corresponding to this configuration change to asynchronous task mode.
-        
-        @param request: ListFunctionAsyncInvokeConfigsRequest
-        @param headers: ListFunctionAsyncInvokeConfigsHeaders
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ListFunctionAsyncInvokeConfigsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.limit):
             query['limit'] = request.limit
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
         real_headers = {}
@@ -3921,22 +3889,14 @@
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.ListFunctionAsyncInvokeConfigsRequest,
         headers: fc__open_20210406_models.ListFunctionAsyncInvokeConfigsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.ListFunctionAsyncInvokeConfigsResponse:
-        """
-        StatefulAsyncInvocation indicates whether the asynchronous task feature is enabled. If StatefulAsyncInvocation is set to true, the asynchronous task is enabled. All asynchronous invocations to the function corresponding to this configuration change to asynchronous task mode.
-        
-        @param request: ListFunctionAsyncInvokeConfigsRequest
-        @param headers: ListFunctionAsyncInvokeConfigsHeaders
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: ListFunctionAsyncInvokeConfigsResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.limit):
             query['limit'] = request.limit
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
         real_headers = {}
@@ -3976,36 +3936,24 @@
 
     def list_function_async_invoke_configs(
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.ListFunctionAsyncInvokeConfigsRequest,
     ) -> fc__open_20210406_models.ListFunctionAsyncInvokeConfigsResponse:
-        """
-        StatefulAsyncInvocation indicates whether the asynchronous task feature is enabled. If StatefulAsyncInvocation is set to true, the asynchronous task is enabled. All asynchronous invocations to the function corresponding to this configuration change to asynchronous task mode.
-        
-        @param request: ListFunctionAsyncInvokeConfigsRequest
-        @return: ListFunctionAsyncInvokeConfigsResponse
-        """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.ListFunctionAsyncInvokeConfigsHeaders()
         return self.list_function_async_invoke_configs_with_options(service_name, function_name, request, headers, runtime)
 
     async def list_function_async_invoke_configs_async(
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.ListFunctionAsyncInvokeConfigsRequest,
     ) -> fc__open_20210406_models.ListFunctionAsyncInvokeConfigsResponse:
-        """
-        StatefulAsyncInvocation indicates whether the asynchronous task feature is enabled. If StatefulAsyncInvocation is set to true, the asynchronous task is enabled. All asynchronous invocations to the function corresponding to this configuration change to asynchronous task mode.
-        
-        @param request: ListFunctionAsyncInvokeConfigsRequest
-        @return: ListFunctionAsyncInvokeConfigsResponse
-        """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.ListFunctionAsyncInvokeConfigsHeaders()
         return await self.list_function_async_invoke_configs_with_options_async(service_name, function_name, request, headers, runtime)
 
     def list_functions_with_options(
         self,
         service_name: str,
@@ -4125,16 +4073,16 @@
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.ListInstancesRequest,
         headers: fc__open_20210406_models.ListInstancesHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.ListInstancesResponse:
         """
-        The ListInstances operation allows you to query the available instances of a function.
-        Available instances are instances that are processing requests or can be scheduled to process requests. Available instances queried by the ListInstances operation are the same as those that can be used when you call the InvokeFunction operation with the same values specified for the `serviceName`, `functionName`, and `qualifier` parameters.
+        The maximum number of resources to return. Valid values: \\[0,1000].
+        The number of returned resources is less than or equal to the specified number.
         
         @param request: ListInstancesRequest
         @param headers: ListInstancesHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListInstancesResponse
         """
         UtilClient.validate_model(request)
@@ -4175,16 +4123,16 @@
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.ListInstancesRequest,
         headers: fc__open_20210406_models.ListInstancesHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.ListInstancesResponse:
         """
-        The ListInstances operation allows you to query the available instances of a function.
-        Available instances are instances that are processing requests or can be scheduled to process requests. Available instances queried by the ListInstances operation are the same as those that can be used when you call the InvokeFunction operation with the same values specified for the `serviceName`, `functionName`, and `qualifier` parameters.
+        The maximum number of resources to return. Valid values: \\[0,1000].
+        The number of returned resources is less than or equal to the specified number.
         
         @param request: ListInstancesRequest
         @param headers: ListInstancesHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListInstancesResponse
         """
         UtilClient.validate_model(request)
@@ -4223,16 +4171,16 @@
     def list_instances(
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.ListInstancesRequest,
     ) -> fc__open_20210406_models.ListInstancesResponse:
         """
-        The ListInstances operation allows you to query the available instances of a function.
-        Available instances are instances that are processing requests or can be scheduled to process requests. Available instances queried by the ListInstances operation are the same as those that can be used when you call the InvokeFunction operation with the same values specified for the `serviceName`, `functionName`, and `qualifier` parameters.
+        The maximum number of resources to return. Valid values: \\[0,1000].
+        The number of returned resources is less than or equal to the specified number.
         
         @param request: ListInstancesRequest
         @return: ListInstancesResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.ListInstancesHeaders()
         return self.list_instances_with_options(service_name, function_name, request, headers, runtime)
@@ -4240,16 +4188,16 @@
     async def list_instances_async(
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.ListInstancesRequest,
     ) -> fc__open_20210406_models.ListInstancesResponse:
         """
-        The ListInstances operation allows you to query the available instances of a function.
-        Available instances are instances that are processing requests or can be scheduled to process requests. Available instances queried by the ListInstances operation are the same as those that can be used when you call the InvokeFunction operation with the same values specified for the `serviceName`, `functionName`, and `qualifier` parameters.
+        The maximum number of resources to return. Valid values: \\[0,1000].
+        The number of returned resources is less than or equal to the specified number.
         
         @param request: ListInstancesRequest
         @return: ListInstancesResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.ListInstancesHeaders()
         return await self.list_instances_with_options_async(service_name, function_name, request, headers, runtime)
@@ -4999,15 +4947,15 @@
     def list_stateful_async_invocation_functions_with_options(
         self,
         request: fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsRequest,
         headers: fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsResponse:
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The metadata of the service and function to which the asynchronous task belongs.
         
         @param request: ListStatefulAsyncInvocationFunctionsRequest
         @param headers: ListStatefulAsyncInvocationFunctionsHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListStatefulAsyncInvocationFunctionsResponse
         """
         UtilClient.validate_model(request)
@@ -5048,15 +4996,15 @@
     async def list_stateful_async_invocation_functions_with_options_async(
         self,
         request: fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsRequest,
         headers: fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsResponse:
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The metadata of the service and function to which the asynchronous task belongs.
         
         @param request: ListStatefulAsyncInvocationFunctionsRequest
         @param headers: ListStatefulAsyncInvocationFunctionsHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListStatefulAsyncInvocationFunctionsResponse
         """
         UtilClient.validate_model(request)
@@ -5095,29 +5043,29 @@
         )
 
     def list_stateful_async_invocation_functions(
         self,
         request: fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsRequest,
     ) -> fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsResponse:
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The metadata of the service and function to which the asynchronous task belongs.
         
         @param request: ListStatefulAsyncInvocationFunctionsRequest
         @return: ListStatefulAsyncInvocationFunctionsResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsHeaders()
         return self.list_stateful_async_invocation_functions_with_options(request, headers, runtime)
 
     async def list_stateful_async_invocation_functions_async(
         self,
         request: fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsRequest,
     ) -> fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsResponse:
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The metadata of the service and function to which the asynchronous task belongs.
         
         @param request: ListStatefulAsyncInvocationFunctionsRequest
         @return: ListStatefulAsyncInvocationFunctionsResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.ListStatefulAsyncInvocationFunctionsHeaders()
         return await self.list_stateful_async_invocation_functions_with_options_async(request, headers, runtime)
@@ -5127,15 +5075,15 @@
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.ListStatefulAsyncInvocationsRequest,
         headers: fc__open_20210406_models.ListStatefulAsyncInvocationsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.ListStatefulAsyncInvocationsResponse:
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The name of the service to which the asynchronous task belongs.
         
         @param request: ListStatefulAsyncInvocationsRequest
         @param headers: ListStatefulAsyncInvocationsHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListStatefulAsyncInvocationsResponse
         """
         UtilClient.validate_model(request)
@@ -5198,15 +5146,15 @@
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.ListStatefulAsyncInvocationsRequest,
         headers: fc__open_20210406_models.ListStatefulAsyncInvocationsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.ListStatefulAsyncInvocationsResponse:
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The name of the service to which the asynchronous task belongs.
         
         @param request: ListStatefulAsyncInvocationsRequest
         @param headers: ListStatefulAsyncInvocationsHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListStatefulAsyncInvocationsResponse
         """
         UtilClient.validate_model(request)
@@ -5267,15 +5215,15 @@
     def list_stateful_async_invocations(
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.ListStatefulAsyncInvocationsRequest,
     ) -> fc__open_20210406_models.ListStatefulAsyncInvocationsResponse:
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The name of the service to which the asynchronous task belongs.
         
         @param request: ListStatefulAsyncInvocationsRequest
         @return: ListStatefulAsyncInvocationsResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.ListStatefulAsyncInvocationsHeaders()
         return self.list_stateful_async_invocations_with_options(service_name, function_name, request, headers, runtime)
@@ -5283,15 +5231,15 @@
     async def list_stateful_async_invocations_async(
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.ListStatefulAsyncInvocationsRequest,
     ) -> fc__open_20210406_models.ListStatefulAsyncInvocationsResponse:
         """
-        StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The name of the service to which the asynchronous task belongs.
         
         @param request: ListStatefulAsyncInvocationsRequest
         @return: ListStatefulAsyncInvocationsResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.ListStatefulAsyncInvocationsHeaders()
         return await self.list_stateful_async_invocations_with_options_async(service_name, function_name, request, headers, runtime)
@@ -5699,15 +5647,15 @@
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.PutFunctionAsyncInvokeConfigRequest,
         headers: fc__open_20210406_models.PutFunctionAsyncInvokeConfigHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.PutFunctionAsyncInvokeConfigResponse:
         """
-        StatefulAsyncInvocation specifies the configurations of the asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The maximum validity period of messages.
         
         @param request: PutFunctionAsyncInvokeConfigRequest
         @param headers: PutFunctionAsyncInvokeConfigHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: PutFunctionAsyncInvokeConfigResponse
         """
         UtilClient.validate_model(request)
@@ -5758,15 +5706,15 @@
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.PutFunctionAsyncInvokeConfigRequest,
         headers: fc__open_20210406_models.PutFunctionAsyncInvokeConfigHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> fc__open_20210406_models.PutFunctionAsyncInvokeConfigResponse:
         """
-        StatefulAsyncInvocation specifies the configurations of the asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The maximum validity period of messages.
         
         @param request: PutFunctionAsyncInvokeConfigRequest
         @param headers: PutFunctionAsyncInvokeConfigHeaders
         @param runtime: runtime options for this request RuntimeOptions
         @return: PutFunctionAsyncInvokeConfigResponse
         """
         UtilClient.validate_model(request)
@@ -5815,15 +5763,15 @@
     def put_function_async_invoke_config(
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.PutFunctionAsyncInvokeConfigRequest,
     ) -> fc__open_20210406_models.PutFunctionAsyncInvokeConfigResponse:
         """
-        StatefulAsyncInvocation specifies the configurations of the asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The maximum validity period of messages.
         
         @param request: PutFunctionAsyncInvokeConfigRequest
         @return: PutFunctionAsyncInvokeConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.PutFunctionAsyncInvokeConfigHeaders()
         return self.put_function_async_invoke_config_with_options(service_name, function_name, request, headers, runtime)
@@ -5831,15 +5779,15 @@
     async def put_function_async_invoke_config_async(
         self,
         service_name: str,
         function_name: str,
         request: fc__open_20210406_models.PutFunctionAsyncInvokeConfigRequest,
     ) -> fc__open_20210406_models.PutFunctionAsyncInvokeConfigResponse:
         """
-        StatefulAsyncInvocation specifies the configurations of the asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
+        The maximum validity period of messages.
         
         @param request: PutFunctionAsyncInvokeConfigRequest
         @return: PutFunctionAsyncInvokeConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = fc__open_20210406_models.PutFunctionAsyncInvokeConfigHeaders()
         return await self.put_function_async_invoke_config_with_options_async(service_name, function_name, request, headers, runtime)
```

### Comparing `alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406/models.py` & `alibabacloud_fc-open20210406-2.0.9/alibabacloud_fc_open20210406/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -3294,20 +3294,20 @@
         additional_version_weight: Dict[str, float] = None,
         alias_name: str = None,
         description: str = None,
         resolve_policy: str = None,
         route_policy: RoutePolicy = None,
         version_id: str = None,
     ):
-        # The canary release version to which the alias points and the weight of the canary release version.
+        # The additional version to which the alias points and the weight of the additional version.
         # 
-        # *   The canary release version takes effect only when the function is invoked.
+        # *   The additional version takes effect only when the function is invoked.
         # *   The value consists of a version number and a specific weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
         self.additional_version_weight = additional_version_weight
-        # The name of the alias.  The name contains only letters, digits, hyphens (-), and underscores (\_). The name must be 1 to 128 characters in length and cannot start with a digit or hyphen (-).  The name cannot be **LATEST**.
+        # The name of the alias. The name can contain letters, digits, underscores (\_), and hyphens (-) only. The name cannot start with a digit or a hyphen (-). The name must be 1 to 128 characters in length. The name cannot be set to **LATEST**\
         self.alias_name = alias_name
         # The description of the alias.
         self.description = description
         # The canary release mode. Valid values:
         # 
         # *   **Random**: random canary release. This is the default value.
         # *   **Content**: rule-based canary release.
@@ -3365,17 +3365,17 @@
         additional_version_weight: Dict[str, float] = None,
         alias_name: str = None,
         created_time: str = None,
         description: str = None,
         last_modified_time: str = None,
         version_id: str = None,
     ):
-        # The canary release version to which the alias points and the weight of the canary release version.
+        # The additional version to which the alias points and the weight of the additional version.
         # 
-        # *   The canary release version takes effect only when the function is invoked.
+        # *   The additional version takes effect only when the function is invoked.
         # *   The value consists of a version number and a specific weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
         self.additional_version_weight = additional_version_weight
         # The name of the alias.
         self.alias_name = alias_name
         # The time when the alias was created.
         self.created_time = created_time
         # The description of the alias.
@@ -3751,21 +3751,17 @@
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_code_checksum: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The CRC-64 value of the function code package.
         self.x_fc_code_checksum = x_fc_code_checksum
-        # The time on which the function is invoked. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date
-        # The trace ID of the request. The value is the same as that of the requestId parameter in the response.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3823,69 +3819,36 @@
         instance_soft_concurrency: int = None,
         instance_type: str = None,
         layers: List[str] = None,
         memory_size: int = None,
         runtime: str = None,
         timeout: int = None,
     ):
-        # The port on which the HTTP server listens for the custom runtime or custom container runtime.
         self.ca_port = ca_port
-        # The code of the function. The code must be packaged into a ZIP file. Choose **code** or **customContainerConfig** for the function.
         self.code = code
-        # The number of vCPUs of the function. The value must be a multiple of 0.05.
         self.cpu = cpu
-        # The configurations of the custom container runtime. After you configure the custom container runtime, Function Compute can execute the function in a container created from a custom image. Choose **code** or **customContainerConfig** for the function.
         self.custom_container_config = custom_container_config
-        # The custom Domain Name System (DNS) configurations of the function.
         self.custom_dns = custom_dns
-        # The custom health check configurations of the function. This parameter is applicable to only custom runtimes and custom containers.
         self.custom_health_check_config = custom_health_check_config
-        # The configurations of the custom runtime.
         self.custom_runtime_config = custom_runtime_config
-        # The description of the function.
         self.description = description
-        # The disk size of the function. Unit: MB. Valid values: 512 and 10240.
         self.disk_size = disk_size
-        # The environment variables that you configured for the function. You can obtain the values of the environment variables from the function. For more information, see [Overview](~~69777~~).
         self.environment_variables = environment_variables
-        # The name of the function. The name can contain letters, digits, underscores (\_), and hyphens (-) only. The name cannot start with a digit or a hyphen (-). The name must be 1 to 64 characters in length.
         self.function_name = function_name
-        # The GPU memory capacity for the function. Unit: MB. The value must be a multiple of 1,024.
         self.gpu_memory_size = gpu_memory_size
-        # The handler of the function. The format varies based on the programming language. For more information, see [Function handlers](~~157704~~).
         self.handler = handler
-        # The timeout period for the execution of the Initializer hook. Unit: seconds. Default value: 3. Valid values: 1 to 300. When this period expires, the execution of the Initializer hook is terminated.
         self.initialization_timeout = initialization_timeout
-        # The handler of the Initializer hook. For more information, see [Initializer hooks](~~157704~~).
         self.initializer = initializer
-        # The number of requests that can be concurrently processed by a single instance.
         self.instance_concurrency = instance_concurrency
-        # The lifecycle configurations of the instance.
         self.instance_lifecycle_config = instance_lifecycle_config
-        # The soft concurrency of the instance. You can use this parameter to implement graceful scale-up of instances. If the number of concurrent requests on an instance is greater than the value of soft concurrency, an instance scale-up is triggered. For example, if your instance requires a long time to start, you can specify a suitable soft concurrency to start the instance in advance.
-        # 
-        # The value must be less than or equal to that of the **instanceConcurrency** parameter.
         self.instance_soft_concurrency = instance_soft_concurrency
-        # The instance type of the function. Valid values:
-        # 
-        # *   **e1**: elastic instance
-        # *   **c1**: performance instance
-        # *   **fc.gpu.tesla.1**: GPU-accelerated instance (Tesla T4)
-        # *   **fc.gpu.ampere.1**: GPU-accelerated instance (Ampere A10)
-        # *   **g1**: same as **fc.gpu.tesla.1**\
         self.instance_type = instance_type
-        # The information about layers.
-        # 
-        # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name as a layer with a larger subscript.
         self.layers = layers
-        # The memory size for the function. Unit: MB. The value must be a multiple of 64. The memory size varies based on the function instance type. For more information, see [Instance types](~~179379~~).
         self.memory_size = memory_size
-        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom** and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
         self.runtime = runtime
-        # The timeout period for the execution of the function. Unit: seconds. Default value: 3. Minimum value: 1. When the period ends, the execution of the function is terminated.
         self.timeout = timeout
 
     def validate(self):
         if self.code:
             self.code.validate()
         if self.custom_container_config:
             self.custom_container_config.validate()
@@ -4036,77 +3999,40 @@
         instance_type: str = None,
         last_modified_time: str = None,
         layers: List[str] = None,
         memory_size: int = None,
         runtime: str = None,
         timeout: int = None,
     ):
-        # The port on which the HTTP server listens for the custom runtime or custom container runtime.
         self.ca_port = ca_port
-        # The CRC-64 value of the function code package.
         self.code_checksum = code_checksum
-        # The size of the function code package that is returned by the system. Unit: bytes.
         self.code_size = code_size
-        # The number of vCPUs of the function. The value is a multiple of 0.05.
         self.cpu = cpu
-        # The time when the function was created.
         self.created_time = created_time
-        # The configurations of the custom container runtime. After you configure the custom container runtime, Function Compute can execute the function in a container created from a custom image.
         self.custom_container_config = custom_container_config
-        # The custom DNS configurations of the function.
         self.custom_dns = custom_dns
-        # The custom health check configuration of the function. This parameter is applicable only to custom runtimes and custom containers.
         self.custom_health_check_config = custom_health_check_config
-        # The configurations of the custom runtime.
         self.custom_runtime_config = custom_runtime_config
-        # The description of the function.
         self.description = description
-        # The disk size of the function. Unit: MB. Valid values: 512 and 10240.
         self.disk_size = disk_size
-        # The environment variables that are configured for the function. You can obtain the values of the environment variables from the function. For more information, see [Environment variables](~~69777~~).
         self.environment_variables = environment_variables
-        # The unique ID that is generated by the system for the function.
         self.function_id = function_id
-        # The name of the function.
         self.function_name = function_name
-        # The GPU memory capacity for the function. Unit: MB. The value is a multiple of 1,024.
         self.gpu_memory_size = gpu_memory_size
-        # The handler of the function.
         self.handler = handler
-        # The timeout period for the execution of the Initializer hook. Unit: seconds. Default value: 3. Minimum value: 1. When the period ends, the execution of the Initializer hook is terminated.
         self.initialization_timeout = initialization_timeout
-        # The handler of the Initializer hook. The format is determined by the programming language.
         self.initializer = initializer
-        # The number of requests that can be concurrently processed by a single instance.
         self.instance_concurrency = instance_concurrency
-        # The lifecycle configurations of the instance.
         self.instance_lifecycle_config = instance_lifecycle_config
-        # The soft concurrency of the instance. You can use this parameter to implement graceful scale-up of instances. If the number of concurrent requests on an instance is greater than the value of soft concurrency, an instance scale-up is triggered. For example, if your instance requires a long time to start, you can specify a suitable soft concurrency to start the instance in advance.
-        # 
-        # The value must be less than or equal to that of the **instanceConcurrency** parameter.
         self.instance_soft_concurrency = instance_soft_concurrency
-        # The instance type of the function. Valid values:
-        # 
-        # *   **e1**: elastic instance
-        # *   **c1**: performance instance
-        # *   **fc.gpu.tesla.1**: GPU-accelerated instance (Tesla T4)
-        # *   **fc.gpu.ampere.1**: GPU-accelerated instance (Ampere A10)
-        # *   **g1**: same as **fc.gpu.tesla.1**\
         self.instance_type = instance_type
-        # The time when the function was last modified.
         self.last_modified_time = last_modified_time
-        # An array that consists of the information of layers.
-        # 
-        # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name as a layer with a larger subscript.
         self.layers = layers
-        # The memory size that is configured for the function. Unit: MB.
         self.memory_size = memory_size
-        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom** and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
         self.runtime = runtime
-        # The timeout period for the execution of the function. Unit: seconds. Default value: 60. Valid values: 1 to 600. When this period expires, the execution of the function is terminated.
         self.timeout = timeout
 
     def validate(self):
         if self.custom_container_config:
             self.custom_container_config.validate()
         if self.custom_dns:
             self.custom_dns.validate()
@@ -4292,19 +4218,19 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # The description of the layer.
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The checksum of the layer code package.
         self.x_fc_date = x_fc_date
-        # The trace ID of the invocation request of Function Compute.
+        # The information about the layer code package.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4338,19 +4264,19 @@
 class CreateLayerVersionRequest(TeaModel):
     def __init__(
         self,
         code: Code = None,
         compatible_runtime: List[str] = None,
         description: str = None,
     ):
-        # The code of the layer.
+        # The name of the layer.
         self.code = code
-        # The list of runtime environments that are supported by the layer.
+        # The name of the runtime. Valid values: **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **php7.2**, **go1**, **dotnetcore2.1** and **custom**.
         self.compatible_runtime = compatible_runtime
-        # The description of the layer.
+        # The name of the layer.
         self.description = description
 
     def validate(self):
         if self.code:
             self.code.validate()
 
     def to_map(self):
@@ -4389,33 +4315,32 @@
         codesize: int = None,
         compatible_runtime: List[str] = None,
         create_time: str = None,
         description: str = None,
         layer_name: str = None,
         version: int = None,
     ):
-        # The access mode of the layer.
+        # Creates a layer version.
         self.acl = acl
-        # The name of the layer.
         self.arn = arn
-        # The information about the layer code package.
+        # The access mode of the layer.
         self.code = code
-        # The checksum of the layer code package.
+        # Example 1
         self.code_checksum = code_checksum
         # The size of the layer code package. Unit: Byte.
         self.codesize = codesize
-        # The list of runtime environments that are supported by the layer.
+        # Luoni
         self.compatible_runtime = compatible_runtime
-        # The time when the layer version was created. The time follows the **yyyy-MM-ddTHH:mm:ssZ** format.
+        # Creates a layer version.
         self.create_time = create_time
-        # The description of the layer version.
-        self.description = description
         # The name of the layer.
+        self.description = description
+        # The list of runtime environments that are supported by the layer.
         self.layer_name = layer_name
-        # The version of the layer.
+        # The time when the layer version was created. The time follows the **yyyy-MM-ddTHH:mm:ssZ** format.
         self.version = version
 
     def validate(self):
         if self.code:
             self.code.validate()
 
     def to_map(self):
@@ -4842,19 +4767,19 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
-        self.x_fc_account_id = x_fc_account_id
         # The time when the request is initiated on the client. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
-        self.x_fc_date = x_fc_date
+        self.x_fc_account_id = x_fc_account_id
         # The custom request ID.
+        self.x_fc_date = x_fc_date
+        # The ETag that is used to modify the trigger. This parameter is used to ensure that the modified trigger is consistent with the trigger to be modified.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4892,43 +4817,43 @@
         invocation_role: str = None,
         qualifier: str = None,
         source_arn: str = None,
         trigger_config: str = None,
         trigger_name: str = None,
         trigger_type: str = None,
     ):
-        # The description of the trigger.
+        # The ID of your Alibaba Cloud account.
         self.description = description
-        # The role that is used by the event source such as OSS to invoke the function. For more information, see [Overview](~~53102~~).
-        self.invocation_role = invocation_role
         # The version or alias of the service.
-        self.qualifier = qualifier
+        self.invocation_role = invocation_role
         # The Alibaba Cloud Resource Name (ARN) of the event source for the trigger.
-        self.source_arn = source_arn
+        self.qualifier = qualifier
         # The configurations of the trigger. The configurations vary based on the trigger type. For more information about the format, see the following topics:
         # 
         # * OSS trigger: [OSSTriggerConfig](~~struct:OSSTriggerConfig~~).
         # * Log Service trigger: [LogTriggerConfig](~~struct:LogTriggerConfig~~).
         # * Time trigger: [TimeTriggerConfig](~~struct:LogTriggerConfig~~).
         # * HTTP trigger: [HTTPTriggerConfig](~~struct:HTTPTriggerConfig~~).
         # * Tablestore trigger: Specify the **SourceArn** parameter and leave this parameter empty.
         # * Alibaba Cloud CDN event trigger: [CDNEventsTriggerConfig](~~struct:CDNEventsTriggerConfig~~).
         # * MNS topic trigger: [MnsTopicTriggerConfig](~~struct:MnsTopicTriggerConfig~~).
-        self.trigger_config = trigger_config
+        self.source_arn = source_arn
         # The name of the trigger. The name contains only letters, digits, hyphens (-), and underscores (\_). The name must be 1 to 128 characters in length and cannot start with a digit or hyphen (-).
-        self.trigger_name = trigger_name
+        self.trigger_config = trigger_config
         # The type of the trigger. Valid values:
         # 
         # *   **oss**: OSS event trigger. For more information, see [Overview](~~62922~~).
         # *   **log**: Log Service trigger. For more information, see [Overview](~~84386~~).
         # *   **timer**: time trigger. For more information, see [Overview](~~68172~~).
         # *   **http**: HTTP trigger. For more information, see [Overview](~~71229~~).
         # *   **tablestore**: Tablestore trigger. For more information, see [Overview](~~100092~~).
         # *   **cdn_events**: CDN event trigger. For more information, see [Overview](~~73333~~).
         # *   **mns_topic**: MNS topic trigger. For more information, see [Overview](~~97032~~).
+        self.trigger_name = trigger_name
+        # The description of the trigger.
         self.trigger_type = trigger_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4984,39 +4909,38 @@
         trigger_config: str = None,
         trigger_id: str = None,
         trigger_name: str = None,
         trigger_type: str = None,
         url_internet: str = None,
         url_intranet: str = None,
     ):
-        # The time when the trigger was created.
+        # The ARN of the RAM role that is used by the event source to invoke the function.
         self.created_time = created_time
-        # The description of the trigger.
+        # The unique ID of the trigger.
         self.description = description
-        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
+        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
         self.domain_name = domain_name
-        # The ARN of the RAM role that is used by the event source to invoke the function.
-        self.invocation_role = invocation_role
         # The time when the trigger was last modified.
-        self.last_modified_time = last_modified_time
+        self.invocation_role = invocation_role
         # The version of the service.
-        self.qualifier = qualifier
+        self.last_modified_time = last_modified_time
         # The ARN of the event source.
-        self.source_arn = source_arn
+        self.qualifier = qualifier
         # The configurations of the trigger. The configurations vary based on the trigger type.
+        self.source_arn = source_arn
+        # The name of the trigger. The name contains only letters, digits, hyphens (-), and underscores (\_). The name must be 1 to 128 characters in length and cannot start with a digit or hyphen (-).
         self.trigger_config = trigger_config
-        # The unique ID of the trigger.
+        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
         self.trigger_id = trigger_id
-        # The name of the trigger. The name contains only letters, digits, hyphens (-), and underscores (\_). The name must be 1 to 128 characters in length and cannot start with a digit or hyphen (-).
-        self.trigger_name = trigger_name
         # The trigger type, such as **oss**, **log**, **tablestore**, **timer**, **http**, **cdn_events**, and **mns_topic**.
+        self.trigger_name = trigger_name
+        # The description of the trigger.
         self.trigger_type = trigger_type
-        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
-        self.url_internet = url_internet
         # The private endpoint. In a VPC, you can access HTTP triggers by using HTTP or HTTPS.
+        self.url_internet = url_internet
         self.url_intranet = url_intranet
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5132,19 +5056,18 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # Binds a VPC.
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # {"name":"CreateVpcBinding","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/services/{serviceName}/bindings","deprecated":0,"method":"POST","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"serviceName\",\"position\":\"Path\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"A short description of struct\",\"description\":\"The name of the service. \",\"example\":\"demo-service\"},{\"name\":\"body\",\"position\":\"Body\",\"style\":\"json\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Object\",\"params\":[{\"name\":\"vpcId\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of the VPC to be bound. \",\"example\":\"v-xxxx\"}],\"description\":\"The structure of the request. \"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. Specify the time in the yyyy-mm-ddhh:mm:ss format. \",\"example\":\"2022-01-0112:00:00\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The custom request ID. \",\"example\":\"asdf****\"}]","response_headers":"[]","response":"{}","body_style":"json","errors":"{}"}
         self.x_fc_date = x_fc_date
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5176,15 +5099,15 @@
 
 
 class CreateVpcBindingRequest(TeaModel):
     def __init__(
         self,
         vpc_id: str = None,
     ):
-        # The ID of the VPC to be bound.
+        # Example 1
         self.vpc_id = vpc_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5243,23 +5166,20 @@
         common_headers: Dict[str, str] = None,
         if_match: str = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # If the ETag specified in the request matches the ETag value of the object, OSS transmits the object and returns 200 OK. If the ETag specified in the request does not match the ETag value of the object, OSS returns 412 Precondition Failed. 
-        # The ETag value of a resource is used to check whether the resource has changed. You can check data integrity by using the ETag value. 
-        # Default value: null
+        # {"name":"DeleteAlias","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/services/{serviceName}/aliases/{aliasName}","deprecated":0,"method":"DELETE","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"serviceName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the service.\",\"description\":\"The name of the service.\",\"example\":\"demo-service\"},{\"name\":\"aliasName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the alias.\",\"description\":\"The name of the alias.\",\"example\":\"test\"},{\"name\":\"If-Match\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"If the ETag specified in the request matches the ETag value of the object, OSS transmits the object and returns 200 OK. If the ETag specified in the request does not match the ETag value of the object, OSS returns 412 Precondition Failed. \\nThe ETag value of a resource is used to check whether the resource has changed. You can check data integrity by using the ETag value. \\nDefault value: null\",\"example\":\"e19d5cd5af0378da05f63f891c7467af\"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. \",\"example\":\"2020-12-1210:00:00\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The trace ID of the invocation request of Function Compute. \",\"example\":\"r9s89isisi****\"}]","response_headers":"[]","response":"{}","errors":"{}"}
         self.if_match = if_match
-        # The ID of your Alibaba Cloud account.
+        # 139490
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Xiaoqi
         self.x_fc_date = x_fc_date
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5333,19 +5253,18 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # 150868
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Xiawan
         self.x_fc_date = x_fc_date
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5416,21 +5335,19 @@
         common_headers: Dict[str, str] = None,
         if_match: str = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ETag value of the resource. This value is used to ensure that the modified resource is consistent with the resource to be modified. The ETag value is returned in the responses of the CREATE, GET, and UPDATE operations.
+        # $.parameters[8].schema.description
         self.if_match = if_match
-        # The ID of your Alibaba Cloud account.
+        # {"name":"DeleteFunction","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/services/{serviceName}/functions/{functionName}","deprecated":0,"method":"DELETE","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"If-Match\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The ETag value of the resource. This value is used to ensure that the modified resource is consistent with the resource to be modified. The ETag value is returned in the responses of the CREATE, GET, and UPDATE operations.\",\"description\":\"The ETag value of the resource. This value is used to ensure that the modified resource is consistent with the resource to be modified. The ETag value is returned in the responses of the CREATE, GET, and UPDATE operations. \",\"example\":\"e19d5cd5af0378da05f63f891c7467af\"},{\"name\":\"serviceName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the service.\",\"description\":\"The name of the service. \",\"example\":\"demoService\"},{\"name\":\"functionName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the function.\",\"description\":\"The name of the function. \",\"example\":\"demoFunction\"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The start time when the function is invoked. Specify the time in the yyyy-mm-ddhh:mm:ss format. \",\"example\":\"2022-01-01 12:00:00\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The trace ID of the request for Function Compute API. The value is the same as that of the requestId parameter in the response. \",\"example\":\"test-trace-id\"}]","response_headers":"[]","response":"{}","errors":"{}"}
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date
-        # The trace ID of the request for Function Compute API. The value is the same as that of the requestId parameter in the response.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5504,19 +5421,18 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # {"name":"DeleteFunctionAsyncInvokeConfig","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/services/{serviceName}/functions/{functionName}/async-invoke-config","deprecated":0,"method":"DELETE","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"serviceName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the service.\",\"description\":\"The name of the service. \",\"example\":\"demo-service\"},{\"name\":\"functionName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the function.\",\"description\":\"The name of the function. \",\"example\":\"helloworld\"},{\"name\":\"qualifier\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The qualifier.\",\"description\":\"The qualifier. \",\"example\":\"test\"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. \",\"example\":\"None\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The trace ID of the invocation request of Function Compute.\",\"example\":\"asdf*****\"}]","response_headers":"[]","response":"{}","errors":"{}"}
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Jianyi
         self.x_fc_date = x_fc_date
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5548,15 +5464,15 @@
 
 
 class DeleteFunctionAsyncInvokeConfigRequest(TeaModel):
     def __init__(
         self,
         qualifier: str = None,
     ):
-        # The qualifier.
+        # Deletes the asynchronous invocation configurations of a function in a service.
         self.qualifier = qualifier
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5615,21 +5531,19 @@
         common_headers: Dict[str, str] = None,
         if_match: str = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # If the ETag specified in the request matches the ETag value of the OndemandConfig, FC returns 200 OK. If the ETag specified in the request does not match the ETag value of the object, FC returns 412 Precondition Failed.
+        # Xiaoqi
         self.if_match = if_match
-        # The ID of your Alibaba Cloud account.
+        # 65332
         self.x_fc_account_id = x_fc_account_id
-        # The start time when the function is invoked. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date
-        # The trace ID of the request for Function Compute API, which is also the unique ID of the request.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5665,15 +5579,15 @@
 
 
 class DeleteFunctionOnDemandConfigRequest(TeaModel):
     def __init__(
         self,
         qualifier: str = None,
     ):
-        # The alias of the service or LATEST.
+        # Deletes the on-demand configuration of a function.
         self.qualifier = qualifier
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5731,19 +5645,18 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # 320124
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Luoni
         self.x_fc_date = x_fc_date
-        # The trace ID of the request for Function Compute API.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5814,21 +5727,19 @@
         common_headers: Dict[str, str] = None,
         if_match: str = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ETag value of the service. This value is used to ensure that the modified service is consistent with the service to be modified. The ETag value is returned in the responses of the [CreateService](~~175256~~), [UpdateService](~~188167~~), and [GetService](~~189225~~) operations.
+        # Examples
         self.if_match = if_match
-        # The ID of your Alibaba Cloud account.
+        # Liuxia
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5902,19 +5813,17 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # Xiaoqi
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5985,21 +5894,17 @@
         common_headers: Dict[str, str] = None,
         if_match: str = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # This parameter is used to ensure that the modified resource is consistent with the resource to be modified. You can obtain the parameter value from the responses of [CreateTrigger](~~415729~~), [GetTrigger](~~415732~~), and [UpdateTrigger](~~415731~~) operations.
         self.if_match = if_match
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The time when the request is initiated on the client. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6073,19 +5978,18 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # Deletes a bound VPC.
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # {"name":"DeleteVpcBinding","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/services/{serviceName}/bindings/{vpcId}","deprecated":0,"method":"DELETE","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"serviceName\",\"position\":\"Path\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The name of the service. \",\"example\":\"demoService\"},{\"name\":\"vpcId\",\"position\":\"Path\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of the VPC to be unbound. \",\"example\":\"vpc-xxxx\"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. Specify the time in the yyyy-mm-ddhh:mm:ss format. \",\"example\":\"2022-01-0112:00:00\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The custom request ID. \",\"example\":\"asdf****\"}]","response_headers":"[]","response":"{}","errors":"{}"}
         self.x_fc_date = x_fc_date
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6155,19 +6059,16 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6199,15 +6100,14 @@
 
 
 class DeregisterEventSourceRequest(TeaModel):
     def __init__(
         self,
         qualifier: str = None,
     ):
-        # The version or alias of the service.
         self.qualifier = qualifier
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6267,17 +6167,17 @@
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Example 1
         self.x_fc_date = x_fc_date
-        # The custom request ID.
+        # Queries available zones within the current account.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6310,17 +6210,16 @@
 
 class GetAccountSettingsResponseBody(TeaModel):
     def __init__(
         self,
         available_azs: List[str] = None,
         default_role: str = None,
     ):
-        # The list of zones.
+        # Liuxia
         self.available_azs = available_azs
-        # The default RAM role.
         self.default_role = default_role
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6394,15 +6293,15 @@
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The start time when the function is invoked. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The time on which the function is invoked. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date
         # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
@@ -6443,33 +6342,33 @@
         created_time: str = None,
         description: str = None,
         last_modified_time: str = None,
         resolve_policy: str = None,
         route_policy: RoutePolicy = None,
         version_id: str = None,
     ):
-        # The canary release version to which the alias points and the weight of the canary release version. 
+        # The additional version to which the alias points and the weight of the additional version.
         # 
-        # - The canary release version takes effect only when the function is invoked. 
-        # - The value consists of a version number and the corresponding weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
+        # *   The additional version takes effect only when the function is invoked.
+        # *   The value consists of a version number and a specific weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
         self.additional_version_weight = additional_version_weight
         # The name of the alias.
         self.alias_name = alias_name
         # The time when the alias was created.
         self.created_time = created_time
         # The description of the alias.
         self.description = description
         # The time when the alias was last modified.
         self.last_modified_time = last_modified_time
         # The canary release mode. Valid values:
         # 
-        # - **Random**: random canary release. This is the default value.
-        # - **Content**: rule-based canary release.
+        # *   **Random**: random canary release. This is the default value.
+        # *   **Content**: rule-based canary release.
         self.resolve_policy = resolve_policy
-        # Canary release rule. The traffic that meets the conditions of the canary release rule is diverted to the canary release instances.
+        # The canary release rule. Traffic that meets the canary release rule is routed to the canary release instance.
         self.route_policy = route_policy
         # The version to which the alias points.
         self.version_id = version_id
 
     def validate(self):
         if self.route_policy:
             self.route_policy.validate()
@@ -6767,19 +6666,19 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # The custom request ID.
         self.x_fc_account_id = x_fc_account_id
-        # The time on which the function is invoked. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
+        # The value that is used to ensure that the modified function is consistent with the function that is expected to be modified.
         self.x_fc_date = x_fc_date
-        # The custom request ID.
+        # The definition of the function.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6811,15 +6710,15 @@
 
 
 class GetFunctionRequest(TeaModel):
     def __init__(
         self,
         qualifier: str = None,
     ):
-        # The version or alias of the service.
+        # The ID of your Alibaba Cloud account.
         self.qualifier = qualifier
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6866,85 +6765,81 @@
         last_modified_time: str = None,
         layers: List[str] = None,
         layers_arn_v2: List[str] = None,
         memory_size: int = None,
         runtime: str = None,
         timeout: int = None,
     ):
-        # The port on which the HTTP server listens for the custom runtime or custom container runtime.
+        # The list of layers (ARN V1 version).
+        # 
+        # > If multiple layers exist, the layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file with the same name in the layer with a larger subscript. >
+        # 
+        # **\
+        # 
+        # **Warning:** This parameter is to be deprecated. Use layersArnV2.
         self.ca_port = ca_port
-        # The CRC-64 value of the function code package.
+        # The time when the function was created.
         self.code_checksum = code_checksum
-        # The size of the function code package. Unit: byte.
+        # The description of the function.
         self.code_size = code_size
-        # The number of vCPUs of the function. The value must be a multiple of 0.05.
+        # The GPU memory capacity for the function. Unit: MB. The memory capacity must be a multiple of 1024 MB.
         self.cpu = cpu
-        # The time when the function was created.
+        # The environment variables that are configured for the function. You can obtain the values of the environment variables from the function. For more information, see [Environment variables](~~69777~~).
         self.created_time = created_time
-        # The configurations of the custom container runtime. After you configure the custom container runtime, Function Compute can execute the function in a container created from a custom image.
+        # The name of the layer resource (ARN V1 version).
         self.custom_container_config = custom_container_config
-        # The custom DNS configurations of the function.
-        self.custom_dns = custom_dns
         # The custom health check configuration of the function. This parameter is applicable only to custom runtimes and custom containers.
+        self.custom_dns = custom_dns
+        # The name of the layer resource (ARN V2 version).
         self.custom_health_check_config = custom_health_check_config
-        # The configurations of the custom runtime.
+        # The list of layers (ARN V2 version).
+        # 
+        # > If multiple layers exist, the layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name and a larger subscript in the layer.
         self.custom_runtime_config = custom_runtime_config
-        # The description of the function.
+        # The environment variables that you configured for the function.
         self.description = description
-        # The disk size of the function. Unit: MB. Valid values: 512 and 10240.
         self.disk_size = disk_size
-        # The environment variables that are configured for the function. You can obtain the values of the environment variables from the function. For more information, see [Environment variables](~~69777~~).
-        self.environment_variables = environment_variables
         # The ID that is generated by the system for the function. Each function ID is unique in Function Compute.
+        self.environment_variables = environment_variables
+        # The handler of the function. For more information, see [Function handler](~~157704~~).
         self.function_id = function_id
-        # The name of the function.
+        # The time when the function was last modified.
         self.function_name = function_name
-        # The GPU memory capacity for the function. Unit: MB. The memory capacity must be a multiple of 1024 MB.
         self.gpu_memory_size = gpu_memory_size
-        # The handler of the function. For more information, see [Function handler](~~157704~~).
+        # The memory size for the function. Unit: MB. The memory size must be a multiple of 64 MB. The memory size varies based on the function instance type. For more information, see [Instance types](~~179379~~).
         self.handler = handler
-        # The timeout period for the execution of the initializer function. Unit: seconds. Default value: 3. Valid values: 1 to 300. When this period ends, the execution of the initializer function is terminated.
+        # The port on which the HTTP server listens for the custom runtime or custom container runtime.
         self.initialization_timeout = initialization_timeout
-        # The handler of the initializer function. The format of the value is determined by the programming language that you use. For more information, see [Initializer function](~~157704~~).
+        # The configurations of the custom container runtime. After you configure the custom container runtime, Function Compute can execute the function in a container created from a custom image.
         self.initializer = initializer
-        # The number of requests that can be concurrently processed by a single instance.
-        self.instance_concurrency = instance_concurrency
-        # The lifecycle configurations of the instance.
-        self.instance_lifecycle_config = instance_lifecycle_config
-        # The soft concurrency of the instance. You can use this parameter to implement graceful scale-up of instances. If the number of concurrent requests on an instance is greater than the number of the soft concurrency, the instance scale-up is triggered. For example, if your instance requires a long time to start, you can specify a suitable soft concurrency to start the instance in advance.
-        # 
-        # The value must be less than or equal to that of the **instanceConcurrency** parameter.
-        self.instance_soft_concurrency = instance_soft_concurrency
         # The instance type of the function. Valid values:
         # 
         # *   **e1**: elastic instance
         # *   **c1**: performance instance
         # *   **fc.gpu.tesla.1**: GPU-accelerated instances (Tesla T4)
         # *   **fc.gpu.ampere.1**: GPU-accelerated instances (Ampere A10)
         # *   **g1**: same fc.gpu.tesla.1
+        self.instance_concurrency = instance_concurrency
+        # The configurations of the custom runtime.
+        self.instance_lifecycle_config = instance_lifecycle_config
+        # The lifecycle configurations of the instance.
+        self.instance_soft_concurrency = instance_soft_concurrency
+        # The custom DNS configurations of the function.
         self.instance_type = instance_type
-        # The time when the function was last modified.
+        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore2.1**, **custom**, and **custom-container**.
         self.last_modified_time = last_modified_time
-        # The list of layers (ARN V1 version).
-        # 
-        # > If multiple layers exist, the layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file with the same name in the layer with a larger subscript. >
-        # 
-        # **\
-        # 
-        # **Warning:** This parameter is to be deprecated. Use layersArnV2.
+        # The number of requests that can be concurrently processed by a single instance.
         self.layers = layers
-        # The list of layers (ARN V2 version).
-        # 
-        # > If multiple layers exist, the layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name and a larger subscript in the layer.
+        # The number of vCPUs of the function. The value must be a multiple of 0.05.
         self.layers_arn_v2 = layers_arn_v2
-        # The memory size for the function. Unit: MB. The memory size must be a multiple of 64 MB. The memory size varies based on the function instance type. For more information, see [Instance types](~~179379~~).
+        # The timeout period for the execution of the function. Unit: seconds. Default value: 60. Valid values: 1 to 600. When this period expires, the execution of the function is terminated.
         self.memory_size = memory_size
-        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore2.1**, **custom**, and **custom-container**.
+        # The timeout period for the execution of the initializer function. Unit: seconds. Default value: 3. Valid values: 1 to 300. When this period ends, the execution of the initializer function is terminated.
         self.runtime = runtime
-        # The timeout period for the execution of the function. Unit: seconds. Default value: 60. Valid values: 1 to 600. When this period expires, the execution of the function is terminated.
+        # The handler of the initializer function. The format of the value is determined by the programming language that you use. For more information, see [Initializer function](~~157704~~).
         self.timeout = timeout
 
     def validate(self):
         if self.custom_container_config:
             self.custom_container_config.validate()
         if self.custom_dns:
             self.custom_dns.validate()
@@ -7134,19 +7029,16 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The time when the Function Compute is called. The format is **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7178,15 +7070,14 @@
 
 
 class GetFunctionAsyncInvokeConfigRequest(TeaModel):
     def __init__(
         self,
         qualifier: str = None,
     ):
-        # The qualifier.
         self.qualifier = qualifier
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7214,34 +7105,22 @@
         last_modified_time: str = None,
         max_async_event_age_in_seconds: int = None,
         max_async_retry_attempts: int = None,
         qualifier: str = None,
         service: str = None,
         stateful_invocation: bool = None,
     ):
-        # The time when the desktop group was created.
         self.created_time = created_time
-        # The configuration structure of the destination for asynchronous invocations.
         self.destination_config = destination_config
-        # The name of the function.
         self.function = function
-        # The time when the configuration was last modified.
         self.last_modified_time = last_modified_time
-        # The maximum validity period of a message.
         self.max_async_event_age_in_seconds = max_async_event_age_in_seconds
-        # The maximum number of retries allowed after an asynchronous invocation fails.
         self.max_async_retry_attempts = max_async_retry_attempts
-        # The version or alias of the service to which the function belongs.
         self.qualifier = qualifier
-        # The name of the service.
         self.service = service
-        # Indicates whether the asynchronous task feature is enabled.
-        # 
-        # *   **true**: The asynchronous task feature is enabled.
-        # *   **false**: The asynchronous task feature is disabled.
         self.stateful_invocation = stateful_invocation
 
     def validate(self):
         if self.destination_config:
             self.destination_config.validate()
 
     def to_map(self):
@@ -7343,19 +7222,16 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The time on which the function is invoked. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7387,15 +7263,14 @@
 
 
 class GetFunctionCodeRequest(TeaModel):
     def __init__(
         self,
         qualifier: str = None,
     ):
-        # The version or alias of the service.
         self.qualifier = qualifier
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7416,17 +7291,15 @@
 
 class GetFunctionCodeResponseBody(TeaModel):
     def __init__(
         self,
         checksum: str = None,
         url: str = None,
     ):
-        # The CRC-64 value of the function code package.
         self.checksum = checksum
-        # The URL of the function code package.
         self.url = url
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7653,19 +7526,19 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # This parameter is returned only when the information about a specific layer version is queried.
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The location of the layer code.
         self.x_fc_date = x_fc_date
-        # The trace ID of the request for Function Compute API.
+        # The structure of the layer code.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7952,19 +7825,22 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # The Alibaba Cloud Resource Name (ARN) of the resource. 
+        # > **Note:** You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource. You can manage tags only for services for top level resources.
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The tag dictionary. Valid values:
+        # - **key**: the key of the tag. 
+        # - **value**: the value of the tag.
         self.x_fc_date = x_fc_date
-        # The custom request ID.
+        # Example 1
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7996,17 +7872,16 @@
 
 
 class GetResourceTagsRequest(TeaModel):
     def __init__(
         self,
         resource_arn: str = None,
     ):
-        # The Alibaba Cloud Resource Name (ARN) of the resource. 
-        # 
-        # > You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource. You can manage tags only for services for top level resources.
+        # The ARN of the resource. 
+        # > **Note:** You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource.
         self.resource_arn = resource_arn
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8027,19 +7902,16 @@
 
 class GetResourceTagsResponseBody(TeaModel):
     def __init__(
         self,
         resource_arn: str = None,
         tags: Dict[str, str] = None,
     ):
-        # The ARN of the resource. 
-        # 
-        # > You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource.
+        # 147258
         self.resource_arn = resource_arn
-        # The tag dictionary.
         self.tags = tags
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8359,31 +8231,25 @@
         x_fc_code_checksum: str = None,
         x_fc_date: str = None,
         x_fc_invocation_type: str = None,
         x_fc_log_type: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # The list of events that trigger the asynchronous task.
         self.x_fc_account_id = x_fc_account_id
-        # The CRC-64 value of the function code package. This value is used to check data integrity. The value is automatically calculated by the tool.
+        # The structure of the asynchronous task.
         self.x_fc_code_checksum = x_fc_code_checksum
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Alibaba Cloud provides SDKs for multiple programming languages to help you integrate Alibaba Cloud services by using APIs. We recommend that you use an SDK to call API operations. This frees you from manual signature verification.
         self.x_fc_date = x_fc_date
-        # The invocation method. 
-        # 
-        # - **Sync**: synchronous invocation 
-        # - **Async**: asynchronous invocation
+        # StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
         self.x_fc_invocation_type = x_fc_invocation_type
-        # The method used to return logs. Valid values: 
-        # 
-        # - **Tail**: returns the last 4 KB of logs that are generated for the current request. 
-        # - **None**: does not return logs for the current request. This is the default value.
+        # The latest version of Function Compute API.
         self.x_fc_log_type = x_fc_log_type
-        # The trace ID of the invocation request of Function Compute.
+        # You can search for API operations, call and debug API operations online, and dynamically generate executable sample code for SDKs.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8427,15 +8293,15 @@
 
 
 class GetStatefulAsyncInvocationRequest(TeaModel):
     def __init__(
         self,
         qualifier: str = None,
     ):
-        # The version or alias of the service to which the asynchronous task belongs.
+        # The ID of the instance that is used to run the asynchronous task.
         self.qualifier = qualifier
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8503,19 +8369,19 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
-        self.x_fc_account_id = x_fc_account_id
         # The time when the request is initiated on the client. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
-        self.x_fc_date = x_fc_date
+        self.x_fc_account_id = x_fc_account_id
         # The custom request ID.
+        self.x_fc_date = x_fc_date
+        # The ETag that is used to modify the trigger. This parameter is used to ensure that the modified trigger is consistent with the trigger to be modified.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8559,47 +8425,46 @@
         trigger_config: str = None,
         trigger_id: str = None,
         trigger_name: str = None,
         trigger_type: str = None,
         url_internet: str = None,
         url_intranet: str = None,
     ):
-        # The time when the trigger was created.
+        # The ARN of the RAM role that is used by the event source to invoke the function.
         self.created_time = created_time
-        # The description of the trigger.
+        # The unique ID of the trigger.
         self.description = description
-        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
+        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
         self.domain_name = domain_name
-        # The ARN of the RAM role that is used by the event source to invoke the function.
-        self.invocation_role = invocation_role
         # The time when the trigger was last modified.
-        self.last_modified_time = last_modified_time
+        self.invocation_role = invocation_role
         # The version or alias of the service.
-        self.qualifier = qualifier
+        self.last_modified_time = last_modified_time
         # The ARN of the event source.
-        self.source_arn = source_arn
+        self.qualifier = qualifier
         # The configurations of the trigger. The configurations vary based on the trigger type. For more information about the format, see the following topics:
         # 
         # *   OSS trigger: [OSSTriggerConfig](~~struct:OSSTriggerConfig~~).
         # *   Log Service trigger: [LogTriggerConfig](~~struct:LogTriggerConfig~~).
         # *   Time trigger: [TimeTriggerConfig](~~struct:TimeTriggerConfig~~).
         # *   HTTP trigger: [HTTPTriggerConfig](~~struct:HTTPTriggerConfig~~).
         # *   Tablestore trigger: Specify the **SourceArn** parameter and leave this parameter empty.
         # *   Alibaba Cloud CDN event trigger: [CDNEventsTriggerConfig](~~struct:CDNEventsTriggerConfig~~).
         # *   MNS topic trigger: [MnsTopicTriggerConfig](~~struct:MnsTopicTriggerConfig~~).
+        self.source_arn = source_arn
+        # The name of the trigger.
         self.trigger_config = trigger_config
-        # The unique ID of the trigger.
+        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
         self.trigger_id = trigger_id
-        # The name of the trigger.
-        self.trigger_name = trigger_name
         # The trigger type, such as **oss**, **log**, **tablestore**, **timer**, **http**, **cdn_events**, and **mns_topic**.
+        self.trigger_name = trigger_name
+        # The description of the trigger.
         self.trigger_type = trigger_type
-        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
-        self.url_internet = url_internet
         # The private endpoint. In a VPC, you can access HTTP triggers by using HTTP or HTTPS.
+        self.url_internet = url_internet
         self.url_intranet = url_intranet
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8714,14 +8579,15 @@
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_invocation_type: str = None,
         x_fc_log_type: str = None,
+        x_fc_stateful_async_invocation_enable: str = None,
         x_fc_stateful_async_invocation_id: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
         # The time when the function is invoked. The format is **EEE,d MMM yyyy HH:mm:ss GMT**.
@@ -8732,14 +8598,15 @@
         # *   **Async**: asynchronous
         self.x_fc_invocation_type = x_fc_invocation_type
         # The method used to return logs. Valid values:
         # 
         # *   **Tail**: returns the last 4 KB of logs that are generated for the current request.
         # *   **None**: No logs are returned for the current request. Default value: None.
         self.x_fc_log_type = x_fc_log_type
+        self.x_fc_stateful_async_invocation_enable = x_fc_stateful_async_invocation_enable
         # The ID of the asynchronous task. You must enable the asynchronous task feature in advance.
         # 
         # > When you use an SDK to invoke a function, we recommend that you specify a business-related ID to facilitate subsequent operations. For example, you can use the video name as the invocation ID for a video-processing function. This way, you can use the ID to check whether the video is processed or terminate the processing of the video. The ID must start with a letter or an underscore (\_) and can contain letters, digits, underscores (\_), and hyphens (-). The ID can be up to 128 characters in length. If you do not specify the ID of the asynchronous invocation, Function Compute automatically generates an ID.
         self.x_fc_stateful_async_invocation_id = x_fc_stateful_async_invocation_id
         # The trace ID of the request for Function Compute API. The value is the same as that of the **requestId** parameter in the response.
         self.x_fc_trace_id = x_fc_trace_id
 
@@ -8758,14 +8625,16 @@
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
 
     def from_map(self, m: dict = None):
@@ -8776,14 +8645,16 @@
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
 
 
@@ -8870,15 +8741,15 @@
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The start time when the function is invoked. Specify the time in the yyyy-mm-ddhh:mm:ss format.
+        # The time on which the function is invoked. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date
         # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
@@ -8915,21 +8786,21 @@
     def __init__(
         self,
         limit: int = None,
         next_token: str = None,
         prefix: str = None,
         start_key: str = None,
     ):
-        # The maximum number of resources to return.
+        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
         self.limit = limit
-        # The token used to obtain more results.
+        # The token required to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
         self.next_token = next_token
-        # The prefix.
+        # The prefix that the names of returned resources must contain.
         self.prefix = prefix
-        # The starting position of the result list.
+        # The starting position of the result list. The returned resources are sorted in alphabetical order, and the resources that include and follow the resource specified by the startKey parameter are returned.
         self.start_key = start_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8968,25 +8839,33 @@
         created_time: str = None,
         description: str = None,
         last_modified_time: str = None,
         resolve_policy: str = None,
         route_policy: RoutePolicy = None,
         version_id: str = None,
     ):
-        # The weight of the canary release version.
+        # The additional version to which the alias points and the weight of the additional version.
+        # 
+        # *   The additional version takes effect only when the function is invoked.
+        # *   The value consists of a version number and a specific weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
         self.additional_version_weight = additional_version_weight
         # The name of the alias.
         self.alias_name = alias_name
-        # The creation time.
+        # The time when the ConfigMaps were created.
         self.created_time = created_time
         # The description of the alias.
         self.description = description
-        # The last update time.
+        # The time at which the system parameter was last modified.
         self.last_modified_time = last_modified_time
+        # The canary release mode. Valid values:
+        # 
+        # *   **Random**: random canary release. This is the default value.
+        # *   **Content**: rule-based canary release.
         self.resolve_policy = resolve_policy
+        # The canary release rule. Traffic that meets the canary release rule is routed to the canary release instance.
         self.route_policy = route_policy
         # The ID of the version.
         self.version_id = version_id
 
     def validate(self):
         if self.route_policy:
             self.route_policy.validate()
@@ -9419,19 +9298,19 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # $.parameters[7].schema.enumValueTitles
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # $.parameters[8].schema.description
         self.x_fc_date = x_fc_date
-        # The trace ID of the invocation request of Function Compute.
+        # $.parameters[8].schema.example
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9463,15 +9342,15 @@
 
 
 class ListEventSourcesRequest(TeaModel):
     def __init__(
         self,
         qualifier: str = None,
     ):
-        # The version or alias of the service.
+        # $.parameters[7].schema.example
         self.qualifier = qualifier
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9492,17 +9371,16 @@
 
 class ListEventSourcesResponseBodyEventSources(TeaModel):
     def __init__(
         self,
         created_time: str = None,
         source_arn: str = None,
     ):
-        # The time when the event source was created.
         self.created_time = created_time
-        # The ARN of the event source.
+        # Jianyi
         self.source_arn = source_arn
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9526,15 +9404,15 @@
 
 
 class ListEventSourcesResponseBody(TeaModel):
     def __init__(
         self,
         event_sources: List[ListEventSourcesResponseBodyEventSources] = None,
     ):
-        # The information about event sources.
+        # Queries all the event sources of a function.
         self.event_sources = event_sources
 
     def validate(self):
         if self.event_sources:
             for k in self.event_sources:
                 if k:
                     k.validate()
@@ -9613,31 +9491,19 @@
         x_fc_code_checksum: str = None,
         x_fc_date: str = None,
         x_fc_invocation_type: str = None,
         x_fc_log_type: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The CRC-64 value of the function code package. This value is used to check data integrity. The value is automatically calculated by the tool.
         self.x_fc_code_checksum = x_fc_code_checksum
-        # The time when the Function Compute is called. The format is **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date
-        # The invocation method.
-        # 
-        # *   **Sync**: synchronous
-        # *   **Async**: asynchronous
         self.x_fc_invocation_type = x_fc_invocation_type
-        # The method used to return logs. Valid values:
-        # 
-        # *   **Tail**: returns the last 4 KB of logs that are generated for the current request.
-        # *   **None**: No logs are returned for the current request. Default value: None.
         self.x_fc_log_type = x_fc_log_type
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9682,17 +9548,15 @@
 
 class ListFunctionAsyncInvokeConfigsRequest(TeaModel):
     def __init__(
         self,
         limit: int = None,
         next_token: str = None,
     ):
-        # The maximum number of resources to return.
         self.limit = limit
-        # The token required to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
         self.next_token = next_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9724,36 +9588,22 @@
         last_modified_time: str = None,
         max_async_event_age_in_seconds: int = None,
         max_async_retry_attempts: int = None,
         qualifier: str = None,
         service: str = None,
         stateful_invocation: bool = None,
     ):
-        # The time when the desktop group was created.
         self.created_time = created_time
-        # The configuration structure of the destination for asynchronous invocations. If you have not configured this parameter, this parameter is null.
         self.destination_config = destination_config
-        # The name of the function.
         self.function = function
-        # The time when the configuration was last modified.
         self.last_modified_time = last_modified_time
-        # The maximum validity period of a message. If you have not configured this parameter, this parameter is null.
         self.max_async_event_age_in_seconds = max_async_event_age_in_seconds
-        # The maximum number of retries allowed after an asynchronous invocation fails. If you have not configured this parameter, this parameter is null.
         self.max_async_retry_attempts = max_async_retry_attempts
-        # The version or alias of the service.
         self.qualifier = qualifier
-        # The name of the service.
         self.service = service
-        # Indicates whether the asynchronous task feature is enabled.
-        # 
-        # *   **true**: The asynchronous task feature is enabled.
-        # *   **false**: The asynchronous task feature is disabled.
-        # 
-        # If you have not configured this parameter, this parameter is null.
         self.stateful_invocation = stateful_invocation
 
     def validate(self):
         if self.destination_config:
             self.destination_config.validate()
 
     def to_map(self):
@@ -9808,17 +9658,15 @@
 
 class ListFunctionAsyncInvokeConfigsResponseBody(TeaModel):
     def __init__(
         self,
         configs: List[ListFunctionAsyncInvokeConfigsResponseBodyConfigs] = None,
         next_token: str = None,
     ):
-        # The list of asynchronous invocation configurations.
         self.configs = configs
-        # The token used to obtain more results.
         self.next_token = next_token
 
     def validate(self):
         if self.configs:
             for k in self.configs:
                 if k:
                     k.validate()
@@ -10078,15 +9926,15 @@
         self.last_modified_time = last_modified_time
         # The information about layers.
         # 
         # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name as a layer with a larger subscript.
         self.layers = layers
         # The memory size that is configured for the function. Unit: MB.
         self.memory_size = memory_size
-        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom** and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
+        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.10**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom.debian10**, **custom**, and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
         self.runtime = runtime
         # The timeout period for the execution of the function. Unit: seconds. Default value: 60. Valid values: 1 to 600. When this period expires, the execution of the function is terminated.
         self.timeout = timeout
 
     def validate(self):
         if self.custom_container_config:
             self.custom_container_config.validate()
@@ -10301,15 +10149,15 @@
 class ListInstancesHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # Queries the available instances of a function.
         self.x_fc_account_id = x_fc_account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10335,21 +10183,19 @@
 class ListInstancesRequest(TeaModel):
     def __init__(
         self,
         instance_ids: List[str] = None,
         limit: int = None,
         qualifier: str = None,
     ):
-        # The IDs of the instance.
+        # The name of the service.
         self.instance_ids = instance_ids
-        # The maximum number of resources to return. Valid values: \[0,1000].
-        # 
-        # The number of returned resources is less than or equal to the specified number.
+        # The ID of your Alibaba Cloud account.
         self.limit = limit
-        # The version or alias.
+        # The ID of the instance.
         self.qualifier = qualifier
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10378,17 +10224,15 @@
 
 class ListInstancesResponseBodyInstances(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         version_id: str = None,
     ):
-        # The ID of the instance.
         self.instance_id = instance_id
-        # The version of the service to which the instance belongs. If the instance belongs to the LATEST alias, 0 is returned as the version.
         self.version_id = version_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10412,15 +10256,15 @@
 
 
 class ListInstancesResponseBody(TeaModel):
     def __init__(
         self,
         instances: List[ListInstancesResponseBodyInstances] = None,
     ):
-        # The information about instances.
+        # 210234
         self.instances = instances
 
     def validate(self):
         if self.instances:
             for k in self.instances:
                 if k:
                     k.validate()
@@ -10666,19 +10510,16 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The time when the function is invoked. The format is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date
-        # The trace ID of the request for Function Compute API.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10715,25 +10556,19 @@
         limit: int = None,
         next_token: str = None,
         official: bool = None,
         prefix: str = None,
         public: bool = None,
         start_key: str = None,
     ):
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned configurations is less than or equal to the specified number.
         self.limit = limit
-        # The token required to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
         self.next_token = next_token
-        # Specifies whether to obtain the official public layer. When the official parameter is set to true, the public field does not take effect. The default value is false.
         self.official = official
-        # The name prefix of the layer. The names of returned resources must contain the prefix. If the name prefix is a, the names of returned resources must start with a.
         self.prefix = prefix
-        # Specifies whether to obtain only the common layer. Default value: false.
         self.public = public
-        # The name of the start layer. The returned layers are sorted in alphabetical order, and the layers that include and follow the layer specified by the startKey parameter are returned.
         self.start_key = start_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10774,17 +10609,15 @@
 
 class ListLayersResponseBody(TeaModel):
     def __init__(
         self,
         layers: List[Layer] = None,
         next_token: str = None,
     ):
-        # The information about layers.
         self.layers = layers
-        # The name of the start layer for the next query, which is also the token used to obtain more results.
         self.next_token = next_token
 
     def validate(self):
         if self.layers:
             for k in self.layers:
                 if k:
                     k.validate()
@@ -10864,19 +10697,19 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # $.parameters[8].schema.description
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # $.parameters[8].schema.example
         self.x_fc_date = x_fc_date
-        # The trace ID of the invocation request of Function Compute.
+        # $.parameters[8].schema.enumValueTitles
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10911,21 +10744,21 @@
     def __init__(
         self,
         limit: int = None,
         next_token: str = None,
         prefix: str = None,
         start_key: str = None,
     ):
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
+        # The time when Function Compute API is called.
         self.limit = limit
-        # The token used to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
+        # The ID of your Alibaba Cloud account.
         self.next_token = next_token
-        # The prefix that the names of returned resources must contain. If the name prefix is a, the names of returned resources must start with a.
+        # The returned data.
         self.prefix = prefix
-        # The returned resources are sorted in alphabetical order, and the resources that include and follow the resource specified by the startKey parameter are returned.
+        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
         self.start_key = start_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10958,17 +10791,17 @@
 
 class ListOnDemandConfigsResponseBody(TeaModel):
     def __init__(
         self,
         configs: List[OnDemandConfig] = None,
         next_token: str = None,
     ):
-        # The information about the provisioned configuration.
+        # $.parameters[9].schema.enumValueTitles
         self.configs = configs
-        # The token used to obtain more results. If this parameter is left empty, all the results are returned.
+        # {"name":"ListOnDemandConfigs","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/on-demand-configs","deprecated":0,"method":"GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"prefix\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The prefix that the names of returned resources must contain. If the name prefix is a, the names of returned resources must start with a. \",\"description\":\"The prefix that the names of returned resources must contain. If the name prefix is a, the names of returned resources must start with a. \",\"example\":\"prefix_text\"},{\"name\":\"startKey\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The returned resources are sorted in alphabetical order, and the resources that include and follow the resource specified by the startKey parameter are returned. \",\"description\":\"The returned resources are sorted in alphabetical order, and the resources that include and follow the resource specified by the startKey parameter are returned. \",\"example\":\"nextservice\"},{\"name\":\"nextToken\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The token used to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call. \",\"description\":\"The token used to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call. \",\"example\":\"8bj81uI8n****\"},{\"name\":\"limit\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"title\":\"The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number. \",\"description\":\"The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number. \",\"example\":\"20\"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. \",\"example\":\"2020-12-1210:00:00\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The trace ID of the invocation request of Function Compute. \",\"example\":\"rid281s******\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"configs\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Array\",\"subType\":\"Object\",\"example\":\"[{\"maximumInstanceCount\": 10, \"resource\": \"services/serviceName-bb7f36eb-7f1b-4c42-8f64-401b32ecbf31.aliasName/functions/functionName\"}]\",\"description\":\"The information about the on-demand configuration. \",\"children\":[{\"name\":\"resource\",\"required\":false,\"checkBlank\":false,\"visibility\":\"public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The details of the function.\",\"description\":\"The description of the resource. \",\"example\":\"123#serviceName#alias#functionName\"},{\"name\":\"maximumInstanceCount\",\"required\":false,\"checkBlank\":false,\"visibility\":\"public\",\"deprecated\":false,\"type\":\"Long\",\"title\":\"todo\",\"description\":\"The maximum number of on-demand instances. \",\"example\":\"10\"}],\"title\":\"The information about the provisioned configuration.\"},{\"name\":\"nextToken\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The token used to obtain more results. If this parameter is left empty, all the results are returned. \",\"description\":\"The token used to obtain more results. If this parameter is left empty, all the results are returned. \",\"example\":\"next_token\"}],\"title\":\"Schema of Response\",\"description\":\"The returned data. \"}","errors":"{}"}
         self.next_token = next_token
 
     def validate(self):
         if self.configs:
             for k in self.configs:
                 if k:
                     k.validate()
@@ -11048,19 +10881,19 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # The actual number of provisioned instances.
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Specifies whether to always allocate CPU to a function instance.
         self.x_fc_date = x_fc_date
-        # The trace ID of the invocation request of Function Compute.
+        # The configurations of scheduled auto scaling.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11095,21 +10928,21 @@
     def __init__(
         self,
         limit: int = None,
         next_token: str = None,
         qualifier: str = None,
         service_name: str = None,
     ):
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
+        # Queries provisioned instances.
         self.limit = limit
-        # The token used to obtain more results. You do not need to provide this parameter in the first call. The tokens for subsequent queries are obtained from the returned results.
+        # Alibaba Cloud provides SDKs for multiple programming languages to help you integrate Alibaba Cloud services by using APIs. We recommend that you use an SDK to call API operations. This frees you from manual signature verification.
         self.next_token = next_token
-        # The qualifier of the service to which resources belong. The qualifier must be aliasName and used together with the serviceName parameter.
+        # The token used to obtain more results.
         self.qualifier = qualifier
-        # The name of the service to which resources belong.
+        # It is a tool used to manage and configure Alibaba Cloud resources. After simple installation and configuration, you can use Alibaba Cloud CLI to manage multiple Alibaba Cloud services and migrate your data and business to the cloud with ease.
         self.service_name = service_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11147,27 +10980,31 @@
         current: int = None,
         current_error: str = None,
         resource: str = None,
         scheduled_actions: List[ScheduledActions] = None,
         target: int = None,
         target_tracking_policies: List[TargetTrackingPolicies] = None,
     ):
-        # Specifies whether to always allocate CPU to a function instance.
         self.always_allocate_cpu = always_allocate_cpu
-        # The actual number of provisioned instances.
+        # The expected number of provisioned instances.
         self.current = current
-        # The error message returned if a provisioned instance fails to be created.
+        # 139490
         self.current_error = current_error
-        # The description of the resource.
+        # Details about the scheduled scaling policy. You can use the scheduled scaling policy to flexibly configure provisioned instances. You can specify the number of provisioned instances to the desired value at the scheduled time. This way, the number of provisioned instances can meet the concurrency requirements of your business.
         self.resource = resource
-        # The configurations of scheduled auto scaling.
+        # The ID of your Alibaba Cloud account.
         self.scheduled_actions = scheduled_actions
-        # The expected number of provisioned instances.
+        # The configuration of metric-based auto scaling. Provisioned instances are scaled in or out every minute based on the concurrency utilization of provisioned instances. 
+        # 
+        # - If the metric value exceeds the value of the metricTarget parameter, the system scales out provisioned instances based on a progressive policy to make the metric value closer to the value of the metricTarget parameter. 
+        # - When the metric value is smaller than the value of the metricTarget parameter, the system scales in provisioned instances based on a conservative policy to make the metric value close to the value of the metricTarget parameter. 
+        # 
+        # After you specify the maximum and minimum numbers of provisioned instances, the system scales in or out provisioned instances within the range from the minimum number to the maximum number. If the number of provisioned instances is beyond the range, the scaling stops.
         self.target = target
-        # The configurations of metric-based auto scaling.
+        # Example 1
         self.target_tracking_policies = target_tracking_policies
 
     def validate(self):
         if self.scheduled_actions:
             for k in self.scheduled_actions:
                 if k:
                     k.validate()
@@ -11229,17 +11066,17 @@
 
 class ListProvisionConfigsResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         provision_configs: List[ListProvisionConfigsResponseBodyProvisionConfigs] = None,
     ):
-        # The token used to obtain more results.
+        # The qualifier of the service to which resources belong. The qualifier must be aliasName and used together with the serviceName parameter.
         self.next_token = next_token
-        # The information about provisioned instances.
+        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.provision_configs = provision_configs
 
     def validate(self):
         if self.provision_configs:
             for k in self.provision_configs:
                 if k:
                     k.validate()
@@ -11319,19 +11156,16 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The time when the Function Compute API is called. The format is **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11364,17 +11198,15 @@
 
 class ListReservedCapacitiesRequest(TeaModel):
     def __init__(
         self,
         limit: str = None,
         next_token: str = None,
     ):
-        # The maximum number of resources to return. Valid values: \[1, 100].
         self.limit = limit
-        # The token that determines the start point of the query.
         self.next_token = next_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11399,17 +11231,15 @@
 
 class ListReservedCapacitiesResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         reserved_capacities: List[OpenReservedCapacity] = None,
     ):
-        # The token used to obtain more results.
         self.next_token = next_token
-        # The information about subscription instances.
         self.reserved_capacities = reserved_capacities
 
     def validate(self):
         if self.reserved_capacities:
             for k in self.reserved_capacities:
                 if k:
                     k.validate()
@@ -11493,15 +11323,15 @@
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
         # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date
-        # The trace ID of the invocation request of Function Compute.
+        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11536,23 +11366,21 @@
     def __init__(
         self,
         direction: str = None,
         limit: int = None,
         next_token: str = None,
         start_key: str = None,
     ):
-        # The order in which the returned versions are sorted. Valid values:
-        #   - **FORWARD**: in ascending order. 
-        #   - **BACKWARD**: in descending order. This is the default value.
+        # The name of the service.
         self.direction = direction
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
-        self.limit = limit
         # The token used to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
+        self.limit = limit
+        # The description of the service version.
         self.next_token = next_token
-        # The starting position of the result list. The returned resources are sorted based on the version number, and the resources that include and follow the resource specified by the startKey parameter are returned.
+        # The time when the service version was created.
         self.start_key = start_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11587,21 +11415,20 @@
     def __init__(
         self,
         created_time: str = None,
         description: str = None,
         last_modified_time: str = None,
         version_id: str = None,
     ):
-        # The time when the service version was created.
+        # $.parameters[10].schema.enumValueTitles
         self.created_time = created_time
-        # The description of the service version.
+        # Queries all the versions of a service.
         self.description = description
-        # The time when the service version was last modified.
+        # Xiaoqi
         self.last_modified_time = last_modified_time
-        # The version of the service.
         self.version_id = version_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11635,21 +11462,19 @@
 class ListServiceVersionsResponseBody(TeaModel):
     def __init__(
         self,
         direction: str = None,
         next_token: str = None,
         versions: List[ListServiceVersionsResponseBodyVersions] = None,
     ):
-        # The order in which the returned versions are sorted. Valid values:
-        #   - **FORWARD**: in ascending order. 
-        #   - **BACKWARD**: in descending order. This is the default value.
+        # The information about the version.
         self.direction = direction
-        # The token used to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
+        # $.parameters[9].schema.description
         self.next_token = next_token
-        # The list of versions.
+        # $.parameters[9].schema.enumValueTitles
         self.versions = versions
 
     def validate(self):
         if self.versions:
             for k in self.versions:
                 if k:
                     k.validate()
@@ -12042,19 +11867,19 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # It is a tool used to manage and configure Alibaba Cloud resources. After simple installation and configuration, you can use Alibaba Cloud CLI to manage multiple Alibaba Cloud services and migrate your data and business to the cloud with ease.
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The token used to obtain more results. If this parameter is left empty, all the results are returned.
         self.x_fc_date = x_fc_date
-        # The trace ID of the request for Function Compute API.
+        # The details of returned data.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12087,17 +11912,17 @@
 
 class ListStatefulAsyncInvocationFunctionsRequest(TeaModel):
     def __init__(
         self,
         limit: int = None,
         next_token: str = None,
     ):
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
+        # The latest version of Function Compute API.
         self.limit = limit
-        # The starting position of the query. If this parameter is left empty, the query starts from the beginning. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
+        # Alibaba Cloud provides SDKs for multiple programming languages to help you integrate Alibaba Cloud services by using APIs. We recommend that you use an SDK to call API operations. This frees you from manual signature verification.
         self.next_token = next_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12122,17 +11947,17 @@
 
 class ListStatefulAsyncInvocationFunctionsResponseBody(TeaModel):
     def __init__(
         self,
         data: List[AsyncConfigMeta] = None,
         next_token: str = None,
     ):
-        # The details of returned data.
+        # The trace ID of the request for Function Compute API.
         self.data = data
-        # The token used to obtain more results. If this parameter is left empty, all the results are returned.
+        # 2022-01-28 18:04:38
         self.next_token = next_token
 
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
@@ -12215,31 +12040,28 @@
         x_fc_code_checksum: str = None,
         x_fc_date: str = None,
         x_fc_invocation_type: str = None,
         x_fc_log_type: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # It is a tool used to manage and configure Alibaba Cloud resources. After simple installation and configuration, you can use Alibaba Cloud CLI to manage multiple Alibaba Cloud services and migrate your data and business to the cloud with ease.
         self.x_fc_account_id = x_fc_account_id
-        # The CRC-64 value of the function code package. This value is used to check data integrity. The value is automatically calculated by the tool.
+        # Alibaba Cloud CLI
         self.x_fc_code_checksum = x_fc_code_checksum
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
-        self.x_fc_date = x_fc_date
-        # The invocation method. 
+        # - **true**: returns the invocationPayload parameter in the response. 
+        # - **false**: does not return the invocationPayload parameter in the response. 
         # 
-        # - **Sync**: synchronous invocation 
-        # - **Async**: asynchronous invocation
+        # > The `invocationPayload` parameter indicates the input parameters of an asynchronous task.
+        self.x_fc_date = x_fc_date
+        # The token used to obtain more results. If this parameter is left empty, all the results are returned.
         self.x_fc_invocation_type = x_fc_invocation_type
-        # The method used to return logs. Valid values: 
-        # 
-        # - **Tail**: returns the last 4 KB of logs that are generated for the current request. 
-        # - **None**: does not return logs for the current request. This is the default value.
+        # The time when Function Compute API is called.
         self.x_fc_log_type = x_fc_log_type
-        # The trace ID of the invocation request of Function Compute.
+        # The CRC-64 value of the function code package. This value is used to check data integrity. The value is automatically calculated by the tool.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12291,47 +12113,31 @@
         next_token: str = None,
         qualifier: str = None,
         sort_order_by_time: str = None,
         started_time_begin: int = None,
         started_time_end: int = None,
         status: str = None,
     ):
-        # - **true**: returns the invocationPayload parameter in the response. 
-        # - **false**: does not return the invocationPayload parameter in the response. 
-        # 
-        # > The `invocationPayload` parameter indicates the input parameters of an asynchronous task.
+        # You can search for API operations, call and debug API operations online, and dynamically generate executable sample code for SDKs.
         self.include_payload = include_payload
-        # The name prefix of the asynchronous invocation. The names of returned resources must contain the prefix. For example, if invocationidPrefix is set to job, the names of returned resources must start with job.
+        # Alibaba Cloud provides SDKs for multiple programming languages to help you integrate Alibaba Cloud services by using APIs. We recommend that you use an SDK to call API operations. This frees you from manual signature verification.
         self.invocation_id_prefix = invocation_id_prefix
-        # The maximum number of asynchronous invocations to return. Valid values: [1, 100]. Default value: 50.
+        # The list of events that trigger the asynchronous task.
         self.limit = limit
-        # The token used to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
+        # The ID of the instance that is used to run the asynchronous task.
         self.next_token = next_token
-        # The version or alias of the service to which the asynchronous task belongs.
+        # The number of retries after the asynchronous task fails.
         self.qualifier = qualifier
-        # The order in which the returned asynchronous invocations are sorted. Valid values:
-        # 
-        # - **asc**: in ascending order 
-        # - **desc**: in descending order
+        # StatefulAsyncInvocation: asynchronous task. Asynchronous tasks allow you to manage the states on the basis of common asynchronous invocations, which is more suitable for task scenarios.
         self.sort_order_by_time = sort_order_by_time
-        # The start time of the asynchronous task.
+        # The structure of the asynchronous task.
         self.started_time_begin = started_time_begin
-        # The end time of the asynchronous task.
+        # The latest version of Function Compute API.
         self.started_time_end = started_time_end
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
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12384,17 +12190,17 @@
 
 class ListStatefulAsyncInvocationsResponseBody(TeaModel):
     def __init__(
         self,
         invocations: List[StatefulAsyncInvocation] = None,
         next_token: str = None,
     ):
-        # The information about asynchronous tasks.
+        # The version or alias of the service to which the asynchronous task belongs.
         self.invocations = invocations
-        # The token used to obtain more results. If this parameter is left empty, all the results are returned.
+        # The returned data.
         self.next_token = next_token
 
     def validate(self):
         if self.invocations:
             for k in self.invocations:
                 if k:
                     k.validate()
@@ -12474,19 +12280,19 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # Queries all tagged services.
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # {"name":"ListTaggedResources","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/tags","deprecated":0,"method":"GET","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"nextToken\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The token used to obtain more results. You do not need to provide this parameter in the first call. The tokens for subsequent queries are obtained from the returned results. \",\"example\":\"a-service\"},{\"name\":\"limit\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Integer\",\"description\":\"The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number. \",\"example\":\"20\"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. Specify the time in the yyyy-mm-ddhh:mm:ss format. \",\"example\":\"2022-01-01 12:00:00\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The custom request ID. \",\"example\":\"my-test-trace-id\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"nextToken\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The token used to obtain more results. You do not need to provide this parameter in the first call. The tokens for subsequent queries are obtained from the returned results. \",\"example\":\"a-service\"},{\"name\":\"resources\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Array\",\"subType\":\"Object\",\"children\":[{\"name\":\"resourceArn\",\"required\":false,\"checkBlank\":false,\"visibility\":\"public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"resourceArn\",\"description\":\"The Alibaba Cloud Resource Name (ARN). \\n> You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource. You can manage tags only for services for top level resources. \",\"example\":\"acs:fc:cn-shanghai:188077086902****:services/demo\"},{\"name\":\"tags\",\"required\":false,\"checkBlank\":false,\"visibility\":\"public\",\"deprecated\":false,\"type\":\"Map\",\"keyType\":\"String\",\"value\":{\"type\":\"String\",\"required\":false,\"checkBlank\":false,\"visibility\":\"public\",\"deprecated\":false,\"description\":\"The tag dictionary. A tag consists of the following parameters:\\n  - **key**: the key of the tag. \\n  - **value**: the value of the tag. \",\"example\":\"{\\\"k1\\\":\\\"v1\\\" , \\\"k2\\\":\\\"v2\\\"}\"},\"title\":\"tags\",\"description\":\"The tag dictionary. \"}],\"description\":\"The information about tagged services.\"}],\"title\":\"Schema of Response\",\"description\":\"Schema of Response\"}","errors":"{}"}
         self.x_fc_date = x_fc_date
-        # The custom request ID.
+        # 147258
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12519,15 +12325,15 @@
 
 class ListTaggedResourcesRequest(TeaModel):
     def __init__(
         self,
         limit: int = None,
         next_token: str = None,
     ):
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
+        # Example 1
         self.limit = limit
         # The token used to obtain more results. You do not need to provide this parameter in the first call. The tokens for subsequent queries are obtained from the returned results.
         self.next_token = next_token
 
     def validate(self):
         pass
 
@@ -12554,17 +12360,15 @@
 
 class ListTaggedResourcesResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         resources: List[Resource] = None,
     ):
-        # The token used to obtain more results. You do not need to provide this parameter in the first call. The tokens for subsequent queries are obtained from the returned results.
         self.next_token = next_token
-        # The information about tagged services.
         self.resources = resources
 
     def validate(self):
         if self.resources:
             for k in self.resources:
                 if k:
                     k.validate()
@@ -12644,19 +12448,19 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
-        self.x_fc_account_id = x_fc_account_id
         # The time when the request is initiated on the client. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
-        self.x_fc_date = x_fc_date
+        self.x_fc_account_id = x_fc_account_id
         # The custom request ID.
+        self.x_fc_date = x_fc_date
+        # The returned data.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12691,21 +12495,21 @@
     def __init__(
         self,
         limit: int = None,
         next_token: str = None,
         prefix: str = None,
         start_key: str = None,
     ):
-        # The maximum number of resources to return. Default value: 20. Maximum value: 100. The number of returned resources is less than or equal to the specified number.
-        self.limit = limit
         # The token required to obtain more results. You do not need to provide this parameter in the first call. The tokens for subsequent queries are obtained from the returned results.
-        self.next_token = next_token
+        self.limit = limit
         # The prefix that the names of returned resources must contain.
-        self.prefix = prefix
+        self.next_token = next_token
         # The returned resources are sorted in alphabetical order, and the resources that include and follow the resource specified by the startKey parameter are returned.
+        self.prefix = prefix
+        # The ID of your Alibaba Cloud account.
         self.start_key = start_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12749,47 +12553,46 @@
         trigger_config: str = None,
         trigger_id: str = None,
         trigger_name: str = None,
         trigger_type: str = None,
         url_internet: str = None,
         url_intranet: str = None,
     ):
-        # The time when the trigger was created.
+        # The ARN of the RAM role that is used by the event source to invoke the function.
         self.created_time = created_time
-        # The description of the trigger.
+        # The unique ID of the trigger.
         self.description = description
-        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
+        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
         self.domain_name = domain_name
-        # The ARN of the RAM role that is used by the event source to invoke the function.
-        self.invocation_role = invocation_role
         # The time when the trigger was last modified.
-        self.last_modified_time = last_modified_time
+        self.invocation_role = invocation_role
         # The version or alias of the service.
-        self.qualifier = qualifier
+        self.last_modified_time = last_modified_time
         # The ARN of the event source.
-        self.source_arn = source_arn
+        self.qualifier = qualifier
         # The configurations of the trigger. The configurations vary based on the trigger type. For more information about the format, see the following topics:
         # 
         # *   OSS trigger: [OSSTriggerConfig](~~struct:OSSTriggerConfig~~).
         # *   Log Service trigger: [LogTriggerConfig](~~struct:LogTriggerConfig~~).
         # *   Time trigger: [TimeTriggerConfig](~~struct:TimeTriggerConfig~~).
         # *   HTTP trigger: [HTTPTriggerConfig](~~struct:HTTPTriggerConfig~~).
         # *   Tablestore trigger: Specify the **SourceArn** parameter and leave this parameter empty.
         # *   Alibaba Cloud CDN event trigger: [CDNEventsTriggerConfig](~~struct:CDNEventsTriggerConfig~~).
         # *   MNS topic trigger: [MnsTopicTriggerConfig](~~struct:MnsTopicTriggerConfig~~).
+        self.source_arn = source_arn
+        # The name of the trigger.
         self.trigger_config = trigger_config
-        # The unique ID of the trigger.
+        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
         self.trigger_id = trigger_id
-        # The name of the trigger.
-        self.trigger_name = trigger_name
         # The trigger type, such as **oss**, **log**, **tablestore**, **timer**, **http**, **cdn\_events**, and **mns\_topic**.
+        self.trigger_name = trigger_name
+        # The description of the trigger.
         self.trigger_type = trigger_type
-        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
-        self.url_internet = url_internet
         # The private endpoint. In a VPC, you can access HTTP triggers by using HTTP or HTTPS.
+        self.url_internet = url_internet
         self.url_intranet = url_intranet
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12858,17 +12661,17 @@
 
 class ListTriggersResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         triggers: List[ListTriggersResponseBodyTriggers] = None,
     ):
-        # The token used to obtain more results. If this parameter is left empty, all the results are returned.
-        self.next_token = next_token
         # The information about triggers.
+        self.next_token = next_token
+        # The details of the trigger.
         self.triggers = triggers
 
     def validate(self):
         if self.triggers:
             for k in self.triggers:
                 if k:
                     k.validate()
@@ -12948,19 +12751,19 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # The time when Function Compute API is called. Specify the time in the yyyy-mm-ddhh:mm:ss format.
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Example 1
         self.x_fc_date = x_fc_date
-        # The custom request ID.
+        # Queries the list of VPCs.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12992,15 +12795,14 @@
 
 
 class ListVpcBindingsResponseBody(TeaModel):
     def __init__(
         self,
         vpc_ids: List[str] = None,
     ):
-        # The IDs of bound VPCs.
         self.vpc_ids = vpc_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13075,15 +12877,15 @@
         self.common_headers = common_headers
         # The ETag value of the service. This value is used to ensure that the modified service is consistent with the service to be modified. The ETag value is returned in the responses of the [CreateService](~~175256~~), [UpdateService](~~188167~~), and [GetService](~~189225~~) operations.
         self.if_match = if_match
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
         # The start time when the function is invoked. Specify the time in the yyyy-mm-ddhh:mm:ss format.
         self.x_fc_date = x_fc_date
-        # The trace ID of the invocation request of Function Compute.
+        # 2020-12-1210:00:00
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13150,21 +12952,21 @@
     def __init__(
         self,
         created_time: str = None,
         description: str = None,
         last_modified_time: str = None,
         version_id: str = None,
     ):
-        # The time when the service version was created.
+        # The returned data.
         self.created_time = created_time
-        # The description of the service version.
+        # The creation time.
         self.description = description
-        # The time when the service version was last modified.
+        # The description of the service version.
         self.last_modified_time = last_modified_time
-        # The version of the service.
+        # The last update time.
         self.version_id = version_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13244,19 +13046,19 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # The name of the service.
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The creation time.
         self.x_fc_date = x_fc_date
-        # The trace ID of the invocation request of Function Compute.
+        # The maximum number of retries allowed after an asynchronous invocation fails. Default value: 3. Valid values: 0 to 8.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13292,26 +13094,23 @@
         self,
         destination_config: DestinationConfig = None,
         max_async_event_age_in_seconds: int = None,
         max_async_retry_attempts: int = None,
         stateful_invocation: bool = None,
         qualifier: str = None,
     ):
-        # The configuration structure of the destination for asynchronous invocation.
+        # You can search for API operations, call and debug API operations online, and dynamically generate executable sample code for SDKs.
         self.destination_config = destination_config
-        # The maximum validity period of messages. Valid values: 1 to 2592000. Unit: seconds.
+        # Alibaba Cloud CLI
         self.max_async_event_age_in_seconds = max_async_event_age_in_seconds
-        # The maximum number of retries allowed after an asynchronous invocation fails. Default value: 3. Valid values: 0 to 8.
+        # The information about the asynchronous invocation configuration.
         self.max_async_retry_attempts = max_async_retry_attempts
-        # Specifies whether to enable the asynchronous task feature. 
-        # 
-        # - **true**: enables the asynchronous task feature. 
-        # - **false**: does not enable the asynchronous task feature.
-        self.stateful_invocation = stateful_invocation
         # The version or alias of the service.
+        self.stateful_invocation = stateful_invocation
+        # The latest version of Function Compute API.
         self.qualifier = qualifier
 
     def validate(self):
         if self.destination_config:
             self.destination_config.validate()
 
     def to_map(self):
@@ -13357,34 +13156,37 @@
         last_modified_time: str = None,
         max_async_event_age_in_seconds: int = None,
         max_async_retry_attempts: int = None,
         qualifier: str = None,
         service: str = None,
         stateful_invocation: bool = None,
     ):
-        # The creation time.
+        # Sat, 14 Jul 2017 07:02:38 GMT
         self.created_time = created_time
-        # The configuration structure of the destination for asynchronous invocation.
+        # The trace ID of the invocation request of Function Compute.
         self.destination_config = destination_config
         # The name of the function.
         self.function = function
-        # The time when the configuration was last modified.
+        # The configuration structure of the destination for asynchronous invocation.
         self.last_modified_time = last_modified_time
-        # The maximum validity period of messages.
+        # Specifies whether to enable the asynchronous task feature. 
+        # 
+        # - **true**: enables the asynchronous task feature. 
+        # - **false**: does not enable the asynchronous task feature.
         self.max_async_event_age_in_seconds = max_async_event_age_in_seconds
-        # The maximum number of retries allowed after an asynchronous invocation fails.
+        # The ID of your Alibaba Cloud account.
         self.max_async_retry_attempts = max_async_retry_attempts
-        # The qualifier.
-        self.qualifier = qualifier
-        # The name of the service.
-        self.service = service
         # Specifies whether to enable the asynchronous task feature. 
         # 
         # - **true**: enables the asynchronous task feature. 
         # - **false**: does not enable the asynchronous task feature.
+        self.qualifier = qualifier
+        # Creates or modifies an asynchronous invocation configuration for a function.
+        self.service = service
+        # Jianyi
         self.stateful_invocation = stateful_invocation
 
     def validate(self):
         if self.destination_config:
             self.destination_config.validate()
 
     def to_map(self):
@@ -13487,21 +13289,21 @@
         common_headers: Dict[str, str] = None,
         if_match: str = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # If the ETag specified in the request matches the ETag value of the OndemandConfig, FC returns 200 OK. If the ETag specified in the request does not match the ETag value of the object, FC returns 412 Precondition Failed.
+        # The name of the service.
         self.if_match = if_match
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The start time when the function is invoked. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # Example 1
         self.x_fc_date = x_fc_date
-        # The trace ID of the request for Function Compute API, which is also the unique ID of the request.
+        # Creates function rules.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13538,17 +13340,17 @@
 
 class PutFunctionOnDemandConfigRequest(TeaModel):
     def __init__(
         self,
         maximum_instance_count: int = None,
         qualifier: str = None,
     ):
-        # The maximum number of on-demand instances. For more information, see [Instance scaling limits](~~185038~~).
+        # The maximum number of instances.
         self.maximum_instance_count = maximum_instance_count
-        # The alias of the service or LATEST.
+        # The trace ID of the request for Function Compute API, which is also the unique ID of the request.
         self.qualifier = qualifier
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13573,17 +13375,15 @@
 
 class PutFunctionOnDemandConfigResponseBody(TeaModel):
     def __init__(
         self,
         maximum_instance_count: int = None,
         resource: str = None,
     ):
-        # The maximum number of instances.
         self.maximum_instance_count = maximum_instance_count
-        # The description of the resource.
         self.resource = resource
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13655,19 +13455,16 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The time when the operation is called. The format is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date
-        # The trace ID of the request for Function Compute API.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13699,18 +13496,14 @@
 
 
 class PutLayerACLRequest(TeaModel):
     def __init__(
         self,
         public: bool = None,
     ):
-        # Specifies whether the layer is public.
-        # 
-        # *   **true**: Public.
-        # *   **false**: Not public.
         self.public = public
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14013,19 +13806,17 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
+        # Jianyi
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date
-        # The trace ID of the invocation request of Function Compute.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14058,17 +13849,17 @@
 
 class RegisterEventSourceRequest(TeaModel):
     def __init__(
         self,
         source_arn: str = None,
         qualifier: str = None,
     ):
-        # The Alibaba Cloud Resource Name (ARN) of the event source.
+        # {"name":"RegisterEventSource","product":"FC-Open","version":"2021-04-06","path":"/2021-04-06/services/{serviceName}/functions/{functionName}/event-sources","deprecated":0,"method":"POST","protocol":"HTTP|HTTPS","hidden":0,"timeout":10000,"parameter_type":"Single","params":"[{\"name\":\"serviceName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the service.\",\"description\":\"The name of the service. \",\"example\":\"demo-service\"},{\"name\":\"functionName\",\"position\":\"Path\",\"required\":true,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The name of the function.\",\"description\":\"The name of the function. \",\"example\":\"demo-function\"},{\"name\":\"qualifier\",\"position\":\"Query\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The version or alias of the service.\",\"description\":\"The version or alias of the service. \",\"example\":\"LATEST\"},{\"name\":\"body\",\"position\":\"Body\",\"style\":\"json\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"Object\",\"params\":[{\"name\":\"sourceArn\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The Alibaba Cloud Resource Name (ARN) of the event source.\",\"description\":\"The Alibaba Cloud Resource Name (ARN) of the event source.\",\"example\":\"acs:eventbridge:cn-shanghai:123456:eventbus/mns-test/rule/fc-test1/target/abc\"}],\"description\":\"The body of the request. \"},{\"name\":\"X-Fc-Account-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The ID of your Alibaba Cloud account. \",\"example\":\"188077086902****\"},{\"name\":\"X-Fc-Date\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The time when Function Compute API is called. \",\"example\":\"Sat, 14 Jul 2017 07:02:38 GMT\"},{\"name\":\"X-Fc-Trace-Id\",\"position\":\"Header\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"description\":\"The trace ID of the invocation request of Function Compute. \",\"example\":\"asdf****\"}]","response_headers":"[]","response":"{\"type\":\"Object\",\"children\":[{\"name\":\"sourceArn\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The Alibaba Cloud Resource Name (ARN) of the event source.\",\"description\":\"The ARN of the event source. \",\"example\":\"acs:eventbridge:cn-shanghai:123456:eventbus/mns-test/rule/fc-test1/target/abc\"},{\"name\":\"createdTime\",\"required\":false,\"checkBlank\":false,\"visibility\":\"Public\",\"deprecated\":false,\"type\":\"String\",\"title\":\"The creation time.\",\"description\":\"The time when the event source was created. \",\"example\":\"2016-08-15T16:06:05.000+0000\"}],\"title\":\"Schema of Response\",\"description\":\"The returned data. \"}","body_style":"json","errors":"{}"}
         self.source_arn = source_arn
-        # The version or alias of the service.
+        # asdf****\
         self.qualifier = qualifier
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14093,17 +13884,15 @@
 
 class RegisterEventSourceResponseBody(TeaModel):
     def __init__(
         self,
         created_time: str = None,
         source_arn: str = None,
     ):
-        # The time when the event source was created.
         self.created_time = created_time
-        # The ARN of the event source.
         self.source_arn = source_arn
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14175,19 +13964,16 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The time when the function is invoked. The format of the value is: EEE,d MMM yyyy HH:mm:ss GMT.
         self.x_fc_date = x_fc_date
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14367,19 +14153,16 @@
         self,
         common_headers: Dict[str, str] = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The time when the function is invoked. The format is **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date
-        # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14412,19 +14195,15 @@
 
 class TagResourceRequest(TeaModel):
     def __init__(
         self,
         resource_arn: str = None,
         tags: Dict[str, str] = None,
     ):
-        # The ARN of the resource.
-        # 
-        # > You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource. You can manage tags only for services for top level resources.
         self.resource_arn = resource_arn
-        # The tag dictionary.
         self.tags = tags
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14488,15 +14267,15 @@
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The time when Function Compute API is called. Specify the time in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
+        # The time when the function is invoked. The value is in the **EEE,d MMM yyyy HH:mm:ss GMT** format.
         self.x_fc_date = x_fc_date
         # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
@@ -14533,18 +14312,19 @@
     def __init__(
         self,
         all: bool = None,
         resource_arn: str = None,
         tag_keys: List[str] = None,
     ):
         # Specifies whether to remove all tags. This parameter takes effect only when no tag key is specified. Valid values:
-        #   - **true**: removes all tags. 
-        #   - **false**: does not remove all tags.
+        # 
+        # *   **true**\
+        # *   **false**\
         self.all = all
-        # The ARN of the resource. 
+        # The Alibaba Cloud Resource Name (ARN) of the resource.
         # 
         # > You can use the value of this parameter to query the information about the resource, such as the account, service, and region information of the resource. You can manage tags only for services for top level resources.
         self.resource_arn = resource_arn
         # The keys of the tags that you want to remove.
         self.tag_keys = tag_keys
 
     def validate(self):
@@ -14671,17 +14451,17 @@
         self,
         additional_version_weight: Dict[str, float] = None,
         description: str = None,
         resolve_policy: str = None,
         route_policy: RoutePolicy = None,
         version_id: str = None,
     ):
-        # The canary release version to which the alias points and the weight of the canary release version.
+        # The additional version to which the alias points and the weight of the additional version.
         # 
-        # *   The canary release version takes effect only when the function is invoked.
+        # *   The additional version takes effect only when the function is invoked.
         # *   The value consists of a version number and a specific weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
         self.additional_version_weight = additional_version_weight
         # The description of the alias.
         self.description = description
         # The canary release mode. Valid values:
         # 
         # *   **Random**: random canary release. This is the default value.
@@ -14736,17 +14516,17 @@
         additional_version_weight: Dict[str, float] = None,
         alias_name: str = None,
         created_time: str = None,
         description: str = None,
         last_modified_time: str = None,
         version_id: str = None,
     ):
-        # The canary release version to which the alias points and the weight of the canary release version.
+        # The additional version to which the alias points and the weight of the additional version.
         # 
-        # *   The canary release version takes effect only when the function is invoked.
+        # *   The additional version takes effect only when the function is invoked.
         # *   The value consists of a version number and a specific weight. For example, 2:0.05 indicates that when a function is invoked, Version 2 is the canary release version, 5% of the traffic is distributed to the canary release version, and 95% of the traffic is distributed to the major version.
         self.additional_version_weight = additional_version_weight
         # The name of the alias.
         self.alias_name = alias_name
         # The time when the alias was created.
         self.created_time = created_time
         # The description of the alias.
@@ -15116,23 +14896,18 @@
         if_match: str = None,
         x_fc_account_id: str = None,
         x_fc_code_checksum: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # The parameter that is used to ensure that the modified resource is consistent with the resource to be modified. The value of this parameter is returned in the responses of the [CreateFunction](~~415747~~), [GetFunction](~~415750~~), and [UpdateFunction](~~415749~~) operations.
         self.if_match = if_match
-        # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The CRC-64 value of the function code package.
         self.x_fc_code_checksum = x_fc_code_checksum
-        # The time on which the function is invoked. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date
-        # The trace ID of the request. The value is the same as that of the requestId parameter in the response.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15193,70 +14968,35 @@
         instance_soft_concurrency: int = None,
         instance_type: str = None,
         layers: List[str] = None,
         memory_size: int = None,
         runtime: str = None,
         timeout: int = None,
     ):
-        # The number of requests that can be concurrently processed by a single instance.
         self.instance_concurrency = instance_concurrency
-        # The port on which the HTTP server listens for the custom runtime or custom container runtime.
         self.ca_port = ca_port
-        # The packaged code of the function. **Function code packages** can be provided with the following two methods. You must use only one of the methods in a request.
-        # 
-        # *   Specify the name of the Object Storage Service (OSS) bucket and object where the code package is stored. The names are specified in the **ossBucketName** and **ossObjectName** parameters.
-        # *   Specify the Base64-encoded content of the ZIP file by using the **zipFile** parameter.
         self.code = code
-        # The number of vCPUs of the function. The value must be a multiple of 0.05.
         self.cpu = cpu
-        # The configuration of the custom container. After you configure the custom container, Function Compute can execute the function in a container created from a custom image.
         self.custom_container_config = custom_container_config
-        # The custom DNS configurations of the function.
         self.custom_dns = custom_dns
-        # The custom health check configurations of the function. This parameter is applicable to only custom runtimes and custom containers.
         self.custom_health_check_config = custom_health_check_config
-        # The configurations of the custom runtime.
         self.custom_runtime_config = custom_runtime_config
-        # The description of the function.
         self.description = description
-        # The disk size of the function. Unit: MB. Valid values: 512 and 10240.
         self.disk_size = disk_size
-        # The environment variables that are configured for the function. You can obtain the values of the environment variables from the function. For more information, see [Environment variables](~~69777~~).
         self.environment_variables = environment_variables
-        # The GPU memory capacity for the function. Unit: MB. The value must be a multiple of 1,024.
         self.gpu_memory_size = gpu_memory_size
-        # The handler of the function. The format varies based on the programming language. For more information, see [Function handlers](~~157704~~).
         self.handler = handler
-        # The timeout period for the execution of the Initializer hook. Unit: seconds. Default value: 3. Minimum value: 1. When the period ends, the execution of the Initializer hook is terminated.
         self.initialization_timeout = initialization_timeout
-        # The handler of the Initializer hook. The format is determined by the programming language. For more information, see [Function handlers](~~157704~~).
         self.initializer = initializer
-        # The lifecycle configurations of the instance.
         self.instance_lifecycle_config = instance_lifecycle_config
-        # The soft concurrency of the instance. You can use this parameter to implement graceful scale-up of instances. If the number of concurrent requests on an instance is greater than the value of soft concurrency, an instance scale-up is triggered. For example, if your instance requires a long time to start, you can specify a suitable soft concurrency to start the instance in advance.
-        # 
-        # The value must be less than or equal to that of the **instanceConcurrency** parameter.
         self.instance_soft_concurrency = instance_soft_concurrency
-        # The instance type of the function. Valid values:
-        # 
-        # *   **e1**: elastic instance
-        # *   **c1**: performance instance
-        # *   **fc.gpu.tesla.1**: GPU-accelerated instance (Tesla T4)
-        # *   **fc.gpu.ampere.1**: GPU-accelerated instance (Ampere A10)
-        # *   **g1**: same as **fc.gpu.tesla.1**\
         self.instance_type = instance_type
-        # The information about layers.
-        # 
-        # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name as a layer with a larger subscript.
         self.layers = layers
-        # The memory size for the function. Unit: MB. The memory size must be a multiple of 64. The memory size varies based on the function instance type. For more information, see [Instance types](~~179379~~).
         self.memory_size = memory_size
-        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom** and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
         self.runtime = runtime
-        # The timeout period for the execution of the function. Unit: seconds. Default value: 3. Minimum value: 1. When the period ends, the execution of the function is terminated.
         self.timeout = timeout
 
     def validate(self):
         if self.code:
             self.code.validate()
         if self.custom_container_config:
             self.custom_container_config.validate()
@@ -15403,77 +15143,40 @@
         instance_type: str = None,
         last_modified_time: str = None,
         layers: List[str] = None,
         memory_size: int = None,
         runtime: str = None,
         timeout: int = None,
     ):
-        # The port on which the HTTP server listens for the custom runtime or custom container runtime.
         self.ca_port = ca_port
-        # The CRC-64 value of the function code package.
         self.code_checksum = code_checksum
-        # The size of the function code package that is returned by the system. Unit: bytes.
         self.code_size = code_size
-        # The number of vCPUs of the function. The value must be a multiple of 0.05.
         self.cpu = cpu
-        # The time when the function was created.
         self.created_time = created_time
-        # The configurations of the custom container runtime. After you configure the custom container runtime, Function Compute can execute the function in a container created from a custom image.
         self.custom_container_config = custom_container_config
-        # The custom DNS configurations of the function.
         self.custom_dns = custom_dns
-        # The custom health check configuration of the function. This parameter is applicable only to custom runtimes and custom containers.
         self.custom_health_check_config = custom_health_check_config
-        # The configurations of the custom runtime.
         self.custom_runtime_config = custom_runtime_config
-        # The description of the function.
         self.description = description
-        # The disk size of the function. Unit: MB. Valid values: 512 and 10240.
         self.disk_size = disk_size
-        # The environment variables that are configured for the function. You can obtain the values of the environment variables from the function. For more information, see [Environment variables](~~69777~~).
         self.environment_variables = environment_variables
-        # The unique ID that is generated by the system for the function.
         self.function_id = function_id
-        # The name of the function.
         self.function_name = function_name
-        # The GPU memory capacity for the function. Unit: MB. The value must be a multiple of 1,024.
         self.gpu_memory_size = gpu_memory_size
-        # The handler of the function.
         self.handler = handler
-        # The timeout period for the execution of the Initializer hook. Unit: seconds. Default value: 3. Minimum value: 1. When the period ends, the execution of the Initializer hook is terminated.
         self.initialization_timeout = initialization_timeout
-        # The handler of the Initializer hook. The format is determined by the programming language.
         self.initializer = initializer
-        # The number of requests that can be concurrently processed by a single instance.
         self.instance_concurrency = instance_concurrency
-        # The lifecycle configurations of the instance.
         self.instance_lifecycle_config = instance_lifecycle_config
-        # The soft concurrency of the instance. You can use this parameter to implement graceful scale-up of instances. If the number of concurrent requests on an instance is greater than the value of soft concurrency, an instance scale-up is triggered. For example, if your instance requires a long time to start, you can specify a suitable soft concurrency to start the instance in advance.
-        # 
-        # The value must be less than or equal to that of the **instanceConcurrency** parameter.
         self.instance_soft_concurrency = instance_soft_concurrency
-        # The instance type of the function. Valid values:
-        # 
-        # *   **e1**: elastic instance
-        # *   **c1**: performance instance
-        # *   **fc.gpu.tesla.1**: GPU-accelerated instance (Tesla T4)
-        # *   **fc.gpu.ampere.1**: GPU-accelerated instance (Ampere A10)
-        # *   **g1**: same as **fc.gpu.tesla.1**\
         self.instance_type = instance_type
-        # The time when the function was last modified.
         self.last_modified_time = last_modified_time
-        # An array that consists of the information of layers.
-        # 
-        # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name as a layer with a larger subscript.
         self.layers = layers
-        # The memory size that is configured for the function. Unit: MB.
         self.memory_size = memory_size
-        # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom** and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
         self.runtime = runtime
-        # The timeout period for the execution. Unit: seconds.
         self.timeout = timeout
 
     def validate(self):
         if self.custom_container_config:
             self.custom_container_config.validate()
         if self.custom_dns:
             self.custom_dns.validate()
@@ -15981,21 +15684,21 @@
         common_headers: Dict[str, str] = None,
         if_match: str = None,
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
-        # This parameter is used to ensure that the modified resource is consistent with the resource to be modified. You can obtain the parameter value from the responses of [CreateTrigger](~~190054~~), [GetTrigger](~~190056~~), and [UpdateTrigger](~~190055~~) operations.
+        # The name of the service.
         self.if_match = if_match
-        # The ID of your Alibaba Cloud account.
-        self.x_fc_account_id = x_fc_account_id
         # The time when the request is initiated on the client. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
-        self.x_fc_date = x_fc_date
+        self.x_fc_account_id = x_fc_account_id
         # The custom request ID.
+        self.x_fc_date = x_fc_date
+        # The ETag that is used to modify the trigger. This parameter is used to ensure that the modified trigger is consistent with the trigger to be modified.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16034,29 +15737,29 @@
     def __init__(
         self,
         description: str = None,
         invocation_role: str = None,
         qualifier: str = None,
         trigger_config: str = None,
     ):
-        # The description of the trigger.
+        # The ID of your Alibaba Cloud account.
         self.description = description
-        # The role that is used by the event source such as OSS to invoke the function. For more information, see [Overview](~~53102~~).
-        self.invocation_role = invocation_role
         # The version or alias of the service.
-        self.qualifier = qualifier
+        self.invocation_role = invocation_role
         # The configurations of the trigger. The configurations vary based on the trigger type. For more information about the format, see the following topics:
         # 
         # *   OSS trigger: [OSSTriggerConfig](~~struct:OSSTriggerConfig~~).
         # *   Log Service trigger: [LogTriggerConfig](~~struct:LogTriggerConfig~~).
         # *   Time trigger: [TimeTriggerConfig](~~struct:TimeTriggerConfig~~).
         # *   HTTP trigger: [HTTPTriggerConfig](~~struct:HTTPTriggerConfig~~).
         # *   Tablestore trigger: Specify the **SourceArn** parameter and leave this parameter empty.
         # *   Alibaba Cloud CDN event trigger: [CDNEventsTriggerConfig](~~struct:CDNEventsTriggerConfig~~).
         # *   MNS topic trigger: [MnsTopicTriggerConfig](~~struct:MnsTopicTriggerConfig~~).
+        self.qualifier = qualifier
+        # The description of the trigger.
         self.trigger_config = trigger_config
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16100,39 +15803,38 @@
         trigger_config: str = None,
         trigger_id: str = None,
         trigger_name: str = None,
         trigger_type: str = None,
         url_internet: str = None,
         url_intranet: str = None,
     ):
-        # The time when the audio or video file was created.
+        # The ARN of the RAM role that is used by the event source to invoke the function.
         self.created_time = created_time
-        # The description of the trigger.
+        # The unique ID of the trigger.
         self.description = description
-        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
+        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
         self.domain_name = domain_name
-        # The ARN of the RAM role that is used by the event source to invoke the function.
-        self.invocation_role = invocation_role
         # The last modification time.
-        self.last_modified_time = last_modified_time
+        self.invocation_role = invocation_role
         # The version or alias of the service.
-        self.qualifier = qualifier
+        self.last_modified_time = last_modified_time
         # The ARN of the event source.
-        self.source_arn = source_arn
+        self.qualifier = qualifier
         # The configurations of the trigger. The configurations vary based on the trigger type.
+        self.source_arn = source_arn
+        # The name of the trigger.
         self.trigger_config = trigger_config
-        # The unique ID of the trigger.
+        # The domain name used to invoke the function by using HTTP. You can add this domain name as the prefix to the endpoint of Function Compute. This way, you can invoke the function that corresponds to the trigger by using HTTP. For example, `{domainName}.cn-shanghai.fc.aliyuncs.com`.
         self.trigger_id = trigger_id
-        # The name of the trigger.
-        self.trigger_name = trigger_name
         # The trigger type, such as **oss**, **log**, **tablestore**, **timer**, **http**, **cdn_events**, and **mns_topic**.
+        self.trigger_name = trigger_name
+        # The description of the trigger.
         self.trigger_type = trigger_type
-        # The public domain address. You can access HTTP triggers over the Internet by using HTTP or HTTPS.
-        self.url_internet = url_internet
         # The private endpoint. In a VPC, you can access HTTP triggers by using HTTP or HTTPS.
+        self.url_internet = url_internet
         self.url_intranet = url_intranet
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/PKG-INFO` & `alibabacloud_fc-open20210406-2.0.9/alibabacloud_fc_open20210406.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-fc-open20210406
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud FC-Open (20210406) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc-open20210406-2.0.8/setup.py` & `alibabacloud_fc-open20210406-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_fc-open20210406.
 
-Created on 11/04/2023
+Created on 30/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_fc_open20210406"
 NAME = "alibabacloud_fc-open20210406" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud FC-Open (20210406) SDK Library for Python"
```

