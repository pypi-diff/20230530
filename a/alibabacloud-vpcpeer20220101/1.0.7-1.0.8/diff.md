# Comparing `tmp/alibabacloud_vpcpeer20220101-1.0.7.tar.gz` & `tmp/alibabacloud_vpcpeer20220101-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_vpcpeer20220101-1.0.7.tar", last modified: Fri Feb 24 02:19:34 2023, max compression
+gzip compressed data, was "dist/alibabacloud_vpcpeer20220101-1.0.8.tar", last modified: Tue May 30 08:05:33 2023, max compression
```

## Comparing `alibabacloud_vpcpeer20220101-1.0.7.tar` & `alibabacloud_vpcpeer20220101-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      329 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2352 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1034 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/alibabacloud_vpcpeer20220101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/alibabacloud_vpcpeer20220101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27917 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/alibabacloud_vpcpeer20220101/client.py
--rw-r--r--   0 root         (0) root         (0)    48380 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/alibabacloud_vpcpeer20220101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/alibabacloud_vpcpeer20220101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2352 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/alibabacloud_vpcpeer20220101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/alibabacloud_vpcpeer20220101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/alibabacloud_vpcpeer20220101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/alibabacloud_vpcpeer20220101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/alibabacloud_vpcpeer20220101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2630 2023-02-24 02:19:34.000000 alibabacloud_vpcpeer20220101-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:05:33.000000 alibabacloud_vpcpeer20220101-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      379 2023-05-30 08:05:32.000000 alibabacloud_vpcpeer20220101-1.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-30 08:05:32.000000 alibabacloud_vpcpeer20220101-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-30 08:05:32.000000 alibabacloud_vpcpeer20220101-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-05-30 08:05:33.000000 alibabacloud_vpcpeer20220101-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-05-30 08:05:32.000000 alibabacloud_vpcpeer20220101-1.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-05-30 08:05:32.000000 alibabacloud_vpcpeer20220101-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:05:33.000000 alibabacloud_vpcpeer20220101-1.0.8/alibabacloud_vpcpeer20220101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-30 08:05:32.000000 alibabacloud_vpcpeer20220101-1.0.8/alibabacloud_vpcpeer20220101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39319 2023-05-30 08:05:32.000000 alibabacloud_vpcpeer20220101-1.0.8/alibabacloud_vpcpeer20220101/client.py
+-rw-r--r--   0 root         (0) root         (0)    66967 2023-05-30 08:05:32.000000 alibabacloud_vpcpeer20220101-1.0.8/alibabacloud_vpcpeer20220101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:05:33.000000 alibabacloud_vpcpeer20220101-1.0.8/alibabacloud_vpcpeer20220101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-05-30 08:05:33.000000 alibabacloud_vpcpeer20220101-1.0.8/alibabacloud_vpcpeer20220101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2023-05-30 08:05:33.000000 alibabacloud_vpcpeer20220101-1.0.8/alibabacloud_vpcpeer20220101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 08:05:33.000000 alibabacloud_vpcpeer20220101-1.0.8/alibabacloud_vpcpeer20220101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-30 08:05:33.000000 alibabacloud_vpcpeer20220101-1.0.8/alibabacloud_vpcpeer20220101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-30 08:05:33.000000 alibabacloud_vpcpeer20220101-1.0.8/alibabacloud_vpcpeer20220101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-30 08:05:33.000000 alibabacloud_vpcpeer20220101-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2630 2023-05-30 08:05:32.000000 alibabacloud_vpcpeer20220101-1.0.8/setup.py
```

### Comparing `alibabacloud_vpcpeer20220101-1.0.7/LICENSE` & `alibabacloud_vpcpeer20220101-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_vpcpeer20220101-1.0.7/PKG-INFO` & `alibabacloud_vpcpeer20220101-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_vpcpeer20220101
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud VpcPeer (20220101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_vpcpeer20220101-1.0.7/README-CN.md` & `alibabacloud_vpcpeer20220101-1.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_vpcpeer20220101-1.0.7/README.md` & `alibabacloud_vpcpeer20220101-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_vpcpeer20220101-1.0.7/alibabacloud_vpcpeer20220101/models.py` & `alibabacloud_vpcpeer20220101-1.0.8/alibabacloud_vpcpeer20220101/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 
 class AcceptVpcPeerConnectionRequest(TeaModel):
     def __init__(
         self,
         client_token: str = None,
         dry_run: bool = None,
         instance_id: str = None,
+        resource_group_id: str = None,
         resource_owner_account: str = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
         self.instance_id = instance_id
+        self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28,26 +30,30 @@
         result = dict()
         if self.client_token is not None:
             result['ClientToken'] = self.client_token
         if self.dry_run is not None:
             result['DryRun'] = self.dry_run
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ClientToken') is not None:
             self.client_token = m.get('ClientToken')
         if m.get('DryRun') is not None:
             self.dry_run = m.get('DryRun')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         return self
 
 
 class AcceptVpcPeerConnectionResponseBody(TeaModel):
     def __init__(
@@ -127,24 +133,26 @@
         accepting_region_id: str = None,
         accepting_vpc_id: str = None,
         client_token: str = None,
         description: str = None,
         dry_run: bool = None,
         name: str = None,
         region_id: str = None,
+        resource_group_id: str = None,
         vpc_id: str = None,
     ):
         self.accepting_ali_uid = accepting_ali_uid
         self.accepting_region_id = accepting_region_id
         self.accepting_vpc_id = accepting_vpc_id
         self.client_token = client_token
         self.description = description
         self.dry_run = dry_run
         self.name = name
         self.region_id = region_id
+        self.resource_group_id = resource_group_id
         self.vpc_id = vpc_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -164,14 +172,16 @@
             result['Description'] = self.description
         if self.dry_run is not None:
             result['DryRun'] = self.dry_run
         if self.name is not None:
             result['Name'] = self.name
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
         if self.vpc_id is not None:
             result['VpcId'] = self.vpc_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AcceptingAliUid') is not None:
@@ -186,14 +196,16 @@
             self.description = m.get('Description')
         if m.get('DryRun') is not None:
             self.dry_run = m.get('DryRun')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class CreateVpcPeerConnectionResponseBody(TeaModel):
     def __init__(
@@ -545,14 +557,15 @@
         gmt_expired: str = None,
         gmt_modified: str = None,
         instance_id: str = None,
         name: str = None,
         owner_id: int = None,
         region_id: str = None,
         request_id: str = None,
+        resource_group_id: str = None,
         status: str = None,
         tags: List[GetVpcPeerConnectionAttributeResponseBodyTags] = None,
         vpc: GetVpcPeerConnectionAttributeResponseBodyVpc = None,
     ):
         self.accepting_owner_uid = accepting_owner_uid
         self.accepting_region_id = accepting_region_id
         self.accepting_vpc = accepting_vpc
@@ -563,14 +576,15 @@
         self.gmt_expired = gmt_expired
         self.gmt_modified = gmt_modified
         self.instance_id = instance_id
         self.name = name
         self.owner_id = owner_id
         self.region_id = region_id
         self.request_id = request_id
+        self.resource_group_id = resource_group_id
         self.status = status
         self.tags = tags
         self.vpc = vpc
 
     def validate(self):
         if self.accepting_vpc:
             self.accepting_vpc.validate()
@@ -611,14 +625,16 @@
             result['Name'] = self.name
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
         if self.status is not None:
             result['Status'] = self.status
         result['Tags'] = []
         if self.tags is not None:
             for k in self.tags:
                 result['Tags'].append(k.to_map() if k else None)
         if self.vpc is not None:
@@ -652,14 +668,16 @@
             self.name = m.get('Name')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         self.tags = []
         if m.get('Tags') is not None:
             for k in m.get('Tags'):
                 temp_model = GetVpcPeerConnectionAttributeResponseBodyTags()
                 self.tags.append(temp_model.from_map(k))
@@ -709,14 +727,260 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetVpcPeerConnectionAttributeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListTagResourcesRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListTagResourcesRequest(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        region_id: str = None,
+        resource_id: List[str] = None,
+        resource_type: str = None,
+        tag: List[ListTagResourcesRequestTag] = None,
+    ):
+        self.max_results = max_results
+        self.next_token = next_token
+        self.region_id = region_id
+        self.resource_id = resource_id
+        self.resource_type = resource_type
+        self.tag = tag
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = ListTagResourcesRequestTag()
+                self.tag.append(temp_model.from_map(k))
+        return self
+
+
+class ListTagResourcesResponseBodyTagResources(TeaModel):
+    def __init__(
+        self,
+        region_no: str = None,
+        resource_id: str = None,
+        resource_type: str = None,
+        tag_key: str = None,
+        tag_value: str = None,
+    ):
+        self.region_no = region_no
+        self.resource_id = resource_id
+        self.resource_type = resource_type
+        self.tag_key = tag_key
+        self.tag_value = tag_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.region_no is not None:
+            result['RegionNo'] = self.region_no
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        if self.tag_value is not None:
+            result['TagValue'] = self.tag_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RegionNo') is not None:
+            self.region_no = m.get('RegionNo')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
+        return self
+
+
+class ListTagResourcesResponseBody(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        request_id: str = None,
+        tag_resources: List[ListTagResourcesResponseBodyTagResources] = None,
+    ):
+        self.max_results = max_results
+        self.next_token = next_token
+        self.request_id = request_id
+        self.tag_resources = tag_resources
+
+    def validate(self):
+        if self.tag_resources:
+            for k in self.tag_resources:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['TagResources'] = []
+        if self.tag_resources is not None:
+            for k in self.tag_resources:
+                result['TagResources'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.tag_resources = []
+        if m.get('TagResources') is not None:
+            for k in m.get('TagResources'):
+                temp_model = ListTagResourcesResponseBodyTagResources()
+                self.tag_resources.append(temp_model.from_map(k))
+        return self
+
+
+class ListTagResourcesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListTagResourcesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListTagResourcesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListVpcPeerConnectionsRequestTags(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
         self.key = key
@@ -750,22 +1014,24 @@
     def __init__(
         self,
         instance_id: str = None,
         max_results: int = None,
         name: str = None,
         next_token: str = None,
         region_id: str = None,
+        resource_group_id: str = None,
         tags: List[ListVpcPeerConnectionsRequestTags] = None,
         vpc_id: List[str] = None,
     ):
         self.instance_id = instance_id
         self.max_results = max_results
         self.name = name
         self.next_token = next_token
         self.region_id = region_id
+        self.resource_group_id = resource_group_id
         self.tags = tags
         self.vpc_id = vpc_id
 
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
@@ -783,14 +1049,16 @@
             result['MaxResults'] = self.max_results
         if self.name is not None:
             result['Name'] = self.name
         if self.next_token is not None:
             result['NextToken'] = self.next_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
         result['Tags'] = []
         if self.tags is not None:
             for k in self.tags:
                 result['Tags'].append(k.to_map() if k else None)
         if self.vpc_id is not None:
             result['VpcId'] = self.vpc_id
         return result
@@ -803,14 +1071,16 @@
             self.max_results = m.get('MaxResults')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('NextToken') is not None:
             self.next_token = m.get('NextToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
         self.tags = []
         if m.get('Tags') is not None:
             for k in m.get('Tags'):
                 temp_model = ListVpcPeerConnectionsRequestTags()
                 self.tags.append(temp_model.from_map(k))
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
@@ -854,22 +1124,24 @@
     def __init__(
         self,
         instance_id: str = None,
         max_results: int = None,
         name: str = None,
         next_token: str = None,
         region_id: str = None,
+        resource_group_id: str = None,
         tags: List[ListVpcPeerConnectionsShrinkRequestTags] = None,
         vpc_id_shrink: str = None,
     ):
         self.instance_id = instance_id
         self.max_results = max_results
         self.name = name
         self.next_token = next_token
         self.region_id = region_id
+        self.resource_group_id = resource_group_id
         self.tags = tags
         self.vpc_id_shrink = vpc_id_shrink
 
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
@@ -887,14 +1159,16 @@
             result['MaxResults'] = self.max_results
         if self.name is not None:
             result['Name'] = self.name
         if self.next_token is not None:
             result['NextToken'] = self.next_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
         result['Tags'] = []
         if self.tags is not None:
             for k in self.tags:
                 result['Tags'].append(k.to_map() if k else None)
         if self.vpc_id_shrink is not None:
             result['VpcId'] = self.vpc_id_shrink
         return result
@@ -907,14 +1181,16 @@
             self.max_results = m.get('MaxResults')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('NextToken') is not None:
             self.next_token = m.get('NextToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
         self.tags = []
         if m.get('Tags') is not None:
             for k in m.get('Tags'):
                 temp_model = ListVpcPeerConnectionsShrinkRequestTags()
                 self.tags.append(temp_model.from_map(k))
         if m.get('VpcId') is not None:
             self.vpc_id_shrink = m.get('VpcId')
@@ -1044,14 +1320,15 @@
         gmt_create: str = None,
         gmt_expired: str = None,
         gmt_modified: str = None,
         instance_id: str = None,
         name: str = None,
         owner_id: int = None,
         region_id: str = None,
+        resource_group_id: str = None,
         status: str = None,
         tags: List[ListVpcPeerConnectionsResponseBodyVpcPeerConnectsTags] = None,
         vpc: ListVpcPeerConnectionsResponseBodyVpcPeerConnectsVpc = None,
     ):
         self.accepting_owner_uid = accepting_owner_uid
         self.accepting_region_id = accepting_region_id
         self.accepting_vpc = accepting_vpc
@@ -1061,14 +1338,15 @@
         self.gmt_create = gmt_create
         self.gmt_expired = gmt_expired
         self.gmt_modified = gmt_modified
         self.instance_id = instance_id
         self.name = name
         self.owner_id = owner_id
         self.region_id = region_id
+        self.resource_group_id = resource_group_id
         self.status = status
         self.tags = tags
         self.vpc = vpc
 
     def validate(self):
         if self.accepting_vpc:
             self.accepting_vpc.validate()
@@ -1107,14 +1385,16 @@
             result['InstanceId'] = self.instance_id
         if self.name is not None:
             result['Name'] = self.name
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
         if self.status is not None:
             result['Status'] = self.status
         result['Tags'] = []
         if self.tags is not None:
             for k in self.tags:
                 result['Tags'].append(k.to_map() if k else None)
         if self.vpc is not None:
@@ -1146,14 +1426,16 @@
             self.instance_id = m.get('InstanceId')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         self.tags = []
         if m.get('Tags') is not None:
             for k in m.get('Tags'):
                 temp_model = ListVpcPeerConnectionsResponseBodyVpcPeerConnectsTags()
                 self.tags.append(temp_model.from_map(k))
@@ -1506,7 +1788,310 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RejectVpcPeerConnectionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class TagResourcesRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class TagResourcesRequest(TeaModel):
+    def __init__(
+        self,
+        client_token: str = None,
+        region_id: str = None,
+        resource_id: List[str] = None,
+        resource_type: str = None,
+        tag: List[TagResourcesRequestTag] = None,
+    ):
+        self.client_token = client_token
+        self.region_id = region_id
+        self.resource_id = resource_id
+        self.resource_type = resource_type
+        self.tag = tag
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = TagResourcesRequestTag()
+                self.tag.append(temp_model.from_map(k))
+        return self
+
+
+class TagResourcesResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class TagResourcesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: TagResourcesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = TagResourcesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UnTagResourcesRequest(TeaModel):
+    def __init__(
+        self,
+        all: bool = None,
+        client_token: str = None,
+        region_id: str = None,
+        resource_id: List[str] = None,
+        resource_type: str = None,
+        tag_key: List[str] = None,
+    ):
+        self.all = all
+        self.client_token = client_token
+        self.region_id = region_id
+        self.resource_id = resource_id
+        self.resource_type = resource_type
+        self.tag_key = tag_key
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.all is not None:
+            result['All'] = self.all
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('All') is not None:
+            self.all = m.get('All')
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        return self
+
+
+class UnTagResourcesResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class UnTagResourcesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UnTagResourcesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UnTagResourcesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_vpcpeer20220101-1.0.7/alibabacloud_vpcpeer20220101.egg-info/PKG-INFO` & `alibabacloud_vpcpeer20220101-1.0.8/alibabacloud_vpcpeer20220101.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-vpcpeer20220101
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud VpcPeer (20220101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_vpcpeer20220101-1.0.7/setup.py` & `alibabacloud_vpcpeer20220101-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_vpcpeer20220101.
 
-Created on 24/02/2023
+Created on 30/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_vpcpeer20220101"
 NAME = "alibabacloud_vpcpeer20220101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud VpcPeer (20220101) SDK Library for Python"
```

