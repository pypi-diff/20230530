# Comparing `tmp/aliyun-python-sdk-vpcpeer-1.0.0.tar.gz` & `tmp/aliyun-python-sdk-vpcpeer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-vpcpeer-1.0.0.tar", last modified: Fri Feb 24 02:17:55 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-vpcpeer-1.0.1.tar", last modified: Tue May 30 07:59:54 2023, max compression
```

## Comparing `aliyun-python-sdk-vpcpeer-1.0.0.tar` & `aliyun-python-sdk-vpcpeer-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      575 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1557 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyun_python_sdk_vpcpeer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1557 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyun_python_sdk_vpcpeer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      923 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyun_python_sdk_vpcpeer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyun_python_sdk_vpcpeer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyun_python_sdk_vpcpeer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyun_python_sdk_vpcpeer.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/
--rw-r--r--   0 root         (0) root         (0)     2104 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/AcceptVpcPeerConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/CreateVpcPeerConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2016 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/DeleteVpcPeerConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/GetVpcPeerConnectionAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2670 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/ListVpcPeerConnectionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/ModifyVpcPeerConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/RejectVpcPeerConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2472 2023-02-24 02:17:55.000000 aliyun-python-sdk-vpcpeer-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/AcceptVpcPeerConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/CreateVpcPeerConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/DeleteVpcPeerConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/GetVpcPeerConnectionAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/ListVpcPeerConnectionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/ModifyVpcPeerConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/RejectVpcPeerConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/UnTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/setup.py
```

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/LICENSE` & `aliyun-python-sdk-vpcpeer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/PKG-INFO` & `aliyun-python-sdk-vpcpeer-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-vpcpeer
-Version: 1.0.0
+Version: 1.0.1
 Summary: The vpcpeer module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-vpcpeer
```

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/README.rst` & `aliyun-python-sdk-vpcpeer-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/aliyun_python_sdk_vpcpeer.egg-info/PKG-INFO` & `aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-vpcpeer
-Version: 1.0.0
+Version: 1.0.1
 Summary: The vpcpeer module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-vpcpeer
```

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/aliyun_python_sdk_vpcpeer.egg-info/SOURCES.txt` & `aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,11 +11,14 @@
 aliyunsdkvpcpeer/__init__.py
 aliyunsdkvpcpeer/endpoint.py
 aliyunsdkvpcpeer/request/__init__.py
 aliyunsdkvpcpeer/request/v20220101/AcceptVpcPeerConnectionRequest.py
 aliyunsdkvpcpeer/request/v20220101/CreateVpcPeerConnectionRequest.py
 aliyunsdkvpcpeer/request/v20220101/DeleteVpcPeerConnectionRequest.py
 aliyunsdkvpcpeer/request/v20220101/GetVpcPeerConnectionAttributeRequest.py
+aliyunsdkvpcpeer/request/v20220101/ListTagResourcesRequest.py
 aliyunsdkvpcpeer/request/v20220101/ListVpcPeerConnectionsRequest.py
 aliyunsdkvpcpeer/request/v20220101/ModifyVpcPeerConnectionRequest.py
 aliyunsdkvpcpeer/request/v20220101/RejectVpcPeerConnectionRequest.py
+aliyunsdkvpcpeer/request/v20220101/TagResourcesRequest.py
+aliyunsdkvpcpeer/request/v20220101/UnTagResourcesRequest.py
 aliyunsdkvpcpeer/request/v20220101/__init__.py
```

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/endpoint.py` & `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/AcceptVpcPeerConnectionRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/RejectVpcPeerConnectionRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpcpeer.endpoint import endpoint_data
 
-class AcceptVpcPeerConnectionRequest(RpcRequest):
+class RejectVpcPeerConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'VpcPeer', '2022-01-01', 'AcceptVpcPeerConnection','vpcpeer')
+		RpcRequest.__init__(self, 'VpcPeer', '2022-01-01', 'RejectVpcPeerConnection','vpcpeer')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/CreateVpcPeerConnectionRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/CreateVpcPeerConnectionRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,14 +42,19 @@
 	def set_Description(self, Description):  # String
 		self.add_body_params('Description', Description)
 	def get_AcceptingAliUid(self): # Long
 		return self.get_body_params().get('AcceptingAliUid')
 
 	def set_AcceptingAliUid(self, AcceptingAliUid):  # Long
 		self.add_body_params('AcceptingAliUid', AcceptingAliUid)
