# Comparing `tmp/aws_prototyping_sdk.type_safe_api-0.18.9.tar.gz` & `tmp/aws_prototyping_sdk.type_safe_api-0.19.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.18.9.tar", last modified: Mon May 15 04:27:57 2023, max compression
+gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.19.5.tar", last modified: Tue May 30 03:06:14 2023, max compression
```

## Comparing `aws_prototyping_sdk.type_safe_api-0.18.9.tar` & `aws_prototyping_sdk.type_safe_api-0.19.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:27:57.550965 aws_prototyping_sdk.type_safe_api-0.18.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-15 04:27:38.000000 aws_prototyping_sdk.type_safe_api-0.18.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 04:27:38.000000 aws_prototyping_sdk.type_safe_api-0.18.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    61480 2023-05-15 04:27:57.550965 aws_prototyping_sdk.type_safe_api-0.18.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-05-15 04:27:38.000000 aws_prototyping_sdk.type_safe_api-0.18.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-15 04:27:38.000000 aws_prototyping_sdk.type_safe_api-0.18.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 04:27:57.550965 aws_prototyping_sdk.type_safe_api-0.18.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-15 04:27:38.000000 aws_prototyping_sdk.type_safe_api-0.18.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:27:57.538965 aws_prototyping_sdk.type_safe_api-0.18.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:27:57.538965 aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:27:57.546965 aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk/type_safe_api/
--rw-r--r--   0 runner    (1001) docker     (123)   301873 2023-05-15 04:27:38.000000 aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk/type_safe_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:27:57.546965 aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk/type_safe_api/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-15 04:27:38.000000 aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   879466 2023-05-15 04:27:38.000000 aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.9.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:27:38.000000 aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk/type_safe_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:27:57.542965 aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk.type_safe_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    61480 2023-05-15 04:27:57.000000 aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-15 04:27:57.000000 aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:27:57.000000 aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-15 04:27:57.000000 aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 04:27:57.000000 aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:06:14.735804 aws_prototyping_sdk.type_safe_api-0.19.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    65065 2023-05-30 03:06:14.731804 aws_prototyping_sdk.type_safe_api-0.19.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    64124 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 03:06:14.735804 aws_prototyping_sdk.type_safe_api-0.19.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:06:14.723804 aws_prototyping_sdk.type_safe_api-0.19.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:06:14.727804 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:06:14.731804 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/type_safe_api/
+-rw-r--r--   0 runner    (1001) docker     (123)   615180 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/type_safe_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:06:14.731804 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/type_safe_api/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   973612 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.19.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 03:05:53.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk/type_safe_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:06:14.727804 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    65065 2023-05-30 03:06:14.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-30 03:06:14.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 03:06:14.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 03:06:14.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 03:06:14.000000 aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.9/LICENSE` & `aws_prototyping_sdk.type_safe_api-0.19.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.9/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.19.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.type_safe_api
-Version: 0.18.9
+Version: 0.19.5
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -591,15 +591,39 @@
 
 #### Integrations
 
 Integrations are used by API Gateway to service requests.
 
 ##### Lambda Integration
 
-Currently, the only built-in integration is a lambda integration. You can construct one using `Integrations.lambda(yourLambdaFunction)`.
+For integrating an API operation with a lambda, you can use `Integrations.lambda(yourLambdaFunction)`.
+
+##### Mock Integration
+
+To mock an API operation, you can use the `MockIntegrations` class which you'll find in your generated infrastructure package. This contains an integration for every response that can be returned by your operations.
+
+For example:
+
+```python
+import { Api, MockIntegrations } from "myapi-typescript-infra";
+
+new Api(this, "Api", {
+  integrations: {
+    sayHello: {
+      integration: MockIntegrations.sayHello200({ message: "This is a mocked successful response!" }),
+    },
+  },
+});
+```
+
+If you're using the `TypeSafeRestApi` construct directly without generated infrastructure, or need to mock a response not defined in your model, you can use `Integrations.mock`. API gateway will respond with the status code and body provided, eg:
+
+```python
+Integrations.mock({ statusCode: 200, body: JSON.stringify({ message: "hello world!" }) })
+```
 
 ##### Custom Integrations
 
 You can implement your own integrations by inheriting the `Integration` class and implementing its `render` method. This method is responsible for returning a snippet of OpenAPI which will be added as the `x-amazon-apigateway-integration` for an operation. Please refer to the [API Gateway Swagger Extensions documentation](https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-swagger-extensions-integration.html) for more details.
 
 You can also optionally override the `grant` method if you need to use CDK to grant API Gateway access to invoke your integration.
 
