# Comparing `tmp/qwak_core-0.0.87.tar.gz` & `tmp/qwak_core-0.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.87.tar", max compression
+gzip compressed data, was "qwak_core-0.0.88.tar", max compression
```

## Comparing `qwak_core-0.0.87.tar` & `qwak_core-0.0.88.tar`

### file list

```diff
@@ -1,582 +1,582 @@
--rw-r--r--   0        0        0      264 2023-05-29 14:46:06.332707 qwak_core-0.0.87/README.md
--rw-r--r--   0        0        0        0 2023-05-29 14:47:37.745174 qwak_core-0.0.87/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-29 14:47:37.765174 qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-29 14:47:19.201079 qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.765174 qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-29 14:47:37.761174 qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-29 14:47:18.873078 qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.761174 qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-29 14:47:37.765174 qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-29 14:47:19.037079 qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.765174 qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-29 14:47:37.757174 qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-29 14:47:18.385075 qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-29 14:47:37.757174 qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-29 14:47:37.757174 qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-29 14:47:18.549076 qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.757174 qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-29 14:47:37.761174 qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-29 14:47:18.709077 qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.761174 qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-29 14:47:37.745174 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-29 14:47:18.225074 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-29 14:47:37.745174 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5707 2023-05-29 14:47:37.745174 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8170 2023-05-29 14:47:19.361080 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.749174 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-29 14:47:37.749174 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-29 14:47:19.685082 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.749174 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-29 14:47:37.753174 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-29 14:47:19.853083 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-29 14:47:37.753174 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-29 14:47:37.749174 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-29 14:47:19.525081 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.749174 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-29 14:47:37.753174 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-29 14:47:20.017084 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.753174 qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-29 14:47:37.793175 qwak_core-0.0.87/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-29 14:47:22.321096 qwak_core-0.0.87/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.793175 qwak_core-0.0.87/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-29 14:47:37.797175 qwak_core-0.0.87/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-29 14:47:22.489096 qwak_core-0.0.87/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-29 14:47:37.797175 qwak_core-0.0.87/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-29 14:47:37.941175 qwak_core-0.0.87/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-29 14:47:27.217121 qwak_core-0.0.87/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.941175 qwak_core-0.0.87/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-29 14:47:37.941175 qwak_core-0.0.87/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-29 14:47:27.381121 qwak_core-0.0.87/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-29 14:47:37.945175 qwak_core-0.0.87/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-29 14:47:37.945175 qwak_core-0.0.87/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-29 14:47:28.221126 qwak_core-0.0.87/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-29 14:47:37.949175 qwak_core-0.0.87/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-29 14:47:37.945175 qwak_core-0.0.87/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-29 14:47:28.057125 qwak_core-0.0.87/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.945175 qwak_core-0.0.87/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-05-29 14:47:37.949175 qwak_core-0.0.87/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-05-29 14:47:28.381126 qwak_core-0.0.87/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.949175 qwak_core-0.0.87/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-29 14:47:37.949175 qwak_core-0.0.87/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-29 14:47:28.541127 qwak_core-0.0.87/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-29 14:47:37.953175 qwak_core-0.0.87/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-29 14:47:38.029176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-29 14:47:35.549163 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.033176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-05-29 14:47:38.025176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-05-29 14:47:35.225162 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.029176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-29 14:47:38.029176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-29 14:47:35.385162 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.029176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-29 14:47:38.021176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-29 14:47:34.889160 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-29 14:47:38.025176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-29 14:47:38.025176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-29 14:47:35.061161 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.025176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-29 14:47:38.037176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-29 14:47:36.029166 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.037176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-29 14:47:38.033176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-29 14:47:35.869165 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.033176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-29 14:47:38.033176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-29 14:47:35.709164 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.033176 qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-29 14:47:38.021176 qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-29 14:47:34.713159 qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.021176 qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-29 14:47:38.017176 qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-29 14:47:34.373157 qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.017176 qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-29 14:47:38.017176 qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-29 14:47:34.553158 qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-29 14:47:38.021176 qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    20255 2023-05-29 14:47:37.973175 qwak_core-0.0.87/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    17495 2023-05-29 14:47:30.205136 qwak_core-0.0.87/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    20359 2023-05-29 14:47:37.973175 qwak_core-0.0.87/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-29 14:47:37.973175 qwak_core-0.0.87/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-29 14:47:30.041135 qwak_core-0.0.87/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.973175 qwak_core-0.0.87/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11691 2023-05-29 14:47:37.965175 qwak_core-0.0.87/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18850 2023-05-29 14:47:29.717133 qwak_core-0.0.87/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.965175 qwak_core-0.0.87/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-29 14:47:37.965175 qwak_core-0.0.87/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-29 14:47:29.877134 qwak_core-0.0.87/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.965175 qwak_core-0.0.87/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-29 14:47:37.969175 qwak_core-0.0.87/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-29 14:47:30.369137 qwak_core-0.0.87/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-29 14:47:37.969175 qwak_core-0.0.87/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-29 14:47:37.969175 qwak_core-0.0.87/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-29 14:47:30.717139 qwak_core-0.0.87/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-29 14:47:37.969175 qwak_core-0.0.87/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-29 14:47:37.981176 qwak_core-0.0.87/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-29 14:47:31.057140 qwak_core-0.0.87/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.981176 qwak_core-0.0.87/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-29 14:47:37.981176 qwak_core-0.0.87/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-29 14:47:31.221141 qwak_core-0.0.87/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-29 14:47:37.981176 qwak_core-0.0.87/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-29 14:47:37.957175 qwak_core-0.0.87/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-29 14:47:29.225131 qwak_core-0.0.87/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.961175 qwak_core-0.0.87/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-29 14:47:37.961175 qwak_core-0.0.87/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-29 14:47:29.389132 qwak_core-0.0.87/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-29 14:47:37.961175 qwak_core-0.0.87/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-29 14:47:37.953175 qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-29 14:47:28.885129 qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.957175 qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-29 14:47:37.953175 qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-29 14:47:28.717128 qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.953175 qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-29 14:47:37.957175 qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-29 14:47:29.061130 qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-29 14:47:37.957175 qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-29 14:47:37.781175 qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-29 14:47:21.493091 qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.781175 qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-29 14:47:37.785174 qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-29 14:47:21.665092 qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.785174 qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-29 14:47:37.785174 qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-29 14:47:21.829093 qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-29 14:47:37.785174 qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-29 14:47:37.925175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-29 14:47:26.221115 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.925175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-29 14:47:37.921175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-29 14:47:26.057115 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-29 14:47:37.921175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2023-05-29 14:47:37.905175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2023-05-29 14:47:24.557107 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.905175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2023-05-29 14:47:37.901175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2023-05-29 14:47:24.377106 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.905175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-29 14:47:37.897175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-29 14:47:23.821103 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.897175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-29 14:47:37.901175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-29 14:47:24.177105 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-29 14:47:37.901175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-29 14:47:37.905175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-29 14:47:24.729108 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.909175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-29 14:47:37.909175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-29 14:47:24.893109 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-29 14:47:37.909175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25269 2023-05-29 14:47:37.897175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37664 2023-05-29 14:47:23.997104 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.901175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-29 14:47:37.909175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-29 14:47:25.061110 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.913175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    11277 2023-05-29 14:47:37.913175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    15070 2023-05-29 14:47:25.229110 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.913175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-29 14:47:37.925175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-29 14:47:37.209172 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.925175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-29 14:47:37.929175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-29 14:47:37.405173 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-29 14:47:37.929175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-29 14:47:37.929175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-29 14:47:26.717118 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.929175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-29 14:47:37.933175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-29 14:47:26.881119 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-29 14:47:37.933175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-29 14:47:37.933175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-29 14:47:27.045120 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.933175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-29 14:47:37.937175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-29 14:47:27.717123 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.937175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-29 14:47:37.937175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-29 14:47:27.545122 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-29 14:47:37.937175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-29 14:47:37.941175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-29 14:47:27.889124 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.941175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-29 14:47:37.913175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-29 14:47:25.397111 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.917175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-29 14:47:37.917175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-29 14:47:25.561112 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.917175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-29 14:47:37.917175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-29 14:47:25.729113 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-29 14:47:37.921175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-29 14:47:37.921175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-29 14:47:25.893114 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.921175 qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-29 14:47:38.037176 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-29 14:47:36.197167 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.041176 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-29 14:47:38.041176 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-29 14:47:36.357167 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-29 14:47:38.041176 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-29 14:47:38.041176 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-29 14:47:36.521168 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.041176 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-29 14:47:38.045176 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-29 14:47:36.689169 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-29 14:47:38.045176 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-29 14:47:38.045176 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-29 14:47:36.861170 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-29 14:47:38.045176 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-29 14:47:38.049176 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-29 14:47:37.029171 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.049176 qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-29 14:47:37.981176 qwak_core-0.0.87/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-29 14:47:31.381142 qwak_core-0.0.87/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.985175 qwak_core-0.0.87/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-29 14:47:37.985175 qwak_core-0.0.87/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-29 14:47:31.541143 qwak_core-0.0.87/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-29 14:47:37.985175 qwak_core-0.0.87/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-29 14:47:37.813175 qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-29 14:47:23.157100 qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.825175 qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-29 14:47:37.837175 qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-29 14:47:23.321101 qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.849175 qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-29 14:47:37.861175 qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-29 14:47:23.485102 qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-29 14:47:37.873175 qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-29 14:47:37.885175 qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-29 14:47:23.649102 qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.897175 qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-29 14:47:37.961175 qwak_core-0.0.87/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-29 14:47:29.553133 qwak_core-0.0.87/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-29 14:47:37.961175 qwak_core-0.0.87/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-05-29 14:47:37.985175 qwak_core-0.0.87/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-05-29 14:47:31.701144 qwak_core-0.0.87/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.989176 qwak_core-0.0.87/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-05-29 14:47:37.989176 qwak_core-0.0.87/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-05-29 14:47:31.861144 qwak_core-0.0.87/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-05-29 14:47:37.989176 qwak_core-0.0.87/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-29 14:47:38.001175 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-29 14:47:32.853150 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.001175 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-29 14:47:38.001175 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-29 14:47:33.033151 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.001175 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-29 14:47:38.005176 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-29 14:47:33.201151 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.005176 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-29 14:47:38.005176 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-29 14:47:33.365152 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.005176 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-29 14:47:38.009176 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-29 14:47:33.537153 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.009176 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-29 14:47:38.009176 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-29 14:47:33.717154 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-29 14:47:38.009176 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-29 14:47:38.013176 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-29 14:47:33.881155 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.013176 qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-29 14:47:37.993176 qwak_core-0.0.87/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-29 14:47:32.185146 qwak_core-0.0.87/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.993176 qwak_core-0.0.87/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-29 14:47:37.997176 qwak_core-0.0.87/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-29 14:47:32.669149 qwak_core-0.0.87/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.997176 qwak_core-0.0.87/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-29 14:47:37.993176 qwak_core-0.0.87/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-29 14:47:32.349147 qwak_core-0.0.87/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-29 14:47:37.993176 qwak_core-0.0.87/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-05-29 14:47:37.997176 qwak_core-0.0.87/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-05-29 14:47:32.513148 qwak_core-0.0.87/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.997176 qwak_core-0.0.87/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-29 14:47:37.977176 qwak_core-0.0.87/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-29 14:47:30.893139 qwak_core-0.0.87/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-29 14:47:37.977176 qwak_core-0.0.87/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-29 14:47:37.777175 qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-29 14:47:22.821098 qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-29 14:47:37.781175 qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-29 14:47:37.777175 qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-29 14:47:22.653097 qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.777175 qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-29 14:47:37.781175 qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-29 14:47:22.993099 qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-29 14:47:37.781175 qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-29 14:47:37.977176 qwak_core-0.0.87/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-29 14:47:30.541138 qwak_core-0.0.87/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-29 14:47:37.977176 qwak_core-0.0.87/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-29 14:47:37.989176 qwak_core-0.0.87/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-29 14:47:32.021145 qwak_core-0.0.87/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-29 14:47:37.993176 qwak_core-0.0.87/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-29 14:47:37.773174 qwak_core-0.0.87/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-29 14:47:20.829088 qwak_core-0.0.87/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.777175 qwak_core-0.0.87/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-29 14:47:37.773174 qwak_core-0.0.87/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-29 14:47:20.665087 qwak_core-0.0.87/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-29 14:47:37.773174 qwak_core-0.0.87/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-29 14:47:37.765174 qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-29 14:47:20.177085 qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.769174 qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-29 14:47:37.769174 qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-29 14:47:20.341085 qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.769174 qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-29 14:47:37.769174 qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-29 14:47:20.501086 qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-29 14:47:37.773174 qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-29 14:47:38.013176 qwak_core-0.0.87/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-29 14:47:34.209156 qwak_core-0.0.87/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-29 14:47:38.017176 qwak_core-0.0.87/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-29 14:47:38.013176 qwak_core-0.0.87/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-29 14:47:34.045156 qwak_core-0.0.87/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:38.013176 qwak_core-0.0.87/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    10851 2023-05-29 14:47:37.789175 qwak_core-0.0.87/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    13974 2023-05-29 14:47:21.993094 qwak_core-0.0.87/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.789175 qwak_core-0.0.87/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3044 2023-05-29 14:47:37.789175 qwak_core-0.0.87/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2641 2023-05-29 14:47:22.153095 qwak_core-0.0.87/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 14:47:37.793175 qwak_core-0.0.87/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-29 14:47:40.633189 qwak_core-0.0.87/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-29 14:47:40.633189 qwak_core-0.0.87/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-29 14:46:06.332707 qwak_core-0.0.87/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14847 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-29 14:46:06.336707 qwak_core-0.0.87/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-29 14:46:06.340707 qwak_core-0.0.87/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.87/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.87/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-30 08:55:08.428245 qwak_core-0.0.88/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 08:56:51.538623 qwak_core-0.0.88/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-30 08:56:51.558623 qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-30 08:56:31.670165 qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.562624 qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-30 08:56:51.554623 qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-30 08:56:31.322157 qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.558623 qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-30 08:56:51.558623 qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-30 08:56:31.494161 qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.558623 qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-30 08:56:51.550623 qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-30 08:56:30.798145 qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-30 08:56:51.550623 qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-30 08:56:51.550623 qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-30 08:56:30.974149 qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.554623 qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4901 2023-05-30 08:56:51.554623 qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5995 2023-05-30 08:56:31.146153 qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.554623 qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-30 08:56:51.538623 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-30 08:56:30.622141 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-30 08:56:51.538623 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5707 2023-05-30 08:56:51.538623 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8170 2023-05-30 08:56:31.846169 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.542623 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-30 08:56:51.542623 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-30 08:56:32.194177 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.546623 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-30 08:56:51.546623 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-30 08:56:32.370181 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-30 08:56:51.546623 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-30 08:56:51.542623 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-30 08:56:32.022173 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.542623 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-30 08:56:51.546623 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-30 08:56:32.550185 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.550623 qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-30 08:56:51.590624 qwak_core-0.0.88/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-30 08:56:35.046243 qwak_core-0.0.88/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.590624 qwak_core-0.0.88/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-30 08:56:51.590624 qwak_core-0.0.88/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-30 08:56:35.226247 qwak_core-0.0.88/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-30 08:56:51.590624 qwak_core-0.0.88/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-30 08:56:51.658626 qwak_core-0.0.88/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-30 08:56:40.326364 qwak_core-0.0.88/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.658626 qwak_core-0.0.88/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-30 08:56:51.658626 qwak_core-0.0.88/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-30 08:56:40.502369 qwak_core-0.0.88/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-30 08:56:51.658626 qwak_core-0.0.88/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-30 08:56:51.662626 qwak_core-0.0.88/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-30 08:56:41.390389 qwak_core-0.0.88/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-30 08:56:51.662626 qwak_core-0.0.88/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-30 08:56:51.662626 qwak_core-0.0.88/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-30 08:56:41.214385 qwak_core-0.0.88/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.662626 qwak_core-0.0.88/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-05-30 08:56:51.666626 qwak_core-0.0.88/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-05-30 08:56:41.566393 qwak_core-0.0.88/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.666626 qwak_core-0.0.88/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-30 08:56:51.666626 qwak_core-0.0.88/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-30 08:56:41.746397 qwak_core-0.0.88/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-30 08:56:51.666626 qwak_core-0.0.88/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-30 08:56:51.754628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-30 08:56:49.322572 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.754628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-05-30 08:56:51.750628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-05-30 08:56:48.962564 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.750628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-30 08:56:51.754628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-30 08:56:49.138568 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.754628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-30 08:56:51.746628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-30 08:56:48.602555 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-30 08:56:51.746628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-30 08:56:51.750628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-30 08:56:48.786559 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.750628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-30 08:56:51.762628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-30 08:56:49.846584 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.762628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-30 08:56:51.758628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-30 08:56:49.670580 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.758628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-30 08:56:51.758628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-30 08:56:49.498576 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.758628 qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-30 08:56:51.746628 qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-30 08:56:48.418551 qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.746628 qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-30 08:56:51.738628 qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-30 08:56:48.030542 qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.742628 qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-30 08:56:51.742628 qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-30 08:56:48.246547 qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-30 08:56:51.742628 qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20255 2023-05-30 08:56:51.694627 qwak_core-0.0.88/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    17495 2023-05-30 08:56:43.562439 qwak_core-0.0.88/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-05-30 08:56:51.694627 qwak_core-0.0.88/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-30 08:56:51.690626 qwak_core-0.0.88/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-30 08:56:43.378435 qwak_core-0.0.88/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.690626 qwak_core-0.0.88/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11691 2023-05-30 08:56:51.682626 qwak_core-0.0.88/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18850 2023-05-30 08:56:43.014426 qwak_core-0.0.88/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.682626 qwak_core-0.0.88/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-30 08:56:51.682626 qwak_core-0.0.88/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-30 08:56:43.194430 qwak_core-0.0.88/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.686627 qwak_core-0.0.88/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-30 08:56:51.686627 qwak_core-0.0.88/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-30 08:56:43.738443 qwak_core-0.0.88/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-30 08:56:51.686627 qwak_core-0.0.88/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-30 08:56:51.686627 qwak_core-0.0.88/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-30 08:56:44.122452 qwak_core-0.0.88/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-30 08:56:51.690626 qwak_core-0.0.88/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-30 08:56:51.698627 qwak_core-0.0.88/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-30 08:56:44.494460 qwak_core-0.0.88/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.698627 qwak_core-0.0.88/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-30 08:56:51.702627 qwak_core-0.0.88/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-30 08:56:44.666464 qwak_core-0.0.88/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-30 08:56:51.702627 qwak_core-0.0.88/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-30 08:56:51.674626 qwak_core-0.0.88/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-30 08:56:42.482414 qwak_core-0.0.88/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.678626 qwak_core-0.0.88/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-30 08:56:51.678626 qwak_core-0.0.88/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-30 08:56:42.658418 qwak_core-0.0.88/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-30 08:56:51.678626 qwak_core-0.0.88/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-30 08:56:51.670626 qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-30 08:56:42.114406 qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.670626 qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-30 08:56:51.670626 qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-30 08:56:41.934402 qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.670626 qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-30 08:56:51.674626 qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-30 08:56:42.302410 qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-30 08:56:51.674626 qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-30 08:56:51.578624 qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-30 08:56:34.158222 qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.578624 qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-30 08:56:51.582624 qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-30 08:56:34.334226 qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.582624 qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-30 08:56:51.582624 qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-30 08:56:34.514230 qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-30 08:56:51.582624 qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-30 08:56:51.638625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-30 08:56:39.258340 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.638625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-30 08:56:51.634625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-30 08:56:39.086336 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-30 08:56:51.638625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2023-05-30 08:56:51.618625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2023-05-30 08:56:37.474299 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.618625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2023-05-30 08:56:51.614625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2023-05-30 08:56:37.298295 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.614625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-30 08:56:51.610625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-30 08:56:36.742282 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.610625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-30 08:56:51.614625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-30 08:56:37.118291 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-30 08:56:51.614625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-30 08:56:51.618625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-30 08:56:37.654303 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.622625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-30 08:56:51.622625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-30 08:56:37.834307 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-30 08:56:51.622625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25269 2023-05-30 08:56:51.610625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37664 2023-05-30 08:56:36.930286 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.610625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-30 08:56:51.622625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-30 08:56:38.010311 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.626625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    11277 2023-05-30 08:56:51.626625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    15070 2023-05-30 08:56:38.190315 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.626625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-30 08:56:51.638625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-30 08:56:51.094613 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.642625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-30 08:56:51.642625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-30 08:56:51.274617 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-30 08:56:51.642625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-30 08:56:51.642625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-30 08:56:39.794352 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.646625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-30 08:56:51.646625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-30 08:56:39.974356 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-30 08:56:51.646625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-30 08:56:51.650626 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-30 08:56:40.150360 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.650626 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-30 08:56:51.654626 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-30 08:56:40.862377 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.654626 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-30 08:56:51.650626 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-30 08:56:40.682373 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-30 08:56:51.650626 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-30 08:56:51.654626 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-30 08:56:41.038381 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.654626 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-30 08:56:51.626625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-30 08:56:38.370319 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.630625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-30 08:56:51.630625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-30 08:56:38.550323 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.630625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-30 08:56:51.630625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-30 08:56:38.730328 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-30 08:56:51.634625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-30 08:56:51.634625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-30 08:56:38.910332 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.634625 qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-30 08:56:51.762628 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-30 08:56:50.022588 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.762628 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-30 08:56:51.766628 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-30 08:56:50.198592 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-30 08:56:51.766628 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-30 08:56:51.766628 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-30 08:56:50.370596 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.770628 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-30 08:56:51.770628 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-30 08:56:50.554600 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-30 08:56:51.770628 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-30 08:56:51.770628 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-30 08:56:50.742605 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-30 08:56:51.774628 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-30 08:56:51.774628 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-30 08:56:50.918609 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.774628 qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-30 08:56:51.702627 qwak_core-0.0.88/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-30 08:56:44.842469 qwak_core-0.0.88/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.702627 qwak_core-0.0.88/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-30 08:56:51.706627 qwak_core-0.0.88/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-30 08:56:45.018473 qwak_core-0.0.88/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-30 08:56:51.706627 qwak_core-0.0.88/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-30 08:56:51.594624 qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-30 08:56:36.034265 qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.598624 qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-30 08:56:51.598624 qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-30 08:56:36.210270 qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.602625 qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-30 08:56:51.602625 qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-30 08:56:36.386273 qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-30 08:56:51.606624 qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-30 08:56:51.606624 qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-30 08:56:36.558277 qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.606624 qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-30 08:56:51.678626 qwak_core-0.0.88/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-30 08:56:42.834422 qwak_core-0.0.88/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-30 08:56:51.682626 qwak_core-0.0.88/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-05-30 08:56:51.706627 qwak_core-0.0.88/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-05-30 08:56:45.194477 qwak_core-0.0.88/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.706627 qwak_core-0.0.88/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-05-30 08:56:51.710627 qwak_core-0.0.88/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-05-30 08:56:45.370481 qwak_core-0.0.88/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-05-30 08:56:51.710627 qwak_core-0.0.88/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-30 08:56:51.722627 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-30 08:56:46.422505 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.722627 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-30 08:56:51.722627 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-30 08:56:46.598509 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.726627 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-30 08:56:51.726627 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-30 08:56:46.774513 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.726627 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-30 08:56:51.726627 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-30 08:56:46.954517 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.730627 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-30 08:56:51.730627 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-30 08:56:47.138522 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.730627 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-30 08:56:51.730627 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-30 08:56:47.330526 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-30 08:56:51.734628 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-30 08:56:51.734628 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-30 08:56:47.506530 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.734628 qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-30 08:56:51.714627 qwak_core-0.0.88/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-30 08:56:45.722489 qwak_core-0.0.88/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.714627 qwak_core-0.0.88/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-30 08:56:51.718627 qwak_core-0.0.88/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-30 08:56:46.250501 qwak_core-0.0.88/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.718627 qwak_core-0.0.88/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-30 08:56:51.714627 qwak_core-0.0.88/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-30 08:56:45.898493 qwak_core-0.0.88/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-30 08:56:51.714627 qwak_core-0.0.88/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-05-30 08:56:51.718627 qwak_core-0.0.88/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-05-30 08:56:46.074497 qwak_core-0.0.88/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.718627 qwak_core-0.0.88/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-30 08:56:51.698627 qwak_core-0.0.88/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-30 08:56:44.314456 qwak_core-0.0.88/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-30 08:56:51.698627 qwak_core-0.0.88/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-30 08:56:51.574624 qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-30 08:56:35.634256 qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-30 08:56:51.574624 qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-30 08:56:51.570624 qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-30 08:56:35.426251 qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.574624 qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-30 08:56:51.578624 qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-30 08:56:35.842261 qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-30 08:56:51.578624 qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-30 08:56:51.694627 qwak_core-0.0.88/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-30 08:56:43.926447 qwak_core-0.0.88/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-30 08:56:51.694627 qwak_core-0.0.88/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-30 08:56:51.710627 qwak_core-0.0.88/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-30 08:56:45.546485 qwak_core-0.0.88/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-30 08:56:51.710627 qwak_core-0.0.88/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-30 08:56:51.570624 qwak_core-0.0.88/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-30 08:56:33.442206 qwak_core-0.0.88/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.570624 qwak_core-0.0.88/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-30 08:56:51.566624 qwak_core-0.0.88/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-30 08:56:33.266202 qwak_core-0.0.88/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-30 08:56:51.570624 qwak_core-0.0.88/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-30 08:56:51.562624 qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-30 08:56:32.726189 qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.562624 qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-30 08:56:51.562624 qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-30 08:56:32.902193 qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.566624 qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-30 08:56:51.566624 qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-30 08:56:33.078197 qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-30 08:56:51.566624 qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-30 08:56:51.738628 qwak_core-0.0.88/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-30 08:56:47.854538 qwak_core-0.0.88/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-30 08:56:51.738628 qwak_core-0.0.88/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-30 08:56:51.734628 qwak_core-0.0.88/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-30 08:56:47.682534 qwak_core-0.0.88/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.738628 qwak_core-0.0.88/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    10851 2023-05-30 08:56:51.586624 qwak_core-0.0.88/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    13974 2023-05-30 08:56:34.690235 qwak_core-0.0.88/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.586624 qwak_core-0.0.88/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3044 2023-05-30 08:56:51.586624 qwak_core-0.0.88/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2641 2023-05-30 08:56:34.866238 qwak_core-0.0.88/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-30 08:56:51.586624 qwak_core-0.0.88/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-30 08:56:52.966656 qwak_core-0.0.88/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-30 08:56:52.966656 qwak_core-0.0.88/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.428245 qwak_core-0.0.88/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14847 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-30 08:55:08.432245 qwak_core-0.0.88/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-30 08:55:08.436245 qwak_core-0.0.88/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.88/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.88/PKG-INFO
```

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7qwak/administration/authenticated_user/v1/details.proto\x12)qwak.administration.authenticated_user.v1\"/\n\x0bUserDetails\x12\n\n\x02id\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\"|\n\x12\x45nvironmentDetails\x12\n\n\x02id\x18\x01 \x01(\t\x12Z\n\rconfiguration\x18\x02 \x01(\x0b\x32\x43.qwak.administration.authenticated_user.v1.EnvironmentConfiguration\"\xa5\x02\n\x18\x45nvironmentConfiguration\x12\x19\n\x11\x65\x64ge_services_url\x18\x01 \x01(\t\x12\x1d\n\x15management_access_url\x18\x06 \x01(\t\x12\x15\n\rmodel_api_url\x18\x02 \x01(\t\x12\x1e\n\x16\x61nalytics_data_api_url\x18\x03 \x01(\t\x12\x1d\n\x15object_storage_bucket\x18\x04 \x01(\t\x12\x19\n\x11\x62i_system_api_key\x18\x05 \x01(\t\x12^\n\x13\x63loud_configuration\x18\x07 \x01(\x0b\x32\x41.qwak.administration.authenticated_user.v1.QwakCloudConfiguration\"\x8e\x01\n\x16QwakCloudConfiguration\x12\x63\n\x17\x61ws_cloud_configuration\x18\x01 \x01(\x0b\x32@.qwak.administration.authenticated_user.v1.AwsCloudConfigurationH\x00\x42\x0f\n\rconfiguration\"N\n\x15\x41wsCloudConfiguration\x12\x0e\n\x06region\x18\x01 \x01(\t\x12\x10\n\x08role_arn\x18\x02 \x01(\t\x12\x13\n\x0b\x65xternal_id\x18\x03 \x01(\tBN\n4com.qwak.ai.administration.api.authenticated_user.v1P\x01Z\x14.;authenticated_userb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7qwak/administration/authenticated_user/v1/details.proto\x12)qwak.administration.authenticated_user.v1\"/\n\x0bUserDetails\x12\n\n\x02id\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\"|\n\x12\x45nvironmentDetails\x12\n\n\x02id\x18\x01 \x01(\t\x12Z\n\rconfiguration\x18\x02 \x01(\x0b\x32\x43.qwak.administration.authenticated_user.v1.EnvironmentConfiguration\"\xa5\x02\n\x18\x45nvironmentConfiguration\x12\x19\n\x11\x65\x64ge_services_url\x18\x01 \x01(\t\x12\x1d\n\x15management_access_url\x18\x06 \x01(\t\x12\x15\n\rmodel_api_url\x18\x02 \x01(\t\x12\x1e\n\x16\x61nalytics_data_api_url\x18\x03 \x01(\t\x12\x1d\n\x15object_storage_bucket\x18\x04 \x01(\t\x12\x19\n\x11\x62i_system_api_key\x18\x05 \x01(\t\x12^\n\x13\x63loud_configuration\x18\x07 \x01(\x0b\x32\x41.qwak.administration.authenticated_user.v1.QwakCloudConfiguration\"\x8e\x01\n\x16QwakCloudConfiguration\x12\x63\n\x17\x61ws_cloud_configuration\x18\x01 \x01(\x0b\x32@.qwak.administration.authenticated_user.v1.AwsCloudConfigurationH\x00\x42\x0f\n\rconfiguration\"a\n\x15\x41wsCloudConfiguration\x12\x0e\n\x06region\x18\x01 \x01(\t\x12\x10\n\x08role_arn\x18\x02 \x01(\t\x12\x13\n\x0b\x65xternal_id\x18\x03 \x01(\t\x12\x11\n\tworkgroup\x18\x04 \x01(\tBN\n4com.qwak.ai.administration.api.authenticated_user.v1P\x01Z\x14.;authenticated_userb\x06proto3')
 
 
 
 _USERDETAILS = DESCRIPTOR.message_types_by_name['UserDetails']
 _ENVIRONMENTDETAILS = DESCRIPTOR.message_types_by_name['EnvironmentDetails']
 _ENVIRONMENTCONFIGURATION = DESCRIPTOR.message_types_by_name['EnvironmentConfiguration']
 _QWAKCLOUDCONFIGURATION = DESCRIPTOR.message_types_by_name['QwakCloudConfiguration']
@@ -67,9 +67,9 @@
   _ENVIRONMENTDETAILS._serialized_start=151
   _ENVIRONMENTDETAILS._serialized_end=275
   _ENVIRONMENTCONFIGURATION._serialized_start=278
   _ENVIRONMENTCONFIGURATION._serialized_end=571
   _QWAKCLOUDCONFIGURATION._serialized_start=574
   _QWAKCLOUDCONFIGURATION._serialized_end=716
   _AWSCLOUDCONFIGURATION._serialized_start=718
-  _AWSCLOUDCONFIGURATION._serialized_end=796
+  _AWSCLOUDCONFIGURATION._serialized_end=815
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -114,23 +114,27 @@
 
 class AwsCloudConfiguration(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     REGION_FIELD_NUMBER: builtins.int
     ROLE_ARN_FIELD_NUMBER: builtins.int
     EXTERNAL_ID_FIELD_NUMBER: builtins.int
+    WORKGROUP_FIELD_NUMBER: builtins.int
     region: builtins.str
     """The region of the environment"""
     role_arn: builtins.str
     """The role ARN which qwak platform perform actions on behalf"""
     external_id: builtins.str
     """The external id that is needed to assume the role_arn"""
+    workgroup: builtins.str
+    """The workgroup that is needed to perform actions on Athena"""
     def __init__(
         self,
         *,
         region: builtins.str = ...,
         role_arn: builtins.str = ...,
         external_id: builtins.str = ...,
+        workgroup: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["external_id", b"external_id", "region", b"region", "role_arn", b"role_arn"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["external_id", b"external_id", "region", b"region", "role_arn", b"role_arn", "workgroup", b"workgroup"]) -> None: ...
 
 global___AwsCloudConfiguration = AwsCloudConfiguration
```

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.88/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.88/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.88/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/pyproject.toml` & `qwak_core-0.0.88/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.87"
+version = "0.0.88"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.87/qwak/automations/__init__.py` & `qwak_core-0.0.88/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/automations/automation_executions.py` & `qwak_core-0.0.88/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/automations/automations.py` & `qwak_core-0.0.88/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.88/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.88/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/automations/common.py` & `qwak_core-0.0.88/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.88/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.88/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.88/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.88/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.88/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/alert_management/client.py` & `qwak_core-0.0.88/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/analytics/client.py` & `qwak_core-0.0.88/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/audience/client.py` & `qwak_core-0.0.88/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/automation_management/client.py` & `qwak_core-0.0.88/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.88/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.88/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.88/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.88/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/build_management/client.py` & `qwak_core-0.0.88/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.88/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.88/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/deployment/client.py` & `qwak_core-0.0.88/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.88/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.88/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.88/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.88/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/instance_template/client.py` & `qwak_core-0.0.88/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.88/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/logging_client/client.py` & `qwak_core-0.0.88/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/model_management/client.py` & `qwak_core-0.0.88/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/project/client.py` & `qwak_core-0.0.88/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/secret_service/client.py` & `qwak_core-0.0.88/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.88/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.88/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.88/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.88/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.88/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.88/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.88/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.88/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.88/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.88/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.88/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.88/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.88/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.88/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.88/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/offline/client.py` & `qwak_core-0.0.88/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/feature_store/online/client.py` & `qwak_core-0.0.88/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/inner/const.py` & `qwak_core-0.0.88/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.88/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.88/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.88/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.88/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/inner/singleton_meta.py` & `qwak_core-0.0.88/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/inner/tool/auth.py` & `qwak_core-0.0.88/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.88/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.88/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.88/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.88/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/adapters/__init__.py` & `qwak_core-0.0.88/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.88/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.88/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.88/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.88/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.88/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/base.py` & `qwak_core-0.0.88/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/decorators/api.py` & `qwak_core-0.0.88/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.88/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/experiment_tracking.py` & `qwak_core-0.0.88/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/schema.py` & `qwak_core-0.0.88/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/schema_entities.py` & `qwak_core-0.0.88/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.88/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.88/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.88/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.88/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.88/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.88/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.88/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.88/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.88/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.88/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.88/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.88/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.88/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.88/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.88/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.88/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.88/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.88/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.88/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/qwak_client/client.py` & `qwak_core-0.0.88/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.88/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/qwak_client/models/model.py` & `qwak_core-0.0.88/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.88/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.88/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/tools/logger/logger.py` & `qwak_core-0.0.88/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak/tools/logger/logging.yml` & `qwak_core-0.0.88/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.88/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/qwak_services_mock/services_mock.py` & `qwak_core-0.0.88/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.87/setup.py` & `qwak_core-0.0.88/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.87',
+    'version': '0.0.88',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.87/PKG-INFO` & `qwak_core-0.0.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.87
+Version: 0.0.88
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