+	def get_ResourceGroupId(self): # String
+		return self.get_body_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_body_params('ResourceGroupId', ResourceGroupId)
 	def get_AcceptingRegionId(self): # String
 		return self.get_body_params().get('AcceptingRegionId')
 
 	def set_AcceptingRegionId(self, AcceptingRegionId):  # String
 		self.add_body_params('AcceptingRegionId', AcceptingRegionId)
 	def get_DryRun(self): # Boolean
 		return self.get_body_params().get('DryRun')
```

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/DeleteVpcPeerConnectionRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/DeleteVpcPeerConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/GetVpcPeerConnectionAttributeRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/GetVpcPeerConnectionAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/ListVpcPeerConnectionsRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/ListTagResourcesRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpcpeer.endpoint import endpoint_data
 
-class ListVpcPeerConnectionsRequest(RpcRequest):
+class ListTagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'VpcPeer', '2022-01-01', 'ListVpcPeerConnections','vpcpeer')
+		RpcRequest.__init__(self, 'VpcPeer', '2022-01-01', 'ListTagResources','vpcpeer')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_NextToken(self): # String
-		return self.get_body_params().get('NextToken')
+		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
-		self.add_body_params('NextToken', NextToken)
-	def get_Tagss(self): # RepeatList
-		return self.get_query_params().get('Tags')
-
-	def set_Tagss(self, Tags):  # RepeatList
-		for depth1 in range(len(Tags)):
-			if Tags[depth1].get('Key') is not None:
-				self.add_query_param('Tags.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
-			if Tags[depth1].get('Value') is not None:
-				self.add_query_param('Tags.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
-	def get_InstanceId(self): # String
-		return self.get_body_params().get('InstanceId')
-
-	def set_InstanceId(self, InstanceId):  # String
-		self.add_body_params('InstanceId', InstanceId)
-	def get_VpcId(self): # Array
-		return self.get_body_params().get('VpcId')
-
-	def set_VpcId(self, VpcId):  # Array
-		for index1, value1 in enumerate(VpcId):
-			self.add_body_params('VpcId.' + str(index1 + 1), value1)
-	def get_Name(self): # String
-		return self.get_body_params().get('Name')
+		self.add_query_param('NextToken', NextToken)
+	def get_Tags(self): # RepeatList
+		return self.get_query_params().get('Tag')
+
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Key') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+			if Tag[depth1].get('Value') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
+	def get_ResourceIds(self): # RepeatList
+		return self.get_query_params().get('ResourceId')
+
+	def set_ResourceIds(self, ResourceId):  # RepeatList
+		for depth1 in range(len(ResourceId)):
+			self.add_query_param('ResourceId.' + str(depth1 + 1), ResourceId[depth1])
+	def get_ResourceType(self): # String
+		return self.get_query_params().get('ResourceType')
 
-	def set_Name(self, Name):  # String
-		self.add_body_params('Name', Name)
+	def set_ResourceType(self, ResourceType):  # String
+		self.add_query_param('ResourceType', ResourceType)
 	def get_MaxResults(self): # Integer
-		return self.get_body_params().get('MaxResults')
+		return self.get_query_params().get('MaxResults')
 
 	def set_MaxResults(self, MaxResults):  # Integer
-		self.add_body_params('MaxResults', MaxResults)
+		self.add_query_param('MaxResults', MaxResults)
```

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/ModifyVpcPeerConnectionRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/ModifyVpcPeerConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/aliyunsdkvpcpeer/request/v20220101/RejectVpcPeerConnectionRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/AcceptVpcPeerConnectionRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,30 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvpcpeer.endpoint import endpoint_data
 
-class RejectVpcPeerConnectionRequest(RpcRequest):
+class AcceptVpcPeerConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'VpcPeer', '2022-01-01', 'RejectVpcPeerConnection','vpcpeer')
+		RpcRequest.__init__(self, 'VpcPeer', '2022-01-01', 'AcceptVpcPeerConnection','vpcpeer')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ClientToken(self): # String
 		return self.get_body_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_body_params('ClientToken', ClientToken)
+	def get_ResourceGroupId(self): # String
+		return self.get_body_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_body_params('ResourceGroupId', ResourceGroupId)
 	def get_DryRun(self): # Boolean
 		return self.get_body_params().get('DryRun')
 
 	def set_DryRun(self, DryRun):  # Boolean
 		self.add_body_params('DryRun', DryRun)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_body_params().get('ResourceOwnerAccount')
```

### Comparing `aliyun-python-sdk-vpcpeer-1.0.0/setup.py` & `aliyun-python-sdk-vpcpeer-1.0.1/setup.py`

 * *Files identical despite different names*