@@ -1127,72 +1151,88 @@
   },
   ...
 });
 ```
 
 ##### Usage in a React Website
 
-First, make sure you create an instance of the API client (making sure to set the base URL and fetch instance). For example:
+First, make sure you add a dependency on the generated hooks library, eg in your `.projenrc`:
+
+```python
+const api = new TypeSafeApiProject({ ... });
+
+new CloudscapeReactTsWebsite({
+  ...,
+  deps: [
+    ...
+    api.library.typescriptReactQueryHooks!.package.packageName,
+  ],
+});
+```
+
+Next, create an instance of the API client (making sure to set the base URL and fetch instance). For example:
 
 ```python
-export const useMyApiClient = () =>
+// NB: client may be named differently if you have tagged your operations
+import { DefaultApi } from "myapi-typescript-react-query-hooks";
+
+export const useApiClient = () =>
   useMemo(
     () =>
-      new MyApi(
+      new DefaultApi(
         new Configuration({
           basePath:
             "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
           fetchApi: window.fetch.bind(window),
         })
       ),
     []
   );
 ```
 
 Note that if you are using the [Cloudscape React Website](../cloudscape-react-ts-website/README.md) with [AWS NorthStar](https://aws.github.io/aws-northstar/) and IAM (Sigv4) Auth for your API, you can use NorthStar's [`useSigv4Client()` hook](https://aws.github.io/aws-northstar/?path=/story/components-cognitoauth-sigv4client-docs--page) to create
 an instance of `fetch` which will sign requests with the logged in user's credentials. For example:
 
 ```python
-export const useMyApiClient = () => {
+export const useApiClient = () => {
   const client = useSigv4Client();
   return useMemo(
     () =>
-      client
-        ? new MyApi(
-            new Configuration({
-              basePath:
-                "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
-              fetchApi: client,
-            })
-          )
-        : undefined,
+      new DefaultApi(
+        new Configuration({
+          basePath:
+            "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
+          fetchApi: client,
+        })
+      ),
     [client]
   );
 };
 ```
 
 Next, instantiate the client provider above where you would like to use the hooks in your component hierarchy (such as above your router). For example:
 
 ```tsx
+// NB: client provider may be named differently if you have tagged your operations
 import { DefaultApiClientProvider } from "myapi-typescript-react-query-hooks";
 
-const api = useMyApiClient();
+const api = useApiClient();
 
-return api ? (
+return (
   <DefaultApiClientProvider apiClient={api}>
     {/* Components within the provider may make use of the hooks */}
   </DefaultApiClientProvider>
-) : (
-  <p>Loading...</p>
 );
 ```
 
 Finally, you can import and use your generated hooks. For example:
 
 ```tsx
+import { useSayHello } from "myapi-typescript-react-query-hooks";
+
 export const MyComponent: FC<MyComponentProps> = () => {
   const sayHello = useSayHello({ name: "World" });
 
   return sayHello.isLoading ? (
     <p>Loading...</p>
   ) : sayHello.isError ? (
     <p>Error!</p>
@@ -1265,14 +1305,31 @@
       },
     },
   },
   ...
 });
 ```
 
+##### Custom QueryClient
+
+If you wish to customise the react-query `QueryClient`, pass a custom instance to the client provider, eg:
+
+```tsx
+import { DefaultApiClientProvider } from "myapi-typescript-react-query-hooks";
+import { QueryClient } from "@tanstack/react-query";
+
+const queryClient = new QueryClient({ ... });
+
+return (
+  <DefaultApiClientProvider apiClient={api} client={queryClient}>
+    {/* Components within the provider may make use of the hooks */}
+  </DefaultApiClientProvider>
+);
+```
+
 ### Quick Start: Python
 
 This guide assumes you want to write your CDK infrastructure in Python and your lambda handlers in Python, however note that you your infrastructure language and lambda handler language(s) are not tied to one another, you can mix and match as you like. Just specify the language in `runtime.languages` for any language you would like to write lambda handlers in.
 
 #### Create Your API Project
 
 Use the project in your `.projenrc.ts`. It can either be part of an [`nx-monorepo`](../nx-monorepo/README.md) (recommended) or used in a standalone fashion.
@@ -1738,7 +1795,60 @@
 Make sure you do not deploy your CDK stack with `type-safe-api-local` set to `true`, since this uses an inline API definition which bloats the CloudFormation template and can exceed the maximum template size depending on the size of your API.
 
 ##### Limitations
 
 Note that there is currently a limitation with SAM CLI where it does not support mock integrations, which means that the development server will not respond to OPTIONS requests even if you specified `corsOptions: { ... }` in your `Api` construct. This is being tracked as a [feature request here](https://github.com/aws/aws-sam-cli/issues/4973).
 
 Note also that your API business logic may include operations which do not work locally, or may interact with real AWS resources depending on the AWS credentials you start your local development server with.
+
+#### Customising OpenAPI Generator CLI
+
+[OpenAPI Generator CLI](https://github.com/OpenAPITools/openapi-generator-cli) is used to generate the infrastructure, runtime and library projects. You can customise some of its properties for specific projects if you like. Note that changing the `version` may cause generated code to be broken, since it's written assuming the default version.
+
+For example, to customise the maven repository used to pull the OpenAPI Generator jar, you can configure the `TypeSafeApiProject` as follows:
+
+```python
+const openApiGeneratorCliConfig: OpenApiGeneratorCliConfig = {
+  repository: {
+    downloadUrl:
+      "https://my.custom.maven.repo/maven2/${groupId}/${artifactId}/${versionName}/${artifactId}-${versionName}.jar",
+  },
+};
+
+const project = new TypeSafeApiProject({
+  infrastructure: {
+    language: Language.TYPESCRIPT,
+    options: {
+      // Note here the options are typed as "GeneratedTypeScriptProjectOptions" but you can
+      // pass a partial one to avoid having to specify a custom project name etc
+      typescript: {
+        openApiGeneratorCliConfig,
+      } satisfies Partial<GeneratedTypeScriptProjectOptions> as any,
+    },
+  },
+  runtime: {
+    languages: [Language.TYPESCRIPT],
+    options: {
+      typescript: {
+        openApiGeneratorCliConfig,
+      } satisfies Partial<GeneratedTypeScriptProjectOptions> as any,
+    },
+  },
+  library: {
+    libraries: [Library.TYPESCRIPT_REACT_QUERY_HOOKS],
+    options: {
+      typescriptReactQueryHooks: {
+        openApiGeneratorCliConfig,
+      } satisfies Partial<GeneratedTypeScriptProjectOptions> as any,
+    },
+  },
+  documentation: {
+    formats: [DocumentationFormat.HTML2],
+    options: {
+      html2: {
+        openApiGeneratorCliConfig,
+      },
+    },
+  },
+  ...
+});
+```
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.9/README.md` & `aws_prototyping_sdk.type_safe_api-0.19.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -567,15 +567,39 @@
 
 #### Integrations
 
 Integrations are used by API Gateway to service requests.
 
 ##### Lambda Integration
 
-Currently, the only built-in integration is a lambda integration. You can construct one using `Integrations.lambda(yourLambdaFunction)`.
+For integrating an API operation with a lambda, you can use `Integrations.lambda(yourLambdaFunction)`.
+
+##### Mock Integration
+
+To mock an API operation, you can use the `MockIntegrations` class which you'll find in your generated infrastructure package. This contains an integration for every response that can be returned by your operations.
+
+For example:
+
+```python
+import { Api, MockIntegrations } from "myapi-typescript-infra";
+
+new Api(this, "Api", {
+  integrations: {
+    sayHello: {
+      integration: MockIntegrations.sayHello200({ message: "This is a mocked successful response!" }),
+    },
+  },
+});
+```
+
+If you're using the `TypeSafeRestApi` construct directly without generated infrastructure, or need to mock a response not defined in your model, you can use `Integrations.mock`. API gateway will respond with the status code and body provided, eg:
+
+```python
+Integrations.mock({ statusCode: 200, body: JSON.stringify({ message: "hello world!" }) })
+```
 
 ##### Custom Integrations
 
 You can implement your own integrations by inheriting the `Integration` class and implementing its `render` method. This method is responsible for returning a snippet of OpenAPI which will be added as the `x-amazon-apigateway-integration` for an operation. Please refer to the [API Gateway Swagger Extensions documentation](https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-swagger-extensions-integration.html) for more details.
 
 You can also optionally override the `grant` method if you need to use CDK to grant API Gateway access to invoke your integration.
 
@@ -1103,72 +1127,88 @@
   },
   ...
 });
 ```
 
 ##### Usage in a React Website
 
