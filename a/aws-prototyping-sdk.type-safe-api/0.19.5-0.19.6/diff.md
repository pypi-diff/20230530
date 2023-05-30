# Comparing `tmp/aws_prototyping_sdk.type_safe_api-0.19.5.tar.gz` & `tmp/aws_prototyping_sdk.type_safe_api-0.19.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.19.5.tar", last modified: Tue May 30 03:06:14 2023, max compression
+gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.19.6.tar", last modified: Tue May 30 03:52:39 2023, max compression
```

## Comparing `aws_prototyping_sdk.type_safe_api-0.19.5.tar` & `aws_prototyping_sdk.type_safe_api-0.19.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:06:14.735804 aws_prototyping_sdk.type_safe_api-0.19.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    65065 2023-05-30 03:06:14.731804 aws_prototyping_sdk.type_safe_api-0.19.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    64124 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 03:06:14.735804 aws_prototyping_sdk.type_safe_api-0.19.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:06:14.723804 aws_prototyping_sdk.type_safe_api-0.19.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:06:14.727804 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:06:14.731804 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/type_safe_api/
--rw-r--r--   0 runner    (1001) docker     (123)   615180 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/type_safe_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:06:14.731804 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/type_safe_api/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   973612 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.19.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/type_safe_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:06:14.727804 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    65065 2023-05-30 03:06:14.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-30 03:06:14.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 03:06:14.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 03:06:14.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 03:06:14.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:52:39.519909 aws_prototyping_sdk.type_safe_api-0.19.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    65065 2023-05-30 03:52:39.519909 aws_prototyping_sdk.type_safe_api-0.19.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    64124 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 03:52:39.519909 aws_prototyping_sdk.type_safe_api-0.19.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:52:39.511908 aws_prototyping_sdk.type_safe_api-0.19.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:52:39.511908 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:52:39.519909 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/
+-rw-r--r--   0 runner    (1001) docker     (123)   624082 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:52:39.519909 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   979031 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.19.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 03:52:20.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:52:39.515909 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    65065 2023-05-30 03:52:39.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-30 03:52:39.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 03:52:39.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 03:52:39.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 03:52:39.000000 aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.5/LICENSE` & `aws_prototyping_sdk.type_safe_api-0.19.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.5/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.19.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.type_safe_api
-Version: 0.19.5
+Version: 0.19.6
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.5/README.md` & `aws_prototyping_sdk.type_safe_api-0.19.6/README.md`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.5/setup.py` & `aws_prototyping_sdk.type_safe_api-0.19.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.type_safe_api",
-    "version": "0.19.5",
+    "version": "0.19.6",
     "description": "@aws-prototyping-sdk/type-safe-api",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_prototyping_sdk.type_safe_api",
         "aws_prototyping_sdk.type_safe_api._jsii"
     ],
     "package_data": {
         "aws_prototyping_sdk.type_safe_api._jsii": [
-            "type-safe-api@0.19.5.jsii.tgz"
+            "type-safe-api@0.19.6.jsii.tgz"
         ],
         "aws_prototyping_sdk.type_safe_api": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/type_safe_api/__init__.py` & `aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk/type_safe_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2305,14 +2305,76 @@
 
     def __repr__(self) -> str:
         return "ApiGatewayIntegrationTlsConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+@jsii.data_type(
+    jsii_type="@aws-prototyping-sdk/type-safe-api.ApiKeyOptions",
+    jsii_struct_bases=[],
+    name_mapping={"source": "source", "required_by_default": "requiredByDefault"},
+)
+class ApiKeyOptions:
+    def __init__(
+        self,
+        *,
+        source: _aws_cdk_aws_apigateway_ceddda9d.ApiKeySourceType,
+        required_by_default: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''(experimental) Options for API keys.
+
+        :param source: (experimental) Source type for an API key.
+        :param required_by_default: (experimental) Set to true to require an API key on all operations by default. Only applicable when the source is HEADER.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__cd712e0b528a2a814e998fe599840c879dcf57fc7aea3ad93aea819af03fee2a)
+            check_type(argname="argument source", value=source, expected_type=type_hints["source"])
+            check_type(argname="argument required_by_default", value=required_by_default, expected_type=type_hints["required_by_default"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "source": source,
+        }
+        if required_by_default is not None:
+            self._values["required_by_default"] = required_by_default
+
+    @builtins.property
+    def source(self) -> _aws_cdk_aws_apigateway_ceddda9d.ApiKeySourceType:
+        '''(experimental) Source type for an API key.
+
+        :stability: experimental
+        '''
+        result = self._values.get("source")
+        assert result is not None, "Required property 'source' is missing"
+        return typing.cast(_aws_cdk_aws_apigateway_ceddda9d.ApiKeySourceType, result)
+
+    @builtins.property
+    def required_by_default(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Set to true to require an API key on all operations by default.
+
+        Only applicable when the source is HEADER.
+
+        :stability: experimental
+        '''
+        result = self._values.get("required_by_default")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "ApiKeyOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class Authorizer(
     metaclass=jsii.JSIIAbstractClass,
     jsii_type="@aws-prototyping-sdk/type-safe-api.Authorizer",
 ):
     '''(experimental) An authorizer for authorizing API requests.
 
     :stability: experimental
@@ -5478,43 +5540,54 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
     jsii_type="@aws-prototyping-sdk/type-safe-api.TypeSafeApiIntegration",
     jsii_struct_bases=[],
-    name_mapping={"integration": "integration", "authorizer": "authorizer"},
+    name_mapping={
+        "integration": "integration",
+        "authorizer": "authorizer",
+        "options": "options",
+    },
 )
 class TypeSafeApiIntegration:
     def __init__(
         self,
         *,
         integration: Integration,
         authorizer: typing.Optional[Authorizer] = None,
+        options: typing.Optional[typing.Union["TypeSafeApiIntegrationOptions", typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''(experimental) Defines an integration for an individual API operation.
 
-        :param integration: (experimental) The lambda function to service the api operation.
+        :param integration: (experimental) The integration to service the api operation.
         :param authorizer: (experimental) The authorizer to use for this api operation (overrides the default).
+        :param options: (experimental) Options for the integration.
 
         :stability: experimental
         '''
+        if isinstance(options, dict):
+            options = TypeSafeApiIntegrationOptions(**options)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6aac208a4d52a45aa5a05fdd9df9236f624116cf700032ca2ec93451ea1ee14c)
             check_type(argname="argument integration", value=integration, expected_type=type_hints["integration"])
             check_type(argname="argument authorizer", value=authorizer, expected_type=type_hints["authorizer"])
+            check_type(argname="argument options", value=options, expected_type=type_hints["options"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "integration": integration,
         }
         if authorizer is not None:
             self._values["authorizer"] = authorizer
+        if options is not None:
+            self._values["options"] = options
 
     @builtins.property
     def integration(self) -> Integration:
-        '''(experimental) The lambda function to service the api operation.
+        '''(experimental) The integration to service the api operation.
 
         :stability: experimental
         '''
         result = self._values.get("integration")
         assert result is not None, "Required property 'integration' is missing"
         return typing.cast(Integration, result)
 
@@ -5523,26 +5596,85 @@
         '''(experimental) The authorizer to use for this api operation (overrides the default).
 
         :stability: experimental
         '''
         result = self._values.get("authorizer")
         return typing.cast(typing.Optional[Authorizer], result)
 
+    @builtins.property
+    def options(self) -> typing.Optional["TypeSafeApiIntegrationOptions"]:
+        '''(experimental) Options for the integration.
+
+        :stability: experimental
+        '''
+        result = self._values.get("options")
+        return typing.cast(typing.Optional["TypeSafeApiIntegrationOptions"], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
         return "TypeSafeApiIntegration(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+@jsii.data_type(
+    jsii_type="@aws-prototyping-sdk/type-safe-api.TypeSafeApiIntegrationOptions",
+    jsii_struct_bases=[],
+    name_mapping={"api_key_required": "apiKeyRequired"},
+)
+class TypeSafeApiIntegrationOptions:
+    def __init__(
+        self,
+        *,
+        api_key_required: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''(experimental) Options for an integration.
+
+        :param api_key_required: (experimental) Require an API key to invoke this operation. Overrides the default setting if present. This is only applicable when the API key source is HEADER. Default: false
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__dd841177be00ab24afd6ef8e8d79684af4aa8a6d71e19911ed314e4324e4a377)
+            check_type(argname="argument api_key_required", value=api_key_required, expected_type=type_hints["api_key_required"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if api_key_required is not None:
+            self._values["api_key_required"] = api_key_required
+
+    @builtins.property
+    def api_key_required(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Require an API key to invoke this operation.
+
+        Overrides the default setting if present.
+        This is only applicable when the API key source is HEADER.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("api_key_required")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "TypeSafeApiIntegrationOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class TypeSafeApiModelProject(
     _projen_04054675.Project,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-prototyping-sdk/type-safe-api.TypeSafeApiModelProject",
 ):
     '''
     :stability: experimental
@@ -5931,48 +6063,56 @@
 
 @jsii.data_type(
     jsii_type="@aws-prototyping-sdk/type-safe-api.TypeSafeApiOptions",
     jsii_struct_bases=[],
     name_mapping={
         "integrations": "integrations",
         "operation_lookup": "operationLookup",
+        "api_key_options": "apiKeyOptions",
         "cors_options": "corsOptions",
         "default_authorizer": "defaultAuthorizer",
     },
 )
 class TypeSafeApiOptions:
     def __init__(
         self,
         *,
         integrations: typing.Mapping[builtins.str, typing.Union[TypeSafeApiIntegration, typing.Dict[builtins.str, typing.Any]]],
         operation_lookup: typing.Mapping[builtins.str, typing.Union[OperationDetails, typing.Dict[builtins.str, typing.Any]]],
+        api_key_options: typing.Optional[typing.Union[ApiKeyOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         cors_options: typing.Optional[typing.Union[_aws_cdk_aws_apigateway_ceddda9d.CorsOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         default_authorizer: typing.Optional[Authorizer] = None,
     ) -> None:
         '''(experimental) Options required alongside an Open API specification to create API Gateway resources.
 
         :param integrations: (experimental) A mapping of API operation to its integration.
         :param operation_lookup: (experimental) Details about each operation.
+        :param api_key_options: (experimental) Options for API keys.
         :param cors_options: (experimental) Cross Origin Resource Sharing options for the API.
         :param default_authorizer: (experimental) The default authorizer to use for your api. When omitted, no default authorizer is used. Authorizers specified at the integration level will override this for that operation.
 
         :stability: experimental
         '''
+        if isinstance(api_key_options, dict):
+            api_key_options = ApiKeyOptions(**api_key_options)
         if isinstance(cors_options, dict):
             cors_options = _aws_cdk_aws_apigateway_ceddda9d.CorsOptions(**cors_options)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ddffe68493ea33b13b142dd3a74d4b71e0e9eb563dc8d340916de145a0d0dfd3)
             check_type(argname="argument integrations", value=integrations, expected_type=type_hints["integrations"])
             check_type(argname="argument operation_lookup", value=operation_lookup, expected_type=type_hints["operation_lookup"])
+            check_type(argname="argument api_key_options", value=api_key_options, expected_type=type_hints["api_key_options"])
             check_type(argname="argument cors_options", value=cors_options, expected_type=type_hints["cors_options"])
             check_type(argname="argument default_authorizer", value=default_authorizer, expected_type=type_hints["default_authorizer"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "integrations": integrations,
             "operation_lookup": operation_lookup,
         }
+        if api_key_options is not None:
+            self._values["api_key_options"] = api_key_options
         if cors_options is not None:
             self._values["cors_options"] = cors_options
         if default_authorizer is not None:
             self._values["default_authorizer"] = default_authorizer
 
     @builtins.property
     def integrations(self) -> typing.Mapping[builtins.str, TypeSafeApiIntegration]:
@@ -5991,14 +6131,23 @@
         :stability: experimental
         '''
         result = self._values.get("operation_lookup")
         assert result is not None, "Required property 'operation_lookup' is missing"
         return typing.cast(typing.Mapping[builtins.str, OperationDetails], result)
 
     @builtins.property
+    def api_key_options(self) -> typing.Optional[ApiKeyOptions]:
+        '''(experimental) Options for API keys.
+
+        :stability: experimental
+        '''
+        result = self._values.get("api_key_options")
+        return typing.cast(typing.Optional[ApiKeyOptions], result)
+
+    @builtins.property
     def cors_options(
         self,
     ) -> typing.Optional[_aws_cdk_aws_apigateway_ceddda9d.CorsOptions]:
         '''(experimental) Cross Origin Resource Sharing options for the API.
 
         :stability: experimental
         '''
@@ -6619,14 +6768,15 @@
         fail_on_warnings: typing.Optional[builtins.bool] = None,
         parameters: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         policy: typing.Optional[_aws_cdk_aws_iam_ceddda9d.PolicyDocument] = None,
         rest_api_name: typing.Optional[builtins.str] = None,
         retain_deployments: typing.Optional[builtins.bool] = None,
         integrations: typing.Mapping[builtins.str, typing.Union[TypeSafeApiIntegration, typing.Dict[builtins.str, typing.Any]]],
         operation_lookup: typing.Mapping[builtins.str, typing.Union[OperationDetails, typing.Dict[builtins.str, typing.Any]]],
+        api_key_options: typing.Optional[typing.Union[ApiKeyOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         cors_options: typing.Optional[typing.Union[_aws_cdk_aws_apigateway_ceddda9d.CorsOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         default_authorizer: typing.Optional[Authorizer] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param spec_path: (experimental) Path to the JSON open api spec.
@@ -6642,14 +6792,15 @@
         :param fail_on_warnings: Indicates whether to roll back the resource if a warning occurs while API Gateway is creating the RestApi resource. Default: false
         :param parameters: Custom header parameters for the request. Default: - No parameters.
         :param policy: A policy document that contains the permissions for this RestApi. Default: - No policy.
         :param rest_api_name: A name for the API Gateway RestApi resource. Default: - ID of the RestApi construct.
         :param retain_deployments: Retains old deployment resources when the API changes. This allows manually reverting stages to point to old deployments via the AWS Console. Default: false
         :param integrations: (experimental) A mapping of API operation to its integration.
         :param operation_lookup: (experimental) Details about each operation.
+        :param api_key_options: (experimental) Options for API keys.
         :param cors_options: (experimental) Cross Origin Resource Sharing options for the API.
         :param default_authorizer: (experimental) The default authorizer to use for your api. When omitted, no default authorizer is used. Authorizers specified at the integration level will override this for that operation.
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8e4821d6581d103cd1939ca5166c26d862d1742c080c74994a7cd4722c1c2d19)
@@ -6669,50 +6820,64 @@
             fail_on_warnings=fail_on_warnings,
             parameters=parameters,
             policy=policy,
             rest_api_name=rest_api_name,
             retain_deployments=retain_deployments,
             integrations=integrations,
             operation_lookup=operation_lookup,
+            api_key_options=api_key_options,
             cors_options=cors_options,
             default_authorizer=default_authorizer,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="api")
     def api(self) -> _aws_cdk_aws_apigateway_ceddda9d.SpecRestApi:
-        '''
+        '''(experimental) Underlying API Gateway API construct.
+
         :stability: experimental
         '''
         return typing.cast(_aws_cdk_aws_apigateway_ceddda9d.SpecRestApi, jsii.get(self, "api"))
 
     @builtins.property
+    @jsii.member(jsii_name="extendedApiSpecification")
+    def extended_api_specification(self) -> typing.Any:
+        '''(experimental) The OpenAPI specification with applied API gateway extensions.
+
+        :stability: experimental
+        '''
+        return typing.cast(typing.Any, jsii.get(self, "extendedApiSpecification"))
+
+    @builtins.property
     @jsii.member(jsii_name="ipSet")
     def ip_set(self) -> typing.Optional[_aws_cdk_aws_wafv2_ceddda9d.CfnIPSet]:
-        '''
+        '''(experimental) Reference to the IP set if created.
+
         :stability: experimental
         '''
         return typing.cast(typing.Optional[_aws_cdk_aws_wafv2_ceddda9d.CfnIPSet], jsii.get(self, "ipSet"))
 
     @builtins.property
     @jsii.member(jsii_name="webAcl")
     def web_acl(self) -> typing.Optional[_aws_cdk_aws_wafv2_ceddda9d.CfnWebACL]:
-        '''
+        '''(experimental) Reference to the webacl, if created.
+
         :stability: experimental
         '''
         return typing.cast(typing.Optional[_aws_cdk_aws_wafv2_ceddda9d.CfnWebACL], jsii.get(self, "webAcl"))
 
     @builtins.property
     @jsii.member(jsii_name="webAclAssociation")
     def web_acl_association(
         self,
     ) -> typing.Optional[_aws_cdk_aws_wafv2_ceddda9d.CfnWebACLAssociation]:
-        '''
+        '''(experimental) Reference to the web acl association if created.
+
         :stability: experimental
         '''
         return typing.cast(typing.Optional[_aws_cdk_aws_wafv2_ceddda9d.CfnWebACLAssociation], jsii.get(self, "webAclAssociation"))
 
 
 @jsii.data_type(
     jsii_type="@aws-prototyping-sdk/type-safe-api.TypeSafeRestApiProps",
@@ -6731,14 +6896,15 @@
         "fail_on_warnings": "failOnWarnings",
         "parameters": "parameters",
         "policy": "policy",
         "rest_api_name": "restApiName",
         "retain_deployments": "retainDeployments",
         "integrations": "integrations",
         "operation_lookup": "operationLookup",
+        "api_key_options": "apiKeyOptions",
         "cors_options": "corsOptions",
         "default_authorizer": "defaultAuthorizer",
         "spec_path": "specPath",
         "web_acl_options": "webAclOptions",
     },
 )
 class TypeSafeRestApiProps(
@@ -6759,14 +6925,15 @@
         fail_on_warnings: typing.Optional[builtins.bool] = None,
         parameters: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         policy: typing.Optional[_aws_cdk_aws_iam_ceddda9d.PolicyDocument] = None,
         rest_api_name: typing.Optional[builtins.str] = None,
         retain_deployments: typing.Optional[builtins.bool] = None,
         integrations: typing.Mapping[builtins.str, typing.Union[TypeSafeApiIntegration, typing.Dict[builtins.str, typing.Any]]],
         operation_lookup: typing.Mapping[builtins.str, typing.Union[OperationDetails, typing.Dict[builtins.str, typing.Any]]],
+        api_key_options: typing.Optional[typing.Union[ApiKeyOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         cors_options: typing.Optional[typing.Union[_aws_cdk_aws_apigateway_ceddda9d.CorsOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         default_authorizer: typing.Optional[Authorizer] = None,
         spec_path: builtins.str,
         web_acl_options: typing.Optional[typing.Union[TypeSafeApiWebAclOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''(experimental) Configuration for the TypeSafeRestApi construct.
 
@@ -6781,25 +6948,28 @@
         :param fail_on_warnings: Indicates whether to roll back the resource if a warning occurs while API Gateway is creating the RestApi resource. Default: false
         :param parameters: Custom header parameters for the request. Default: - No parameters.
         :param policy: A policy document that contains the permissions for this RestApi. Default: - No policy.
         :param rest_api_name: A name for the API Gateway RestApi resource. Default: - ID of the RestApi construct.
         :param retain_deployments: Retains old deployment resources when the API changes. This allows manually reverting stages to point to old deployments via the AWS Console. Default: false
         :param integrations: (experimental) A mapping of API operation to its integration.
         :param operation_lookup: (experimental) Details about each operation.
+        :param api_key_options: (experimental) Options for API keys.
         :param cors_options: (experimental) Cross Origin Resource Sharing options for the API.
         :param default_authorizer: (experimental) The default authorizer to use for your api. When omitted, no default authorizer is used. Authorizers specified at the integration level will override this for that operation.
         :param spec_path: (experimental) Path to the JSON open api spec.
         :param web_acl_options: (experimental) Options for the AWS WAF v2 WebACL associated with the api. By default, a Web ACL with the AWS default managed rule set will be associated with the API. These options may disable or override the defaults.
 
         :stability: experimental
         '''
         if isinstance(deploy_options, dict):
             deploy_options = _aws_cdk_aws_apigateway_ceddda9d.StageOptions(**deploy_options)
         if isinstance(domain_name, dict):
             domain_name = _aws_cdk_aws_apigateway_ceddda9d.DomainNameOptions(**domain_name)
+        if isinstance(api_key_options, dict):
+            api_key_options = ApiKeyOptions(**api_key_options)
         if isinstance(cors_options, dict):
             cors_options = _aws_cdk_aws_apigateway_ceddda9d.CorsOptions(**cors_options)
         if isinstance(web_acl_options, dict):
             web_acl_options = TypeSafeApiWebAclOptions(**web_acl_options)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6abf7110490d9869d975a50b9fe29f98259a9a230be2bbcde1c8e0ea1fd15771)
             check_type(argname="argument cloud_watch_role", value=cloud_watch_role, expected_type=type_hints["cloud_watch_role"])
@@ -6813,14 +6983,15 @@
             check_type(argname="argument fail_on_warnings", value=fail_on_warnings, expected_type=type_hints["fail_on_warnings"])
             check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
             check_type(argname="argument policy", value=policy, expected_type=type_hints["policy"])
             check_type(argname="argument rest_api_name", value=rest_api_name, expected_type=type_hints["rest_api_name"])
             check_type(argname="argument retain_deployments", value=retain_deployments, expected_type=type_hints["retain_deployments"])
             check_type(argname="argument integrations", value=integrations, expected_type=type_hints["integrations"])
             check_type(argname="argument operation_lookup", value=operation_lookup, expected_type=type_hints["operation_lookup"])
+            check_type(argname="argument api_key_options", value=api_key_options, expected_type=type_hints["api_key_options"])
             check_type(argname="argument cors_options", value=cors_options, expected_type=type_hints["cors_options"])
             check_type(argname="argument default_authorizer", value=default_authorizer, expected_type=type_hints["default_authorizer"])
             check_type(argname="argument spec_path", value=spec_path, expected_type=type_hints["spec_path"])
             check_type(argname="argument web_acl_options", value=web_acl_options, expected_type=type_hints["web_acl_options"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "integrations": integrations,
             "operation_lookup": operation_lookup,
@@ -6848,14 +7019,16 @@
             self._values["parameters"] = parameters
         if policy is not None:
             self._values["policy"] = policy
         if rest_api_name is not None:
             self._values["rest_api_name"] = rest_api_name
         if retain_deployments is not None:
             self._values["retain_deployments"] = retain_deployments
+        if api_key_options is not None:
+            self._values["api_key_options"] = api_key_options
         if cors_options is not None:
             self._values["cors_options"] = cors_options
         if default_authorizer is not None:
             self._values["default_authorizer"] = default_authorizer
         if web_acl_options is not None:
             self._values["web_acl_options"] = web_acl_options
 
@@ -7031,14 +7204,23 @@
         :stability: experimental
         '''
         result = self._values.get("operation_lookup")
         assert result is not None, "Required property 'operation_lookup' is missing"
         return typing.cast(typing.Mapping[builtins.str, OperationDetails], result)
 
     @builtins.property
+    def api_key_options(self) -> typing.Optional[ApiKeyOptions]:
+        '''(experimental) Options for API keys.
+
+        :stability: experimental
+        '''
+        result = self._values.get("api_key_options")
+        return typing.cast(typing.Optional[ApiKeyOptions], result)
+
+    @builtins.property
     def cors_options(
         self,
     ) -> typing.Optional[_aws_cdk_aws_apigateway_ceddda9d.CorsOptions]:
         '''(experimental) Cross Origin Resource Sharing options for the API.
 
         :stability: experimental
         '''
@@ -12406,14 +12588,15 @@
         )
 
 
 __all__ = [
     "ApiGatewayIntegration",
     "ApiGatewayIntegrationResponse",
     "ApiGatewayIntegrationTlsConfig",
+    "ApiKeyOptions",
     "Authorizer",
     "AuthorizerProps",
     "Authorizers",
     "CidrAllowList",
     "CognitoAuthorizer",
     "CognitoAuthorizerProps",
     "CustomAuthorizer",
@@ -12467,14 +12650,15 @@
     "SmithyDefinitionOptions",
     "SmithyMavenConfiguration",
     "SmithyModelOptions",
     "SmithyProjection",
     "SmithyServiceName",
     "SmithyTransform",
     "TypeSafeApiIntegration",
+    "TypeSafeApiIntegrationOptions",
     "TypeSafeApiModelProject",
     "TypeSafeApiModelProjectOptions",
     "TypeSafeApiOptions",
     "TypeSafeApiProject",
     "TypeSafeApiProjectOptions",
     "TypeSafeApiWebAclOptions",
     "TypeSafeRestApi",
@@ -12517,14 +12701,22 @@
 def _typecheckingstub__13da332b7a7dcdfb32928a99f0c6dc04a61d0d2e03fed3b12937ae3d342aea5b(
     *,
     insecure_skip_verification: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__cd712e0b528a2a814e998fe599840c879dcf57fc7aea3ad93aea819af03fee2a(
+    *,
+    source: _aws_cdk_aws_apigateway_ceddda9d.ApiKeySourceType,
+    required_by_default: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__2a0b3bb1dc7df594503f85f7e4e203386d8288de3b7e59c33559a1bce31752f5(
     *,
     authorization_type: _aws_cdk_aws_apigateway_ceddda9d.AuthorizationType,
     authorizer_id: builtins.str,
     authorization_scopes: typing.Optional[typing.Sequence[builtins.str]] = None,
 ) -> None:
     """Type checking stubs"""
@@ -12844,14 +13036,22 @@
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__6aac208a4d52a45aa5a05fdd9df9236f624116cf700032ca2ec93451ea1ee14c(
     *,
     integration: Integration,
     authorizer: typing.Optional[Authorizer] = None,
+    options: typing.Optional[typing.Union[TypeSafeApiIntegrationOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__dd841177be00ab24afd6ef8e8d79684af4aa8a6d71e19911ed314e4324e4a377(
+    *,
+    api_key_required: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ab9fbe8ba5379dfe513c8876edcc903cdd8e15a6de4c21aa838dc6c6c7b2402a(
     *,
     name: builtins.str,
@@ -12872,14 +13072,15 @@
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ddffe68493ea33b13b142dd3a74d4b71e0e9eb563dc8d340916de145a0d0dfd3(
     *,
     integrations: typing.Mapping[builtins.str, typing.Union[TypeSafeApiIntegration, typing.Dict[builtins.str, typing.Any]]],
     operation_lookup: typing.Mapping[builtins.str, typing.Union[OperationDetails, typing.Dict[builtins.str, typing.Any]]],
+    api_key_options: typing.Optional[typing.Union[ApiKeyOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     cors_options: typing.Optional[typing.Union[_aws_cdk_aws_apigateway_ceddda9d.CorsOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     default_authorizer: typing.Optional[Authorizer] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__abde6fa90ff9fea9e430aaca82f0c910c5ecc24d1205ba19958f47080d5b15fb(
@@ -12931,14 +13132,15 @@
     fail_on_warnings: typing.Optional[builtins.bool] = None,
     parameters: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     policy: typing.Optional[_aws_cdk_aws_iam_ceddda9d.PolicyDocument] = None,
     rest_api_name: typing.Optional[builtins.str] = None,
     retain_deployments: typing.Optional[builtins.bool] = None,
     integrations: typing.Mapping[builtins.str, typing.Union[TypeSafeApiIntegration, typing.Dict[builtins.str, typing.Any]]],
     operation_lookup: typing.Mapping[builtins.str, typing.Union[OperationDetails, typing.Dict[builtins.str, typing.Any]]],
+    api_key_options: typing.Optional[typing.Union[ApiKeyOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     cors_options: typing.Optional[typing.Union[_aws_cdk_aws_apigateway_ceddda9d.CorsOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     default_authorizer: typing.Optional[Authorizer] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__6abf7110490d9869d975a50b9fe29f98259a9a230be2bbcde1c8e0ea1fd15771(
@@ -12954,14 +13156,15 @@
     fail_on_warnings: typing.Optional[builtins.bool] = None,
     parameters: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     policy: typing.Optional[_aws_cdk_aws_iam_ceddda9d.PolicyDocument] = None,
     rest_api_name: typing.Optional[builtins.str] = None,
     retain_deployments: typing.Optional[builtins.bool] = None,
     integrations: typing.Mapping[builtins.str, typing.Union[TypeSafeApiIntegration, typing.Dict[builtins.str, typing.Any]]],
     operation_lookup: typing.Mapping[builtins.str, typing.Union[OperationDetails, typing.Dict[builtins.str, typing.Any]]],
+    api_key_options: typing.Optional[typing.Union[ApiKeyOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     cors_options: typing.Optional[typing.Union[_aws_cdk_aws_apigateway_ceddda9d.CorsOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     default_authorizer: typing.Optional[Authorizer] = None,
     spec_path: builtins.str,
     web_acl_options: typing.Optional[typing.Union[TypeSafeApiWebAclOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.type-safe-api
-Version: 0.19.5
+Version: 0.19.6
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt` & `aws_prototyping_sdk.type_safe_api-0.19.6/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
 src/aws_prototyping_sdk/type_safe_api/__init__.py
 src/aws_prototyping_sdk/type_safe_api/py.typed
 src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
-src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.19.5.jsii.tgz
+src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.19.6.jsii.tgz
```

