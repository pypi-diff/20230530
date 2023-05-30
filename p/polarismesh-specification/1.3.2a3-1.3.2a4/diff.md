# Comparing `tmp/polarismesh_specification-1.3.2a3.tar.gz` & `tmp/polarismesh_specification-1.3.2a4.tar.gz`

## Comparing `polarismesh_specification-1.3.2a3.tar` & `polarismesh_specification-1.3.2a4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
--rw-r--r--   0        0        0     8796 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
--rw-r--r--   0        0        0    16012 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
--rw-r--r--   0        0        0     8034 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
--rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
--rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
--rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/__init__.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/__init__.pyi
--rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/code_pb2.py
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/code_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/model_pb2.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/model_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/namespace_pb2.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/security/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/security/__init__.pyi
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/security/auth_pb2.py
--rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
--rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
--rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
--rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
--rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
--rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
--rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
--rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
--rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
--rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/.gitignore
--rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/LICENSE.txt
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/README.md
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/pyproject.toml
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a3/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
+-rw-r--r--   0        0        0     8796 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
+-rw-r--r--   0        0        0    16012 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
+-rw-r--r--   0        0        0     8034 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
+-rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
+-rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
+-rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/__init__.pyi
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/code_pb2.py
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/code_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/model_pb2.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/namespace_pb2.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/security/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/security/__init__.pyi
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/security/auth_pb2.py
+-rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
+-rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
+-rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
+-rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
+-rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
+-rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
+-rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
+-rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
+-rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
+-rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/.gitignore
+-rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/LICENSE.txt
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/README.md
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/pyproject.toml
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a4/PKG-INFO
```

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/code_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/code_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/code_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/model_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/model_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/model_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/namespace_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/namespace_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/security/auth_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/security/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/security/auth_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/security/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/client_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/client_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 from ..service_manage import client_pb2 as client__pb2
 from ..service_manage import service_pb2 as service__pb2
 from ..service_manage import request_pb2 as request__pb2
 from ..service_manage import response_pb2 as response__pb2
 from ..service_manage import heartbeat_pb2 as heartbeat__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rgrpcapi.proto\x12\x02v1\x1a\x0c\x63lient.proto\x1a\rservice.proto\x1a\rrequest.proto\x1a\x0eresponse.proto\x1a\x0fheartbeat.proto2\xe6\x03\n\x0bPolarisGRPC\x12*\n\x0cReportClient\x12\n.v1.Client\x1a\x0c.v1.Response\"\x00\x12\x30\n\x10RegisterInstance\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12\x32\n\x12\x44\x65registerInstance\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12;\n\x08\x44iscover\x12\x13.v1.DiscoverRequest\x1a\x14.v1.DiscoverResponse\"\x00(\x01\x30\x01\x12)\n\tHeartbeat\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12\x45\n\x0e\x42\x61tchHeartbeat\x12\x15.v1.HeartbeatsRequest\x1a\x16.v1.HeartbeatsResponse\"\x00(\x01\x30\x01\x12J\n\x11\x42\x61tchGetHeartbeat\x12\x18.v1.GetHeartbeatsRequest\x1a\x19.v1.GetHeartbeatsResponse\"\x00\x12J\n\x11\x42\x61tchDelHeartbeat\x12\x18.v1.DelHeartbeatsRequest\x1a\x19.v1.DelHeartbeatsResponse\"\x00\x42\x93\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\x12PolarisGRPCServiceZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rgrpcapi.proto\x12\x02v1\x1a\x0c\x63lient.proto\x1a\rservice.proto\x1a\rrequest.proto\x1a\x0eresponse.proto\x1a\x0fheartbeat.proto2\x87\x02\n\x0bPolarisGRPC\x12*\n\x0cReportClient\x12\n.v1.Client\x1a\x0c.v1.Response\"\x00\x12\x30\n\x10RegisterInstance\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12\x32\n\x12\x44\x65registerInstance\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x12;\n\x08\x44iscover\x12\x13.v1.DiscoverRequest\x1a\x14.v1.DiscoverResponse\"\x00(\x01\x30\x01\x12)\n\tHeartbeat\x12\x0c.v1.Instance\x1a\x0c.v1.Response\"\x00\x32\xf5\x01\n\x14PolarisHeartbeatGRPC\x12\x45\n\x0e\x42\x61tchHeartbeat\x12\x15.v1.HeartbeatsRequest\x1a\x16.v1.HeartbeatsResponse\"\x00(\x01\x30\x01\x12J\n\x11\x42\x61tchGetHeartbeat\x12\x18.v1.GetHeartbeatsRequest\x1a\x19.v1.GetHeartbeatsResponse\"\x00\x12J\n\x11\x42\x61tchDelHeartbeat\x12\x18.v1.DelHeartbeatsRequest\x1a\x19.v1.DelHeartbeatsResponse\"\x00\x42\x93\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\x12PolarisGRPCServiceZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpcapi_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageB\022PolarisGRPCServiceZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
   _POLARISGRPC._serialized_start=99
-  _POLARISGRPC._serialized_end=585
+  _POLARISGRPC._serialized_end=362
+  _POLARISHEARTBEATGRPC._serialized_start=365
+  _POLARISHEARTBEATGRPC._serialized_end=610
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,29 +39,14 @@
                 response_deserializer=response__pb2.DiscoverResponse.FromString,
                 )
         self.Heartbeat = channel.unary_unary(
                 '/v1.PolarisGRPC/Heartbeat',
                 request_serializer=service__pb2.Instance.SerializeToString,
                 response_deserializer=response__pb2.Response.FromString,
                 )
-        self.BatchHeartbeat = channel.stream_stream(
-                '/v1.PolarisGRPC/BatchHeartbeat',
-                request_serializer=heartbeat__pb2.HeartbeatsRequest.SerializeToString,
-                response_deserializer=heartbeat__pb2.HeartbeatsResponse.FromString,
-                )
-        self.BatchGetHeartbeat = channel.unary_unary(
-                '/v1.PolarisGRPC/BatchGetHeartbeat',
-                request_serializer=heartbeat__pb2.GetHeartbeatsRequest.SerializeToString,
-                response_deserializer=heartbeat__pb2.GetHeartbeatsResponse.FromString,
-                )
-        self.BatchDelHeartbeat = channel.unary_unary(
-                '/v1.PolarisGRPC/BatchDelHeartbeat',
-                request_serializer=heartbeat__pb2.DelHeartbeatsRequest.SerializeToString,
-                response_deserializer=heartbeat__pb2.DelHeartbeatsResponse.FromString,
-                )
 
 
 class PolarisGRPCServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def ReportClient(self, request, context):
         """客户端上报
@@ -94,35 +79,14 @@
     def Heartbeat(self, request, context):
         """被调方上报心跳
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def BatchHeartbeat(self, request_iterator, context):
-        """被调方批量上报心跳
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def BatchGetHeartbeat(self, request, context):
-        """批量获取心跳记录
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def BatchDelHeartbeat(self, request, context):
-        """批量删除心跳记录
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
 
 def add_PolarisGRPCServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ReportClient': grpc.unary_unary_rpc_method_handler(
                     servicer.ReportClient,
                     request_deserializer=client__pb2.Client.FromString,
                     response_serializer=response__pb2.Response.SerializeToString,
@@ -143,29 +107,14 @@
                     response_serializer=response__pb2.DiscoverResponse.SerializeToString,
             ),
             'Heartbeat': grpc.unary_unary_rpc_method_handler(
                     servicer.Heartbeat,
                     request_deserializer=service__pb2.Instance.FromString,
                     response_serializer=response__pb2.Response.SerializeToString,
             ),
-            'BatchHeartbeat': grpc.stream_stream_rpc_method_handler(
-                    servicer.BatchHeartbeat,
-                    request_deserializer=heartbeat__pb2.HeartbeatsRequest.FromString,
-                    response_serializer=heartbeat__pb2.HeartbeatsResponse.SerializeToString,
-            ),
-            'BatchGetHeartbeat': grpc.unary_unary_rpc_method_handler(
-                    servicer.BatchGetHeartbeat,
-                    request_deserializer=heartbeat__pb2.GetHeartbeatsRequest.FromString,
-                    response_serializer=heartbeat__pb2.GetHeartbeatsResponse.SerializeToString,
-            ),
-            'BatchDelHeartbeat': grpc.unary_unary_rpc_method_handler(
-                    servicer.BatchDelHeartbeat,
-                    request_deserializer=heartbeat__pb2.DelHeartbeatsRequest.FromString,
-                    response_serializer=heartbeat__pb2.DelHeartbeatsResponse.SerializeToString,
-            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'v1.PolarisGRPC', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -253,26 +202,105 @@
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/v1.PolarisGRPC/Heartbeat',
             service__pb2.Instance.SerializeToString,
             response__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
+
+class PolarisHeartbeatGRPCStub(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.BatchHeartbeat = channel.stream_stream(
+                '/v1.PolarisHeartbeatGRPC/BatchHeartbeat',
+                request_serializer=heartbeat__pb2.HeartbeatsRequest.SerializeToString,
+                response_deserializer=heartbeat__pb2.HeartbeatsResponse.FromString,
+                )
+        self.BatchGetHeartbeat = channel.unary_unary(
+                '/v1.PolarisHeartbeatGRPC/BatchGetHeartbeat',
+                request_serializer=heartbeat__pb2.GetHeartbeatsRequest.SerializeToString,
+                response_deserializer=heartbeat__pb2.GetHeartbeatsResponse.FromString,
+                )
+        self.BatchDelHeartbeat = channel.unary_unary(
+                '/v1.PolarisHeartbeatGRPC/BatchDelHeartbeat',
+                request_serializer=heartbeat__pb2.DelHeartbeatsRequest.SerializeToString,
+                response_deserializer=heartbeat__pb2.DelHeartbeatsResponse.FromString,
+                )
+
+
+class PolarisHeartbeatGRPCServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def BatchHeartbeat(self, request_iterator, context):
+        """被调方批量上报心跳
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def BatchGetHeartbeat(self, request, context):
+        """批量获取心跳记录
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def BatchDelHeartbeat(self, request, context):
+        """批量删除心跳记录
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_PolarisHeartbeatGRPCServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'BatchHeartbeat': grpc.stream_stream_rpc_method_handler(
+                    servicer.BatchHeartbeat,
+                    request_deserializer=heartbeat__pb2.HeartbeatsRequest.FromString,
+                    response_serializer=heartbeat__pb2.HeartbeatsResponse.SerializeToString,
+            ),
+            'BatchGetHeartbeat': grpc.unary_unary_rpc_method_handler(
+                    servicer.BatchGetHeartbeat,
+                    request_deserializer=heartbeat__pb2.GetHeartbeatsRequest.FromString,
+                    response_serializer=heartbeat__pb2.GetHeartbeatsResponse.SerializeToString,
+            ),
+            'BatchDelHeartbeat': grpc.unary_unary_rpc_method_handler(
+                    servicer.BatchDelHeartbeat,
+                    request_deserializer=heartbeat__pb2.DelHeartbeatsRequest.FromString,
+                    response_serializer=heartbeat__pb2.DelHeartbeatsResponse.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'v1.PolarisHeartbeatGRPC', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class PolarisHeartbeatGRPC(object):
+    """Missing associated documentation comment in .proto file."""
+
     @staticmethod
     def BatchHeartbeat(request_iterator,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.stream_stream(request_iterator, target, '/v1.PolarisGRPC/BatchHeartbeat',
+        return grpc.experimental.stream_stream(request_iterator, target, '/v1.PolarisHeartbeatGRPC/BatchHeartbeat',
             heartbeat__pb2.HeartbeatsRequest.SerializeToString,
             heartbeat__pb2.HeartbeatsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def BatchGetHeartbeat(request,
@@ -281,15 +309,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/v1.PolarisGRPC/BatchGetHeartbeat',
+        return grpc.experimental.unary_unary(request, target, '/v1.PolarisHeartbeatGRPC/BatchGetHeartbeat',
             heartbeat__pb2.GetHeartbeatsRequest.SerializeToString,
             heartbeat__pb2.GetHeartbeatsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def BatchDelHeartbeat(request,
@@ -298,12 +326,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/v1.PolarisGRPC/BatchDelHeartbeat',
+        return grpc.experimental.unary_unary(request, target, '/v1.PolarisHeartbeatGRPC/BatchDelHeartbeat',
             heartbeat__pb2.DelHeartbeatsRequest.SerializeToString,
             heartbeat__pb2.DelHeartbeatsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/request_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/request_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/response_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/response_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/service_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/service_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi` & `polarismesh_specification-1.3.2a4/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/LICENSE.txt` & `polarismesh_specification-1.3.2a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/README.md` & `polarismesh_specification-1.3.2a4/README.md`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/pyproject.toml` & `polarismesh_specification-1.3.2a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a3/PKG-INFO` & `polarismesh_specification-1.3.2a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polarismesh-specification
-Version: 1.3.2a3
+Version: 1.3.2a4
 Project-URL: Documentation, https://github.com/polarismesh/specification#readme
 Project-URL: Issues, https://github.com/polarismesh/specification/issues
 Project-URL: Source, https://github.com/polarismesh/specification
 Author-email: "{authemail@qq.com}" <authemail@qq.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