-First, make sure you create an instance of the API client (making sure to set the base URL and fetch instance). For example:
+First, make sure you add a dependency on the generated hooks library, eg in your `.projenrc`:
 
 ```python
-export const useMyApiClient = () =>
+const api = new TypeSafeApiProject({ ... });
+
+new CloudscapeReactTsWebsite({
+  ...,
+  deps: [
+    ...
+    api.library.typescriptReactQueryHooks!.package.packageName,
+  ],
+});
+```
+
+Next, create an instance of the API client (making sure to set the base URL and fetch instance). For example:
+
+```python
+// NB: client may be named differently if you have tagged your operations
+import { DefaultApi } from "myapi-typescript-react-query-hooks";
+
+export const useApiClient = () =>
   useMemo(
     () =>
-      new MyApi(
+      new DefaultApi(
         new Configuration({
           basePath:
             "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
           fetchApi: window.fetch.bind(window),
         })
       ),
     []
   );
 ```
 
 Note that if you are using the [Cloudscape React Website](../cloudscape-react-ts-website/README.md) with [AWS NorthStar](https://aws.github.io/aws-northstar/) and IAM (Sigv4) Auth for your API, you can use NorthStar's [`useSigv4Client()` hook](https://aws.github.io/aws-northstar/?path=/story/components-cognitoauth-sigv4client-docs--page) to create
 an instance of `fetch` which will sign requests with the logged in user's credentials. For example:
 
 ```python
-export const useMyApiClient = () => {
+export const useApiClient = () => {
   const client = useSigv4Client();
   return useMemo(
     () =>
-      client
-        ? new MyApi(
-            new Configuration({
-              basePath:
-                "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
-              fetchApi: client,
-            })
-          )
-        : undefined,
+      new DefaultApi(
+        new Configuration({
+          basePath:
+            "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
+          fetchApi: client,
+        })
+      ),
     [client]
   );
 };
 ```
 
 Next, instantiate the client provider above where you would like to use the hooks in your component hierarchy (such as above your router). For example:
 
 ```tsx
+// NB: client provider may be named differently if you have tagged your operations
 import { DefaultApiClientProvider } from "myapi-typescript-react-query-hooks";
 
-const api = useMyApiClient();
+const api = useApiClient();
 
-return api ? (
+return (
   <DefaultApiClientProvider apiClient={api}>
     {/* Components within the provider may make use of the hooks */}
   </DefaultApiClientProvider>
-) : (
-  <p>Loading...</p>
 );
 ```
 
 Finally, you can import and use your generated hooks. For example:
 
 ```tsx
+import { useSayHello } from "myapi-typescript-react-query-hooks";
+
 export const MyComponent: FC<MyComponentProps> = () => {
   const sayHello = useSayHello({ name: "World" });
 
   return sayHello.isLoading ? (
     <p>Loading...</p>
   ) : sayHello.isError ? (
     <p>Error!</p>
@@ -1241,14 +1281,31 @@
       },
     },
   },
   ...
 });
 ```
 
+##### Custom QueryClient
+
+If you wish to customise the react-query `QueryClient`, pass a custom instance to the client provider, eg:
+
+```tsx
+import { DefaultApiClientProvider } from "myapi-typescript-react-query-hooks";
+import { QueryClient } from "@tanstack/react-query";
+
+const queryClient = new QueryClient({ ... });
+
+return (
+  <DefaultApiClientProvider apiClient={api} client={queryClient}>
+    {/* Components within the provider may make use of the hooks */}
+  </DefaultApiClientProvider>
+);
+```
+
 ### Quick Start: Python
 
 This guide assumes you want to write your CDK infrastructure in Python and your lambda handlers in Python, however note that you your infrastructure language and lambda handler language(s) are not tied to one another, you can mix and match as you like. Just specify the language in `runtime.languages` for any language you would like to write lambda handlers in.
 
 #### Create Your API Project
 
 Use the project in your `.projenrc.ts`. It can either be part of an [`nx-monorepo`](../nx-monorepo/README.md) (recommended) or used in a standalone fashion.
@@ -1714,7 +1771,60 @@
 Make sure you do not deploy your CDK stack with `type-safe-api-local` set to `true`, since this uses an inline API definition which bloats the CloudFormation template and can exceed the maximum template size depending on the size of your API.
 
 ##### Limitations
 
 Note that there is currently a limitation with SAM CLI where it does not support mock integrations, which means that the development server will not respond to OPTIONS requests even if you specified `corsOptions: { ... }` in your `Api` construct. This is being tracked as a [feature request here](https://github.com/aws/aws-sam-cli/issues/4973).
 
 Note also that your API business logic may include operations which do not work locally, or may interact with real AWS resources depending on the AWS credentials you start your local development server with.
+
+#### Customising OpenAPI Generator CLI
+
+[OpenAPI Generator CLI](https://github.com/OpenAPITools/openapi-generator-cli) is used to generate the infrastructure, runtime and library projects. You can customise some of its properties for specific projects if you like. Note that changing the `version` may cause generated code to be broken, since it's written assuming the default version.
+
+For example, to customise the maven repository used to pull the OpenAPI Generator jar, you can configure the `TypeSafeApiProject` as follows:
+
+```python
+const openApiGeneratorCliConfig: OpenApiGeneratorCliConfig = {
+  repository: {
+    downloadUrl:
+      "https://my.custom.maven.repo/maven2/${groupId}/${artifactId}/${versionName}/${artifactId}-${versionName}.jar",
+  },
+};
+
+const project = new TypeSafeApiProject({
+  infrastructure: {
+    language: Language.TYPESCRIPT,
+    options: {
+      // Note here the options are typed as "GeneratedTypeScriptProjectOptions" but you can
+      // pass a partial one to avoid having to specify a custom project name etc
+      typescript: {
+        openApiGeneratorCliConfig,
+      } satisfies Partial<GeneratedTypeScriptProjectOptions> as any,
+    },
+  },
+  runtime: {
+    languages: [Language.TYPESCRIPT],
+    options: {
+      typescript: {
+        openApiGeneratorCliConfig,
+      } satisfies Partial<GeneratedTypeScriptProjectOptions> as any,
+    },
+  },
+  library: {
+    libraries: [Library.TYPESCRIPT_REACT_QUERY_HOOKS],
+    options: {
+      typescriptReactQueryHooks: {
+        openApiGeneratorCliConfig,
+      } satisfies Partial<GeneratedTypeScriptProjectOptions> as any,
+    },
+  },
+  documentation: {
+    formats: [DocumentationFormat.HTML2],
+    options: {
+      html2: {
+        openApiGeneratorCliConfig,
+      },
+    },
+  },
+  ...
+});
+```
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.9/setup.py` & `aws_prototyping_sdk.type_safe_api-0.19.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.type_safe_api",
-    "version": "0.18.9",
+    "version": "0.19.5",
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
-            "type-safe-api@0.18.9.jsii.tgz"
+            "type-safe-api@0.19.5.jsii.tgz"
         ],
         "aws_prototyping_sdk.type_safe_api": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.type-safe-api
-Version: 0.18.9
+Version: 0.19.5
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -591,15 +591,39 @@
 
 #### Integrations
 
 Integrations are used by API Gateway to service requests.
 
 ##### Lambda Integration
 
-Currently, the only built-in integration is a lambda integration. You can construct one using `Integrations.lambda(yourLambdaFunction)`.
+For integrating an API operation with a lambda, you can use `Integrations.lambda(yourLambdaFunction)`.
+
+##### Mock Integration
+
+To mock an API operation, you can use the `MockIntegrations` class which you'll find in your generated infrastructure package. This contains an integration for every response that can be returned by your operations.
+
+For example:
+
+```python
+import { Api, MockIntegrations } from "myapi-typescript-infra";
+
+new Api(this, "Api", {
+  integrations: {
+    sayHello: {
+      integration: MockIntegrations.sayHello200({ message: "This is a mocked successful response!" }),
+    },
+  },
+});
+```
+
+If you're using the `TypeSafeRestApi` construct directly without generated infrastructure, or need to mock a response not defined in your model, you can use `Integrations.mock`. API gateway will respond with the status code and body provided, eg:
+
+```python
+Integrations.mock({ statusCode: 200, body: JSON.stringify({ message: "hello world!" }) })
+```
 
 ##### Custom Integrations
 
 You can implement your own integrations by inheriting the `Integration` class and implementing its `render` method. This method is responsible for returning a snippet of OpenAPI which will be added as the `x-amazon-apigateway-integration` for an operation. Please refer to the [API Gateway Swagger Extensions documentation](https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-swagger-extensions-integration.html) for more details.
 
 You can also optionally override the `grant` method if you need to use CDK to grant API Gateway access to invoke your integration.
 
@@ -1127,72 +1151,88 @@
   },
   ...
 });
 ```
 
 ##### Usage in a React Website
 
-First, make sure you create an instance of the API client (making sure to set the base URL and fetch instance). For example:
+First, make sure you add a dependency on the generated hooks library, eg in your `.projenrc`:
+
+```python
+const api = new TypeSafeApiProject({ ... });
+
+new CloudscapeReactTsWebsite({
+  ...,
+  deps: [
+    ...
+    api.library.typescriptReactQueryHooks!.package.packageName,
+  ],
+});
+```
+
+Next, create an instance of the API client (making sure to set the base URL and fetch instance). For example:
 
 ```python
