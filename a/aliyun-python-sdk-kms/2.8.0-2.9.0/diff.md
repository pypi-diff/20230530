# Comparing `tmp/aliyun-python-sdk-kms-2.8.0.tar.gz` & `tmp/aliyun-python-sdk-kms-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-kms-2.8.0.tar", last modified: Tue Oct  8 03:28:14 2019, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-kms-2.9.0.tar", last modified: Tue Dec 31 06:51:59 2019, max compression
```

## Comparing `aliyun-python-sdk-kms-2.8.0.tar` & `aliyun-python-sdk-kms-2.9.0.tar`

### file list

```diff
@@ -1,47 +1,53 @@
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/
--rw-rw-r--   0 admin     (1140) admin     (1140)        0 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/MANIFEST.in
--rw-rw-r--   0 admin     (1140) admin     (1140)     2452 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/setup.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1537 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/PKG-INFO
--rw-rw-r--   0 admin     (1140) admin     (1140)       59 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/setup.cfg
--rw-rw-r--   0 admin     (1140) admin     (1140)      527 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/README.rst
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyun_python_sdk_kms.egg-info/
--rw-rw-r--   0 admin     (1140) admin     (1140)       30 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyun_python_sdk_kms.egg-info/requires.txt
--rw-rw-r--   0 admin     (1140) admin     (1140)     1537 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyun_python_sdk_kms.egg-info/PKG-INFO
--rw-rw-r--   0 admin     (1140) admin     (1140)       13 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyun_python_sdk_kms.egg-info/top_level.txt
--rw-rw-r--   0 admin     (1140) admin     (1140)        1 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyun_python_sdk_kms.egg-info/dependency_links.txt
--rw-rw-r--   0 admin     (1140) admin     (1140)     1961 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyun_python_sdk_kms.egg-info/SOURCES.txt
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/
--rw-rw-r--   0 admin     (1140) admin     (1140)        0 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/__init__.py
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/
--rw-rw-r--   0 admin     (1140) admin     (1140)     1756 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ListAliasesByKeyIdRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2008 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/GenerateDataKeyWithoutPlaintextRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1606 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/UpdateKeyDescriptionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2070 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ImportKeyMaterialRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1434 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DeleteAliasRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1594 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ListKeysRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1410 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DescribeKeyRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1782 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/EncryptRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1576 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/UpdateAliasRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1422 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DeleteKeyMaterialRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1406 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/EnableKeyRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1848 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/GetParametersForImportRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1568 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/UntagResourceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1652 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ScheduleKeyDeletionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1886 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/UpdateRotationPolicyRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1546 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/TagResourceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1608 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DescribeKeyVersionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2410 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/CreateKeyRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)        0 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/__init__.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1408 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DisableKeyRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1600 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ListAliasesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1750 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ListKeyVersionsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1670 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DecryptRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1276 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DescribeServiceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1976 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/GenerateDataKeyRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1276 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DescribeRegionsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1422 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/CancelKeyDeletionRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1576 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/CreateAliasRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1420 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ListResourceTagsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)       21 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/__init__.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1088 2019-10-08 03:28:14.000000 aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/endpoint.py
+drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2019-12-31 06:51:59.000000 aliyun-python-sdk-kms-2.9.0/
+-rw-rw-r--   0 admin     (1017) admin     (1017)        0 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/MANIFEST.in
+drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2019-12-31 06:51:59.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/
+-rw-rw-r--   0 admin     (1017) admin     (1017)       21 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/__init__.py
+drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2019-12-31 06:51:59.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/
+-rw-rw-r--   0 admin     (1017) admin     (1017)        0 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/__init__.py
+drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2019-12-31 06:51:59.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1608 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DescribeKeyVersionRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1434 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DeleteAliasRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1576 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/UpdateAliasRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1408 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DisableKeyRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1546 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/TagResourceRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1750 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ListKeyVersionsRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1938 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/AsymmetricEncryptRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)        0 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/__init__.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1420 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ListResourceTagsRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2008 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/GenerateDataKeyWithoutPlaintextRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1606 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/UpdateKeyDescriptionRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1848 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/GetParametersForImportRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1968 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/AsymmetricDecryptRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1276 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DescribeServiceRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1914 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/AsymmetricSignRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1406 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/EnableKeyRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1670 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DecryptRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1422 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DeleteKeyMaterialRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1422 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/CancelKeyDeletionRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1594 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ListKeysRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1576 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/CreateAliasRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1420 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/CreateKeyVersionRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1782 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/EncryptRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1600 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ListAliasesRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2564 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/CreateKeyRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2060 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/AsymmetricVerifyRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1568 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/UntagResourceRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1756 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ListAliasesByKeyIdRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2070 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ImportKeyMaterialRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1596 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/GetPublicKeyRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1276 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DescribeRegionsRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1886 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/UpdateRotationPolicyRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1410 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DescribeKeyRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1976 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/GenerateDataKeyRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1652 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ScheduleKeyDeletionRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1088 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/endpoint.py
+drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2019-12-31 06:51:59.000000 aliyun-python-sdk-kms-2.9.0/aliyun_python_sdk_kms.egg-info/
+-rw-rw-r--   0 admin     (1017) admin     (1017)        1 2019-12-31 06:51:59.000000 aliyun-python-sdk-kms-2.9.0/aliyun_python_sdk_kms.egg-info/dependency_links.txt
+-rw-rw-r--   0 admin     (1017) admin     (1017)       13 2019-12-31 06:51:59.000000 aliyun-python-sdk-kms-2.9.0/aliyun_python_sdk_kms.egg-info/top_level.txt
+-rw-rw-r--   0 admin     (1017) admin     (1017)       30 2019-12-31 06:51:59.000000 aliyun-python-sdk-kms-2.9.0/aliyun_python_sdk_kms.egg-info/requires.txt
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2305 2019-12-31 06:51:59.000000 aliyun-python-sdk-kms-2.9.0/aliyun_python_sdk_kms.egg-info/SOURCES.txt
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1537 2019-12-31 06:51:59.000000 aliyun-python-sdk-kms-2.9.0/aliyun_python_sdk_kms.egg-info/PKG-INFO
+-rw-rw-r--   0 admin     (1017) admin     (1017)       59 2019-12-31 06:51:59.000000 aliyun-python-sdk-kms-2.9.0/setup.cfg
+-rw-rw-r--   0 admin     (1017) admin     (1017)      527 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/README.rst
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1537 2019-12-31 06:51:59.000000 aliyun-python-sdk-kms-2.9.0/PKG-INFO
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2452 2019-12-31 06:51:58.000000 aliyun-python-sdk-kms-2.9.0/setup.py
```

### Comparing `aliyun-python-sdk-kms-2.8.0/setup.py` & `aliyun-python-sdk-kms-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/PKG-INFO` & `aliyun-python-sdk-kms-2.9.0/aliyun_python_sdk_kms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-kms
-Version: 2.8.0
+Version: 2.9.0
 Summary: The kms module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-kms