-export const useMyApiClient = () =>
+// NB: client may be named differently if you have tagged your operations
+import { DefaultApi } from "myapi-typescript-react-query-hooks";
+
+export const useApiClient = () =>
   useMemo(
     () =>
-      new MyApi(
+      new DefaultApi(
         new Configuration({
           basePath:
             "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
           fetchApi: window.fetch.bind(window),
         })
       ),
     []
   );
 ```
 
 Note that if you are using the [Cloudscape React Website](../cloudscape-react-ts-website/README.md) with [AWS NorthStar](https://aws.github.io/aws-northstar/) and IAM (Sigv4) Auth for your API, you can use NorthStar's [`useSigv4Client()` hook](https://aws.github.io/aws-northstar/?path=/story/components-cognitoauth-sigv4client-docs--page) to create
 an instance of `fetch` which will sign requests with the logged in user's credentials. For example:
 
 ```python
-export const useMyApiClient = () => {
+export const useApiClient = () => {
   const client = useSigv4Client();
   return useMemo(
     () =>
-      client
-        ? new MyApi(
-            new Configuration({
-              basePath:
-                "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
-              fetchApi: client,
-            })
-          )
-        : undefined,
+      new DefaultApi(
+        new Configuration({
+          basePath:
+            "https://example123.execute-api.ap-southeast-2.amazonaws.com/prod",
+          fetchApi: client,
+        })
+      ),
     [client]
   );
 };
 ```
 
 Next, instantiate the client provider above where you would like to use the hooks in your component hierarchy (such as above your router). For example:
 
 ```tsx
+// NB: client provider may be named differently if you have tagged your operations
 import { DefaultApiClientProvider } from "myapi-typescript-react-query-hooks";
 
-const api = useMyApiClient();
+const api = useApiClient();
 
-return api ? (
+return (
   <DefaultApiClientProvider apiClient={api}>
     {/* Components within the provider may make use of the hooks */}
   </DefaultApiClientProvider>
-) : (
-  <p>Loading...</p>
 );
 ```
 
 Finally, you can import and use your generated hooks. For example:
 
 ```tsx
+import { useSayHello } from "myapi-typescript-react-query-hooks";
+
 export const MyComponent: FC<MyComponentProps> = () => {
   const sayHello = useSayHello({ name: "World" });
 
   return sayHello.isLoading ? (
     <p>Loading...</p>
   ) : sayHello.isError ? (
     <p>Error!</p>
@@ -1265,14 +1305,31 @@
       },
     },
   },
   ...
 });
 ```
 
+##### Custom QueryClient
+
+If you wish to customise the react-query `QueryClient`, pass a custom instance to the client provider, eg:
+
+```tsx
+import { DefaultApiClientProvider } from "myapi-typescript-react-query-hooks";
+import { QueryClient } from "@tanstack/react-query";
+
+const queryClient = new QueryClient({ ... });
+
+return (
+  <DefaultApiClientProvider apiClient={api} client={queryClient}>
+    {/* Components within the provider may make use of the hooks */}
+  </DefaultApiClientProvider>
+);
+```
+
 ### Quick Start: Python
 
 This guide assumes you want to write your CDK infrastructure in Python and your lambda handlers in Python, however note that you your infrastructure language and lambda handler language(s) are not tied to one another, you can mix and match as you like. Just specify the language in `runtime.languages` for any language you would like to write lambda handlers in.
 
 #### Create Your API Project
 
 Use the project in your `.projenrc.ts`. It can either be part of an [`nx-monorepo`](../nx-monorepo/README.md) (recommended) or used in a standalone fashion.
@@ -1738,7 +1795,60 @@
 Make sure you do not deploy your CDK stack with `type-safe-api-local` set to `true`, since this uses an inline API definition which bloats the CloudFormation template and can exceed the maximum template size depending on the size of your API.
 
 ##### Limitations
 
 Note that there is currently a limitation with SAM CLI where it does not support mock integrations, which means that the development server will not respond to OPTIONS requests even if you specified `corsOptions: { ... }` in your `Api` construct. This is being tracked as a [feature request here](https://github.com/aws/aws-sam-cli/issues/4973).
 
 Note also that your API business logic may include operations which do not work locally, or may interact with real AWS resources depending on the AWS credentials you start your local development server with.
+
+#### Customising OpenAPI Generator CLI
+
+[OpenAPI Generator CLI](https://github.com/OpenAPITools/openapi-generator-cli) is used to generate the infrastructure, runtime and library projects. You can customise some of its properties for specific projects if you like. Note that changing the `version` may cause generated code to be broken, since it's written assuming the default version.
+
+For example, to customise the maven repository used to pull the OpenAPI Generator jar, you can configure the `TypeSafeApiProject` as follows:
+
+```python
+const openApiGeneratorCliConfig: OpenApiGeneratorCliConfig = {
+  repository: {
+    downloadUrl:
+      "https://my.custom.maven.repo/maven2/${groupId}/${artifactId}/${versionName}/${artifactId}-${versionName}.jar",
+  },
+};
+
+const project = new TypeSafeApiProject({
+  infrastructure: {
+    language: Language.TYPESCRIPT,
+    options: {
+      // Note here the options are typed as "GeneratedTypeScriptProjectOptions" but you can
+      // pass a partial one to avoid having to specify a custom project name etc
+      typescript: {
+        openApiGeneratorCliConfig,
+      } satisfies Partial<GeneratedTypeScriptProjectOptions> as any,
+    },
+  },
+  runtime: {
+    languages: [Language.TYPESCRIPT],
+    options: {
+      typescript: {
+        openApiGeneratorCliConfig,
+      } satisfies Partial<GeneratedTypeScriptProjectOptions> as any,
+    },
+  },
+  library: {
+    libraries: [Library.TYPESCRIPT_REACT_QUERY_HOOKS],
+    options: {
+      typescriptReactQueryHooks: {
+        openApiGeneratorCliConfig,
+      } satisfies Partial<GeneratedTypeScriptProjectOptions> as any,
+    },
+  },
+  documentation: {
+    formats: [DocumentationFormat.HTML2],
+    options: {
+      html2: {
+        openApiGeneratorCliConfig,
+      },
+    },
+  },
+  ...
+});
+```
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.9/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt` & `aws_prototyping_sdk.type_safe_api-0.19.5/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
 src/aws_prototyping_sdk/type_safe_api/__init__.py
 src/aws_prototyping_sdk/type_safe_api/py.typed
 src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
-src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.9.jsii.tgz
+src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.19.5.jsii.tgz
```