```

### Comparing `aliyun-python-sdk-kms-2.8.0/README.rst` & `aliyun-python-sdk-kms-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyun_python_sdk_kms.egg-info/PKG-INFO` & `aliyun-python-sdk-kms-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-kms
-Version: 2.8.0
+Version: 2.9.0
 Summary: The kms module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-kms
```

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyun_python_sdk_kms.egg-info/SOURCES.txt` & `aliyun-python-sdk-kms-2.9.0/aliyun_python_sdk_kms.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,30 +5,36 @@
 aliyun_python_sdk_kms.egg-info/SOURCES.txt
 aliyun_python_sdk_kms.egg-info/dependency_links.txt
 aliyun_python_sdk_kms.egg-info/requires.txt
 aliyun_python_sdk_kms.egg-info/top_level.txt
 aliyunsdkkms/__init__.py
 aliyunsdkkms/endpoint.py
 aliyunsdkkms/request/__init__.py
+aliyunsdkkms/request/v20160120/AsymmetricDecryptRequest.py
+aliyunsdkkms/request/v20160120/AsymmetricEncryptRequest.py
+aliyunsdkkms/request/v20160120/AsymmetricSignRequest.py
+aliyunsdkkms/request/v20160120/AsymmetricVerifyRequest.py
 aliyunsdkkms/request/v20160120/CancelKeyDeletionRequest.py
 aliyunsdkkms/request/v20160120/CreateAliasRequest.py
 aliyunsdkkms/request/v20160120/CreateKeyRequest.py
+aliyunsdkkms/request/v20160120/CreateKeyVersionRequest.py
 aliyunsdkkms/request/v20160120/DecryptRequest.py
 aliyunsdkkms/request/v20160120/DeleteAliasRequest.py
 aliyunsdkkms/request/v20160120/DeleteKeyMaterialRequest.py
 aliyunsdkkms/request/v20160120/DescribeKeyRequest.py
 aliyunsdkkms/request/v20160120/DescribeKeyVersionRequest.py
 aliyunsdkkms/request/v20160120/DescribeRegionsRequest.py
 aliyunsdkkms/request/v20160120/DescribeServiceRequest.py
 aliyunsdkkms/request/v20160120/DisableKeyRequest.py
 aliyunsdkkms/request/v20160120/EnableKeyRequest.py
 aliyunsdkkms/request/v20160120/EncryptRequest.py
 aliyunsdkkms/request/v20160120/GenerateDataKeyRequest.py
 aliyunsdkkms/request/v20160120/GenerateDataKeyWithoutPlaintextRequest.py
 aliyunsdkkms/request/v20160120/GetParametersForImportRequest.py
+aliyunsdkkms/request/v20160120/GetPublicKeyRequest.py
 aliyunsdkkms/request/v20160120/ImportKeyMaterialRequest.py
 aliyunsdkkms/request/v20160120/ListAliasesByKeyIdRequest.py
 aliyunsdkkms/request/v20160120/ListAliasesRequest.py
 aliyunsdkkms/request/v20160120/ListKeyVersionsRequest.py
 aliyunsdkkms/request/v20160120/ListKeysRequest.py
 aliyunsdkkms/request/v20160120/ListResourceTagsRequest.py
 aliyunsdkkms/request/v20160120/ScheduleKeyDeletionRequest.py
```

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ListAliasesByKeyIdRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ListAliasesByKeyIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/GenerateDataKeyWithoutPlaintextRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/GenerateDataKeyWithoutPlaintextRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/UpdateKeyDescriptionRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/UpdateKeyDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ImportKeyMaterialRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ImportKeyMaterialRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DeleteAliasRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DeleteAliasRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ListKeysRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ListKeysRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DescribeKeyRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DescribeKeyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/EncryptRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/EncryptRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/UpdateAliasRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/UpdateAliasRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DeleteKeyMaterialRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DeleteKeyMaterialRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/EnableKeyRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/EnableKeyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/GetParametersForImportRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/GetParametersForImportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/UntagResourceRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/UntagResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ScheduleKeyDeletionRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ScheduleKeyDeletionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/UpdateRotationPolicyRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/UpdateRotationPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/TagResourceRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/TagResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DescribeKeyVersionRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DescribeKeyVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/CreateKeyRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/CreateKeyRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,20 @@
 
 	def get_Description(self):
 		return self.get_query_params().get('Description')
 
 	def set_Description(self,Description):
 		self.add_query_param('Description',Description)
 
+	def get_KeySpec(self):
+		return self.get_query_params().get('KeySpec')
+
+	def set_KeySpec(self,KeySpec):
+		self.add_query_param('KeySpec',KeySpec)
+
 	def get_RotationInterval(self):
 		return self.get_query_params().get('RotationInterval')
 
 	def set_RotationInterval(self,RotationInterval):
 		self.add_query_param('RotationInterval',RotationInterval)
 
 	def get_EnableAutomaticRotation(self):
```

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DisableKeyRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DisableKeyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ListAliasesRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ListAliasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ListKeyVersionsRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ListKeyVersionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DecryptRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DecryptRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DescribeServiceRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DescribeServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/GenerateDataKeyRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/GenerateDataKeyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/DescribeRegionsRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/CancelKeyDeletionRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/CancelKeyDeletionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/CreateAliasRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/CreateAliasRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/request/v20160120/ListResourceTagsRequest.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/request/v20160120/ListResourceTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-kms-2.8.0/aliyunsdkkms/endpoint.py` & `aliyun-python-sdk-kms-2.9.0/aliyunsdkkms/endpoint.py`

 * *Files identical despite different names*

