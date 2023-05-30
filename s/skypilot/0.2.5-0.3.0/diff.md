# Comparing `tmp/skypilot-0.2.5.tar.gz` & `tmp/skypilot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-0.2.5.tar", last modified: Mon Mar 20 17:47:00 2023, max compression
+gzip compressed data, was "/Users/zongheng/Dropbox/workspace/riselab/sky-computing/dist/.tmp-oi70v4yj/skypilot-0.3.0.tar", last modified: Tue May 30 00:13:43 2023, max compression
```

## Comparing `skypilot-0.2.5.tar` & `skypilot-0.3.0.tar`

### file list

```diff
@@ -1,181 +1,192 @@
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.556915 skypilot-0.2.5/
--rwxr-xr-x   0 romilb     (501) staff       (20)    12170 2022-12-30 18:13:08.000000 skypilot-0.2.5/LICENSE
--rw-r--r--   0 romilb     (501) staff       (20)      438 2023-03-16 05:48:32.000000 skypilot-0.2.5/MANIFEST.in
--rw-r--r--   0 romilb     (501) staff       (20)     7474 2023-03-20 17:47:00.556797 skypilot-0.2.5/PKG-INFO
--rw-r--r--   0 romilb     (501) staff       (20)     6555 2023-03-16 01:04:50.000000 skypilot-0.2.5/README.md
--rw-r--r--   0 romilb     (501) staff       (20)      548 2023-03-19 02:09:05.000000 skypilot-0.2.5/pyproject.toml
--rw-r--r--   0 romilb     (501) staff       (20)       38 2023-03-20 17:47:00.556946 skypilot-0.2.5/setup.cfg
--rw-r--r--   0 romilb     (501) staff       (20)     6552 2023-03-17 02:16:19.000000 skypilot-0.2.5/setup.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.530701 skypilot-0.2.5/sky/
--rw-r--r--   0 romilb     (501) staff       (20)     2016 2023-03-20 17:45:21.000000 skypilot-0.2.5/sky/__init__.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.531808 skypilot-0.2.5/sky/adaptors/
--rw-------   0 romilb     (501) staff       (20)        0 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/adaptors/__init__.py
--rw-r--r--   0 romilb     (501) staff       (20)     2607 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/adaptors/aws.py
--rwxr-xr-x   0 romilb     (501) staff       (20)      989 2023-02-04 00:48:18.000000 skypilot-0.2.5/sky/adaptors/azure.py
--rwxr-xr-x   0 romilb     (501) staff       (20)      852 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/adaptors/docker.py
--rwxr-xr-x   0 romilb     (501) staff       (20)     2190 2023-02-04 00:48:18.000000 skypilot-0.2.5/sky/adaptors/gcp.py
--rw-r--r--   0 romilb     (501) staff       (20)    13595 2023-03-16 21:56:42.000000 skypilot-0.2.5/sky/authentication.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.534037 skypilot-0.2.5/sky/backends/
--rw-r--r--   0 romilb     (501) staff       (20)      414 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/backends/__init__.py
--rw-r--r--   0 romilb     (501) staff       (20)     5542 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/backends/backend.py
--rw-r--r--   0 romilb     (501) staff       (20)   105610 2023-03-20 14:27:45.000000 skypilot-0.2.5/sky/backends/backend_utils.py
--rw-r--r--   0 romilb     (501) staff       (20)   174467 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 romilb     (501) staff       (20)     8148 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/backends/docker_utils.py
--rw-r--r--   0 romilb     (501) staff       (20)    16091 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.534290 skypilot-0.2.5/sky/backends/monkey_patches/
--rw-r--r--   0 romilb     (501) staff       (20)     3436 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 romilb     (501) staff       (20)    23998 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/backends/onprem_utils.py
--rwxr-xr-x   0 romilb     (501) staff       (20)     5903 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/backends/wheel_utils.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.534715 skypilot-0.2.5/sky/benchmark/
--rw-------   0 romilb     (501) staff       (20)        0 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/benchmark/__init__.py
--rw-r--r--   0 romilb     (501) staff       (20)     8723 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/benchmark/benchmark_state.py
--rw-r--r--   0 romilb     (501) staff       (20)    24632 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/benchmark/benchmark_utils.py
--rwxr-xr-x   0 romilb     (501) staff       (20)     2358 2023-02-04 00:48:18.000000 skypilot-0.2.5/sky/check.py
--rw-r--r--   0 romilb     (501) staff       (20)   154836 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/cli.py
--rw-r--r--   0 romilb     (501) staff       (20)     5960 2023-03-17 02:16:19.000000 skypilot-0.2.5/sky/cloud_stores.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.536112 skypilot-0.2.5/sky/clouds/
--rw-r--r--   0 romilb     (501) staff       (20)      575 2023-03-16 05:48:32.000000 skypilot-0.2.5/sky/clouds/__init__.py
--rw-r--r--   0 romilb     (501) staff       (20)    24381 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/clouds/aws.py
--rw-r--r--   0 romilb     (501) staff       (20)    17073 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/clouds/azure.py
--rw-r--r--   0 romilb     (501) staff       (20)    17424 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/clouds/cloud.py
--rw-r--r--   0 romilb     (501) staff       (20)    30574 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/clouds/gcp.py
--rw-r--r--   0 romilb     (501) staff       (20)    10123 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/clouds/lambda_cloud.py
--rw-r--r--   0 romilb     (501) staff       (20)     7653 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/clouds/local.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.537654 skypilot-0.2.5/sky/clouds/service_catalog/
--rw-r--r--   0 romilb     (501) staff       (20)    12820 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 romilb     (501) staff       (20)    10586 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 romilb     (501) staff       (20)     6329 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 romilb     (501) staff       (20)    22007 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/clouds/service_catalog/common.py
--rw-r--r--   0 romilb     (501) staff       (20)     1500 2023-03-16 21:56:42.000000 skypilot-0.2.5/sky/clouds/service_catalog/config.py
--rwxr-xr-x   0 romilb     (501) staff       (20)      282 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/clouds/service_catalog/constants.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.538635 skypilot-0.2.5/sky/clouds/service_catalog/data_fetchers/
--rw-------   0 romilb     (501) staff       (20)        0 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 romilb     (501) staff       (20)    17099 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 romilb     (501) staff       (20)     8233 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 romilb     (501) staff       (20)    21996 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 romilb     (501) staff       (20)     4155 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 romilb     (501) staff       (20)    18729 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 romilb     (501) staff       (20)     5225 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 romilb     (501) staff       (20)    38515 2023-03-16 21:56:42.000000 skypilot-0.2.5/sky/core.py
--rw-r--r--   0 romilb     (501) staff       (20)     2477 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/dag.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.540090 skypilot-0.2.5/sky/data/
--rwxr-xr-x   0 romilb     (501) staff       (20)      128 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/data/__init__.py
--rw-r--r--   0 romilb     (501) staff       (20)     4856 2023-03-17 02:16:19.000000 skypilot-0.2.5/sky/data/data_transfer.py
--rw-r--r--   0 romilb     (501) staff       (20)     7038 2023-03-17 02:16:19.000000 skypilot-0.2.5/sky/data/data_utils.py
--rwxr-xr-x   0 romilb     (501) staff       (20)     2958 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/data/mounting_utils.py
--rw-r--r--   0 romilb     (501) staff       (20)    58975 2023-03-17 02:16:19.000000 skypilot-0.2.5/sky/data/storage.py
--rwxr-xr-x   0 romilb     (501) staff       (20)     1082 2023-02-04 00:48:18.000000 skypilot-0.2.5/sky/data/storage_utils.py
--rw-r--r--   0 romilb     (501) staff       (20)     5672 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/exceptions.py
--rw-r--r--   0 romilb     (501) staff       (20)    35628 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/execution.py
--rw-r--r--   0 romilb     (501) staff       (20)    24559 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/global_user_state.py
--rw-r--r--   0 romilb     (501) staff       (20)    43009 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/optimizer.py
--rw-r--r--   0 romilb     (501) staff       (20)    39182 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/resources.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.540442 skypilot-0.2.5/sky/setup_files/
--rw-r--r--   0 romilb     (501) staff       (20)      438 2023-03-16 05:48:32.000000 skypilot-0.2.5/sky/setup_files/MANIFEST.in
--rw-r--r--   0 romilb     (501) staff       (20)     6552 2023-03-17 02:16:19.000000 skypilot-0.2.5/sky/setup_files/setup.py
--rw-r--r--   0 romilb     (501) staff       (20)     3216 2023-03-16 21:56:42.000000 skypilot-0.2.5/sky/sky_logging.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.542374 skypilot-0.2.5/sky/skylet/
--rwxr-xr-x   0 romilb     (501) staff       (20)    12568 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/LICENCE
--rw-------   0 romilb     (501) staff       (20)        0 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/__init__.py
--rw-r--r--   0 romilb     (501) staff       (20)     4378 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/skylet/autostop_lib.py
--rw-r--r--   0 romilb     (501) staff       (20)     2118 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/skylet/configs.py
--rwxr-xr-x   0 romilb     (501) staff       (20)      408 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/constants.py
--rw-r--r--   0 romilb     (501) staff       (20)     7619 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/skylet/events.py
--rw-r--r--   0 romilb     (501) staff       (20)    27462 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/skylet/job_lib.py
--rw-r--r--   0 romilb     (501) staff       (20)    17792 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/skylet/log_lib.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.525204 skypilot-0.2.5/sky/skylet/providers/
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.543756 skypilot-0.2.5/sky/skylet/providers/aws/
--rwxr-xr-x   0 romilb     (501) staff       (20)      110 2023-02-04 00:48:18.000000 skypilot-0.2.5/sky/skylet/providers/aws/__init__.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.544037 skypilot-0.2.5/sky/skylet/providers/aws/cloudwatch/
--rw-------   0 romilb     (501) staff       (20)        0 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/providers/aws/cloudwatch/__init__.py
--rwxr-xr-x   0 romilb     (501) staff       (20)    31879 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
--rw-r--r--   0 romilb     (501) staff       (20)    51687 2023-02-21 01:40:26.000000 skypilot-0.2.5/sky/skylet/providers/aws/config.py
--rw-r--r--   0 romilb     (501) staff       (20)    28940 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/skylet/providers/aws/node_provider.py
--rwxr-xr-x   0 romilb     (501) staff       (20)     5917 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/providers/aws/utils.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.545000 skypilot-0.2.5/sky/skylet/providers/azure/
--rwxr-xr-x   0 romilb     (501) staff       (20)       97 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/providers/azure/__init__.py
--rwxr-xr-x   0 romilb     (501) staff       (20)     3270 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/providers/azure/azure-config-template.json
--rwxr-xr-x   0 romilb     (501) staff       (20)    10157 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/providers/azure/azure-vm-template.json
--rwxr-xr-x   0 romilb     (501) staff       (20)     4371 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/providers/azure/config.py
--rw-r--r--   0 romilb     (501) staff       (20)    16632 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/skylet/providers/azure/node_provider.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.545729 skypilot-0.2.5/sky/skylet/providers/gcp/
--rwxr-xr-x   0 romilb     (501) staff       (20)       91 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/providers/gcp/__init__.py
--rw-r--r--   0 romilb     (501) staff       (20)    31015 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/skylet/providers/gcp/config.py
--rw-r--r--   0 romilb     (501) staff       (20)     2738 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/skylet/providers/gcp/constants.py
--rw-r--r--   0 romilb     (501) staff       (20)    26192 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/skylet/providers/gcp/node.py
--rw-r--r--   0 romilb     (501) staff       (20)    14276 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/skylet/providers/gcp/node_provider.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.546222 skypilot-0.2.5/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 romilb     (501) staff       (20)      112 2023-02-21 01:40:26.000000 skypilot-0.2.5/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 romilb     (501) staff       (20)     7306 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/skylet/providers/lambda_cloud/lambda_utils.py
--rw-r--r--   0 romilb     (501) staff       (20)    10315 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.547814 skypilot-0.2.5/sky/skylet/ray_patches/
--rwxr-xr-x   0 romilb     (501) staff       (20)     3467 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/ray_patches/__init__.py
--rwxr-xr-x   0 romilb     (501) staff       (20)      294 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/ray_patches/autoscaler.py.patch
--rwxr-xr-x   0 romilb     (501) staff       (20)       86 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/ray_patches/azure_cli.py.patch
--rwxr-xr-x   0 romilb     (501) staff       (20)      391 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/ray_patches/cli.py.patch
--rwxr-xr-x   0 romilb     (501) staff       (20)      107 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/ray_patches/command_runner.py.patch
--rwxr-xr-x   0 romilb     (501) staff       (20)     1020 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/ray_patches/job_manager.py.patch
--rwxr-xr-x   0 romilb     (501) staff       (20)      512 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/ray_patches/log_monitor.py.patch
--rwxr-xr-x   0 romilb     (501) staff       (20)      658 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rwxr-xr-x   0 romilb     (501) staff       (20)      289 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/ray_patches/updater.py.patch
--rwxr-xr-x   0 romilb     (501) staff       (20)      549 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/ray_patches/worker.py.patch
--rwxr-xr-x   0 romilb     (501) staff       (20)      603 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/skylet.py
--rwxr-xr-x   0 romilb     (501) staff       (20)     2561 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 romilb     (501) staff       (20)     5386 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/skypilot_config.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.548861 skypilot-0.2.5/sky/spot/
--rwxr-xr-x   0 romilb     (501) staff       (20)     1346 2023-02-04 00:48:18.000000 skypilot-0.2.5/sky/spot/__init__.py
--rwxr-xr-x   0 romilb     (501) staff       (20)      561 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/spot/constants.py
--rw-r--r--   0 romilb     (501) staff       (20)    17550 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/spot/controller.py
--rw-r--r--   0 romilb     (501) staff       (20)    19459 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/spot/recovery_strategy.py
--rw-r--r--   0 romilb     (501) staff       (20)    13506 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/spot/spot_state.py
--rw-r--r--   0 romilb     (501) staff       (20)    25198 2023-03-16 21:56:42.000000 skypilot-0.2.5/sky/spot/spot_utils.py
--rw-r--r--   0 romilb     (501) staff       (20)    34536 2023-03-17 02:16:19.000000 skypilot-0.2.5/sky/task.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.550767 skypilot-0.2.5/sky/templates/
--rw-r--r--   0 romilb     (501) staff       (20)     9546 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 romilb     (501) staff       (20)     9134 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 romilb     (501) staff       (20)    10557 2023-03-16 21:56:42.000000 skypilot-0.2.5/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 romilb     (501) staff       (20)      505 2023-02-21 01:40:26.000000 skypilot-0.2.5/sky/templates/gcp-tpu-create.sh.j2
--rwxr-xr-x   0 romilb     (501) staff       (20)      328 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/templates/gcp-tpu-delete.sh.j2
--rw-r--r--   0 romilb     (501) staff       (20)     6633 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/templates/lambda-ray.yml.j2
--rwxr-xr-x   0 romilb     (501) staff       (20)     1424 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/templates/local-ray.yml.j2
--rw-r--r--   0 romilb     (501) staff       (20)     2233 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/templates/spot-controller.yaml.j2
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.551254 skypilot-0.2.5/sky/usage/
--rw-------   0 romilb     (501) staff       (20)        0 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/usage/__init__.py
--rw-r--r--   0 romilb     (501) staff       (20)      633 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/usage/constants.py
--rw-r--r--   0 romilb     (501) staff       (20)    16946 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/usage/usage_lib.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.553668 skypilot-0.2.5/sky/utils/
--rwxr-xr-x   0 romilb     (501) staff       (20)       25 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/utils/__init__.py
--rw-r--r--   0 romilb     (501) staff       (20)     2806 2023-02-21 01:40:26.000000 skypilot-0.2.5/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.553868 skypilot-0.2.5/sky/utils/cli_utils/
--rw-------   0 romilb     (501) staff       (20)        0 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 romilb     (501) staff       (20)    12789 2023-03-16 21:56:42.000000 skypilot-0.2.5/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 romilb     (501) staff       (20)    14180 2023-03-16 05:48:32.000000 skypilot-0.2.5/sky/utils/command_runner.py
--rw-r--r--   0 romilb     (501) staff       (20)    11033 2023-03-16 21:56:42.000000 skypilot-0.2.5/sky/utils/common_utils.py
--rw-r--r--   0 romilb     (501) staff       (20)     1853 2023-03-16 01:04:50.000000 skypilot-0.2.5/sky/utils/db_utils.py
--rwxr-xr-x   0 romilb     (501) staff       (20)      852 2023-02-04 00:48:18.000000 skypilot-0.2.5/sky/utils/env_options.py
--rw-r--r--   0 romilb     (501) staff       (20)     4705 2023-03-16 21:56:42.000000 skypilot-0.2.5/sky/utils/log_utils.py
--rw-r--r--   0 romilb     (501) staff       (20)     6535 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/utils/schemas.py
--rw-r--r--   0 romilb     (501) staff       (20)     4078 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/utils/subprocess_utils.py
--rwxr-xr-x   0 romilb     (501) staff       (20)     3965 2023-02-04 00:48:18.000000 skypilot-0.2.5/sky/utils/timeline.py
--rw-r--r--   0 romilb     (501) staff       (20)     4186 2023-03-19 02:09:05.000000 skypilot-0.2.5/sky/utils/tpu_utils.py
--rw-r--r--   0 romilb     (501) staff       (20)      812 2023-03-16 21:56:42.000000 skypilot-0.2.5/sky/utils/ux_utils.py
--rwxr-xr-x   0 romilb     (501) staff       (20)      701 2022-12-30 18:13:10.000000 skypilot-0.2.5/sky/utils/validator.py
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.554487 skypilot-0.2.5/skypilot.egg-info/
--rwxr-xr-x   0 romilb     (501) staff       (20)     7474 2023-03-20 17:47:00.000000 skypilot-0.2.5/skypilot.egg-info/PKG-INFO
--rwxr-xr-x   0 romilb     (501) staff       (20)     4556 2023-03-20 17:47:00.000000 skypilot-0.2.5/skypilot.egg-info/SOURCES.txt
--rwxr-xr-x   0 romilb     (501) staff       (20)        1 2023-03-20 17:47:00.000000 skypilot-0.2.5/skypilot.egg-info/dependency_links.txt
--rwxr-xr-x   0 romilb     (501) staff       (20)       36 2023-03-20 17:47:00.000000 skypilot-0.2.5/skypilot.egg-info/entry_points.txt
--rwxr-xr-x   0 romilb     (501) staff       (20)      609 2023-03-20 17:47:00.000000 skypilot-0.2.5/skypilot.egg-info/requires.txt
--rwxr-xr-x   0 romilb     (501) staff       (20)        4 2023-03-20 17:47:00.000000 skypilot-0.2.5/skypilot.egg-info/top_level.txt
-drwxr-xr-x   0 romilb     (501) staff       (20)        0 2023-03-20 17:47:00.556632 skypilot-0.2.5/tests/
--rw-r--r--   0 romilb     (501) staff       (20)     2597 2023-03-16 01:04:50.000000 skypilot-0.2.5/tests/test_cli.py
--rwxr-xr-x   0 romilb     (501) staff       (20)      260 2022-12-30 18:13:10.000000 skypilot-0.2.5/tests/test_global_user_state.py
--rw-r--r--   0 romilb     (501) staff       (20)     1076 2023-02-21 01:40:26.000000 skypilot-0.2.5/tests/test_list_accelerators.py
--rwxr-xr-x   0 romilb     (501) staff       (20)    14008 2022-12-30 18:13:10.000000 skypilot-0.2.5/tests/test_onprem.py
--rw-r--r--   0 romilb     (501) staff       (20)    19435 2023-03-19 02:09:05.000000 skypilot-0.2.5/tests/test_optimizer_dryruns.py
--rw-r--r--   0 romilb     (501) staff       (20)     4663 2023-03-19 02:09:05.000000 skypilot-0.2.5/tests/test_optimizer_random_dag.py
--rwxr-xr-x   0 romilb     (501) staff       (20)       94 2022-12-30 18:13:10.000000 skypilot-0.2.5/tests/test_pycryptodome_version.py
--rw-r--r--   0 romilb     (501) staff       (20)    83622 2023-03-19 02:09:05.000000 skypilot-0.2.5/tests/test_smoke.py
--rw-r--r--   0 romilb     (501) staff       (20)     7206 2023-03-16 01:04:50.000000 skypilot-0.2.5/tests/test_spot.py
--rwxr-xr-x   0 romilb     (501) staff       (20)     3526 2022-12-30 18:13:10.000000 skypilot-0.2.5/tests/test_storage.py
--rwxr-xr-x   0 romilb     (501) staff       (20)     1070 2022-12-30 18:13:10.000000 skypilot-0.2.5/tests/test_wheels.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/
+-rw-r--r--   0 zongheng   (502) staff       (20)    12170 2022-04-03 15:38:40.000000 skypilot-0.3.0/LICENSE
+-rw-r--r--   0 zongheng   (502) staff       (20)      473 2023-05-28 16:45:59.000000 skypilot-0.3.0/MANIFEST.in
+-rw-r--r--   0 zongheng   (502) staff       (20)     8079 2023-05-30 00:13:43.000000 skypilot-0.3.0/PKG-INFO
+-rw-r--r--   0 zongheng   (502) staff       (20)     7163 2023-05-28 16:45:59.000000 skypilot-0.3.0/README.md
+-rw-r--r--   0 zongheng   (502) staff       (20)      519 2023-05-28 16:43:06.000000 skypilot-0.3.0/pyproject.toml
+-rw-r--r--   0 zongheng   (502) staff       (20)       38 2023-05-30 00:13:43.000000 skypilot-0.3.0/setup.cfg
+-rw-r--r--   0 zongheng   (502) staff       (20)     7159 2023-05-28 17:22:30.000000 skypilot-0.3.0/setup.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/
+-rw-r--r--   0 zongheng   (502) staff       (20)     2044 2023-05-30 00:13:09.000000 skypilot-0.3.0/sky/__init__.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/adaptors/
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/adaptors/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2607 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/adaptors/aws.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      989 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/adaptors/azure.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     7725 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/adaptors/cloudflare.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      852 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/adaptors/docker.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2194 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/adaptors/gcp.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     3052 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/adaptors/ibm.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    15703 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/authentication.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/backends/
+-rw-r--r--   0 zongheng   (502) staff       (20)      414 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/backends/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     5542 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/backends/backend.py
+-rw-r--r--   0 zongheng   (502) staff       (20)   114085 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/backends/backend_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)   183288 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     8321 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/backends/docker_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    16267 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/backends/monkey_patches/
+-rw-r--r--   0 zongheng   (502) staff       (20)     3410 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    24421 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/backends/onprem_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     5903 2023-01-09 22:00:08.000000 skypilot-0.3.0/sky/backends/wheel_utils.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/benchmark/
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-11-22 22:28:46.000000 skypilot-0.3.0/sky/benchmark/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     8723 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    24632 2023-04-19 13:26:02.000000 skypilot-0.3.0/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     3505 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/check.py
+-rw-r--r--   0 zongheng   (502) staff       (20)   161212 2023-05-28 17:22:59.000000 skypilot-0.3.0/sky/cli.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     8588 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/cloud_stores.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/clouds/
+-rw-r--r--   0 zongheng   (502) staff       (20)      617 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/clouds/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    30999 2023-05-28 16:52:14.000000 skypilot-0.3.0/sky/clouds/aws.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    20568 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/azure.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    18690 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/clouds/cloud.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    31458 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/clouds/gcp.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    18104 2023-05-28 16:52:14.000000 skypilot-0.3.0/sky/clouds/ibm.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    10604 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     8062 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/clouds/local.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/clouds/service_catalog/
+-rw-r--r--   0 zongheng   (502) staff       (20)    13177 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    10773 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     6705 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    22851 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1500 2023-04-19 13:26:02.000000 skypilot-0.3.0/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      282 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/clouds/service_catalog/constants.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    20092 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     8421 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    17799 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4155 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    18924 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4656 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     5414 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2281 2022-12-10 11:50:57.000000 skypilot-0.3.0/sky/config.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    38700 2023-05-28 16:58:17.000000 skypilot-0.3.0/sky/core.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2477 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/dag.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/data/
+-rw-r--r--   0 zongheng   (502) staff       (20)      128 2023-01-09 22:00:08.000000 skypilot-0.3.0/sky/data/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     7273 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/data/data_transfer.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     7918 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/data/data_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     3251 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/data/mounting_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    88757 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/data/storage.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1082 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/data/storage_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     5893 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/exceptions.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    36869 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/execution.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    27126 2023-05-28 16:58:17.000000 skypilot-0.3.0/sky/global_user_state.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    44909 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/optimizer.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    41104 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/resources.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/setup_files/
+-rw-r--r--   0 zongheng   (502) staff       (20)      473 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 zongheng   (502) staff       (20)     7159 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/setup_files/setup.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     3216 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/sky_logging.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/
+-rw-r--r--   0 zongheng   (502) staff       (20)    12568 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/LICENSE
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/skylet/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4378 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/skylet/autostop_lib.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2118 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/skylet/configs.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      806 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/skylet/constants.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     9309 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/skylet/events.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    27771 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/skylet/job_lib.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    17792 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/skylet/log_lib.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/aws/
+-rw-r--r--   0 zongheng   (502) staff       (20)      110 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/skylet/providers/aws/__init__.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/aws/cloudwatch/
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/skylet/providers/aws/cloudwatch/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    32698 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    52192 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/aws/config.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    29406 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/aws/node_provider.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     5917 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/skylet/providers/aws/utils.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/azure/
+-rw-r--r--   0 zongheng   (502) staff       (20)       97 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4344 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 zongheng   (502) staff       (20)    10633 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 zongheng   (502) staff       (20)     5756 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    17469 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/azure/node_provider.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/gcp/
+-rw-r--r--   0 zongheng   (502) staff       (20)       91 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/skylet/providers/gcp/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    31015 2023-04-19 03:21:35.000000 skypilot-0.3.0/sky/skylet/providers/gcp/config.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2738 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/skylet/providers/gcp/constants.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    26192 2023-04-18 01:28:59.000000 skypilot-0.3.0/sky/skylet/providers/gcp/node.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    14276 2023-05-14 16:35:23.000000 skypilot-0.3.0/sky/skylet/providers/gcp/node_provider.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/ibm/
+-rw-r--r--   0 zongheng   (502) staff       (20)       94 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    38280 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1290 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    34628 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 zongheng   (502) staff       (20)      112 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     8518 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/skylet/providers/lambda_cloud/lambda_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    13650 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/ray_patches/
+-rw-r--r--   0 zongheng   (502) staff       (20)     2783 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      294 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      391 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      224 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      528 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      658 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      289 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      565 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      603 2023-01-09 22:00:08.000000 skypilot-0.3.0/sky/skylet/skylet.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2649 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     5463 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/skypilot_config.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/spot/
+-rw-r--r--   0 zongheng   (502) staff       (20)     1346 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/spot/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      561 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/spot/constants.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    18420 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/spot/controller.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    19574 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/spot/recovery_strategy.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    13506 2023-04-19 13:26:02.000000 skypilot-0.3.0/sky/spot/spot_state.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    25411 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/spot/spot_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    35504 2023-05-28 16:58:17.000000 skypilot-0.3.0/sky/task.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/templates/
+-rw-r--r--   0 zongheng   (502) staff       (20)    11434 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)     9373 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)    10844 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)      505 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/templates/gcp-tpu-create.sh.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)      328 2022-11-22 22:28:46.000000 skypilot-0.3.0/sky/templates/gcp-tpu-delete.sh.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)     8006 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)     6796 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)     1424 2022-11-22 22:28:46.000000 skypilot-0.3.0/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)     2284 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/templates/spot-controller.yaml.j2
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/usage/
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-11-22 22:28:46.000000 skypilot-0.3.0/sky/usage/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      633 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/usage/constants.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    16946 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/usage/usage_lib.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/utils/
+-rw-r--r--   0 zongheng   (502) staff       (20)       25 2022-11-22 22:28:46.000000 skypilot-0.3.0/sky/utils/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2806 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/utils/cli_utils/
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    14464 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    14688 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/utils/command_runner.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    11033 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/utils/common_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1853 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/utils/db_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      852 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/utils/env_options.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4962 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/utils/log_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     6611 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/utils/schemas.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4078 2023-04-19 13:26:02.000000 skypilot-0.3.0/sky/utils/subprocess_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     3965 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/utils/timeline.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4186 2023-04-19 13:26:02.000000 skypilot-0.3.0/sky/utils/tpu_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1125 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/utils/ux_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      701 2022-11-22 22:28:46.000000 skypilot-0.3.0/sky/utils/validator.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/
+-rw-r--r--   0 zongheng   (502) staff       (20)     8079 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/PKG-INFO
+-rw-r--r--   0 zongheng   (502) staff       (20)     4827 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/SOURCES.txt
+-rw-r--r--   0 zongheng   (502) staff       (20)        1 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/dependency_links.txt
+-rw-r--r--   0 zongheng   (502) staff       (20)       36 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/entry_points.txt
+-rw-r--r--   0 zongheng   (502) staff       (20)     1155 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/requires.txt
+-rw-r--r--   0 zongheng   (502) staff       (20)        4 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/top_level.txt
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/tests/
+-rw-r--r--   0 zongheng   (502) staff       (20)     2574 2023-05-28 16:52:14.000000 skypilot-0.3.0/tests/test_cli.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     5061 2023-05-28 16:43:06.000000 skypilot-0.3.0/tests/test_config.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      300 2021-12-14 23:56:33.000000 skypilot-0.3.0/tests/test_file_mount_helper.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      260 2022-11-22 22:28:46.000000 skypilot-0.3.0/tests/test_global_user_state.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1076 2023-02-24 05:01:20.000000 skypilot-0.3.0/tests/test_list_accelerators.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    14008 2023-02-24 05:01:20.000000 skypilot-0.3.0/tests/test_onprem.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    19443 2023-05-28 16:45:59.000000 skypilot-0.3.0/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4663 2023-04-19 13:26:02.000000 skypilot-0.3.0/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 zongheng   (502) staff       (20)       94 2022-02-17 10:51:09.000000 skypilot-0.3.0/tests/test_pycryptodome_version.py
+-rw-r--r--   0 zongheng   (502) staff       (20)   100651 2023-05-28 17:22:30.000000 skypilot-0.3.0/tests/test_smoke.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     7206 2023-04-03 17:20:30.000000 skypilot-0.3.0/tests/test_spot.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4048 2023-05-28 16:43:06.000000 skypilot-0.3.0/tests/test_storage.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1070 2023-01-09 22:00:08.000000 skypilot-0.3.0/tests/test_wheels.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `skypilot-0.2.5/LICENSE` & `skypilot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/PKG-INFO` & `skypilot-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: skypilot
-Version: 0.2.5
+Version: 0.3.0
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
 Description-Content-Type: text/markdown
 Provides-Extra: aws
 Provides-Extra: azure
 Provides-Extra: gcp
+Provides-Extra: ibm
 Provides-Extra: docker
 Provides-Extra: lambda
+Provides-Extra: cloudflare
 Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
   <img alt="SkyPilot" src="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/skypilot-wide-light-1k.png" width=55%>
 </p>
 
@@ -46,14 +47,21 @@
 </p>
 
 
 <h3 align="center">
     Run jobs on any cloud, easily and cost effectively
 </h3>
 
+----
+:fire: :dromedary_camel: *News* :dromedary_camel: :fire: 
+- [April, 2023] **[**SkyPilot YAMLs released**](./llm/vicuna/) for finetuning & serving the Vicuna model with a single command**!
+- [March, 2023] **[Vicuna LLM chatbot](https://lmsys.org/blog/2023-03-30-vicuna/) trained** [**using SkyPilot**](./llm/vicuna/) **for $300 on spot instances!** 
+- [March, 2023] *Serve* your own LLaMA LLM chatbot (not finetuned) on any cloud: [**example**](./llm/llama-chatbots/), [**repo**](https://github.com/skypilot-org/sky-llama)
+----
+
 SkyPilot is a framework for easily and cost effectively running ML workloads<sup>[1]</sup> on any cloud. 
 
 SkyPilot abstracts away the cloud infra burden:
 - Launch jobs & clusters on any cloud (AWS, Azure, GCP, Lambda Cloud)
 - Find scarce resources across zones/regions/clouds
 - Queue jobs & use cloud object stores
 
@@ -135,15 +143,17 @@
 - [Documentation](https://skypilot.readthedocs.io/en/latest/)
 - [Example: HuggingFace](https://skypilot.readthedocs.io/en/latest/getting-started/tutorial.html) 
 - [Tutorials](https://github.com/skypilot-org/skypilot-tutorial) 
 - [YAML reference](https://skypilot.readthedocs.io/en/latest/reference/yaml-spec.html)
 - Framework examples: [PyTorch DDP](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_torch.yaml),  [Distributed](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_tf_app.py) [TensorFlow](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_app_storage.yaml), [JAX/Flax on TPU](https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/tree/master/examples/stable_diffusion), [Detectron2](https://github.com/skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml), [programmatic grid search](https://github.com/skypilot-org/skypilot/blob/master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml), and [many more](./examples).
 
 More information:
-- [Introductory blog post](https://medium.com/@zongheng_yang/skypilot-ml-and-data-science-on-any-cloud-with-massive-cost-savings-244189cc7c0f)
+- [SkyPilot Blog](https://blog.skypilot.co/)
+  - [Introductory blog post](https://blog.skypilot.co/introducing-skypilot/)
+- [NSDI 2023 paper & talk](https://www.usenix.org/conference/nsdi23/presentation/yang-zongheng)
 
 ## Issues, feature requests, and questions
 We are excited to hear your feedback! 
 * For issues and feature requests, please [open a GitHub issue](https://github.com/skypilot-org/skypilot/issues/new).
 * For questions, please use [GitHub Discussions](https://github.com/skypilot-org/skypilot/discussions).
 
 For general discussions, join us on the [SkyPilot Slack](http://slack.skypilot.co).
```

#### html2text {}

```diff
@@ -1,31 +1,38 @@
-Metadata-Version: 2.1 Name: skypilot Version: 0.2.5 Summary: SkyPilot: An
+Metadata-Version: 2.1 Name: skypilot Version: 0.3.0 Summary: SkyPilot: An
 intercloud broker for the clouds Author: SkyPilot Team License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot Project-URL:
 Issues, https://github.com/skypilot-org/skypilot/issues Project-URL:
 Discussion, https://github.com/skypilot-org/skypilot/discussions Project-URL:
 Documentation, https://skypilot.readthedocs.io/en/latest/ Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: System ::
-Distributed Computing Description-Content-Type: text/markdown Provides-Extra:
-aws Provides-Extra: azure Provides-Extra: gcp Provides-Extra: docker Provides-
-Extra: lambda Provides-Extra: all License-File: LICENSE
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Distributed Computing Description-Content-Type:
+text/markdown Provides-Extra: aws Provides-Extra: azure Provides-Extra: gcp
+Provides-Extra: ibm Provides-Extra: docker Provides-Extra: lambda Provides-
+Extra: cloudflare Provides-Extra: all License-File: LICENSE
                                   [SkyPilot]
                  [Documentation] [GitHub_Release] [Join_Slack]
          **** Run jobs on any cloud, easily and cost effectively ****
-SkyPilot is a framework for easily and cost effectively running ML workloads[1]
-on any cloud. SkyPilot abstracts away the cloud infra burden: - Launch jobs &
-clusters on any cloud (AWS, Azure, GCP, Lambda Cloud) - Find scarce resources
-across zones/regions/clouds - Queue jobs & use cloud object stores SkyPilot
-cuts your cloud costs: * [Managed Spot](https://skypilot.readthedocs.io/en/
-latest/examples/spot-jobs.html): **3x cost savings** using spot VMs, with auto-
+---- :fire: :dromedary_camel: *News* :dromedary_camel: :fire: - [April, 2023]
+**[**SkyPilot YAMLs released**](./llm/vicuna/) for finetuning & serving the
+Vicuna model with a single command**! - [March, 2023] **[Vicuna LLM chatbot]
+(https://lmsys.org/blog/2023-03-30-vicuna/) trained** [**using SkyPilot**](./
+llm/vicuna/) **for $300 on spot instances!** - [March, 2023] *Serve* your own
+LLaMA LLM chatbot (not finetuned) on any cloud: [**example**](./llm/llama-
+chatbots/), [**repo**](https://github.com/skypilot-org/sky-llama) ---- SkyPilot
+is a framework for easily and cost effectively running ML workloads[1] on any
+cloud. SkyPilot abstracts away the cloud infra burden: - Launch jobs & clusters
+on any cloud (AWS, Azure, GCP, Lambda Cloud) - Find scarce resources across
+zones/regions/clouds - Queue jobs & use cloud object stores SkyPilot cuts your
+cloud costs: * [Managed Spot](https://skypilot.readthedocs.io/en/latest/
+examples/spot-jobs.html): **3x cost savings** using spot VMs, with auto-
 recovery from preemptions * [Autostop](https://skypilot.readthedocs.io/en/
 latest/reference/auto-stop.html): hands-free cleanup of idle clusters *
 [Benchmark](https://skypilot.readthedocs.io/en/latest/reference/benchmark/
 index.html): find best VM types for your jobs * Optimizer: **2x cost savings**
 by auto-picking best prices across zones/regions/clouds SkyPilot supports your
 existing GPU, TPU, and CPU workloads, with no code changes. Install with pip
 (choose your clouds) or [from source](https://skypilot.readthedocs.io/en/
@@ -72,17 +79,18 @@
 (https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/
 tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/
 tree/master/examples/stable_diffusion), [Detectron2](https://github.com/
 skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml),
 [programmatic grid search](https://github.com/skypilot-org/skypilot/blob/
 master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://
 github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml),
-and [many more](./examples). More information: - [Introductory blog post]
-(https://medium.com/@zongheng_yang/skypilot-ml-and-data-science-on-any-cloud-
-with-massive-cost-savings-244189cc7c0f) ## Issues, feature requests, and
+and [many more](./examples). More information: - [SkyPilot Blog](https://
+blog.skypilot.co/) - [Introductory blog post](https://blog.skypilot.co/
+introducing-skypilot/) - [NSDI 2023 paper & talk](https://www.usenix.org/
+conference/nsdi23/presentation/yang-zongheng) ## Issues, feature requests, and
 questions We are excited to hear your feedback! * For issues and feature
 requests, please [open a GitHub issue](https://github.com/skypilot-org/
 skypilot/issues/new). * For questions, please use [GitHub Discussions](https://
 github.com/skypilot-org/skypilot/discussions). For general discussions, join us
 on the [SkyPilot Slack](http://slack.skypilot.co). ## Contributing We welcome
 and value all contributions to the project! Please refer to [CONTRIBUTING]
 (CONTRIBUTING.md) for how to get involved. # [1]: While SkyPilot is currently
```

### Comparing `skypilot-0.2.5/README.md` & `skypilot-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 </p>
 
 
 <h3 align="center">
     Run jobs on any cloud, easily and cost effectively
 </h3>
 
+----
+:fire: :dromedary_camel: *News* :dromedary_camel: :fire: 
+- [April, 2023] **[**SkyPilot YAMLs released**](./llm/vicuna/) for finetuning & serving the Vicuna model with a single command**!
+- [March, 2023] **[Vicuna LLM chatbot](https://lmsys.org/blog/2023-03-30-vicuna/) trained** [**using SkyPilot**](./llm/vicuna/) **for $300 on spot instances!** 
+- [March, 2023] *Serve* your own LLaMA LLM chatbot (not finetuned) on any cloud: [**example**](./llm/llama-chatbots/), [**repo**](https://github.com/skypilot-org/sky-llama)
+----
+
 SkyPilot is a framework for easily and cost effectively running ML workloads[^1] on any cloud. 
 
 SkyPilot abstracts away the cloud infra burden:
 - Launch jobs & clusters on any cloud (AWS, Azure, GCP, Lambda Cloud)
 - Find scarce resources across zones/regions/clouds
 - Queue jobs & use cloud object stores
 
@@ -110,15 +117,17 @@
 - [Documentation](https://skypilot.readthedocs.io/en/latest/)
 - [Example: HuggingFace](https://skypilot.readthedocs.io/en/latest/getting-started/tutorial.html) 
 - [Tutorials](https://github.com/skypilot-org/skypilot-tutorial) 
 - [YAML reference](https://skypilot.readthedocs.io/en/latest/reference/yaml-spec.html)
 - Framework examples: [PyTorch DDP](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_torch.yaml),  [Distributed](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_tf_app.py) [TensorFlow](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_app_storage.yaml), [JAX/Flax on TPU](https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/tree/master/examples/stable_diffusion), [Detectron2](https://github.com/skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml), [programmatic grid search](https://github.com/skypilot-org/skypilot/blob/master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml), and [many more](./examples).
 
 More information:
-- [Introductory blog post](https://medium.com/@zongheng_yang/skypilot-ml-and-data-science-on-any-cloud-with-massive-cost-savings-244189cc7c0f)
+- [SkyPilot Blog](https://blog.skypilot.co/)
+  - [Introductory blog post](https://blog.skypilot.co/introducing-skypilot/)
+- [NSDI 2023 paper & talk](https://www.usenix.org/conference/nsdi23/presentation/yang-zongheng)
 
 ## Issues, feature requests, and questions
 We are excited to hear your feedback! 
 * For issues and feature requests, please [open a GitHub issue](https://github.com/skypilot-org/skypilot/issues/new).
 * For questions, please use [GitHub Discussions](https://github.com/skypilot-org/skypilot/discussions).
 
 For general discussions, join us on the [SkyPilot Slack](http://slack.skypilot.co).
```

#### html2text {}

```diff
@@ -1,51 +1,58 @@
                                    [SkyPilot]
                  [Documentation] [GitHub_Release] [Join_Slack]
          **** Run jobs on any cloud, easily and cost effectively ****
-SkyPilot is a framework for easily and cost effectively running ML workloads
-[^1] on any cloud. SkyPilot abstracts away the cloud infra burden: - Launch
-jobs & clusters on any cloud (AWS, Azure, GCP, Lambda Cloud) - Find scarce
-resources across zones/regions/clouds - Queue jobs & use cloud object stores
-SkyPilot cuts your cloud costs: * [Managed Spot](https://
-skypilot.readthedocs.io/en/latest/examples/spot-jobs.html): **3x cost savings**
-using spot VMs, with auto-recovery from preemptions * [Autostop](https://
-skypilot.readthedocs.io/en/latest/reference/auto-stop.html): hands-free cleanup
-of idle clusters * [Benchmark](https://skypilot.readthedocs.io/en/latest/
-reference/benchmark/index.html): find best VM types for your jobs * Optimizer:
-**2x cost savings** by auto-picking best prices across zones/regions/clouds
-SkyPilot supports your existing GPU, TPU, and CPU workloads, with no code
-changes. Install with pip (choose your clouds) or [from source](https://
-skypilot.readthedocs.io/en/latest/getting-started/installation.html): ``` pip
-install "skypilot[aws,gcp,azure,lambda]" ``` ## Getting Started You can find
-our documentation [here](https://skypilot.readthedocs.io/en/latest/). -
-[Installation](https://skypilot.readthedocs.io/en/latest/getting-started/
-installation.html) - [Quickstart](https://skypilot.readthedocs.io/en/latest/
-getting-started/quickstart.html) - [CLI reference](https://
-skypilot.readthedocs.io/en/latest/reference/cli.html) ## SkyPilot in 1 minute A
-SkyPilot task specifies: resource requirements, data to be synced, setup
-commands, and the task commands. Once written in this [**unified interface**]
-(https://skypilot.readthedocs.io/en/latest/reference/yaml-spec.html) (YAML or
-Python API), the task can be launched on any available cloud. This avoids
-vendor lock-in, and allows easily moving jobs to a different provider. Paste
-the following into a file `my_task.yaml`: ```yaml resources: accelerators:
-V100:1 # 1x NVIDIA V100 GPU num_nodes: 1 # Number of VMs to launch # Working
-directory (optional) containing the project codebase. # Its contents are synced
-to ~/sky_workdir/ on the cluster. workdir: ~/torch_examples # Commands to be
-run before executing the job. # Typical use: pip install -r requirements.txt,
-git clone, etc. setup: | pip install torch torchvision # Commands to run as a
-job. # Typical use: launch the main program. run: | cd mnist python main.py --
-epochs 1 ``` Prepare the workdir by cloning: ```bash git clone https://
-github.com/pytorch/examples.git ~/torch_examples ``` Launch with `sky launch`
-(note: [access to GPU instances](https://skypilot.readthedocs.io/en/latest/
-reference/quota.html) is needed for this example): ```bash sky launch
-my_task.yaml ``` SkyPilot then performs the heavy-lifting for you, including:
-1. Find the lowest priced VM instance type across different clouds 2. Provision
-the VM, with auto-failover if the cloud returned capacity errors 3. Sync the
-local `workdir` to the VM 4. Run the task's `setup` commands to prepare the VM
-for running the task 5. Run the task's `run` commands
+---- :fire: :dromedary_camel: *News* :dromedary_camel: :fire: - [April, 2023]
+**[**SkyPilot YAMLs released**](./llm/vicuna/) for finetuning & serving the
+Vicuna model with a single command**! - [March, 2023] **[Vicuna LLM chatbot]
+(https://lmsys.org/blog/2023-03-30-vicuna/) trained** [**using SkyPilot**](./
+llm/vicuna/) **for $300 on spot instances!** - [March, 2023] *Serve* your own
+LLaMA LLM chatbot (not finetuned) on any cloud: [**example**](./llm/llama-
+chatbots/), [**repo**](https://github.com/skypilot-org/sky-llama) ---- SkyPilot
+is a framework for easily and cost effectively running ML workloads[^1] on any
+cloud. SkyPilot abstracts away the cloud infra burden: - Launch jobs & clusters
+on any cloud (AWS, Azure, GCP, Lambda Cloud) - Find scarce resources across
+zones/regions/clouds - Queue jobs & use cloud object stores SkyPilot cuts your
+cloud costs: * [Managed Spot](https://skypilot.readthedocs.io/en/latest/
+examples/spot-jobs.html): **3x cost savings** using spot VMs, with auto-
+recovery from preemptions * [Autostop](https://skypilot.readthedocs.io/en/
+latest/reference/auto-stop.html): hands-free cleanup of idle clusters *
+[Benchmark](https://skypilot.readthedocs.io/en/latest/reference/benchmark/
+index.html): find best VM types for your jobs * Optimizer: **2x cost savings**
+by auto-picking best prices across zones/regions/clouds SkyPilot supports your
+existing GPU, TPU, and CPU workloads, with no code changes. Install with pip
+(choose your clouds) or [from source](https://skypilot.readthedocs.io/en/
+latest/getting-started/installation.html): ``` pip install "skypilot
+[aws,gcp,azure,lambda]" ``` ## Getting Started You can find our documentation
+[here](https://skypilot.readthedocs.io/en/latest/). - [Installation](https://
+skypilot.readthedocs.io/en/latest/getting-started/installation.html) -
+[Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/
+quickstart.html) - [CLI reference](https://skypilot.readthedocs.io/en/latest/
+reference/cli.html) ## SkyPilot in 1 minute A SkyPilot task specifies: resource
+requirements, data to be synced, setup commands, and the task commands. Once
+written in this [**unified interface**](https://skypilot.readthedocs.io/en/
+latest/reference/yaml-spec.html) (YAML or Python API), the task can be launched
+on any available cloud. This avoids vendor lock-in, and allows easily moving
+jobs to a different provider. Paste the following into a file `my_task.yaml`:
+```yaml resources: accelerators: V100:1 # 1x NVIDIA V100 GPU num_nodes: 1 #
+Number of VMs to launch # Working directory (optional) containing the project
+codebase. # Its contents are synced to ~/sky_workdir/ on the cluster. workdir:
+~/torch_examples # Commands to be run before executing the job. # Typical use:
+pip install -r requirements.txt, git clone, etc. setup: | pip install torch
+torchvision # Commands to run as a job. # Typical use: launch the main program.
+run: | cd mnist python main.py --epochs 1 ``` Prepare the workdir by cloning:
+```bash git clone https://github.com/pytorch/examples.git ~/torch_examples ```
+Launch with `sky launch` (note: [access to GPU instances](https://
+skypilot.readthedocs.io/en/latest/reference/quota.html) is needed for this
+example): ```bash sky launch my_task.yaml ``` SkyPilot then performs the heavy-
+lifting for you, including: 1. Find the lowest priced VM instance type across
+different clouds 2. Provision the VM, with auto-failover if the cloud returned
+capacity errors 3. Sync the local `workdir` to the VM 4. Run the task's `setup`
+commands to prepare the VM for running the task 5. Run the task's `run`
+commands
                                 [SkyPilot Demo]
 Refer to [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-
 started/quickstart.html) to get started with SkyPilot. ## Learn more -
 [Documentation](https://skypilot.readthedocs.io/en/latest/) - [Example:
 HuggingFace](https://skypilot.readthedocs.io/en/latest/getting-started/
 tutorial.html) - [Tutorials](https://github.com/skypilot-org/skypilot-tutorial)
 - [YAML reference](https://skypilot.readthedocs.io/en/latest/reference/yaml-
@@ -57,17 +64,18 @@
 (https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/
 tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/
 tree/master/examples/stable_diffusion), [Detectron2](https://github.com/
 skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml),
 [programmatic grid search](https://github.com/skypilot-org/skypilot/blob/
 master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://
 github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml),
-and [many more](./examples). More information: - [Introductory blog post]
-(https://medium.com/@zongheng_yang/skypilot-ml-and-data-science-on-any-cloud-
-with-massive-cost-savings-244189cc7c0f) ## Issues, feature requests, and
+and [many more](./examples). More information: - [SkyPilot Blog](https://
+blog.skypilot.co/) - [Introductory blog post](https://blog.skypilot.co/
+introducing-skypilot/) - [NSDI 2023 paper & talk](https://www.usenix.org/
+conference/nsdi23/presentation/yang-zongheng) ## Issues, feature requests, and
 questions We are excited to hear your feedback! * For issues and feature
 requests, please [open a GitHub issue](https://github.com/skypilot-org/
 skypilot/issues/new). * For questions, please use [GitHub Discussions](https://
 github.com/skypilot-org/skypilot/discussions). For general discussions, join us
 on the [SkyPilot Slack](http://slack.skypilot.co). ## Contributing We welcome
 and value all contributions to the project! Please refer to [CONTRIBUTING]
 (CONTRIBUTING.md) for how to get involved.  [^1]: While SkyPilot is currently
```

### Comparing `skypilot-0.2.5/pyproject.toml` & `skypilot-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 [build-system]
 requires = ["setuptools>=58.0"]
 build-backend = "setuptools.build_meta"
 
-[project]
-name = "skypilot"
-
 [tool.yapf]
 based_on_style = "google"
 allow_split_before_dict_value = false
 
 [tool.pytest.ini_options]
 required_plugins = [
     "pytest-xdist",
```

### Comparing `skypilot-0.2.5/setup.py` & `skypilot-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,17 +61,16 @@
         re.MULTILINE)
     readme = mode_re.sub(r'<img\1>', readme)
     return readme
 
 
 install_requires = [
     'wheel',
-    # NOTE: ray 2.0.1 requires click<=8.0.4,>=7.0; We disable the
-    # shell completion for click<8.0 for backward compatibility.
-    'click<=8.0.4,>=7.0',
+    # NOTE: ray requires click>=7.0
+    'click>=7.0',
     # NOTE: required by awscli. To avoid ray automatically installing
     # the latest version.
     'colorama<0.4.5',
     'cryptography',
     # Jinja has a bug in older versions because of the lack of pinning
     # the version of the underlying markupsafe package. See:
     # https://github.com/pallets/jinja/issues/1585
@@ -80,51 +79,63 @@
     'networkx',
     'oauth2client',
     'pandas',
     'pendulum',
     # PrettyTable with version >=2.0.0 is required for the support of
     # `add_rows` method.
     'PrettyTable>=2.0.0',
-    # Lower local ray version is not fully supported, due to the
-    # autoscaler issues (also tracked in #537).
-    'ray[default]>=1.9.0,<=2.3.0',
+    # Lower version of ray will cause dependency conflict for
+    # click/grpcio/protobuf.
+    'ray[default]>=2.2.0,<=2.4.0',
     'rich',
     'tabulate',
-    'typing-extensions',
-    'filelock',  # TODO(mraheja): Enforce >=3.6.0 when python version is >= 3.7
-    # This is used by ray. The latest 1.44.0 will generate an error
-    # `Fork support is only compatible with the epoll1 and poll
-    # polling strategies`
-    'grpcio>=1.32.0,<=1.43.0',
+    # Light weight requirement, can be replaced with "typing" once
+    # we deprecate Python 3.7 (this will take a while).
+    "typing_extensions; python_version < '3.8'",
+    'filelock>=3.6.0',
+    # Adopted from ray's setup.py:
+    # Tracking issue: https://github.com/ray-project/ray/issues/30984
+    "grpcio >= 1.32.0, <= 1.49.1; python_version < '3.10' and sys_platform == 'darwin'",  # noqa:E501
+    "grpcio >= 1.42.0, <= 1.49.1; python_version >= '3.10' and sys_platform == 'darwin'",  # noqa:E501
+    # Original issue: https://github.com/ray-project/ray/issues/33833
+    "grpcio >= 1.32.0, <= 1.51.3; python_version < '3.10' and sys_platform != 'darwin'",  # noqa:E501
+    "grpcio >= 1.42.0, <= 1.51.3; python_version >= '3.10' and sys_platform != 'darwin'",  # noqa:E501
     'packaging',
-    # The latest 4.21.1 will break ray. Enforce < 4.0.0 until Ray releases the
-    # fix.
-    # https://github.com/ray-project/ray/pull/25211
-    'protobuf<4.0.0',
+    # Adopted from ray's setup.py:
+    # https://github.com/ray-project/ray/blob/86fab1764e618215d8131e8e5068f0d493c77023/python/setup.py#L326
+    'protobuf >= 3.15.3, != 3.19.5',
     'psutil',
     'pulp',
 ]
 
 # NOTE: Change the templates/spot-controller.yaml.j2 file if any of the following
 # packages dependencies are changed.
+aws_dependencies = [
+    # awscli>=1.27.10 is required for SSO support.
+    'awscli',
+    'boto3',
+    # 'Crypto' module used in authentication.py for AWS.
+    'pycryptodome==3.12.0',
+]
 extras_require: Dict[str, List[str]] = {
-    'aws': [
-        # awscli>=1.27.10 is required for SSO support.
-        'awscli',
-        'boto3',
-        # 'Crypto' module used in authentication.py for AWS.
-        'pycryptodome==3.12.0',
-    ],
+    'aws': aws_dependencies,
     # TODO(zongheng): azure-cli is huge and takes a long time to install.
     # Tracked in: https://github.com/Azure/azure-cli/issues/7387
     # azure-identity is needed in node_provider.
-    'azure': ['azure-cli>=2.31.0', 'azure-core', 'azure-identity'],
+    # We need azure-identity>=1.13.0 to enable the customization of the
+    # timeout of AzureCliCredential.
+    'azure': [
+        'azure-cli>=2.31.0', 'azure-core', 'azure-identity>=1.13.0',
+        'azure-mgmt-network'
+    ],
     'gcp': ['google-api-python-client', 'google-cloud-storage'],
+    'ibm': ['ibm-cloud-sdk-core', 'ibm-vpc', 'ibm-platform-services'],
     'docker': ['docker'],
     'lambda': [],
+    'cloudflare': aws_dependencies
 }
 
 extras_require['all'] = sum(extras_require.values(), [])
 
 # Install aws requirements by default, as it is the most common cloud provider,
 # and the installation is quick.
 install_requires += extras_require['aws']
@@ -147,23 +158,22 @@
     author='SkyPilot Team',
     license='Apache 2.0',
     readme='README.md',
     description='SkyPilot: An intercloud broker for the clouds',
     long_description=long_description,
     long_description_content_type='text/markdown',
     setup_requires=['wheel'],
-    requires_python='>=3.6',
+    requires_python='>=3.7',
     install_requires=install_requires,
     extras_require=extras_require,
     entry_points={
         'console_scripts': ['sky = sky.cli:cli'],
     },
     include_package_data=True,
     classifiers=[
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

### Comparing `skypilot-0.2.5/sky/__init__.py` & `skypilot-0.3.0/sky/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The SkyPilot package."""
 import os
 
 # Replaced with the current commit when building the wheels.
-__commit__ = '14cb4b56bb56cbc6b1a59fa35ae59c881348690c'
-__version__ = '0.2.5'
+__commit__ = '3deccb2a7360d086952601188381c28f932e118e'
+__version__ = '0.3.0'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 # Keep this order to avoid cyclic imports
 from sky import backends
 from sky import benchmark
 from sky import clouds
 from sky.clouds.service_catalog import list_accelerators
@@ -21,23 +21,25 @@
 from sky.skylet.job_lib import JobStatus
 from sky.core import (status, start, stop, down, autostop, queue, cancel,
                       tail_logs, download_logs, job_status, spot_queue,
                       spot_status, spot_cancel, storage_ls, storage_delete,
                       cost_report)
 
 # Aliases.
+IBM = clouds.IBM
 AWS = clouds.AWS
 Azure = clouds.Azure
 GCP = clouds.GCP
 Lambda = clouds.Lambda
 Local = clouds.Local
 optimize = Optimizer.optimize
 
 __all__ = [
     '__version__',
+    'IBM',
     'AWS',
     'Azure',
     'GCP',
     'Lambda',
     'Local',
     'Optimizer',
     'OptimizeTarget',
```

### Comparing `skypilot-0.2.5/sky/adaptors/aws.py` & `skypilot-0.3.0/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/adaptors/azure.py` & `skypilot-0.3.0/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/adaptors/docker.py` & `skypilot-0.3.0/sky/adaptors/docker.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/adaptors/gcp.py` & `skypilot-0.3.0/sky/adaptors/gcp.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         if googleapiclient is None or google is None:
             try:
                 import googleapiclient as _googleapiclient
                 import google as _google
                 googleapiclient = _googleapiclient
                 google = _google
             except ImportError:
-                raise ImportError('Fail to import dependencies for GCP.'
-                                  'Try pip install "skypilot[gcp]"') from None
+                raise ImportError('Failed to import dependencies for GCP. '
+                                  'Try: pip install "skypilot[gcp]"') from None
         return func(*args, **kwargs)
 
     return wrapper
 
 
 @import_package
 def build(service_name: str, version: str, *args, **kwargs):
```

### Comparing `skypilot-0.2.5/sky/authentication.py` & `skypilot-0.3.0/sky/authentication.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import copy
 import functools
 import os
 import re
 import socket
 import subprocess
 import sys
-import textwrap
 import time
 from typing import Any, Dict, Tuple
+import uuid
 
 import colorama
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.hazmat.backends import default_backend
+import yaml
 
 from sky import clouds
 from sky import sky_logging
-from sky.adaptors import gcp
+from sky.adaptors import gcp, ibm
 from sky.utils import common_utils
 from sky.utils import subprocess_utils
 from sky.utils import ux_utils
 from sky.skylet.providers.lambda_cloud import lambda_utils
 
 logger = sky_logging.init_logger(__name__)
 
@@ -83,34 +84,30 @@
         #   AssertionError: /home/ubuntu/.ssh/sky-key.pub
         assert os.path.exists(public_key_path), (
             'Private key found, but associated public key '
             f'{public_key_path} does not exist.')
     return private_key_path, public_key_path
 
 
+def _replace_cloud_init_ssh_info_in_config(config: Dict[str, Any],
+                                           public_key: str) -> Dict[str, Any]:
+    config_str = common_utils.dump_yaml_str(config)
+    config_str = config_str.replace('skypilot:ssh_user',
+                                    config['auth']['ssh_user'])
+    config_str = config_str.replace('skypilot:ssh_public_key_content',
+                                    public_key)
+    config = yaml.safe_load(config_str)
+    return config
+
+
 def setup_aws_authentication(config: Dict[str, Any]) -> Dict[str, Any]:
     _, public_key_path = get_or_generate_keys()
     with open(public_key_path, 'r') as f:
         public_key = f.read()
-    # Use cloud init in UserData to set up the authorized_keys to get
-    # around the number of keys limit and permission issues with
-    # ec2.describe_key_pairs.
-    # Note that sudo and shell need to be specified to ensure setup works.
-    # Reference: https://cloudinit.readthedocs.io/en/latest/reference/modules.html#users-and-groups  # pylint: disable=line-too-long
-    for node_type in config['available_node_types']:
-        config['available_node_types'][node_type]['node_config']['UserData'] = (
-            textwrap.dedent(f"""\
-            #cloud-config
-            users:
-            - name: {config['auth']['ssh_user']}
-              shell: /bin/bash
-              sudo: ALL=(ALL) NOPASSWD:ALL
-              ssh-authorized-keys:
-                - {public_key}
-            """))
+    config = _replace_cloud_init_ssh_info_in_config(config, public_key)
     return config
 
 
 # Reference:
 # https://github.com/ray-project/ray/blob/master/python/ray/autoscaler/_private/gcp/config.py
 def _wait_for_compute_global_operation(project_name: str, operation_name: str,
                                        compute: Any) -> None:
@@ -313,23 +310,82 @@
 
 
 def setup_lambda_authentication(config: Dict[str, Any]) -> Dict[str, Any]:
     get_or_generate_keys()
 
     # Ensure ssh key is registered with Lambda Cloud
     lambda_client = lambda_utils.LambdaCloudClient()
-    if lambda_client.ssh_key_name is None:
-        public_key_path = os.path.expanduser(PUBLIC_SSH_KEY_PATH)
-        with open(public_key_path, 'r') as f:
-            public_key = f.read()
-        name = f'sky-key-{common_utils.get_user_hash()}'
-        lambda_client.set_ssh_key(name, public_key)
+    public_key_path = os.path.expanduser(PUBLIC_SSH_KEY_PATH)
+    with open(public_key_path, 'r') as f:
+        public_key = f.read()
+    prefix = f'sky-key-{common_utils.get_user_hash()}'
+    name, exists = lambda_client.get_unique_ssh_key_name(prefix, public_key)
+    if not exists:
+        lambda_client.register_ssh_key(name, public_key)
 
     # Need to use ~ relative path because Ray uses the same
     # path for finding the public key path on both local and head node.
     config['auth']['ssh_public_key'] = PUBLIC_SSH_KEY_PATH
 
     file_mounts = config['file_mounts']
     file_mounts[PUBLIC_SSH_KEY_PATH] = PUBLIC_SSH_KEY_PATH
     config['file_mounts'] = file_mounts
 
     return config
+
+
+def setup_ibm_authentication(config):
+    """ registers keys if they do not exist in sky folder
+    and updates config file.
+    keys default location: '~/.ssh/sky-key' and '~/.ssh/sky-key.pub'
+    """
+
+    def _get_unique_key_name():
+        suffix_len = 10
+        return f'skypilot-key-{str(uuid.uuid4())[:suffix_len]}'
+
+    client = ibm.client(region=config['provider']['region'])
+    resource_group_id = config['provider']['resource_group_id']
+
+    _, public_key_path = get_or_generate_keys()
+    with open(os.path.abspath(os.path.expanduser(public_key_path)),
+              'r',
+              encoding='utf-8') as file:
+        ssh_key_data = file.read()
+    # pylint: disable=E1136
+    try:
+        res = client.create_key(public_key=ssh_key_data,
+                                name=_get_unique_key_name(),
+                                resource_group={
+                                    'id': resource_group_id
+                                },
+                                type='rsa').get_result()
+        vpc_key_id = res['id']
+        logger.debug(f'Created new key: {res["name"]}')
+
+    except ibm.ibm_cloud_sdk_core.ApiException as e:
+        if 'Key with fingerprint already exists' in e.message:
+            for key in client.list_keys().result['keys']:
+                if (ssh_key_data in key['public_key'] or
+                        key['public_key'] in ssh_key_data):
+                    vpc_key_id = key['id']
+                    logger.debug(f'Reusing key:{key["name"]}, '
+                                 f'matching existing public key.')
+                    break
+        elif 'Key with name already exists' in e.message:
+            raise Exception("""a key with chosen name
+                already registered in the specified region""") from e
+        else:
+            raise Exception('Failed to register a key') from e
+
+    config['auth']['ssh_private_key'] = PRIVATE_SSH_KEY_PATH
+
+    for node_type in config['available_node_types']:
+        config['available_node_types'][node_type]['node_config'][
+            'key_id'] = vpc_key_id
+
+    # Add public key path to file mounts
+    file_mounts = config['file_mounts']
+    file_mounts[PUBLIC_SSH_KEY_PATH] = PUBLIC_SSH_KEY_PATH
+    config['file_mounts'] = file_mounts
+
+    return config
```

### Comparing `skypilot-0.2.5/sky/backends/backend.py` & `skypilot-0.3.0/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/backends/backend_utils.py` & `skypilot-0.3.0/sky/backends/backend_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 from datetime import datetime
 import difflib
 import enum
 import getpass
 import json
 import os
 import pathlib
+import random
 import re
 import subprocess
 import tempfile
 import textwrap
 import time
 import typing
-from typing import Any, Dict, List, Optional, Sequence, Set, Tuple, Union
+from typing import (Any, Dict, List, Mapping, Optional, Sequence, Set, Tuple,
+                    Union)
 from typing_extensions import Literal
 import uuid
 
 import colorama
 import filelock
 import jinja2
 import jsonschema
@@ -47,14 +49,15 @@
 from sky.utils import log_utils
 from sky.utils import subprocess_utils
 from sky.utils import timeline
 from sky.utils import tpu_utils
 from sky.utils import ux_utils
 from sky.utils import validator
 from sky.usage import usage_lib
+from sky.adaptors import ibm
 
 if typing.TYPE_CHECKING:
     from sky import resources
     from sky import task as task_lib
     from sky.backends import cloud_vm_ray_backend
     from sky.backends import local_docker_backend
 
@@ -79,18 +82,20 @@
 # Intentionally not using prefix 'rf' for the string format because yapf have a
 # bug with python=3.6.
 # 10.133.0.5: ray.worker.default,
 _LAUNCHING_IP_PATTERN = re.compile(
     r'({}): ray[._]worker[._]default'.format(IP_ADDR_REGEX))
 WAIT_HEAD_NODE_IP_MAX_ATTEMPTS = 3
 
-# We use fixed IP address to avoid DNS lookup blocking the check, for machine
-# with no internet connection.
+# We check network connection by going through _TEST_IP_LIST. We may need to
+# check multiple IPs because some IPs may be blocked on certain networks.
+# Fixed IP addresses are used to avoid DNS lookup blocking the check, for
+# machine with no internet connection.
 # Refer to: https://stackoverflow.com/questions/3764291/how-can-i-see-if-theres-an-available-and-active-network-connection-in-python # pylint: disable=line-too-long
-_TEST_IP = 'https://8.8.8.8'
+_TEST_IP_LIST = ['https://1.1.1.1', 'https://8.8.8.8']
 
 # Allow each CPU thread take 2 tasks.
 # Note: This value cannot be too small, otherwise OOM issue may occur.
 DEFAULT_TASK_CPU_DEMAND = 0.5
 
 # Mapping from reserved cluster names to the corresponding group name (logging
 # purpose).
@@ -120,16 +125,21 @@
 }
 # For these keys, don't use the old yaml's version and instead use the new yaml's.
 #  - zone: The zone field of the old yaml may be '1a,1b,1c' (AWS) while the actual
 #    zone of the launched cluster is '1a'. If we restore, then on capacity errors
 #    it's possible to failover to 1b, which leaves a leaked instance in 1a. Here,
 #    we use the new yaml's zone field, which is guaranteed to be the existing zone
 #    '1a'.
+# - UserData: The UserData field of the old yaml may be outdated, and we want to
+#   use the new yaml's UserData field, which contains the authorized key setup as
+#   well as the disabling of the auto-update with apt-get.
 _RAY_YAML_KEYS_TO_RESTORE_EXCEPTIONS = [
     ('provider', 'availability_zone'),
+    ('available_node_types', 'ray.head.default', 'node_config', 'UserData'),
+    ('available_node_types', 'ray.worker.default', 'node_config', 'UserData'),
 ]
 
 
 def is_ip(s: str) -> bool:
     """Returns whether this string matches IP_ADDR_REGEX."""
     return len(re.findall(IP_ADDR_REGEX, s)) == 1
 
@@ -262,15 +272,15 @@
     rsync_output = str(
         subprocess.check_output(
             f'rsync {command_runner.RSYNC_DISPLAY_OPTION} '
             f'{command_runner.RSYNC_FILTER_OPTION} '
             f'{git_exclude_filter} --dry-run {path!r}',
             shell=True).splitlines()[-1])
     total_bytes = rsync_output.split(' ')[3].replace(',', '')
-    return int(total_bytes) // 10**6
+    return int(float(total_bytes)) // 10**6
 
 
 class FileMountHelper(object):
     """Helper for handling file mounts."""
 
     @classmethod
     def wrap_file_mount(cls, path: str) -> str:
@@ -696,15 +706,15 @@
                 break
             if 'Host' in config_str:
                 break
 
 
 def _replace_yaml_dicts(
         new_yaml: str, old_yaml: str, restore_key_names: Set[str],
-        restore_key_names_exceptions: Sequence[Sequence[str]]) -> str:
+        restore_key_names_exceptions: Sequence[Tuple[str, ...]]) -> str:
     """Replaces 'new' with 'old' for all keys in restore_key_names.
 
     The replacement will be applied recursively and only for the blocks
     with the key in key_names, and have the same ancestors in both 'new'
     and 'old' YAML tree.
 
     The restore_key_names_exceptions is a list of key names that should not
@@ -768,27 +778,30 @@
 
     Returns: {provisioner: path to yaml, the provisioning spec}.
       'provisioner' can be
         - 'ray'
         - 'tpu-create-script' (if TPU is requested)
         - 'tpu-delete-script' (if TPU is requested)
     Raises:
-        exceptions.ResourcesUnavailableError: if the region/zones requested does not appear
-            in the catalog, or an ssh_proxy_command is specified but not for the given region.
+        exceptions.ResourcesUnavailableError: if the region/zones requested does
+            not appear in the catalog, or an ssh_proxy_command is specified but
+            not for the given region.
     """
     # task.best_resources may not be equal to to_provision if the user
     # is running a job with less resources than the cluster has.
     cloud = to_provision.cloud
-    # This can raise a ResourcesUnavailableError, when the region/zones requested
-    # does not appear in the catalog. It can be triggered when the user changed
-    # the catalog file, while there is a cluster in the removed region/zone.
-    # TODO(zhwu): We should change the exception type to a more specific one,
-    # as the ResourcesUnavailableError is overly used. Also, it would be better
-    # to move the check out of this function, i.e. the caller should be
-    # responsible for the validation.
+    # This can raise a ResourcesUnavailableError, when the region/zones
+    # requested does not appear in the catalog. It can be triggered when the
+    # user changed the catalog file, while there is a cluster in the removed
+    # region/zone.
+    #
+    # TODO(zhwu): We should change the exception type to a more specific one, as
+    # the ResourcesUnavailableError is overly used. Also, it would be better to
+    # move the check out of this function, i.e. the caller should be responsible
+    # for the validation.
     resources_vars = cloud.make_deploy_resources_variables(
         to_provision, region, zones)
     config_dict = {}
 
     azure_subscription_id = None
     if isinstance(cloud, clouds.Azure):
         azure_subscription_id = cloud.get_project_id(dryrun=dryrun)
@@ -814,23 +827,49 @@
         (str(cloud).lower(), 'ssh_proxy_command'), None)
     if (isinstance(ssh_proxy_command_config, str) or
             ssh_proxy_command_config is None):
         ssh_proxy_command = ssh_proxy_command_config
     else:
         # ssh_proxy_command_config: Dict[str, str], region_name -> command
         # This type check is done by skypilot_config at config load time.
-        if region_name not in ssh_proxy_command_config:
-            # Skip this region. The upper layer will handle the failover to
-            # other regions.
-            raise exceptions.ResourcesUnavailableError(
-                f'No ssh_proxy_command provided for region {region_name}. Skipped.'
-            )
-        ssh_proxy_command = ssh_proxy_command_config[region_name]
+
+        # There are two cases:
+        if keep_launch_fields_in_existing_config:
+            # (1) We're re-provisioning an existing cluster.
+            #
+            # We use None for ssh_proxy_command, which will be restored to the
+            # cluster's original value later by _replace_yaml_dicts().
+            ssh_proxy_command = None
+        else:
+            # (2) We're launching a new cluster.
+            #
+            # Resources.get_valid_regions_for_launchable() respects the keys (regions)
+            # in ssh_proxy_command in skypilot_config. So here we add an assert.
+            assert region_name in ssh_proxy_command_config, (
+                region_name, ssh_proxy_command_config)
+            ssh_proxy_command = ssh_proxy_command_config[region_name]
     logger.debug(f'Using ssh_proxy_command: {ssh_proxy_command!r}')
 
+    # User-supplied instance tags.
+    instance_tags = {}
+    instance_tags = skypilot_config.get_nested(
+        (str(cloud).lower(), 'instance_tags'), {})
+    if not isinstance(instance_tags, dict):
+        with ux_utils.print_exception_no_traceback():
+            raise ValueError('Custom instance_tags in config.yaml should '
+                             f'be a dict, but received {type(instance_tags)}.')
+
+    # Dump the Ray ports to a file for Ray job submission
+    ray_port = constants.SKY_REMOTE_RAY_PORT
+    ray_dashboard_port = constants.SKY_REMOTE_RAY_DASHBOARD_PORT
+    # Note we can not use json.dumps which will add a space between ":" and its value
+    # which causes the yaml parser to fail.
+    port_dict_str = f'{{"ray_port":{ray_port}, "ray_dashboard_port":{ray_dashboard_port}}}'
+    dump_port_command = f'python -c \'import json, os; json.dump({port_dict_str}, open(os.path.expanduser("{constants.SKY_REMOTE_RAY_PORT_FILE}"), "w"))\''
+
     # Use a tmp file path to avoid incomplete YAML file being re-used in the
     # future.
     tmp_yaml_path = yaml_path + '.tmp'
     fill_template(
         cluster_config_template,
         dict(
             resources_vars,
@@ -855,22 +894,30 @@
                 'vpc_name': skypilot_config.get_nested(('aws', 'vpc_name'),
                                                        None),
                 'use_internal_ips': skypilot_config.get_nested(
                     ('aws', 'use_internal_ips'), False),
                 # Not exactly AWS only, but we only test it's supported on AWS
                 # for now:
                 'ssh_proxy_command': ssh_proxy_command,
+                # User-supplied instance tags.
+                'instance_tags': instance_tags,
 
                 # Azure only:
                 'azure_subscription_id': azure_subscription_id,
                 'resource_group': f'{cluster_name}-{region_name}',
 
                 # GCP only:
                 'gcp_project_id': gcp_project_id,
 
+                # Port of Ray (GCS server).
+                # Ray's default port 6379 is conflicted with Redis.
+                'ray_port': ray_port,
+                'ray_dashboard_port': ray_dashboard_port,
+                'ray_temp_dir': constants.SKY_REMOTE_RAY_TEMPDIR,
+                'dump_port_command': dump_port_command,
                 # Ray version.
                 'ray_version': constants.SKY_REMOTE_RAY_VERSION,
                 # Cloud credentials for cloud storage.
                 'credentials': credentials,
                 # Sky remote utils.
                 'sky_remote_path': SKY_REMOTE_PATH,
                 'sky_local_path': str(local_wheel_path),
@@ -975,14 +1022,16 @@
         config = auth.setup_aws_authentication(config)
     elif isinstance(cloud, clouds.GCP):
         config = auth.setup_gcp_authentication(config)
     elif isinstance(cloud, clouds.Azure):
         config = auth.setup_azure_authentication(config)
     elif isinstance(cloud, clouds.Lambda):
         config = auth.setup_lambda_authentication(config)
+    elif isinstance(cloud, clouds.IBM):
+        config = auth.setup_ibm_authentication(config)
     else:
         assert isinstance(cloud, clouds.Local), cloud
         # Local cluster case, authentication is already filled by the user
         # in the local cluster config (in ~/.sky/local/...). There is no need
         # for Sky to generate authentication.
         pass
     common_utils.dump_yaml(cluster_config_file, config)
@@ -1172,15 +1221,16 @@
             rc, stdout, stderr = runner.run(cmd,
                                             log_path=log_path,
                                             stream_logs=stream_logs,
                                             require_outputs=True)
             subprocess_utils.handle_returncode(
                 rc,
                 cmd, ('Failed to run command before rsync '
-                      f'{origin_source} -> {target}.'),
+                      f'{origin_source} -> {target}. '
+                      'Ensure that the network is stable, then retry.'),
                 stderr=stdout + stderr)
 
         if run_rsync:
             assert source is not None
             # TODO(zhwu): Optimize for large amount of files.
             # zip / transfer / unzip
             runner.rsync(
@@ -1491,70 +1541,97 @@
 
 def check_network_connection():
     # Tolerate 3 retries as it is observed that connections can fail.
     adapter = adapters.HTTPAdapter(max_retries=retry_lib.Retry(total=3))
     http = requests.Session()
     http.mount('https://', adapter)
     http.mount('http://', adapter)
-    try:
-        http.head(_TEST_IP, timeout=3)
-    except (requests.Timeout, requests.exceptions.ConnectionError) as e:
-        raise exceptions.NetworkError(
-            'Could not refresh the cluster. Network seems down.') from e
+    for i, ip in enumerate(_TEST_IP_LIST):
+        try:
+            http.head(ip, timeout=3)
+            return
+        except (requests.Timeout, requests.exceptions.ConnectionError) as e:
+            if i == len(_TEST_IP_LIST) - 1:
+                raise exceptions.NetworkError('Could not refresh the cluster. '
+                                              'Network seems down.') from e
 
 
 def _process_cli_query(
-    cloud: str, cluster: str, query_cmd: str, deliminiator: str,
-    status_map: Dict[str, global_user_state.ClusterStatus]
+    cloud: str,
+    cluster: str,
+    query_cmd: str,
+    deliminator: str,
+    status_map: Mapping[str, Optional[global_user_state.ClusterStatus]],
+    max_retries: int = 3,
 ) -> List[global_user_state.ClusterStatus]:
     """Run the cloud CLI query and returns cluster status.
 
     Args:
         cloud: The cloud provider name.
         cluster: The cluster name.
         query_cmd: The cloud CLI query command.
-        deliminiator: The deliminiator separating the status in the output
+        deliminator: The deliminator separating the status in the output
             of the query command.
         status_map: A map from the CLI status string to the corresponding
             global_user_state.ClusterStatus.
+        max_retries: Maximum number of retries before giving up. For AWS only.
+
     Returns:
         A list of global_user_state.ClusterStatus of all existing nodes in the
         cluster. The list can be empty if none of the nodes in the clusters are
         found, i.e. the nodes are all terminated.
     """
     returncode, stdout, stderr = log_lib.run_with_log(query_cmd,
                                                       '/dev/null',
                                                       require_outputs=True,
                                                       shell=True)
     logger.debug(f'{query_cmd} returned {returncode}.\n'
                  '**** STDOUT ****\n'
                  f'{stdout}\n'
                  '**** STDERR ****\n'
                  f'{stderr}')
+
+    # Cloud-specific error handling.
     if (cloud == str(clouds.Azure()) and returncode == 2 and
             'argument --ids: expected at least one argument' in stderr):
         # Azure CLI has a returncode 2 when the cluster is not found, as
         # --ids <empty> is passed to the query command. In that case, the
         # cluster should be considered as DOWN.
         return []
+    if (cloud == str(clouds.AWS()) and returncode != 0 and
+            'Unable to locate credentials. You can configure credentials by '
+            'running "aws configure"' in stdout + stderr):
+        # AWS: has run into this rare error with spot controller (which has an
+        # assumed IAM role and is working fine most of the time).
+        #
+        # We do not know the root cause. For now, the hypothesis is instance
+        # metadata service is temporarily unavailable. So, we retry the query.
+        if max_retries > 0:
+            logger.info('Encountered AWS "Unable to locate credentials" '
+                        'error. Retrying.')
+            time.sleep(random.uniform(0, 1) * 2)
+            return _process_cli_query(cloud, cluster, query_cmd, deliminator,
+                                      status_map, max_retries - 1)
 
     if returncode != 0:
         with ux_utils.print_exception_no_traceback():
             raise exceptions.ClusterStatusFetchingError(
                 f'Failed to query {cloud} cluster {cluster!r} status: '
                 f'{stdout + stderr}')
 
     cluster_status = stdout.strip()
     if cluster_status == '':
         return []
-    return [
-        status_map[s]
-        for s in cluster_status.split(deliminiator)
-        if status_map[s] is not None
-    ]
+
+    statuses = []
+    for s in cluster_status.split(deliminator):
+        node_status = status_map[s]
+        if node_status is not None:
+            statuses.append(node_status)
+    return statuses
 
 
 def _query_status_aws(
     cluster: str,
     ray_config: Dict[str, Any],
 ) -> List[global_user_state.ClusterStatus]:
     status_map = {
@@ -1631,14 +1708,16 @@
 
     # GCP does not clean up preempted TPU VMs. We remove it ourselves.
     # TODO(wei-lin): handle multi-node cases.
     if use_tpu_vm and len(status_list) == 0:
         logger.debug(f'Terminating preempted TPU VM cluster {cluster}')
         backend = backends.CloudVmRayBackend()
         handle = global_user_state.get_handle_from_cluster_name(cluster)
+        assert isinstance(handle,
+                          backends.CloudVmRayResourceHandle), (cluster, handle)
         # Do not use refresh cluster status during teardown, as that will
         # cause inifinite recursion by calling cluster status refresh
         # again.
         # The caller of this function, `_update_cluster_status_no_lock() ->
         # _get_cluster_status_via_cloud_cli()`, will do the post teardown
         # cleanup, which will remove the cluster entry from the status table
         # & the ssh config file.
@@ -1678,14 +1757,56 @@
     #     f'az vm list --show-details --query "['
     #     f'?tags.\\"ray-cluster-name\\" == \'{handle.cluster_name}\' '
     #     '&& tags.\\"ray-node-type\\" == \'head\'].powerState" -o tsv'
     # )
     return _process_cli_query('Azure', cluster, query_cmd, '\t', status_map)
 
 
+def _query_status_ibm(
+    cluster: str,
+    ray_config: Dict[str, Any],
+) -> List[global_user_state.ClusterStatus]:
+    """
+    returns a list of Statuses for each of the cluster's nodes.
+    this function gets called when running `sky status` with -r flag and the cluster's head node is either stopped or down.
+    """
+
+    status_map: Dict[str, Any] = {
+        'pending': global_user_state.ClusterStatus.INIT,
+        'starting': global_user_state.ClusterStatus.INIT,
+        'restarting': global_user_state.ClusterStatus.INIT,
+        'running': global_user_state.ClusterStatus.UP,
+        'stopping': global_user_state.ClusterStatus.STOPPED,
+        'stopped': global_user_state.ClusterStatus.STOPPED,
+        'deleting': None,
+        'failed': global_user_state.ClusterStatus.INIT,
+        'cluster_deleted': []
+    }
+
+    client = ibm.client(region=ray_config['provider']['region'])
+    search_client = ibm.search_client()
+    # pylint: disable=E1136
+    vpcs_filtered_by_tags_and_region = search_client.search(
+        query=
+        f'type:vpc AND tags:{cluster} AND region:{ray_config["provider"]["region"]}',
+        fields=['tags', 'region', 'type'],
+        limit=1000).get_result()['items']
+    if not vpcs_filtered_by_tags_and_region:
+        # a vpc could have been removed unkownlingly to skypilot, such as
+        # via `sky autostop --down`, or simply manually (e.g. via console).
+        logger.warning('No vpc exists in '
+                       f'{ray_config["provider"]["region"]} '
+                       f'with tag: {cluster}')
+        return status_map['cluster_deleted']
+    vpc_id = vpcs_filtered_by_tags_and_region[0]['crn'].rsplit(':', 1)[-1]
+    instances = client.list_instances(vpc_id=vpc_id).get_result()['instances']
+
+    return [status_map[instance['status']] for instance in instances]
+
+
 def _query_status_lambda(
         cluster: str,
         ray_config: Dict[str, Any],  # pylint: disable=unused-argument
 ) -> List[global_user_state.ClusterStatus]:
     status_map = {
         'booting': global_user_state.ClusterStatus.INIT,
         'active': global_user_state.ClusterStatus.UP,
@@ -1694,23 +1815,26 @@
     }
     # TODO(ewzeng): filter by hash_filter_string to be safe
     status_list = []
     vms = lambda_utils.LambdaCloudClient().list_instances()
     possible_names = [f'{cluster}-head', f'{cluster}-worker']
     for node in vms:
         if node.get('name') in possible_names:
-            status_list.append(status_map[node['status']])
+            node_status = status_map[node['status']]
+            if node_status is not None:
+                status_list.append(node_status)
     return status_list
 
 
 _QUERY_STATUS_FUNCS = {
     'AWS': _query_status_aws,
     'GCP': _query_status_gcp,
     'Azure': _query_status_azure,
     'Lambda': _query_status_lambda,
+    'IBM': _query_status_ibm,
 }
 
 
 def check_owner_identity(cluster_name: str) -> None:
     """Check if current user is the same as the user who created the cluster.
 
     Raises:
@@ -1740,15 +1864,43 @@
     # NOTE: a user who upgrades SkyPilot and switches to a new cloud identity
     # immediately without `sky status --refresh` first, will cause a leakage
     # of the existing cluster. We deem this an acceptable tradeoff mainly
     # because multi-identity is not common (at least at the moment).
     if owner_identity is None:
         global_user_state.set_owner_identity_for_cluster(
             cluster_name, current_user_identity)
-    elif owner_identity != current_user_identity:
+    else:
+        assert isinstance(owner_identity, list)
+        # It is OK if the owner identity is shorter, which will happen when
+        # the cluster is launched before #1808. In that case, we only check
+        # the same length (zip will stop at the shorter one).
+        for i, (owner,
+                current) in enumerate(zip(owner_identity,
+                                          current_user_identity)):
+            if owner == current:
+                if i != 0:
+                    logger.warning(
+                        f'The cluster was owned by {owner_identity}, but '
+                        f'a new identity {current_user_identity} is activated. We still '
+                        'allow the operation as the two identities are likely to have '
+                        'the same access to the cluster. Please be aware that this can '
+                        'cause unexpected cluster leakage if the two identities are not '
+                        'actually equivalent (e.g., belong to the same person).'
+                    )
+                if i != 0 or len(owner_identity) != len(current_user_identity):
+                    # We update the owner of a cluster, when:
+                    # 1. The strictest identty (i.e. the first one) does not
+                    # match, but the latter ones match.
+                    # 2. The length of the two identities are different, which
+                    # will only happen when the cluster is launched before #1808.
+                    # Update the user identity to avoid showing the warning above
+                    # again.
+                    global_user_state.set_owner_identity_for_cluster(
+                        cluster_name, current_user_identity)
+                return  # The user identity matches.
         with ux_utils.print_exception_no_traceback():
             raise exceptions.ClusterOwnerIdentityMismatchError(
                 f'{cluster_name!r} ({cloud}) is owned by account '
                 f'{owner_identity!r}, but the activated account '
                 f'is {current_user_identity!r}.')
 
 
@@ -2105,43 +2257,55 @@
         # if the user is not the owner of the cluster.
         ux_utils.console_newline()
         logger.warning(
             f'Failed to refresh the status for cluster {cluster_name!r}. It is '
             f'not fatal, but {operation} might hang if the cluster is not up.\n'
             f'Detailed reason: {e}')
         record = global_user_state.get_cluster_from_name(cluster_name)
-        cluster_status, handle = record['status'], record['handle']
+        if record is None:
+            cluster_status, handle = None, None
+        else:
+            cluster_status, handle = record['status'], record['handle']
 
+    bright = colorama.Style.BRIGHT
+    reset = colorama.Style.RESET_ALL
     if handle is None:
         with ux_utils.print_exception_no_traceback():
             raise ValueError(
                 f'{colorama.Fore.YELLOW}Cluster {cluster_name!r} does not '
-                f'exist.{colorama.Style.RESET_ALL}')
+                f'exist.{reset}')
     backend = get_backend_from_handle(handle)
     if check_cloud_vm_ray_backend and not isinstance(
             backend, backends.CloudVmRayBackend):
         with ux_utils.print_exception_no_traceback():
             raise exceptions.NotSupportedError(
                 f'{colorama.Fore.YELLOW}{operation.capitalize()}: skipped for '
                 f'cluster {cluster_name!r}. It is only supported by backend: '
                 f'{backends.CloudVmRayBackend.NAME}.'
-                f'{colorama.Style.RESET_ALL}')
+                f'{reset}')
     if cluster_status != global_user_state.ClusterStatus.UP:
         if onprem_utils.check_if_local_cloud(cluster_name):
             raise exceptions.ClusterNotUpError(
                 constants.UNINITIALIZED_ONPREM_CLUSTER_MESSAGE.format(
                     cluster_name),
                 cluster_status=cluster_status)
         with ux_utils.print_exception_no_traceback():
+            hint_for_init = ''
+            if cluster_status == global_user_state.ClusterStatus.INIT:
+                hint_for_init = (
+                    f'{reset} Wait for a launch to finish, or use this command '
+                    f'to try to transition the cluster to UP: {bright}sky '
+                    f'start {cluster_name}{reset}')
             raise exceptions.ClusterNotUpError(
                 f'{colorama.Fore.YELLOW}{operation.capitalize()}: skipped for '
                 f'cluster {cluster_name!r} (status: {cluster_status.value}). '
                 'It is only allowed for '
                 f'{global_user_state.ClusterStatus.UP.value} clusters.'
-                f'{colorama.Style.RESET_ALL}',
+                f'{hint_for_init}'
+                f'{reset}',
                 cluster_status=cluster_status)
 
     if handle.head_ip is None:
         with ux_utils.print_exception_no_traceback():
             raise exceptions.ClusterNotUpError(
                 f'Cluster {cluster_name!r} has been stopped or not properly '
                 'set up. Please re-launch it with `sky start`.',
@@ -2158,15 +2322,15 @@
     LOCAL = 'local'
 
 
 def get_clusters(
     include_reserved: bool,
     refresh: bool,
     cloud_filter: CloudFilter = CloudFilter.CLOUDS_AND_DOCKER,
-    cluster_names: Optional[Union[str, Sequence[str]]] = None,
+    cluster_names: Optional[Union[str, List[str]]] = None,
 ) -> List[Dict[str, Any]]:
     """Returns a list of cached or optionally refreshed cluster records.
 
     Combs through the database (in ~/.sky/state.db) to get a list of records
     corresponding to launched clusters (filtered by `cluster_names` if it is
     specified). The refresh flag can be used to force a refresh of the status
     of the clusters.
@@ -2311,14 +2475,20 @@
 @typing.overload
 def get_backend_from_handle(
     handle: 'local_docker_backend.LocalDockerResourceHandle'
 ) -> 'local_docker_backend.LocalDockerBackend':
     ...
 
 
+@typing.overload
+def get_backend_from_handle(
+        handle: backends.ResourceHandle) -> backends.Backend:
+    ...
+
+
 def get_backend_from_handle(
         handle: backends.ResourceHandle) -> backends.Backend:
     """Gets a Backend object corresponding to a handle.
 
     Inspects handle type to infer the backend used for the resource.
     """
     backend: backends.Backend
@@ -2417,37 +2587,43 @@
                         field, known_fields, 1)
                     if most_similar_field:
                         err_msg += (f'\nInstead of {field!r}, did you mean '
                                     f'{most_similar_field[0]!r}?')
                     else:
                         err_msg += f'\nFound unsupported field {field!r}.'
         else:
-            err_msg = err_msg_prefix + e.message
+            # Example e.json_path value: '$.resources'
+            err_msg = (err_msg_prefix + e.message +
+                       f'. Check problematic field(s): {e.json_path}')
 
     if err_msg:
         with ux_utils.print_exception_no_traceback():
             raise ValueError(err_msg)
 
 
 def check_public_cloud_enabled():
-    """Checks if any of the public clouds is enabled."""
+    """Checks if any of the public clouds is enabled.
+
+    Exceptions:
+        exceptions.NoCloudAccessError: if no public cloud is enabled.
+    """
 
     def _no_public_cloud():
         enabled_clouds = global_user_state.get_enabled_clouds()
         return (len(enabled_clouds) == 0 or
                 (len(enabled_clouds) == 1 and
                  isinstance(enabled_clouds[0], clouds.Local)))
 
     if not _no_public_cloud():
         return
 
     sky_check.check(quiet=True)
     if _no_public_cloud():
         with ux_utils.print_exception_no_traceback():
-            raise RuntimeError(
+            raise exceptions.NoCloudAccessError(
                 'Cloud access is not set up. Run: '
                 f'{colorama.Style.BRIGHT}sky check{colorama.Style.RESET_ALL}')
 
 
 def run_command_and_handle_ssh_failure(runner: command_runner.SSHCommandRunner,
                                        command: str,
                                        failure_message: str) -> str:
```

### Comparing `skypilot-0.2.5/sky/backends/cloud_vm_ray_backend.py` & `skypilot-0.3.0/sky/backends/cloud_vm_ray_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,17 @@
 _PATH_SIZE_MEGABYTES_WARN_THRESHOLD = 256
 
 # Timeout (seconds) for provision progress: if in this duration no new nodes
 # are launched, abort and failover.
 _NODES_LAUNCHING_PROGRESS_TIMEOUT = {
     clouds.AWS: 90,
     clouds.Azure: 90,
-    clouds.GCP: 90,
-    clouds.Lambda: 120,
+    clouds.GCP: 120,
+    clouds.Lambda: 150,
+    clouds.IBM: 160,
     clouds.Local: 90,
 }
 
 # Time gap between retries after failing to provision in all possible places.
 # Used only if --retry-until-up is set.
 _RETRY_UNTIL_UP_INIT_GAP_SECONDS = 60
 
@@ -100,14 +101,17 @@
 _TPU_NOT_FOUND_ERROR = 'ERROR: (gcloud.compute.tpus.delete) NOT_FOUND'
 
 _CTRL_C_TIP_MESSAGE = ('INFO: Tip: use Ctrl-C to exit log streaming '
                        '(task will not be killed).')
 
 _MAX_RAY_UP_RETRY = 5
 
+# Number of retries for getting zones.
+_MAX_GET_ZONE_RETRY = 3
+
 _JOB_ID_PATTERN = re.compile(r'Job ID: ([0-9]+)')
 
 # Path to the monkey-patched ray up script.
 # We don't do import then __file__ because that script needs to be filled in
 # (so import would fail).
 _RAY_UP_WITH_MONKEY_PATCHED_HASH_LAUNCH_CONF_PATH = (
     pathlib.Path(sky.__file__).resolve().parent / 'backends' /
@@ -116,14 +120,15 @@
 
 def _get_cluster_config_template(cloud):
     cloud_to_template = {
         clouds.AWS: 'aws-ray.yml.j2',
         clouds.Azure: 'azure-ray.yml.j2',
         clouds.GCP: 'gcp-ray.yml.j2',
         clouds.Lambda: 'lambda-ray.yml.j2',
+        clouds.IBM: 'ibm-ray.yml.j2',
         clouds.Local: 'local-ray.yml.j2',
     }
     return cloud_to_template[type(cloud)]
 
 
 def write_ray_up_script_with_patched_launch_hash_fn(
     cluster_config_path: str,
@@ -194,16 +199,16 @@
                      setup_log_path: Optional[str] = None,
                      is_local: bool = False) -> None:
         assert not self._has_prologue, 'add_prologue() called twice?'
         self._has_prologue = True
         self.job_id = job_id
         # Should use 'auto' or 'ray://<internal_head_ip>:10001' rather than
         # 'ray://localhost:10001', or 'ray://127.0.0.1:10001', for public cloud.
-        # Otherwise, it will a bug of ray job failed to get the placement group
-        # in ray <= 2.0.1.
+        # Otherwise, ray will fail to get the placement group because of a bug
+        # in ray job.
         # TODO(mluo): Check why 'auto' not working with on-prem cluster and
         # whether the placement group issue also occurs in on-prem cluster.
         ray_address = 'ray://localhost:10001' if is_local else 'auto'
         self._code = [
             textwrap.dedent(f"""\
             import getpass
             import hashlib
@@ -224,15 +229,25 @@
             from sky.skylet import autostop_lib
             from sky.skylet import constants
             from sky.skylet import job_lib
             from sky.utils import log_utils
 
             SKY_REMOTE_WORKDIR = {constants.SKY_REMOTE_WORKDIR!r}
 
-            ray.init(address={ray_address!r}, namespace='__sky__{job_id}__', log_to_driver=True)
+            kwargs = dict()
+            # Only set the `_temp_dir` to SkyPilot's ray cluster directory when the directory
+            # exists for backward compatibility for the VM launched before #1790.
+            if os.path.exists({constants.SKY_REMOTE_RAY_TEMPDIR!r}):
+                kwargs['_temp_dir'] = {constants.SKY_REMOTE_RAY_TEMPDIR!r}
+            ray.init(
+                address={ray_address!r},
+                namespace='__sky__{job_id}__',
+                log_to_driver=True,
+                **kwargs
+            )
             run_fn = None
             futures = []
             """),
             # FIXME: This is a hack to make sure that the functions can be found
             # by ray.remote. This should be removed once we have a better way to
             # specify dependencies for ray.
             inspect.getsource(log_lib.process_subprocess_stream),
@@ -653,14 +668,23 @@
                         launchable_resources.copy(zone=zone.name))
                 elif code == 8:
                     # Error code 8 means TPU resources is out of
                     # capacity. Example:
                     # {'code': 8, 'message': 'There is no more capacity in the zone "europe-west4-a"; you can try in another zone where Cloud TPU Nodes are offered (see https://cloud.google.com/tpu/docs/regions) [EID: 0x1bc8f9d790be9142]'} # pylint: disable=line-too-long
                     self._blocked_resources.add(
                         launchable_resources.copy(zone=zone.name))
+                elif code == 'RESOURCE_NOT_FOUND':
+                    # https://github.com/skypilot-org/skypilot/issues/1797
+                    # In the inner provision loop we have used retries to
+                    # recover but failed. This indicates this zone is most
+                    # likely out of capacity. The provision loop will terminate
+                    # any potentially live VMs before moving onto the next
+                    # zone.
+                    self._blocked_resources.add(
+                        launchable_resources.copy(zone=zone.name))
                 else:
                     assert False, error
         elif len(httperror_str) >= 1:
             logger.info(f'Got {httperror_str[0]}')
             if ('Requested disk size cannot be smaller than the image size'
                     in httperror_str[0]):
                 logger.info('Skipping all regions due to disk size issue.')
@@ -829,14 +853,45 @@
         for e in errors:
             if e.find('Regions with capacity available:') != -1:
                 for r in clouds.Lambda.regions():
                     if e.find(r.name) == -1:
                         self._blocked_resources.add(
                             launchable_resources.copy(region=r.name, zone=None))
 
+    def _update_blocklist_on_ibm_error(
+            self, launchable_resources: 'resources_lib.Resources',
+            region: 'clouds.Region', zones: Optional[List['clouds.Zone']],
+            stdout: str, stderr: str):
+
+        style = colorama.Style
+        stdout_splits = stdout.split('\n')
+        stderr_splits = stderr.split('\n')
+        errors = [
+            s.strip()
+            for s in stdout_splits + stderr_splits
+            if 'ERR' in s.strip() or 'PANIC' in s.strip()
+        ]
+        if not errors:
+            logger.info('====== stdout ======')
+            for s in stdout_splits:
+                print(s)
+            logger.info('====== stderr ======')
+            for s in stderr_splits:
+                print(s)
+            with ux_utils.print_exception_no_traceback():
+                raise RuntimeError('Errors occurred during provision; '
+                                   'check logs above.')
+        logger.warning(f'Got error(s) on IBM cluster, in {region.name}:')
+        messages = '\n\t'.join(errors)
+        logger.warning(f'{style.DIM}\t{messages}{style.RESET_ALL}')
+
+        for zone in zones:  # type: ignore[union-attr]
+            self._blocked_resources.add(
+                launchable_resources.copy(zone=zone.name))
+
     def _update_blocklist_on_local_error(
             self, launchable_resources: 'resources_lib.Resources',
             region: 'clouds.Region', zones: Optional[List['clouds.Zone']],
             stdout: str, stderr: str):
         del zones  # Unused.
         style = colorama.Style
         stdout_splits = stdout.split('\n')
@@ -893,14 +948,15 @@
 
         # TODO(zongheng): refactor into Cloud interface?
         handlers = {
             clouds.AWS: self._update_blocklist_on_aws_error,
             clouds.Azure: self._update_blocklist_on_azure_error,
             clouds.GCP: self._update_blocklist_on_gcp_error,
             clouds.Lambda: self._update_blocklist_on_lambda_error,
+            clouds.IBM: self._update_blocklist_on_ibm_error,
             clouds.Local: self._update_blocklist_on_local_error,
         }
         cloud = launchable_resources.cloud
         cloud_type = type(cloud)
         if cloud_type not in handlers:
             raise NotImplementedError(
                 f'Cloud {cloud} unknown, or has not added '
@@ -962,16 +1018,17 @@
                     ] if to_provision.zone is not None else None
             if zones is None:
                 # Reuse the zone field in the ray yaml as the
                 # prev_resources.zone field may not be set before the previous
                 # cluster is launched.
                 handle = global_user_state.get_handle_from_cluster_name(
                     cluster_name)
-                assert handle is not None, (
-                    f'handle should not be None {cluster_name!r}')
+                assert isinstance(handle, CloudVmRayResourceHandle), (
+                    'handle should be CloudVmRayResourceHandle (found: '
+                    f'{type(handle)}) {cluster_name!r}')
                 config = common_utils.read_yaml(handle.cluster_yaml)
                 # This is for the case when the zone field is not set in the
                 # launched resources in a previous launch (e.g., ctrl-c during
                 # launch and multi-node cluster before PR #1700).
                 zones_str = config.get('provider', {}).get('availability_zone')
                 if zones_str is not None:
                     zones = [
@@ -1139,23 +1196,25 @@
         self,
         to_provision: resources_lib.Resources,
         num_nodes: int,
         requested_resources: Set[resources_lib.Resources],
         dryrun: bool,
         stream_logs: bool,
         cluster_name: str,
-        cloud_user_identity: Optional[str],
+        cloud_user_identity: Optional[List[str]],
         prev_cluster_status: Optional[global_user_state.ClusterStatus],
     ):
         """The provision retry loop."""
         style = colorama.Style
         fore = colorama.Fore
         # Get log_path name
         log_path = os.path.join(self.log_dir, 'provision.log')
         log_abs_path = os.path.abspath(log_path)
+        os.makedirs(self.log_dir, exist_ok=True)
+        os.system(f'touch {log_path}')
         tail_cmd = f'tail -n100 -f {log_path}'
         logger.info('To view detailed progress: '
                     f'{style.BRIGHT}{tail_cmd}{style.RESET_ALL}')
 
         # Get previous cluster status
         cluster_exists = prev_cluster_status is not None
         is_prev_cluster_healthy = prev_cluster_status in [
@@ -1433,15 +1492,15 @@
             # up' (sky launch) twice on a cluster with >1 node, the worker node
             # gets disconnected/killed by ray autoscaler; the whole task will
             # just freeze.  (Doesn't affect 1-node clusters.)  With this flag,
             # ray processes no longer restart and this bug doesn't show.
             # Downside is existing tasks on the cluster will keep running
             # (which may be ok with the semantics of 'sky launch' twice).
             # Tracked in https://github.com/ray-project/ray/issues/20402.
-            # Ref: https://github.com/ray-project/ray/blob/releases/2.2.0/python/ray/autoscaler/sdk/sdk.py#L16-L49  # pylint: disable=line-too-long
+            # Ref: https://github.com/ray-project/ray/blob/releases/2.4.0/python/ray/autoscaler/sdk/sdk.py#L16-L49  # pylint: disable=line-too-long
             script_path = write_ray_up_script_with_patched_launch_hash_fn(
                 cluster_config_file, ray_up_kwargs={'no_restart': True})
 
             # Redirect stdout/err to the file and streaming (if stream_logs).
             # With stdout/err redirected, 'ray up' will have no color and
             # different order from directly running in the console. The
             # `--log-style` and `--log-color` flags do not work. To reproduce,
@@ -1519,14 +1578,26 @@
             if isinstance(to_provision_cloud, clouds.GCP):
                 if ('Quota exceeded for quota metric \'List requests\' and '
                         'limit \'List requests per minute\'' in stderr):
                     logger.info(
                         'Retrying due to list request rate limit exceeded.')
                     return True
 
+                # https://github.com/skypilot-org/skypilot/issues/1797
+                # "The resource 'projects/xxx/zones/us-central1-b/instances/ray-yyy-head-<hash>-compute' was not found" # pylint: disable=line-too-long
+                pattern = (r'\'code\': \'RESOURCE_NOT_FOUND\'.*The resource'
+                           r'.*instances\/.*-compute\' was not found')
+                result = re.search(pattern, stderr)
+                if result is not None:
+                    # Retry. Unlikely will succeed if it's due to no capacity.
+                    logger.info(
+                        'Retrying due to the possibly flaky RESOURCE_NOT_FOUND '
+                        'error.')
+                    return True
+
             if ('Processing file mounts' in stdout and
                     'Running setup commands' not in stdout and
                     'Failed to setup head node.' in stderr):
                 logger.info(
                     'Retrying runtime setup due to ssh connection issue.')
                 return True
 
@@ -1656,15 +1727,15 @@
             return
         launched_resources = handle.launched_resources
         # Ray cluster should already be running if the system admin has setup
         # Ray.
         if isinstance(launched_resources.cloud, clouds.Local):
             raise RuntimeError(
                 'The command `ray status` errored out on the head node '
-                'of the local cluster. Check if ray[default]==2.0.1 '
+                'of the local cluster. Check if ray[default]==2.4.0 '
                 'is installed or running correctly.')
         backend.run_on_head(handle, 'ray stop', use_cached_head_ip=False)
 
         # Runs `ray up <kwargs>` with our monkey-patched launch hash
         # calculation. See the monkey patch file for why.
         script_path = write_ray_up_script_with_patched_launch_hash_fn(
             handle.cluster_yaml, ray_up_kwargs={'restart_only': True})
@@ -2257,15 +2328,15 @@
                         raise exceptions.ResourcesUnavailableError(
                             error_message,
                             failover_history=e.failover_history) from None
             if dryrun:
                 return None
             cluster_config_file = config_dict['ray']
 
-            handle = self.ResourceHandle(
+            handle = CloudVmRayResourceHandle(
                 cluster_name=cluster_name,
                 cluster_yaml=cluster_config_file,
                 launched_nodes=config_dict['launched_nodes'],
                 launched_resources=config_dict['launched_resources'],
                 # TPU.
                 tpu_create_script=config_dict.get('tpu-create-script'),
                 tpu_delete_script=config_dict.get('tpu-delete-script'))
@@ -2292,16 +2363,28 @@
                 if get_zone_cmd is not None:
                     ssh_credentials = backend_utils.ssh_credential_from_yaml(
                         handle.cluster_yaml)
                     runners = command_runner.SSHCommandRunner.make_runner_list(
                         ip_list, **ssh_credentials)
 
                     def _get_zone(runner):
-                        returncode, stdout, stderr = runner.run(
-                            get_zone_cmd, require_outputs=True)
+                        retry_count = 0
+                        backoff = common_utils.Backoff(initial_backoff=1,
+                                                       max_backoff_factor=3)
+                        while True:
+                            returncode, stdout, stderr = runner.run(
+                                get_zone_cmd,
+                                require_outputs=True,
+                                stream_logs=False)
+                            if returncode == 0:
+                                break
+                            retry_count += 1
+                            if retry_count <= _MAX_GET_ZONE_RETRY:
+                                time.sleep(backoff.current_backoff())
+                                continue
                         subprocess_utils.handle_returncode(
                             returncode,
                             get_zone_cmd,
                             f'Failed to get zone for {cluster_name!r}',
                             stderr=stderr,
                             stream_logs=stream_logs)
                         return stdout.strip()
@@ -2319,15 +2402,15 @@
             self._update_after_cluster_provisioned(handle, task,
                                                    prev_cluster_status, ip_list,
                                                    lock_path)
             return handle
 
     def _update_after_cluster_provisioned(
             self, handle: CloudVmRayResourceHandle, task: task_lib.Task,
-            prev_cluster_status: global_user_state.ClusterStatus,
+            prev_cluster_status: Optional[global_user_state.ClusterStatus],
             ip_list: List[str], lock_path: str) -> None:
         usage_lib.messages.usage.update_cluster_resources(
             handle.launched_nodes, handle.launched_resources)
         usage_lib.messages.usage.update_final_cluster_status(
             global_user_state.ClusterStatus.UP)
 
         # Update job queue to avoid stale jobs (when restarted), before
@@ -2427,14 +2510,16 @@
         num_nodes = handle.launched_nodes
         plural = 's' if num_nodes > 1 else ''
         logger.info(
             f'{fore.CYAN}Syncing workdir (to {num_nodes} node{plural}): '
             f'{style.BRIGHT}{workdir}{style.RESET_ALL}'
             f' -> '
             f'{style.BRIGHT}{SKY_REMOTE_WORKDIR}{style.RESET_ALL}')
+        os.makedirs(self.log_dir, exist_ok=True)
+        os.system(f'touch {log_path}')
         tail_cmd = f'tail -n100 -f {log_path}'
         logger.info('To view detailed progress: '
                     f'{style.BRIGHT}{tail_cmd}{style.RESET_ALL}')
         with log_utils.safe_rich_status('[bold cyan]Syncing[/]'):
             subprocess_utils.run_in_parallel(_sync_workdir_node, runners)
 
     def _sync_file_mounts(
@@ -2583,17 +2668,18 @@
             executable = onprem_utils.get_python_executable(handle.cluster_name)
             ray_command = (f'{cd} && {executable} -u {script_path} '
                            f'> {remote_log_path} 2>&1')
             job_submit_cmd = self._setup_and_create_job_cmd_on_local_head(
                 handle, ray_command, ray_job_id)
         else:
             job_submit_cmd = (
+                'RAY_DASHBOARD_PORT=$(python -c "from sky.skylet import job_lib; print(job_lib.get_job_submission_port())" 2> /dev/null || echo 8265);'  # pylint: disable=line-too-long
                 f'{cd} && mkdir -p {remote_log_dir} && ray job submit '
-                f'--address=http://127.0.0.1:8265 --submission-id {ray_job_id} '
-                '--no-wait '
+                '--address=http://127.0.0.1:$RAY_DASHBOARD_PORT '
+                f'--submission-id {ray_job_id} --no-wait '
                 f'"{executable} -u {script_path} > {remote_log_path} 2>&1"')
 
         returncode, stdout, stderr = self.run_on_head(handle,
                                                       job_submit_cmd,
                                                       stream_logs=False,
                                                       require_outputs=True)
         subprocess_utils.handle_returncode(returncode,
@@ -2673,20 +2759,22 @@
         runner.run(f'mkdir -p {remote_log_dir}; chmod a+rwx {remote_run_file}',
                    stream_logs=False)
         switch_user_cmd = job_lib.make_job_command_with_user_switching(
             ssh_user, remote_run_file)
         switch_user_cmd = ' '.join(switch_user_cmd)
         job_submit_cmd = (
             'ray job submit '
-            f'--address=http://127.0.0.1:8265 --submission-id {ray_job_id} '
+            '--address='
+            f'http://127.0.0.1:{constants.SKY_REMOTE_RAY_DASHBOARD_PORT} '
+            f'--submission-id {ray_job_id} '
             f'--no-wait -- {switch_user_cmd}')
         return job_submit_cmd
 
-    def _add_job(self, handle: CloudVmRayResourceHandle, job_name: str,
-                 resources_str: str) -> int:
+    def _add_job(self, handle: CloudVmRayResourceHandle,
+                 job_name: Optional[str], resources_str: str) -> int:
         username = getpass.getuser()
         code = job_lib.JobLibCodeGen.add_job(job_name, username,
                                              self.run_timestamp, resources_str)
         returncode, job_id_str, stderr = self.run_on_head(handle,
                                                           code,
                                                           stream_logs=False,
                                                           require_outputs=True,
@@ -2766,30 +2854,71 @@
                 if not storage.persistent:
                     storage.delete()
 
     def _teardown(self,
                   handle: CloudVmRayResourceHandle,
                   terminate: bool,
                   purge: bool = False):
+        """Tear down/ Stop the cluster.
+
+        Args:
+            handle: The handle to the cluster.
+            terminate: Terminate or stop the cluster.
+            purge: Purge the cluster record from the cluster table, even if
+                the teardown fails.
+        Raises:
+            exceptions.ClusterOwnerIdentityMismatchError: If the cluster is
+                owned by another user.
+            exceptions.CloudUserIdentityError: if we fail to get the current
+                user identity.
+            RuntimeError: If the cluster fails to be terminated/stopped.
+        """
         cluster_name = handle.cluster_name
         # Check if the cluster is owned by the current user. Raise
         # exceptions.ClusterOwnerIdentityMismatchError
-        backend_utils.check_owner_identity(cluster_name)
+        yellow = colorama.Fore.YELLOW
+        reset = colorama.Style.RESET_ALL
+        is_identity_mismatch_and_purge = False
+        try:
+            backend_utils.check_owner_identity(cluster_name)
+        except exceptions.ClusterOwnerIdentityMismatchError as e:
+            if purge:
+                logger.error(e)
+                verbed = 'terminated' if terminate else 'stopped'
+                logger.warning(
+                    f'{yellow}Purge (-p/--purge) is set, ignoring the '
+                    f'identity mismatch error and removing '
+                    f'the cluser record from cluster table.{reset}\n{yellow}It '
+                    'is the user\'s responsibility to ensure that this '
+                    f'cluster is actually {verbed} on the cloud.{reset}')
+                is_identity_mismatch_and_purge = True
+            else:
+                raise
+
         lock_path = os.path.expanduser(
             backend_utils.CLUSTER_STATUS_LOCK_PATH.format(cluster_name))
 
         try:
             # TODO(mraheja): remove pylint disabling when filelock
             # version updated
             # pylint: disable=abstract-class-instantiated
             with filelock.FileLock(
                     lock_path,
                     backend_utils.CLUSTER_STATUS_LOCK_TIMEOUT_SECONDS):
-                success = self.teardown_no_lock(handle, terminate, purge)
-            if success and terminate:
+                self.teardown_no_lock(
+                    handle,
+                    terminate,
+                    purge,
+                    # When --purge is set and we already see an ID mismatch
+                    # error, we skip the refresh codepath. This is because
+                    # refresh checks current user identity can throw
+                    # ClusterOwnerIdentityMismatchError. The argument/flag
+                    # `purge` should bypass such ID mismatch errors.
+                    refresh_cluster_status=not is_identity_mismatch_and_purge)
+            if terminate:
                 common_utils.remove_file_if_exists(lock_path)
         except filelock.Timeout as e:
             raise RuntimeError(
                 f'Cluster {cluster_name!r} is locked by {lock_path}. '
                 'Check to see if it is still being launched.') from e
 
     # --- CloudVMRayBackend Specific APIs ---
@@ -2968,22 +3097,25 @@
         )
 
     def teardown_no_lock(self,
                          handle: CloudVmRayResourceHandle,
                          terminate: bool,
                          purge: bool = False,
                          post_teardown_cleanup: bool = True,
-                         refresh_cluster_status: bool = True) -> bool:
+                         refresh_cluster_status: bool = True) -> None:
         """Teardown the cluster without acquiring the cluster status lock.
 
         NOTE: This method should not be called without holding the cluster
         status lock already.
 
         refresh_cluster_status is only used internally in the status refresh
         process, and should not be set to False in other cases.
+
+        Raises:
+            RuntimeError: If the cluster fails to be terminated/stopped.
         """
         if refresh_cluster_status:
             prev_cluster_status, _ = (
                 backend_utils.refresh_cluster_status_handle(
                     handle.cluster_name, acquire_per_cluster_status_lock=False))
         else:
             record = global_user_state.get_cluster_from_name(
@@ -2994,15 +3126,14 @@
             # When the cluster is not in the cluster table, we guarantee that
             # all related resources / cache / config are cleaned up, i.e. it
             # is safe to skip and return True.
             ux_utils.console_newline()
             logger.warning(
                 f'Cluster {handle.cluster_name!r} is already terminated. '
                 'Skipped.')
-            return True
         log_path = os.path.join(os.path.expanduser(self.log_dir),
                                 'teardown.log')
         log_abs_path = os.path.abspath(log_path)
         cloud = handle.launched_resources.cloud
         config = common_utils.read_yaml(handle.cluster_yaml)
         cluster_name = handle.cluster_name
         use_tpu_vm = config['provider'].get('_has_tpus', False)
@@ -3015,14 +3146,50 @@
                                             f'[green]{cluster_name}'):
                 returncode, stdout, stderr = log_lib.run_with_log(
                     terminate_cmd,
                     log_abs_path,
                     shell=True,
                     stream_logs=False,
                     require_outputs=True)
+
+        elif (isinstance(cloud, clouds.IBM) and terminate and
+              prev_cluster_status == global_user_state.ClusterStatus.STOPPED):
+            # pylint: disable= W0622 W0703 C0415
+            from sky.adaptors import ibm
+            from sky.skylet.providers.ibm.vpc_provider import IBMVPCProvider
+
+            config_provider = common_utils.read_yaml(
+                handle.cluster_yaml)['provider']
+            region = config_provider['region']
+            cluster_name = handle.cluster_name
+            search_client = ibm.search_client()
+            vpc_found = False
+            # pylint: disable=unsubscriptable-object
+            vpcs_filtered_by_tags_and_region = search_client.search(
+                query=f'type:vpc AND tags:{cluster_name} AND region:{region}',
+                fields=['tags', 'region', 'type'],
+                limit=1000).get_result()['items']
+            try:
+                # pylint: disable=line-too-long
+                vpc_id = vpcs_filtered_by_tags_and_region[0]['crn'].rsplit(
+                    ':', 1)[-1]
+                vpc_found = True
+            except Exception:
+                logger.critical('failed to locate vpc for ibm cloud')
+                returncode = -1
+
+            if vpc_found:
+                # # pylint: disable=line-too-long E1136
+                # Delete VPC and it's associated resources
+                vpc_provider = IBMVPCProvider(
+                    config_provider['resource_group_id'], region, cluster_name)
+                vpc_provider.delete_vpc(vpc_id, region)
+                # successfully removed cluster as no exception was raised
+                returncode = 0
+
         elif (terminate and
               (prev_cluster_status == global_user_state.ClusterStatus.STOPPED or
                use_tpu_vm)):
             # For TPU VMs, gcloud CLI is used for VM termination.
             if isinstance(cloud, clouds.AWS):
                 # TODO(zhwu): Room for optimization. We can move these cloud
                 # specific handling to the cloud class.
@@ -3106,41 +3273,41 @@
             # '(ResourceGroupNotFound)': this indicates the resource group on
             #   Azure is not found. That means the cluster is already deleted
             #   on the cloud. So it's safe & good UX to not print a failure
             #   message.
             elif ('TPU must be specified.' not in stderr and
                   'SKYPILOT_ERROR_NO_NODES_LAUNCHED: ' not in stderr and
                   '(ResourceGroupNotFound)' not in stderr):
-                logger.error(
+                raise RuntimeError(
                     _TEARDOWN_FAILURE_MESSAGE.format(
                         extra_reason='',
                         cluster_name=handle.cluster_name,
                         stdout=stdout,
                         stderr=stderr))
-                return False
 
         # No need to clean up if the cluster is already terminated
         # (i.e., prev_status is None), as the cleanup has already been done
         # if the cluster is removed from the status table.
         if post_teardown_cleanup:
-            return self.post_teardown_cleanup(handle, terminate, purge)
-        else:
-            return True
+            self.post_teardown_cleanup(handle, terminate, purge)
 
     def post_teardown_cleanup(self,
                               handle: CloudVmRayResourceHandle,
                               terminate: bool,
-                              purge: bool = False) -> bool:
+                              purge: bool = False) -> None:
         """Cleanup local configs/caches and delete TPUs after teardown.
 
         This method will handle the following cleanup steps:
         * Deleting the TPUs;
         * Removing ssh configs for the cluster;
         * Updating the local state of the cluster;
         * Removing the terminated cluster's scripts and ray yaml files.
+
+        Raises:
+            RuntimeError: If it fails to delete the TPU.
         """
         log_path = os.path.join(os.path.expanduser(self.log_dir),
                                 'teardown.log')
         log_abs_path = os.path.abspath(log_path)
 
         if (handle.tpu_delete_script is not None and
                 os.path.exists(handle.tpu_delete_script)):
@@ -3155,21 +3322,20 @@
                     logger.info('TPU not found. '
                                 'It should have been deleted already.')
                 elif purge:
                     logger.warning(
                         _TEARDOWN_PURGE_WARNING.format(
                             reason='stopping/terminating TPU'))
                 else:
-                    logger.error(
+                    raise RuntimeError(
                         _TEARDOWN_FAILURE_MESSAGE.format(
                             extra_reason='It is caused by TPU failure.',
                             cluster_name=handle.cluster_name,
                             stdout=tpu_stdout,
                             stderr=tpu_stderr))
-                    return False
 
         # The cluster file must exist because the cluster_yaml will only
         # be removed after the cluster entry in the database is removed.
         config = common_utils.read_yaml(handle.cluster_yaml)
         auth_config = config['auth']
         backend_utils.SSHConfigHelper.remove_cluster(handle.cluster_name,
                                                      handle.head_ip,
@@ -3185,15 +3351,14 @@
                 common_utils.remove_file_if_exists(handle.tpu_create_script)
                 common_utils.remove_file_if_exists(handle.tpu_delete_script)
 
             # Clean up generated config
             # No try-except is needed since Ray will fail to teardown the
             # cluster if the cluster_yaml is missing.
             common_utils.remove_file_if_exists(handle.cluster_yaml)
-        return True
 
     def set_autostop(self,
                      handle: CloudVmRayResourceHandle,
                      idle_minutes_to_autostop: Optional[int],
                      down: bool = False,
                      stream_logs: bool = True) -> None:
         if idle_minutes_to_autostop is not None:
@@ -3395,14 +3560,16 @@
                         '.gitignore to exclude large files, as large sizes '
                         f'will slow down rsync. {style.RESET_ALL}')
                 if os.path.islink(full_src):
                     logger.warning(
                         f'{fore.YELLOW}Source path {src!r} is a symlink. '
                         f'Symlink contents are not uploaded.{style.RESET_ALL}')
 
+        os.makedirs(self.log_dir, exist_ok=True)
+        os.system(f'touch {log_path}')
         tail_cmd = f'tail -n100 -f {log_path}'
         logger.info('To view detailed progress: '
                     f'{style.BRIGHT}{tail_cmd}{style.RESET_ALL}')
 
         for dst, src in file_mounts.items():
             # TODO: room for improvement.  Here there are many moving parts
             # (download gsutil on remote, run gsutil on remote).  Consider
@@ -3532,23 +3699,36 @@
             # Get the first store and use it to mount
             store = list(storage_obj.stores.values())[0]
             mount_cmd = store.mount_command(dst)
             src_print = (storage_obj.source
                          if storage_obj.source else storage_obj.name)
             if isinstance(src_print, list):
                 src_print = ', '.join(src_print)
-            backend_utils.parallel_data_transfer_to_nodes(
-                runners,
-                source=src_print,
-                target=dst,
-                cmd=mount_cmd,
-                run_rsync=False,
-                action_message='Mounting',
-                log_path=log_path,
-            )
+            try:
+                backend_utils.parallel_data_transfer_to_nodes(
+                    runners,
+                    source=src_print,
+                    target=dst,
+                    cmd=mount_cmd,
+                    run_rsync=False,
+                    action_message='Mounting',
+                    log_path=log_path,
+                )
+            except exceptions.CommandError as e:
+                if e.returncode == exceptions.MOUNT_PATH_NON_EMPTY_CODE:
+                    mount_path = (f'{colorama.Fore.RED}'
+                                  f'{colorama.Style.BRIGHT}{dst}'
+                                  f'{colorama.Style.RESET_ALL}')
+                    error_msg = (f'Mount path {mount_path} is non-empty.'
+                                 f' {mount_path} may be a standard unix '
+                                 f'path or may contain files from a previous'
+                                 f' task. To fix, change the mount path'
+                                 f' to an empty or non-existent path.')
+                    raise RuntimeError(error_msg) from None
+
         end = time.time()
         logger.debug(f'Storage mount sync took {end - start} seconds.')
 
     def _execute_task_one_node(self, handle: CloudVmRayResourceHandle,
                                task: task_lib.Task, job_id: int,
                                detach_run: bool) -> None:
         # Launch the command as a Ray task.
```

### Comparing `skypilot-0.2.5/sky/backends/docker_utils.py` & `skypilot-0.3.0/sky/backends/docker_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 SKY_DOCKER_SETUP_SCRIPT = 'sky_setup.sh'
 SKY_DOCKER_RUN_SCRIPT = 'sky_run.sh'
 SKY_DOCKER_WORKDIR = 'sky_workdir'
 
 
 def create_dockerfile(
     base_image: str,
-    setup_command: str,
+    setup_command: Optional[str],
     copy_path: str,
     build_dir: str,
     run_command: Optional[str] = None,
 ) -> Tuple[str, Dict[str, str]]:
     """Writes a valid dockerfile to the specified path.
 
     performs three operations:
@@ -154,14 +154,17 @@
     2. Copy dockerfile to this directory and copy contents
     3. Run the dockerbuild
     """
     # Get tempdir
     temp_dir = tempfile.mkdtemp(prefix='sky_local_')
 
     # Create dockerfile
+    if callable(task.run):
+        raise ValueError(
+            'Cannot build docker image for a task.run with function.')
     _, img_metadata = create_dockerfile(base_image=task.docker_image,
                                         setup_command=task.setup,
                                         copy_path=f'{SKY_DOCKER_WORKDIR}/',
                                         run_command=task.run,
                                         build_dir=temp_dir)
 
     dst = os.path.join(temp_dir, SKY_DOCKER_WORKDIR)
@@ -182,14 +185,15 @@
 
     return tag, img_metadata
 
 
 def build_dockerimage_from_task(
         task: task_mod.Task) -> Tuple[str, Dict[str, str]]:
     """ Builds a docker image from a Task"""
+    assert task.name is not None, task
     tag, img_metadata = build_dockerimage(task, tag=task.name)
     return tag, img_metadata
 
 
 def push_dockerimage(local_tag, remote_name):
     raise NotImplementedError('Pushing images is not yet implemented.')
```

### Comparing `skypilot-0.2.5/sky/backends/local_docker_backend.py` & `skypilot-0.3.0/sky/backends/local_docker_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
                detach_setup: bool) -> None:
         """Launches a container and runs a sleep command on it.
 
         setup() in LocalDockerBackend runs the container with a sleep job
         so that the container is kept alive and we can issue docker exec cmds
         to it to handle sky exec commands.
         """
-        del task, detach_setup  # unused
+        del detach_setup  # unused
         style = colorama.Style
         assert handle in self.images, \
             f'No image found for {handle}, have you run Backend.provision()?'
         image_tag, metadata = self.images[handle]
         volumes = self.volume_mounts[handle]
         runtime = 'nvidia' if self._use_gpu else None
         logger.info(f'Image {image_tag} found. Running container now. use_gpu '
@@ -354,14 +354,18 @@
                     # Remove 'skymeta_' from key
                     metadata[k[len(_DOCKER_LABEL_PREFIX):]] = v
             self.images[c.name] = [c.image, metadata]
             self.containers[c.name] = c
 
     def _execute_task_one_node(self, handle: LocalDockerResourceHandle,
                                task: 'task_lib.Task') -> None:
+        if callable(task.run):
+            raise NotImplementedError(
+                'Tasks with callable run commands are not supported in '
+                'LocalDockerBackend.')
         container = self.containers[handle]
         _, image_metadata = self.images[handle]
         with tempfile.NamedTemporaryFile(mode='w') as temp_file:
             script_contents = docker_utils.bash_codegen(
                 workdir_name=image_metadata['workdir_name'],
                 multiline_cmds=task.run)
             temp_file.write(script_contents)
```

### Comparing `skypilot-0.2.5/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-0.3.0/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import hashlib
 import json
 import os
 
 from ray.autoscaler import sdk
 
 
-# Ref: https://github.com/ray-project/ray/blob/releases/2.2.0/python/ray/autoscaler/_private/util.py#L392-L404
+# Ref: https://github.com/ray-project/ray/blob/releases/2.4.0/python/ray/autoscaler/_private/util.py#L396-L408
 def monkey_patch_hash_launch_conf(node_conf, auth):
     hasher = hashlib.sha1()
     # For hashing, we replace the path to the key with the key
     # itself. This is to make sure the hashes are the same even if keys
     # live at different locations on different machines.
     full_auth = auth.copy()
     full_auth.pop('ssh_proxy_command', None)  # NOTE: skypilot changes.
@@ -46,15 +46,15 @@
             with open(os.path.expanduser(auth[key_type])) as key:
                 full_auth[key_type] = key.read()
     hasher.update(
         json.dumps([node_conf, full_auth], sort_keys=True).encode('utf-8'))
     return hasher.hexdigest()
 
 
-# Ref: https://github.com/ray-project/ray/blob/840215bc09e942b50cad0ab2db96a8fdc79217c1/python/ray/autoscaler/_private/commands.py#L854-L912
+# Ref: https://github.com/ray-project/ray/blob/releases/2.4.0/python/ray/autoscaler/_private/commands.py#L854-L912
 def monkey_patch_should_create_new_head(
     head_node_id,
     new_launch_hash,
     new_head_node_type,
     provider,
 ) -> bool:
     if not head_node_id:
```

### Comparing `skypilot-0.2.5/sky/backends/onprem_utils.py` & `skypilot-0.3.0/sky/backends/onprem_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,17 +367,19 @@
 
         subprocess_utils.run_in_parallel(_stop_ray_workers,
                                          [head_runner] + worker_runners)
 
     # Launching Ray on the head node.
     head_resources = json.dumps(custom_resources[0], separators=(',', ':'))
     head_gpu_count = sum(list(custom_resources[0].values()))
-    head_cmd = ('ray start --head --port=6379 '
-                '--object-manager-port=8076 --dashboard-port 8265 '
-                f'--resources={head_resources!r} --num-gpus={head_gpu_count}')
+    head_cmd = (f'ray start --head --port={constants.SKY_REMOTE_RAY_PORT} '
+                '--object-manager-port=8076 '
+                f'--dashboard-port {constants.SKY_REMOTE_RAY_DASHBOARD_PORT} '
+                f'--resources={head_resources!r} --num-gpus={head_gpu_count} '
+                f'--temp-dir {constants.SKY_REMOTE_RAY_TEMPDIR}')
 
     with console.status('[bold cyan]Launching ray cluster on head'):
         backend_utils.run_command_and_handle_ssh_failure(
             head_runner,
             head_cmd,
             failure_message='Failed to launch ray on head node.')
 
@@ -394,15 +396,17 @@
     # Connect head node's Ray dashboard to worker nodes
     # Worker nodes need access to Ray dashboard to poll the
     # JobSubmissionClient (in subprocess_daemon.py) for completed,
     # failed, or cancelled jobs.
     ssh_options = command_runner.ssh_options_list(
         ssh_private_key=remote_ssh_key, ssh_control_name=None)
     ssh_options = ' '.join(ssh_options)
-    port_cmd = (f'ssh -tt -L 8265:localhost:8265 '
+    ray_dashboard_port = constants.SKY_REMOTE_RAY_DASHBOARD_PORT
+    port_cmd = ('ssh -tt -L '
+                f'{ray_dashboard_port}:localhost:{ray_dashboard_port} '
                 f'{ssh_options} {ssh_user}@{head_ip} '
                 '\'while true; do sleep 86400; done\'')
     with console.status('[bold cyan]Waiting for workers.'):
 
         def _start_ray_workers(
                 runner_tuple: Tuple[command_runner.SSHCommandRunner, int]):
             runner, idx = runner_tuple
@@ -410,18 +414,22 @@
                 runner,
                 'ray stop -f',
                 failure_message=f'Failed to stop ray on {runner.ip}.')
 
             worker_resources = json.dumps(custom_resources[idx + 1],
                                           separators=(',', ':'))
             worker_gpu_count = sum(list(custom_resources[idx + 1].values()))
-            worker_cmd = (f'ray start --address={head_ip}:6379 '
-                          '--object-manager-port=8076 --dashboard-port 8265 '
-                          f'--resources={worker_resources!r} '
-                          f'--num-gpus={worker_gpu_count}')
+            worker_cmd = (
+                'ray start '
+                f'--address={head_ip}:{constants.SKY_REMOTE_RAY_PORT} '
+                '--object-manager-port=8076 --dashboard-port '
+                f'{constants.SKY_REMOTE_RAY_DASHBOARD_PORT} '
+                f'--resources={worker_resources!r} '
+                f'--num-gpus={worker_gpu_count} '
+                f'--temp-dir {constants.SKY_REMOTE_RAY_TEMPDIR}')
             backend_utils.run_command_and_handle_ssh_failure(
                 runner,
                 worker_cmd,
                 failure_message=
                 f'Failed to launch ray on worker node {runner.ip}.')
 
             # Connecting ray dashboard with worker node.
```

### Comparing `skypilot-0.2.5/sky/backends/wheel_utils.py` & `skypilot-0.3.0/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/benchmark/benchmark_state.py` & `skypilot-0.3.0/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/benchmark/benchmark_utils.py` & `skypilot-0.3.0/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/check.py` & `skypilot-0.3.0/sky/check.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Credential checks: check cloud credentials and enable clouds."""
 from typing import Dict
 
 import click
 
 from sky import clouds
 from sky import global_user_state
+from sky.adaptors import cloudflare
 
 
 def check(quiet: bool = False) -> None:
     echo = (lambda *_args, **_kwargs: None) if quiet else click.echo
     echo('Checking credentials to enable clouds for SkyPilot.')
 
     enabled_clouds = []
@@ -26,15 +27,31 @@
         if ok:
             enabled_clouds.append(str(cloud))
             if reason is not None:
                 echo(f'    Hint: {reason}')
         else:
             echo(f'    Reason: {reason}')
 
-    if len(enabled_clouds) == 0:
+    # Currently, clouds.CLOUD_REGISTRY.values() does not
+    # support r2 as only clouds with computing instances
+    # are added as 'cloud'. This will be removed when
+    # cloudflare/r2 is added as a 'cloud'.
+    cloud = 'Cloudflare (for R2 object store)'
+    echo(f'  Checking {cloud}...', nl=False)
+    r2_is_enabled, reason = cloudflare.check_credentials()
+    echo('\r', nl=False)
+    status_msg = 'enabled' if r2_is_enabled else 'disabled'
+    status_color = 'green' if r2_is_enabled else 'red'
+    echo('  ' +
+         click.style(f'{cloud}: {status_msg}', fg=status_color, bold=True) +
+         ' ' * 10)
+    if not r2_is_enabled:
+        echo(f'    Reason: {reason}')
+
+    if len(enabled_clouds) == 0 and not r2_is_enabled:
         click.echo(
             click.style(
                 'No cloud is enabled. SkyPilot will not be able to run any '
                 'task. Run `sky check` for more info.',
                 fg='red',
                 bold=True))
         raise SystemExit()
@@ -57,8 +74,16 @@
     and a list of patterns that will be excluded (used as rsync_exclude).
     """
     enabled_clouds = global_user_state.get_enabled_clouds()
     file_mounts = {}
     for cloud in enabled_clouds:
         cloud_file_mounts = cloud.get_credential_file_mounts()
         file_mounts.update(cloud_file_mounts)
+    # Currently, get_enabled_clouds() does not support r2
+    # as only clouds with computing instances are marked
+    # as enabled by skypilot. This will be removed when
+    # cloudflare/r2 is added as a 'cloud'.
+    r2_is_enabled, _ = cloudflare.check_credentials()
+    if r2_is_enabled:
+        r2_credential_mounts = cloudflare.get_credential_file_mounts()
+        file_mounts.update(r2_credential_mounts)
     return file_mounts
```

### Comparing `skypilot-0.2.5/sky/cli.py` & `skypilot-0.3.0/sky/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import multiprocessing
 import os
 import shlex
 import subprocess
 import sys
 import textwrap
 import typing
-from typing import Any, Dict, List, Optional, Sequence, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 import click
 import colorama
 from rich import progress as rich_progress
 import yaml
 
 import sky
@@ -100,15 +100,15 @@
 }
 
 # The maximum number of in-progress spot jobs to show in the status
 # command.
 _NUM_SPOT_JOBS_TO_SHOW_IN_STATUS = 5
 
 
-def _get_glob_clusters(clusters: Sequence[str]) -> List[str]:
+def _get_glob_clusters(clusters: List[str]) -> List[str]:
     """Returns a list of clusters that match the glob pattern."""
     glob_clusters = []
     for cluster in clusters:
         glob_cluster = global_user_state.get_glob_cluster_names(cluster)
         if len(glob_cluster) == 0:
             if onprem_utils.check_if_local_cloud(cluster):
                 click.echo(
@@ -116,15 +116,15 @@
                         cluster=cluster))
             else:
                 click.echo(f'Cluster {cluster} not found.')
         glob_clusters.extend(glob_cluster)
     return list(set(glob_clusters))
 
 
-def _get_glob_storages(storages: Sequence[str]) -> List[str]:
+def _get_glob_storages(storages: List[str]) -> List[str]:
     """Returns a list of storages that match the glob pattern."""
     glob_storages = []
     for storage_object in storages:
         glob_storage = global_user_state.get_glob_storage_name(storage_object)
         if len(glob_storage) == 0:
             click.echo(f'Storage {storage_object} not found.')
         else:
@@ -217,14 +217,20 @@
                                 help='If true, use TPU VMs.')
 
     disk_size = click.option('--disk-size',
                              default=None,
                              type=int,
                              required=False,
                              help=('OS disk size in GBs.'))
+    disk_tier = click.option('--disk-tier',
+                             default=None,
+                             type=str,
+                             required=False,
+                             help=('OS disk tier. Could be one of "low", '
+                                   '"medium", "high". Default: medium'))
     no_confirm = click.option('--yes',
                               '-y',
                               is_flag=True,
                               default=False,
                               required=False,
                               help='Skip confirmation prompt.')
     idle_autostop = click.option('--idle-minutes-to-autostop',
@@ -295,14 +301,15 @@
         spot_option,
         *([tpuvm_option] if cli_func.__name__ == 'tpunode' else []),
 
         # Attach options
         screen_option,
         tmux_option,
         disk_size,
+        disk_tier,
     ]
     decorator = functools.reduce(lambda res, f: f(res),
                                  reversed(click_decorators), cli_func)
 
     return decorator
 
 
@@ -584,15 +591,16 @@
                            zone: Optional[str] = None,
                            gpus: Optional[str] = None,
                            cpus: Optional[str] = None,
                            memory: Optional[str] = None,
                            instance_type: Optional[str] = None,
                            use_spot: Optional[bool] = None,
                            image_id: Optional[str] = None,
-                           disk_size: Optional[int] = None) -> Dict[str, Any]:
+                           disk_size: Optional[int] = None,
+                           disk_tier: Optional[str] = None) -> Dict[str, Any]:
     """Parses the override parameters into a dictionary."""
     override_params: Dict[str, Any] = {}
     if cloud is not None:
         if cloud.lower() == 'none':
             override_params['cloud'] = None
         else:
             override_params['cloud'] = clouds.CLOUD_REGISTRY.from_str(cloud)
@@ -631,14 +639,16 @@
     if image_id is not None:
         if image_id.lower() == 'none':
             override_params['image_id'] = None
         else:
             override_params['image_id'] = image_id
     if disk_size is not None:
         override_params['disk_size'] = disk_size
+    if disk_tier is not None:
+        override_params['disk_tier'] = disk_tier
     return override_params
 
 
 def _default_interactive_node_name(node_type: str):
     """Returns a deterministic name to refer to the same node."""
     # FIXME: this technically can collide in Azure/GCP with another
     # same-username user.  E.g., sky-gpunode-ubuntu.  Not a problem on AWS
@@ -677,14 +687,17 @@
         node_type: Only used for interactive node. Node type to attach to VM.
     """
     handle = global_user_state.get_handle_from_cluster_name(cluster_name)
     if handle is None:
         return
 
     if node_type is not None:
+        assert isinstance(handle,
+                          backends.CloudVmRayResourceHandle), (node_type,
+                                                               handle)
         inferred_node_type = _infer_interactive_node_type(
             handle.launched_resources)
         if node_type != inferred_node_type:
             name_arg = ''
             if cluster_name != _default_interactive_node_name(
                     inferred_node_type):
                 name_arg = f' -c {cluster_name}'
@@ -717,15 +730,15 @@
     if cluster is None:
         cluster = backend_utils.generate_cluster_name()
     maybe_status, _ = backend_utils.refresh_cluster_status_handle(cluster)
     if maybe_status is None:
         # Show the optimize log before the prompt if the cluster does not exist.
         try:
             backend_utils.check_public_cloud_enabled()
-        except RuntimeError as e:
+        except exceptions.NoCloudAccessError as e:
             # Catch the exception where the public cloud is not enabled, and
             # only print the error message without the error type.
             click.secho(e, fg='yellow')
             sys.exit(1)
         dag = sky.optimize(dag)
     task = dag.tasks[0]
 
@@ -872,14 +885,15 @@
         no_confirm=no_confirm,
         idle_minutes_to_autostop=idle_minutes_to_autostop,
         down=down,
         retry_until_up=retry_until_up,
         node_type=node_type,
     )
     handle = global_user_state.get_handle_from_cluster_name(cluster_name)
+    assert isinstance(handle, backends.CloudVmRayResourceHandle), handle
 
     # Use ssh rather than 'ray attach' to suppress ray messages, speed up
     # connection, and for allowing adding 'cd workdir' in the future.
     # Disable check, since the returncode could be non-zero if the user Ctrl-D.
     commands = []
     if session_manager == 'screen':
         commands += ['screen', '-D', '-R']
@@ -966,14 +980,15 @@
     cpus: Optional[str] = None,
     memory: Optional[str] = None,
     instance_type: Optional[str] = None,
     num_nodes: Optional[int] = None,
     use_spot: Optional[bool] = None,
     image_id: Optional[str] = None,
     disk_size: Optional[int] = None,
+    disk_tier: Optional[str] = None,
     env: Optional[List[Tuple[str, str]]] = None,
     # spot launch specific
     spot_recovery: Optional[str] = None,
 ) -> sky.Task:
     entrypoint = ' '.join(entrypoint)
     is_yaml, yaml_config = _check_yaml(entrypoint)
     entrypoint: Optional[str]
@@ -985,38 +1000,40 @@
         if not entrypoint:
             entrypoint = None
         else:
             # Treat entrypoint as a bash command.
             click.secho('Task from command: ', fg='yellow', nl=False)
             click.secho(entrypoint, bold=True)
 
-    if onprem_utils.check_local_cloud_args(cloud, cluster, yaml_config):
-        cloud = 'local'
-
     if is_yaml:
+        assert entrypoint is not None
         usage_lib.messages.usage.update_user_task_yaml(entrypoint)
         task = sky.Task.from_yaml(entrypoint)
     else:
         task = sky.Task(name='sky-cmd', run=entrypoint)
         task.set_resources({sky.Resources()})
 
     # Override.
     if workdir is not None:
         task.workdir = workdir
 
+    if onprem_utils.check_local_cloud_args(cloud, cluster, yaml_config):
+        cloud = 'local'
+
     override_params = _parse_override_params(cloud=cloud,
                                              region=region,
                                              zone=zone,
                                              gpus=gpus,
                                              cpus=cpus,
                                              memory=memory,
                                              instance_type=instance_type,
                                              use_spot=use_spot,
                                              image_id=image_id,
-                                             disk_size=disk_size)
+                                             disk_size=disk_size,
+                                             disk_tier=disk_tier)
     # Spot launch specific.
     if spot_recovery is not None:
         if spot_recovery.lower() == 'none':
             override_params['spot_recovery'] = None
         else:
             override_params['spot_recovery'] = spot_recovery
 
@@ -1026,15 +1043,15 @@
 
     task.set_resources({new_resources})
 
     if num_nodes is not None:
         task.num_nodes = num_nodes
     if name is not None:
         task.name = name
-    task.set_envs(env)
+    task.update_envs(env)
     # TODO(wei-lin): move this validation into Python API.
     if new_resources.accelerators is not None:
         acc, _ = list(new_resources.accelerators.items())[0]
         if acc.startswith('tpu-') and task.num_nodes > 1:
             raise ValueError('Multi-node TPU cluster is not supported. '
                              f'Got num_nodes={task.num_nodes}.')
     return task
@@ -1166,14 +1183,22 @@
           '``--memory=16`` (exactly 16GB), ``--memory=16+`` (at least 16GB))'))
 @click.option('--disk-size',
               default=None,
               type=int,
               required=False,
               help=('OS disk size in GBs.'))
 @click.option(
+    '--disk-tier',
+    default=None,
+    type=str,
+    required=False,
+    help=(
+        'OS disk tier. Could be one of "low", "medium", "high". Default: medium'
+    ))
+@click.option(
     '--idle-minutes-to-autostop',
     '-i',
     default=None,
     type=int,
     required=False,
     help=('Automatically stop the cluster after this many minutes '
           'of idleness, i.e., no running or pending jobs in the cluster\'s job '
@@ -1232,14 +1257,15 @@
     memory: Optional[str],
     instance_type: Optional[str],
     num_nodes: Optional[int],
     use_spot: Optional[bool],
     image_id: Optional[str],
     env: List[Tuple[str, str]],
     disk_size: Optional[int],
+    disk_tier: Optional[str],
     idle_minutes_to_autostop: Optional[int],
     down: bool,  # pylint: disable=redefined-outer-name
     retry_until_up: bool,
     yes: bool,
     no_setup: bool,
 ):
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
@@ -1278,14 +1304,15 @@
         memory=memory,
         instance_type=instance_type,
         num_nodes=num_nodes,
         use_spot=use_spot,
         image_id=image_id,
         env=env,
         disk_size=disk_size,
+        disk_tier=disk_tier,
     )
 
     backend: backends.Backend
     if backend_name == backends.LocalDockerBackend.NAME:
         backend = backends.LocalDockerBackend()
     elif backend_name == backends.CloudVmRayBackend.NAME:
         backend = backends.CloudVmRayBackend()
@@ -1434,34 +1461,39 @@
     sky.exec(task, backend=backend, cluster_name=cluster, detach_run=detach_run)
 
 
 def _get_spot_jobs(
         refresh: bool,
         skip_finished: bool,
         show_all: bool,
-        limit_num_jobs_to_show: bool = False) -> Tuple[Optional[int], str]:
+        limit_num_jobs_to_show: bool = False,
+        is_called_by_user: bool = False) -> Tuple[Optional[int], str]:
     """Get the in-progress spot jobs.
 
     Args:
         refresh: Query the latest statuses, restarting the spot controller if
             stopped.
         skip_finished: Show only in-progress jobs.
         show_all: Show all information of each spot job (e.g., region, price).
         limit_num_jobs_to_show: If True, limit the number of jobs to show to
             _NUM_SPOT_JOBS_TO_SHOW_IN_STATUS, which is mainly used by
             `sky status`.
+        is_called_by_user: If this function is called by user directly, or an
+            internal call.
 
     Returns:
         A tuple of (num_in_progress_jobs, msg). If num_in_progress_jobs is None,
         it means there is an error when querying the spot jobs. In this case,
         msg contains the error message. Otherwise, msg contains the formatted
         spot job table.
     """
     num_in_progress_jobs = None
     try:
+        if not is_called_by_user:
+            usage_lib.messages.usage.set_internal()
         with sky_logging.silent():
             # Make the call silent
             spot_jobs = core.spot_queue(refresh=refresh,
                                         skip_finished=skip_finished)
         num_in_progress_jobs = len(spot_jobs)
     except exceptions.ClusterNotUpError as e:
         controller_status = e.cluster_status
@@ -1575,15 +1607,16 @@
         if show_spot_jobs:
             # Run the spot job query in parallel to speed up the status query.
             spot_jobs_future = pool.apply_async(
                 _get_spot_jobs,
                 kwds=dict(refresh=False,
                           skip_finished=True,
                           show_all=False,
-                          limit_num_jobs_to_show=not all))
+                          limit_num_jobs_to_show=not all,
+                          is_called_by_user=False))
         click.echo(f'{colorama.Fore.CYAN}{colorama.Style.BRIGHT}Clusters'
                    f'{colorama.Style.RESET_ALL}')
         query_clusters: Optional[List[str]] = None
         if clusters:
             query_clusters = _get_glob_clusters(clusters)
         cluster_records = core.status(cluster_names=query_clusters,
                                       refresh=refresh)
@@ -1667,47 +1700,69 @@
               default=False,
               is_flag=True,
               required=False,
               help='Show all information in full.')
 @usage_lib.entrypoint
 def cost_report(all: bool):  # pylint: disable=redefined-builtin
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
-    """Show cost reports for each cluster.
+    """Show estimated costs for launched clusters.
 
-    The following fields for each cluster are recorded: cluster name,
-    resources, launched time, duration that cluster was up,
-    and total cost.
+    For each cluster, this shows: cluster name, resources, launched time,
+    duration that cluster was up, and total estimated cost.
 
     The estimated cost column indicates the price for the cluster based on the
-    type of resources being used and the duration of use up until the call
-    to status. This means if the cluster is UP, successive calls to report
-    will show increasing price. The estimated cost is calculated based on
-    the local cache of the cluster status, and may not be accurate for
-    the cluster with autostop/use_spot set or terminated/stopped
-    on the cloud console.
+    type of resources being used and the duration of use up until now. This
+    means if the cluster is UP, successive calls to cost-report will show
+    increasing price.
+
+    This CLI is experimental. The estimated cost is calculated based on the
+    local cache of the cluster status, and may not be accurate for:
+
+    - Clusters with autostop/use_spot set; or
+
+    - Clusters that were terminated/stopped on the cloud console.
     """
     cluster_records = core.cost_report()
+
     nonreserved_cluster_records = []
     reserved_clusters = dict()
     for cluster_record in cluster_records:
         cluster_name = cluster_record['name']
         if cluster_name in backend_utils.SKY_RESERVED_CLUSTER_NAMES:
             cluster_group_name = backend_utils.SKY_RESERVED_CLUSTER_NAMES[
                 cluster_name]
-            reserved_clusters[cluster_group_name] = cluster_record
+            # to display most recent entry for each reserved cluster
+            # TODO(sgurram): fix assumption of sorted order of clusters
+            if cluster_group_name not in reserved_clusters:
+                reserved_clusters[cluster_group_name] = cluster_record
         else:
             nonreserved_cluster_records.append(cluster_record)
 
-    status_utils.show_cost_report_table(nonreserved_cluster_records, all)
+    total_cost = status_utils.get_total_cost_of_displayed_records(
+        nonreserved_cluster_records, all)
 
+    status_utils.show_cost_report_table(nonreserved_cluster_records, all)
     for cluster_group_name, cluster_record in reserved_clusters.items():
         status_utils.show_cost_report_table(
             [cluster_record], all, reserved_group_name=cluster_group_name)
+        total_cost += cluster_record['total_cost']
+
+    click.echo(f'\n{colorama.Style.BRIGHT}'
+               f'Total Cost: ${total_cost:.2f}{colorama.Style.RESET_ALL}')
+
+    if not all:
+        click.secho(
+            f'Showing up to {status_utils.NUM_COST_REPORT_LINES} '
+            'most recent clusters. '
+            'To see all clusters in history, '
+            'pass the --all flag.',
+            fg='yellow')
+
     click.secho(
-        'NOTE: This feature is experimental. '
+        'This feature is experimental. '
         'Costs for clusters with auto{stop,down} '
         'scheduled may not be accurate.',
         fg='yellow')
 
 
 @cli.command()
 @click.option('--all-users',
@@ -1724,15 +1779,15 @@
               help='Show only pending/running jobs\' information.')
 @click.argument('clusters',
                 required=False,
                 type=str,
                 nargs=-1,
                 **_get_shell_complete_args(_complete_cluster_name))
 @usage_lib.entrypoint
-def queue(clusters: Sequence[str], skip_finished: bool, all_users: bool):
+def queue(clusters: List[str], skip_finished: bool, all_users: bool):
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
     """Show the job queue for cluster(s)."""
     click.secho('Fetching and parsing job queue...', fg='yellow')
     show_local_clusters = False
     if clusters:
         clusters = _get_glob_clusters(clusters)
     else:
@@ -1774,28 +1829,29 @@
 
 @cli.command()
 @click.option(
     '--sync-down',
     '-s',
     is_flag=True,
     default=False,
-    help='Sync down the logs of the job (this is useful for distributed jobs to'
-    'download a separate log for each job from all the workers).')
+    help='Sync down the logs of a job to the local machine. For a distributed'
+    ' job, a separate log file from each worker will be downloaded.')
 @click.option(
     '--status',
     is_flag=True,
     default=False,
     help=('If specified, do not show logs but exit with a status code for the '
           'job\'s status: 0 for succeeded, or 1 for all other statuses.'))
 @click.option(
     '--follow/--no-follow',
     is_flag=True,
     default=True,
-    help=('Follow the logs of the job. [default: --follow] '
-          'If --no-follow is specified, print the log so far and exit.'))
+    help=('Follow the logs of a job. '
+          'If --no-follow is specified, print the log so far and exit. '
+          '[default: --follow]'))
 @click.argument('cluster',
                 required=True,
                 type=str,
                 **_get_shell_complete_args(_complete_cluster_name))
 @click.argument('job_ids', type=str, nargs=-1)
 # TODO(zhwu): support logs by job name
 @usage_lib.entrypoint
@@ -1809,20 +1865,22 @@
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
     """Tail the log of a job.
 
     If JOB_ID is not provided, the latest job on the cluster will be used.
 
     1. If no flags are provided, tail the logs of the job_id specified. At most
     one job_id can be provided.
-    2. If --status is specified, print the status of the job and exit with
-    returncode 0 if the job is succeeded, or 1 otherwise. At most one job_id can
+
+    2. If ``--status`` is specified, print the status of the job and exit with
+    returncode 0 if the job succeeded, or 1 otherwise. At most one job_id can
     be specified.
-    3. If --sync-down is specified, the logs of the job will be downloaded from
-    the cluster and saved to the local machine under `~/sky_logs`. Mulitple
-    job_ids can be specified.
+
+    3. If ``--sync-down`` is specified, the logs of the job will be downloaded
+    from the cluster and saved to the local machine under
+    ``~/sky_logs``. Mulitple job_ids can be specified.
     """
     if sync_down and status:
         raise click.UsageError(
             'Both --sync_down and --status are specified '
             '(ambiguous). To fix: specify at most one of them.')
 
     if len(job_ids) > 1 and not sync_down:
@@ -1942,15 +2000,15 @@
               '-y',
               is_flag=True,
               default=False,
               required=False,
               help='Skip confirmation prompt.')
 @usage_lib.entrypoint
 def stop(
-    clusters: Tuple[str],
+    clusters: List[str],
     all: Optional[bool],  # pylint: disable=redefined-builtin
     yes: bool,
 ):
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
     """Stop cluster(s).
 
     CLUSTER is the name (or glob pattern) of the cluster to stop.  If both
@@ -2020,15 +2078,15 @@
               '-y',
               is_flag=True,
               default=False,
               required=False,
               help='Skip confirmation prompt.')
 @usage_lib.entrypoint
 def autostop(
-    clusters: Tuple[str],
+    clusters: List[str],
     all: Optional[bool],  # pylint: disable=redefined-builtin
     idle_minutes: Optional[int],
     cancel: bool,  # pylint: disable=redefined-outer-name
     down: bool,  # pylint: disable=redefined-outer-name
     yes: bool,
 ):
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
@@ -2143,15 +2201,15 @@
     is_flag=True,
     required=False,
     help=('Force start the cluster even if it is already UP. Useful for '
           'upgrading the SkyPilot runtime on the cluster.'))
 @usage_lib.entrypoint
 # pylint: disable=redefined-builtin
 def start(
-        clusters: Sequence[str],
+        clusters: List[str],
         all: bool,
         yes: bool,
         idle_minutes_to_autostop: Optional[int],
         down: bool,  # pylint: disable=redefined-outer-name
         retry_until_up: bool,
         force: bool):
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
@@ -2332,15 +2390,15 @@
               is_flag=True,
               default=False,
               required=False,
               help='Ignore cloud provider errors (if any). '
               'Useful for cleaning up manually deleted cluster(s).')
 @usage_lib.entrypoint
 def down(
-    clusters: Tuple[str],
+    clusters: List[str],
     all: Optional[bool],  # pylint: disable=redefined-builtin
     yes: bool,
     purge: bool,
 ):
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
     """Tear down cluster(s).
 
@@ -2387,15 +2445,17 @@
         click.echo('Managed spot controller has already been torn down.')
         return
 
     if cluster_status == global_user_state.ClusterStatus.INIT:
         with ux_utils.print_exception_no_traceback():
             raise exceptions.NotSupportedError(
                 f'{colorama.Fore.RED}Tearing down the spot controller while '
-                'it is in INIT state is not supported, as we cannot '
+                'it is in INIT state is not supported (this means a spot '
+                'launch is in progress or the previous launch failed), as we '
+                'cannot '
                 'guarantee that all the spot jobs are finished. Please wait '
                 'until the spot controller is UP or fix it with '
                 f'{colorama.Style.BRIGHT}sky start '
                 f'{spot_lib.SPOT_CONTROLLER_NAME}{colorama.Style.RESET_ALL}.')
     msg = (f'{colorama.Fore.YELLOW}WARNING: Tearing down the managed '
            f'spot controller ({cluster_status.value}). Please be '
            f'aware of the following:{colorama.Style.RESET_ALL}'
@@ -2435,15 +2495,15 @@
                 raise exceptions.NotSupportedError(msg)
         else:
             click.echo(' * No in-progress spot jobs found. It should be safe '
                        'to terminate (see caveats above).')
 
 
 def _down_or_stop_clusters(
-        names: Sequence[str],
+        names: List[str],
         apply_to_all: Optional[bool],
         down: bool,  # pylint: disable=redefined-outer-name
         no_confirm: bool,
         purge: bool = False,
         idle_minutes_to_autostop: Optional[int] = None) -> None:
     """Tears down or (auto-)stops a cluster (or all clusters).
 
@@ -2600,15 +2660,15 @@
                     core.down(name, purge=purge)
                 else:
                     core.stop(name, purge=purge)
             except RuntimeError as e:
                 message = (
                     f'{colorama.Fore.RED}{operation} cluster {name}...failed. '
                     f'{colorama.Style.RESET_ALL}'
-                    f'\n\tReason: {common_utils.format_exception(e)}.')
+                    f'\nReason: {common_utils.format_exception(e)}.')
             except (exceptions.NotSupportedError,
                     exceptions.ClusterOwnerIdentityMismatchError) as e:
                 message = str(e)
             else:  # no exception raised
                 message = (
                     f'{colorama.Fore.GREEN}{operation} cluster {name}...done.'
                     f'{colorama.Style.RESET_ALL}')
@@ -2636,16 +2696,16 @@
 # pylint: disable=redefined-outer-name
 def gpunode(cluster: str, yes: bool, port_forward: Optional[List[int]],
             cloud: Optional[str], region: Optional[str], zone: Optional[str],
             instance_type: Optional[str], cpus: Optional[str],
             memory: Optional[str], gpus: Optional[str],
             use_spot: Optional[bool], screen: Optional[bool],
             tmux: Optional[bool], disk_size: Optional[int],
-            idle_minutes_to_autostop: Optional[int], down: bool,
-            retry_until_up: bool):
+            disk_tier: Optional[str], idle_minutes_to_autostop: Optional[int],
+            down: bool, retry_until_up: bool):
     """Launch or attach to an interactive GPU node.
 
     Examples:
 
     .. code-block:: bash
 
         # Launch a default gpunode.
@@ -2694,15 +2754,16 @@
                               region=region,
                               zone=zone,
                               instance_type=instance_type,
                               cpus=cpus,
                               memory=memory,
                               accelerators=gpus,
                               use_spot=use_spot,
-                              disk_size=disk_size)
+                              disk_size=disk_size,
+                              disk_tier=disk_tier)
 
     _create_and_ssh_into_node(
         'gpunode',
         resources,
         cluster_name=name,
         port_forward=port_forward,
         session_manager=session_manager,
@@ -2718,16 +2779,17 @@
 @usage_lib.entrypoint
 # pylint: disable=redefined-outer-name
 def cpunode(cluster: str, yes: bool, port_forward: Optional[List[int]],
             cloud: Optional[str], region: Optional[str], zone: Optional[str],
             instance_type: Optional[str], cpus: Optional[str],
             memory: Optional[str], use_spot: Optional[bool],
             screen: Optional[bool], tmux: Optional[bool],
-            disk_size: Optional[int], idle_minutes_to_autostop: Optional[int],
-            down: bool, retry_until_up: bool):
+            disk_size: Optional[int], disk_tier: Optional[str],
+            idle_minutes_to_autostop: Optional[int], down: bool,
+            retry_until_up: bool):
     """Launch or attach to an interactive CPU node.
 
     Examples:
 
     .. code-block:: bash
 
         # Launch a default cpunode.
@@ -2772,15 +2834,16 @@
     resources = sky.Resources(cloud=cloud_provider,
                               region=region,
                               zone=zone,
                               instance_type=instance_type,
                               cpus=cpus,
                               memory=memory,
                               use_spot=use_spot,
-                              disk_size=disk_size)
+                              disk_size=disk_size,
+                              disk_tier=disk_tier)
 
     _create_and_ssh_into_node(
         'cpunode',
         resources,
         cluster_name=name,
         port_forward=port_forward,
         session_manager=session_manager,
@@ -2797,16 +2860,17 @@
 # pylint: disable=redefined-outer-name
 def tpunode(cluster: str, yes: bool, port_forward: Optional[List[int]],
             region: Optional[str], zone: Optional[str],
             instance_type: Optional[str], cpus: Optional[str],
             memory: Optional[str], tpus: Optional[str],
             use_spot: Optional[bool], tpu_vm: Optional[bool],
             screen: Optional[bool], tmux: Optional[bool],
-            disk_size: Optional[int], idle_minutes_to_autostop: Optional[int],
-            down: bool, retry_until_up: bool):
+            disk_size: Optional[int], disk_tier: Optional[str],
+            idle_minutes_to_autostop: Optional[int], down: bool,
+            retry_until_up: bool):
     """Launch or attach to an interactive TPU node.
 
     Examples:
 
     .. code-block:: bash
 
         # Launch a default tpunode.
@@ -2858,15 +2922,16 @@
                               zone=zone,
                               instance_type=instance_type,
                               cpus=cpus,
                               memory=memory,
                               accelerators=tpus,
                               accelerator_args=accelerator_args,
                               use_spot=use_spot,
-                              disk_size=disk_size)
+                              disk_size=disk_size,
+                              disk_tier=disk_tier)
 
     _create_and_ssh_into_node(
         'tpunode',
         resources,
         cluster_name=name,
         port_forward=port_forward,
         session_manager=session_manager,
@@ -2877,25 +2942,28 @@
         retry_until_up=retry_until_up,
     )
 
 
 @cli.command()
 @usage_lib.entrypoint
 def check():
-    """Determine the set of clouds available to use.
+    """Check which clouds are available to use.
+
+    This checks access credentials for all clouds supported by SkyPilot. If a
+    cloud is detected to be inaccessible, the reason and correction steps will
+    be shown.
 
-    This checks access credentials for AWS, Azure and GCP; on failure, it shows
-    the reason and suggests correction steps. Tasks will only run on clouds
-    that you have access to.
+    The enabled clouds are cached and form the "search space" to be considered
+    for each task.
     """
     sky_check.check()
 
 
 @cli.command()
-@click.argument('gpu_name', required=False)
+@click.argument('accelerator_str', required=False)
 @click.option('--all',
               '-a',
               is_flag=True,
               default=False,
               help='Show details of all GPU/TPU/accelerator offerings.')
 @click.option('--cloud',
               default=None,
@@ -2908,61 +2976,73 @@
     help=
     ('The region to use. If not specified, shows accelerators from all regions.'
     ),
 )
 @service_catalog.use_default_catalog
 @usage_lib.entrypoint
 def show_gpus(
-        gpu_name: Optional[str],
+        accelerator_str: Optional[str],
         all: bool,  # pylint: disable=redefined-builtin
         cloud: Optional[str],
         region: Optional[str]):
-    """Show supported GPU/TPU/accelerators.
+    """Show supported GPU/TPU/accelerators and their prices.
 
     The names and counts shown can be set in the ``accelerators`` field in task
     YAMLs, or in the ``--gpus`` flag in CLI commands. For example, if this
     table shows 8x V100s are supported, then the string ``V100:8`` will be
     accepted by the above.
 
-    To show the detailed information of a GPU/TPU type (which clouds offer it,
-    the quantity in each VM type, etc.), use ``sky show-gpus <gpu>``.
+    To show the detailed information of a GPU/TPU type (its price, which clouds
+    offer it, the quantity in each VM type, etc.), use ``sky show-gpus <gpu>``.
 
     To show all accelerators, including less common ones and their detailed
     information, use ``sky show-gpus --all``.
 
-    NOTE: If region is not specified, the price displayed for each instance type
-    is the lowest across all regions for both on-demand and spot instances.
+    Definitions of certain fields:
+
+    * ``DEVICE_MEM``: Memory of a single device; does not depend on the device
+      count of the instance (VM).
+
+    * ``HOST_MEM``: Memory of the host instance (VM).
+
+    If ``--region`` is not specified, the price displayed for each instance
+    type is the lowest across all regions for both on-demand and spot
+    instances. There may be multiple regions with the same lowest price.
     """
     # validation for the --region flag
     if region is not None and cloud is None:
         raise click.UsageError(
             'The --region flag is only valid when the --cloud flag is set.')
+    # This will validate 'cloud' and raise if not found.
+    clouds.CLOUD_REGISTRY.from_str(cloud)
     service_catalog.validate_region_zone(region, None, clouds=cloud)
     show_all = all
-    if show_all and gpu_name is not None:
+    if show_all and accelerator_str is not None:
         raise click.UsageError('--all is only allowed without a GPU name.')
 
     def _list_to_str(lst):
         return ', '.join([str(e) for e in lst])
 
     def _output():
         gpu_table = log_utils.create_table(
-            ['NVIDIA_GPU', 'AVAILABLE_QUANTITIES'])
+            ['COMMON_GPU', 'AVAILABLE_QUANTITIES'])
         tpu_table = log_utils.create_table(
             ['GOOGLE_TPU', 'AVAILABLE_QUANTITIES'])
         other_table = log_utils.create_table(
             ['OTHER_GPU', 'AVAILABLE_QUANTITIES'])
 
-        if gpu_name is None:
+        name, quantity = None, None
+
+        if accelerator_str is None:
             result = service_catalog.list_accelerator_counts(
                 gpus_only=True,
                 clouds=cloud,
                 region_filter=region,
             )
-            # NVIDIA GPUs
+            # "Common" GPUs
             for gpu in service_catalog.get_common_gpus():
                 if gpu in result:
                     gpu_table.add_row([gpu, _list_to_str(result.pop(gpu))])
             yield from gpu_table.get_string()
 
             # Google TPUs
             for tpu in service_catalog.get_tpus():
@@ -2976,71 +3056,102 @@
             if show_all:
                 yield '\n\n'
                 for gpu, qty in sorted(result.items()):
                     other_table.add_row([gpu, _list_to_str(qty)])
                 yield from other_table.get_string()
                 yield '\n\n'
             else:
+                yield ('\n\nHint: use -a/--all to see all accelerators '
+                       '(including non-common ones) and pricing.')
                 return
+        else:
+            # Parse accelerator string
+            accelerator_split = accelerator_str.split(':')
+            if len(accelerator_split) > 2:
+                raise click.UsageError(
+                    f'Invalid accelerator string {accelerator_str}. '
+                    'Expected format: <accelerator_name>[:<quantity>].')
+            if len(accelerator_split) == 2:
+                name = accelerator_split[0]
+                # Check if quantity is valid
+                try:
+                    quantity = int(accelerator_split[1])
+                    if quantity <= 0:
+                        raise ValueError(
+                            'Quantity cannot be non-positive integer.')
+                except ValueError as invalid_quantity:
+                    raise click.UsageError(
+                        f'Invalid accelerator quantity {accelerator_split[1]}. '
+                        'Expected a positive integer.') from invalid_quantity
+            else:
+                name, quantity = accelerator_str, None
 
-        # Show detailed accelerator information
         result = service_catalog.list_accelerators(gpus_only=True,
-                                                   name_filter=gpu_name,
+                                                   name_filter=name,
+                                                   quantity_filter=quantity,
                                                    region_filter=region,
                                                    clouds=cloud)
         if len(result) == 0:
-            yield f'Resources \'{gpu_name}\' not found. '
+            quantity_str = (f' with requested quantity {quantity}'
+                            if quantity else '')
+            yield f'Resources \'{name}\'{quantity_str} not found. '
             yield 'Try \'sky show-gpus --all\' '
             yield 'to show available accelerators.'
             return
 
-        yield '*NOTE*: for most GCP accelerators, '
-        yield 'INSTANCE_TYPE == (attachable) means '
-        yield 'the host VM\'s cost is not included.\n\n'
+        if cloud is None or cloud.lower() == 'gcp':
+            yield '*NOTE*: for most GCP accelerators, '
+            yield 'INSTANCE_TYPE == (attachable) means '
+            yield 'the host VM\'s cost is not included.\n\n'
+
         import pandas as pd  # pylint: disable=import-outside-toplevel
         for i, (gpu, items) in enumerate(result.items()):
             accelerator_table_headers = [
                 'GPU',
                 'QTY',
                 'CLOUD',
                 'INSTANCE_TYPE',
+                'DEVICE_MEM',
                 'vCPUs',
-                'HOST_MEMORY',
+                'HOST_MEM',
                 'HOURLY_PRICE',
                 'HOURLY_SPOT_PRICE',
             ]
             if not show_all:
                 accelerator_table_headers.append('REGION')
             accelerator_table = log_utils.create_table(
                 accelerator_table_headers)
             for item in items:
                 instance_type_str = item.instance_type if not pd.isna(
                     item.instance_type) else '(attachable)'
                 cpu_count = item.cpu_count
                 if pd.isna(cpu_count):
                     cpu_str = '-'
-                elif isinstance(cpu_count, float):
-                    if cpu_count.is_integer():
+                elif isinstance(cpu_count, (float, int)):
+                    if int(cpu_count) == cpu_count:
                         cpu_str = str(int(cpu_count))
                     else:
                         cpu_str = f'{cpu_count:.1f}'
-                mem_str = f'{item.memory:.0f}GB' if not pd.isna(
+                device_memory_str = (f'{item.device_memory:.0f}GB' if
+                                     not pd.isna(item.device_memory) else '-')
+                host_memory_str = f'{item.memory:.0f}GB' if not pd.isna(
                     item.memory) else '-'
                 price_str = f'$ {item.price:.3f}' if not pd.isna(
                     item.price) else '-'
                 spot_price_str = f'$ {item.spot_price:.3f}' if not pd.isna(
                     item.spot_price) else '-'
                 region_str = item.region if not pd.isna(item.region) else '-'
                 accelerator_table_vals = [
                     item.accelerator_name,
                     item.accelerator_count,
                     item.cloud,
                     instance_type_str,
+                    device_memory_str,
                     cpu_str,
-                    mem_str,
+                    host_memory_str,
                     price_str,
                     spot_price_str,
                 ]
                 if not show_all:
                     accelerator_table_vals.append(region_str)
                 accelerator_table.add_row(accelerator_table_vals)
 
@@ -3054,15 +3165,15 @@
         for out in _output():
             click.echo(out, nl=False)
         click.echo()
 
 
 @cli.group(cls=_NaturalOrderGroup)
 def storage():
-    """Storage related commands."""
+    """SkyPilot Storage CLI."""
     pass
 
 
 @storage.command('ls', cls=_DocumentedCodeCommand)
 @usage_lib.entrypoint
 def storage_ls():
     """List storage objects created."""
@@ -3080,15 +3191,15 @@
 @click.option('--all',
               '-a',
               default=False,
               is_flag=True,
               required=False,
               help='Delete all storage objects.')
 @usage_lib.entrypoint
-def storage_delete(names: Sequence[str], all: bool):  # pylint: disable=redefined-builtin
+def storage_delete(names: List[str], all: bool):  # pylint: disable=redefined-builtin
     """Delete storage objects.
 
     Examples:
 
     .. code-block:: bash
 
         # Delete two storage objects.
@@ -3111,15 +3222,15 @@
 
     for name in names:
         sky.storage_delete(name)
 
 
 @cli.group(cls=_NaturalOrderGroup)
 def admin():
-    """Sky administrator commands for local clusters."""
+    """SkyPilot On-prem administrator CLI."""
     pass
 
 
 @admin.command('deploy', cls=_DocumentedCodeCommand)
 @click.argument('clusterspec_yaml', required=True, type=str, nargs=-1)
 @usage_lib.entrypoint
 def admin_deploy(clusterspec_yaml: str):
@@ -3187,15 +3298,15 @@
     click.secho(f'Saved in {sanitized_yaml_path} \n', fg='yellow', nl=False)
     click.secho(f'Successfully deployed local cluster {local_cluster_name!r}\n',
                 fg='green')
 
 
 @cli.group(cls=_NaturalOrderGroup)
 def spot():
-    """Commands for managed spot jobs."""
+    """Managed Spot commands (spot instances with auto-recovery)."""
     pass
 
 
 @spot.command('launch', cls=_DocumentedCodeCommand)
 @click.argument('entrypoint',
                 required=True,
                 type=str,
@@ -3223,30 +3334,39 @@
               help='Spot recovery strategy to use for the managed spot task.')
 @click.option('--disk-size',
               default=None,
               type=int,
               required=False,
               help=('OS disk size in GBs.'))
 @click.option(
+    '--disk-tier',
+    default=None,
+    type=str,
+    required=False,
+    help=(
+        'OS disk tier. Could be one of "low", "medium", "high". Default: medium'
+    ))
+@click.option(
     '--detach-run',
     '-d',
     default=False,
     is_flag=True,
     help=('If True, as soon as a job is submitted, return from this call '
           'and do not stream execution logs.'))
 @click.option(
     '--retry-until-up',
     '-r',
-    default=False,
+    default=True,
     is_flag=True,
     required=False,
-    help=('Whether to retry provisioning infinitely until the cluster is up, '
-          'if we fail to launch the cluster on any possible region/cloud due '
-          'to unavailability errors. This applies to launching the the spot '
-          'clusters (both initial and recovery attempts).'))
+    help=('(Default: True; this flag is deprecated and will be removed in a '
+          'future release.) Whether to retry provisioning infinitely until the '
+          'cluster is up, if unavailability errors are encountered. This '
+          'applies to launching the spot clusters (both the initial and any '
+          'recovery attempts), not the spot controller.'))
 @click.option('--yes',
               '-y',
               is_flag=True,
               default=False,
               required=False,
               help='Skip confirmation prompt.')
 @timeline.event
@@ -3264,14 +3384,15 @@
     instance_type: Optional[str],
     num_nodes: Optional[int],
     use_spot: Optional[bool],
     image_id: Optional[str],
     spot_recovery: Optional[str],
     env: List[Tuple[str, str]],
     disk_size: Optional[int],
+    disk_tier: Optional[str],
     detach_run: bool,
     retry_until_up: bool,
     yes: bool,
 ):
     """Launch a managed spot job from a YAML or a command.
 
     If ENTRYPOINT points to a valid YAML file, it is read in as the task
@@ -3301,14 +3422,15 @@
         memory=memory,
         instance_type=instance_type,
         num_nodes=num_nodes,
         use_spot=use_spot,
         image_id=image_id,
         env=env,
         disk_size=disk_size,
+        disk_tier=disk_tier,
         spot_recovery=spot_recovery,
     )
 
     if not yes:
         prompt = f'Launching a new spot task {name!r}. Proceed?'
         if prompt is not None:
             click.confirm(prompt, default=True, abort=True, show_default=True)
@@ -3318,14 +3440,22 @@
     # against the regex, and the cloud-specific validation will be done by
     # the spot controller when actually launching the spot cluster.
     resources = list(task.resources)[0]
     task_cloud = (resources.cloud
                   if resources.cloud is not None else clouds.Cloud)
     task_cloud.check_cluster_name_is_valid(name)
 
+    # Deprecation.
+    if not retry_until_up:
+        click.secho(
+            'Flag --retry-until-up is deprecated and will be removed in a '
+            'future release (defaults to True). Please file an issue if this '
+            'does not work for you.',
+            fg='yellow')
+
     sky.spot_launch(task,
                     name,
                     detach_run=detach_run,
                     retry_until_up=retry_until_up)
 
 
 @spot.command('queue', cls=_DocumentedCodeCommand)
@@ -3350,46 +3480,71 @@
               required=False,
               help='Show only pending/running jobs\' information.')
 @usage_lib.entrypoint
 # pylint: disable=redefined-builtin
 def spot_queue(all: bool, refresh: bool, skip_finished: bool):
     """Show statuses of managed spot jobs.
 
-    \b
     Each spot job can have one of the following statuses:
 
-    \b
-    - SUBMITTED: The job is submitted to the spot controller.
-    - STARTING: The job is starting (starting a spot cluster).
-    - RUNNING: The job is running.
-    - RECOVERING: The spot cluster is recovering from a preemption.
-    - SUCCEEDED: The job succeeded.
-    - FAILED: The job failed due to an error from the job itself.
-    - FAILED_NO_RESOURCES: The job failed due to resources being unavailable
-        after a maximum number of retry attempts.
-    - FAILED_CONTROLLER: The job failed due to an unexpected error in the spot
-        controller.
-    - CANCELLING: The job was requested to be cancelled by the user, and the
-        cancellation is in progress.
-    - CANCELLED: The job was cancelled by the user.
+    - ``PENDING``: Job is waiting for a free slot on the spot controller to be
+      accepted.
+
+    - ``SUBMITTED``: Job is submitted to and accepted by the spot controller.
+
+    - ``STARTING``: Job is starting (provisioning a spot cluster).
+
+    - ``RUNNING``: Job is running.
+
+    - ``RECOVERING``: The spot cluster is recovering from a preemption.
+
+    - ``SUCCEEDED``: Job succeeded.
+
+    - ``CANCELLING``: Job was requested to be cancelled by the user, and the
+      cancellation is in progress.
 
-    If the job failed, either due to user code or spot unavailability, the error
-    log can be found with ``sky spot logs --controller job_id``.
+    - ``CANCELLED``: Job was cancelled by the user.
+
+    - ``FAILED``: Job failed due to an error from the job itself.
+
+    - ``FAILED_SETUP``: Job failed due to an error from the job's ``setup``
+      commands.
+
+    - ``FAILED_PRECHECKS``: Job failed due to an error from our prechecks such
+      as invalid cluster names or an infeasible resource is specified.
+
+    - ``FAILED_NO_RESOURCE``: Job failed due to resources being unavailable
+      after a maximum number of retries.
+
+    - ``FAILED_CONTROLLER``: Job failed due to an unexpected error in the spot
+      controller.
+
+    If the job failed, either due to user code or spot unavailability, the
+    error log can be found with ``sky spot logs --controller``, e.g.:
+
+    .. code-block:: bash
+
+      sky spot logs --controller job_id
+
+    This also shows the logs for provisioning and any preemption and recovery
+    attempts.
 
     (Tip) To fetch job statuses every 60 seconds, use ``watch``:
 
     .. code-block:: bash
 
       watch -n60 sky spot queue
+
     """
     click.secho('Fetching managed spot job statuses...', fg='yellow')
     with log_utils.safe_rich_status('[cyan]Checking spot jobs[/]'):
         _, msg = _get_spot_jobs(refresh=refresh,
                                 skip_finished=skip_finished,
-                                show_all=all)
+                                show_all=all,
+                                is_called_by_user=True)
     if not skip_finished:
         in_progress_only_hint = ''
     else:
         in_progress_only_hint = ' (showing in-progress jobs only)'
     click.echo(f'{colorama.Fore.CYAN}{colorama.Style.BRIGHT}'
                f'Managed spot jobs{colorama.Style.RESET_ALL}'
                f'{in_progress_only_hint}\n{msg}')
@@ -3418,28 +3573,27 @@
               required=False,
               help='Skip confirmation prompt.')
 @usage_lib.entrypoint
 # pylint: disable=redefined-builtin
 def spot_cancel(name: Optional[str], job_ids: Tuple[int], all: bool, yes: bool):
     """Cancel managed spot jobs.
 
-    You can provide either a job name or a list of job ids to be cancelled.
+    You can provide either a job name or a list of job IDs to be cancelled.
     They are exclusive options.
+
     Examples:
 
     .. code-block:: bash
 
-        # Cancel managed spot job with name 'my-job'
-        $ sky spot cancel -n my-job
-
-        # Cancel managed spot jobs with IDs 1, 2, 3
-        $ sky spot cancel 1 2 3
-
+      # Cancel managed spot job with name 'my-job'
+      $ sky spot cancel -n my-job
+      \b
+      # Cancel managed spot jobs with IDs 1, 2, 3
+      $ sky spot cancel 1 2 3
     """
-
     _, handle = spot_lib.is_spot_controller_up(
         'All managed spot jobs should have finished.')
     if handle is None:
         # Hint messages already printed by the call above.
         sys.exit(1)
 
     job_id_str = ','.join(map(str, job_ids))
@@ -3540,15 +3694,15 @@
         if not isinstance(candidate, dict):
             raise ValueError('Each resource candidate must be a dictionary.')
     return candidates
 
 
 @cli.group(cls=_NaturalOrderGroup)
 def bench():
-    """Sky Benchmark related commands."""
+    """SkyPilot Benchmark CLI."""
     pass
 
 
 @bench.command('launch', cls=_DocumentedCodeCommand)
 @click.argument('entrypoint',
                 required=True,
                 type=str,
@@ -3567,14 +3721,22 @@
                     'Example values: "T4:4,V100:8" (without blank spaces).'))
 @click.option('--disk-size',
               default=None,
               type=int,
               required=False,
               help=('OS disk size in GBs.'))
 @click.option(
+    '--disk-tier',
+    default=None,
+    type=str,
+    required=False,
+    help=(
+        'OS disk tier. Could be one of "low", "medium", "high". Default: medium'
+    ))
+@click.option(
     '--idle-minutes-to-autostop',
     '-i',
     default=None,
     type=int,
     required=False,
     help=('Automatically stop the cluster after this many minutes '
           'of idleness after setup/file_mounts. This is equivalent to '
@@ -3597,14 +3759,15 @@
     zone: Optional[str],
     gpus: Optional[str],
     num_nodes: Optional[int],
     use_spot: Optional[bool],
     image_id: Optional[str],
     env: List[Tuple[str, str]],
     disk_size: Optional[int],
+    disk_tier: Optional[str],
     idle_minutes_to_autostop: Optional[int],
     yes: bool,
 ) -> None:
     """Benchmark a task on different resources.
 
     Example usage: `sky bench launch mytask.yaml -b mytask --gpus V100,T4`
     will benchmark your task on a V100 cluster and a T4 cluster simultaneously.
@@ -3653,14 +3816,17 @@
                 raise click.BadParameter(f'use_spot {message}')
         if image_id is not None:
             if any('image_id' in candidate for candidate in candidates):
                 raise click.BadParameter(f'image_id {message}')
         if disk_size is not None:
             if any('disk_size' in candidate for candidate in candidates):
                 raise click.BadParameter(f'disk_size {message}')
+        if disk_tier is not None:
+            if any('disk_tier' in candidate for candidate in candidates):
+                raise click.BadParameter(f'disk_tier {message}')
 
     # The user can specify the benchmark candidates in either of the two ways:
     # 1. By specifying resources.candidates in the YAML.
     # 2. By specifying gpu types as a command line argument (--gpus).
     override_gpu = None
     if gpus is not None:
         gpu_list = gpus.split(',')
@@ -3695,15 +3861,16 @@
         config['num_nodes'] = num_nodes
     override_params = _parse_override_params(cloud=cloud,
                                              region=region,
                                              zone=zone,
                                              gpus=override_gpu,
                                              use_spot=use_spot,
                                              image_id=image_id,
-                                             disk_size=disk_size)
+                                             disk_size=disk_size,
+                                             disk_tier=disk_tier)
     resources_config.update(override_params)
     if 'cloud' in resources_config:
         cloud = resources_config.pop('cloud')
         if cloud is not None:
             resources_config['cloud'] = str(cloud)
     if 'region' in resources_config:
         if resources_config['region'] is None:
@@ -4066,14 +4233,15 @@
                        f'{backend_utils.RESET_BOLD} '
                        'before deleting the benchmark report.')
             success = False
         else:
             bucket_name = benchmark_state.get_benchmark_from_name(
                 benchmark)['bucket']
             handle = global_user_state.get_handle_from_storage_name(bucket_name)
+            assert handle is not None, bucket_name
             bucket_type = list(handle.sky_stores.keys())[0]
             benchmark_utils.remove_benchmark_logs(benchmark, bucket_name,
                                                   bucket_type)
             benchmark_state.delete_benchmark(benchmark)
             message = (f'{colorama.Fore.GREEN}Benchmark report for '
                        f'{benchmark} deleted.{colorama.Style.RESET_ALL}')
             success = True
```

### Comparing `skypilot-0.2.5/sky/cloud_stores.py` & `skypilot-0.3.0/sky/cloud_stores.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 * Better implementation (e.g., fsspec, smart_open, using each cloud's SDK).
 """
 import subprocess
 import urllib.parse
 
 from sky.clouds import gcp
 from sky.data import data_utils
-from sky.adaptors import aws
+from sky.adaptors import aws, cloudflare
 
 
 class CloudStorage:
     """Interface for a cloud object store."""
 
     def is_directory(self, url: str) -> bool:
         """Returns whether 'url' is a directory.
@@ -142,21 +142,85 @@
         """Downloads a file using gsutil."""
         download_via_gsutil = f'{self._GSUTIL} -m cp {source} {destination}'
         all_commands = [self._GET_GSUTIL]
         all_commands.append(download_via_gsutil)
         return ' && '.join(all_commands)
 
 
+class R2CloudStorage(CloudStorage):
+    """Cloudflare Cloud Storage."""
+
+    # List of commands to install AWS CLI
+    _GET_AWSCLI = [
+        'aws --version >/dev/null 2>&1 || pip3 install awscli',
+    ]
+
+    def is_directory(self, url: str) -> bool:
+        """Returns whether R2 'url' is a directory.
+
+        In cloud object stores, a "directory" refers to a regular object whose
+        name is a prefix of other objects.
+        """
+        r2 = cloudflare.resource('s3')
+        bucket_name, path = data_utils.split_r2_path(url)
+        bucket = r2.Bucket(bucket_name)
+
+        num_objects = 0
+        for obj in bucket.objects.filter(Prefix=path):
+            num_objects += 1
+            if obj.key == path:
+                return False
+            # If there are more than 1 object in filter, then it is a directory
+            if num_objects == 3:
+                return True
+
+        # A directory with few or no items
+        return True
+
+    def make_sync_dir_command(self, source: str, destination: str) -> str:
+        """Downloads using AWS CLI."""
+        # AWS Sync by default uses 10 threads to upload files to the bucket.
+        # To increase parallelism, modify max_concurrent_requests in your
+        # aws config file (Default path: ~/.aws/config).
+        endpoint_url = cloudflare.create_endpoint()
+        if 'r2://' in source:
+            source = source.replace('r2://', 's3://')
+        download_via_awscli = ('AWS_SHARED_CREDENTIALS_FILE='
+                               f'{cloudflare.R2_CREDENTIALS_PATH} '
+                               'aws s3 sync --no-follow-symlinks '
+                               f'{source} {destination} '
+                               f'--endpoint {endpoint_url} '
+                               f'--profile={cloudflare.R2_PROFILE_NAME}')
+
+        all_commands = list(self._GET_AWSCLI)
+        all_commands.append(download_via_awscli)
+        return ' && '.join(all_commands)
+
+    def make_sync_file_command(self, source: str, destination: str) -> str:
+        """Downloads a file using AWS CLI."""
+        endpoint_url = cloudflare.create_endpoint()
+        download_via_awscli = ('AWS_SHARED_CREDENTIALS_FILE='
+                               f'{cloudflare.R2_CREDENTIALS_PATH} '
+                               f'aws s3 cp s3://{source} {destination} '
+                               f'--endpoint {endpoint_url} '
+                               f'--profile={cloudflare.R2_PROFILE_NAME}')
+
+        all_commands = list(self._GET_AWSCLI)
+        all_commands.append(download_via_awscli)
+        return ' && '.join(all_commands)
+
+
 def get_storage_from_path(url: str) -> CloudStorage:
     """Returns a CloudStorage by identifying the scheme:// in a URL."""
     result = urllib.parse.urlsplit(url)
 
     if result.scheme not in _REGISTRY:
         assert False, (f'Scheme {result.scheme} not found in'
                        f' supported storage ({_REGISTRY.keys()}); path {url}')
     return _REGISTRY[result.scheme]
 
 
 _REGISTRY = {
     'gs': GcsCloudStorage(),
     's3': S3CloudStorage(),
+    'r2': R2CloudStorage()
 }
```

### Comparing `skypilot-0.2.5/sky/clouds/__init__.py` & `skypilot-0.3.0/sky/clouds/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from sky.clouds.cloud import Region
 from sky.clouds.cloud import Zone
 from sky.clouds.aws import AWS
 from sky.clouds.azure import Azure
 from sky.clouds.gcp import GCP
 from sky.clouds.lambda_cloud import Lambda
 from sky.clouds.local import Local
+from sky.clouds.ibm import IBM
 
 __all__ = [
+    'IBM',
     'AWS',
     'Azure',
     'Cloud',
     'GCP',
     'Lambda',
     'Local',
     'CloudImplementationFeatures',
```

### Comparing `skypilot-0.2.5/sky/clouds/aws.py` & `skypilot-0.3.0/sky/clouds/aws.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Amazon Web Services."""
+import enum
 import functools
 import json
 import os
+import re
 import subprocess
 import typing
-from typing import Dict, Iterator, List, Optional, Tuple
+from typing import Dict, Iterator, List, Optional, Tuple, Any
 
 from sky import clouds
 from sky import exceptions
 from sky.adaptors import aws
 from sky.clouds import service_catalog
 from sky.utils import common_utils
 from sky.utils import ux_utils
@@ -36,14 +38,42 @@
 _CREDENTIAL_FILES = [
     'credentials',
 ]
 
 DEFAULT_AMI_GB = 45
 
 
+class AWSIdentityType(enum.Enum):
+    """AWS identity type.
+
+    The account type is determined by the current user identity, based on `aws
+    configure list`. We will check the existence of the value in the output of
+    `aws configure list` to determine the account type.
+    """
+    #       Name                    Value             Type    Location
+    #       ----                    -----             ----    --------
+    #    profile                     1234              env    ...
+    # access_key     ****************abcd              sso
+    # secret_key     ****************abcd              sso
+    #     region                <not set>             None    None
+    SSO = 'sso'
+
+    ENV = 'env'
+
+    IAM_ROLE = 'iam-role'
+
+    #       Name                    Value             Type    Location
+    #       ----                    -----             ----    --------
+    #    profile                <not set>             None    None
+    # access_key     ****************abcd shared-credentials-file
+    # secret_key     ****************abcd shared-credentials-file
+    #     region                us-east-1      config-file    ~/.aws/config
+    SHARED_CREDENTIALS_FILE = 'shared-credentials-file'
+
+
 @clouds.CLOUD_REGISTRY.register
 class AWS(clouds.Cloud):
     """Amazon Web Services."""
 
     _REPR = 'AWS'
 
     # AWS has a limit of the tag value length to 256 characters.
@@ -265,17 +295,19 @@
     def is_same_cloud(self, other: clouds.Cloud):
         return isinstance(other, AWS)
 
     @classmethod
     def get_default_instance_type(
             cls,
             cpus: Optional[str] = None,
-            memory: Optional[str] = None) -> Optional[str]:
+            memory: Optional[str] = None,
+            disk_tier: Optional[str] = None) -> Optional[str]:
         return service_catalog.get_default_instance_type(cpus=cpus,
                                                          memory=memory,
+                                                         disk_tier=disk_tier,
                                                          clouds='aws')
 
     # TODO: factor the following three methods, as they are the same logic
     # between Azure and AWS.
     @classmethod
     def get_accelerators_from_instance_type(
         cls,
@@ -290,15 +322,15 @@
         instance_type: str,
     ) -> Tuple[Optional[float], Optional[float]]:
         return service_catalog.get_vcpus_mem_from_instance_type(instance_type,
                                                                 clouds='aws')
 
     def make_deploy_resources_variables(
             self, resources: 'resources_lib.Resources', region: 'clouds.Region',
-            zones: Optional[List['clouds.Zone']]) -> Dict[str, Optional[str]]:
+            zones: Optional[List['clouds.Zone']]) -> Dict[str, Any]:
         assert zones is not None, (region, zones)
 
         region_name = region.name
         zone_names = [zone.name for zone in zones]
 
         r = resources
         # r.accelerators is cleared but .instance_type encodes the info.
@@ -313,14 +345,15 @@
         return {
             'instance_type': r.instance_type,
             'custom_resources': custom_resources,
             'use_spot': r.use_spot,
             'region': region_name,
             'zones': ','.join(zone_names),
             'image_id': image_id,
+            **AWS._get_disk_specs(r.disk_tier)
         }
 
     def get_feasible_launchable_resources(self,
                                           resources: 'resources_lib.Resources'):
         if resources.instance_type is not None:
             assert resources.is_launchable(), resources
             # Treat Resources(AWS, p3.2x, V100) as Resources(AWS, p3.2x).
@@ -343,15 +376,17 @@
             return resource_list
 
         # Currently, handle a filter on accelerators only.
         accelerators = resources.accelerators
         if accelerators is None:
             # Return a default instance type with the given number of vCPUs.
             default_instance_type = AWS.get_default_instance_type(
-                cpus=resources.cpus, memory=resources.memory)
+                cpus=resources.cpus,
+                memory=resources.memory,
+                disk_tier=resources.disk_tier)
             if default_instance_type is None:
                 return ([], [])
             else:
                 return (_make([default_instance_type]), [])
 
         assert len(accelerators) == 1, resources
         acc, acc_count = list(accelerators.items())[0]
@@ -401,27 +436,35 @@
             cls.get_current_user_identity()
         except exceptions.CloudUserIdentityError as e:
             return False, str(e)
 
         static_credential_exists = os.path.isfile(
             os.path.expanduser('~/.aws/credentials'))
         hints = None
-        if cls._is_current_identity_sso():
-            hints = 'AWS SSO is set. '
+        identity_type = cls._current_identity_type()
+        single_cloud_hint = (
+            ' It will work if you use AWS only, but will cause problems '
+            'if you want to use multiple clouds. To set up static credentials, '
+            'try: aws configure')
+        if identity_type == AWSIdentityType.SSO:
+            hints = 'AWS SSO is set.'
             if static_credential_exists:
                 hints += (
                     ' To ensure multiple clouds work correctly, please use SkyPilot '
                     'with static credentials (e.g., ~/.aws/credentials) by unsetting '
                     'the AWS_PROFILE environment variable.')
             else:
-                hints += (
-                    ' It will work if you use AWS only, but will cause problems '
-                    'if you want to use multiple clouds. To set up static credentials, '
-                    'try: aws configure')
-
+                hints += single_cloud_hint
+        elif identity_type == AWSIdentityType.IAM_ROLE:
+            # When using an IAM role, the credentials may not exist in the
+            # ~/.aws/credentials file. So we don't check for the existence of the
+            # file. This will happen when the user is on a VM (or spot-controller)
+            # created by an SSO account, i.e. the VM will be assigned the IAM
+            # role: skypilot-v1.
+            hints = f'AWS IAM role is set.{single_cloud_hint}'
         else:
             # This file is required because it is required by the VMs launched on
             # other clouds to access private s3 buckets and resources like EC2.
             # `get_current_user_identity` does not guarantee this file exists.
             if not static_credential_exists:
                 return (False, '~/.aws/credentials does not exist. ' +
                         cls._STATIC_CREDENTIAL_HELP_STR)
@@ -429,44 +472,105 @@
         # Fetch the AWS catalogs
         from sky.clouds.service_catalog import aws_catalog  # pylint: disable=import-outside-toplevel,unused-import
         # Trigger the fetch of the availability zones mapping.
         aws_catalog.get_default_instance_type()
         return True, hints
 
     @classmethod
-    def _is_current_identity_sso(cls) -> bool:
+    def _current_identity_type(cls) -> Optional[AWSIdentityType]:
         proc = subprocess.run('aws configure list',
                               shell=True,
                               check=False,
                               stdout=subprocess.PIPE,
                               stderr=subprocess.PIPE)
         if proc.returncode != 0:
-            return False
-        return 'sso' in proc.stdout.decode().split()
+            return None
+        stdout = proc.stdout.decode()
+
+        # We determine the identity type by looking at the output of
+        # `aws configure list`. The output looks like:
+        #   Name                   Value         Type    Location
+        #   ----                   -----         ----    --------
+        #   profile                <not set>     None    None
+        #   access_key     *       <not set>     sso     None
+        #   secret_key     *       <not set>     sso     None
+        #   region                 <not set>     None    None
+        # We try to determine the identity type by looking for the
+        # string "sso"/"iam-role" in the output, i.e. the "Type" column.
+
+        def _is_access_key_of_type(type_str: str) -> bool:
+            # The dot (.) does not match line separators.
+            results = re.findall(fr'access_key.*{type_str}', stdout)
+            if len(results) > 1:
+                raise RuntimeError(
+                    f'Unexpected `aws configure list` output:\n{stdout}')
+            return len(results) == 1
+
+        if _is_access_key_of_type(AWSIdentityType.SSO.value):
+            return AWSIdentityType.SSO
+        elif _is_access_key_of_type(AWSIdentityType.IAM_ROLE.value):
+            return AWSIdentityType.IAM_ROLE
+        elif _is_access_key_of_type(AWSIdentityType.ENV.value):
+            return AWSIdentityType.ENV
+        else:
+            return AWSIdentityType.SHARED_CREDENTIALS_FILE
 
     @classmethod
-    def get_current_user_identity(cls) -> Optional[str]:
-        """Returns the identity of the user on this cloud.
+    def get_current_user_identity(cls) -> Optional[List[str]]:
+        """Returns a [UserId, Account] list that uniquely identifies the user.
+
+        These fields come from `aws sts get-caller-identity`. We permit the same
+        actual user to:
+
+          - switch between different root accounts (after which both elements
+            of the list will be different) and have their clusters owned by
+            each account be protected; or
+
+          - within the same root account, switch between different IAM
+            users, and treat [user_id=1234, account=A] and
+            [user_id=4567, account=A] to be the *same*. Namely, switching
+            between these IAM roles within the same root account will cause
+            the first element of the returned list to differ, and will allow
+            the same actual user to continue to interact with their clusters.
+            Note: this is not 100% safe, since the IAM users can have very
+            specific permissions, that disallow them to access the clusters
+            but it is a reasonable compromise as that could be rare.
+
+        Returns:
+            A list of strings that uniquely identifies the user on this cloud.
+            For identity check, we will fallback through the list of strings
+            until we find a match, and print a warning if we fail for the
+            first string.
 
         Raises:
             exceptions.CloudUserIdentityError: if the user identity cannot be
                 retrieved.
         """
         try:
             sts = aws.client('sts')
-            # The caller identity contains 3 fields: UserId, AccountId, Arn.
-            # 'UserId' is unique across all AWS entity, which looks like
+            # The caller identity contains 3 fields: UserId, Account, Arn.
+            # 1. 'UserId' is unique across all AWS entity, which looks like
             # "AROADBQP57FF2AEXAMPLE:role-session-name"
-            # 'AccountId' can be shared by multiple users under the same
+            # 2. 'Account' can be shared by multiple users under the same
             # organization
-            # 'Arn' is the full path to the user, which can be reused when
+            # 3. 'Arn' is the full path to the user, which can be reused when
             # the user is deleted and recreated.
             # Refer to https://docs.aws.amazon.com/cli/latest/reference/sts/get-caller-identity.html # pylint: disable=line-too-long
             # and https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_variables.html#principaltable # pylint: disable=line-too-long
-            user_id = sts.get_caller_identity()['UserId']
+            user_info = sts.get_caller_identity()
+            # Allow fallback to AccountId if UserId does not match, because:
+            # 1. In the case where multiple IAM users belong a single root account,
+            # those users normally share the visibility of the VMs, so we do not
+            # need to identity them with each other. (There can be some cases,
+            # when an IAM user is given a limited permission by the admin, we may
+            # ignore that case for now, or print out a warning if the underlying
+            # userid changed for a cluster).
+            # 2. In the case where the multiple users belong to an organization,
+            # those users will have different account id, so fallback works.
+            user_ids = [user_info['UserId'], user_info['Account']]
         except aws.botocore_exceptions().NoCredentialsError:
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.CloudUserIdentityError(
                     f'AWS credentials are not set. {cls._STATIC_CREDENTIAL_HELP_STR}'
                 ) from None
         except aws.botocore_exceptions().ClientError:
             with ux_utils.print_exception_no_traceback():
@@ -503,34 +607,40 @@
                     f' {cls._sso_credentials_help_str(expired=True)}') from None
         except Exception as e:  # pylint: disable=broad-except
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.CloudUserIdentityError(
                     f'Failed to get AWS user.\n'
                     f'  Reason: {common_utils.format_exception(e, use_bracket=True)}.'
                 ) from None
-        return user_id
+        return user_ids
 
     def get_credential_file_mounts(self) -> Dict[str, str]:
-        # TODO(skypilot): ~/.aws/credentials is required for users using multiple clouds.
-        # If this file does not exist, users can launch on AWS via AWS SSO and assign
-        # IAM role to the cluster.
-        # However, if users launch clusters in a non-AWS cloud, those clusters do not
-        # understand AWS IAM role so will not be able to access private AWS EC2 resources
-        # and S3 buckets.
-
-        # The file should not be uploaded if the user is using SSO, as the credential
-        # file can be from a different account, and will make autopstop/autodown/spot
+        # The credentials file should not be uploaded if the user identity is
+        # not SHARED_CREDENTIALS_FILE, since we cannot be sure if the currently
+        # active user identity is the same as the one encoded in the credentials
+        # file.  If they are indeed different identities, then uploading the
+        # credential file to a launched node will make autostop/autodown/spot
         # controller misbehave.
-
-        # TODO(zhwu/zongheng): We can also avoid uploading the credential file for the
-        # cluster launched on AWS even if the user is using static credentials. We need
-        # to define a mechanism to find out the cloud provider of the cluster to be
-        # launched in this function and make sure the cluster will not be used for
-        # launching clusters in other clouds, e.g. spot controller.
-        if self._is_current_identity_sso():
+        #
+        # TODO(skypilot): ~/.aws/credentials is required for users using
+        # multiple clouds.  If this file does not exist, users can launch on AWS
+        # via AWS SSO or assumed IAM role (only when the user is on an AWS
+        # cluster) and assign IAM role to the cluster.  However, if users launch
+        # clusters in a non-AWS cloud, those clusters do not understand AWS IAM
+        # role so will not be able to access private AWS EC2 resources and S3
+        # buckets.
+        #
+        # TODO(zhwu/zongheng): We can also avoid uploading the credential file
+        # for the cluster launched on AWS even if the user is using static
+        # credentials. We need to define a mechanism to find out the cloud
+        # provider of the cluster to be launched in this function and make sure
+        # the cluster will not be used for launching clusters in other clouds,
+        # e.g. spot controller.
+        if self._current_identity_type(
+        ) != AWSIdentityType.SHARED_CREDENTIALS_FILE:
             return {}
         return {
             f'~/.aws/{filename}': f'~/.aws/{filename}'
             for filename in _CREDENTIAL_FILES
             if os.path.exists(os.path.expanduser(f'~/.aws/{filename}'))
         }
 
@@ -540,7 +650,31 @@
     def accelerator_in_region_or_zone(self,
                                       accelerator: str,
                                       acc_count: int,
                                       region: Optional[str] = None,
                                       zone: Optional[str] = None) -> bool:
         return service_catalog.accelerator_in_region_or_zone(
             accelerator, acc_count, region, zone, 'aws')
+
+    @classmethod
+    def check_disk_tier_enabled(cls, instance_type: str,
+                                disk_tier: str) -> None:
+        del instance_type, disk_tier  # unused
+
+    @classmethod
+    def _get_disk_type(cls, disk_tier: str) -> str:
+        return 'standard' if disk_tier == 'low' else 'gp3'
+
+    @classmethod
+    def _get_disk_specs(cls, disk_tier: Optional[str]) -> Dict[str, Any]:
+        tier = disk_tier or cls._DEFAULT_DISK_TIER
+        tier2iops = {
+            'high': 7000,
+            'medium': 3500,
+            'low': 0,  # only gp3 is required to set iops
+        }
+        return {
+            'disk_tier': cls._get_disk_type(tier),
+            'disk_iops': tier2iops[tier],
+            'disk_throughput': tier2iops[tier] // 16,
+            'custom_disk_perf': tier != 'low',
+        }
```

### Comparing `skypilot-0.2.5/sky/clouds/azure.py` & `skypilot-0.3.0/sky/clouds/azure.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Azure."""
 import functools
 import json
 import os
+import re
 import subprocess
 import typing
 from typing import Dict, Iterator, List, Optional, Tuple
 
 import colorama
 
 from sky import clouds
@@ -110,17 +111,19 @@
     def is_same_cloud(self, other):
         return isinstance(other, Azure)
 
     @classmethod
     def get_default_instance_type(
             cls,
             cpus: Optional[str] = None,
-            memory: Optional[str] = None) -> Optional[str]:
+            memory: Optional[str] = None,
+            disk_tier: Optional[str] = None) -> Optional[str]:
         return service_catalog.get_default_instance_type(cpus=cpus,
                                                          memory=memory,
+                                                         disk_tier=disk_tier,
                                                          clouds='azure')
 
     def _get_image_config(self, gen_version, instance_type):
         # az vm image list \
         #  --publisher microsoft-dsvm --all --output table
         # nvidia-driver: 495.29.05, cuda: 11.5
 
@@ -233,49 +236,72 @@
         return {
             'instance_type': r.instance_type,
             'custom_resources': custom_resources,
             'use_spot': r.use_spot,
             'region': region_name,
             # Azure does not support specific zones.
             'zones': None,
-            **image_config
+            **image_config,
+            'disk_tier': Azure._get_disk_type(r.disk_tier)
         }
 
     def get_feasible_launchable_resources(self, resources):
+
+        def failover_disk_tier(instance_type: str,
+                               disk_tier: Optional[str]) -> Optional[str]:
+            if disk_tier is None:
+                ok, _ = Azure.check_disk_tier(instance_type,
+                                              clouds.Cloud._DEFAULT_DISK_TIER)
+                if not ok:
+                    # Auto failover to low disk tier when disk tier
+                    # are not specified
+                    return 'low'
+            # The disk_tier specified by the user will be checked in the
+            # initialization of the Resources.
+            return disk_tier
+
         if resources.use_spot:
             # TODO(zhwu): our azure subscription offer ID does not support spot.
             # Need to support it.
             return ([], [])
         if resources.instance_type is not None:
             assert resources.is_launchable(), resources
             # Treat Resources(AWS, p3.2x, V100) as Resources(AWS, p3.2x).
-            resources = resources.copy(accelerators=None)
+            resources = resources.copy(
+                accelerators=None,
+                disk_tier=failover_disk_tier(resources.instance_type,
+                                             resources.disk_tier),
+            )
             return ([resources], [])
 
         def _make(instance_list):
             resource_list = []
             for instance_type in instance_list:
                 r = resources.copy(
                     cloud=Azure(),
                     instance_type=instance_type,
+                    disk_tier=failover_disk_tier(instance_type,
+                                                 resources.disk_tier),
                     # Setting this to None as Azure doesn't separately bill /
                     # attach the accelerators.  Billed as part of the VM type.
                     accelerators=None,
                     cpus=None,
                     memory=None,
                 )
                 resource_list.append(r)
             return resource_list
 
         # Currently, handle a filter on accelerators only.
         accelerators = resources.accelerators
         if accelerators is None:
             # Return a default instance type with the given number of vCPUs.
             default_instance_type = Azure.get_default_instance_type(
-                cpus=resources.cpus, memory=resources.memory)
+                cpus=resources.cpus,
+                memory=resources.memory,
+                disk_tier=resources.disk_tier)
             if default_instance_type is None:
                 return ([], [])
             else:
                 return (_make([default_instance_type]), [])
 
         assert len(accelerators) == 1, resources
         acc, acc_count = list(accelerators.items())[0]
@@ -344,15 +370,15 @@
                                       region: Optional[str] = None,
                                       zone: Optional[str] = None) -> bool:
         return service_catalog.accelerator_in_region_or_zone(
             accelerator, acc_count, region, zone, 'azure')
 
     @classmethod
     @functools.lru_cache(maxsize=1)  # Cache since getting identity is slow.
-    def get_current_user_identity(cls) -> Optional[str]:
+    def get_current_user_identity(cls) -> Optional[List[str]]:
         """Returns the cloud user identity."""
         # This returns the user's email address + [subscription_id].
         retry_cnt = 0
         while True:
             retry_cnt += 1
             try:
                 import knack  # pylint: disable=import-outside-toplevel
@@ -386,15 +412,15 @@
                     ) from e
         try:
             project_id = cls.get_project_id()
         except (ModuleNotFoundError, RuntimeError) as e:
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.CloudUserIdentityError(
                     'Failed to get Azure project ID.') from e
-        return f'{account_email} [subscription_id={project_id}]'
+        return [f'{account_email} [subscription_id={project_id}]']
 
     @classmethod
     def get_project_id(cls, dryrun: bool = False) -> str:
         if dryrun:
             return 'dryrun-project-id'
         try:
             azure_subscription_id = azure.get_subscription_id()
@@ -410,7 +436,57 @@
             with ux_utils.print_exception_no_traceback():
                 raise RuntimeError(
                     'Failed to get subscription id from azure cli. '
                     'Make sure you have logged in and run this Azure '
                     'cli command: "az account set -s <subscription_id>".'
                 ) from e
         return azure_subscription_id
+
+    @classmethod
+    def _is_s_series(cls, instance_type: Optional[str]) -> bool:
+        # For azure naming convention, see https://learn.microsoft.com/en-us/azure/virtual-machines/vm-naming-conventions  # pylint: disable=line-too-long
+        if instance_type is None:
+            return True
+        x = re.match(
+            r'(Standard|Basic)_([A-Z]+)([0-9]+)(-[0-9]+)?'
+            r'([a-z]*)(_[A-Z]+[0-9]+)?(_v[0-9])?(_Promo)?', instance_type)
+        assert x is not None, f'Unknown instance type: {instance_type}'
+        return 's' in x.group(5)
+
+    @classmethod
+    def check_disk_tier(cls, instance_type: Optional[str],
+                        disk_tier: Optional[str]) -> Tuple[bool, str]:
+        if disk_tier is None:
+            return True, ''
+        if disk_tier == 'high':
+            return False, ('Azure disk_tier=high is not supported now. '
+                           'Please use disk_tier={low, medium} instead.')
+        # Only S-series supported premium ssd
+        # see https://stackoverflow.com/questions/48590520/azure-requested-operation-cannot-be-performed-because-storage-account-type-pre  # pylint: disable=line-too-long
+        if cls._get_disk_type(
+                disk_tier
+        ) == 'Premium_LRS' and not Azure._is_s_series(instance_type):
+            return False, (
+                'Azure premium SSDs are only supported for S-series '
+                'instances. To use disk_tier=medium, please make sure '
+                'instance_type is specified to an S-series instance.')
+        return True, ''
+
+    @classmethod
+    def check_disk_tier_enabled(cls, instance_type: str,
+                                disk_tier: str) -> None:
+        ok, msg = cls.check_disk_tier(instance_type, disk_tier)
+        if not ok:
+            with ux_utils.print_exception_no_traceback():
+                raise ValueError(msg)
+
+    @classmethod
+    def _get_disk_type(cls, disk_tier: Optional[str]) -> str:
+        tier = disk_tier or cls._DEFAULT_DISK_TIER
+        # TODO(tian): Maybe use PremiumV2_LRS/UltraSSD_LRS? Notice these two
+        # cannot be used as OS disks so we might need data disk support
+        tier2name = {
+            'high': 'Disabled',
+            'medium': 'Premium_LRS',
+            'low': 'Standard_LRS',
+        }
+        return tier2name[tier]
```

### Comparing `skypilot-0.2.5/sky/clouds/cloud.py` & `skypilot-0.3.0/sky/clouds/cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     """Registry of clouds."""
 
     def from_str(self, name: Optional[str]) -> Optional['Cloud']:
         if name is None:
             return None
         if name.lower() not in self:
             with ux_utils.print_exception_no_traceback():
-                raise ValueError(f'Cloud {name} is not a valid cloud among '
+                raise ValueError(f'Cloud {name!r} is not a valid cloud among '
                                  f'{list(self.keys())}')
         return self.get(name.lower())
 
     def register(self, cloud_cls: Type['Cloud']) -> Type['Cloud']:
         name = cloud_cls.__name__.lower()
         assert name not in self, f'{name} already registered'
         self[name] = cloud_cls()
@@ -68,14 +68,15 @@
 CLOUD_REGISTRY = _CloudRegistry()
 
 
 class Cloud:
     """A cloud provider."""
 
     _REPR = '<Cloud>'
+    _DEFAULT_DISK_TIER = 'medium'
 
     @classmethod
     def _cloud_unsupported_features(
             cls) -> Dict[CloudImplementationFeatures, str]:
         """The features not supported by the cloud implementation.
 
         This method is used by check_features_are_supported() to check if the
@@ -247,28 +248,35 @@
         """Returns {acc: acc_count} held by 'instance_type', if any."""
         raise NotImplementedError
 
     @classmethod
     def get_default_instance_type(
             cls,
             cpus: Optional[str] = None,
-            memory: Optional[str] = None) -> Optional[str]:
-        """Returns the default instance type with the given #vCPUs and memory.
+            memory: Optional[str] = None,
+            disk_tier: Optional[str] = None) -> Optional[str]:
+        """Returns the default instance type with the given #vCPUs, memory and
+        disk tier.
 
         For example, if cpus='4', this method returns the default instance type
         with 4 vCPUs.  If cpus='4+', this method returns the default instance
         type with 4 or more vCPUs.
 
         If 'memory=4', this method returns the default instance type with 4GB
         memory.  If 'memory=4+', this method returns the default instance
         type with 4GB or more memory.
 
-        When cpus is None or memory is None, this method will never return None.
-        This method may return None if the cloud's default instance family
-        does not have a VM with the given number of vCPUs (e.g., when cpus='7').
+        If disk_rier='medium', this method returns the default instance type
+        that support medium disk tier.
+
+        When cpus is None, memory is None or disk tier is None, this method will
+        never return None. This method may return None if the cloud's default
+        instance family does not have a VM with the given number of vCPUs
+        (e.g., when cpus='7') or does not have a VM with the give disk tier
+        (e.g. Azure, disk_tier='high').
         """
         raise NotImplementedError
 
     @classmethod
     def is_image_tag_valid(cls, image_tag: str, region: Optional[str]) -> bool:
         """Validates that the image tag is valid for this cloud."""
         return service_catalog.is_image_tag_valid(image_tag,
@@ -291,16 +299,17 @@
         """Checks if the user has access credentials to this cloud.
 
         Returns a boolean of whether the user can access this cloud, and a
         string describing the reason if the user cannot access.
         """
         raise NotImplementedError
 
+    # TODO(zhwu): Make the return type immutable.
     @classmethod
-    def get_current_user_identity(cls) -> Optional[str]:
+    def get_current_user_identity(cls) -> Optional[List[str]]:
         """(Advanced) Returns currently active user identity of this cloud.
 
         The user "identity" is associated with each SkyPilot cluster they
         creates. This is used in protecting cluster operations, such as
         provision, teardown and status refreshing, in a multi-identity
         scenario, where the same user/device can switch between different
         cloud identities. We check that the user identity matches before:
@@ -315,18 +324,27 @@
 
         The choice of what constitutes an identity is up to each cloud's
         implementation. In general, to suffice for the above purposes,
         ensure that different identities should imply different sets of
         resources are used when the user invoked each cloud's default
         CLI/API.
 
+        The returned identity is a list of strings. The list is in the order of
+        strictness, i.e., the first element is the most strict identity, and
+        the last element is the least strict identity.
+        When performing an identity check between the current active identity
+        and the owner identity associated with a cluster, we compare the two
+        lists in order: if a position does not match, we go to the next. To
+        see an example, see the docstring of the AWS.get_current_user_identity.
+
+
         Example identities (see cloud implementations):
-            - AWS: unique aws:user_id
-            - GCP: email address + project ID
-            - Azure: email address + subscription ID
+            - AWS: [UserId, AccountId]
+            - GCP: [email address + project ID]
+            - Azure: [email address + subscription ID]
 
         Returns:
             None if the cloud does not have a concept of user identity
             (access protection will be disabled for these clusters);
             otherwise the currently active user identity.
         Raises:
             exceptions.CloudUserIdentityError: If the user identity cannot be
@@ -435,9 +453,19 @@
             cloud_name = '' if cls is Cloud else f' on {cls._REPR}'
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.InvalidClusterNameError(
                     f'Cluster name {cluster_name!r} has {len(cluster_name)} '
                     'chars; maximum length is '
                     f'{max_cluster_name_len_limit} chars{cloud_name}.')
 
+    @classmethod
+    def check_disk_tier_enabled(cls, instance_type: str,
+                                disk_tier: str) -> None:
+        """Errors out if the disk tier is not supported by the cloud provider.
+
+        Raises:
+            exceptions.NotSupportedError: If the disk tier is not supported.
+        """
+        raise NotImplementedError
+
     def __repr__(self):
         return self._REPR
```

### Comparing `skypilot-0.2.5/sky/clouds/gcp.py` & `skypilot-0.3.0/sky/clouds/gcp.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,22 +46,23 @@
     'access_tokens.db',
     'configurations',
     'legacy_credentials',
     'active_config',
 ]
 
 _GCLOUD_INSTALLATION_LOG = '~/.sky/logs/gcloud_installation.log'
+_GCLOUD_VERSION = '424.0.0'
 # Need to be run with /bin/bash
 # We factor out the installation logic to keep it align in both spot
 # controller and cloud stores.
 GCLOUD_INSTALLATION_COMMAND = f'pushd /tmp &>/dev/null && \
     gcloud --help > /dev/null 2>&1 || \
     {{ mkdir -p {os.path.dirname(_GCLOUD_INSTALLATION_LOG)} && \
-    wget --quiet https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-sdk-382.0.0-linux-x86_64.tar.gz > {_GCLOUD_INSTALLATION_LOG} && \
-    tar xzf google-cloud-sdk-382.0.0-linux-x86_64.tar.gz >> {_GCLOUD_INSTALLATION_LOG} && \
+    wget --quiet https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-sdk-{_GCLOUD_VERSION}-linux-x86_64.tar.gz > {_GCLOUD_INSTALLATION_LOG} && \
+    tar xzf google-cloud-sdk-{_GCLOUD_VERSION}-linux-x86_64.tar.gz >> {_GCLOUD_INSTALLATION_LOG} && \
     rm -rf ~/google-cloud-sdk >> {_GCLOUD_INSTALLATION_LOG}  && \
     mv google-cloud-sdk ~/ && \
     ~/google-cloud-sdk/install.sh -q >> {_GCLOUD_INSTALLATION_LOG} 2>&1 && \
     echo "source ~/google-cloud-sdk/path.bash.inc > /dev/null 2>&1" >> ~/.bashrc && \
     source ~/google-cloud-sdk/path.bash.inc >> {_GCLOUD_INSTALLATION_LOG} 2>&1; }} && \
     {{ cp {GCP_CONFIG_SKY_BACKUP_PATH} {GCP_CONFIG_PATH} > /dev/null 2>&1 || true; }} && \
     popd &>/dev/null'
@@ -265,17 +266,19 @@
                                      'GCP.') from None
             raise
 
     @classmethod
     def get_default_instance_type(
             cls,
             cpus: Optional[str] = None,
-            memory: Optional[str] = None) -> Optional[str]:
+            memory: Optional[str] = None,
+            disk_tier: Optional[str] = None) -> Optional[str]:
         return service_catalog.get_default_instance_type(cpus=cpus,
                                                          memory=memory,
+                                                         disk_tier=disk_tier,
                                                          clouds='gcp')
 
     def make_deploy_resources_variables(
             self, resources: 'resources.Resources', region: 'clouds.Region',
             zones: Optional[List['clouds.Zone']]) -> Dict[str, Optional[str]]:
         assert zones is not None, (region, zones)
 
@@ -348,25 +351,29 @@
         if image_id.startswith('skypilot:'):
             image_id = service_catalog.get_image_id_from_tag(image_id,
                                                              clouds='gcp')
 
         assert image_id is not None, (image_id, r)
         resources_vars['image_id'] = image_id
 
+        resources_vars['disk_tier'] = GCP._get_disk_type(r.disk_tier)
+
         return resources_vars
 
     def get_feasible_launchable_resources(self, resources):
         if resources.instance_type is not None:
             assert resources.is_launchable(), resources
             return ([resources], [])
 
         if resources.accelerators is None:
             # Return a default instance type with the given number of vCPUs.
             host_vm_type = GCP.get_default_instance_type(
-                cpus=resources.cpus, memory=resources.memory)
+                cpus=resources.cpus,
+                memory=resources.memory,
+                disk_tier=resources.disk_tier)
             if host_vm_type is None:
                 return ([], [])
             else:
                 r = resources.copy(
                     cloud=GCP(),
                     instance_type=host_vm_type,
                     accelerators=None,
@@ -567,17 +574,18 @@
         permissions = {'permissions': GCP_PREMISSION_CHECK_LIST}
         request = service.projects().testIamPermissions(resource=project,
                                                         body=permissions)
         ret_permissions = request.execute().get('permissions', [])
         if len(ret_permissions) < len(GCP_PREMISSION_CHECK_LIST):
             diffs = set(GCP_PREMISSION_CHECK_LIST).difference(
                 set(ret_permissions))
+            identity_str = identity[0] if identity else None
             return False, (
                 'The following permissions are not enabled for the current '
-                f'GCP identity ({identity}):\n    '
+                f'GCP identity ({identity_str}):\n    '
                 f'{diffs}\n    '
                 'For more details, visit: https://skypilot.readthedocs.io/en/latest/reference/faq.html#what-are-the-required-iam-permissons-on-gcp-for-skypilot')  # pylint: disable=line-too-long
         return True, None
 
     def get_credential_file_mounts(self) -> Dict[str, str]:
         # Create a backup of the config_default file, as the original file can
         # be modified on the remote cluster by ray causing authentication
@@ -602,15 +610,15 @@
             for filename in _CREDENTIAL_FILES
         }
         credentials[GCP_CONFIG_SKY_BACKUP_PATH] = GCP_CONFIG_SKY_BACKUP_PATH
         return credentials
 
     @classmethod
     @functools.lru_cache(maxsize=1)  # Cache since getting identity is slow.
-    def get_current_user_identity(cls) -> Optional[str]:
+    def get_current_user_identity(cls) -> Optional[List[str]]:
         """Returns the email address + project id of the active user."""
         try:
             account = _run_output('gcloud auth list --filter=status:ACTIVE '
                                   '--format="value(account)"')
         except subprocess.CalledProcessError as e:
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.CloudUserIdentityError(
@@ -623,23 +631,24 @@
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.CloudUserIdentityError(
                     'No GCP account is activated. Try running `gcloud '
                     'auth list --filter=status:ACTIVE '
                     '--format="value(account)"` and ensure it correctly '
                     'returns the current user.')
         try:
-            return f'{account} [project_id={cls.get_project_id()}]'
+            project_id = cls.get_project_id()
         except Exception as e:  # pylint: disable=broad-except
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.CloudUserIdentityError(
                     f'Failed to get GCP user identity with unknown '
                     f'exception.\n'
                     '  Reason: '
                     f'{common_utils.format_exception(e, use_bracket=True)}'
                 ) from e
+        return [f'{account} [project_id={project_id}]']
 
     def instance_type_exists(self, instance_type):
         return service_catalog.instance_type_exists(instance_type, 'gcp')
 
     def accelerator_in_region_or_zone(self,
                                       accelerator: str,
                                       acc_count: int,
@@ -682,7 +691,22 @@
     @staticmethod
     def check_accelerator_attachable_to_host(
             instance_type: str,
             accelerators: Optional[Dict[str, int]],
             zone: Optional[str] = None) -> None:
         service_catalog.check_accelerator_attachable_to_host(
             instance_type, accelerators, zone, 'gcp')
+
+    @classmethod
+    def check_disk_tier_enabled(cls, instance_type: str,
+                                disk_tier: str) -> None:
+        del instance_type, disk_tier  # unused
+
+    @classmethod
+    def _get_disk_type(cls, disk_tier: Optional[str]) -> str:
+        tier = disk_tier or cls._DEFAULT_DISK_TIER
+        tier2name = {
+            'high': 'pd-ssd',
+            'medium': 'pd-balanced',
+            'low': 'pd-standard',
+        }
+        return tier2name[tier]
```

### Comparing `skypilot-0.2.5/sky/clouds/lambda_cloud.py` & `skypilot-0.3.0/sky/clouds/lambda_cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Lambda Cloud."""
 import json
 import typing
 from typing import Dict, Iterator, List, Optional, Tuple
 
 from sky import clouds
+from sky import exceptions
 from sky.clouds import service_catalog
 from sky.skylet.providers.lambda_cloud import lambda_utils
 
 if typing.TYPE_CHECKING:
     # Renaming to avoid shadowing variables.
     from sky import resources as resources_lib
 
@@ -110,17 +111,19 @@
         # Returns true if the two clouds are the same cloud type.
         return isinstance(other, Lambda)
 
     @classmethod
     def get_default_instance_type(
             cls,
             cpus: Optional[str] = None,
-            memory: Optional[str] = None) -> Optional[str]:
+            memory: Optional[str] = None,
+            disk_tier: Optional[str] = None) -> Optional[str]:
         return service_catalog.get_default_instance_type(cpus=cpus,
                                                          memory=memory,
+                                                         disk_tier=disk_tier,
                                                          clouds='lambda')
 
     @classmethod
     def get_accelerators_from_instance_type(
         cls,
         instance_type: str,
     ) -> Optional[Dict[str, int]]:
@@ -155,15 +158,15 @@
             'instance_type': resources.instance_type,
             'custom_resources': custom_resources,
             'region': region.name,
         }
 
     def get_feasible_launchable_resources(self,
                                           resources: 'resources_lib.Resources'):
-        if resources.use_spot:
+        if resources.use_spot or resources.disk_tier is not None:
             return ([], [])
         if resources.instance_type is not None:
             assert resources.is_launchable(), resources
             # Accelerators are part of the instance type in Lambda Cloud
             resources = resources.copy(accelerators=None)
             return ([resources], [])
 
@@ -183,15 +186,17 @@
             return resource_list
 
         # Currently, handle a filter on accelerators only.
         accelerators = resources.accelerators
         if accelerators is None:
             # Return a default instance type with the given number of vCPUs.
             default_instance_type = Lambda.get_default_instance_type(
-                cpus=resources.cpus, memory=resources.memory)
+                cpus=resources.cpus,
+                memory=resources.memory,
+                disk_tier=resources.disk_tier)
             if default_instance_type is None:
                 return ([], [])
             else:
                 return (_make([default_instance_type]), [])
 
         assert len(accelerators) == 1, resources
         acc, acc_count = list(accelerators.items())[0]
@@ -225,15 +230,15 @@
     def get_credential_file_mounts(self) -> Dict[str, str]:
         return {
             f'~/.lambda_cloud/{filename}': f'~/.lambda_cloud/{filename}'
             for filename in _CREDENTIAL_FILES
         }
 
     @classmethod
-    def get_current_user_identity(cls) -> Optional[str]:
+    def get_current_user_identity(cls) -> Optional[List[str]]:
         # TODO(ewzeng): Implement get_current_user_identity for Lambda
         return None
 
     def instance_type_exists(self, instance_type: str) -> bool:
         return service_catalog.instance_type_exists(instance_type, 'lambda')
 
     def validate_region_zone(self, region: Optional[str], zone: Optional[str]):
@@ -248,7 +253,13 @@
                                       zone: Optional[str] = None) -> bool:
         return service_catalog.accelerator_in_region_or_zone(
             accelerator, acc_count, region, zone, 'lambda')
 
     @classmethod
     def regions(cls) -> List['clouds.Region']:
         return service_catalog.regions(clouds='lambda')
+
+    @classmethod
+    def check_disk_tier_enabled(cls, instance_type: str,
+                                disk_tier: str) -> None:
+        raise exceptions.NotSupportedError(
+            'Lambda does not support disk tiers.')
```

### Comparing `skypilot-0.2.5/sky/clouds/local.py` & `skypilot-0.3.0/sky/clouds/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Local/On-premise."""
 import subprocess
 import typing
 from typing import Dict, Iterator, List, Optional, Tuple
 
 from sky import clouds
+from sky import exceptions
 
 if typing.TYPE_CHECKING:
     # Renaming to avoid shadowing variables.
     from sky import resources as resources_lib
 
 
 def _run_output(cmd):
@@ -106,17 +107,18 @@
     def is_same_cloud(self, other: clouds.Cloud) -> bool:
         # Returns true if the two clouds are the same cloud type.
         return isinstance(other, Local)
 
     @classmethod
     def get_default_instance_type(cls,
                                   cpus: Optional[str] = None,
-                                  memory: Optional[str] = None) -> str:
+                                  memory: Optional[str] = None,
+                                  disk_tier: Optional[str] = None) -> str:
         # There is only "1" instance type for local cloud: on-prem
-        del cpus, memory  # Unused.
+        del cpus, memory, disk_tier  # Unused.
         return Local._DEFAULT_INSTANCE_TYPE
 
     @classmethod
     def get_vcpus_mem_from_instance_type(
             cls, instance_type: str) -> Tuple[Optional[float], Optional[float]]:
         return None, None
 
@@ -138,14 +140,16 @@
             self, resources: 'resources_lib.Resources',
             region: Optional['clouds.Region'],
             zones: Optional[List['clouds.Zone']]) -> Dict[str, Optional[str]]:
         return {}
 
     def get_feasible_launchable_resources(self,
                                           resources: 'resources_lib.Resources'):
+        if resources.disk_tier is not None:
+            return ([], [])
         # The entire local cluster's resources is considered launchable, as the
         # check for task resources is deferred later.
         # The check for task resources meeting cluster resources is run in
         # cloud_vm_ray_backend._check_task_resources_smaller_than_cluster.
         resources = resources.copy(
             instance_type=Local.get_default_instance_type(),
             # Setting this to None as AWS doesn't separately bill /
@@ -189,7 +193,13 @@
         # Returns true if the region name is same as Local cloud's
         # one and only region: 'Local'.
         assert zone is None
         if region is None or region != Local.LOCAL_REGION.name:
             raise ValueError(f'Region {region!r} does not match the Local'
                              ' cloud region {Local.LOCAL_REGION.name!r}.')
         return region, zone
+
+    @classmethod
+    def check_disk_tier_enabled(cls, instance_type: str,
+                                disk_tier: str) -> None:
+        raise exceptions.NotSupportedError(
+            'Local cloud does not support disk tiers.')
```

### Comparing `skypilot-0.2.5/sky/clouds/service_catalog/__init__.py` & `skypilot-0.3.0/sky/clouds/service_catalog/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from sky.clouds.service_catalog.config import use_default_catalog
 
 if typing.TYPE_CHECKING:
     from sky.clouds import cloud
     from sky.clouds.service_catalog import common
 
 CloudFilter = Optional[Union[List[str], str]]
-_ALL_CLOUDS = ('aws', 'azure', 'gcp', 'lambda')
+_ALL_CLOUDS = ('aws', 'azure', 'gcp', 'ibm', 'lambda')
 
 
 def _map_clouds_catalog(clouds: CloudFilter, method_name: str, *args, **kwargs):
     if clouds is None:
         clouds = list(_ALL_CLOUDS)
     single = isinstance(clouds, str)
     if single:
@@ -48,50 +48,54 @@
 
 
 @use_default_catalog
 def list_accelerators(
     gpus_only: bool = True,
     name_filter: Optional[str] = None,
     region_filter: Optional[str] = None,
+    quantity_filter: Optional[int] = None,
     clouds: CloudFilter = None,
     case_sensitive: bool = True,
 ) -> 'Dict[str, List[common.InstanceTypeInfo]]':
     """List the names of all accelerators offered by Sky.
 
     This will include all accelerators offered by Sky, including those
     that may not be available in the user's account.
 
     Returns: A dictionary of canonical accelerator names mapped to a list
     of instance type offerings. See usage in cli.py.
     """
     results = _map_clouds_catalog(clouds, 'list_accelerators', gpus_only,
-                                  name_filter, region_filter, case_sensitive)
+                                  name_filter, region_filter, quantity_filter,
+                                  case_sensitive)
     if not isinstance(results, list):
         results = [results]
     ret: Dict[str,
               List['common.InstanceTypeInfo']] = collections.defaultdict(list)
     for result in results:
         for gpu, items in result.items():
             ret[gpu] += items
     return dict(ret)
 
 
 def list_accelerator_counts(
     gpus_only: bool = True,
     name_filter: Optional[str] = None,
     region_filter: Optional[str] = None,
+    quantity_filter: Optional[int] = None,
     clouds: CloudFilter = None,
 ) -> Dict[str, List[int]]:
     """List all accelerators offered by Sky and available counts.
 
     Returns: A dictionary of canonical accelerator names mapped to a list
     of available counts. See usage in cli.py.
     """
     results = _map_clouds_catalog(clouds, 'list_accelerators', gpus_only,
-                                  name_filter, region_filter, False)
+                                  name_filter, region_filter, quantity_filter,
+                                  False)
     if not isinstance(results, list):
         results = [results]
     accelerator_counts: Dict[str, Set[int]] = collections.defaultdict(set)
     for result in results:
         for gpu, items in result.items():
             for item in items:
                 accelerator_counts[gpu].add(item.accelerator_count)
@@ -170,28 +174,29 @@
     """Returns the number of virtual CPUs from a instance type."""
     return _map_clouds_catalog(clouds, 'get_vcpus_mem_from_instance_type',
                                instance_type)
 
 
 def get_default_instance_type(cpus: Optional[str] = None,
                               memory: Optional[str] = None,
+                              disk_tier: Optional[str] = None,
                               clouds: CloudFilter = None) -> Optional[str]:
     """Returns the cloud's default instance type for given #vCPUs and memory.
 
     For example, if cpus='4', this method returns the default instance type
     with 4 vCPUs.  If cpus='4+', this method returns the default instance
     type with 4 or more vCPUs.
 
     If memory_gb_or_ratio is not specified, this method returns the General
     Purpose instance type with the given number of vCPUs. If memory_gb_or_ratio
     is specified, this method returns the cheapest instance type that meets
     the given CPU and memory requirement.
     """
     return _map_clouds_catalog(clouds, 'get_default_instance_type', cpus,
-                               memory)
+                               memory, disk_tier)
 
 
 def get_accelerators_from_instance_type(
         instance_type: str,
         clouds: CloudFilter = None) -> Optional[Dict[str, int]]:
     """Returns the accelerators from a instance type."""
     return _map_clouds_catalog(clouds, 'get_accelerators_from_instance_type',
@@ -284,15 +289,24 @@
     _map_clouds_catalog(clouds, 'check_accelerator_attachable_to_host',
                         instance_type, accelerators, zone)
 
 
 def get_common_gpus() -> List[str]:
     """Returns a list of commonly used GPU names."""
     return [
-        'V100', 'V100-32GB', 'A100', 'A100-80GB', 'P100', 'K80', 'T4', 'M60'
+        'A10',
+        'A10G',
+        'A100',
+        'A100-80GB',
+        'K80',
+        'M60',
+        'P100',
+        'T4',
+        'V100',
+        'V100-32GB',
     ]
 
 
 def get_tpus() -> List[str]:
     """Returns a list of TPU names."""
     # TODO(wei-lin): refactor below hard-coded list.
     return [
```

### Comparing `skypilot-0.2.5/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-0.3.0/sky/clouds/service_catalog/aws_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,17 @@
     not supported by the user account.
 
     Returns:
         A dataframe with column 'AvailabilityZone' that's correctly replaced
         with the zone name (e.g. us-east-1a).
     """
     try:
-        user_identity = aws.AWS.get_current_user_identity()
-        assert user_identity is not None, 'user_identity is None'
+        user_identity_list = aws.AWS.get_current_user_identity()
+        assert user_identity_list, user_identity_list
+        user_identity = user_identity_list[0]
         aws_user_hash = hashlib.md5(user_identity.encode()).hexdigest()[:8]
     except exceptions.CloudUserIdentityError:
         glob_name = common.get_catalog_path('aws/az_mappings-*.csv')
         # Find the most recent file that matches the glob.
         # We check the existing files because the user could remove the
         # credentials after a cluster is created. Using the latest mapping
         # file is better than using the default mapping file because the
@@ -176,15 +177,17 @@
 def get_vcpus_mem_from_instance_type(
         instance_type: str) -> Tuple[Optional[float], Optional[float]]:
     return common.get_vcpus_mem_from_instance_type_impl(_get_df(),
                                                         instance_type)
 
 
 def get_default_instance_type(cpus: Optional[str] = None,
-                              memory: Optional[str] = None) -> Optional[str]:
+                              memory: Optional[str] = None,
+                              disk_tier: Optional[str] = None) -> Optional[str]:
+    del disk_tier  # unused
     if cpus is None and memory is None:
         cpus = f'{_DEFAULT_NUM_VCPUS}+'
 
     if memory is None:
         memory_gb_or_ratio = f'{_DEFAULT_MEMORY_CPU_RATIO}x'
     else:
         memory_gb_or_ratio = memory
@@ -242,20 +245,21 @@
     return us_region_list + other_region_list
 
 
 def list_accelerators(
         gpus_only: bool,
         name_filter: Optional[str],
         region_filter: Optional[str],
+        quantity_filter: Optional[int],
         case_sensitive: bool = True
 ) -> Dict[str, List[common.InstanceTypeInfo]]:
     """Returns all instance types in AWS offering accelerators."""
     return common.list_accelerators_impl('AWS', _get_df(), gpus_only,
                                          name_filter, region_filter,
-                                         case_sensitive)
+                                         quantity_filter, case_sensitive)
 
 
 def get_image_id_from_tag(tag: str, region: Optional[str]) -> Optional[str]:
     """Returns the image id from the tag."""
     return common.get_image_id_from_tag_impl(_image_df, tag, region)
```

### Comparing `skypilot-0.2.5/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-0.3.0/sky/clouds/service_catalog/azure_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 This module loads the service catalog file and can be used to query
 instance types and pricing information for Azure.
 """
 import re
 from typing import Dict, List, Optional, Tuple
 
 from sky import clouds as cloud_lib
+from sky.clouds import Azure
 from sky.clouds.service_catalog import common
 from sky.utils import ux_utils
 
 _df = common.read_catalog('azure/vms.csv')
 
 # We will select from the following three instance families:
 _DEFAULT_INSTANCE_FAMILY = [
     # The latest general-purpose instance family as of Mar. 2023.
     # CPU: Intel Ice Lake 8370C.
     # Memory: 4 GiB RAM per 1 vCPU;
-    'D_v5',
+    'Ds_v5',
     # The latest memory-optimized instance family as of Mar. 2023.
     # CPU: Intel Ice Lake 8370C.
     # Memory: 8 GiB RAM per 1 vCPU.
-    'E_v5',
+    'Es_v5',
     # The latest compute-optimized instance family as of Mar 2023.
     # CPU: Intel Ice Lake 8370C, Cascade Lake 8272CL, or Skylake 8168.
     # Memory: 2 GiB RAM per 1 vCPU.
     'Fs_v2'
 ]
 _DEFAULT_NUM_VCPUS = 8
 _DEFAULT_MEMORY_CPU_RATIO = 4
@@ -93,23 +94,29 @@
         x = re.match(r'([A-Za-z]+)([0-9]+)(.*)', instance_type)
         assert x is not None, x
         instance_family = x.group(1) + x.group(3)
     return instance_family
 
 
 def get_default_instance_type(cpus: Optional[str] = None,
-                              memory: Optional[str] = None) -> Optional[str]:
+                              memory: Optional[str] = None,
+                              disk_tier: Optional[str] = None) -> Optional[str]:
     if cpus is None and memory is None:
         cpus = f'{_DEFAULT_NUM_VCPUS}+'
     if memory is None:
         memory_gb_or_ratio = f'{_DEFAULT_MEMORY_CPU_RATIO}x'
     else:
         memory_gb_or_ratio = memory
     df = _df[_df['InstanceType'].apply(_get_instance_family).isin(
         _DEFAULT_INSTANCE_FAMILY)]
+
+    def _filter_disk_type(instance_type: str) -> bool:
+        return Azure.check_disk_tier(instance_type, disk_tier)[0]
+
+    df = df.loc[df['InstanceType'].apply(_filter_disk_type)]
     return common.get_instance_type_for_cpus_mem_impl(df, cpus,
                                                       memory_gb_or_ratio)
 
 
 def get_accelerators_from_instance_type(
         instance_type: str) -> Optional[Dict[str, int]]:
     return common.get_accelerators_from_instance_type_impl(_df, instance_type)
@@ -150,12 +157,14 @@
     return _df[_df['InstanceType'] == instance_type]['Generation'].iloc[0]
 
 
 def list_accelerators(
         gpus_only: bool,
         name_filter: Optional[str],
         region_filter: Optional[str],
+        quantity_filter: Optional[int],
         case_sensitive: bool = True
 ) -> Dict[str, List[common.InstanceTypeInfo]]:
     """Returns all instance types in Azure offering GPUs."""
     return common.list_accelerators_impl('Azure', _df, gpus_only, name_filter,
-                                         region_filter, case_sensitive)
+                                         region_filter, quantity_filter,
+                                         case_sensitive)
```

### Comparing `skypilot-0.2.5/sky/clouds/service_catalog/common.py` & `skypilot-0.3.0/sky/clouds/service_catalog/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common utilities for service catalog."""
+import ast
 import hashlib
 import os
 import time
 from typing import Dict, List, NamedTuple, Optional, Tuple
 
 import difflib
 import filelock
@@ -27,24 +28,26 @@
 
     - cloud: Cloud name.
     - instance_type: String that can be used in YAML to specify this instance
       type. E.g. `p3.2xlarge`.
     - accelerator_name: Canonical name of the accelerator. E.g. `V100`.
     - accelerator_count: Number of accelerators offered by this instance type.
     - cpu_count: Number of vCPUs offered by this instance type.
+    - device_memory: Device memory in GiB.
     - memory: Instance memory in GiB.
     - price: Regular instance price per hour (cheapest across all regions).
     - spot_price: Spot instance price per hour (cheapest across all regions).
     - region: Region where this instance type belongs to.
     """
     cloud: str
     instance_type: Optional[str]
     accelerator_name: str
     accelerator_count: int
     cpu_count: Optional[float]
+    device_memory: Optional[float]
     memory: Optional[float]
     price: float
     spot_price: float
     region: str
 
 
 def get_catalog_path(filename: str) -> str:
@@ -174,16 +177,16 @@
         if len(candidate_loc) > 0:
             candidate_strs = ', '.join(candidate_loc)
             candidate_strs = f'\nDid you mean one of these: {candidate_strs!r}?'
         return candidate_strs
 
     def _get_all_supported_regions_str() -> str:
         all_regions: List[str] = sorted(df['Region'].unique().tolist())
-        return \
-        f'\nList of supported {cloud_name} regions: {", ".join(all_regions)!r}'
+        return (f'\nList of supported {cloud_name} regions: '
+                f'{", ".join(all_regions)!r}')
 
     validated_region, validated_zone = region, zone
 
     filter_df = df
     if region is not None:
         filter_df = filter_df[filter_df['Region'] == region]
         if len(filter_df) == 0:
@@ -419,45 +422,61 @@
 
 def list_accelerators_impl(
     cloud: str,
     df: pd.DataFrame,
     gpus_only: bool,
     name_filter: Optional[str],
     region_filter: Optional[str],
+    quantity_filter: Optional[int],
     case_sensitive: bool = True,
 ) -> Dict[str, List[InstanceTypeInfo]]:
     """Lists accelerators offered in a cloud service catalog.
 
     `name_filter` is a regular expression used to filter accelerator names
     using pandas.Series.str.contains.
 
     Returns a mapping from the canonical names of accelerators to a list of
     instance types offered by this cloud.
     """
     if gpus_only:
         df = df[~df['GpuInfo'].isna()]
+    df = df.copy()  # avoid column assignment warning
+
+    try:
+        gpu_info_df = df['GpuInfo'].apply(ast.literal_eval)
+        df['DeviceMemoryGiB'] = gpu_info_df.apply(
+            lambda row: row['Gpus'][0]['MemoryInfo']['SizeInMiB']) / 1024.0
+    except ValueError:
+        # TODO(zongheng,woosuk): GCP/Azure catalogs do not have well-formed
+        # GpuInfo fields. So the above will throw:
+        #  ValueError: malformed node or string: <_ast.Name object at ..>
+        df['DeviceMemoryGiB'] = None
+
     df = df[[
         'InstanceType',
         'AcceleratorName',
         'AcceleratorCount',
         'vCPUs',
-        'MemoryGiB',
+        'DeviceMemoryGiB',  # device memory
+        'MemoryGiB',  # host memory
         'Price',
         'SpotPrice',
         'Region',
     ]].dropna(subset=['AcceleratorName']).drop_duplicates()
     if name_filter is not None:
         df = df[df['AcceleratorName'].str.contains(name_filter,
                                                    case=case_sensitive,
                                                    regex=True)]
     if region_filter is not None:
         df = df[df['Region'].str.contains(region_filter,
                                           case=case_sensitive,
                                           regex=True)]
     df['AcceleratorCount'] = df['AcceleratorCount'].astype(int)
+    if quantity_filter is not None:
+        df = df[df['AcceleratorCount'] == quantity_filter]
     grouped = df.groupby('AcceleratorName')
 
     def make_list_from_df(rows):
         # Only keep the lowest prices across regions.
         rows = rows.groupby([
             'InstanceType', 'AcceleratorName', 'AcceleratorCount', 'vCPUs',
             'MemoryGiB'
@@ -466,14 +485,15 @@
         ret = rows.apply(
             lambda row: InstanceTypeInfo(
                 cloud,
                 row['InstanceType'],
                 row['AcceleratorName'],
                 row['AcceleratorCount'],
                 row['vCPUs'],
+                row['DeviceMemoryGiB'],
                 row['MemoryGiB'],
                 row['Price'],
                 row['SpotPrice'],
                 row['Region'],
             ),
             axis='columns',
         ).tolist()
```

### Comparing `skypilot-0.2.5/sky/clouds/service_catalog/config.py` & `skypilot-0.3.0/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 This script takes about 1 minute to finish.
 """
 import argparse
 import datetime
 import itertools
 from multiprocessing import pool as mp_pool
 import os
+import sys
 import subprocess
 from typing import Dict, List, Optional, Set, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from sky.adaptors import aws
+from sky.utils import ux_utils
 
 # Enable most of the regions. Each user's account may have a subset of these
 # enabled; this is ok because we take the intersection of the list here with
 # the user-specific enabled regions in `aws_catalog`, via the "availability
 # zone mapping".
 # TODO(zhwu): fix the regions with no supported AMI (maybe by finding AMIs
 # similar to the Deep Learning AMI).
@@ -55,24 +57,40 @@
     'GpuInfo', 'Price', 'SpotPrice', 'Region', 'AvailabilityZone'
 ]
 
 # NOTE: the hard-coded us-east-1 URL is not a typo. AWS pricing endpoint is
 # only available in this region, but it serves pricing information for all
 # regions.
 PRICING_TABLE_URL_FMT = 'https://pricing.us-east-1.amazonaws.com/offers/v1.0/aws/AmazonEC2/current/{region}/index.csv'  # pylint: disable=line-too-long
+# Hardcode the regions that offer p4de.24xlarge as our credential does not have
+# the permission to query the offerings of the instance.
+# Ref: https://aws.amazon.com/ec2/instance-types/p4/
+P4DE_REGIONS = ['us-east-1', 'us-west-2']
 
 regions_enabled: Optional[Set[str]] = None
 
 
 def get_enabled_regions() -> Set[str]:
     # Should not be called concurrently.
     global regions_enabled
     if regions_enabled is None:
         aws_client = aws.client('ec2', region_name='us-east-1')
-        user_cloud_regions = aws_client.describe_regions()['Regions']
+        try:
+            user_cloud_regions = aws_client.describe_regions()['Regions']
+        except aws.botocore_exceptions().ClientError as e:
+            if e.response['Error']['Code'] == 'UnauthorizedOperation':
+                with ux_utils.print_exception_no_traceback():
+                    raise RuntimeError(
+                        'Failed to retrieve AWS regions. '
+                        'Please ensure that the `ec2:DescribeRegions` action '
+                        'is enabled for your AWS account in IAM. '
+                        'Ref: https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeRegions.html'  # pylint: disable=line-too-long
+                    ) from None
+            else:
+                raise
         regions_enabled = {r['RegionName'] for r in user_cloud_regions}
         regions_enabled = regions_enabled.intersection(set(ALL_REGIONS))
     return regions_enabled
 
 
 def _get_instance_types(region: str) -> pd.DataFrame:
     client = aws.client('ec2', region_name=region)
@@ -99,22 +117,33 @@
 
 
 def _get_availability_zones(region: str) -> Optional[pd.DataFrame]:
     client = aws.client('ec2', region_name=region)
     zones = []
     try:
         response = client.describe_availability_zones()
-    except aws.botocore_exceptions().ClientError:
-        # The user's AWS account may not have access to this region.
-        # The error looks like:
-        # botocore.exceptions.ClientError: An error occurred
-        # (AuthFailure) when calling the DescribeAvailabilityZones
-        # operation: AWS was not able to validate the provided
-        # access credentials
-        return None
+    except aws.botocore_exceptions().ClientError as e:
+        if e.response['Error']['Code'] == 'AuthFailure':
+            # The user's AWS account may not have access to this region.
+            # The error looks like:
+            # botocore.exceptions.ClientError: An error occurred
+            # (AuthFailure) when calling the DescribeAvailabilityZones
+            # operation: AWS was not able to validate the provided
+            # access credentials
+            return None
+        elif e.response['Error']['Code'] == 'UnauthorizedOperation':
+            with ux_utils.print_exception_no_traceback():
+                raise RuntimeError(
+                    'Failed to retrieve availability zone. '
+                    'Please ensure that the `ec2:DescribeAvailabilityZones` '
+                    'action is enabled for your AWS account in IAM. '
+                    'Ref: https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeAvailabilityZones.html'  # pylint: disable=line-too-long
+                ) from None
+        else:
+            raise
     for resp in response['AvailabilityZones']:
         zones.append({
             'AvailabilityZoneName': resp['ZoneName'],
             'AvailabilityZone': resp['ZoneId'],
         })
     return pd.DataFrame(zones)
 
@@ -162,14 +191,43 @@
         ret = ret + response['SpotPriceHistory']
     df = pd.DataFrame(ret)[['InstanceType', 'AvailabilityZone', 'SpotPrice']]
     df = df.rename(columns={'AvailabilityZone': 'AvailabilityZoneName'})
     df = df.set_index(['InstanceType', 'AvailabilityZoneName'])
     return df
 
 
+def _patch_p4de(region: str, df: pd.DataFrame,
+                pricing_df: pd.DataFrame) -> pd.DataFrame:
+    # Hardcoded patch for p4de.24xlarge, as our credentials doesn't have access
+    # to the instance type.
+    # Columns:
+    # InstanceType,AcceleratorName,AcceleratorCount,vCPUs,MemoryGiB,GpuInfo,
+    # Price,SpotPrice,Region,AvailabilityZone
+    records = []
+    for zone in df[df['Region'] == region]['AvailabilityZone'].unique():
+        records.append({
+            'InstanceType': 'p4de.24xlarge',
+            'AcceleratorName': 'A100-80GB',
+            'AcceleratorCount': 8,
+            'vCPUs': 96,
+            'MemoryGiB': 1152,
+            'GpuInfo':
+                ('{\'Gpus\': [{\'Name\': \'A100-80GB\', \'Manufacturer\': '
+                 '\'NVIDIA\', \'Count\': 8, \'MemoryInfo\': {\'SizeInMiB\': '
+                 '81920}}], \'TotalGpuMemoryInMiB\': 655360}'),
+            'AvailabilityZone': zone,
+            'Region': region,
+            'Price': pricing_df[pricing_df['InstanceType'] == 'p4de.24xlarge']
+                     ['Price'].values[0],
+            'SpotPrice': np.nan,
+        })
+    df = pd.concat([df, pd.DataFrame.from_records(records)])
+    return df
+
+
 def _get_instance_types_df(region: str) -> Union[str, pd.DataFrame]:
     try:
         # Fetch the zone info first to make sure the account has access to the
         # region.
         zone_df = _get_availability_zones(region)
         if zone_df is None:
             raise RuntimeError(f'No access to region {region}')
@@ -243,19 +301,22 @@
                       right_index=True,
                       how='outer')
 
         # Extract vCPUs, memory, and accelerator info from the columns.
         df = pd.concat(
             [df, df.apply(get_additional_columns, axis='columns')],
             axis='columns')
-        # patch the GpuInfo for p4de.24xlarge
-        df.loc[df['InstanceType'] == 'p4de.24xlarge', 'GpuInfo'] = 'A100-80GB'
+        # patch the df for p4de.24xlarge
+        if region in P4DE_REGIONS:
+            df = _patch_p4de(region, df, pricing_df)
+        if 'GpuInfo' not in df.columns:
+            df['GpuInfo'] = np.nan
         df = df[USEFUL_COLUMNS]
     except Exception as e:  # pylint: disable=broad-except
-        print(f'{region} failed with {e}')
+        print(f'{region} failed with {e}', file=sys.stderr)
         return region
     return df
 
 
 def get_all_regions_instance_types_df(regions: Set[str]) -> pd.DataFrame:
     with mp_pool.Pool() as pool:
         df_or_regions = pool.map(_get_instance_types_df, regions)
@@ -263,15 +324,15 @@
     for df_or_region in df_or_regions:
         if isinstance(df_or_region, str):
             print(f'{df_or_region} failed')
         else:
             new_dfs.append(df_or_region)
 
     df = pd.concat(new_dfs)
-    df.sort_values(['InstanceType', 'Region'], inplace=True)
+    df.sort_values(['InstanceType', 'Region', 'AvailabilityZone'], inplace=True)
     return df
 
 
 # Fetch Images
 # https://console.aws.amazon.com/ec2/v2/home?region=us-east-1#Images:visibility=public-images;v=3;search=:64,:Ubuntu%2020,:Deep%20Learning%20AMI%20GPU%20PyTorch # pylint: disable=line-too-long
 # Current AMIs (we have to use different PyTorch versions for different OS as Ubuntu 18.04
 # does not have the latest PyTorch version):
@@ -398,17 +459,18 @@
         # guard against network issues or glitches in the AWS API.
         fetched_regions = set(df['Region'].unique())
         if fetched_regions != user_regions:
             # This is a sanity check to make sure that the regions we
             # requested are the same as the ones we fetched.
             # The mismatch could happen for network issues or glitches
             # in the AWS API.
+            diff = user_regions - fetched_regions
             raise RuntimeError(
                 f'{name}: Fetched regions {fetched_regions} does not match '
-                f'requested regions {user_regions}.')
+                f'requested regions {user_regions}; Diff: {diff}')
 
     instance_df = get_all_regions_instance_types_df(user_regions)
     _check_regions_integrity(instance_df, 'instance types')
 
     os.makedirs('aws', exist_ok=True)
     instance_df.to_csv('aws/vms.csv', index=False)
     print('AWS Service Catalog saved to aws/vms.csv')
```

### Comparing `skypilot-0.2.5/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,21 @@
     'southcentralus',
     'westcentralus',
     'westus',
     'westus2',
     # 'WestUS3',   # WestUS3 pricing table is broken as of 2021/11.
 ]
 
+# Exclude the following regions as they do not have ProductName in the
+# pricing table. Reference: #1768
+EXCLUDED_REGIONS = {
+    'eastus2euap',
+    'centraluseuap',
+}
+
 
 def get_regions() -> List[str]:
     """Get all available regions."""
     proc = subprocess.run(
         'az account list-locations  --query "[?not_null(metadata.latitude)] '
         '.{RegionName:name , RegionDisplayName:regionalDisplayName}" -o json',
         shell=True,
@@ -238,13 +245,13 @@
     parser.add_argument(
         '--all-regions',
         action='store_true',
         help='Fetch all global regions, not just the U.S. ones.')
     args = parser.parse_args()
 
     region_filter = get_regions() if args.all_regions else US_REGIONS
-    region_filter = set(region_filter)
+    region_filter = set(region_filter) - EXCLUDED_REGIONS
 
     instance_df = get_all_regions_instance_types_df(region_filter)
     os.makedirs('azure', exist_ok=True)
     instance_df.to_csv('azure/vms.csv', index=False)
     print('Azure Service Catalog saved to azure/vms.csv')
```

### Comparing `skypilot-0.2.5/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-0.3.0/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,17 @@
     # officially documented.
     if instance_type == 'TPU-VM':
         return None, None
     return common.get_vcpus_mem_from_instance_type_impl(_df, instance_type)
 
 
 def get_default_instance_type(cpus: Optional[str] = None,
-                              memory: Optional[str] = None) -> Optional[str]:
+                              memory: Optional[str] = None,
+                              disk_tier: Optional[str] = None) -> Optional[str]:
+    del disk_tier  # unused
     if cpus is None and memory is None:
         cpus = f'{_DEFAULT_NUM_VCPUS}+'
     if memory is None:
         memory_gb_or_ratio = f'{_DEFAULT_MEMORY_CPU_RATIO}x'
     else:
         memory_gb_or_ratio = memory
     instance_type_prefix = tuple(
@@ -318,19 +320,21 @@
     return cheapest['SpotPrice']
 
 
 def list_accelerators(
     gpus_only: bool,
     name_filter: Optional[str] = None,
     region_filter: Optional[str] = None,
+    quantity_filter: Optional[int] = None,
     case_sensitive: bool = True,
 ) -> Dict[str, List[common.InstanceTypeInfo]]:
     """Returns all instance types in GCP offering GPUs."""
     results = common.list_accelerators_impl('GCP', _df, gpus_only, name_filter,
-                                            region_filter, case_sensitive)
+                                            region_filter, quantity_filter,
+                                            case_sensitive)
 
     a100_infos = results.get('A100', []) + results.get('A100-80GB', [])
     if not a100_infos:
         return results
 
     # Unlike other GPUs that can be attached to different sizes of N1 VMs,
     # A100 GPUs can only be attached to fixed-size A2 VMs.
```

### Comparing `skypilot-0.2.5/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-0.3.0/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,17 @@
 
 def get_vcpus_mem_from_instance_type(
         instance_type: str) -> Tuple[Optional[float], Optional[float]]:
     return common.get_vcpus_mem_from_instance_type_impl(_df, instance_type)
 
 
 def get_default_instance_type(cpus: Optional[str] = None,
-                              memory: Optional[str] = None) -> Optional[str]:
+                              memory: Optional[str] = None,
+                              disk_tier: Optional[str] = None) -> Optional[str]:
+    del disk_tier  # unused
     if cpus is None and memory is None:
         cpus = f'{_DEFAULT_NUM_VCPUS}+'
     if memory is None:
         memory_gb_or_ratio = f'{_DEFAULT_MEMORY_CPU_RATIO}x'
     else:
         memory_gb_or_ratio = memory
     return common.get_instance_type_for_cpus_mem_impl(_df, cpus,
@@ -122,12 +124,14 @@
     return us_region_list + other_region_list
 
 
 def list_accelerators(
         gpus_only: bool,
         name_filter: Optional[str],
         region_filter: Optional[str],
+        quantity_filter: Optional[int],
         case_sensitive: bool = True
 ) -> Dict[str, List[common.InstanceTypeInfo]]:
     """Returns all instance types in Lambda offering GPUs."""
     return common.list_accelerators_impl('Lambda', _df, gpus_only, name_filter,
-                                         region_filter, case_sensitive)
+                                         region_filter, quantity_filter,
+                                         case_sensitive)
```

### Comparing `skypilot-0.2.5/sky/core.py` & `skypilot-0.3.0/sky/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """SDK functions for cluster/job management."""
 import getpass
 import sys
-from typing import Any, Dict, List, Optional, Sequence, Union
+from typing import Any, Dict, List, Optional, Union
 
 import colorama
 
 from sky import clouds
 from sky import dag
 from sky import task
 from sky import backends
@@ -29,15 +29,15 @@
 # = Cluster Management =
 # ======================
 
 # pylint: disable=redefined-builtin
 
 
 @usage_lib.entrypoint
-def status(cluster_names: Optional[Union[str, Sequence[str]]] = None,
+def status(cluster_names: Optional[Union[str, List[str]]] = None,
            refresh: bool = False) -> List[Dict[str, Any]]:
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
     """Get cluster statuses.
 
     If cluster_names is given, return those clusters. Otherwise, return all
     clusters.
 
@@ -299,38 +299,39 @@
     if cluster_name in backend_utils.SKY_RESERVED_CLUSTER_NAMES:
         raise exceptions.NotSupportedError(
             f'Stopping sky reserved cluster {cluster_name!r} '
             f'is not supported.')
     handle = global_user_state.get_handle_from_cluster_name(cluster_name)
     if handle is None:
         raise ValueError(f'Cluster {cluster_name!r} does not exist.')
-    if tpu_utils.is_tpu_vm_pod(handle.launched_resources):
-        # Reference:
-        # https://cloud.google.com/tpu/docs/managing-tpus-tpu-vm#stopping_a_with_gcloud  # pylint: disable=line-too-long
-        raise exceptions.NotSupportedError(
-            f'Stopping cluster {cluster_name!r} with TPU VM Pod '
-            'is not supported.')
-
-    # Check cloud supports stopping instances
-    cloud = handle.launched_resources.cloud
-    cloud.check_features_are_supported(
-        {clouds.CloudImplementationFeatures.STOP})
 
     backend = backend_utils.get_backend_from_handle(handle)
-    if (isinstance(backend, backends.CloudVmRayBackend) and
-            handle.launched_resources.use_spot):
-        # Disable spot instances to be stopped.
-        # TODO(suquark): enable GCP+spot to be stopped in the future.
-        raise exceptions.NotSupportedError(
-            f'{colorama.Fore.YELLOW}Stopping cluster '
-            f'{cluster_name!r}...skipped.{colorama.Style.RESET_ALL}\n'
-            '  Stopping spot instances is not supported as the attached '
-            'disks will be lost.\n'
-            '  To terminate the cluster instead, run: '
-            f'{colorama.Style.BRIGHT}sky down {cluster_name}')
+
+    if isinstance(backend, backends.CloudVmRayBackend):
+        assert isinstance(handle, backends.CloudVmRayResourceHandle), handle
+        if tpu_utils.is_tpu_vm_pod(handle.launched_resources):
+            # Reference:
+            # https://cloud.google.com/tpu/docs/managing-tpus-tpu-vm#stopping_a_with_gcloud  # pylint: disable=line-too-long
+            raise exceptions.NotSupportedError(
+                f'Stopping cluster {cluster_name!r} with TPU VM Pod '
+                'is not supported.')
+        # Check cloud supports stopping instances
+        cloud = handle.launched_resources.cloud
+        cloud.check_features_are_supported(
+            {clouds.CloudImplementationFeatures.STOP})
+        if handle.launched_resources.use_spot:
+            # Disable spot instances to be stopped.
+            # TODO(suquark): enable GCP+spot to be stopped in the future.
+            raise exceptions.NotSupportedError(
+                f'{colorama.Fore.YELLOW}Stopping cluster '
+                f'{cluster_name!r}... skipped.{colorama.Style.RESET_ALL}\n'
+                '  Stopping spot instances is not supported as the attached '
+                'disks will be lost.\n'
+                '  To terminate the cluster instead, run: '
+                f'{colorama.Style.BRIGHT}sky down {cluster_name}')
     usage_lib.record_cluster_name_for_current_operation(cluster_name)
     backend.teardown(handle, terminate=False, purge=purge)
 
 
 @usage_lib.entrypoint
 def down(cluster_name: str, purge: bool = False) -> None:
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
@@ -346,14 +347,15 @@
 
     Args:
         cluster_name: name of the cluster to down.
         purge: whether to ignore cloud provider errors (if any).
 
     Raises:
         ValueError: the specified cluster does not exist.
+        RuntimeError: failed to tear down the cluster.
         sky.exceptions.NotSupportedError: the specified cluster is the managed
           spot controller.
     """
     handle = global_user_state.get_handle_from_cluster_name(cluster_name)
     if handle is None:
         raise ValueError(f'Cluster {cluster_name!r} does not exist.')
 
@@ -800,15 +802,15 @@
         jobs = list(filter(lambda job: not job['status'].is_terminal(), jobs))
     return jobs
 
 
 @usage_lib.entrypoint
 # pylint: disable=redefined-builtin
 def spot_cancel(name: Optional[str] = None,
-                job_ids: Optional[Sequence[int]] = None,
+                job_ids: Optional[List[int]] = None,
                 all: bool = False) -> None:
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
     """Cancel managed spot jobs.
 
     Please refer to the sky.cli.spot_cancel for the document.
 
     Raises:
```

### Comparing `skypilot-0.2.5/sky/dag.py` & `skypilot-0.3.0/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/data/data_transfer.py` & `skypilot-0.3.0/sky/data/data_transfer.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 - S3 -> Local
 - Local -> GCS
 - GCS -> Local
 - S3 -> GCS
 
 TODO:
 - All combinations of Azure Transfer
+- All combinations of R2 Transfer
 - GCS -> S3
 """
 import json
 import subprocess
 import time
 
 import colorama
@@ -112,27 +113,84 @@
                 'Storage Transfer Service console at '
                 'https://cloud.google.com/storage-transfer-service')
             return
     logger.info(
         f'Transfer finished in {(time.time() - start) / 60:.2f} minutes.')
 
 
+def s3_to_r2(s3_bucket_name: str, r2_bucket_name: str) -> None:
+    """Creates a one-time transfer from Amazon S3 to Google Cloud Storage.
+
+    Can be viewed from: https://console.cloud.google.com/transfer/cloud
+    it will block until the transfer is complete.
+
+    Args:
+      s3_bucket_name: str; Name of the Amazon S3 Bucket
+      r2_bucket_name: str; Name of the Cloudflare R2 Bucket
+    """
+    raise NotImplementedError('Moving data directly from clouds to R2 is '
+                              'currently not supported. Please specify '
+                              'a local source for the storage object.')
+
+
 def gcs_to_s3(gs_bucket_name: str, s3_bucket_name: str) -> None:
     """Creates a one-time transfer from Google Cloud Storage to Amazon S3.
 
      Args:
       gs_bucket_name: str; Name of the Google Cloud Storage Bucket
       s3_bucket_name: str; Name of the Amazon S3 Bucket
     """
     sync_command = (f'gsutil -m rsync -rd gs://{gs_bucket_name} '
                     f's3://{s3_bucket_name}')
 
     subprocess.call(sync_command, shell=True)
 
 
+def gcs_to_r2(gs_bucket_name: str, r2_bucket_name: str) -> None:
+    """Creates a one-time transfer from Google Cloud Storage to Amazon S3.
+
+     Args:
+      gs_bucket_name: str; Name of the Google Cloud Storage Bucket
+      r2_bucket_name: str; Name of the Cloudflare R2 Bucket
+    """
+    raise NotImplementedError('Moving data directly from clouds to R2 is '
+                              'currently not supported. Please specify '
+                              'a local source for the storage object.')
+
+
+def r2_to_gcs(r2_bucket_name: str, gs_bucket_name: str) -> None:
+    """Creates a one-time transfer from Cloudflare R2 to Google Cloud Storage.
+
+    Can be viewed from: https://console.cloud.google.com/transfer/cloud
+    it will block until the transfer is complete.
+
+    Args:
+      r2_bucket_name: str; Name of the Cloudflare R2 Bucket
+      gs_bucket_name: str; Name of the Google Cloud Storage Bucket
+    """
+    raise NotImplementedError('Moving data directly from R2 to clouds is '
+                              'currently not supported. Please specify '
+                              'a local source for the storage object.')
+
+
+def r2_to_s3(r2_bucket_name: str, s3_bucket_name: str) -> None:
+    """Creates a one-time transfer from Amazon S3 to Google Cloud Storage.
+
+    Can be viewed from: https://console.cloud.google.com/transfer/cloud
+    it will block until the transfer is complete.
+
+    Args:
+      r2_bucket_name: str; Name of the Cloudflare R2 Bucket\
+      s3_bucket_name: str; Name of the Amazon S3 Bucket
+    """
+    raise NotImplementedError('Moving data directly from R2 to clouds is '
+                              'currently not supported. Please specify '
+                              'a local source for the storage object.')
+
+
 def _add_bucket_iam_member(bucket_name: str, role: str, member: str) -> None:
     storage_client = gcp.storage_client()
     bucket = storage_client.bucket(bucket_name)
 
     policy = bucket.get_iam_policy(requested_policy_version=3)
     policy.bindings.append({'role': role, 'members': {member}})
```

### Comparing `skypilot-0.2.5/sky/data/data_utils.py` & `skypilot-0.3.0/sky/data/data_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import subprocess
 from typing import Any, Callable, Dict, List, Optional, Tuple
 import urllib.parse
 
 from sky import exceptions
 from sky import sky_logging
-from sky.adaptors import aws, gcp
+from sky.adaptors import aws, gcp, cloudflare
 from sky.utils import ux_utils
 
 Client = Any
 
 logger = sky_logging.init_logger(__name__)
 
 
@@ -36,14 +36,26 @@
     """
     path_parts = gcs_path.replace('gs://', '').split('/')
     bucket = path_parts.pop(0)
     key = '/'.join(path_parts)
     return bucket, key
 
 
+def split_r2_path(r2_path: str) -> Tuple[str, str]:
+    """Splits R2 Path into Bucket name and Relative Path to Bucket
+
+    Args:
+      r2_path: str; R2 Path, e.g. r2://imagenet/train/
+    """
+    path_parts = r2_path.replace('r2://', '').split('/')
+    bucket = path_parts.pop(0)
+    key = '/'.join(path_parts)
+    return bucket, key
+
+
 def create_s3_client(region: str = 'us-east-2') -> Client:
     """Helper method that connects to Boto3 client for S3 Bucket
 
     Args:
       region: str; Region name, e.g. us-west-1, us-east-2
     """
     return aws.client('s3', region_name=region)
@@ -69,14 +81,34 @@
     try:
         gcp.storage_client().get_bucket(name)
         return True
     except gcp.not_found_exception():
         return False
 
 
+def create_r2_client(region: str = 'auto') -> Client:
+    """Helper method that connects to Boto3 client for R2 Bucket
+
+    Args:
+      region: str; Region for CLOUDFLARE R2 is set to auto
+    """
+    return cloudflare.client('s3', region)
+
+
+def verify_r2_bucket(name: str) -> bool:
+    """Helper method that checks if the R2 bucket exists
+
+    Args:
+      name: str; Name of R2 Bucket (without r2:// prefix)
+    """
+    r2 = cloudflare.resource('s3')
+    bucket = r2.Bucket(name)
+    return bucket in r2.buckets.all()
+
+
 def is_cloud_store_url(url):
     result = urllib.parse.urlsplit(url)
     # '' means non-cloud URLs.
     return result.netloc
 
 
 def _group_files_by_dir(
@@ -114,15 +146,15 @@
                     dirsync_command_generator: Callable[[str, str], str],
                     bucket_name: str,
                     access_denied_message: str,
                     create_dirs: bool = False,
                     max_concurrent_uploads: Optional[int] = None) -> None:
     """Helper function to run parallel uploads for a list of paths.
 
-    Used by S3Store and GCSStore to run rsync commands in parallel by
+    Used by S3Store, GCSStore, and R2Store to run rsync commands in parallel by
     providing appropriate command generators.
 
     Args:
         source_path_list: List of paths to local files or directories
         filesync_command_generator: Callable that generates rsync command
             for a list of files belonging to the same dir.
         dirsync_command_generator: Callable that generates rsync command
```

### Comparing `skypilot-0.2.5/sky/data/mounting_utils.py` & `skypilot-0.3.0/sky/data/mounting_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """Helper functions for object store mounting in Sky Storage"""
 import random
 import textwrap
+from typing import Optional
+
+from sky import exceptions
 
 
 def get_mounting_command(
     mount_path: str,
     install_cmd: str,
     mount_cmd: str,
+    version_check_cmd: Optional[str] = None,
 ) -> str:
     """
     Generates the mounting command for a given bucket. Generated script first
     unmounts any existing mount at the mount path, checks and installs the
     mounting utility if required, creates the mount path and finally mounts
     the bucket.
 
@@ -20,14 +24,17 @@
           single line.
         mount_cmd: Command to mount the bucket. Should be single line.
 
     Returns:
         str: Mounting command with the mounting script as a heredoc.
     """
     mount_binary = mount_cmd.split()[0]
+    installed_check = f'[ -x "$(command -v {mount_binary})" ]'
+    if version_check_cmd is not None:
+        installed_check += f' && {version_check_cmd}'
     script = textwrap.dedent(f"""
         #!/usr/bin/env bash
         set -e
 
         MOUNT_PATH={mount_path}
         MOUNT_BINARY={mount_binary}
 
@@ -35,31 +42,31 @@
         if grep -q $MOUNT_PATH /proc/mounts ; then
             echo "Path already mounted - unmounting..."
             fusermount -uz "$MOUNT_PATH"
             echo "Successfully unmounted $MOUNT_PATH."
         fi
 
         # Install MOUNT_BINARY if not already installed
-        if ! [ -x "$(command -v $MOUNT_BINARY)" ]; then
+        if {installed_check}; then
+          echo "$MOUNT_BINARY already installed. Proceeding..."
+        else
           echo "Installing $MOUNT_BINARY..."
           {install_cmd}
-        else
-          echo "$MOUNT_BINARY already installed. Proceeding..."
         fi
 
         # Check if mount path exists
         if [ ! -d "$MOUNT_PATH" ]; then
           echo "Mount path $MOUNT_PATH does not exist. Creating..."
           sudo mkdir -p $MOUNT_PATH
           sudo chmod 777 $MOUNT_PATH
         else
           # Check if mount path contains files
           if [ "$(ls -A $MOUNT_PATH)" ]; then
-            echo "Mount path $MOUNT_PATH is not empty. Please make sure its empty."
-            exit 1
+            echo "Mount path $MOUNT_PATH is not empty. Please mount to another path or remove it first."
+            exit {exceptions.MOUNT_PATH_NON_EMPTY_CODE}
           fi
         fi
         echo "Mounting $SOURCE_BUCKET to $MOUNT_PATH with $MOUNT_BINARY..."
         {mount_cmd}
         echo "Mounting done."
     """)
```

### Comparing `skypilot-0.2.5/sky/data/storage.py` & `skypilot-0.3.0/sky/data/storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Storage and Store Classes for Sky Data."""
 import enum
 import os
+import re
 import subprocess
 import time
 import typing
-from typing import Any, Dict, Optional, Tuple, Type, Union, List
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 import urllib.parse
 
 import colorama
 
 from sky import clouds
 from sky.adaptors import aws
 from sky.adaptors import gcp
+from sky.adaptors import cloudflare
 from sky.backends import backend_utils
 from sky.utils import schemas
 from sky.data import data_transfer
 from sky.data import data_utils
 from sky.data import mounting_utils
 from sky import exceptions
 from sky import global_user_state
@@ -32,30 +34,42 @@
 StorageHandle = Any
 StorageStatus = global_user_state.StorageStatus
 Path = str
 SourceType = Union[Path, List[Path]]
 
 # Clouds with object storage implemented in this module. Azure Blob
 # Storage isn't supported yet (even though Azure is).
-STORE_ENABLED_CLOUDS = [clouds.AWS(), clouds.GCP()]
+# TODO(Doyoung): need to add clouds.CLOUDFLARE() to support
+# R2 to be an option as preferred store type
+STORE_ENABLED_CLOUDS: List[str] = [
+    str(clouds.AWS()), str(clouds.GCP()), cloudflare.NAME
+]
 
 # Maximum number of concurrent rsync upload processes
 _MAX_CONCURRENT_UPLOADS = 32
 
 _BUCKET_FAIL_TO_CONNECT_MESSAGE = (
-    'Failed to connect to an existing bucket {name!r}.\n'
-    'Please check if:\n  1. the bucket name is taken and/or '
-    '\n  2. the bucket permissions are not setup correctly.')
+    'Failed to access existing bucket {name!r}. '
+    'This is likely because it is a private bucket you do not have access to.\n'
+    'To fix: \n'
+    '  1. If you are trying to create a new bucket: use a different name.\n'
+    '  2. If you are trying to connect to an existing bucket: make sure '
+    'your cloud credentials have access to it.')
+
+_BUCKET_EXTERNALLY_DELETED_DEBUG_MESSAGE = (
+    'Bucket {bucket_name!r} does not exist. '
+    'It may have been deleted externally.')
 
 
 class StoreType(enum.Enum):
     """Enum for the different types of stores."""
     S3 = 'S3'
     GCS = 'GCS'
     AZURE = 'AZURE'
+    R2 = 'R2'
 
     @classmethod
     def from_cloud(cls, cloud: clouds.Cloud) -> 'StoreType':
         if isinstance(cloud, clouds.AWS):
             return StoreType.S3
         elif isinstance(cloud, clouds.GCP):
             return StoreType.GCS
@@ -66,14 +80,16 @@
 
     @classmethod
     def from_store(cls, store: 'AbstractStore') -> 'StoreType':
         if isinstance(store, S3Store):
             return StoreType.S3
         elif isinstance(store, GcsStore):
             return StoreType.GCS
+        elif isinstance(store, R2Store):
+            return StoreType.R2
         else:
             with ux_utils.print_exception_no_traceback():
                 raise ValueError(f'Unknown store type: {store}')
 
 
 class StorageMode(enum.Enum):
     MOUNT = 'MOUNT'
@@ -97,14 +113,17 @@
 
 
 def get_store_prefix(storetype: StoreType) -> str:
     if storetype == StoreType.S3:
         return 's3://'
     elif storetype == StoreType.GCS:
         return 'gs://'
+    # R2 storages use 's3://' as a prefix for various aws cli commands
+    elif storetype == StoreType.R2:
+        return 's3://'
     elif storetype == StoreType.AZURE:
         with ux_utils.print_exception_no_traceback():
             raise ValueError('Azure Blob Storage is not supported yet.')
     else:
         with ux_utils.print_exception_no_traceback():
             raise ValueError(f'Unknown store type: {storetype}')
 
@@ -147,33 +166,39 @@
                     f'\n\tregion={self.region},'
                     f'\n\tis_sky_managed={self.is_sky_managed})')
 
     def __init__(self,
                  name: str,
                  source: Optional[SourceType],
                  region: Optional[str] = None,
-                 is_sky_managed: Optional[bool] = None):
+                 is_sky_managed: Optional[bool] = None,
+                 sync_on_reconstruction: Optional[bool] = True):
         """Initialize AbstractStore
 
         Args:
             name: Store name
             source: Data source for the store
             region: Region to place the bucket in
             is_sky_managed: Whether the store is managed by Sky. If None, it
               must be populated by the implementing class during initialization.
+            sync_on_reconstruction: bool; Whether to sync data if the storage
+              object is found in the global_user_state and reconstructed from
+              there. This is set to false when the Storage object is created not
+              for direct use, e.g. for sky storage delete.
 
         Raises:
             StorageBucketCreateError: If bucket creation fails
             StorageBucketGetError: If fetching existing bucket fails
             StorageInitError: If general initialization fails
         """
         self.name = name
         self.source = source
         self.region = region
         self.is_sky_managed = is_sky_managed
+        self.sync_on_reconstruction = sync_on_reconstruction
         # Whether sky is responsible for the lifecycle of the Store.
         self._validate()
         self.initialize()
 
     @classmethod
     def from_metadata(cls, metadata: StoreMetadata, **override_args):
         """Create a Store from a StoreMetadata object.
@@ -181,15 +206,17 @@
         Used when reconstructing Storage and Store objects from
         global_user_state.
         """
         return cls(name=override_args.get('name', metadata.name),
                    source=override_args.get('source', metadata.source),
                    region=override_args.get('region', metadata.region),
                    is_sky_managed=override_args.get('is_sky_managed',
-                                                    metadata.is_sky_managed))
+                                                    metadata.is_sky_managed),
+                   sync_on_reconstruction=override_args.get(
+                       'sync_on_reconstruction', True))
 
     def get_metadata(self) -> StoreMetadata:
         return self.StoreMetadata(name=self.name,
                                   source=self.source,
                                   region=self.region,
                                   is_sky_managed=self.is_sky_managed)
 
@@ -369,29 +396,28 @@
           mode: StorageMode; Specify how the storage object is manifested on
             the remote VM. Can be either MOUNT or COPY. Defaults to MOUNT.
           sync_on_reconstruction: bool; Whether to sync the data if the storage
             object is found in the global_user_state and reconstructed from
             there. This is set to false when the Storage object is created not
             for direct use, e.g. for sky storage delete.
         """
-        self.name = name
+        self.name: str
         self.source = source
         self.persistent = persistent
         self.mode = mode
         assert mode in StorageMode
         self.sync_on_reconstruction = sync_on_reconstruction
 
         # TODO(romilb, zhwu): This is a workaround to support storage deletion
         # for spot. Once sky storage supports forced management for external
         # buckets, this can be deprecated.
         self.force_delete = False
 
         # Validate and correct inputs if necessary
-        self._validate_storage_spec()
-        assert self.name is not None
+        self._validate_storage_spec(name)
 
         # Sky optimizer either adds a storage object instance or selects
         # from existing ones
         self.stores = {} if stores is None else stores
 
         # Logic to rebuild Storage if it is in global user state
         handle = global_user_state.get_handle_from_storage_name(self.name)
@@ -400,19 +426,28 @@
             # Reconstruct the Storage object from the global_user_state
             logger.debug('Detected existing storage object, '
                          f'loading Storage: {self.name}')
             for s_type, s_metadata in self.handle.sky_stores.items():
                 # When initializing from global_user_state, we override the
                 # source from the YAML
                 if s_type == StoreType.S3:
-                    store = S3Store.from_metadata(s_metadata,
-                                                  source=self.source)
+                    store = S3Store.from_metadata(
+                        s_metadata,
+                        source=self.source,
+                        sync_on_reconstruction=self.sync_on_reconstruction)
                 elif s_type == StoreType.GCS:
-                    store = GcsStore.from_metadata(s_metadata,
-                                                   source=self.source)
+                    store = GcsStore.from_metadata(
+                        s_metadata,
+                        source=self.source,
+                        sync_on_reconstruction=self.sync_on_reconstruction)
+                elif s_type == StoreType.R2:
+                    store = R2Store.from_metadata(
+                        s_metadata,
+                        source=self.source,
+                        sync_on_reconstruction=self.sync_on_reconstruction)
                 else:
                     with ux_utils.print_exception_no_traceback():
                         raise ValueError(f'Unknown store type: {s_type}')
 
                 self._add_store(store, is_reconstructed=True)
 
             # TODO(romilb): This logic should likely be in add_store to move
@@ -441,25 +476,27 @@
                 # If source is a pre-existing bucket, connect to the bucket
                 # If the bucket does not exist, this will error out
                 if isinstance(self.source, str):
                     if self.source.startswith('s3://'):
                         self.add_store(StoreType.S3)
                     elif self.source.startswith('gs://'):
                         self.add_store(StoreType.GCS)
+                    elif self.source.startswith('r2://'):
+                        self.add_store(StoreType.R2)
 
     @staticmethod
     def _validate_source(
             source: SourceType, mode: StorageMode,
             sync_on_reconstruction: bool) -> Tuple[SourceType, bool]:
         """Validates the source path.
 
         Args:
           source: str; File path where the data is initially stored. Can be a
-            local path or a cloud URI (s3://, gs://, etc.). Local paths do not
-            need to be absolute.
+            local path or a cloud URI (s3://, gs://, r2:// etc.).
+            Local paths do not need to be absolute.
           mode: StorageMode; StorageMode of the storage object
 
         Returns:
           Tuple[source, is_local_source]
           source: str; The source path.
           is_local_path: bool; Whether the source is a local path. False if URI.
         """
@@ -521,15 +558,15 @@
                             'that the file will be uploaded to the root of the '
                             'bucket and will appear at <destination_path>/'
                             f'{os.path.basename(source)}. Alternatively, you '
                             'can directly upload the file to the VM without '
                             'using a bucket by writing <destination_path>: '
                             f'{source} in the file_mounts section of your YAML')
                 is_local_source = True
-            elif split_path.scheme in ['s3', 'gs']:
+            elif split_path.scheme in ['s3', 'gs', 'r2']:
                 is_local_source = False
                 # Storage mounting does not support mounting specific files from
                 # cloud store - ensure path points to only a directory
                 if mode == StorageMode.MOUNT:
                     if split_path.path.strip('/') != '':
                         with ux_utils.print_exception_no_traceback():
                             raise exceptions.StorageModeError(
@@ -537,65 +574,90 @@
                                 ' mounting specific files from cloud'
                                 ' storage. Please use COPY mode or'
                                 ' specify only the bucket name as'
                                 ' the source.')
             else:
                 with ux_utils.print_exception_no_traceback():
                     raise exceptions.StorageSourceError(
-                        f'Supported paths: local, s3://, gs://. Got: {source}')
+                        f'Supported paths: local, s3://, gs://, '
+                        f'r2://. Got: {source}')
         return source, is_local_source
 
-    def _validate_storage_spec(self) -> None:
+    def _validate_storage_spec(self, name: Optional[str]) -> None:
         """
         Validates the storage spec and updates local fields if necessary.
         """
+
+        def validate_name(name):
+            """ Checks for validating the storage name.
+
+            Checks if the name starts the s3, gcs or r2 prefix and raise error
+            if it does. Store specific validation checks (e.g., S3 specific
+            rules) happen in the corresponding store class.
+            """
+            prefix = name.split('://')[0]
+            prefix = prefix.lower()
+            if prefix in ['s3', 'gs', 'r2']:
+                with ux_utils.print_exception_no_traceback():
+                    raise exceptions.StorageNameError(
+                        'Prefix detected: `name` cannot start with '
+                        f'{prefix}://. If you are trying to use an existing '
+                        'bucket created outside of SkyPilot, please specify it '
+                        'using the `source` field (e.g. '
+                        '`source: s3://mybucket/`). If you are trying to '
+                        'create a new bucket, please use the `store` field to '
+                        'specify the store type (e.g. `store: s3`).')
+
         if self.source is None:
             # If the mode is COPY, the source must be specified
             if self.mode == StorageMode.COPY:
                 # Check if a Storage object already exists in global_user_state
                 # (e.g. used as scratch previously). Such storage objects can be
                 # mounted in copy mode even though they have no source in the
                 # yaml spec (the name is the source).
-                handle = global_user_state.get_handle_from_storage_name(
-                    self.name)
-                if handle is not None:
-                    return
-                else:
+                handle = global_user_state.get_handle_from_storage_name(name)
+                if handle is None:
                     with ux_utils.print_exception_no_traceback():
                         raise exceptions.StorageSourceError(
                             'New storage object: source must be specified when '
                             'using COPY mode.')
             else:
                 # If source is not specified in COPY mode, the intent is to
                 # create a bucket and use it as scratch disk. Name must be
                 # specified to create bucket.
-                if not self.name:
+                if not name:
                     with ux_utils.print_exception_no_traceback():
                         raise exceptions.StorageSpecError(
                             'Storage source or storage name must be specified.')
-                else:
-                    # Create bucket and mount
-                    return
+            assert name is not None, handle
+            validate_name(name)
+            self.name = name
+            return
         elif self.source is not None:
             source, is_local_source = Storage._validate_source(
                 self.source, self.mode, self.sync_on_reconstruction)
-            if not self.name:
+            if not name:
                 if is_local_source:
                     with ux_utils.print_exception_no_traceback():
                         raise exceptions.StorageNameError(
                             'Storage name must be specified if the source is '
                             'local.')
                 else:
                     assert isinstance(source, str)
                     # Set name to source bucket name and continue
-                    self.name = urllib.parse.urlsplit(source).netloc
+                    name = urllib.parse.urlsplit(source).netloc
+                    assert name is not None, source
+                    self.name = name
                     return
             else:
                 if is_local_source:
                     # If name is specified and source is local, upload to bucket
+                    assert name is not None, source
+                    validate_name(name)
+                    self.name = name
                     return
                 else:
                     # Both name and source should not be specified if the source
                     # is a URI. Name will be inferred from the URI.
                     with ux_utils.print_exception_no_traceback():
                         raise exceptions.StorageSpecError(
                             'Storage name should not be specified if the '
@@ -607,37 +669,41 @@
     def add_store(self, store_type: Union[str, StoreType]) -> AbstractStore:
         """Initializes and adds a new store to the storage.
 
         Invoked by the optimizer after it has selected a store to
         add it to Storage.
 
         Args:
-          store_type: StoreType; Type of the storage [S3, GCS, AZURE]
+          store_type: StoreType; Type of the storage [S3, GCS, AZURE, R2]
         """
         if isinstance(store_type, str):
             store_type = StoreType(store_type)
 
         if store_type in self.stores:
             logger.info(f'Storage type {store_type} already exists.')
             return self.stores[store_type]
 
         store_cls: Type[AbstractStore]
         if store_type == StoreType.S3:
             store_cls = S3Store
         elif store_type == StoreType.GCS:
             store_cls = GcsStore
+        elif store_type == StoreType.R2:
+            store_cls = R2Store
         else:
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.StorageSpecError(
                     f'{store_type} not supported as a Store.')
 
-        assert self.name is not None, self.name
         # Initialize store object and get/create bucket
         try:
-            store = store_cls(name=self.name, source=self.source)
+            store = store_cls(
+                name=self.name,
+                source=self.source,
+                sync_on_reconstruction=self.sync_on_reconstruction)
         except exceptions.StorageBucketCreateError:
             # Creation failed, so this must be sky managed store. Add failure
             # to state.
             logger.error(f'Could not create {store_type} store '
                          f'with name {self.name}.')
             global_user_state.set_storage_status(self.name,
                                                  StorageStatus.INIT_FAILED)
@@ -808,38 +874,119 @@
 
 
 class S3Store(AbstractStore):
     """S3Store inherits from Storage Object and represents the backend
     for S3 buckets.
     """
 
-    ACCESS_DENIED_MESSAGE = 'Access Denied'
+    _ACCESS_DENIED_MESSAGE = 'Access Denied'
 
     def __init__(self,
                  name: str,
                  source: str,
                  region: Optional[str] = 'us-east-2',
-                 is_sky_managed: Optional[bool] = None):
+                 is_sky_managed: Optional[bool] = None,
+                 sync_on_reconstruction: bool = True):
         self.client: 'boto3.client.Client'
         self.bucket: 'StorageHandle'
-        super().__init__(name, source, region, is_sky_managed)
+        super().__init__(name, source, region, is_sky_managed,
+                         sync_on_reconstruction)
 
     def _validate(self):
         if self.source is not None and isinstance(self.source, str):
             if self.source.startswith('s3://'):
                 assert self.name == data_utils.split_s3_path(self.source)[0], (
                     'S3 Bucket is specified as path, the name should be the'
                     ' same as S3 bucket.')
             elif self.source.startswith('gs://'):
                 assert self.name == data_utils.split_gcs_path(self.source)[0], (
                     'GCS Bucket is specified as path, the name should be '
                     'the same as GCS bucket.')
                 assert data_utils.verify_gcs_bucket(self.name), (
                     f'Source specified as {self.source}, a GCS bucket. ',
                     'GCS Bucket should exist.')
+            elif self.source.startswith('r2://'):
+                assert self.name == data_utils.split_r2_path(self.source)[0], (
+                    'R2 Bucket is specified as path, the name should be '
+                    'the same as R2 bucket.')
+                assert data_utils.verify_r2_bucket(self.name), (
+                    f'Source specified as {self.source}, a R2 bucket. ',
+                    'R2 Bucket should exist.')
+        # Validate name
+        self.name = self.validate_name(self.name)
+
+        # Check if the storage is enabled
+        enabled_storage_clouds = global_user_state.get_enabled_storage_clouds()
+        if str(clouds.AWS()) not in enabled_storage_clouds:
+            with ux_utils.print_exception_no_traceback():
+                raise exceptions.ResourcesUnavailableError(
+                    'Storage \'store: s3\' specified, but ' \
+                    'AWS access is disabled. To fix, enable '\
+                    'AWS by running `sky check`. More info: '\
+                    'https://skypilot.readthedocs.io/en/latest/getting-started/installation.html.' # pylint: disable=line-too-long
+                    )
+
+    @classmethod
+    def validate_name(cls, name) -> str:
+        """Validates the name of the S3 store.
+
+        Source for rules: https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucketnamingrules.html # pylint: disable=line-too-long
+        """
+
+        def _raise_no_traceback_name_error(err_str):
+            with ux_utils.print_exception_no_traceback():
+                raise exceptions.StorageNameError(err_str)
+
+        if name is not None and isinstance(name, str):
+            if not 3 <= len(name) <= 63:
+                _raise_no_traceback_name_error(
+                    f'Invalid store name: name {name} must be between 3 (min) '
+                    'and 63 (max) characters long.')
+
+            # Check for valid characters and start/end with a letter or number
+            pattern = r'^[a-z0-9][-a-z0-9.]*[a-z0-9]$'
+            if not re.match(pattern, name):
+                _raise_no_traceback_name_error(
+                    f'Invalid store name: name {name} can consist only of '
+                    'lowercase letters, numbers, dots (.), and hyphens (-). '
+                    'It must begin and end with a letter or number.')
+
+            # Check for two adjacent periods
+            if '..' in name:
+                _raise_no_traceback_name_error(
+                    f'Invalid store name: name {name} must not contain '
+                    'two adjacent periods.')
+
+            # Check for IP address format
+            ip_pattern = r'^(?:\d{1,3}\.){3}\d{1,3}$'
+            if re.match(ip_pattern, name):
+                _raise_no_traceback_name_error(
+                    f'Invalid store name: name {name} must not be formatted as '
+                    'an IP address (for example, 192.168.5.4).')
+
+            # Check for 'xn--' prefix
+            if name.startswith('xn--'):
+                _raise_no_traceback_name_error(
+                    f'Invalid store name: name {name} must not start with the '
+                    'prefix "xn--".')
+
+            # Check for '-s3alias' suffix
+            if name.endswith('-s3alias'):
+                _raise_no_traceback_name_error(
+                    f'Invalid store name: name {name} must not end with the '
+                    'suffix "-s3alias".')
+
+            # Check for '--ol-s3' suffix
+            if name.endswith('--ol-s3'):
+                _raise_no_traceback_name_error(
+                    f'Invalid store name: name {name} must not end with the '
+                    'suffix "--ol-s3".')
+        else:
+            _raise_no_traceback_name_error('Store name must be specified.')
+        return name
 
     def initialize(self):
         """Initializes the S3 store object on the cloud.
 
         Initialization involves fetching bucket if exists, or creating it if
         it does not.
 
@@ -870,25 +1017,32 @@
             if isinstance(self.source, list):
                 self.batch_aws_rsync(self.source, create_dirs=True)
             elif self.source is not None:
                 if self.source.startswith('s3://'):
                     pass
                 elif self.source.startswith('gs://'):
                     self._transfer_to_s3()
+                elif self.source.startswith('r2://'):
+                    self._transfer_to_s3()
                 else:
                     self.batch_aws_rsync([self.source])
         except exceptions.StorageUploadError:
             raise
         except Exception as e:
             raise exceptions.StorageUploadError(
                 f'Upload failed for store {self.name}') from e
 
     def delete(self) -> None:
-        self._delete_s3_bucket(self.name)
-        logger.info(f'{colorama.Fore.GREEN}Deleted S3 bucket {self.name}.'
+        deleted_by_skypilot = self._delete_s3_bucket(self.name)
+        if deleted_by_skypilot:
+            msg_str = f'Deleted S3 bucket {self.name}.'
+        else:
+            msg_str = f'S3 bucket {self.name} may have been deleted ' \
+                      f'externally. Removing from local state.'
+        logger.info(f'{colorama.Fore.GREEN}{msg_str}'
                     f'{colorama.Style.RESET_ALL}')
 
     def get_handle(self) -> StorageHandle:
         return aws.resource('s3').Bucket(self.name)
 
     def batch_aws_rsync(self,
                         source_path_list: List[Path],
@@ -937,30 +1091,34 @@
                 f'[bold cyan]Syncing '
                 f'[green]{source_message}[/] to [green]s3://{self.name}/[/]'):
             data_utils.parallel_upload(
                 source_path_list,
                 get_file_sync_command,
                 get_dir_sync_command,
                 self.name,
-                self.ACCESS_DENIED_MESSAGE,
+                self._ACCESS_DENIED_MESSAGE,
                 create_dirs=create_dirs,
                 max_concurrent_uploads=_MAX_CONCURRENT_UPLOADS)
 
     def _transfer_to_s3(self) -> None:
         assert isinstance(self.source, str), self.source
         if self.source.startswith('gs://'):
             data_transfer.gcs_to_s3(self.name, self.name)
+        elif self.source.startswith('r2://'):
+            data_transfer.r2_to_s3(self.name, self.name)
 
-    def _get_bucket(self) -> Tuple[StorageHandle, bool]:
+    def _get_bucket(self) -> Tuple[Optional[StorageHandle], bool]:
         """Obtains the S3 bucket.
 
-        If the bucket exists, this method will connect to the bucket.
-        If the bucket does not exist, there are two cases:
+        If the bucket exists, this method will return the bucket.
+        If the bucket does not exist, there are three cases:
           1) Raise an error if the bucket source starts with s3://
-          2) Create a new bucket otherwise
+          2) Return None if bucket has been externally deleted and
+             sync_on_reconstruction is False
+          3) Create and return a new bucket otherwise
 
         Raises:
             StorageBucketCreateError: If creating the bucket fails
             StorageBucketGetError: If fetching a bucket fails
         """
         s3 = aws.resource('s3')
         bucket = s3.Bucket(self.name)
@@ -977,27 +1135,31 @@
             # AccessDenied error for buckets that are private and not owned by
             # user.
             if error_code == '403':
                 command = f'aws s3 ls {self.name}'
                 with ux_utils.print_exception_no_traceback():
                     raise exceptions.StorageBucketGetError(
                         _BUCKET_FAIL_TO_CONNECT_MESSAGE.format(name=self.name) +
-                        f' To debug, consider using {command}.') from e
+                        f' To debug, consider running `{command}`.') from e
 
         if isinstance(self.source, str) and self.source.startswith('s3://'):
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.StorageBucketGetError(
                     'Attempted to connect to a non-existent bucket: '
                     f'{self.source}. Consider using `aws s3 ls '
                     f'{self.source}` to debug.')
 
         # If bucket cannot be found in both private and public settings,
-        # the bucket is created by Sky.
-        bucket = self._create_s3_bucket(self.name)
-        return bucket, True
+        # the bucket is to be created by Sky. However, creation is skipped if
+        # Store object is being reconstructed for deletion.
+        if self.sync_on_reconstruction:
+            bucket = self._create_s3_bucket(self.name)
+            return bucket, True
+        else:
+            return None, False
 
     def _download_file(self, remote_path: str, local_path: str) -> None:
         """Downloads file from remote to local on s3 bucket
         using the boto3 API
 
         Args:
           remote_path: str; Remote path on S3 bucket
@@ -1047,58 +1209,72 @@
         except aws.botocore_exceptions().ClientError as e:
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.StorageBucketCreateError(
                     f'Attempted to create a bucket '
                     f'{self.name} but failed.') from e
         return aws.resource('s3').Bucket(bucket_name)
 
-    def _delete_s3_bucket(self, bucket_name: str) -> None:
+    def _delete_s3_bucket(self, bucket_name: str) -> bool:
         """Deletes S3 bucket, including all objects in bucket
 
         Args:
           bucket_name: str; Name of bucket
+
+        Returns:
+         bool; True if bucket was deleted, False if it was deleted externally.
         """
         # Deleting objects is very slow programatically
         # (i.e. bucket.objects.all().delete() is slow).
         # In addition, standard delete operations (i.e. via `aws s3 rm`)
         # are slow, since AWS puts deletion markers.
         # https://stackoverflow.com/questions/49239351/why-is-it-so-much-slower-to-delete-objects-in-aws-s3-than-it-is-to-create-them
         # The fastest way to delete is to run `aws s3 rb --force`,
         # which removes the bucket by force.
         remove_command = f'aws s3 rb s3://{bucket_name} --force'
         try:
             with log_utils.safe_rich_status(
                     f'[bold cyan]Deleting S3 bucket {bucket_name}[/]'):
-                subprocess.check_output(remove_command.split(' '))
+                subprocess.check_output(remove_command.split(' '),
+                                        stderr=subprocess.STDOUT)
         except subprocess.CalledProcessError as e:
-            logger.error(e.output)
-            with ux_utils.print_exception_no_traceback():
-                raise exceptions.StorageBucketDeleteError(
-                    f'Failed to delete S3 bucket {bucket_name}.')
+            if 'NoSuchBucket' in e.output.decode('utf-8'):
+                logger.debug(
+                    _BUCKET_EXTERNALLY_DELETED_DEBUG_MESSAGE.format(
+                        bucket_name=bucket_name))
+                return False
+            else:
+                logger.error(e.output)
+                with ux_utils.print_exception_no_traceback():
+                    raise exceptions.StorageBucketDeleteError(
+                        f'Failed to delete S3 bucket {bucket_name}.')
 
         # Wait until bucket deletion propagates on AWS servers
         while data_utils.verify_s3_bucket(bucket_name):
             time.sleep(0.1)
+        return True
 
 
 class GcsStore(AbstractStore):
     """GcsStore inherits from Storage Object and represents the backend
     for GCS buckets.
     """
 
-    ACCESS_DENIED_MESSAGE = 'AccessDeniedException'
+    _ACCESS_DENIED_MESSAGE = 'AccessDeniedException'
+    GCSFUSE_VERSION = '0.42.3'
 
     def __init__(self,
                  name: str,
                  source: str,
                  region: Optional[str] = 'us-central1',
-                 is_sky_managed: Optional[bool] = None):
+                 is_sky_managed: Optional[bool] = None,
+                 sync_on_reconstruction: Optional[bool] = True):
         self.client: 'storage.Client'
         self.bucket: StorageHandle
-        super().__init__(name, source, region, is_sky_managed)
+        super().__init__(name, source, region, is_sky_managed,
+                         sync_on_reconstruction)
 
     def _validate(self):
         if self.source is not None:
             if isinstance(self.source, str):
                 if self.source.startswith('s3://'):
                     assert self.name == data_utils.split_s3_path(
                         self.source
@@ -1110,14 +1286,92 @@
                         'S3 Bucket should exist.')
                 elif self.source.startswith('gs://'):
                     assert self.name == data_utils.split_gcs_path(
                         self.source
                     )[0], (
                         'GCS Bucket is specified as path, the name should be '
                         'the same as GCS bucket.')
+                elif self.source.startswith('r2://'):
+                    assert self.name == data_utils.split_r2_path(
+                        self.source
+                    )[0], ('R2 Bucket is specified as path, the name should be '
+                           'the same as R2 bucket.')
+                    assert data_utils.verify_r2_bucket(self.name), (
+                        f'Source specified as {self.source}, a R2 bucket. ',
+                        'R2 Bucket should exist.')
+        # Validate name
+        self.name = self.validate_name(self.name)
+        # Check if the storage is enabled
+        enabled_storage_clouds = global_user_state.get_enabled_storage_clouds()
+        if str(clouds.GCP()) not in enabled_storage_clouds:
+            with ux_utils.print_exception_no_traceback():
+                raise exceptions.ResourcesUnavailableError(
+                    'Storage \'store: gcs\' specified, but ' \
+                    'GCP access is disabled. To fix, enable '\
+                    'GCP by running `sky check`. '\
+                    'More info: https://skypilot.readthedocs.io/en/latest/getting-started/installation.html.' # pylint: disable=line-too-long
+                    )
+
+    @classmethod
+    def validate_name(cls, name) -> str:
+        """Validates the name of the GCS store.
+
+        Source for rules: https://cloud.google.com/storage/docs/buckets#naming
+        """
+
+        def _raise_no_traceback_name_error(err_str):
+            with ux_utils.print_exception_no_traceback():
+                raise exceptions.StorageNameError(err_str)
+
+        if name is not None and isinstance(name, str):
+            # Check for overall length
+            if not 3 <= len(name) <= 222:
+                _raise_no_traceback_name_error(
+                    f'Invalid store name: name {name} must contain 3-222 '
+                    'characters.')
+
+            # Check for valid characters and start/end with a number or letter
+            pattern = r'^[a-z0-9][-a-z0-9._]*[a-z0-9]$'
+            if not re.match(pattern, name):
+                _raise_no_traceback_name_error(
+                    f'Invalid store name: name {name} can only contain '
+                    'lowercase letters, numeric characters, dashes (-), '
+                    'underscores (_), and dots (.). Spaces are not allowed. '
+                    'Names must start and end with a number or letter.')
+
+            # Check for 'goog' prefix and 'google' in the name
+            if name.startswith('goog') or any(
+                    s in name
+                    for s in ['google', 'g00gle', 'go0gle', 'g0ogle']):
+                _raise_no_traceback_name_error(
+                    f'Invalid store name: name {name} cannot begin with the '
+                    '"goog" prefix or contain "google" in various forms.')
+
+            # Check for dot-separated components length
+            components = name.split('.')
+            if any(len(component) > 63 for component in components):
+                _raise_no_traceback_name_error(
+                    'Invalid store name: Dot-separated components in name '
+                    f'{name} can be no longer than 63 characters.')
+
+            if '..' in name or '.-' in name or '-.' in name:
+                _raise_no_traceback_name_error(
+                    f'Invalid store name: name {name} must not contain two '
+                    'adjacent periods or a dot next to a hyphen.')
+
+            # Check for IP address format
+            ip_pattern = r'^(?:\d{1,3}\.){3}\d{1,3}$'
+            if re.match(ip_pattern, name):
+                _raise_no_traceback_name_error(
+                    f'Invalid store name: name {name} cannot be represented as '
+                    'an IP address in dotted-decimal notation '
+                    '(for example, 192.168.5.4).')
+        else:
+            _raise_no_traceback_name_error('Store name must be specified.')
+        return name
 
     def initialize(self):
         """Initializes the GCS store object on the cloud.
 
         Initialization involves fetching bucket if exists, or creating it if
         it does not.
 
@@ -1148,27 +1402,34 @@
             if isinstance(self.source, list):
                 self.batch_gsutil_rsync(self.source, create_dirs=True)
             elif self.source is not None:
                 if self.source.startswith('gs://'):
                     pass
                 elif self.source.startswith('s3://'):
                     self._transfer_to_gcs()
+                elif self.source.startswith('r2://'):
+                    self._transfer_to_gcs()
                 else:
                     # If a single directory is specified in source, upload
                     # contents to root of bucket by suffixing /*.
                     self.batch_gsutil_rsync([self.source])
         except exceptions.StorageUploadError:
             raise
         except Exception as e:
             raise exceptions.StorageUploadError(
                 f'Upload failed for store {self.name}') from e
 
     def delete(self) -> None:
-        self._delete_gcs_bucket(self.name)
-        logger.info(f'{colorama.Fore.GREEN}Deleted GCS bucket {self.name}.'
+        deleted_by_skypilot = self._delete_gcs_bucket(self.name)
+        if deleted_by_skypilot:
+            msg_str = f'Deleted GCS bucket {self.name}.'
+        else:
+            msg_str = f'GCS bucket {self.name} may have been deleted ' \
+                      f'externally. Removing from local state.'
+        logger.info(f'{colorama.Fore.GREEN}{msg_str}'
                     f'{colorama.Style.RESET_ALL}')
 
     def get_handle(self) -> StorageHandle:
         return self.client.get_bucket(self.name)
 
     def batch_gsutil_cp(self,
                         source_path_list: List[Path],
@@ -1201,15 +1462,15 @@
         sync_command = (f'echo "{copy_list}" | '
                         f'gsutil -m cp -e -n -r -I gs://{self.name}')
 
         with log_utils.safe_rich_status(
                 f'[bold cyan]Syncing '
                 f'[green]{source_message}[/] to [green]gs://{self.name}/[/]'):
             data_utils.run_upload_cli(sync_command,
-                                      self.ACCESS_DENIED_MESSAGE,
+                                      self._ACCESS_DENIED_MESSAGE,
                                       bucket_name=self.name)
 
     def batch_gsutil_rsync(self,
                            source_path_list: List[Path],
                            create_dirs: bool = False) -> None:
         """Invokes gsutil rsync to batch upload a list of local paths
 
@@ -1251,29 +1512,33 @@
                 f'[bold cyan]Syncing '
                 f'[green]{source_message}[/] to [green]gs://{self.name}/[/]'):
             data_utils.parallel_upload(
                 source_path_list,
                 get_file_sync_command,
                 get_dir_sync_command,
                 self.name,
-                self.ACCESS_DENIED_MESSAGE,
+                self._ACCESS_DENIED_MESSAGE,
                 create_dirs=create_dirs,
                 max_concurrent_uploads=_MAX_CONCURRENT_UPLOADS)
 
     def _transfer_to_gcs(self) -> None:
         if isinstance(self.source, str) and self.source.startswith('s3://'):
             data_transfer.s3_to_gcs(self.name, self.name)
+        elif isinstance(self.source, str) and self.source.startswith('r2://'):
+            data_transfer.r2_to_gcs(self.name, self.name)
 
     def _get_bucket(self) -> Tuple[StorageHandle, bool]:
         """Obtains the GCS bucket.
         If the bucket exists, this method will connect to the bucket.
 
-        If the bucket does not exist, there are two cases:
+        If the bucket does not exist, there are three cases:
           1) Raise an error if the bucket source starts with gs://
-          2) Create a new bucket otherwise
+          2) Return None if bucket has been externally deleted and
+             sync_on_reconstruction is False
+          3) Create and return a new bucket otherwise
 
         Raises:
             StorageBucketCreateError: If creating the bucket fails
             StorageBucketGetError: If fetching a bucket fails
         """
         try:
             bucket = self.client.get_bucket(self.name)
@@ -1281,16 +1546,23 @@
         except gcp.not_found_exception() as e:
             if isinstance(self.source, str) and self.source.startswith('gs://'):
                 with ux_utils.print_exception_no_traceback():
                     raise exceptions.StorageBucketGetError(
                         'Attempted to connect to a non-existent bucket: '
                         f'{self.source}') from e
             else:
-                bucket = self._create_gcs_bucket(self.name)
-                return bucket, True
+
+                # If bucket cannot be found (i.e., does not exist), it is to be
+                # created by Sky. However, creation is skipped if Store object
+                # is being reconstructed for deletion.
+                if self.sync_on_reconstruction:
+                    bucket = self._create_gcs_bucket(self.name)
+                    return bucket, True
+                else:
+                    return None, False
         except gcp.forbidden_exception():
             # Try public bucket to see if bucket exists
             logger.info(
                 'External Bucket detected; Connecting to external bucket...')
             try:
                 a_client = gcp.anonymous_storage_client()
                 bucket = a_client.bucket(self.name)
@@ -1298,37 +1570,40 @@
                 next(bucket.list_blobs())
                 return bucket, False
             except (gcp.not_found_exception(), ValueError) as e:
                 command = f'gsutil ls gs://{self.name}'
                 with ux_utils.print_exception_no_traceback():
                     raise exceptions.StorageBucketGetError(
                         _BUCKET_FAIL_TO_CONNECT_MESSAGE.format(name=self.name) +
-                        f' To debug, consider using {command}.') from e
+                        f' To debug, consider running `{command}`.') from e
 
     def mount_command(self, mount_path: str) -> str:
         """Returns the command to mount the bucket to the mount_path.
 
         Uses gcsfuse to mount the bucket.
 
         Args:
           mount_path: str; Path to mount the bucket to.
         """
         install_cmd = ('wget -nc https://github.com/GoogleCloudPlatform/gcsfuse'
-                       '/releases/download/v0.41.10/gcsfuse_0.41.10_amd64.deb '
+                       f'/releases/download/v{self.GCSFUSE_VERSION}/'
+                       f'gcsfuse_{self.GCSFUSE_VERSION}_amd64.deb '
                        '-O /tmp/gcsfuse.deb && '
                        'sudo dpkg --install /tmp/gcsfuse.deb')
         mount_cmd = ('gcsfuse -o allow_other '
                      '--implicit-dirs '
                      f'--stat-cache-capacity {self._STAT_CACHE_CAPACITY} '
                      f'--stat-cache-ttl {self._STAT_CACHE_TTL} '
                      f'--type-cache-ttl {self._TYPE_CACHE_TTL} '
                      f'--rename-dir-limit {self._RENAME_DIR_LIMIT} '
                      f'{self.bucket.name} {mount_path}')
+        version_check_cmd = (
+            f'gcsfuse --version | grep -q {self.GCSFUSE_VERSION}')
         return mounting_utils.get_mounting_command(mount_path, install_cmd,
-                                                   mount_cmd)
+                                                   mount_cmd, version_check_cmd)
 
     def _download_file(self, remote_path: str, local_path: str) -> None:
         """Downloads file from remote to local on GS bucket
 
         Args:
           remote_path: str; Remote path on GS bucket
           local_path: str; Local path on user's device
@@ -1355,34 +1630,394 @@
                     f'Attempted to create a bucket {self.name} but failed.'
                 ) from e
         logger.info(
             f'Created GCS bucket {new_bucket.name} in {new_bucket.location} '
             f'with storage class {new_bucket.storage_class}')
         return new_bucket
 
-    def _delete_gcs_bucket(self, bucket_name: str) -> None:
+    def _delete_gcs_bucket(self, bucket_name: str) -> bool:
         """Deletes GCS bucket, including all objects in bucket
 
         Args:
           bucket_name: str; Name of bucket
+
+        Returns:
+         bool; True if bucket was deleted, False if it was deleted externally.
         """
-        try:
-            self.client.get_bucket(bucket_name)
-        except gcp.forbidden_exception() as e:
-            # Try public bucket to see if bucket exists
-            with ux_utils.print_exception_no_traceback():
-                raise PermissionError(
-                    'External Bucket detected. User not allowed to delete '
-                    'external bucket.') from e
 
-        try:
-            with log_utils.safe_rich_status(
-                    f'[bold cyan]Deleting GCS bucket {bucket_name}[/]'):
+        with log_utils.safe_rich_status(
+                f'[bold cyan]Deleting GCS bucket {bucket_name}[/]'):
+            try:
+                self.client.get_bucket(bucket_name)
+            except gcp.forbidden_exception() as e:
+                # Try public bucket to see if bucket exists
+                with ux_utils.print_exception_no_traceback():
+                    raise PermissionError(
+                        'External Bucket detected. User not allowed to delete '
+                        'external bucket.') from e
+            except gcp.not_found_exception():
+                # If bucket does not exist, it may have been deleted externally.
+                # Do a no-op in that case.
+                logger.debug(
+                    _BUCKET_EXTERNALLY_DELETED_DEBUG_MESSAGE.format(
+                        bucket_name=bucket_name))
+                return False
+            try:
                 remove_obj_command = ('gsutil -m rm -r'
                                       f' gs://{bucket_name}')
                 subprocess.check_output(remove_obj_command.split(' '),
                                         stderr=subprocess.STDOUT)
-        except subprocess.CalledProcessError as e:
-            logger.error(e.output)
+                return True
+            except subprocess.CalledProcessError as e:
+                logger.error(e.output)
+                with ux_utils.print_exception_no_traceback():
+                    raise exceptions.StorageBucketDeleteError(
+                        f'Failed to delete GCS bucket {bucket_name}.')
+
+
+class R2Store(AbstractStore):
+    """R2Store inherits from S3Store Object and represents the backend
+    for R2 buckets.
+    """
+
+    _ACCESS_DENIED_MESSAGE = 'Access Denied'
+
+    def __init__(self,
+                 name: str,
+                 source: str,
+                 region: Optional[str] = 'auto',
+                 is_sky_managed: Optional[bool] = None,
+                 sync_on_reconstruction: Optional[bool] = True):
+        self.client: 'boto3.client.Client'
+        self.bucket: 'StorageHandle'
+        super().__init__(name, source, region, is_sky_managed,
+                         sync_on_reconstruction)
+
+    def _validate(self):
+        if self.source is not None and isinstance(self.source, str):
+            if self.source.startswith('s3://'):
+                assert self.name == data_utils.split_s3_path(self.source)[0], (
+                    'S3 Bucket is specified as path, the name should be the'
+                    ' same as S3 bucket.')
+                assert data_utils.verify_s3_bucket(self.name), (
+                    f'Source specified as {self.source}, a S3 bucket. ',
+                    'S3 Bucket should exist.')
+            elif self.source.startswith('gs://'):
+                assert self.name == data_utils.split_gcs_path(self.source)[0], (
+                    'GCS Bucket is specified as path, the name should be '
+                    'the same as GCS bucket.')
+                assert data_utils.verify_gcs_bucket(self.name), (
+                    f'Source specified as {self.source}, a GCS bucket. ',
+                    'GCS Bucket should exist.')
+            elif self.source.startswith('r2://'):
+                assert self.name == data_utils.split_r2_path(self.source)[0], (
+                    'R2 Bucket is specified as path, the name should be '
+                    'the same as R2 bucket.')
+        # Validate name
+        self.name = S3Store.validate_name(self.name)
+        # Check if the storage is enabled
+        enabled_storage_clouds = global_user_state.get_enabled_storage_clouds()
+        if cloudflare.NAME not in enabled_storage_clouds:
             with ux_utils.print_exception_no_traceback():
-                raise exceptions.StorageBucketDeleteError(
-                    f'Failed to delete GCS bucket {bucket_name}.')
+                raise exceptions.ResourcesUnavailableError(
+                    'Storage \'store: r2\' specified, but ' \
+                    'Cloudflare R2 access is disabled. To fix, '\
+                    'enable Cloudflare R2 by running `sky check`. '\
+                    'More info: https://skypilot.readthedocs.io/en/latest/getting-started/installation.html.'  # pylint: disable=line-too-long
+                    )
+
+    def initialize(self):
+        """Initializes the R2 store object on the cloud.
+
+        Initialization involves fetching bucket if exists, or creating it if
+        it does not.
+
+        Raises:
+          StorageBucketCreateError: If bucket creation fails
+          StorageBucketGetError: If fetching existing bucket fails
+          StorageInitError: If general initialization fails.
+        """
+        self.client = data_utils.create_r2_client(self.region)
+        self.bucket, is_new_bucket = self._get_bucket()
+        if self.is_sky_managed is None:
+            # If is_sky_managed is not specified, then this is a new storage
+            # object (i.e., did not exist in global_user_state) and we should
+            # set the is_sky_managed property.
+            # If is_sky_managed is specified, then we take no action.
+            self.is_sky_managed = is_new_bucket
+
+    def upload(self):
+        """Uploads source to store bucket.
+
+        Upload must be called by the Storage handler - it is not called on
+        Store initialization.
+
+        Raises:
+            StorageUploadError: if upload fails.
+        """
+        try:
+            if isinstance(self.source, list):
+                self.batch_aws_rsync(self.source, create_dirs=True)
+            elif self.source is not None:
+                if self.source.startswith('s3://'):
+                    self._transfer_to_r2()
+                elif self.source.startswith('gs://'):
+                    self._transfer_to_r2()
+                elif self.source.startswith('r2://'):
+                    pass
+                else:
+                    self.batch_aws_rsync([self.source])
+        except exceptions.StorageUploadError:
+            raise
+        except Exception as e:
+            raise exceptions.StorageUploadError(
+                f'Upload failed for store {self.name}') from e
+
+    def delete(self) -> None:
+        deleted_by_skypilot = self._delete_r2_bucket(self.name)
+        if deleted_by_skypilot:
+            msg_str = f'Deleted R2 bucket {self.name}.'
+        else:
+            msg_str = f'R2 bucket {self.name} may have been deleted ' \
+                      f'externally. Removing from local state.'
+        logger.info(f'{colorama.Fore.GREEN}{msg_str}'
+                    f'{colorama.Style.RESET_ALL}')
+
+    def get_handle(self) -> StorageHandle:
+        return cloudflare.resource('s3').Bucket(self.name)
+
+    def batch_aws_rsync(self,
+                        source_path_list: List[Path],
+                        create_dirs: bool = False) -> None:
+        """Invokes aws s3 sync to batch upload a list of local paths to S3
+
+        AWS Sync by default uses 10 threads to upload files to the bucket.  To
+        increase parallelism, modify max_concurrent_requests in your aws config
+        file (Default path: ~/.aws/config).
+
+        Since aws s3 sync does not support batch operations, we construct
+        multiple commands to be run in parallel.
+
+        Args:
+            source_path_list: List of paths to local files or directories
+            create_dirs: If the local_path is a directory and this is set to
+                False, the contents of the directory are directly uploaded to
+                root of the bucket. If the local_path is a directory and this is
+                set to True, the directory is created in the bucket root and
+                contents are uploaded to it.
+        """
+
+        def get_file_sync_command(base_dir_path, file_names):
+            includes = ' '.join(
+                [f'--include "{file_name}"' for file_name in file_names])
+            endpoint_url = cloudflare.create_endpoint()
+            sync_command = ('AWS_SHARED_CREDENTIALS_FILE='
+                            f'{cloudflare.R2_CREDENTIALS_PATH} '
+                            'aws s3 sync --no-follow-symlinks --exclude="*" '
+                            f'{includes} {base_dir_path} '
+                            f's3://{self.name} '
+                            f'--endpoint {endpoint_url} '
+                            f'--profile={cloudflare.R2_PROFILE_NAME}')
+            return sync_command
+
+        def get_dir_sync_command(src_dir_path, dest_dir_name):
+            # we exclude .git directory from the sync
+            endpoint_url = cloudflare.create_endpoint()
+            sync_command = (
+                'AWS_SHARED_CREDENTIALS_FILE='
+                f'{cloudflare.R2_CREDENTIALS_PATH} '
+                'aws s3 sync --no-follow-symlinks --exclude ".git/*" '
+                f'{src_dir_path} '
+                f's3://{self.name}/{dest_dir_name} '
+                f'--endpoint {endpoint_url} '
+                f'--profile={cloudflare.R2_PROFILE_NAME}')
+            return sync_command
+
+        # Generate message for upload
+        if len(source_path_list) > 1:
+            source_message = f'{len(source_path_list)} paths'
+        else:
+            source_message = source_path_list[0]
+
+        with log_utils.safe_rich_status(
+                f'[bold cyan]Syncing '
+                f'[green]{source_message}[/] to [green]r2://{self.name}/[/]'):
+            data_utils.parallel_upload(
+                source_path_list,
+                get_file_sync_command,
+                get_dir_sync_command,
+                self.name,
+                self._ACCESS_DENIED_MESSAGE,
+                create_dirs=create_dirs,
+                max_concurrent_uploads=_MAX_CONCURRENT_UPLOADS)
+
+    def _transfer_to_r2(self) -> None:
+        assert isinstance(self.source, str), self.source
+        if self.source.startswith('gs://'):
+            data_transfer.gcs_to_r2(self.name, self.name)
+        elif self.source.startswith('s3://'):
+            data_transfer.s3_to_r2(self.name, self.name)
+
+    def _get_bucket(self) -> Tuple[StorageHandle, bool]:
+        """Obtains the R2 bucket.
+
+        If the bucket exists, this method will return the bucket.
+        If the bucket does not exist, there are three cases:
+          1) Raise an error if the bucket source starts with s3://
+          2) Return None if bucket has been externally deleted and
+             sync_on_reconstruction is False
+          3) Create and return a new bucket otherwise
+
+        Raises:
+            StorageBucketCreateError: If creating the bucket fails
+            StorageBucketGetError: If fetching a bucket fails
+        """
+        r2 = cloudflare.resource('s3')
+        bucket = r2.Bucket(self.name)
+        endpoint_url = cloudflare.create_endpoint()
+        try:
+            # Try Public bucket case.
+            # This line does not error out if the bucket is an external public
+            # bucket or if it is a user's bucket that is publicly
+            # accessible.
+            self.client.head_bucket(Bucket=self.name)
+            return bucket, False
+        except aws.botocore_exceptions().ClientError as e:
+            error_code = e.response['Error']['Code']
+            # AccessDenied error for buckets that are private and not owned by
+            # user.
+            if error_code == '403':
+                command = ('AWS_SHARED_CREDENTIALS_FILE='
+                           f'{cloudflare.R2_CREDENTIALS_PATH} '
+                           f'aws s3 ls s3://{self.name} '
+                           f'--endpoint {endpoint_url} '
+                           f'--profile={cloudflare.R2_PROFILE_NAME}')
+                with ux_utils.print_exception_no_traceback():
+                    raise exceptions.StorageBucketGetError(
+                        _BUCKET_FAIL_TO_CONNECT_MESSAGE.format(name=self.name) +
+                        f' To debug, consider running `{command}`.') from e
+
+        if isinstance(self.source, str) and self.source.startswith('r2://'):
+            with ux_utils.print_exception_no_traceback():
+                raise exceptions.StorageBucketGetError(
+                    'Attempted to connect to a non-existent bucket: '
+                    f'{self.source}. Consider using '
+                    '`AWS_SHARED_CREDENTIALS_FILE='
+                    f'{cloudflare.R2_CREDENTIALS_PATH} aws s3 ls '
+                    f's3://{self.name} '
+                    f'--endpoint {endpoint_url} '
+                    f'--profile={cloudflare.R2_PROFILE_NAME}\' '
+                    'to debug.')
+
+        # If bucket cannot be found in both private and public settings,
+        # the bucket is to be created by Sky. However, skip creation if
+        # Store object is being reconstructed for deletion.
+        if self.sync_on_reconstruction:
+            bucket = self._create_r2_bucket(self.name)
+            return bucket, True
+        else:
+            return None, False
+
+    def _download_file(self, remote_path: str, local_path: str) -> None:
+        """Downloads file from remote to local on r2 bucket
+        using the boto3 API
+
+        Args:
+          remote_path: str; Remote path on R2 bucket
+          local_path: str; Local path on user's device
+        """
+        self.bucket.download_file(remote_path, local_path)
+
+    def mount_command(self, mount_path: str) -> str:
+        """Returns the command to mount the bucket to the mount_path.
+
+        Uses goofys to mount the bucket.
+
+        Args:
+          mount_path: str; Path to mount the bucket to.
+        """
+        install_cmd = ('sudo wget -nc https://github.com/romilbhardwaj/goofys/'
+                       'releases/download/0.24.0-romilb-upstream/goofys '
+                       '-O /usr/local/bin/goofys && '
+                       'sudo chmod +x /usr/local/bin/goofys')
+        endpoint_url = cloudflare.create_endpoint()
+        mount_cmd = (
+            f'AWS_SHARED_CREDENTIALS_FILE={cloudflare.R2_CREDENTIALS_PATH} '
+            f'AWS_PROFILE={cloudflare.R2_PROFILE_NAME} goofys -o allow_other '
+            f'--stat-cache-ttl {self._STAT_CACHE_TTL} '
+            f'--type-cache-ttl {self._TYPE_CACHE_TTL} '
+            f'--endpoint {endpoint_url} '
+            f'{self.bucket.name} {mount_path}')
+        return mounting_utils.get_mounting_command(mount_path, install_cmd,
+                                                   mount_cmd)
+
+    def _create_r2_bucket(self,
+                          bucket_name: str,
+                          region='auto') -> StorageHandle:
+        """Creates R2 bucket with specific name in specific region
+
+        Args:
+          bucket_name: str; Name of bucket
+          region: str; Region name, r2 automatically sets region
+        Raises:
+          StorageBucketCreateError: If bucket creation fails.
+        """
+        r2_client = self.client
+        try:
+            if region is None:
+                r2_client.create_bucket(Bucket=bucket_name)
+            else:
+                location = {'LocationConstraint': region}
+                r2_client.create_bucket(Bucket=bucket_name,
+                                        CreateBucketConfiguration=location)
+                logger.info(f'Created R2 bucket {bucket_name} in {region}')
+        except aws.botocore_exceptions().ClientError as e:
+            with ux_utils.print_exception_no_traceback():
+                raise exceptions.StorageBucketCreateError(
+                    f'Attempted to create a bucket '
+                    f'{self.name} but failed.') from e
+        return cloudflare.resource('s3').Bucket(bucket_name)
+
+    def _delete_r2_bucket(self, bucket_name: str) -> bool:
+        """Deletes R2 bucket, including all objects in bucket
+
+        Args:
+          bucket_name: str; Name of bucket
+
+        Returns:
+         bool; True if bucket was deleted, False if it was deleted externally.
+        """
+        # Deleting objects is very slow programatically
+        # (i.e. bucket.objects.all().delete() is slow).
+        # In addition, standard delete operations (i.e. via `aws s3 rm`)
+        # are slow, since AWS puts deletion markers.
+        # https://stackoverflow.com/questions/49239351/why-is-it-so-much-slower-to-delete-objects-in-aws-s3-than-it-is-to-create-them
+        # The fastest way to delete is to run `aws s3 rb --force`,
+        # which removes the bucket by force.
+        endpoint_url = cloudflare.create_endpoint()
+        remove_command = (
+            f'AWS_SHARED_CREDENTIALS_FILE={cloudflare.R2_CREDENTIALS_PATH} '
+            f'aws s3 rb s3://{bucket_name} --force '
+            f'--endpoint {endpoint_url} '
+            f'--profile={cloudflare.R2_PROFILE_NAME}')
+        try:
+            with log_utils.safe_rich_status(
+                    f'[bold cyan]Deleting R2 bucket {bucket_name}[/]'):
+                subprocess.check_output(remove_command,
+                                        stderr=subprocess.STDOUT,
+                                        shell=True)
+        except subprocess.CalledProcessError as e:
+            if 'NoSuchBucket' in e.output.decode('utf-8'):
+                logger.debug(
+                    _BUCKET_EXTERNALLY_DELETED_DEBUG_MESSAGE.format(
+                        bucket_name=bucket_name))
+                return False
+            else:
+                logger.error(e.output)
+                with ux_utils.print_exception_no_traceback():
+                    raise exceptions.StorageBucketDeleteError(
+                        f'Failed to delete R2 bucket {bucket_name}.')
+
+        # Wait until bucket deletion propagates on AWS servers
+        while data_utils.verify_r2_bucket(bucket_name):
+            time.sleep(0.1)
+        return True
```

### Comparing `skypilot-0.2.5/sky/data/storage_utils.py` & `skypilot-0.3.0/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/exceptions.py` & `skypilot-0.3.0/sky/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 if typing.TYPE_CHECKING:
     from sky import global_user_state
 
 # Return code for keyboard interruption and SIGTSTP
 KEYBOARD_INTERRUPT_CODE = 130
 SIGTSTP_CODE = 146
 RSYNC_FILE_NOT_FOUND_CODE = 23
+# Arbitrarily chosen value. Used in SkyPilot's storage mounting scripts
+MOUNT_PATH_NON_EMPTY_CODE = 42
 
 
 class ResourcesUnavailableError(Exception):
     """Raised when resources are unavailable.
 
     This is mainly used for the APIs in sky.execution; please refer to
     the docstring of sky.launch for more details about how the
@@ -88,16 +90,18 @@
                    f'\n{error_msg}')
         super().__init__(message)
 
 
 class ClusterNotUpError(Exception):
     """Raised when a cluster is not up."""
 
-    def __init__(self, message: str,
-                 cluster_status: 'global_user_state.ClusterStatus') -> None:
+    def __init__(
+            self, message: str,
+            cluster_status: Optional['global_user_state.ClusterStatus']
+    ) -> None:
         super().__init__(message)
         self.cluster_status = cluster_status
 
 
 class ClusterSetUpError(Exception):
     """Raised when a cluster has setup error."""
     pass
@@ -198,7 +202,12 @@
     """Raised when the cloud identity is invalid."""
     pass
 
 
 class ClusterOwnerIdentityMismatchError(Exception):
     """The cluster's owner identity does not match the current user identity."""
     pass
+
+
+class NoCloudAccessError(Exception):
+    """Raised when all clouds are disabled."""
+    pass
```

### Comparing `skypilot-0.2.5/sky/execution.py` & `skypilot-0.3.0/sky/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     detach_run: bool = False,
     idle_minutes_to_autostop: Optional[int] = None,
     no_setup: bool = False,
     # Internal only:
     # pylint: disable=invalid-name
     _is_launched_by_spot_controller: bool = False,
 ) -> None:
-    """Execute a entrypoint.
+    """Execute an entrypoint.
 
     If sky.Task is given or DAG has not been optimized yet, this will call
     sky.optimize() for the caller.
 
     Args:
       entrypoint: sky.Task or sky.Dag.
       dryrun: bool; if True, only print the provision info (e.g., cluster
@@ -411,14 +411,15 @@
                 1. Empty: iff the first-ever sky.optimize() fails to
                 find a feasible resource; no pre-check or actual launch is
                 attempted.
                 2. Non-empty: iff at least 1 exception from either
                 our pre-checks (e.g., cluster name invalid) or a region/zone
                 throwing resource unavailability.
         exceptions.CommandError: any ssh command error.
+        exceptions.NoCloudAccessError: if all clouds are disabled.
     Other exceptions may be raised depending on the backend.
     """
     entrypoint = task
     backend_utils.check_cluster_name_not_reserved(cluster_name,
                                                   operation_str='sky.launch')
     _execute(
         entrypoint=entrypoint,
@@ -591,29 +592,30 @@
             'user_config_path': None,
             'spot_controller': controller_name,
             # Note: actual spot cluster name will be <task_name>-<spot job ID>
             'task_name': name,
             'uuid': task_uuid,
             'gcloud_installation_commands': gcp.GCLOUD_INSTALLATION_COMMAND,
             'is_dev': env_options.Options.IS_DEVELOPER.get(),
+            'is_debug': env_options.Options.SHOW_DEBUG_INFO.get(),
             'disable_logging': env_options.Options.DISABLE_LOGGING.get(),
             'logging_user_hash': common_utils.get_user_hash(),
             'retry_until_up': retry_until_up,
             'user': os.environ.get('USER', None),
         }
         if skypilot_config.loaded():
             # Look up the contents of the already loaded configs via the
             # 'skypilot_config' module. Don't simply read the on-disk file as
             # it may have changed since this process started.
             #
-            # Pop any proxy command, because the controller would've been
-            # launched behind the proxy, and in general any nodes we launch may
-            # not have or need the proxy setup. (If the controller needs to
-            # launch spot clusters in another region/VPC, the user should
-            # properly set up VPC peering, which will allow the
+            # Set any proxy command to None, because the controller would've
+            # been launched behind the proxy, and in general any nodes we
+            # launch may not have or need the proxy setup. (If the controller
+            # needs to launch spot clusters in another region/VPC, the user
+            # should properly set up VPC peering, which will allow the
             # cross-region/VPC communication. The proxy command is orthogonal
             # to this scenario.)
             #
             # This file will be uploaded to the controller node and will be
             # used throughout the spot job's recovery attempts (i.e., if it
             # relaunches due to preemption, we make sure the same config is
             # used).
@@ -624,19 +626,31 @@
             # in the new VPC. This happens if the two VPCs don’t have peering
             # set up. Like other places in the code, we assume properly setting
             # up networking is user's responsibilities.
             # TODO(zongheng): consider adding a basic check that checks
             # controller VPC (or name) == the spot job's VPC (or name). It may
             # not be a sufficient check (as it's always possible that peering
             # is not set up), but it may catch some obvious errors.
-            # TODO(zhwu): hacky. We should pop the proxy command of the cloud
-            # where the controller is launched (currently, only aws user uses
-            # proxy_command).
-            config_dict = skypilot_config.pop_nested(
-                ('aws', 'ssh_proxy_command'))
+            # TODO(zhwu): hacky. We should only set the proxy command of the
+            # cloud where the controller is launched (currently, only aws user
+            # uses proxy_command).
+            proxy_command_key = ('aws', 'ssh_proxy_command')
+            ssh_proxy_command = skypilot_config.get_nested(
+                proxy_command_key, None)
+            if isinstance(ssh_proxy_command, str):
+                config_dict = skypilot_config.set_nested(
+                    proxy_command_key, None)
+            elif isinstance(ssh_proxy_command, dict):
+                # Instead of removing the key, we set the value to empty string
+                # so that the controller will only try the regions specified by
+                # the keys.
+                ssh_proxy_command = {k: None for k in ssh_proxy_command}
+                config_dict = skypilot_config.set_nested(
+                    proxy_command_key, ssh_proxy_command)
+
             with tempfile.NamedTemporaryFile(mode='w', delete=False) as tmpfile:
                 common_utils.dump_yaml(tmpfile.name, config_dict)
                 vars_to_fill.update({
                     'user_config_path': tmpfile.name,
                     'env_var_skypilot_config':
                         skypilot_config.ENV_VAR_SKYPILOT_CONFIG,
                 })
@@ -684,19 +698,27 @@
     original_file_mounts = task.file_mounts if task.file_mounts else {}
     original_storage_mounts = task.storage_mounts if task.storage_mounts else {}
 
     copy_mounts = task.get_local_to_remote_file_mounts()
     if copy_mounts is None:
         copy_mounts = {}
 
-    has_local_source_paths = (task.workdir is not None) or copy_mounts
-    if has_local_source_paths:
-        logger.info(
-            f'{colorama.Fore.YELLOW}Translating file_mounts with local '
-            f'source paths to SkyPilot Storage...{colorama.Style.RESET_ALL}')
+    has_local_source_paths_file_mounts = bool(copy_mounts)
+    has_local_source_paths_workdir = task.workdir is not None
+
+    msg = None
+    if has_local_source_paths_workdir and has_local_source_paths_file_mounts:
+        msg = 'workdir and file_mounts with local source paths'
+    elif has_local_source_paths_file_mounts:
+        msg = 'file_mounts with local source paths'
+    elif has_local_source_paths_workdir:
+        msg = 'workdir'
+    if msg:
+        logger.info(f'{colorama.Fore.YELLOW}Translating {msg} to SkyPilot '
+                    f'Storage...{colorama.Style.RESET_ALL}')
 
     # Step 1: Translate the workdir to SkyPilot storage.
     new_storage_mounts = {}
     if task.workdir is not None:
         bucket_name = spot.constants.SPOT_WORKDIR_BUCKET_NAME.format(
             username=getpass.getuser(), id=run_id)
         workdir = task.workdir
@@ -722,14 +744,15 @@
     # Step 2: Translate the local file mounts with folder in src to SkyPilot
     # storage.
     # TODO(zhwu): Optimize this by:
     # 1. Use the same bucket for all the mounts.
     # 2. When the src is the same, use the same bucket.
     copy_mounts_with_file_in_src = {}
     for i, (dst, src) in enumerate(copy_mounts.items()):
+        assert task.file_mounts is not None
         task.file_mounts.pop(dst)
         if os.path.isfile(os.path.abspath(os.path.expanduser(src))):
             copy_mounts_with_file_in_src[dst] = src
             continue
         bucket_name = spot.constants.SPOT_FM_BUCKET_NAME.format(
             username=getpass.getuser(),
             id=f'{run_id}-{i}',
@@ -815,15 +838,16 @@
             assert len(store_types) == 1, (
                 'We only support one store type for now.', storage_obj.stores)
             store_type = store_types[0]
             if store_type == storage_lib.StoreType.S3:
                 storage_obj.source = f's3://{storage_obj.name}'
             elif store_type == storage_lib.StoreType.GCS:
                 storage_obj.source = f'gs://{storage_obj.name}'
+            elif store_type == storage_lib.StoreType.R2:
+                storage_obj.source = f'r2://{storage_obj.name}'
             else:
                 with ux_utils.print_exception_no_traceback():
                     raise exceptions.NotSupportedError(
                         f'Unsupported store type: {store_type}')
-            storage_obj.name = None
             storage_obj.force_delete = True
 
     return task
```

### Comparing `skypilot-0.2.5/sky/global_user_state.py` & `skypilot-0.3.0/sky/global_user_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 import typing
 from typing import Any, Dict, List, Tuple, Optional, Set
 import uuid
 
 import colorama
 
 from sky import clouds
-from sky.utils import db_utils
+from sky.adaptors import cloudflare
+from sky.data import storage as storage_lib
 from sky.utils import common_utils
+from sky.utils import db_utils
 
 if typing.TYPE_CHECKING:
     from sky import backends
     from sky.data import Storage
 
 _ENABLED_CLOUDS_KEY = 'enabled_clouds'
 
@@ -193,15 +195,17 @@
     usage_intervals = _get_cluster_usage_intervals(cluster_hash)
 
     # first time a cluster is being launched
     if not usage_intervals:
         usage_intervals = []
 
     # if this is the cluster init or we are starting after a stop
-    if len(usage_intervals) == 0 or usage_intervals[-1][-1] is not None:
+    if not usage_intervals or usage_intervals[-1][-1] is not None:
+        assert cluster_launched_at is not None, (cluster_name, is_launch,
+                                                 usage_intervals)
         usage_intervals.append((cluster_launched_at, None))
 
     if requested_resources:
         assert len(requested_resources) == 1, requested_resources
         requested_resources = list(requested_resources)[0]
 
     _DB.cursor.execute(
@@ -268,14 +272,16 @@
             cluster_name,
             # owner
             cluster_name,
             # cluster_hash
             cluster_hash,
         ))
 
+    launched_nodes = getattr(cluster_handle, 'launched_nodes', None)
+    launched_resources = getattr(cluster_handle, 'launched_resources', None)
     _DB.cursor.execute(
         'INSERT or REPLACE INTO cluster_history'
         '(cluster_hash, name, num_nodes, requested_resources, '
         'launched_resources, usage_intervals) '
         'VALUES ('
         # hash
         '?, '
@@ -291,55 +297,57 @@
         '?)',
         (
             # hash
             cluster_hash,
             # name
             cluster_name,
             # number of nodes
-            cluster_handle.launched_nodes,
+            launched_nodes,
             # requested resources
             pickle.dumps(requested_resources),
             # launched resources
-            pickle.dumps(cluster_handle.launched_resources),
+            pickle.dumps(launched_resources),
             # usage intervals
             pickle.dumps(usage_intervals),
         ))
 
     _DB.conn.commit()
 
 
 def update_last_use(cluster_name: str):
     """Updates the last used command for the cluster."""
     _DB.cursor.execute('UPDATE clusters SET last_use=(?) WHERE name=(?)',
                        (common_utils.get_pretty_entry_point(), cluster_name))
     _DB.conn.commit()
 
 
-def remove_cluster(cluster_name: str, terminate: bool) -> float:
+def remove_cluster(cluster_name: str, terminate: bool) -> None:
     """Removes cluster_name mapping."""
     cluster_hash = _get_hash_for_existing_cluster(cluster_name)
     usage_intervals = _get_cluster_usage_intervals(cluster_hash)
 
     # usage_intervals is not None and not empty
     if usage_intervals:
+        assert cluster_hash is not None, cluster_name
         start_time = usage_intervals.pop()[0]
         end_time = int(time.time())
         usage_intervals.append((start_time, end_time))
         _set_cluster_usage_intervals(cluster_hash, usage_intervals)
 
     if terminate:
         _DB.cursor.execute('DELETE FROM clusters WHERE name=(?)',
                            (cluster_name,))
     else:
         handle = get_handle_from_cluster_name(cluster_name)
         if handle is None:
             return
         # Must invalidate IP list: otherwise 'sky cpunode'
         # on a stopped cpunode will directly try to ssh, which leads to timeout.
-        handle.stable_internal_external_ips = None
+        if hasattr(handle, 'stable_internal_external_ips'):
+            handle.stable_internal_external_ips = None
         _DB.cursor.execute(
             'UPDATE clusters SET handle=(?), status=(?) '
             'WHERE name=(?)', (
                 pickle.dumps(handle),
                 ClusterStatus.STOPPED.value,
                 cluster_name,
             ))
@@ -349,14 +357,15 @@
 def get_handle_from_cluster_name(
         cluster_name: str) -> Optional['backends.ResourceHandle']:
     assert cluster_name is not None, 'cluster_name cannot be None'
     rows = _DB.cursor.execute('SELECT handle FROM clusters WHERE name=(?)',
                               (cluster_name,))
     for (handle,) in rows:
         return pickle.loads(handle)
+    return None
 
 
 def get_glob_cluster_names(cluster_name: str) -> List[str]:
     assert cluster_name is not None, 'cluster_name cannot be None'
     rows = _DB.cursor.execute('SELECT name FROM clusters WHERE name GLOB (?)',
                               (cluster_name,))
     return [row[0] for row in rows]
@@ -392,71 +401,83 @@
 def get_cluster_launch_time(cluster_name: str) -> Optional[int]:
     rows = _DB.cursor.execute('SELECT launched_at FROM clusters WHERE name=(?)',
                               (cluster_name,))
     for (launch_time,) in rows:
         if launch_time is None:
             return None
         return int(launch_time)
+    return None
 
 
 def get_cluster_metadata(cluster_name: str) -> Optional[Dict[str, Any]]:
     rows = _DB.cursor.execute('SELECT metadata FROM clusters WHERE name=(?)',
                               (cluster_name,))
     for (metadata,) in rows:
         if metadata is None:
             return None
         return json.loads(metadata)
+    return None
 
 
 def set_cluster_metadata(cluster_name: str, metadata: Dict[str, Any]) -> None:
     _DB.cursor.execute('UPDATE clusters SET metadata=(?) WHERE name=(?)', (
         json.dumps(metadata),
         cluster_name,
     ))
     count = _DB.cursor.rowcount
     _DB.conn.commit()
     assert count <= 1, count
     if count == 0:
         raise ValueError(f'Cluster {cluster_name} not found.')
 
 
-def _get_cluster_usage_intervals(cluster_hash: str) -> Optional[Dict[str, Any]]:
+def _get_cluster_usage_intervals(
+        cluster_hash: Optional[str]
+) -> Optional[List[Tuple[int, Optional[int]]]]:
+    if cluster_hash is None:
+        return None
     rows = _DB.cursor.execute(
         'SELECT usage_intervals FROM cluster_history WHERE cluster_hash=(?)',
         (cluster_hash,))
     for (usage_intervals,) in rows:
         if usage_intervals is None:
             return None
         return pickle.loads(usage_intervals)
+    return None
 
 
-def _get_cluster_launch_time(cluster_hash: str) -> Optional[Dict[str, Any]]:
+def _get_cluster_launch_time(cluster_hash: str) -> Optional[int]:
     usage_intervals = _get_cluster_usage_intervals(cluster_hash)
+    if usage_intervals is None:
+        return None
     return usage_intervals[0][0]
 
 
 def _get_cluster_duration(cluster_hash: str) -> int:
     total_duration = 0
     usage_intervals = _get_cluster_usage_intervals(cluster_hash)
 
     if usage_intervals is None:
         return total_duration
 
     for i, (start_time, end_time) in enumerate(usage_intervals):
         # duration from latest start time to time of query
+        if start_time is None:
+            continue
         if end_time is None:
             assert i == len(usage_intervals) - 1, i
             end_time = int(time.time())
         start_time, end_time = int(start_time), int(end_time)
         total_duration += end_time - start_time
     return total_duration
 
 
-def _set_cluster_usage_intervals(cluster_hash: str,
-                                 usage_intervals: Dict[str, Any]) -> None:
+def _set_cluster_usage_intervals(
+        cluster_hash: str, usage_intervals: List[Tuple[int,
+                                                       Optional[int]]]) -> None:
     _DB.cursor.execute(
         'UPDATE cluster_history SET usage_intervals=(?) WHERE cluster_hash=(?)',
         (
             pickle.dumps(usage_intervals),
             cluster_hash,
         ))
 
@@ -464,19 +485,20 @@
     _DB.conn.commit()
     assert count <= 1, count
     if count == 0:
         raise ValueError(f'Cluster hash {cluster_hash} not found.')
 
 
 def set_owner_identity_for_cluster(cluster_name: str,
-                                   owner_identity: Optional[str]) -> None:
+                                   owner_identity: Optional[List[str]]) -> None:
     if owner_identity is None:
         return
+    owner_identity_str = json.dumps(owner_identity)
     _DB.cursor.execute('UPDATE clusters SET owner=(?) WHERE name=(?)',
-                       (owner_identity, cluster_name))
+                       (owner_identity_str, cluster_name))
 
     count = _DB.cursor.rowcount
     _DB.conn.commit()
     assert count <= 1, count
     if count == 0:
         raise ValueError(f'Cluster {cluster_name} not found.')
 
@@ -484,27 +506,48 @@
 def _get_hash_for_existing_cluster(cluster_name: str) -> Optional[str]:
     rows = _DB.cursor.execute(
         'SELECT cluster_hash FROM clusters WHERE name=(?)', (cluster_name,))
     for (cluster_hash,) in rows:
         if cluster_hash is None:
             return None
         return cluster_hash
+    return None
 
 
 def get_launched_resources_from_cluster_hash(
         cluster_hash: str) -> Optional[Tuple[int, Any]]:
 
     rows = _DB.cursor.execute(
         'SELECT num_nodes, launched_resources '
         'FROM cluster_history WHERE cluster_hash=(?)', (cluster_hash,))
     for (num_nodes, launched_resources) in rows:
         if num_nodes is None or launched_resources is None:
             return None
         launched_resources = pickle.loads(launched_resources)
         return num_nodes, launched_resources
+    return None
+
+
+def _load_owner(record_owner: Optional[str]) -> Optional[List[str]]:
+    if record_owner is None:
+        return None
+    try:
+        result = json.loads(record_owner)
+        if result is not None and not isinstance(result, list):
+            # Backwards compatibility for old records, which were stored as
+            # a string instead of a list. It is possible that json.loads
+            # will parse the string with all numbers as an int, so we need
+            # to convert it back to a list of strings.
+            return [str(result)]
+        return result
+    except json.JSONDecodeError:
+        # Backwards compatibility for old records, which were stored as
+        # a string instead of a list. This will happen when the previous
+        # UserId is a string instead of an int.
+        return [record_owner]
 
 
 def get_cluster_from_name(
         cluster_name: Optional[str]) -> Optional[Dict[str, Any]]:
     rows = _DB.cursor.execute('SELECT * FROM clusters WHERE name=(?)',
                               (cluster_name,)).fetchall()
     for row in rows:
@@ -518,19 +561,20 @@
             'name': name,
             'launched_at': launched_at,
             'handle': pickle.loads(handle),
             'last_use': last_use,
             'status': ClusterStatus[status],
             'autostop': autostop,
             'to_down': bool(to_down),
-            'owner': owner,
+            'owner': _load_owner(owner),
             'metadata': json.loads(metadata),
             'cluster_hash': cluster_hash,
         }
         return record
+    return None
 
 
 def get_clusters() -> List[Dict[str, Any]]:
     rows = _DB.cursor.execute(
         'select * from clusters order by launched_at desc').fetchall()
     records = []
     for row in rows:
@@ -542,15 +586,15 @@
             'name': name,
             'launched_at': launched_at,
             'handle': pickle.loads(handle),
             'last_use': last_use,
             'status': ClusterStatus[status],
             'autostop': autostop,
             'to_down': bool(to_down),
-            'owner': owner,
+            'owner': _load_owner(owner),
             'metadata': json.loads(metadata),
             'cluster_hash': cluster_hash,
         }
 
         records.append(record)
     return records
 
@@ -609,15 +653,36 @@
 def get_enabled_clouds() -> List[clouds.Cloud]:
     rows = _DB.cursor.execute('SELECT value FROM config WHERE key = ?',
                               (_ENABLED_CLOUDS_KEY,))
     ret = []
     for (value,) in rows:
         ret = json.loads(value)
         break
-    return [clouds.CLOUD_REGISTRY.from_str(cloud) for cloud in ret]
+    enabled_clouds: List[clouds.Cloud] = []
+    for c in ret:
+        cloud = clouds.CLOUD_REGISTRY.from_str(c)
+        if cloud is not None:
+            enabled_clouds.append(cloud)
+    return enabled_clouds
+
+
+def get_enabled_storage_clouds() -> List[str]:
+    # This is a temporary solution until https://github.com/skypilot-org/skypilot/issues/1943 # pylint: disable=line-too-long
+    # is resolved by implementing separate 'enabled_storage_clouds'
+    enabled_clouds = get_enabled_clouds()
+    enabled_clouds = [str(cloud) for cloud in enabled_clouds]
+
+    enabled_storage_clouds = [
+        cloud for cloud in enabled_clouds
+        if cloud in storage_lib.STORE_ENABLED_CLOUDS
+    ]
+    r2_is_enabled, _ = cloudflare.check_credentials()
+    if r2_is_enabled:
+        enabled_storage_clouds.append(cloudflare.NAME)
+    return enabled_storage_clouds
 
 
 def set_enabled_clouds(enabled_clouds: List[str]) -> None:
     _DB.cursor.execute('INSERT OR REPLACE INTO config VALUES (?, ?)',
                        (_ENABLED_CLOUDS_KEY, json.dumps(enabled_clouds)))
     _DB.conn.commit()
 
@@ -655,23 +720,25 @@
     count = _DB.cursor.rowcount
     _DB.conn.commit()
     assert count <= 1, count
     if count == 0:
         raise ValueError(f'Storage {storage_name} not found.')
 
 
-def get_storage_status(storage_name: str) -> None:
+def get_storage_status(storage_name: str) -> Optional[StorageStatus]:
     assert storage_name is not None, 'storage_name cannot be None'
     rows = _DB.cursor.execute('SELECT status FROM storage WHERE name=(?)',
                               (storage_name,))
     for (status,) in rows:
         return StorageStatus[status]
+    return None
 
 
-def set_storage_handle(storage_name: str, handle: 'Storage.StorageMetadata'):
+def set_storage_handle(storage_name: str,
+                       handle: 'Storage.StorageMetadata') -> None:
     _DB.cursor.execute('UPDATE storage SET handle=(?) WHERE name=(?)', (
         pickle.dumps(handle),
         storage_name,
     ))
     count = _DB.cursor.rowcount
     _DB.conn.commit()
     assert count <= 1, count
@@ -685,14 +752,15 @@
         return None
     rows = _DB.cursor.execute('SELECT handle FROM storage WHERE name=(?)',
                               (storage_name,))
     for (handle,) in rows:
         if handle is None:
             return None
         return pickle.loads(handle)
+    return None
 
 
 def get_glob_storage_name(storage_name: str) -> List[str]:
     assert storage_name is not None, 'storage_name cannot be None'
     rows = _DB.cursor.execute('SELECT name FROM storage WHERE name GLOB (?)',
                               (storage_name,))
     return [row[0] for row in rows]
```

### Comparing `skypilot-0.2.5/sky/optimizer.py` & `skypilot-0.3.0/sky/optimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Optimizer: assigns best resources to user tasks."""
 import collections
 import enum
 import typing
-from typing import Dict, List, Optional, Tuple
+from typing import Any, Dict, Iterable, List, Optional, Tuple
 
 import colorama
 import numpy as np
 import prettytable
 
 from sky import check
 from sky import clouds
@@ -17,29 +17,28 @@
 from sky import task as task_lib
 from sky.backends import backend_utils
 from sky.utils import env_options
 from sky.utils import ux_utils
 from sky.utils import log_utils
 
 if typing.TYPE_CHECKING:
-    from sky import dag as dag_lib
+    import networkx as nx
+    from sky import dag as dag_lib  # pylint: disable=ungrouped-imports
 
 logger = sky_logging.init_logger(__name__)
 
-Task = task_lib.Task
-
 _DUMMY_SOURCE_NAME = 'skypilot-dummy-source'
 _DUMMY_SINK_NAME = 'skypilot-dummy-sink'
 
 # task -> resources -> estimated cost or time.
-_TaskToCostMap = Dict[Task, Dict[resources_lib.Resources, float]]
+_TaskToCostMap = Dict[task_lib.Task, Dict[resources_lib.Resources, float]]
 # cloud -> list of resources that have the same accelerators.
 _PerCloudCandidates = Dict[clouds.Cloud, List[resources_lib.Resources]]
 # task -> per-cloud candidates
-_TaskToPerCloudCandidates = Dict[Task, _PerCloudCandidates]
+_TaskToPerCloudCandidates = Dict[task_lib.Task, _PerCloudCandidates]
 
 
 # Constants: minimize what target?
 class OptimizeTarget(enum.Enum):
     COST = 0
     TIME = 1
 
@@ -85,30 +84,31 @@
             bandwidth_gbps = 10
             egress_time = gigabytes * 8 / bandwidth_gbps
         else:
             egress_time = 0.0
         return egress_time
 
     @staticmethod
-    def optimize(
-            dag: 'dag_lib.Dag',
-            minimize=OptimizeTarget.COST,
-            blocked_resources: Optional[List[resources_lib.Resources]] = None,
-            quiet: bool = False):
+    def optimize(dag: 'dag_lib.Dag',
+                 minimize=OptimizeTarget.COST,
+                 blocked_resources: Optional[Iterable[
+                     resources_lib.Resources]] = None,
+                 quiet: bool = False):
         """Find the best execution plan for the given DAG.
 
         Args:
             dag: the DAG to optimize.
             minimize: whether to minimize cost or time.
             blocked_resources: a list of resources that should not be used.
             quiet: whether to suppress logging.
 
         Raises:
             exceptions.ResourcesUnavailableError: if no resources are available
                 for a task.
+            exceptions.NoCloudAccessError: if no public clouds are enabled.
         """
         # This function is effectful: mutates every node in 'dag' by setting
         # node.best_resources if it is None.
         Optimizer._add_dummy_source_sink_nodes(dag)
         try:
             unused_best_plan = Optimizer._optimize_objective(
                 dag,
@@ -144,15 +144,15 @@
             if in_degree == 0:
                 zero_indegree_nodes.append(node)
         for node, out_degree in graph.out_degree():
             if out_degree == 0:
                 zero_outdegree_nodes.append(node)
 
         def make_dummy(name):
-            dummy = Task(name)
+            dummy = task_lib.Task(name)
             dummy.set_resources({DummyResources(DummyCloud(), None)})
             dummy.set_time_estimator(lambda _: 0)
             return dummy
 
         with dag:
             source = make_dummy(_DUMMY_SOURCE_NAME)
             for real_source_node in zero_indegree_nodes:
@@ -170,55 +170,57 @@
             return
         assert len(source) == len(sink) == 1, dag.tasks
         dag.remove(source[0])
         dag.remove(sink[0])
 
     @staticmethod
     def _get_egress_info(
-        parent: Task,
+        parent: task_lib.Task,
         parent_resources: resources_lib.Resources,
-        node: Task,
+        node: task_lib.Task,
         resources: resources_lib.Resources,
-    ) -> Tuple[clouds.Cloud, clouds.Cloud, float]:
+    ) -> Tuple[Optional[clouds.Cloud], Optional[clouds.Cloud], float]:
         if isinstance(parent_resources.cloud, DummyCloud):
             # Special case.  The current 'node' is a real
             # source node, and its input may be on a different
             # cloud from 'resources'.
             if node.get_inputs() is None:
-                # A Task may have no inputs specified.
+                # A task_lib.Task may have no inputs specified.
                 return None, None, 0
             src_cloud = node.get_inputs_cloud()
             nbytes = node.get_estimated_inputs_size_gigabytes()
         else:
             src_cloud = parent_resources.cloud
             nbytes = parent.get_estimated_outputs_size_gigabytes()
         dst_cloud = resources.cloud
         return src_cloud, dst_cloud, nbytes
 
     @staticmethod
-    def _egress_cost_or_time(minimize_cost: bool, parent: Task,
+    def _egress_cost_or_time(minimize_cost: bool, parent: task_lib.Task,
                              parent_resources: resources_lib.Resources,
-                             node: Task, resources: resources_lib.Resources):
+                             node: task_lib.Task,
+                             resources: resources_lib.Resources):
         """Computes the egress cost or time depending on 'minimize_cost'."""
         src_cloud, dst_cloud, nbytes = Optimizer._get_egress_info(
             parent, parent_resources, node, resources)
         if nbytes == 0:
             return 0
+        assert src_cloud is not None and dst_cloud is not None
 
         if minimize_cost:
             fn = Optimizer._egress_cost
         else:
             fn = Optimizer._egress_time
         return fn(src_cloud, dst_cloud, nbytes)
 
     @staticmethod
     def _estimate_nodes_cost_or_time(
-        topo_order: List[Task],
+        topo_order: List[task_lib.Task],
         minimize_cost: bool = True,
-        blocked_resources: Optional[List[resources_lib.Resources]] = None,
+        blocked_resources: Optional[Iterable[resources_lib.Resources]] = None,
     ) -> Tuple[_TaskToCostMap, _TaskToPerCloudCandidates]:
         """Estimates the cost/time of each task-resource mapping in the DAG.
 
         Note that the egress cost/time is not considered in this function.
         The estimated run time of a task running on a resource is given by
         `task.estimate_runtime(resources)` or 1 hour by default.
         The estimated cost is `task.num_nodes * resources.get_cost(runtime)`.
@@ -248,25 +250,36 @@
                     _fill_in_launchable_resources(
                         node,
                         blocked_resources
                     )
                 node_to_candidate_map[node] = cloud_candidates
             else:
                 # Dummy sink node.
-                launchable_resources = node.get_resources()
-                launchable_resources = {
-                    list(node.get_resources())[0]: launchable_resources
-                }
+                node_resources = node.get_resources()
+                launchable_resources = {list(node_resources)[0]: node_resources}
 
             num_resources = len(node.get_resources())
             for orig_resources, launchable_list in launchable_resources.items():
                 if not launchable_list:
+                    location_hint = ''
+                    if node.get_resources():
+                        specified_resources = list(node.get_resources())[0]
+                        if specified_resources.zone is not None:
+                            location_hint = (
+                                f' Zone: {specified_resources.zone}.')
+                        elif specified_resources.region:
+                            location_hint = (
+                                f' Region: {specified_resources.region}.')
+
                     error_msg = (
-                        f'No launchable resource found for task {node}. '
-                        'To fix: relax its resource requirements.\n'
+                        'No launchable resource found for task '
+                        f'{node}.{location_hint}\nThis means the '
+                        'catalog does not contain any instance types that '
+                        'satisfy this request.\n'
+                        'To fix: relax or change the resource requirements.\n'
                         'Hint: \'sky show-gpus --all\' '
                         'to list available accelerators.\n'
                         '      \'sky check\' to check the enabled clouds.')
                     with ux_utils.print_exception_no_traceback():
                         raise exceptions.ResourcesUnavailableError(error_msg)
                 if num_resources == 1 and node.time_estimator_func is None:
                     logger.debug(
@@ -303,23 +316,27 @@
                                 '  estimated_cost (not incl. egress): ${:.1f}'.
                                 format(estimated_cost_or_time))
                     node_to_cost_map[node][resources] = estimated_cost_or_time
         return node_to_cost_map, node_to_candidate_map
 
     @staticmethod
     def _optimize_by_dp(
-        topo_order: List[Task],
+        topo_order: List[task_lib.Task],
         node_to_cost_map: _TaskToCostMap,
         minimize_cost: bool = True,
-    ) -> Tuple[Dict[Task, resources_lib.Resources], float]:
+    ) -> Tuple[Dict[task_lib.Task, resources_lib.Resources], float]:
         """Optimizes a chain DAG using a dynamic programming algorithm."""
         # node -> { resources -> best estimated cost }
-        dp_best_objective = collections.defaultdict(dict)
+        dp_best_objective: Dict[task_lib.Task,
+                                Dict[resources_lib.Resources,
+                                     float]] = collections.defaultdict(dict)
         # node -> { resources -> best parent resources }
-        dp_point_backs = collections.defaultdict(dict)
+        dp_point_backs: Dict[task_lib.Task, Dict[
+            resources_lib.Resources,
+            resources_lib.Resources]] = collections.defaultdict(dict)
 
         # Computes dp_best_objective[node][resources]
         # = my estimated cost + min_phw { dp_best_objective(p, phw) +
         #                                 egress_cost(p, phw, hw) }
         # where p is the parent of the node.
         for node_i, node in enumerate(topo_order):
             if node_i == 0:
@@ -360,19 +377,19 @@
             node.best_resources = best_resources
             if node.name != _DUMMY_SOURCE_NAME:
                 best_resources = dp_point_backs[node][best_resources]
         return best_plan, best_total_objective
 
     @staticmethod
     def _optimize_by_ilp(
-        graph,
-        topo_order: List[Task],
+        graph: 'nx.DiGraph',
+        topo_order: List[task_lib.Task],
         node_to_cost_map: _TaskToCostMap,
         minimize_cost: bool = True,
-    ) -> Tuple[Dict[Task, resources_lib.Resources], float]:
+    ) -> Tuple[Dict[task_lib.Task, resources_lib.Resources], float]:
         """Optimizes a general DAG using an ILP solver.
 
         Notations:
             V: the set of nodes (tasks).
             E: the set of edges (dependencies).
             k: node -> [r.cost for r in node.resources].
             F: (node i, node j) -> the egress cost/time between node i and j.
@@ -426,30 +443,32 @@
         # Prepare the constants.
         V = topo_order  # pylint: disable=invalid-name
         E = graph.edges()  # pylint: disable=invalid-name
         k = {
             node: list(resource_cost_map.values())
             for node, resource_cost_map in node_to_cost_map.items()
         }
-        F = collections.defaultdict(dict)  # pylint: disable=invalid-name
+        F: Dict[Any, Dict[Any, List[float]]] = collections.defaultdict(dict)  # pylint: disable=invalid-name
         for u, v in E:
             F[u][v] = []
             for r_u in node_to_cost_map[u].keys():
                 for r_v in node_to_cost_map[v].keys():
                     F[u][v].append(
                         Optimizer._egress_cost_or_time(minimize_cost, u, r_u, v,
                                                        r_v))
 
         # Define the decision variables.
         c = {
             v: pulp.LpVariable.matrix(v.name, (range(len(k[v])),), cat='Binary')
             for v in V
         }
 
-        e = collections.defaultdict(dict)
+        e: Dict[Any,
+                Dict[Any,
+                     List[pulp.LpVariable]]] = collections.defaultdict(dict)
         for u, v in E:
             num_vars = len(c[u]) * len(c[v])
             e[u][v] = pulp.LpVariable.matrix(f'({u.name}->{v.name})',
                                              (range(num_vars),),
                                              cat='Binary')
 
         # Formulate the constraints.
@@ -509,19 +528,19 @@
             node.best_resources = best_resources
             best_plan[node] = best_resources
         return best_plan, best_total_objective
 
     @staticmethod
     def _compute_total_time(
         graph,
-        topo_order: List[Task],
-        plan: Dict[Task, resources_lib.Resources],
+        topo_order: List[task_lib.Task],
+        plan: Dict[task_lib.Task, resources_lib.Resources],
     ) -> float:
         """Estimates the total time of running the DAG by the plan."""
-        cache_finish_time = {}
+        cache_finish_time: Dict[task_lib.Task, float] = {}
 
         def finish_time(node):
             if node in cache_finish_time:
                 return cache_finish_time[node]
 
             resources = plan[node]
             if node.time_estimator_func is None:
@@ -543,16 +562,16 @@
 
         sink_node = topo_order[-1]
         return finish_time(sink_node)
 
     @staticmethod
     def _compute_total_cost(
         graph,
-        topo_order: List[Task],
-        plan: Dict[Task, resources_lib.Resources],
+        topo_order: List[task_lib.Task],
+        plan: Dict[task_lib.Task, resources_lib.Resources],
     ) -> float:
         """Estimates the total cost of running the DAG by the plan."""
         total_cost = 0
         for node in topo_order:
             resources = plan[node]
             if node.time_estimator_func is None:
                 execution_time = 1 * 3600
@@ -603,16 +622,16 @@
             table = _create_table(['SOURCE', 'TARGET', 'SIZE (GB)', metric])
             table.add_rows(reversed(message_data))
             logger.info(f'Egress plan:\n{table}\n')
 
     @staticmethod
     def print_optimized_plan(
         graph,
-        topo_order: List[Task],
-        best_plan: Dict[Task, resources_lib.Resources],
+        topo_order: List[task_lib.Task],
+        best_plan: Dict[task_lib.Task, resources_lib.Resources],
         total_time: float,
         total_cost: float,
         node_to_cost_map: _TaskToCostMap,
         minimize_cost: bool,
     ):
         logger.info('== Optimizer ==')
         ordered_node_to_cost_map = collections.OrderedDict()
@@ -703,23 +722,25 @@
         Optimizer._print_egress_plan(graph, best_plan, minimize_cost)
 
         metric = 'COST ($)' if minimize_cost else 'TIME (hr)'
         field_names = resource_fields + [metric, 'CHOSEN']
 
         num_tasks = len(ordered_node_to_cost_map)
         for task, v in ordered_node_to_cost_map.items():
-            task_str = f'for Task {repr(task)!r}' if num_tasks > 1 else ''
+            task_str = (f'for task_lib.Task {repr(task)!r}'
+                        if num_tasks > 1 else '')
             plural = 's' if task.num_nodes > 1 else ''
             logger.info(
                 f'{colorama.Style.BRIGHT}Considered resources {task_str}'
                 f'({task.num_nodes} node{plural}):'
                 f'{colorama.Style.RESET_ALL}')
 
             # Only print 1 row per cloud.
-            best_per_cloud = {}
+            best_per_cloud: Dict[str, Tuple[resources_lib.Resources,
+                                            float]] = {}
             for resources, cost in v.items():
                 cloud = str(resources.cloud)
                 if cloud in best_per_cloud:
                     if cost < best_per_cloud[cloud][1]:
                         best_per_cloud[cloud] = (resources, cost)
                 else:
                     best_per_cloud[cloud] = (resources, cost)
@@ -729,19 +750,19 @@
             chosen_resources = best_plan[task]
             best_per_cloud[str(chosen_resources.cloud)] = (chosen_resources,
                                                            v[chosen_resources])
 
             rows = []
             for resources, cost in best_per_cloud.values():
                 if minimize_cost:
-                    cost = f'{cost:.2f}'
+                    cost_str = f'{cost:.2f}'
                 else:
-                    cost = f'{cost / 3600:.2f}'
+                    cost_str = f'{cost / 3600:.2f}'
 
-                row = [*_get_resources_element_list(resources), cost, '']
+                row = [*_get_resources_element_list(resources), cost_str, '']
                 if resources == best_plan[task]:
                     # Use tick sign for the chosen resources.
                     row[-1] = (colorama.Fore.GREEN + '   ' + u'\u2714' +
                                colorama.Style.RESET_ALL)
                 rows.append(row)
 
             # NOTE: we've converted the cost to a string above, so we should
@@ -781,17 +802,17 @@
                 logger.info(
                     f'To list more details, run \'sky show-gpus {acc_name}\'.')
 
     @staticmethod
     def _optimize_objective(
         dag: 'dag_lib.Dag',
         minimize_cost: bool = True,
-        blocked_resources: Optional[List[resources_lib.Resources]] = None,
+        blocked_resources: Optional[Iterable[resources_lib.Resources]] = None,
         quiet: bool = False,
-    ) -> Dict[Task, resources_lib.Resources]:
+    ) -> Dict[task_lib.Task, resources_lib.Resources]:
         """Finds the optimal task-resource mapping for the entire DAG.
 
         The optimal mapping should consider the egress cost/time so that
         the total estimated cost/time of the DAG becomes the minimum.
         """
         import networkx as nx  # pylint: disable=import-outside-toplevel
         # TODO: The output of this function is useful. Should generate a
@@ -839,19 +860,18 @@
 
     def get_cost(self, seconds):
         return 0
 
 
 class DummyCloud(clouds.Cloud):
     """A dummy Cloud that has zero egress cost from/to."""
-    _REPR = 'DummyCloud'
     pass
 
 
-def _cloud_in_list(cloud: clouds.Cloud, lst: List[clouds.Cloud]) -> bool:
+def _cloud_in_list(cloud: clouds.Cloud, lst: Iterable[clouds.Cloud]) -> bool:
     return any(cloud.is_same_cloud(c) for c in lst)
 
 
 def _make_launchables_for_valid_region_zones(
     launchable_resources: resources_lib.Resources
 ) -> List[resources_lib.Resources]:
     assert launchable_resources.is_launchable()
@@ -888,51 +908,54 @@
             # On-demand instances.
             # Batch the requests at the granularity of a single region.
             launchables.append(launchable_resources.copy(region=region.name))
     return launchables
 
 
 def _filter_out_blocked_launchable_resources(
-        launchable_resources: List[resources_lib.Resources],
-        blocked_resources: List[resources_lib.Resources]):
+        launchable_resources: Iterable[resources_lib.Resources],
+        blocked_resources: Iterable[resources_lib.Resources]):
     """Whether the resources are blocked."""
     available_resources = []
     for resources in launchable_resources:
         for blocked in blocked_resources:
             if resources.should_be_blocked_by(blocked):
                 break
         else:  # non-blocked launchable resources. (no break)
             available_resources.append(resources)
     return available_resources
 
 
 def _fill_in_launchable_resources(
-    task: Task,
-    blocked_resources: Optional[List[resources_lib.Resources]],
+    task: task_lib.Task,
+    blocked_resources: Optional[Iterable[resources_lib.Resources]],
     try_fix_with_sky_check: bool = True,
 ) -> Tuple[Dict[resources_lib.Resources, List[resources_lib.Resources]],
            _PerCloudCandidates]:
     backend_utils.check_public_cloud_enabled()
     enabled_clouds = global_user_state.get_enabled_clouds()
     launchable = collections.defaultdict(list)
-    cloud_candidates = collections.defaultdict(resources_lib.Resources)
+    cloud_candidates: Dict[clouds.Cloud,
+                           resources_lib.Resources] = collections.defaultdict(
+                               resources_lib.Resources)
     if blocked_resources is None:
         blocked_resources = []
     for resources in task.get_resources():
         if resources.cloud is not None and not _cloud_in_list(
                 resources.cloud, enabled_clouds):
             if try_fix_with_sky_check:
                 # Explicitly check again to update the enabled cloud list.
                 check.check(quiet=True)
                 return _fill_in_launchable_resources(task, blocked_resources,
                                                      False)
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.ResourcesUnavailableError(
-                    f'Task {task} requires {resources.cloud} which is not '
-                    f'enabled. To enable access, run {colorama.Style.BRIGHT}'
+                    f'task_lib.Task {task} requires {resources.cloud} which is '
+                    'not enabled. To enable access, run '
+                    f'{colorama.Style.BRIGHT}'
                     f'sky check {colorama.Style.RESET_ALL}, or change the '
                     'cloud requirement')
         elif resources.is_launchable():
             if isinstance(resources.cloud, clouds.GCP):
                 # Check if the host VM satisfies the max vCPU and memory limits.
                 clouds.GCP.check_accelerator_attachable_to_host(
                     resources.instance_type, resources.accelerators,
@@ -970,16 +993,18 @@
                     # Generate region/zone-specified resources.
                     launchable[resources].extend(
                         _make_launchables_for_valid_region_zones(cheapest))
                     cloud_candidates[cloud] = feasible_resources
                 else:
                     all_fuzzy_candidates.update(fuzzy_candidate_list)
             if len(launchable[resources]) == 0:
+                clouds_str = str(clouds_list) if len(clouds_list) > 1 else str(
+                    clouds_list[0])
                 logger.info(f'No resource satisfying {resources} '
-                            f'on {clouds_list}.')
+                            f'on {clouds_str}.')
                 if len(all_fuzzy_candidates) > 0:
                     logger.info('Did you mean: '
                                 f'{colorama.Fore.CYAN}'
                                 f'{sorted(all_fuzzy_candidates)}'
                                 f'{colorama.Style.RESET_ALL}')
                 else:
                     if resources.cpus is not None:
```

### Comparing `skypilot-0.2.5/sky/resources.py` & `skypilot-0.3.0/sky/resources.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Resources: compute requirements of Tasks."""
 from typing import Dict, List, Optional, Union
+from typing_extensions import Literal
 
 from sky import clouds
 from sky import global_user_state
 from sky import sky_logging
 from sky import spot
 from sky.backends import backend_utils
 from sky.utils import accelerator_registry
@@ -40,15 +41,15 @@
         sky.Resources(accelerators={'V100': 1})
 
         # TODO:
         sky.Resources(requests={'mem': '16g', 'cpu': 8})
     """
     # If any fields changed, increment the version. For backward compatibility,
     # modify the __setstate__ method to handle the old version.
-    _VERSION = 8
+    _VERSION = 9
 
     def __init__(
         self,
         cloud: Optional[clouds.Cloud] = None,
         instance_type: Optional[str] = None,
         cpus: Union[None, int, float, str] = None,
         memory: Union[None, int, float, str] = None,
@@ -56,14 +57,15 @@
         accelerator_args: Optional[Dict[str, str]] = None,
         use_spot: Optional[bool] = None,
         spot_recovery: Optional[str] = None,
         disk_size: Optional[int] = None,
         region: Optional[str] = None,
         zone: Optional[str] = None,
         image_id: Union[Dict[str, str], str, None] = None,
+        disk_tier: Optional[Literal['high', 'medium', 'low']] = None,
     ):
         self._version = self._VERSION
         self._cloud = cloud
         self._region: Optional[str] = None
         self._zone: Optional[str] = None
         self._set_region_zone(region, zone)
 
@@ -93,24 +95,27 @@
             if None in image_id:
                 self._image_id = {self._region: image_id[None].strip()}
             else:
                 self._image_id = {
                     k.strip(): v.strip() for k, v in image_id.items()
                 }
 
+        self._disk_tier = disk_tier
+
         self._set_cpus(cpus)
         self._set_memory(memory)
         self._set_accelerators(accelerators, accelerator_args)
 
         self._try_validate_local()
         self._try_validate_instance_type()
         self._try_validate_cpus_mem()
         self._try_validate_accelerators()
         self._try_validate_spot()
         self._try_validate_image_id()
+        self._try_validate_disk_tier()
 
     def __repr__(self) -> str:
         """Returns a string representation for display.
 
         Examples:
 
             >>> sky.Resources(accelerators='V100')
@@ -157,27 +162,34 @@
         image_id = ''
         if self.image_id is not None:
             if None in self.image_id:
                 image_id = f', image_id={self.image_id[None]}'
             else:
                 image_id = f', image_id={self.image_id!r}'
 
+        disk_tier = ''
+        if self.disk_tier is not None:
+            disk_tier = f', disk_tier={self.disk_tier}'
+
         disk_size = ''
         if self.disk_size != _DEFAULT_DISK_SIZE_GB:
             disk_size = f', disk_size={self.disk_size}'
 
         if self._instance_type is not None:
             instance_type = f'{self._instance_type}'
         else:
             instance_type = ''
 
+        # Do not show region/zone here as `sky status -a` would show them as
+        # separate columns. Also, Resources repr will be printed during
+        # failover, and the region may be dynamically determined.
         hardware_str = (
             f'{instance_type}{use_spot}'
             f'{cpus}{memory}{accelerators}{accelerator_args}{image_id}'
-            f'{disk_size}')
+            f'{disk_tier}{disk_size}')
         # It may have leading ',' (for example, instance_type not set) or empty
         # spaces.  Remove them.
         while hardware_str and hardware_str[0] in (',', ' '):
             hardware_str = hardware_str[1:]
 
         cloud_str = '<Cloud>'
         if self.cloud is not None:
@@ -263,14 +275,18 @@
     def disk_size(self) -> int:
         return self._disk_size
 
     @property
     def image_id(self) -> Optional[Dict[str, str]]:
         return self._image_id
 
+    @property
+    def disk_tier(self) -> str:
+        return self._disk_tier
+
     def _set_cpus(
         self,
         cpus: Union[None, int, float, str],
     ) -> None:
         if cpus is None:
             self._cpus = None
             return
@@ -628,18 +644,20 @@
 
         if self.cloud is None:
             with ux_utils.print_exception_no_traceback():
                 raise ValueError(
                     'Cloud must be specified when image_id is provided.')
 
         if not self._cloud.is_same_cloud(
-                clouds.AWS()) and not self._cloud.is_same_cloud(clouds.GCP()):
+                clouds.IBM()) and not self._cloud.is_same_cloud(
+                    clouds.AWS()) and not self._cloud.is_same_cloud(
+                        clouds.GCP()):
             with ux_utils.print_exception_no_traceback():
                 raise ValueError(
-                    'image_id is only supported for AWS and GCP, please '
+                    'image_id is only supported for AWS, GCP and IBM, please '
                     'explicitly specify the cloud.')
 
         if self._region is not None:
             if self._region not in self._image_id:
                 with ux_utils.print_exception_no_traceback():
                     raise ValueError(
                         f'image_id {self._image_id} should contain the image '
@@ -673,14 +691,28 @@
                 with ux_utils.print_exception_no_traceback():
                     raise ValueError(
                         f'Image {image_id!r} is {image_size}GB, which is '
                         f'larger than the specified disk_size: {self.disk_size}'
                         ' GB. Please specify a larger disk_size to use this '
                         'image.')
 
+    def _try_validate_disk_tier(self) -> None:
+        if self.disk_tier is None:
+            return
+        if self.disk_tier not in ['high', 'medium', 'low']:
+            with ux_utils.print_exception_no_traceback():
+                raise ValueError(
+                    f'Invalid disk_tier {self.disk_tier}. '
+                    'Please use one of "high", "medium", or "low".')
+        if self.instance_type is None:
+            return
+        if self.cloud is not None:
+            self.cloud.check_disk_tier_enabled(self.instance_type,
+                                               self.disk_tier)
+
     def get_cost(self, seconds: float) -> float:
         """Returns cost in USD for the runtime in seconds."""
         hours = seconds / 3600
         # Instance.
         hourly_cost = self.cloud.instance_type_to_hourly_cost(
             self._instance_type, self.use_spot, self._region, self._zone)
         # Accelerators (if any).
@@ -750,14 +782,22 @@
                 self.accelerator_args != other.accelerator_args):
             return False
         # self.accelerator_args == other.accelerator_args
 
         if self.use_spot_specified and self.use_spot != other.use_spot:
             return False
 
+        if self.disk_tier is not None:
+            if other.disk_tier is None:
+                return False
+            if self.disk_tier != other.disk_tier:
+                types = ['low', 'medium', 'high']
+                return types.index(self.disk_tier) < types.index(
+                    other.disk_tier)
+
         # self <= other
         return True
 
     def should_be_blocked_by(self, blocked: 'Resources') -> bool:
         """Whether this Resources matches the blocked Resources.
 
         If a field in `blocked` is None, it should be considered as a wildcard
@@ -804,14 +844,15 @@
                                           self.accelerator_args),
             use_spot=override.pop('use_spot', use_spot),
             spot_recovery=override.pop('spot_recovery', self.spot_recovery),
             disk_size=override.pop('disk_size', self.disk_size),
             region=override.pop('region', self.region),
             zone=override.pop('zone', self.zone),
             image_id=override.pop('image_id', self.image_id),
+            disk_tier=override.pop('disk_tier', self.disk_tier),
         )
         assert len(override) == 0
         return resources
 
     def valid_on_region_zones(self, region: str, zones: List[str]) -> bool:
         """Returns whether this Resources is valid on given region and zones"""
         if self.region is not None and self.region != region:
@@ -854,16 +895,18 @@
             resources_fields['disk_size'] = int(config.pop('disk_size'))
         if config.get('region') is not None:
             resources_fields['region'] = config.pop('region')
         if config.get('zone') is not None:
             resources_fields['zone'] = config.pop('zone')
         if config.get('image_id') is not None:
             logger.warning('image_id in resources is experimental. It only '
-                           'supports AWS/GCP.')
+                           'supports AWS/GCP/IBM.')
             resources_fields['image_id'] = config.pop('image_id')
+        if config.get('disk_tier') is not None:
+            resources_fields['disk_tier'] = config.pop('disk_tier')
 
         assert not config, f'Invalid resource args: {config.keys()}'
         return Resources(**resources_fields)
 
     def to_yaml_config(self) -> Dict[str, Union[str, int]]:
         """Returns a yaml-style dict of config for this resource bundle."""
         config = {}
@@ -882,14 +925,15 @@
         if self._use_spot_specified:
             add_if_not_none('use_spot', self.use_spot)
         config['spot_recovery'] = self.spot_recovery
         config['disk_size'] = self.disk_size
         add_if_not_none('region', self.region)
         add_if_not_none('zone', self.zone)
         add_if_not_none('image_id', self.image_id)
+        add_if_not_none('disk_tier', self.disk_tier)
         return config
 
     def __setstate__(self, state):
         """Set state from pickled state, for backward compatibility."""
         self._version = self._VERSION
 
         # TODO (zhwu): Design our persistent state format with `__getstate__`,
@@ -941,8 +985,11 @@
         if version < 8:
             self._memory = None
 
         image_id = state.get('_image_id', None)
         if isinstance(image_id, str):
             state['_image_id'] = {state.get('_region', None): image_id}
 
+        if version < 9:
+            self._disk_tier = None
+
         self.__dict__.update(state)
```

### Comparing `skypilot-0.2.5/sky/setup_files/setup.py` & `skypilot-0.3.0/sky/setup_files/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,17 +61,16 @@
         re.MULTILINE)
     readme = mode_re.sub(r'<img\1>', readme)
     return readme
 
 
 install_requires = [
     'wheel',
-    # NOTE: ray 2.0.1 requires click<=8.0.4,>=7.0; We disable the
-    # shell completion for click<8.0 for backward compatibility.
-    'click<=8.0.4,>=7.0',
+    # NOTE: ray requires click>=7.0
+    'click>=7.0',
     # NOTE: required by awscli. To avoid ray automatically installing
     # the latest version.
     'colorama<0.4.5',
     'cryptography',
     # Jinja has a bug in older versions because of the lack of pinning
     # the version of the underlying markupsafe package. See:
     # https://github.com/pallets/jinja/issues/1585
@@ -80,51 +79,63 @@
     'networkx',
     'oauth2client',
     'pandas',
     'pendulum',
     # PrettyTable with version >=2.0.0 is required for the support of
     # `add_rows` method.
     'PrettyTable>=2.0.0',
-    # Lower local ray version is not fully supported, due to the
-    # autoscaler issues (also tracked in #537).
-    'ray[default]>=1.9.0,<=2.3.0',
+    # Lower version of ray will cause dependency conflict for
+    # click/grpcio/protobuf.
+    'ray[default]>=2.2.0,<=2.4.0',
     'rich',
     'tabulate',
-    'typing-extensions',
-    'filelock',  # TODO(mraheja): Enforce >=3.6.0 when python version is >= 3.7
-    # This is used by ray. The latest 1.44.0 will generate an error
-    # `Fork support is only compatible with the epoll1 and poll
-    # polling strategies`
-    'grpcio>=1.32.0,<=1.43.0',
+    # Light weight requirement, can be replaced with "typing" once
+    # we deprecate Python 3.7 (this will take a while).
+    "typing_extensions; python_version < '3.8'",
+    'filelock>=3.6.0',
+    # Adopted from ray's setup.py:
+    # Tracking issue: https://github.com/ray-project/ray/issues/30984
+    "grpcio >= 1.32.0, <= 1.49.1; python_version < '3.10' and sys_platform == 'darwin'",  # noqa:E501
+    "grpcio >= 1.42.0, <= 1.49.1; python_version >= '3.10' and sys_platform == 'darwin'",  # noqa:E501
+    # Original issue: https://github.com/ray-project/ray/issues/33833
+    "grpcio >= 1.32.0, <= 1.51.3; python_version < '3.10' and sys_platform != 'darwin'",  # noqa:E501
+    "grpcio >= 1.42.0, <= 1.51.3; python_version >= '3.10' and sys_platform != 'darwin'",  # noqa:E501
     'packaging',
-    # The latest 4.21.1 will break ray. Enforce < 4.0.0 until Ray releases the
-    # fix.
-    # https://github.com/ray-project/ray/pull/25211
-    'protobuf<4.0.0',
+    # Adopted from ray's setup.py:
+    # https://github.com/ray-project/ray/blob/86fab1764e618215d8131e8e5068f0d493c77023/python/setup.py#L326
+    'protobuf >= 3.15.3, != 3.19.5',
     'psutil',
     'pulp',
 ]
 
 # NOTE: Change the templates/spot-controller.yaml.j2 file if any of the following
 # packages dependencies are changed.
+aws_dependencies = [
+    # awscli>=1.27.10 is required for SSO support.
+    'awscli',
+    'boto3',
+    # 'Crypto' module used in authentication.py for AWS.
+    'pycryptodome==3.12.0',
+]
 extras_require: Dict[str, List[str]] = {
-    'aws': [
-        # awscli>=1.27.10 is required for SSO support.
-        'awscli',
-        'boto3',
-        # 'Crypto' module used in authentication.py for AWS.
-        'pycryptodome==3.12.0',
-    ],
+    'aws': aws_dependencies,
     # TODO(zongheng): azure-cli is huge and takes a long time to install.
     # Tracked in: https://github.com/Azure/azure-cli/issues/7387
     # azure-identity is needed in node_provider.
-    'azure': ['azure-cli>=2.31.0', 'azure-core', 'azure-identity'],
+    # We need azure-identity>=1.13.0 to enable the customization of the
+    # timeout of AzureCliCredential.
+    'azure': [
+        'azure-cli>=2.31.0', 'azure-core', 'azure-identity>=1.13.0',
+        'azure-mgmt-network'
+    ],
     'gcp': ['google-api-python-client', 'google-cloud-storage'],
+    'ibm': ['ibm-cloud-sdk-core', 'ibm-vpc', 'ibm-platform-services'],
     'docker': ['docker'],
     'lambda': [],
+    'cloudflare': aws_dependencies
 }
 
 extras_require['all'] = sum(extras_require.values(), [])
 
 # Install aws requirements by default, as it is the most common cloud provider,
 # and the installation is quick.
 install_requires += extras_require['aws']
@@ -147,23 +158,22 @@
     author='SkyPilot Team',
     license='Apache 2.0',
     readme='README.md',
     description='SkyPilot: An intercloud broker for the clouds',
     long_description=long_description,
     long_description_content_type='text/markdown',
     setup_requires=['wheel'],
-    requires_python='>=3.6',
+    requires_python='>=3.7',
     install_requires=install_requires,
     extras_require=extras_require,
     entry_points={
         'console_scripts': ['sky = sky.cli:cli'],
     },
     include_package_data=True,
     classifiers=[
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

### Comparing `skypilot-0.2.5/sky/sky_logging.py` & `skypilot-0.3.0/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/skylet/LICENCE` & `skypilot-0.3.0/sky/skylet/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -199,27 +199,27 @@
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 
 --------------------------------------------------------------------------------
 
 Code in providers/azure from
-https://github.com/ray-project/ray/tree/ray-2.0.1/python/ray/autoscaler/_private/_azure
-Git commit of the release 2.0.1: 03b6bc7b5a305877501110ec04710a9c57011479
+https://github.com/ray-project/ray/tree/ray-2.4.0/python/ray/autoscaler/_private/_azure
+Git commit of the release 2.4.0: a777a028b8dbd7bbae9a7393c98f6cd65f98a5f5
 
 Code in providers/gcp from
-https://github.com/ray-project/ray/tree/ray-2.0.1/python/ray/autoscaler/_private/gcp
-Git commit of the release 2.0.1: 03b6bc7b5a305877501110ec04710a9c57011479
+https://github.com/ray-project/ray/tree/ray-2.4.0/python/ray/autoscaler/_private/gcp
+Git commit of the release 2.4.0: 45ffe6eb99d96488fdec187bb47a4a78d9b5ee92
 
 Code in providers/aws from
-https://github.com/ray-project/ray/tree/ray-2.0.1/python/ray/autoscaler/_private/aws
-Git commit of the release 2.0.1: 03b6bc7b5a305877501110ec04710a9c57011479
+https://github.com/ray-project/ray/tree/ray-2.4.0/python/ray/autoscaler/_private/aws
+Git commit of the release 2.4.0: c27859fa49f6470b98743bdce8288c7242d89699
 
 
-Copyright 2016-2022 Ray developers
+Copyright 2016-2023 Ray developers
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `skypilot-0.2.5/sky/skylet/autostop_lib.py` & `skypilot-0.3.0/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/skylet/configs.py` & `skypilot-0.3.0/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/skylet/events.py` & `skypilot-0.3.0/sky/skylet/events.py`

 * *Files 16% similar despite different names*

```diff
@@ -126,44 +126,74 @@
                 f'{autostop_config.autostop_idle_minutes} minutes. Stopping.')
             self._stop_cluster(autostop_config)
 
     def _stop_cluster(self, autostop_config):
         if (autostop_config.backend ==
                 cloud_vm_ray_backend.CloudVmRayBackend.NAME):
             autostop_lib.set_autostopping_started()
+
+            config = common_utils.read_yaml(self._ray_yaml_path)
+            is_cluster_multinode = config['max_workers'] > 0
+
+            # Even for !is_cluster_multinode, we want to call this to replace
+            # cache_stopped_nodes.
             self._replace_yaml_for_stopping(self._ray_yaml_path,
                                             autostop_config.down)
 
-            # `ray up` is required to reset the upscaling speed and min/max
-            # workers. Otherwise, `ray down --workers-only` will continuously
-            # scale down and up.
-            logger.info('Running ray up.')
-            script = (cloud_vm_ray_backend.
-                      write_ray_up_script_with_patched_launch_hash_fn(
-                          self._ray_yaml_path,
-                          ray_up_kwargs={'restart_only': True}))
-            subprocess.run(
-                [sys.executable, script],
-                check=True,
-                # Use environment variables to disable the ray usage collection
-                # (to avoid overheads and potential issues with the usage)
-                # as sdk does not take the argument for disabling the usage
-                # collection.
-                env=dict(os.environ, RAY_USAGE_STATS_ENABLED='0'),
-            )
+            # Use environment variables to disable the ray usage collection (to
+            # avoid overheads and potential issues with the usage) as sdk does
+            # not take the argument for disabling the usage collection.
+            #
+            # Also clear any cloud-specific credentials set as env vars (e.g.,
+            # AWS's two env vars). Reason: for single-node AWS SSO clusters, we
+            # have seen a weird bug where user image's /etc/profile.d may
+            # contain the two AWS env vars, and so they take effect in the
+            # bootstrap phase of each of these 3 'ray' commands, throwing a
+            # RuntimeError when some private VPC is not found (since the VPC
+            # only exists in the assumed role, not in the custome principal set
+            # by the env vars).  See #1880 for details.
+            env = dict(os.environ, RAY_USAGE_STATS_ENABLED='0')
+            env.pop('AWS_ACCESS_KEY_ID', None)
+            env.pop('AWS_SECRET_ACCESS_KEY', None)
 
-            logger.info('Running ray down.')
-            # Stop the workers first to avoid orphan workers.
-            subprocess.run(
-                ['ray', 'down', '-y', '--workers-only', self._ray_yaml_path],
-                check=True)
+            # We do "initial ray up + ray down --workers-only" only for
+            # multinode clusters as they are not needed for single-node.
+            if is_cluster_multinode:
+                # `ray up` is required to reset the upscaling speed and min/max
+                # workers. Otherwise, `ray down --workers-only` will
+                # continuously scale down and up.
+                logger.info('Running ray up.')
+                script = (cloud_vm_ray_backend.
+                          write_ray_up_script_with_patched_launch_hash_fn(
+                              self._ray_yaml_path,
+                              ray_up_kwargs={'restart_only': True}))
+                # Passing env inherited from os.environ is technically not
+                # needed, because we call `python <script>` rather than `ray
+                # <cmd>`. We just need the {RAY_USAGE_STATS_ENABLED: 0} part.
+                subprocess.run([sys.executable, script], check=True, env=env)
+
+                logger.info('Running ray down.')
+                # Stop the workers first to avoid orphan workers.
+                subprocess.run(
+                    [
+                        'ray', 'down', '-y', '--workers-only',
+                        self._ray_yaml_path
+                    ],
+                    check=True,
+                    # We pass env inherited from os.environ due to calling `ray
+                    # <cmd>`.
+                    env=env)
 
             logger.info('Running final ray down.')
-            subprocess.run(['ray', 'down', '-y', self._ray_yaml_path],
-                           check=True)
+            subprocess.run(
+                ['ray', 'down', '-y', self._ray_yaml_path],
+                check=True,
+                # We pass env inherited from os.environ due to calling `ray
+                # <cmd>`.
+                env=env)
         else:
             raise NotImplementedError
 
     def _replace_yaml_for_stopping(self, yaml_path: str, down: bool):
         with open(yaml_path, 'r') as f:
             yaml_str = f.read()
         yaml_str = self._UPSCALING_PATTERN.sub(r'upscaling_speed: 0', yaml_str)
```

### Comparing `skypilot-0.2.5/sky/skylet/job_lib.py` & `skypilot-0.3.0/sky/skylet/job_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Sky job lib, backed by a sqlite database.
 
 This is a remote utility module that provides job queue functionality.
 """
 import enum
+import json
 import os
 import pathlib
 import shlex
 import time
 import typing
 from typing import Any, Dict, List, Optional
 
@@ -169,15 +170,17 @@
         raise
     try:
         from ray import job_submission  # pylint: disable=import-outside-toplevel
     except ImportError:
         logger.error(
             f'Failed to import job_submission with ray=={ray.__version__}')
         raise
-    return job_submission.JobSubmissionClient(address='http://127.0.0.1:8265')
+    port = get_job_submission_port()
+    return job_submission.JobSubmissionClient(
+        address=f'http://127.0.0.1:{port}')
 
 
 def make_ray_job_id(sky_job_id: int, job_owner: str) -> str:
     return f'{sky_job_id}-{job_owner}'
 
 
 def make_job_command_with_user_switching(username: str,
@@ -315,14 +318,22 @@
     rows = _CURSOR.execute(f'SELECT {field} FROM jobs WHERE job_id=(?)',
                            (job_id,))
     for (timestamp,) in rows:
         return common_utils.encode_payload(timestamp)
     return common_utils.encode_payload(None)
 
 
+def get_job_submission_port():
+    port_path = os.path.expanduser(constants.SKY_REMOTE_RAY_PORT_FILE)
+    if not os.path.exists(port_path):
+        return 8265
+    port = json.load(open(port_path))['ray_dashboard_port']
+    return port
+
+
 def _get_records_from_rows(rows) -> List[Dict[str, Any]]:
     records = []
     for row in rows:
         if row[0] is None:
             break
         # TODO: use namedtuple instead of dict
         records.append({
@@ -388,25 +399,25 @@
     This function queries `ray job status` and processes those results to match
     our semantics.
 
     Though we update job status actively in the generated ray program and
     during job cancelling, we still need this to handle the staleness problem,
     caused by instance restarting and other corner cases (if any).
 
-    This function should only be run on the remote instance with ray==2.0.1.
+    This function should only be run on the remote instance with ray==2.4.0.
     """
     if len(job_ids) == 0:
         return []
 
     # TODO: if too slow, directly query against redis.
     ray_job_ids = [make_ray_job_id(job_id, job_owner) for job_id in job_ids]
 
     job_client = _create_ray_job_submission_client()
 
-    # In ray 2.0.1, job_client.list_jobs returns a list of JobDetails,
+    # In ray 2.4.0, job_client.list_jobs returns a list of JobDetails,
     # which contains the job status (str) and submission_id (str).
     job_detail_lists: List['ray_pydantic.JobDetails'] = job_client.list_jobs()
 
     job_details = {}
     ray_job_ids_set = set(ray_job_ids)
     for job_detail in job_detail_lists:
         if job_detail.submission_id in ray_job_ids_set:
@@ -636,15 +647,15 @@
 
       >> codegen = JobLibCodeGen.add_job(...)
     """
 
     _PREFIX = ['import os', 'from sky.skylet import job_lib, log_lib']
 
     @classmethod
-    def add_job(cls, job_name: str, username: str, run_timestamp: str,
+    def add_job(cls, job_name: Optional[str], username: str, run_timestamp: str,
                 resources_str: str) -> str:
         if job_name is None:
             job_name = '-'
         code = [
             'job_id = job_lib.add_job('
             f'{job_name!r}, '
             f'{username!r}, '
```

### Comparing `skypilot-0.2.5/sky/skylet/log_lib.py` & `skypilot-0.3.0/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py` & `skypilot-0.3.0/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import copy
 import hashlib
 import json
 import logging
 import os
 import time
-from typing import Any, Dict, List, Tuple, Union
+from enum import Enum
+from typing import Any, Callable, Dict, List, Union
 
 import botocore
 
 from sky.skylet.providers.aws.utils import client_cache, resource_cache
 from ray.autoscaler.tags import NODE_KIND_HEAD, TAG_RAY_CLUSTER_NAME, TAG_RAY_NODE_KIND
 
 logger = logging.getLogger(__name__)
@@ -17,40 +18,61 @@
 CLOUDWATCH_RAY_INSTANCE_PROFILE = RAY + "-cloudwatch-v1"
 CLOUDWATCH_RAY_IAM_ROLE = RAY + "-cloudwatch-v1"
 CLOUDWATCH_AGENT_INSTALLED_AMI_TAG = "T6Iq2faj"
 CLOUDWATCH_AGENT_INSTALLED_TAG = "cloudwatch-agent-installed"
 CLOUDWATCH_CONFIG_HASH_TAG_BASE = "cloudwatch-config-hash"
 
 
+class CloudwatchConfigType(str, Enum):
+    AGENT = "agent"
+    DASHBOARD = "dashboard"
+    ALARM = "alarm"
+
+
 class CloudwatchHelper:
     def __init__(
         self, provider_config: Dict[str, Any], node_id: str, cluster_name: str
     ) -> None:
         self.node_id = node_id
         self.cluster_name = cluster_name
         self.provider_config = provider_config
         region = provider_config["region"]
         self.ec2_resource = resource_cache("ec2", region)
         self.ec2_client = self.ec2_resource.meta.client
         self.ssm_client = client_cache("ssm", region)
         cloudwatch_resource = resource_cache("cloudwatch", region)
         self.cloudwatch_client = cloudwatch_resource.meta.client
+        self.CLOUDWATCH_CONFIG_TYPE_TO_CONFIG_VARIABLE_REPLACE_FUNC: Dict[
+            str, Callable
+        ] = {
+            CloudwatchConfigType.AGENT.value: self._replace_cwa_config_vars,
+            CloudwatchConfigType.DASHBOARD.value: self._replace_dashboard_config_vars,
+            CloudwatchConfigType.ALARM.value: self._load_config_file,
+        }
+        self.CLOUDWATCH_CONFIG_TYPE_TO_UPDATE_FUNC_HEAD_NODE: Dict[str, Callable] = {
+            CloudwatchConfigType.AGENT.value: self._restart_cloudwatch_agent,
+            CloudwatchConfigType.DASHBOARD.value: self._put_cloudwatch_dashboard,
+            CloudwatchConfigType.ALARM.value: self._put_cloudwatch_alarm,
+        }
+        self.CLOUDWATCH_CONFIG_TYPE_TO_UPDATE_FUNC_WORKER_NODE: Dict[str, Callable] = {
+            CloudwatchConfigType.AGENT.value: self._restart_cloudwatch_agent,
+            CloudwatchConfigType.ALARM.value: self._put_cloudwatch_alarm,
+        }
 
     def update_from_config(self, is_head_node: bool) -> None:
         """Discovers and applies CloudWatch config updates as required.
 
         Args:
             is_head_node: whether this node is the head node.
         """
-        if CloudwatchHelper.cloudwatch_config_exists(self.provider_config, "agent"):
-            self._update_cloudwatch_config(is_head_node, "agent")
-        if CloudwatchHelper.cloudwatch_config_exists(self.provider_config, "dashboard"):
-            self._update_cloudwatch_config(is_head_node, "dashboard")
-        if CloudwatchHelper.cloudwatch_config_exists(self.provider_config, "alarm"):
-            self._update_cloudwatch_config(is_head_node, "alarm")
+        for config_type in CloudwatchConfigType:
+            if CloudwatchHelper.cloudwatch_config_exists(
+                self.provider_config, config_type.value
+            ):
+                self._update_cloudwatch_config(config_type.value, is_head_node)
 
     def _ec2_health_check_waiter(self, node_id: str) -> None:
         # wait for all EC2 instance checks to complete
         try:
             logger.info(
                 "Waiting for EC2 instance health checks to complete before "
                 "configuring Unified Cloudwatch Agent. This may take a few "
@@ -62,69 +84,67 @@
             logger.error(
                 "Failed while waiting for EC2 instance checks to complete: {}".format(
                     e.message
                 )
             )
             raise e
 
-    def _update_cloudwatch_config(self, is_head_node: bool, config_type: str) -> None:
-        """Update remote CloudWatch configs at Parameter Store,
-        update hash tag value on node and perform associated operations
-        at CloudWatch console if local CloudWatch configs change.
-
-        Args:
-            is_head_node: whether this node is the head node.
-            config_type: CloudWatch config file type.
+    def _update_cloudwatch_config(self, config_type: str, is_head_node: bool) -> None:
+        """
+        check whether update operations are needed in
+        cloudwatch related configs
         """
         cwa_installed = self._setup_cwa()
         param_name = self._get_ssm_param_name(config_type)
         if cwa_installed:
             if is_head_node:
                 cw_config_ssm = self._set_cloudwatch_ssm_config_param(
                     param_name, config_type
                 )
                 cur_cw_config_hash = self._sha1_hash_file(config_type)
                 ssm_cw_config_hash = self._sha1_hash_json(cw_config_ssm)
-                # check if user updated Unified Cloudwatch Agent config file.
+                # check if user updated cloudwatch related config files.
                 # if so, perform corresponding actions.
                 if cur_cw_config_hash != ssm_cw_config_hash:
                     logger.info(
                         "Cloudwatch {} config file has changed.".format(config_type)
                     )
                     self._upload_config_to_ssm_and_set_hash_tag(config_type)
-                    if config_type == "agent":
-                        self._restart_cloudwatch_agent()
-                    elif config_type == "dashboard":
-                        self._put_cloudwatch_dashboard()
-                    elif config_type == "alarm":
-                        self._put_cloudwatch_alarm()
+                    self.CLOUDWATCH_CONFIG_TYPE_TO_UPDATE_FUNC_HEAD_NODE.get(
+                        config_type
+                    )()
             else:
                 head_node_hash = self._get_head_node_config_hash(config_type)
                 cur_node_hash = self._get_cur_node_config_hash(config_type)
                 if head_node_hash != cur_node_hash:
                     logger.info(
                         "Cloudwatch {} config file has changed.".format(config_type)
                     )
-                    if config_type == "agent":
-                        self._restart_cloudwatch_agent()
-                    if config_type == "alarm":
-                        self._put_cloudwatch_alarm()
+                    update_func = (
+                        self.CLOUDWATCH_CONFIG_TYPE_TO_UPDATE_FUNC_WORKER_NODE.get(
+                            config_type
+                        )
+                    )
+                    if update_func:
+                        update_func()
                     self._update_cloudwatch_hash_tag_value(
                         self.node_id, head_node_hash, config_type
                     )
 
     def _put_cloudwatch_dashboard(self) -> Dict[str, Any]:
         """put dashboard to cloudwatch console"""
 
         cloudwatch_config = self.provider_config["cloudwatch"]
         dashboard_config = cloudwatch_config.get("dashboard", {})
         dashboard_name_cluster = dashboard_config.get("name", self.cluster_name)
         dashboard_name = self.cluster_name + "-" + dashboard_name_cluster
 
-        widgets = self._replace_dashboard_config_variables()
+        widgets = self._replace_dashboard_config_vars(
+            CloudwatchConfigType.DASHBOARD.value
+        )
 
         response = self.cloudwatch_client.put_dashboard(
             DashboardName=dashboard_name, DashboardBody=json.dumps({"widgets": widgets})
         )
         issue_count = len(response.get("DashboardValidationMessages", []))
         if issue_count > 0:
             for issue in response.get("DashboardValidationMessages"):
@@ -140,29 +160,29 @@
             )
         else:
             logger.info("Successfully put dashboard to CloudWatch console")
         return response
 
     def _put_cloudwatch_alarm(self) -> None:
         """put CloudWatch metric alarms read from config"""
-        param_name = self._get_ssm_param_name("alarm")
+        param_name = self._get_ssm_param_name(CloudwatchConfigType.ALARM.value)
         data = json.loads(self._get_ssm_param(param_name))
         for item in data:
             item_out = copy.deepcopy(item)
             self._replace_all_config_variables(
                 item_out,
                 self.node_id,
                 self.cluster_name,
                 self.provider_config["region"],
             )
             self.cloudwatch_client.put_metric_alarm(**item_out)
         logger.info("Successfully put alarms to CloudWatch console")
 
     def _send_command_to_node(
-        self, document_name: str, parameters: List[str], node_id: str
+        self, document_name: str, parameters: Dict[str, List[str]], node_id: str
     ) -> Dict[str, Any]:
         """send SSM command to the given nodes"""
         logger.debug(
             "Sending SSM command to {} node(s). Document name: {}. "
             "Parameters: {}.".format(node_id, document_name, parameters)
         )
         response = self.ssm_client.send_command(
@@ -173,30 +193,32 @@
             MaxErrors="0",
         )
         return response
 
     def _ssm_command_waiter(
         self,
         document_name: str,
-        parameters: List[str],
+        parameters: Dict[str, List[str]],
         node_id: str,
         retry_failed: bool = True,
-    ) -> bool:
+    ) -> Dict[str, Any]:
         """wait for SSM command to complete on all cluster nodes"""
 
         # This waiter differs from the built-in SSM.Waiter by
         # optimistically waiting for the command invocation to
         # exist instead of failing immediately, and by resubmitting
         # any failed command until all retry attempts are exhausted
         # by default.
         response = self._send_command_to_node(document_name, parameters, node_id)
         command_id = response["Command"]["CommandId"]
 
         cloudwatch_config = self.provider_config["cloudwatch"]
-        agent_retryer_config = cloudwatch_config.get("agent").get("retryer", {})
+        agent_retryer_config = cloudwatch_config.get(
+            CloudwatchConfigType.AGENT.value
+        ).get("retryer", {})
         max_attempts = agent_retryer_config.get("max_attempts", 120)
         delay_seconds = agent_retryer_config.get("delay_seconds", 30)
         num_attempts = 0
         cmd_invocation_res = {}
         while True:
             num_attempts += 1
             logger.debug(
@@ -279,34 +301,40 @@
             string = string.replace("{cluster_name}", cluster_name)
         if region:
             string = string.replace("{region}", region)
         return string
 
     def _replace_all_config_variables(
         self,
-        collection: Union[dict, list],
+        collection: Union[Dict[str, Any], str],
         node_id: str,
         cluster_name: str,
         region: str,
-    ) -> Tuple[(Union[dict, list], int)]:
+    ) -> Union[str, Dict[str, Any]]:
         """
         Replace known config variable occurrences in the input collection.
-
         The input collection must be either a dict or list.
         Returns a tuple consisting of the output collection and the number of
         modified strings in the collection (which is not necessarily equal to
         the number of variables replaced).
         """
+
         for key in collection:
             if type(collection) is dict:
                 value = collection.get(key)
                 index_key = key
             elif type(collection) is list:
                 value = key
                 index_key = collection.index(key)
+            else:
+                raise ValueError(
+                    f"Can't replace CloudWatch config variables "
+                    f"in unsupported collection type: {type(collection)}."
+                    f"Please check your CloudWatch JSON config files."
+                )
             if type(value) is str:
                 collection[index_key] = self._replace_config_variables(
                     value, node_id, cluster_name, region
                 )
             elif type(value) is dict or type(value) is list:
                 collection[index_key] = self._replace_all_config_variables(
                     value, node_id, cluster_name, region
@@ -340,16 +368,16 @@
                     "Checking for Unified CloudWatch Agent installation".format(
                         config_type
                     )
                 )
                 return self._get_default_empty_config_file_hash()
             else:
                 logger.info(
-                    "Failed to fetch CloudWatch {} config from SSM "
-                    "parameter store.".format(config_type)
+                    "Failed to fetch Unified CloudWatch Agent config from SSM "
+                    "parameter store."
                 )
                 logger.error(e)
                 raise e
         return parameter_value
 
     def _get_default_empty_config_file_hash(self):
         default_cw_config = "{}"
@@ -364,52 +392,46 @@
         logger.info("Successfully fetch ssm parameter: {}".format(parameter_name))
         res = response.get("Parameter", {})
         cwa_parameter = res.get("Value", {})
         return cwa_parameter
 
     def _sha1_hash_json(self, value: str) -> str:
         """calculate the json string sha1 hash"""
-        hash = hashlib.new("sha1")
+        sha1_hash = hashlib.new("sha1")
         binary_value = value.encode("ascii")
-        hash.update(binary_value)
-        sha1_res = hash.hexdigest()
+        sha1_hash.update(binary_value)
+        sha1_res = sha1_hash.hexdigest()
         return sha1_res
 
     def _sha1_hash_file(self, config_type: str) -> str:
         """calculate the config file sha1 hash"""
-        if config_type == "agent":
-            config = self._replace_cwa_config_variables()
-        if config_type == "dashboard":
-            config = self._replace_dashboard_config_variables()
-        if config_type == "alarm":
-            config = self._load_config_file("alarm")
+        config = self.CLOUDWATCH_CONFIG_TYPE_TO_CONFIG_VARIABLE_REPLACE_FUNC.get(
+            config_type
+        )(config_type)
         value = json.dumps(config)
         sha1_res = self._sha1_hash_json(value)
         return sha1_res
 
     def _upload_config_to_ssm_and_set_hash_tag(self, config_type: str):
-        if config_type == "agent":
-            data = self._replace_cwa_config_variables()
-        if config_type == "dashboard":
-            data = self._replace_dashboard_config_variables()
-        if config_type == "alarm":
-            data = self._load_config_file("alarm")
+        data = self.CLOUDWATCH_CONFIG_TYPE_TO_CONFIG_VARIABLE_REPLACE_FUNC.get(
+            config_type
+        )(config_type)
         sha1_hash_value = self._sha1_hash_file(config_type)
         self._upload_config_to_ssm(data, config_type)
         self._update_cloudwatch_hash_tag_value(
             self.node_id, sha1_hash_value, config_type
         )
 
     def _add_cwa_installed_tag(self, node_id: str) -> None:
         self.ec2_client.create_tags(
             Resources=[node_id],
             Tags=[{"Key": CLOUDWATCH_AGENT_INSTALLED_TAG, "Value": "True"}],
         )
         logger.info(
-            "Successfully add Unified Cloudwatch Agent installed "
+            "Successfully add Unified CloudWatch Agent installed "
             "tag on {}".format(node_id)
         )
 
     def _update_cloudwatch_hash_tag_value(
         self, node_id: str, sha1_hash_value: str, config_type: str
     ):
         hash_key_value = "-".join([CLOUDWATCH_CONFIG_HASH_TAG_BASE, config_type])
@@ -440,69 +462,68 @@
             Tier="Intelligent-Tiering",
         )
 
     def _upload_config_to_ssm(self, param: Dict[str, Any], config_type: str):
         param_name = self._get_ssm_param_name(config_type)
         self._put_ssm_param(param, param_name)
 
-    def _replace_cwa_config_variables(self) -> Dict[str, Any]:
+    def _replace_cwa_config_vars(self, config_type: str) -> Dict[str, Any]:
         """
         replace {instance_id}, {region}, {cluster_name}
         variable occurrences in Unified Cloudwatch Agent config file
         """
-        cwa_config = self._load_config_file("agent")
+        cwa_config = self._load_config_file(config_type)
         self._replace_all_config_variables(
             cwa_config,
             self.node_id,
             self.cluster_name,
             self.provider_config["region"],
         )
         return cwa_config
 
-    def _replace_dashboard_config_variables(self) -> List[Dict[str, Any]]:
+    def _replace_dashboard_config_vars(self, config_type: str) -> List[str]:
         """
         replace known variable occurrences in CloudWatch Dashboard config file
         """
-        data = self._load_config_file("dashboard")
+        data = self._load_config_file(config_type)
         widgets = []
         for item in data:
             item_out = self._replace_all_config_variables(
                 item,
                 self.node_id,
                 self.cluster_name,
                 self.provider_config["region"],
             )
-            item_out = copy.deepcopy(item)
             widgets.append(item_out)
         return widgets
 
-    def _replace_alarm_config_variables(self) -> List[Dict[str, Any]]:
+    def _replace_alarm_config_vars(self, config_type: str) -> List[str]:
         """
         replace {instance_id}, {region}, {cluster_name}
         variable occurrences in cloudwatch alarm config file
         """
-        data = self._load_config_file("alarm")
+        data = self._load_config_file(config_type)
         param_data = []
         for item in data:
             item_out = copy.deepcopy(item)
             self._replace_all_config_variables(
                 item_out,
                 self.node_id,
                 self.cluster_name,
                 self.provider_config["region"],
             )
             param_data.append(item_out)
         return param_data
 
     def _restart_cloudwatch_agent(self) -> None:
-        """restart Unified Cloudwatch Agent"""
-        cwa_param_name = self._get_ssm_param_name("agent")
+        """restart Unified CloudWatch Agent"""
+        cwa_param_name = self._get_ssm_param_name(CloudwatchConfigType.AGENT.value)
         logger.info(
-            "Restarting Unified Cloudwatch Agent package on {} node(s).".format(
-                (self.node_id)
+            "Restarting Unified CloudWatch Agent package on node {}.".format(
+                self.node_id
             )
         )
         self._stop_cloudwatch_agent()
         self._start_cloudwatch_agent(cwa_param_name)
 
     def _stop_cloudwatch_agent(self) -> None:
         """stop Unified CloudWatch Agent"""
@@ -687,15 +708,17 @@
 
         Returns:
             default cloudwatch instance profile name if cloudwatch config file
                 exists.
             default ray instance profile name if cloudwatch config file
                 doesn't exist.
         """
-        cwa_cfg_exists = CloudwatchHelper.cloudwatch_config_exists(config, "agent")
+        cwa_cfg_exists = CloudwatchHelper.cloudwatch_config_exists(
+            config, CloudwatchConfigType.AGENT.value
+        )
         return (
             CLOUDWATCH_RAY_INSTANCE_PROFILE
             if cwa_cfg_exists
             else default_instance_profile_name
         )
 
     @staticmethod
@@ -708,15 +731,17 @@
             config: provider section of cluster config file.
             default_iam_role_name: default ray iam role name.
 
         Returns:
             default cloudwatch iam role name if cloudwatch config file exists.
             default ray iam role name if cloudwatch config file doesn't exist.
         """
-        cwa_cfg_exists = CloudwatchHelper.cloudwatch_config_exists(config, "agent")
+        cwa_cfg_exists = CloudwatchHelper.cloudwatch_config_exists(
+            config, CloudwatchConfigType.AGENT.value
+        )
         return CLOUDWATCH_RAY_IAM_ROLE if cwa_cfg_exists else default_iam_role_name
 
     @staticmethod
     def resolve_policy_arns(
         config: Dict[str, Any], iam: Any, default_policy_arns: List[str]
     ) -> List[str]:
         """Attach necessary AWS policies for CloudWatch related operations.
@@ -727,15 +752,17 @@
             default_policy_arns: List of default ray AWS policies.
 
         Returns:
             list of policy arns including additional policies for CloudWatch
                 related operations if cloudwatch agent config is specifed in
                 cluster config file.
         """
-        cwa_cfg_exists = CloudwatchHelper.cloudwatch_config_exists(config, "agent")
+        cwa_cfg_exists = CloudwatchHelper.cloudwatch_config_exists(
+            config, CloudwatchConfigType.AGENT.value
+        )
         if cwa_cfg_exists:
             cloudwatch_managed_policy = {
                 "Version": "2012-10-17",
                 "Statement": [
                     {
                         "Effect": "Allow",
                         "Action": [
```

### Comparing `skypilot-0.2.5/sky/skylet/providers/aws/config.py` & `skypilot-0.3.0/sky/skylet/providers/aws/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,26 +36,33 @@
 DEFAULT_SKYPILOT_INSTANCE_PROFILE = SKYPILOT + "-v1"
 DEFAULT_SKYPILOT_IAM_ROLE = SKYPILOT + "-v1"
 
 # V61.0 has CUDA 11.2
 DEFAULT_AMI_NAME = "AWS Deep Learning AMI (Ubuntu 18.04) V61.0"
 
 # Obtained from https://aws.amazon.com/marketplace/pp/B07Y43P7X5 on 6/10/2022.
+# TODO(alex) : write a unit test to make sure we update AMI version used in
+# ray/autoscaler/aws/example-full.yaml whenever we update this dict.
 # NOTE(skypilot): these are not used; skypilot instead uses the default AMIs in aws.py.
 DEFAULT_AMI = {
     "us-east-1": "ami-0dd6adfad4ad37eec",  # US East (N. Virginia)
     "us-east-2": "ami-0c77cd5ca05bf1281",  # US East (Ohio)
     "us-west-1": "ami-020ab1b368a5ed1db",  # US West (N. California)
     "us-west-2": "ami-0387d929287ab193e",  # US West (Oregon)
     "ca-central-1": "ami-07dbafdbd38f18d98",  # Canada (Central)
     "eu-central-1": "ami-0383bd0c1fc4c63ec",  # EU (Frankfurt)
     "eu-west-1": "ami-0a074b0a311a837ac",  # EU (Ireland)
     "eu-west-2": "ami-094ba2b4651f761ca",  # EU (London)
     "eu-west-3": "ami-031da10fbf225bf5f",  # EU (Paris)
     "sa-east-1": "ami-0be7c1f1dd96d7337",  # SA (Sao Paulo)
+    "ap-northeast-1": "ami-0d69b2fd9641af433",  # Asia Pacific (Tokyo)
+    "ap-northeast-2": "ami-0d6d00bd58046ff91",  # Asia Pacific (Seoul)
+    "ap-northeast-3": "ami-068feab7122f7558d",  # Asia Pacific (Osaka)
+    "ap-southeast-1": "ami-05006b266c1be4e8f",  # Asia Pacific (Singapore)
+    "ap-southeast-2": "ami-066aa744514f9f95c",  # Asia Pacific (Sydney)
 }
 
 # todo: cli_logger should handle this assert properly
 # this should probably also happens somewhere else
 assert StrictVersion(boto3.__version__) >= StrictVersion(
     "1.4.8"
 ), "Boto3 version >= 1.4.8 required, try `pip install -U boto3`"
@@ -424,15 +431,15 @@
     ec2 = _resource("ec2", config)
 
     # Writing the new ssh key to the filesystem fails if the ~/.ssh
     # directory doesn't already exist.
     os.makedirs(os.path.expanduser("~/.ssh"), exist_ok=True)
 
     # Try a few times to get or create a good key pair.
-    MAX_NUM_KEYS = 30
+    MAX_NUM_KEYS = 60
     for i in range(MAX_NUM_KEYS):
 
         key_name = config["provider"].get("key_pair", {}).get("key_name")
 
         key_name, key_path = key_pair(i, config["provider"]["region"], key_name)
         key = _get_key(key_name, config)
```

### Comparing `skypilot-0.2.5/sky/skylet/providers/aws/node_provider.py` & `skypilot-0.3.0/sky/skylet/providers/aws/node_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,14 +495,19 @@
                                 state=instance.state["Name"],
                                 info=state_reason["Message"],
                             ),
                         )
                 break
             except botocore.exceptions.ClientError as exc:
                 if attempt == max_tries:
+                    # SkyPilot: do not adopt the changes from upstream in
+                    # https://github.com/ray-project/ray/commit/c2abfdb2f7eee7f3e4320cb0d9e8e3bd639d5680#diff-eeb7bc1d8342583cf12c40536240dbcc67f089466a18a37bd60f187265a2dc94
+                    # which replaces the exception to NodeLaunchException. As we directly
+                    # handle the exception output in
+                    # cloud_vm_ray_backend._update_blocklist_on_aws_error
                     cli_logger.abort(
                         "Failed to launch instances. Max attempts exceeded.",
                         exc=exc,
                     )
                 else:
                     cli_logger.warning(
                         "create_instances: Attempt failed with {}, retrying.", exc
```

### Comparing `skypilot-0.2.5/sky/skylet/providers/aws/utils.py` & `skypilot-0.3.0/sky/skylet/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-0.3.0/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9443646071589322%*

 * *Differences: {"'parameters'": "{'msi': OrderedDict([('type', 'string'), ('metadata', "*

 * *                 "OrderedDict([('description', 'Managed service identity resource id.')]))]), "*

 * *                 "'nsg': OrderedDict([('type', 'string'), ('metadata', "*

 * *                 "OrderedDict([('description', 'Network security group resource id.')]))]), "*

 * *                 "'subnet': OrderedDict([('type', 'string'), ('metadata', "*

 * *                 "OrderedDict([('descriptions', 'Subnet resource id.')]))]), 'osDiskTier': "*

 * *       […]*

```diff
@@ -52,20 +52,43 @@
         },
         "imageVersion": {
             "metadata": {
                 "description": "The version of the VM image"
             },
             "type": "string"
         },
+        "msi": {
+            "metadata": {
+                "description": "Managed service identity resource id."
+            },
+            "type": "string"
+        },
+        "nsg": {
+            "metadata": {
+                "description": "Network security group resource id."
+            },
+            "type": "string"
+        },
         "osDiskSizeGB": {
             "metadata": {
                 "description": "OS disk size in GBs."
             },
             "type": "int"
         },
+        "osDiskTier": {
+            "allowedValues": [
+                "Premium_LRS",
+                "StandardSSD_LRS",
+                "Standard_LRS"
+            ],
+            "metadata": {
+                "description": "OS disk tier."
+            },
+            "type": "string"
+        },
         "priority": {
             "defaultValue": "Regular",
             "metadata": {
                 "description": "Specifies the priority for the virtual machine."
             },
             "type": "string"
         },
@@ -78,14 +101,20 @@
         },
         "publicKey": {
             "metadata": {
                 "description": "SSH Key for the Virtual Machine"
             },
             "type": "securestring"
         },
+        "subnet": {
+            "metadata": {
+                "descriptions": "Subnet resource id."
+            },
+            "type": "string"
+        },
         "vmCount": {
             "metadata": {
                 "description": "Number of VMs to deploy"
             },
             "type": "int"
         },
         "vmName": {
@@ -126,21 +155,21 @@
                         "name": "[variables('networkIpConfig')]",
                         "properties": {
                             "privateIPAllocationMethod": "Dynamic",
                             "publicIpAddress": {
                                 "id": "[resourceId('Microsoft.Network/publicIPAddresses', concat(variables('publicIPAddressName'), copyIndex()))]"
                             },
                             "subnet": {
-                                "id": "[variables('subnetRef')]"
+                                "id": "[parameters('subnet')]"
                             }
                         }
                     }
                 ],
                 "networkSecurityGroup": {
-                    "id": "[resourceId('Microsoft.Network/networkSecurityGroups','ray-nsg')]"
+                    "id": "[parameters('nsg')]"
                 }
             },
             "type": "Microsoft.Network/networkInterfaces"
         },
         {
             "apiVersion": "2020-06-01",
             "condition": "[not(parameters('provisionPublicIp'))]",
@@ -153,21 +182,21 @@
             "properties": {
                 "ipConfigurations": [
                     {
                         "name": "[variables('networkIpConfig')]",
                         "properties": {
                             "privateIPAllocationMethod": "Dynamic",
                             "subnet": {
-                                "id": "[variables('subnetRef')]"
+                                "id": "[parameters('subnet')]"
                             }
                         }
                     }
                 ],
                 "networkSecurityGroup": {
-                    "id": "[resourceId('Microsoft.Network/networkSecurityGroups','ray-nsg')]"
+                    "id": "[parameters('nsg')]"
                 }
             },
             "type": "Microsoft.Network/networkInterfaces"
         },
         {
             "apiVersion": "2019-02-01",
             "condition": "[parameters('provisionPublicIp')]",
@@ -195,15 +224,15 @@
             },
             "dependsOn": [
                 "[resourceId('Microsoft.Network/networkInterfaces/', concat(variables('networkInterfaceName'), copyIndex()))]"
             ],
             "identity": {
                 "type": "UserAssigned",
                 "userAssignedIdentities": {
-                    "[resourceId('Microsoft.ManagedIdentity/userAssignedIdentities', 'ray-msi-user-identity')]": {}
+                    "[parameters('msi')]": {}
                 }
             },
             "location": "[variables('location')]",
             "name": "[concat(parameters('vmName'), copyIndex())]",
             "properties": {
                 "billingProfile": "[parameters('billingProfile')]",
                 "hardwareProfile": {
@@ -240,27 +269,25 @@
                         "sku": "[parameters('imageSku')]",
                         "version": "[parameters('imageVersion')]"
                     },
                     "osDisk": {
                         "createOption": "fromImage",
                         "diskSizeGB": "[parameters('osDiskSizeGB')]",
                         "managedDisk": {
-                            "storageAccountType": "[variables('osDiskType')]"
+                            "storageAccountType": "[parameters('osDiskTier')]"
                         }
                     }
                 }
             },
             "tags": "[parameters('vmTags')]",
             "type": "Microsoft.Compute/virtualMachines"
         }
     ],
     "variables": {
         "location": "[resourceGroup().location]",
         "networkInterfaceName": "[if(parameters('provisionPublicIp'), variables('networkInterfaceNamePublic'), variables('networkInterfaceNamePrivate'))]",
-        "networkInterfaceNamePrivate": "[concat(parameters('vmName'),'-nic')]",
-        "networkInterfaceNamePublic": "[concat(parameters('vmName'),'-nic-public')]",
+        "networkInterfaceNamePrivate": "[concat(parameters('vmName'), '-nic')]",
+        "networkInterfaceNamePublic": "[concat(parameters('vmName'), '-nic-public')]",
         "networkIpConfig": "[guid(resourceGroup().id, parameters('vmName'))]",
-        "osDiskType": "Standard_LRS",
-        "publicIpAddressName": "[concat(parameters('vmName'), '-ip' )]",
-        "subnetRef": "[resourceId('Microsoft.Network/virtualNetworks/subnets', 'ray-vnet', 'ray-subnet')]"
+        "publicIpAddressName": "[concat(parameters('vmName'), '-ip')]"
     }
 }
```

### Comparing `skypilot-0.2.5/sky/skylet/providers/azure/config.py` & `skypilot-0.3.0/sky/skylet/providers/azure/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import json
 import logging
 import random
+from hashlib import sha256
 from pathlib import Path
 from typing import Any, Callable
 
 from azure.common.credentials import get_cli_profile
 from azure.identity import AzureCliCredential
 from azure.mgmt.resource import ResourceManagementClient
 from azure.mgmt.resource.resources.models import DeploymentMode
 
-RETRIES = 30
-MSI_NAME = "ray-msi-user-identity"
-NSG_NAME = "ray-nsg"
-SUBNET_NAME = "ray-subnet"
-VNET_NAME = "ray-vnet"
+UNIQUE_ID_LEN = 4
 
 logger = logging.getLogger(__name__)
 
 
 def get_azure_sdk_function(client: Any, function_name: str) -> Callable:
     """Retrieve a callable function from Azure SDK client object.
 
     Newer versions of the various client SDKs renamed function names to
     have a begin_ prefix. This function supports both the old and new
     versions of the SDK by first trying the old name and falling back to
     the prefixed new name.
     """
-    func = getattr(client, function_name, getattr(client, f"begin_{function_name}"))
+    func = getattr(
+        client, function_name, getattr(client, f"begin_{function_name}", None)
+    )
     if func is None:
         raise AttributeError(
             "'{obj}' object has no {func} or begin_{func} attribute".format(
                 obj={client.__name__}, func=function_name
             )
         )
     return func
@@ -44,15 +43,20 @@
 
 def _configure_resource_group(config):
     # TODO: look at availability sets
     # https://docs.microsoft.com/en-us/azure/virtual-machines/windows/tutorial-availability-sets
     subscription_id = config["provider"].get("subscription_id")
     if subscription_id is None:
         subscription_id = get_cli_profile().get_subscription_id()
-    resource_client = ResourceManagementClient(AzureCliCredential(), subscription_id)
+    # Increase the timeout to fix the Azure get-access-token (used by ray azure
+    # node_provider) timeout issue.
+    # Tracked in https://github.com/Azure/azure-cli/issues/20404#issuecomment-1249575110
+    resource_client = ResourceManagementClient(
+        AzureCliCredential(process_timeout=30), subscription_id
+    )
     config["provider"]["subscription_id"] = subscription_id
     logger.info("Using subscription id: %s", subscription_id)
 
     assert (
         "resource_group" in config["provider"]
     ), "Provider config must include resource_group field"
     resource_group = config["provider"]["resource_group"]
@@ -61,45 +65,75 @@
         "location" in config["provider"]
     ), "Provider config must include location field"
     params = {"location": config["provider"]["location"]}
 
     if "tags" in config["provider"]:
         params["tags"] = config["provider"]["tags"]
 
-    logger.info("Creating/Updating Resource Group: %s", resource_group)
-    resource_client.resource_groups.create_or_update(
-        resource_group_name=resource_group, parameters=params
+    logger.info("Creating/Updating resource group: %s", resource_group)
+    rg_create_or_update = get_azure_sdk_function(
+        client=resource_client.resource_groups, function_name="create_or_update"
     )
+    rg_create_or_update(resource_group_name=resource_group, parameters=params)
 
     # load the template file
     current_path = Path(__file__).parent
     template_path = current_path.joinpath("azure-config-template.json")
     with open(template_path, "r") as template_fp:
         template = json.load(template_fp)
 
-    # choose a random subnet, skipping most common value of 0
-    random.seed(resource_group)
-    subnet_mask = "10.{}.0.0/16".format(random.randint(1, 254))
+    logger.info("Using cluster name: %s", config["cluster_name"])
+
+    # set unique id for resources in this cluster
+    unique_id = config["provider"].get("unique_id")
+    if unique_id is None:
+        hasher = sha256()
+        hasher.update(config["provider"]["resource_group"].encode("utf-8"))
+        unique_id = hasher.hexdigest()[:UNIQUE_ID_LEN]
+    else:
+        unique_id = str(unique_id)
+    config["provider"]["unique_id"] = unique_id
+    logger.info("Using unique id: %s", unique_id)
+    cluster_id = "{}-{}".format(config["cluster_name"], unique_id)
+
+    subnet_mask = config["provider"].get("subnet_mask")
+    if subnet_mask is None:
+        # choose a random subnet, skipping most common value of 0
+        random.seed(unique_id)
+        subnet_mask = "10.{}.0.0/16".format(random.randint(1, 254))
+    logger.info("Using subnet mask: %s", subnet_mask)
 
     parameters = {
         "properties": {
             "mode": DeploymentMode.incremental,
             "template": template,
-            "parameters": {"subnet": {"value": subnet_mask}},
+            "parameters": {
+                "subnet": {"value": subnet_mask},
+                "clusterId": {"value": cluster_id},
+            },
         }
     }
 
     create_or_update = get_azure_sdk_function(
         client=resource_client.deployments, function_name="create_or_update"
     )
-    create_or_update(
-        resource_group_name=resource_group,
-        deployment_name="ray-config",
-        parameters=parameters,
-    ).wait()
+    outputs = (
+        create_or_update(
+            resource_group_name=resource_group,
+            deployment_name="ray-config",
+            parameters=parameters,
+        )
+        .result()
+        .properties.outputs
+    )
+
+    # append output resource ids to be used with vm creation
+    config["provider"]["msi"] = outputs["msi"]["value"]
+    config["provider"]["nsg"] = outputs["nsg"]["value"]
+    config["provider"]["subnet"] = outputs["subnet"]["value"]
 
     return config
 
 
 def _configure_key_pair(config):
     ssh_user = config["auth"]["ssh_user"]
     public_key = None
```

### Comparing `skypilot-0.2.5/sky/skylet/providers/azure/node_provider.py` & `skypilot-0.3.0/sky/skylet/providers/azure/node_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     TAG_RAY_LAUNCH_CONFIG,
     TAG_RAY_NODE_KIND,
     TAG_RAY_NODE_NAME,
     TAG_RAY_USER_NODE_TYPE,
 )
 
 VM_NAME_MAX_LEN = 64
-VM_NAME_UUID_LEN = 8
+UNIQUE_ID_LEN = 4
 
 logger = logging.getLogger(__name__)
 azure_logger = logging.getLogger("azure.core.pipeline.policies.http_logging_policy")
 azure_logger.setLevel(logging.WARNING)
 
 
 def synchronized(f):
@@ -60,32 +60,40 @@
         # TODO(suquark): This is a temporary patch for resource group.
         # By default, Ray autoscaler assumes the resource group is still here even
         # after the whole cluster is destroyed. However, now we deletes the resource
         # group after tearing down the cluster. To comfort the autoscaler, we need
         # to create/update it here, so the resource group always exists.
         from sky.skylet.providers.azure.config import _configure_resource_group
 
-        _configure_resource_group({"provider": provider_config})
+        _configure_resource_group(
+            {"cluster_name": cluster_name, "provider": provider_config}
+        )
         subscription_id = provider_config["subscription_id"]
         self.cache_stopped_nodes = provider_config.get("cache_stopped_nodes", True)
         # Sky only supports Azure CLI credential for now.
-        credential = AzureCliCredential()
+        # Increase the timeout to fix the Azure get-access-token (used by ray azure
+        # node_provider) timeout issue.
+        # Tracked in https://github.com/Azure/azure-cli/issues/20404#issuecomment-1249575110
+        credential = AzureCliCredential(process_timeout=30)
         self.compute_client = ComputeManagementClient(credential, subscription_id)
         self.network_client = NetworkManagementClient(credential, subscription_id)
         self.resource_client = ResourceManagementClient(credential, subscription_id)
 
         self.lock = RLock()
 
         # cache node objects
         self.cached_nodes = {}
 
     @synchronized
     def _get_filtered_nodes(self, tag_filters):
+        # add cluster name filter to only get nodes from this cluster
+        cluster_tag_filters = {**tag_filters, TAG_RAY_CLUSTER_NAME: self.cluster_name}
+
         def match_tags(vm):
-            for k, v in tag_filters.items():
+            for k, v in cluster_tag_filters.items():
                 if vm.tags.get(k) != v:
                     return False
             return True
 
         vms = self.compute_client.virtual_machines.list(
             resource_group_name=self.provider_config["resource_group"]
         )
@@ -142,15 +150,18 @@
 
         This list must not include terminated nodes. For performance reasons,
         providers are allowed to cache the result of a call to nodes() to
         serve single-node queries (e.g. is_running(node_id)). This means that
         nodes() must be called again to refresh results.
 
         Examples:
-            >>> provider.non_terminated_nodes({TAG_RAY_NODE_KIND: "worker"})
+            >>> from ray.autoscaler.tags import TAG_RAY_NODE_KIND
+            >>> provider = ... # doctest: +SKIP
+            >>> provider.non_terminated_nodes( # doctest: +SKIP
+            ...     {TAG_RAY_NODE_KIND: "worker"})
             ["node-1", "node-2"]
         """
         nodes = self._get_filtered_nodes(tag_filters=tag_filters)
         return [k for k, v in nodes.items() if not v["status"].startswith("deallocat")]
 
     def is_running(self, node_id):
         """Return whether the specified node is running."""
@@ -260,24 +271,29 @@
             template = json.load(template_fp)
 
         # get the tags
         config_tags = node_config.get("tags", {}).copy()
         config_tags.update(tags)
         config_tags[TAG_RAY_CLUSTER_NAME] = self.cluster_name
 
-        name_tag = config_tags.get(TAG_RAY_NODE_NAME, "node")
-        unique_id = uuid4().hex[:VM_NAME_UUID_LEN]
-        vm_name = "{name}-{id}".format(name=name_tag, id=unique_id)
+        vm_name = "{node}-{unique_id}-{vm_id}".format(
+            node=config_tags.get(TAG_RAY_NODE_NAME, "node"),
+            unique_id=self.provider_config["unique_id"],
+            vm_id=uuid4().hex[:UNIQUE_ID_LEN],
+        )[:VM_NAME_MAX_LEN]
         use_internal_ips = self.provider_config.get("use_internal_ips", False)
 
         template_params = node_config["azure_arm_parameters"].copy()
         template_params["vmName"] = vm_name
         template_params["provisionPublicIp"] = not use_internal_ips
         template_params["vmTags"] = config_tags
         template_params["vmCount"] = count
+        template_params["msi"] = self.provider_config["msi"]
+        template_params["nsg"] = self.provider_config["nsg"]
+        template_params["subnet"] = self.provider_config["subnet"]
 
         parameters = {
             "properties": {
                 "mode": DeploymentMode.incremental,
                 "template": template,
                 "parameters": {
                     key: {"value": value} for key, value in template_params.items()
@@ -287,15 +303,15 @@
 
         # TODO: we could get the private/public ips back directly
         create_or_update = get_azure_sdk_function(
             client=self.resource_client.deployments, function_name="create_or_update"
         )
         create_or_update(
             resource_group_name=resource_group,
-            deployment_name="ray-vm-{}".format(name_tag),
+            deployment_name=vm_name,
             parameters=parameters,
         ).wait()
 
     @synchronized
     def set_node_tags(self, node_id, tags):
         """Sets the tag values (string dict) for the specified node."""
         node_tags = self._get_cached_node(node_id)["tags"]
```

### Comparing `skypilot-0.2.5/sky/skylet/providers/gcp/config.py` & `skypilot-0.3.0/sky/skylet/providers/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/skylet/providers/gcp/constants.py` & `skypilot-0.3.0/sky/skylet/providers/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/skylet/providers/gcp/node.py` & `skypilot-0.3.0/sky/skylet/providers/gcp/node.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/skylet/providers/gcp/node_provider.py` & `skypilot-0.3.0/sky/skylet/providers/gcp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/skylet/providers/lambda_cloud/lambda_utils.py` & `skypilot-0.3.0/sky/skylet/providers/lambda_cloud/lambda_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Lambda Cloud helper functions."""
-import os
 import json
+import os
 import requests
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Tuple
 
 CREDENTIALS_PATH = '~/.lambda_cloud/lambda_keys'
 API_ENDPOINT = 'https://cloud.lambdalabs.com/api/v1'
 
 
 class LambdaCloudError(Exception):
     pass
@@ -74,16 +74,16 @@
     if status_code == 200:
         return
     if status_code == 429:
         # https://docs.lambdalabs.com/cloud/rate-limiting/
         raise LambdaCloudError('Your API requests are being rate limited.')
     try:
         resp_json = response.json()
-        code = resp_json['error']['code']
-        message = resp_json['error']['message']
+        code = resp_json.get('error', {}).get('code')
+        message = resp_json.get('error', {}).get('message')
     except (KeyError, json.decoder.JSONDecodeError):
         raise LambdaCloudError(f'Unexpected error. Status code: {status_code}')
     raise LambdaCloudError(f'{code}: {message}')
 
 
 class LambdaCloudClient:
     """Wrapper functions for Lambda Cloud API."""
@@ -93,25 +93,23 @@
         assert os.path.exists(self.credentials), 'Credentials not found'
         with open(self.credentials, 'r') as f:
             lines = [line.strip() for line in f.readlines() if ' = ' in line]
             self._credentials = {
                 line.split(' = ')[0]: line.split(' = ')[1] for line in lines
             }
         self.api_key = self._credentials['api_key']
-        self.ssh_key_name = self._credentials.get('ssh_key_name', None)
         self.headers = {'Authorization': f'Bearer {self.api_key}'}
 
     def create_instances(self,
                          instance_type: str = 'gpu_1x_a100_sxm4',
                          region: str = 'us-east-1',
                          quantity: int = 1,
-                         name: str = '') -> Dict[str, Any]:
+                         name: str = '',
+                         ssh_key_name: str = '') -> List[str]:
         """Launch new instances."""
-        assert self.ssh_key_name is not None
-
         # Optimization:
         # Most API requests are rate limited at ~1 request every second but
         # launch requests are rate limited at ~1 request every 10 seconds.
         # So don't use launch requests to check availability.
         # See https://docs.lambdalabs.com/cloud/rate-limiting/ for more.
         available_regions = self.list_catalog()[instance_type]\
                 ['regions_with_capacity_available']
@@ -127,15 +125,15 @@
                                     'Regions with capacity available: '
                                     f'{aval_reg}'))
 
         # Try to launch instance
         data = json.dumps({
             'region_name': region,
             'instance_type_name': instance_type,
-            'ssh_key_names': [self.ssh_key_name],
+            'ssh_key_names': [ssh_key_name],
             'quantity': quantity,
             'name': name
         })
         response = requests.post(f'{API_ENDPOINT}/instance-operations/launch',
                                  data=data,
                                  headers=self.headers)
         raise_lambda_error(response)
@@ -151,32 +149,64 @@
         response = requests.post(
             f'{API_ENDPOINT}/instance-operations/terminate',
             data=data,
             headers=self.headers)
         raise_lambda_error(response)
         return response.json().get('data', []).get('terminated_instances', [])
 
-    def list_instances(self) -> Dict[str, Any]:
+    def list_instances(self) -> List[Dict[str, Any]]:
         """List existing instances."""
         response = requests.get(f'{API_ENDPOINT}/instances',
                                 headers=self.headers)
         raise_lambda_error(response)
         return response.json().get('data', [])
 
-    def set_ssh_key(self, name: str, pub_key: str) -> None:
-        """Set ssh key."""
+    def list_ssh_keys(self) -> List[Dict[str, str]]:
+        """List ssh keys."""
+        response = requests.get(f'{API_ENDPOINT}/ssh-keys',
+                                headers=self.headers)
+        raise_lambda_error(response)
+        return response.json().get('data', [])
+
+    def get_unique_ssh_key_name(self, prefix: str,
+                                pub_key: str) -> Tuple[str, bool]:
+        """Returns a ssh key name with the given prefix.
+
+        If no names have given prefix, return prefix. If pub_key exists and
+        has name with given prefix, return that name. Otherwise create a
+        UNIQUE name with given prefix.
+
+        The second return value is True iff the returned name already exists.
+        """
+        candidate_keys = [
+            k for k in self.list_ssh_keys()
+            if k.get('name', '').startswith(prefix)
+        ]
+
+        # Prefix not found
+        if not candidate_keys:
+            return prefix, False
+
+        suffix_digits = [0]
+        for key_info in candidate_keys:
+            name = key_info.get('name', '')
+            if key_info.get('public_key', '') == pub_key:
+                return name, True
+            if (len(name) > len(prefix) + 1 and name[len(prefix)] == '-' and
+                    name[len(prefix) + 1:].isdigit()):
+                suffix_digits.append(int(name[len(prefix) + 1:]))
+        return f'{prefix}-{max(suffix_digits) + 1}', False
+
+    def register_ssh_key(self, name: str, pub_key: str) -> None:
+        """Register ssh key with Lambda."""
         data = json.dumps({'name': name, 'public_key': pub_key})
         response = requests.post(f'{API_ENDPOINT}/ssh-keys',
                                  data=data,
                                  headers=self.headers)
         raise_lambda_error(response)
-        self.ssh_key_name = name
-        with open(self.credentials, 'w') as f:
-            f.write(f'api_key = {self.api_key}\n')
-            f.write(f'ssh_key_name = {self.ssh_key_name}\n')
 
     def list_catalog(self) -> Dict[str, Any]:
         """List offered instances and their availability."""
         response = requests.get(f'{API_ENDPOINT}/instance-types',
                                 headers=self.headers)
         raise_lambda_error(response)
         return response.json().get('data', [])
```

### Comparing `skypilot-0.2.5/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-0.3.0/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,18 +16,21 @@
     NODE_KIND_HEAD,
 )
 from sky.skylet.providers.lambda_cloud import lambda_utils
 from sky import authentication as auth
 from sky.utils import command_runner
 from sky.utils import subprocess_utils
 from sky.utils import ux_utils
+from sky.utils import common_utils
 
 _TAG_PATH_PREFIX = '~/.sky/generated/lambda_cloud/metadata'
+_REMOTE_SSH_KEY_NAME = '~/.lambda_cloud/ssh_key_name'
 _REMOTE_RAY_SSH_KEY = '~/ray_bootstrap_key.pem'
-_GET_INTERNAL_IP_CMD = 'ip -4 -br addr show | grep -Eo "10\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)"'
+_REMOTE_RAY_YAML = '~/ray_bootstrap_config.yaml'
+_GET_INTERNAL_IP_CMD = 'ip -4 -br addr show | grep UP | grep -Eo "(10\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)|172\.(1[6-9]|2[0-9]|3[0-1]))\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)"'
 
 logger = logging.getLogger(__name__)
 
 
 def synchronized(f):
 
     def wrapper(self, *args, **kwargs):
@@ -47,22 +50,55 @@
     """
 
     def __init__(self, provider_config: Dict[str, Any],
                  cluster_name: str) -> None:
         NodeProvider.__init__(self, provider_config, cluster_name)
         self.lock = RLock()
         self.lambda_client = lambda_utils.LambdaCloudClient()
-        self.cached_nodes = {}
+        self.cached_nodes: Dict[str, Dict[str, Any]] = {}
         self.metadata = lambda_utils.Metadata(_TAG_PATH_PREFIX, cluster_name)
         self.ssh_key_path = os.path.expanduser(auth.PRIVATE_SSH_KEY_PATH)
-        remote_ssh_key = os.path.expanduser(_REMOTE_RAY_SSH_KEY)
-        if os.path.exists(remote_ssh_key):
-            self.ssh_key_path = remote_ssh_key
 
-    def _guess_and_add_missing_tags(self, vms: Dict[str, Any]) -> None:
+        def _get_ssh_key_name(prefix: str) -> str:
+            public_key_path = os.path.expanduser(auth.PUBLIC_SSH_KEY_PATH)
+            with open(public_key_path, 'r') as f:
+                public_key = f.read()
+            name, exists = self.lambda_client.get_unique_ssh_key_name(
+                prefix, public_key)
+            if not exists:
+                raise lambda_utils.LambdaCloudError('SSH key not found')
+            return name
+
+        ray_yaml_path = os.path.expanduser(_REMOTE_RAY_YAML)
+        self.on_head = (os.path.exists(ray_yaml_path) and
+                        common_utils.read_yaml(ray_yaml_path)['cluster_name']
+                        == cluster_name)
+
+        if self.on_head:
+            self.ssh_key_path = os.path.expanduser(_REMOTE_RAY_SSH_KEY)
+            ssh_key_name_path = os.path.expanduser(_REMOTE_SSH_KEY_NAME)
+            if os.path.exists(ssh_key_name_path):
+                with open(ssh_key_name_path, 'r') as f:
+                    self.ssh_key_name = f.read()
+            else:
+                # At this point, `~/.ssh/sky-key.pub` contains the public
+                # key used to launch this cluster. Use it to determine
+                # ssh key name and store the name in _REMOTE_SSH_KEY_NAME.
+                # Note: this case only runs during cluster launch, so it is
+                # not possible for ~/.ssh/sky-key.pub to already be regenerated
+                # by the user.
+                self.ssh_key_name = _get_ssh_key_name('')
+                with open(ssh_key_name_path, 'w') as f:
+                    f.write(self.ssh_key_name)
+        else:
+            # On local
+            self.ssh_key_name = _get_ssh_key_name(
+                f'sky-key-{common_utils.get_user_hash()}')
+
+    def _guess_and_add_missing_tags(self, vms: List[Dict[str, Any]]) -> None:
         """Adds missing vms to local tag file and guesses their tags."""
         for node in vms:
             if self.metadata.get(node['id']) is not None:
                 pass
             elif node['name'] == f'{self.cluster_name}-head':
                 self.metadata.set(
                     node['id'], {
@@ -82,15 +118,15 @@
                             TAG_RAY_NODE_STATUS: STATUS_UP_TO_DATE,
                             TAG_RAY_NODE_KIND: NODE_KIND_WORKER,
                             TAG_RAY_USER_NODE_TYPE: 'ray_worker_default',
                             TAG_RAY_NODE_NAME: f'ray-{self.cluster_name}-worker',
                         }
                     })
 
-    def _list_instances_in_cluster(self) -> Dict[str, Any]:
+    def _list_instances_in_cluster(self) -> List[Dict[str, Any]]:
         """List running instances in cluster."""
         vms = self.lambda_client.list_instances()
         possible_names = [
             f'{self.cluster_name}-head', f'{self.cluster_name}-worker'
         ]
         return [node for node in vms if node.get('name') in possible_names]
 
@@ -99,37 +135,31 @@
                                                     str]) -> Dict[str, Any]:
 
         def _extract_metadata(vm: Dict[str, Any]) -> Dict[str, Any]:
             metadata = {'id': vm['id'], 'status': vm['status'], 'tags': {}}
             instance_info = self.metadata.get(vm['id'])
             if instance_info is not None:
                 metadata['tags'] = instance_info['tags']
-            with ux_utils.print_exception_no_traceback():
-                if 'ip' not in vm:
-                    raise lambda_utils.LambdaCloudError(
-                        'A node ip address was not found. Either '
-                        '(1) Lambda Cloud has internally errored, or '
-                        '(2) the cluster is still booting. '
-                        'You can manually terminate the cluster on the '
-                        'Lambda Cloud console or (in case 2) wait for '
-                        'booting to finish (~2 minutes).')
-            metadata['external_ip'] = vm['ip']
+            metadata['external_ip'] = vm.get('ip')
             return metadata
 
         def _match_tags(vm: Dict[str, Any]):
             vm_info = self.metadata.get(vm['id'])
             tags = {} if vm_info is None else vm_info['tags']
             for k, v in tag_filters.items():
                 if tags.get(k) != v:
                     return False
             return True
 
         def _get_internal_ip(node: Dict[str, Any]):
             # TODO(ewzeng): cache internal ips in metadata file to reduce
             # ssh overhead.
+            if node['external_ip'] is None:
+                node['internal_ip'] = None
+                return
             runner = command_runner.SSHCommandRunner(node['external_ip'],
                                                      'ubuntu',
                                                      self.ssh_key_path)
             rc, stdout, stderr = runner.run(_GET_INTERNAL_IP_CMD,
                                             require_outputs=True,
                                             stream_logs=False)
             subprocess_utils.handle_returncode(
@@ -169,48 +199,89 @@
 
     def is_terminated(self, node_id: str) -> bool:
         """Return whether the specified node is terminated."""
         return self._get_cached_node(node_id=node_id) is None
 
     def node_tags(self, node_id: str) -> Dict[str, str]:
         """Returns the tags of the given node (string dict)."""
-        return self._get_cached_node(node_id=node_id)['tags']
+        node = self._get_cached_node(node_id=node_id)
+        if node is None:
+            return {}
+        return node['tags']
 
-    def external_ip(self, node_id: str) -> str:
+    def external_ip(self, node_id: str) -> Optional[str]:
         """Returns the external ip of the given node."""
-        return self._get_cached_node(node_id=node_id)['external_ip']
+        node = self._get_cached_node(node_id=node_id)
+        if node is None:
+            return None
+        ip = node.get('external_ip')
+        with ux_utils.print_exception_no_traceback():
+            if ip is None:
+                raise lambda_utils.LambdaCloudError(
+                    'A node ip address was not found. Either '
+                    '(1) Lambda Cloud has internally errored, or '
+                    '(2) the cluster is still booting. '
+                    'You can manually terminate the cluster on the '
+                    'Lambda Cloud console or (in case 2) wait for '
+                    'booting to finish (~2 minutes).')
+        return ip
 
-    def internal_ip(self, node_id: str) -> str:
+    def internal_ip(self, node_id: str) -> Optional[str]:
         """Returns the internal ip (Ray ip) of the given node."""
-        return self._get_cached_node(node_id=node_id)['internal_ip']
+        node = self._get_cached_node(node_id=node_id)
+        if node is None:
+            return None
+        ip = node.get('internal_ip')
+        with ux_utils.print_exception_no_traceback():
+            if ip is None:
+                raise lambda_utils.LambdaCloudError(
+                    'A node ip address was not found. Either '
+                    '(1) Lambda Cloud has internally errored, or '
+                    '(2) the cluster is still booting. '
+                    'You can manually terminate the cluster on the '
+                    'Lambda Cloud console or (in case 2) wait for '
+                    'booting to finish (~2 minutes).')
+        return ip
 
     def create_node(self, node_config: Dict[str, Any], tags: Dict[str, str],
                     count: int) -> None:
         """Creates a number of nodes within the namespace."""
         # Get tags
         config_tags = node_config.get('tags', {}).copy()
         config_tags.update(tags)
         config_tags[TAG_RAY_CLUSTER_NAME] = self.cluster_name
 
         # Create nodes
         instance_type = node_config['InstanceType']
         region = self.provider_config['region']
+
         if config_tags[TAG_RAY_NODE_KIND] == NODE_KIND_HEAD:
             name = f'{self.cluster_name}-head'
+            # Occasionally, the head node will continue running for a short
+            # period after termination. This can lead to the following bug:
+            #   1. Head node autodowns but continues running.
+            #   2. The next autodown event is triggered, which executes ray up.
+            #   3. Head node stops running.
+            # In this case, a new head node is created after the cluster has
+            # terminated. We avoid this with the following check:
+            if self.on_head:
+                raise lambda_utils.LambdaCloudError('Head already exists.')
         else:
             name = f'{self.cluster_name}-worker'
+
         # Lambda launch api only supports launching one node at a time,
         # so we do a loop. Remove loop when launch api allows quantity > 1
         booting_list = []
         for _ in range(count):
             vm_id = self.lambda_client.create_instances(
                 instance_type=instance_type,
                 region=region,
                 quantity=1,
-                name=name)[0]
+                name=name,
+                ssh_key_name=self.ssh_key_name)[0]
             self.metadata.set(vm_id, {'tags': config_tags})
             booting_list.append(vm_id)
             time.sleep(10)  # Avoid api rate limits
 
         # Wait for nodes to finish booting
         while True:
             vms = self._list_instances_in_cluster()
@@ -222,14 +293,15 @@
                 return
             time.sleep(10)
 
     @synchronized
     def set_node_tags(self, node_id: str, tags: Dict[str, str]) -> None:
         """Sets the tag values (string dict) for the specified node."""
         node = self._get_node(node_id)
+        assert node is not None, node_id
         node['tags'].update(tags)
         self.metadata.set(node_id, {'tags': node['tags']})
 
     def terminate_node(self, node_id: str) -> None:
         """Terminates the specified node."""
         self.lambda_client.remove_instances(node_id)
         self.metadata.set(node_id, None)
```

### Comparing `skypilot-0.2.5/sky/skylet/ray_patches/__init__.py` & `skypilot-0.3.0/sky/skylet/ray_patches/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 To get original versions, go to the Ray branch with version:
 
   sky.constants.SKY_REMOTE_RAY_VERSION
 
 Example workflow:
 
-  >> wget https://raw.githubusercontent.com/ray-project/ray/releases/2.0.1/python/ray/autoscaler/_private/command_runner.py
+  >> wget https://raw.githubusercontent.com/ray-project/ray/releases/2.4.0/python/ray/autoscaler/_private/command_runner.py
   >> cp command_runner.py command_runner.py.1
 
   >> # Make some edits to command_runner.py.1...
 
   >> diff command_runner.py command_runner.py.1 >command_runner.py.patch
 
   >> # Inspect command_runner.py.patch.
@@ -65,35 +65,19 @@
 
     from ray._private import worker
     _run_patch(worker.__file__, _to_absolute('worker.py.patch'))
 
     from ray.dashboard.modules.job import cli
     _run_patch(cli.__file__, _to_absolute('cli.py.patch'))
 
-    from ray.dashboard.modules.job import job_manager
-    _run_patch(job_manager.__file__, _to_absolute('job_manager.py.patch'))
-
     from ray.autoscaler._private import autoscaler
     _run_patch(autoscaler.__file__, _to_absolute('autoscaler.py.patch'))
 
     from ray.autoscaler._private import command_runner
     _run_patch(command_runner.__file__, _to_absolute('command_runner.py.patch'))
 
     from ray.autoscaler._private import resource_demand_scheduler
     _run_patch(resource_demand_scheduler.__file__,
                _to_absolute('resource_demand_scheduler.py.patch'))
 
     from ray.autoscaler._private import updater
     _run_patch(updater.__file__, _to_absolute('updater.py.patch'))
-
-    # Fix the Azure get-access-token (used by ray azure node_provider) timeout issue,
-    # by increasing the timeout.
-    # Tracked in https://github.com/Azure/azure-cli/issues/20404#issuecomment-1249575110
-    # Only patch it if azure cli is installed.
-    try:
-        import azure
-        from azure.identity._credentials import azure_cli
-        version = pkg_resources.get_distribution('azure-cli').version
-        _run_patch(azure_cli.__file__, _to_absolute('azure_cli.py.patch'),
-                   version)
-    except ImportError:
-        pass
```

### Comparing `skypilot-0.2.5/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-0.3.0/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 0a1,5
-> # From https://github.com/ray-project/ray/blob/ray-2.0.1/python/ray/autoscaler/_private/resource_demand_scheduler.py
+> # From https://github.com/ray-project/ray/blob/ray-2.4.0/python/ray/autoscaler/_private/resource_demand_scheduler.py
 > # Sky patch changes:
 > #  - no new nodes are allowed to be launched launched when the upscaling_speed is 0
 > #  - comment out "assert not unfulfilled": this seems a buggy assert
 > 
-509c514,517
+450c455,458
 <             if upper_bound > 0:
 ---
 >             # NOTE(sky): do not autoscale when upsclaing speed is 0.
 >             if self.upscaling_speed == 0:
 >                 upper_bound = 0
 >             if upper_bound >= 0:
-646c654
+594c602
 <             assert not unfulfilled
 ---
 >             # assert not unfulfilled  # NOTE(sky): buggy assert.
```

### Comparing `skypilot-0.2.5/sky/skylet/skylet.py` & `skypilot-0.3.0/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/skylet/subprocess_daemon.py` & `skypilot-0.3.0/sky/skylet/subprocess_daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 import argparse
 import requests
 import sys
 import time
 
 import psutil
+
+from sky.skylet import job_lib
 from ray.dashboard.modules.job import common as job_common
 from ray.dashboard.modules.job import sdk as job_sdk
 
 if __name__ == '__main__':
 
     parser = argparse.ArgumentParser()
     parser.add_argument('--parent-pid', type=int, required=True)
@@ -38,15 +40,16 @@
     # If Local Ray job id is passed in, wait until the job
     # is done/cancelled/failed.
     if local_ray_job_id is None:
         wait_for_process = True
     else:
         try:
             # Polls the Job submission client to check job status.
-            client = job_sdk.JobSubmissionClient('http://127.0.0.1:8265')
+            port = job_lib.get_job_submission_port()
+            client = job_sdk.JobSubmissionClient(f'http://127.0.0.1:{port}')
             while True:
                 status_info = client.get_job_status(local_ray_job_id)
                 status = status_info.status
                 if status in {
                         job_common.JobStatus.SUCCEEDED,
                         job_common.JobStatus.STOPPED,
                         job_common.JobStatus.FAILED
```

### Comparing `skypilot-0.2.5/sky/skypilot_config.py` & `skypilot-0.3.0/sky/skypilot_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 to check if the config is successfully loaded.
 
 To read a nested-key config:
 
   >> skypilot_config.get_nested(('auth', 'some_auth_config'), default_value)
 
-To pop a nested-key config:
+To set a value in the nested-key config:
 
-  >> config_dict = skypilot_config.pop_nested(('auth', 'some_key'))
+  >> config_dict = skypilot_config.set_nested(('auth', 'some_key'), value)
 
 This operation returns a deep-copy dict, and is safe in that any key not found
 will not raise an error.
 
 Example usage:
 
 Consider the following config contents:
@@ -39,15 +39,15 @@
     skypilot_config.loaded()  # ==> False
     skypilot_config.get_nested(('a', 'nested'), None)    # ==> None
     skypilot_config.get_nested(('a', 'nonexist'), None)  # ==> None
     skypilot_config.get_nested(('a',), None)             # ==> None
 """
 import copy
 import os
-from typing import Any, Dict, Sequence
+from typing import Any, Dict, Iterable
 
 import yaml
 
 from sky import sky_logging
 from sky import clouds
 from sky.utils import common_utils
 
@@ -70,15 +70,15 @@
 
 logger = sky_logging.init_logger(__name__)
 
 # The loaded config.
 _dict = None
 
 
-def get_nested(keys: Sequence[str], default_value: Any) -> Any:
+def get_nested(keys: Iterable[str], default_value: Any) -> Any:
     """Gets a nested key.
 
     If any key is not found, or any intermediate key does not point to a dict
     value, returns 'default_value'.
     """
     global _dict
     if _dict is None:
@@ -89,48 +89,48 @@
             curr = curr[key]
         else:
             return default_value
     logger.debug(f'User config: {".".join(keys)} -> {curr}')
     return curr
 
 
-def pop_nested(keys: Sequence[str]) -> Dict[str, Any]:
-    """Returns a deep-copied config with the nested key popped.
+def set_nested(keys: Iterable[str], value: Any) -> Dict[str, Any]:
+    """Returns a deep-copied config with the nested key set to value.
 
     Like get_nested(), if any key is not found, this will not raise an error.
     """
     _check_loaded_or_die()
     global _dict
     assert _dict is not None
     curr = copy.deepcopy(_dict)
     to_return = curr
     prev = None
     for i, key in enumerate(keys):
-        if key in curr:
-            prev = curr
-            curr = curr[key]
-            if i == len(keys) - 1:
-                prev.pop(key)
-                logger.debug(f'Popped {keys}. Returning conf: {to_return}')
-        else:
-            # If any key not found, simply return.
-            return to_return
+        if key not in curr:
+            curr[key] = {}
+        prev = curr
+        curr = curr[key]
+        if i == len(keys) - 1:
+            prev_value = prev[key]
+            prev[key] = value
+            logger.debug(f'Set the value of {keys} to {value} (previous: '
+                         f'{prev_value}). Returning conf: {to_return}')
     return to_return
 
 
 def _syntax_check_for_ssh_proxy_command(cloud: str) -> None:
     ssh_proxy_command_config = get_nested((cloud.lower(), 'ssh_proxy_command'),
                                           None)
     if ssh_proxy_command_config is None or isinstance(ssh_proxy_command_config,
                                                       str):
         return
 
     if isinstance(ssh_proxy_command_config, dict):
         for region, cmd in ssh_proxy_command_config.items():
-            if not isinstance(cmd, str):
+            if cmd and not isinstance(cmd, str):
                 raise ValueError(
                     f'Invalid ssh_proxy_command config for region {region!r} '
                     f'(expected a str): {cmd!r}')
         return
     raise ValueError(
         'Invalid ssh_proxy_command config (expected a str or a dict with '
         f'region names as keys): {ssh_proxy_command_config!r}')
```

### Comparing `skypilot-0.2.5/sky/spot/__init__.py` & `skypilot-0.3.0/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/spot/constants.py` & `skypilot-0.3.0/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/spot/controller.py` & `skypilot-0.3.0/sky/spot/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Controller: handles the life cycle of a managed spot cluster (job)."""
 import argparse
 import multiprocessing
 import pathlib
 import time
 import traceback
+from typing import Tuple
 
 import filelock
 
 import sky
 from sky import exceptions
 from sky import global_user_state
 from sky import sky_logging
@@ -17,38 +18,46 @@
 from sky.skylet import job_lib
 from sky.spot import recovery_strategy
 from sky.spot import spot_state
 from sky.spot import spot_utils
 from sky.utils import common_utils
 from sky.utils import subprocess_utils
 
-logger = sky_logging.init_logger(__name__)
+# Use the explicit logger name so that the logger is under the
+# `sky.spot.controller` namespace when executed directly, so as
+# to inherit the setup from the `sky` logger.
+logger = sky_logging.init_logger('sky.spot.controller')
+
+
+def _get_task_and_name(task_yaml: str) -> Tuple['sky.Task', str]:
+    task = sky.Task.from_yaml(task_yaml)
+    assert task.name is not None, task
+    return task, task.name
 
 
 class SpotController:
     """Each spot controller manages the life cycle of one spot cluster (job)."""
 
     def __init__(self, job_id: int, task_yaml: str,
                  retry_until_up: bool) -> None:
         self._job_id = job_id
-        self._task = sky.Task.from_yaml(task_yaml)
-        self._task_name = self._task.name
+        self._task, self._task_name = _get_task_and_name(task_yaml)
 
         self._retry_until_up = retry_until_up
         # TODO(zhwu): this assumes the specific backend.
         self._backend = cloud_vm_ray_backend.CloudVmRayBackend()
 
         # Add a unique identifier to the task environment variables, so that
         # the user can have the same id for multiple recoveries.
         #   Example value: sky-2022-10-04-22-46-52-467694_id-17
         task_envs = self._task.envs or {}
         job_id_env_var = common_utils.get_global_job_id(
             self._backend.run_timestamp, 'spot', str(self._job_id))
         task_envs[constants.JOB_ID_ENV_VAR] = job_id_env_var
-        self._task.set_envs(task_envs)
+        self._task.update_envs(task_envs)
 
         spot_state.set_submitted(
             self._job_id,
             self._task_name,
             self._backend.run_timestamp,
             resources_str=backend_utils.get_task_resources_str(self._task))
         logger.info(f'Submitted spot job; SKYPILOT_JOB_ID: {job_id_env_var}')
@@ -75,16 +84,16 @@
                 due to:
                 1. Any of the underlying failover exceptions is due to resources
                 unavailability.
                 2. The cluster is preempted before the job is submitted.
                 3. Any unexpected error happens during the `sky.launch`.
         Other exceptions may be raised depending on the backend.
         """
-        logger.info(f'Started monitoring spot task {self._task_name} '
-                    f'(id: {self._job_id})')
+        logger.info(f'Started monitoring spot job {self._job_id}, '
+                    f'name: {self._task_name!r}.')
         spot_state.set_starting(self._job_id)
         job_submitted_at = self._strategy_executor.launch()
 
         spot_state.set_started(self._job_id, start_time=job_submitted_at)
         while True:
             time.sleep(spot_utils.JOB_STATUS_CHECK_GAP_SECONDS)
 
@@ -116,14 +125,20 @@
             # For multi-node jobs, since the job may not be set to FAILED
             # immediately (depending on user program) when only some of the
             # nodes are preempted, need to check the actual cluster status.
             if (job_status is not None and not job_status.is_terminal() and
                     self._task.num_nodes == 1):
                 continue
 
+            if job_status in [
+                    job_lib.JobStatus.FAILED, job_lib.JobStatus.FAILED_SETUP
+            ]:
+                # Add a grace period before the check of preemption to avoid
+                # false alarm for job failure.
+                time.sleep(5)
             # Pull the actual cluster status from the cloud provider to
             # determine whether the cluster is preempted.
             (cluster_status,
              handle) = backend_utils.refresh_cluster_status_handle(
                  self._cluster_name, force_refresh=True)
 
             if cluster_status != global_user_state.ClusterStatus.UP:
@@ -144,18 +159,21 @@
                     # The user code has probably crashed, fail immediately.
                     end_time = spot_utils.get_job_timestamp(self._backend,
                                                             self._cluster_name,
                                                             get_end_time=True)
                     logger.info(
                         'The user job failed. Please check the logs below.\n'
                         f'== Logs of the user job (ID: {self._job_id}) ==\n')
-                    self._backend.tail_logs(handle,
-                                            None,
-                                            spot_job_id=self._job_id)
-                    logger.info(f'\n== End of logs (ID: {self._job_id}) ==')
+                    # TODO(zhwu): Download the logs, and stream them from the
+                    # local disk, instead of streaming them from the spot
+                    # cluster, to make it faster and more reliable.
+                    returncode = self._backend.tail_logs(
+                        handle, None, spot_job_id=self._job_id)
+                    logger.info(f'\n== End of logs (ID: {self._job_id}, '
+                                f'tail_logs returncode: {returncode}) ==')
                     spot_status_to_set = spot_state.SpotStatus.FAILED
                     if job_status == job_lib.JobStatus.FAILED_SETUP:
                         spot_status_to_set = spot_state.SpotStatus.FAILED_SETUP
                     failure_reason = (
                         'To see the details, run: '
                         f'sky spot logs --controller {self._job_id}')
 
@@ -262,16 +280,15 @@
     raise exceptions.SpotUserCancelledError(
         f'User sent {user_signal.value} signal.')
 
 
 def _cleanup(job_id: int, task_yaml: str):
     # NOTE: The code to get cluster name is same as what we did in the spot
     # controller, we should keep it in sync with SpotController.__init__()
-    task = sky.Task.from_yaml(task_yaml)
-    task_name = task.name
+    task, task_name = _get_task_and_name(task_yaml)
     cluster_name = spot_utils.generate_spot_cluster_name(task_name, job_id)
     recovery_strategy.terminate_cluster(cluster_name)
     # Clean up Storages with persistent=False.
     # TODO(zhwu): this assumes the specific backend.
     backend = cloud_vm_ray_backend.CloudVmRayBackend()
     backend.teardown_ephemeral_storage(task)
 
@@ -297,34 +314,34 @@
             time.sleep(1)
     except exceptions.SpotUserCancelledError:
         logger.info(f'Cancelling spot job {job_id}...')
         spot_state.set_cancelling(job_id)
         cancelling = True
     finally:
         if controller_process is not None:
-            logger.info(f'Killing controller process {controller_process.pid}')
+            logger.info(f'Killing controller process {controller_process.pid}.')
             # NOTE: it is ok to kill or join a killed process.
             # Kill the controller process first; if its child process is
             # killed first, then the controller process will raise errors.
             # Kill any possible remaining children processes recursively.
             subprocess_utils.kill_children_processes(controller_process.pid,
                                                      force=True)
             controller_process.join()
             logger.info(f'Controller process {controller_process.pid} killed.')
 
-        logger.info(f'Cleaning up spot clusters of job {job_id}.')
+        logger.info(f'Cleaning up spot cluster of job {job_id}.')
         # NOTE: Originally, we send an interruption signal to the controller
         # process and the controller process handles cleanup. However, we
         # figure out the behavior differs from cloud to cloud
         # (e.g., GCP ignores 'SIGINT'). A possible explanation is
         # https://unix.stackexchange.com/questions/356408/strange-problem-with-trap-and-sigint
         # But anyway, a clean solution is killing the controller process
         # directly, and then cleanup the cluster state.
         _cleanup(job_id, task_yaml=task_yaml)
-        logger.info(f'Spot clusters of job {job_id} has been taken down.')
+        logger.info(f'Spot cluster of job {job_id} has been taken down.')
 
         if cancelling:
             spot_state.set_cancelled(job_id)
 
         # We should check job status after 'set_cancelled', otherwise
         # the job status is not terminal.
         job_status = spot_state.get_status(job_id)
```

### Comparing `skypilot-0.2.5/sky/spot/recovery_strategy.py` & `skypilot-0.3.0/sky/spot/recovery_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,16 @@
                 # by the controller process (job_status -> FAILED_SETUP).
                 sky.launch(self.dag,
                            cluster_name=self.cluster_name,
                            detach_setup=True,
                            detach_run=True,
                            _is_launched_by_spot_controller=True)
                 logger.info('Spot cluster launched.')
-            except exceptions.InvalidClusterNameError as e:
+            except (exceptions.InvalidClusterNameError,
+                    exceptions.NoCloudAccessError) as e:
                 logger.error('Failure happened before provisioning. '
                              f'{common_utils.format_exception(e)}')
                 if raise_on_failure:
                     raise exceptions.ProvisionPrechecksError(reasons=[e])
                 return None
             except exceptions.ResourcesUnavailableError as e:
                 # This is raised when the launch fails due to prechecks or
@@ -340,15 +341,16 @@
 
     def _launch(self, max_retry=3, raise_on_failure=True) -> Optional[float]:
         job_submitted_at = super()._launch(max_retry, raise_on_failure)
         if job_submitted_at is not None:
             # Only record the cloud/region if the launch is successful.
             handle = global_user_state.get_handle_from_cluster_name(
                 self.cluster_name)
-            assert handle is not None, 'Cluster should be launched.'
+            assert isinstance(handle, backends.CloudVmRayResourceHandle), (
+                'Cluster should be launched.', handle)
             launched_resources = handle.launched_resources
             self._launched_cloud_region = (launched_resources.cloud,
                                            launched_resources.region)
         return job_submitted_at
 
     def recover(self) -> float:
         # 1. Cancel the jobs and launch the cluster with the STOPPED status,
```

### Comparing `skypilot-0.2.5/sky/spot/spot_state.py` & `skypilot-0.3.0/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/spot/spot_utils.py` & `skypilot-0.3.0/sky/spot/spot_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """User interfaces with managed spot jobs."""
 import collections
 import enum
 import json
 import pathlib
 import shlex
 import time
-from typing import Any, Dict, List, Optional, Sequence, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 import colorama
 import filelock
 
 from sky import backends
 from sky import exceptions
 from sky import global_user_state
@@ -60,14 +60,15 @@
 def get_job_status(backend: 'backends.CloudVmRayBackend',
                    cluster_name: str) -> Optional['job_lib.JobStatus']:
     """Check the status of the job running on the spot cluster.
 
     It can be None, INIT, RUNNING, SUCCEEDED, FAILED, FAILED_SETUP or CANCELLED.
     """
     handle = global_user_state.get_handle_from_cluster_name(cluster_name)
+    assert isinstance(handle, backends.CloudVmRayResourceHandle), handle
     status = None
     try:
         logger.info('=== Checking the job status... ===')
         statuses = backend.get_job_status(handle, stream_logs=False)
         status = list(statuses.values())[0]
         if status is None:
             logger.info('No job found.')
@@ -278,14 +279,15 @@
                 if msg != prev_msg:
                     status_display.update(msg)
                     prev_msg = msg
                 time.sleep(JOB_STATUS_CHECK_GAP_SECONDS)
                 spot_status = spot_state.get_status(job_id)
                 continue
             assert spot_status is not None
+            assert isinstance(handle, backends.CloudVmRayResourceHandle), handle
             status_display.stop()
             returncode = backend.tail_logs(handle,
                                            job_id=None,
                                            spot_job_id=job_id,
                                            follow=follow)
             if returncode == 0:
                 # If the log tailing exit successfully (the real job can be
@@ -378,14 +380,15 @@
         job['job_duration'] = job_duration
         job['status'] = job['status'].value
 
         cluster_name = generate_spot_cluster_name(job['job_name'],
                                                   job['job_id'])
         handle = global_user_state.get_handle_from_cluster_name(cluster_name)
         if handle is not None:
+            assert isinstance(handle, backends.CloudVmRayResourceHandle)
             job['cluster_resources'] = (
                 f'{handle.launched_nodes}x {handle.launched_resources}')
             job['region'] = handle.launched_resources.region
         else:
             job['cluster_resources'] = '-'
             job['region'] = '-'
 
@@ -487,15 +490,15 @@
         code = [
             'job_table = spot_utils.dump_spot_job_queue()',
             'print(job_table, flush=True)',
         ]
         return cls._build(code)
 
     @classmethod
-    def cancel_jobs_by_id(cls, job_ids: Optional[Sequence[int]]) -> str:
+    def cancel_jobs_by_id(cls, job_ids: Optional[List[int]]) -> str:
         code = [
             f'msg = spot_utils.cancel_jobs_by_id({job_ids})',
             'print(msg, end="", flush=True)',
         ]
         return cls._build(code)
 
     @classmethod
```

### Comparing `skypilot-0.2.5/sky/task.py` & `skypilot-0.3.0/sky/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,35 +135,39 @@
             documented above.
           docker_image: (EXPERIMENTAL: Only in effect when LocalDockerBackend
             is used.) The base docker image that this Task will be built on.
             Defaults to 'gpuci/miniforge-cuda:11.4-devel-ubuntu18.04'.
         """
         self.name = name
         self.run = run
-        self.storage_mounts = {}
-        self.storage_plans = {}
+        self.storage_mounts: Dict[str, storage_lib.Storage] = {}
+        self.storage_plans: Dict[storage_lib.Storage,
+                                 storage_lib.StoreType] = {}
         self.setup = setup
         self._envs = envs or {}
         self.workdir = workdir
         self.docker_image = (docker_image if docker_image else
                              'gpuci/miniforge-cuda:11.4-devel-ubuntu18.04')
-        self.num_nodes = num_nodes
+        # Ignore type error due to a mypy bug.
+        # https://github.com/python/mypy/issues/3004
+        self.num_nodes = num_nodes  # type: ignore
 
         self.inputs = None
         self.outputs = None
         self.estimated_inputs_size_gigabytes = None
         self.estimated_outputs_size_gigabytes = None
         # Default to CPUNode
         self.resources = {sky.Resources()}
-        self.time_estimator_func = None
-        self.file_mounts = None
+        self.time_estimator_func: Optional[Callable[['sky.Resources'],
+                                                    int]] = None
+        self.file_mounts: Optional[Dict[str, str]] = None
 
         # Only set when 'self' is a spot controller task: 'self.spot_task' is
         # the underlying managed spot task (Task object).
-        self.spot_task = None
+        self.spot_task: Optional['Task'] = None
 
         # Filled in by the optimizer.  If None, this Task is not planned.
         self.best_resources = None
         # Check if the task is legal.
         self._validate()
 
         dag = sky.dag.get_current_dag()
@@ -285,15 +289,15 @@
                     fm_storages.append((dst_path, src))
                 else:
                     with ux_utils.print_exception_no_traceback():
                         raise ValueError(f'Unable to parse file_mount '
                                          f'{dst_path}:{src}')
             task.set_file_mounts(copy_mounts)
 
-        task_storage_mounts = {}  # type: Dict[str, Storage]
+        task_storage_mounts: Dict[str, storage_lib.Storage] = {}
         all_storages = fm_storages
         for storage in all_storages:
             mount_path = storage[0]
             assert mount_path, \
                 'Storage mount path cannot be empty.'
             try:
                 storage_obj = storage_lib.Storage.from_yaml_config(storage[1])
@@ -329,36 +333,45 @@
         assert not config, f'Invalid task args: {config.keys()}'
         return task
 
     @property
     def num_nodes(self) -> int:
         return self._num_nodes
 
+    @num_nodes.setter
+    def num_nodes(self, num_nodes: Optional[int]) -> None:
+        if num_nodes is None:
+            num_nodes = 1
+        if not isinstance(num_nodes, int) or num_nodes <= 0:
+            with ux_utils.print_exception_no_traceback():
+                raise ValueError(
+                    f'num_nodes should be a positive int. Got: {num_nodes}')
+        self._num_nodes = num_nodes
+
     @property
     def envs(self) -> Dict[str, str]:
         return self._envs
 
-    def set_envs(
-            self, envs: Union[None, Tuple[Tuple[str, str]],
+    def update_envs(
+            self, envs: Union[None, List[Tuple[str, str]],
                               Dict[str, str]]) -> 'Task':
-        """Sets the environment variables for use inside the setup/run commands.
+        """Updates environment variables for use inside the setup/run commands.
 
         Args:
           envs: (optional) either a list of ``(env_name, value)`` or a dict
             ``{env_name: value}``.
 
         Returns:
-          self: The current task, with envs set.
+          self: The current task, with envs updated.
 
         Raises:
           ValueError: if various invalid inputs errors are detected.
         """
         if envs is None:
-            self._envs = {}
-            return self
+            envs = {}
         if isinstance(envs, (list, tuple)):
             keys = set(env[0] for env in envs)
             if len(keys) != len(envs):
                 with ux_utils.print_exception_no_traceback():
                     raise ValueError('Duplicate env keys provided.')
             envs = dict(envs)
         if isinstance(envs, dict):
@@ -370,35 +383,25 @@
                     with ux_utils.print_exception_no_traceback():
                         raise ValueError(f'Invalid env key: {key}')
         else:
             with ux_utils.print_exception_no_traceback():
                 raise ValueError(
                     'envs must be List[Tuple[str, str]] or Dict[str, str]: '
                     f'{envs}')
-        self._envs = envs
+        self._envs.update(envs)
         return self
 
     @property
     def need_spot_recovery(self) -> bool:
         return any(r.spot_recovery is not None for r in self.resources)
 
     @property
     def use_spot(self) -> bool:
         return any(r.use_spot for r in self.resources)
 
-    @num_nodes.setter
-    def num_nodes(self, num_nodes: Optional[int]) -> None:
-        if num_nodes is None:
-            num_nodes = 1
-        if not isinstance(num_nodes, int) or num_nodes <= 0:
-            with ux_utils.print_exception_no_traceback():
-                raise ValueError(
-                    f'num_nodes should be a positive int. Got: {num_nodes}')
-        self._num_nodes = num_nodes
-
     def set_inputs(self, inputs, estimated_size_gigabytes) -> 'Task':
         # E.g., 's3://bucket', 'gs://bucket', or None.
         self.inputs = inputs
         self.estimated_inputs_size_gigabytes = estimated_size_gigabytes
         return self
 
     def get_inputs(self):
@@ -570,14 +573,15 @@
           self: the current task, with file mounts updated.
 
         Raises:
           ValueError: if input paths are invalid.
         """
         if self.file_mounts is None:
             self.file_mounts = {}
+        assert self.file_mounts is not None
         self.file_mounts.update(file_mounts)
         # For validation logic:
         return self.set_file_mounts(self.file_mounts)
 
     def set_storage_mounts(
         self,
         storage_mounts: Optional[Dict[str, storage_lib.Storage]],
@@ -608,15 +612,15 @@
         Returns:
           self: The current task, with storage mounts set.
 
         Raises:
           ValueError: if input paths are invalid.
         """
         if storage_mounts is None:
-            self.storage_mounts = None
+            self.storage_mounts = {}
             return self
         for target, _ in storage_mounts.items():
             # TODO(zhwu): /home/username/sky_workdir as the target path need
             # to be filtered out as well.
             if (target == constants.SKY_REMOTE_WORKDIR and
                     self.workdir is not None):
                 with ux_utils.print_exception_no_traceback():
@@ -678,21 +682,18 @@
             storage_cloud = self.best_resources.cloud
         else:
             resources = list(self.resources)[0]
             storage_cloud = resources.cloud
             if storage_cloud is None:
                 # Get the first enabled cloud.
                 backend_utils.check_public_cloud_enabled()
-                enabled_clouds = global_user_state.get_enabled_clouds()
-
-                for cloud in storage_lib.STORE_ENABLED_CLOUDS:
-                    for enabled_cloud in enabled_clouds:
-                        if cloud.is_same_cloud(enabled_cloud):
-                            storage_cloud = cloud
-                            break
+                enabled_storage_clouds = \
+                    global_user_state.get_enabled_storage_clouds()
+                if enabled_storage_clouds:
+                    storage_cloud = enabled_storage_clouds[0]
         if storage_cloud is None:
             raise ValueError('No available cloud to mount storage.')
         store_type = storage_lib.get_storetype_from_cloud(storage_cloud)
         return store_type
 
     def sync_storage_mounts(self) -> None:
         """(INTERNAL) Eagerly syncs storage mounts to cloud storage.
@@ -713,36 +714,46 @@
         storage_mounts = self.storage_mounts
         storage_plans = self.storage_plans
         for mnt_path, storage in storage_mounts.items():
             if storage.mode == storage_lib.StorageMode.COPY:
                 store_type = storage_plans[storage]
                 if store_type is storage_lib.StoreType.S3:
                     # TODO: allow for Storage mounting of different clouds
-                    if storage.source is not None and not isinstance(
-                            storage.source,
-                            list) and storage.source.startswith('s3://'):
+                    if isinstance(storage.source,
+                                  str) and storage.source.startswith('s3://'):
                         blob_path = storage.source
                     else:
+                        assert storage.name is not None, storage
                         blob_path = 's3://' + storage.name
                     self.update_file_mounts({
                         mnt_path: blob_path,
                     })
                 elif store_type is storage_lib.StoreType.GCS:
+                    if isinstance(storage.source,
+                                  str) and storage.source.startswith('gs://'):
+                        blob_path = storage.source
+                    else:
+                        assert storage.name is not None, storage
+                        blob_path = 'gs://' + storage.name
+                    self.update_file_mounts({
+                        mnt_path: blob_path,
+                    })
+                elif store_type is storage_lib.StoreType.R2:
                     if storage.source is not None and not isinstance(
                             storage.source,
-                            list) and storage.source.startswith('gs://'):
+                            list) and storage.source.startswith('r2://'):
                         blob_path = storage.source
                     else:
-                        blob_path = 'gs://' + storage.name
+                        blob_path = 'r2://' + storage.name
                     self.update_file_mounts({
                         mnt_path: blob_path,
                     })
                 elif store_type is storage_lib.StoreType.AZURE:
                     # TODO when Azure Blob is done: sync ~/.azure
-                    assert False, 'TODO: Azure Blob not mountable yet'
+                    raise NotImplementedError('Azure Blob not mountable yet')
                 else:
                     with ux_utils.print_exception_no_traceback():
                         raise ValueError(f'Storage Type {store_type} '
                                          'does not exist!')
 
     def get_local_to_remote_file_mounts(self) -> Optional[Dict[str, str]]:
         """Returns file mounts of the form (dst=VM path, src=local path).
@@ -824,32 +835,35 @@
             })
         return config
 
     def __rshift__(self, b):
         sky.dag.get_current_dag().add_edge(self, b)
 
     def __repr__(self):
-        if self.name:
+        if self.name and self.name != 'sky-cmd':  # CLI launch with a command
             return self.name
         if isinstance(self.run, str):
             run_msg = self.run.replace('\n', '\\n')
             if len(run_msg) > 20:
                 run_msg = f'run=\'{run_msg[:20]}...\''
             else:
                 run_msg = f'run=\'{run_msg}\''
         elif self.run is None:
-            run_msg = 'run=None'
+            run_msg = 'run=<empty>'
         else:
             run_msg = 'run=<fn>'
 
         s = f'Task({run_msg})'
         if self.inputs is not None:
             s += f'\n  inputs: {self.inputs}'
         if self.outputs is not None:
             s += f'\n  outputs: {self.outputs}'
         if self.num_nodes > 1:
             s += f'\n  nodes: {self.num_nodes}'
-        if len(self.resources) > 1 or not list(self.resources)[0].is_empty():
+        if len(self.resources) > 1:
             s += f'\n  resources: {self.resources}'
+        elif len(
+                self.resources) == 1 and not list(self.resources)[0].is_empty():
+            s += f'\n  resources: {list(self.resources)[0]}'
         else:
             s += '\n  resources: default instances'
         return s
```

### Comparing `skypilot-0.2.5/sky/templates/aws-ray.yml.j2` & `skypilot-0.3.0/sky/templates/aws-ray.yml.j2`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   # NOTE: This is a new field added by SkyPilot and parsed by our own
   # AWSNodeProvider.
   vpc_name: {{vpc_name}}
 {% endif %}
   use_internal_ips: {{use_internal_ips}}
   # Disable launch config check for worker nodes as it can cause resource
   # leakage.
-  # Reference: https://github.com/ray-project/ray/blob/840215bc09e942b50cad0ab2db96a8fdc79217c1/python/ray/autoscaler/_private/autoscaler.py#L1101
+  # Reference: https://github.com/ray-project/ray/blob/cd1ba65e239360c8a7b130f991ed414eccc063ce/python/ray/autoscaler/_private/autoscaler.py#L1115
   # The upper-level SkyPilot code has make sure there will not be resource
   # leakage.
   disable_launch_config_check: true
 
 auth:
   ssh_user: ubuntu
   ssh_private_key: {{ssh_private_key}}
@@ -43,57 +43,114 @@
       InstanceType: {{instance_type}}
       ImageId: {{image_id}}  # Deep Learning AMI (Ubuntu 18.04); see aws.py.
       # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_instances
       BlockDeviceMappings:
         - DeviceName: /dev/sda1
           Ebs:
             VolumeSize: {{disk_size}}
-            # use default Iops for gp3
-            VolumeType: gp3
-            Iops: 3000
-            Throughput: 125 
+            VolumeType: {{disk_tier}}
+            {% if custom_disk_perf %}
+            Iops: {{disk_iops}}
+            Throughput: {{disk_throughput}}
+            {% endif %}
       {% if use_spot %}
       InstanceMarketOptions:
           MarketType: spot
           # Additional options can be found in the boto docs, e.g.
           #   SpotOptions:
           #       MaxPrice: MAX_HOURLY_PRICE
       {% endif %}
+      # Use cloud init in UserData to set up the authorized_keys to get
+      # around the number of keys limit and permission issues with
+      # ec2.describe_key_pairs.
+      # Note that sudo and shell need to be specified to ensure setup works.
+      # Reference: https://cloudinit.readthedocs.io/en/latest/reference/modules.html#users-and-groups
+      # The bootcmd is to disable automatic APT updates, to avoid the lock
+      # when user call `apt install` on the node.
+      # Reference: https://askubuntu.com/questions/1322292/how-do-i-turn-off-automatic-updates-completely-and-for-real
+      UserData: |
+        #cloud-config
+        users:
+          - name: skypilot:ssh_user
+            shell: /bin/bash
+            sudo: ALL=(ALL) NOPASSWD:ALL
+            ssh_authorized_keys:
+              - skypilot:ssh_public_key_content
+        write_files:
+          - path: /etc/apt/apt.conf.d/20auto-upgrades
+            content: |
+              APT::Periodic::Update-Package-Lists "0";
+              APT::Periodic::Download-Upgradeable-Packages "0";
+              APT::Periodic::AutocleanInterval "0";
+              APT::Periodic::Unattended-Upgrade "0";
+          - path: /etc/apt/apt.conf.d/10cloudinit-disable
+            content: |
+              APT::Periodic::Enable "0";
       TagSpecifications:
         - ResourceType: instance
           Tags:
             - Key: skypilot-user
               Value: {{ user }}
+{%- for tag_key, tag_value in instance_tags.items() %}
+            - Key: {{ tag_key }}
+              Value: {{ tag_value }}
+{%- endfor %}
+
 {% if num_nodes > 1 %}
   ray.worker.default:
     min_workers: {{num_nodes - 1}}
     max_workers: {{num_nodes - 1}}
     resources: {}
     node_config:
       InstanceType: {{instance_type}}
       ImageId: {{image_id}}  # Deep Learning AMI (Ubuntu 18.04); see aws.py.
       BlockDeviceMappings:
         - DeviceName: /dev/sda1
           Ebs:
             VolumeSize: {{disk_size}}
-            VolumeType: gp3
-            Iops: 3000
-            Throughput: 125 
+            VolumeType: {{disk_tier}}
+            {% if custom_disk_perf %}
+            Iops: {{disk_iops}}
+            Throughput: {{disk_throughput}}
+            {% endif %}
       {% if use_spot %}
       InstanceMarketOptions:
           MarketType: spot
           # Additional options can be found in the boto docs, e.g.
           #   SpotOptions:
           #       MaxPrice: MAX_HOURLY_PRICE
       {% endif %}
+      UserData: |
+        #cloud-config
+        users:
+          - name: skypilot:ssh_user
+            shell: /bin/bash
+            sudo: ALL=(ALL) NOPASSWD:ALL
+            ssh_authorized_keys:
+              - skypilot:ssh_public_key_content
+        write_files:
+          - path: /etc/apt/apt.conf.d/20auto-upgrades
+            content: |
+              APT::Periodic::Update-Package-Lists "0";
+              APT::Periodic::Download-Upgradeable-Packages "0";
+              APT::Periodic::AutocleanInterval "0";
+              APT::Periodic::Unattended-Upgrade "0";
+          - path: /etc/apt/apt.conf.d/10cloudinit-disable
+            content: |
+              APT::Periodic::Enable "0";
       TagSpecifications:
         - ResourceType: instance
           Tags:
             - Key: skypilot-user
               Value: {{ user }}
+{%- for tag_key, tag_value in instance_tags.items() %}
+            - Key: {{ tag_key }}
+              Value: {{ tag_value }}
+{%- endfor %}
+
 {%- endif %}
 
 head_node_type: ray.head.default
 
 # Format: `REMOTE_PATH : LOCAL_PATH`
 file_mounts: {
   "{{sky_ray_yaml_remote_path}}": "{{sky_ray_yaml_local_path}}",
@@ -120,32 +177,22 @@
   # Make sure python3 & pip3 are available on this image.
   # We set auto_activate_base to be false for pre-installed conda.
   # This also kills the service that is holding the lock on dpkg (problem only exists on aws/azure, not gcp)
   # Line 'sudo bash ..': set the ulimit as suggested by ray docs for performance. https://docs.ray.io/en/latest/cluster/vms/user-guides/large-cluster-best-practices.html#system-configuration
   # Line 'sudo grep ..': set the number of threads per process to unlimited to avoid ray job submit stucking issue when the number of running ray jobs increase.
   # Line 'mkdir -p ..': disable host key check
   # Line 'python3 -c ..': patch the buggy ray files and enable `-o allow_other` option for `goofys`
-  - function mylsof { p=$(for pid in /proc/{0..9}*; do i=$(basename "$pid"); for file in "$pid"/fd/*; do link=$(readlink -e "$file"); if [ "$link" = "$1" ]; then echo "$i"; fi; done; done); echo "$p"; };
-    sudo systemctl stop unattended-upgrades || true;
-    sudo systemctl disable unattended-upgrades || true;
-    sudo sed -i 's/Unattended-Upgrade "1"/Unattended-Upgrade "0"/g' /etc/apt/apt.conf.d/20auto-upgrades || true;
-    p=$(mylsof "/var/lib/dpkg/lock-frontend"); echo "$p";
-    sudo kill -9 `echo "$p" | tail -n 1` || true;
-    sudo rm /var/lib/dpkg/lock-frontend;
-    sudo pkill -9 dpkg;
-    sudo pkill -9 apt-get;
-    sudo dpkg --configure --force-overwrite -a;
-    mkdir -p ~/.ssh; touch ~/.ssh/config;
+  - mkdir -p ~/.ssh; touch ~/.ssh/config;
     pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
     (which conda > /dev/null 2>&1 && conda init > /dev/null) || (wget -nc https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh && bash Miniconda3-latest-Linux-x86_64.sh -b && eval "$(~/miniconda3/bin/conda shell.bash hook)" && conda init && conda config --set auto_activate_base true);
     source ~/.bashrc;
-    (pip3 list | grep ray | grep {{ray_version}} 2>&1 > /dev/null || pip3 install -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app;
-    (pip3 list | grep skypilot && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[aws]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
+    (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app;
+    (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[aws]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
     [ -f /etc/fuse.conf ] && sudo sed -i 's/#user_allow_other/user_allow_other/g' /etc/fuse.conf || (sudo sh -c 'echo "user_allow_other" > /etc/fuse.conf'); # This is needed for `-o allow_other` option for `goofys`;
 
 # Command to start ray on the head node. You don't need to change this.
@@ -157,20 +204,21 @@
 #   current num items (num SSH connections): 1
 head_start_ray_commands:
   # Start skylet daemon. (Should not place it in the head_setup_commands, otherwise it will run before sky is installed.)
   # NOTE: --disable-usage-stats in `ray start` saves 10 seconds of idle wait.
   # Line "which prlimit ..": increase the limit of the number of open files for the raylet process, as the `ulimit` may not take effect at this point, because it requires
   # all the sessions to be reloaded. This is a workaround.
   - ((ps aux | grep -v nohup | grep -v grep | grep -q -- "python3 -m sky.skylet.skylet") || nohup python3 -m sky.skylet.skylet >> ~/.sky/skylet.log 2>&1 &);
-    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --head --port=6379 --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} || exit 1;
+    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
+    {{dump_port_command}};
 
 {%- if num_nodes > 1 %}
 worker_start_ray_commands:
-  - ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:6379 --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} || exit 1;
+  - ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
 {%- else %}
 worker_start_ray_commands: []
 {%- endif %}
 
 head_node: {}
 worker_nodes: {}
```

### Comparing `skypilot-0.2.5/sky/templates/azure-ray.yml.j2` & `skypilot-0.3.0/sky/templates/azure-ray.yml.j2`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     # Keep (otherwise cannot reuse when re-provisioning).
     # teardown(terminate=True) will override this.
     cache_stopped_nodes: True
     # subscription id of the azure user
     subscription_id: {{azure_subscription_id}}
     # Disable launch config check for worker nodes as it can cause resource
     # leakage.
-    # Reference: https://github.com/ray-project/ray/blob/840215bc09e942b50cad0ab2db96a8fdc79217c1/python/ray/autoscaler/_private/autoscaler.py#L1101
+    # Reference: https://github.com/ray-project/ray/blob/cd1ba65e239360c8a7b130f991ed414eccc063ce/python/ray/autoscaler/_private/autoscaler.py#L1115
     # The upper-level SkyPilot code has make sure there will not be resource
     # leakage.
     disable_launch_config_check: true
 
 
 auth:
     ssh_user: azureuser
@@ -41,14 +41,15 @@
             vmSize: {{instance_type}}
             # List images https://docs.microsoft.com/en-us/azure/virtual-machines/linux/cli-ps-findimage
             imagePublisher: {{image_publisher}}
             imageOffer: {{image_offer}}
             imageSku: "{{image_sku}}"
             imageVersion: {{image_version}}
             osDiskSizeGB: {{disk_size}}
+            osDiskTier: {{disk_tier}}
             # optionally set priority to use Spot instances
             {%- if use_spot %}
             priority: Spot
             # set a maximum price for spot instances if desired
             # billingProfile:
             #     maxPrice: -1
             {%- endif %}
@@ -65,14 +66,15 @@
             vmSize: {{instance_type}}
             # List images https://docs.microsoft.com/en-us/azure/virtual-machines/linux/cli-ps-findimage
             imagePublisher: {{image_publisher}}
             imageOffer: {{image_offer}}
             imageSku: "{{image_sku}}"
             imageVersion: {{image_version}}
             osDiskSizeGB: {{disk_size}}
+            osDiskTier: {{disk_tier}}
           {%- if use_spot %}
             priority: Spot
             # set a maximum price for spot instances if desired
             # billingProfile:
             #     maxPrice: -1
           {%- endif %}
 {%- endif %}
@@ -120,16 +122,16 @@
     sudo dpkg --configure --force-overwrite -a;
     mkdir -p ~/.ssh; touch ~/.ssh/config;
     pip3 --version > /dev/null 2>&1 || (curl -sSL https://bootstrap.pypa.io/get-pip.py -o get-pip.py && python3 get-pip.py && echo "PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc);
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
     which conda > /dev/null 2>&1 || (wget -nc https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh && bash Miniconda3-latest-Linux-x86_64.sh -b && eval "$(/home/azureuser/miniconda3/bin/conda shell.bash hook)" && conda init && conda config --set auto_activate_base true);
     source ~/.bashrc;
-    (pip3 list | grep ray | grep {{ray_version}} 2>&1 > /dev/null || pip3 install -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app && touch ~/.sudo_as_admin_successful;
-    (pip3 list | grep skypilot && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[azure]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
+    (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app && touch ~/.sudo_as_admin_successful;
+    (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[azure]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
     [ -f /etc/fuse.conf ] && sudo sed -i 's/#user_allow_other/user_allow_other/g' /etc/fuse.conf || (sudo sh -c 'echo "user_allow_other" > /etc/fuse.conf');
 
 # Command to start ray on the head node. You don't need to change this.
@@ -139,20 +141,21 @@
 #
 # Increment the following for catching performance bugs easier:
 #   current num items (num SSH connections): 2
 head_start_ray_commands:
   # Start skylet daemon. (Should not place it in the head_setup_commands, otherwise it will run before skypilot is installed.)
   # NOTE: --disable-usage-stats in `ray start` saves 10 seconds of idle wait.
   - ((ps aux | grep -v nohup | grep -v grep | grep -q -- "python3 -m sky.skylet.skylet") || nohup python3 -m sky.skylet.skylet >> ~/.sky/skylet.log 2>&1 &);
-    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --head --port=6379 --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} || exit 1;
+    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
+    {{dump_port_command}};
 
 {%- if num_nodes > 1 %}
 worker_start_ray_commands:
-  - ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:6379 --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} || exit 1;
+  - ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
 {%- else %}
 worker_start_ray_commands: []
 {%- endif %}
 
 head_node: {}
 worker_nodes: {}
```

### Comparing `skypilot-0.2.5/sky/templates/gcp-ray.yml.j2` & `skypilot-0.3.0/sky/templates/gcp-ray.yml.j2`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   # The GCP project ID.
   project_id: {{gcp_project_id}}
 {%- if tpu_vm %}
   _has_tpus: True
 {%- endif %}
   # Disable launch config check for worker nodes as it can cause resource
   # leakage.
-  # Reference: https://github.com/ray-project/ray/blob/840215bc09e942b50cad0ab2db96a8fdc79217c1/python/ray/autoscaler/_private/autoscaler.py#L1101
+  # Reference: https://github.com/ray-project/ray/blob/cd1ba65e239360c8a7b130f991ed414eccc063ce/python/ray/autoscaler/_private/autoscaler.py#L1115
   # The upper-level SkyPilot code has make sure there will not be resource
   # leakage.
   disable_launch_config_check: true
 
 auth:
   ssh_user: gcpuser
   ssh_private_key: {{ssh_private_key}}
@@ -50,14 +50,15 @@
         - boot: true
           autoDelete: true
           type: PERSISTENT
           initializeParams:
             diskSizeGb: {{disk_size}}
             # See https://cloud.google.com/deep-learning-vm/docs/images
             sourceImage: {{image_id}}
+            diskType: zones/{{zones}}/diskTypes/{{disk_tier}}
   {%- if gpu is not none %}
       guestAccelerators:
         - acceleratorType: projects/{{gcp_project_id}}/zones/{{zones}}/acceleratorTypes/{{gpu}}
           acceleratorCount: {{gpu_count}}
       metadata:
         items:
           - key: install-nvidia-driver
@@ -92,14 +93,15 @@
         - boot: true
           autoDelete: true
           type: PERSISTENT
           initializeParams:
             diskSizeGb: {{disk_size}}
             # See https://cloud.google.com/deep-learning-vm/docs/images
             sourceImage: {{image_id}}
+            diskType: zones/{{zones}}/diskTypes/{{disk_tier}}
     {%- if gpu is not none %}
       guestAccelerators:
         - acceleratorType: projects/{{gcp_project_id}}/zones/{{zones}}/acceleratorTypes/{{gpu}}
           acceleratorCount: {{gpu_count}}
       metadata:
         items:
           - key: install-nvidia-driver
@@ -164,16 +166,16 @@
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
     which conda > /dev/null 2>&1 || (wget -nc https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh && bash Miniconda3-latest-Linux-x86_64.sh -b && eval "$(/home/gcpuser/miniconda3/bin/conda shell.bash hook)" && conda init && conda config --set auto_activate_base true);
     source ~/.bashrc;
   {%- if tpu_vm %}
     test -f /home/gcpuser/miniconda3/etc/profile.d/conda.sh && source /home/gcpuser/miniconda3/etc/profile.d/conda.sh && conda activate base || true;
     pip3 install --upgrade google-api-python-client;
   {%- endif %}
-    (pip3 list | grep ray | grep {{ray_version}} 2>&1 > /dev/null || pip3 install -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app;
-    (pip3 list | grep skypilot && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[gcp]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
+    (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app;
+    (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[gcp]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
     [ -f /etc/fuse.conf ] && sudo sed -i 's/#user_allow_other/user_allow_other/g' /etc/fuse.conf || (sudo sh -c 'echo "user_allow_other" > /etc/fuse.conf');
 
 # Command to start ray on the head node. You don't need to change this.
@@ -186,22 +188,23 @@
 head_start_ray_commands:
   # Start skylet daemon. (Should not place it in the head_setup_commands, otherwise it will run before sky is installed.)
   # NOTE: --disable-usage-stats in `ray start` saves 10 seconds of idle wait.
   # Line "which prlimit ..": increase the limit of the number of open files for the raylet process, as the `ulimit` may not take effect at this point, because it requires
   # all the sessions to be reloaded. This is a workaround.
   - ((ps aux | grep -v nohup | grep -v grep | grep -q -- "python3 -m sky.skylet.skylet") || nohup python3 -m sky.skylet.skylet >> ~/.sky/skylet.log 2>&1 &);
     export SKYPILOT_NUM_GPUS=0 && which nvidia-smi > /dev/null && SKYPILOT_NUM_GPUS=$(nvidia-smi --query-gpu=index,name --format=csv,noheader | wc -l);
-    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --head --port=6379 --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --num-gpus=$SKYPILOT_NUM_GPUS || exit 1;
+    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --num-gpus=$SKYPILOT_NUM_GPUS --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
+    {{dump_port_command}};
 
 # Worker commands are needed for TPU VM Pods
 {%- if num_nodes > 1 or tpu_vm %}
 worker_start_ray_commands:
   - SKYPILOT_NUM_GPUS=0 && which nvidia-smi > /dev/null && SKYPILOT_NUM_GPUS=$(nvidia-smi --query-gpu=index,name --format=csv,noheader | wc -l);
-    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:6379 --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --num-gpus=$SKYPILOT_NUM_GPUS || exit 1;
+    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --num-gpus=$SKYPILOT_NUM_GPUS --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
 {%- else %}
 worker_start_ray_commands: []
 {%- endif %}
 
 head_node: {}
 worker_nodes: {}
```

### Comparing `skypilot-0.2.5/sky/templates/lambda-ray.yml.j2` & `skypilot-0.3.0/sky/templates/lambda-ray.yml.j2`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 provider:
   type: external
   module: sky.skylet.providers.lambda_cloud.LambdaNodeProvider
   region: {{region}}
   # Disable launch config check for worker nodes as it can cause resource
   # leakage.
-  # Reference: https://github.com/ray-project/ray/blob/840215bc09e942b50cad0ab2db96a8fdc79217c1/python/ray/autoscaler/_private/autoscaler.py#L1101
+  # Reference: https://github.com/ray-project/ray/blob/cd1ba65e239360c8a7b130f991ed414eccc063ce/python/ray/autoscaler/_private/autoscaler.py#L1115
   # The upper-level SkyPilot code has make sure there will not be resource
   # leakage.
   disable_launch_config_check: true
 
 auth:
   ssh_user: ubuntu
   ssh_private_key: {{ssh_private_key}}
@@ -73,16 +73,16 @@
     sudo dpkg --configure -a;
     mkdir -p ~/.ssh; touch ~/.ssh/config;
     rm ~/.local/bin/pip ~/.local/bin/pip3 ~/.local/bin/pip3.8 ~/.local/bin/pip3.10;
     (type -a python | grep -q python3) || echo 'alias python=python3' >> ~/.bashrc;
     (type -a pip | grep -q pip3) || echo 'alias pip=pip3' >> ~/.bashrc;
     which conda > /dev/null 2>&1 || (wget -nc https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh && bash Miniconda3-latest-Linux-x86_64.sh -b && eval "$(~/miniconda3/bin/conda shell.bash hook)" && conda init && conda config --set auto_activate_base true);
     source ~/.bashrc;
-    (pip3 list | grep ray | grep {{ray_version}} 2>&1 > /dev/null || pip3 install -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app && touch ~/.sudo_as_admin_successful;
-    (pip3 list | grep skypilot && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[lambda]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
+    (pip3 list | grep "ray " | grep {{ray_version}} 2>&1 > /dev/null || pip3 install --exists-action w -U ray[default]=={{ray_version}}) && mkdir -p ~/sky_workdir && mkdir -p ~/.sky/sky_app && touch ~/.sudo_as_admin_successful;
+    (pip3 list | grep "skypilot " && [ "$(cat {{sky_remote_path}}/current_sky_wheel_hash)" == "{{sky_wheel_hash}}" ]) || (pip3 uninstall skypilot -y; pip3 install "$(echo {{sky_remote_path}}/{{sky_wheel_hash}}/skypilot-{{sky_version}}*.whl)[lambda]" && echo "{{sky_wheel_hash}}" > {{sky_remote_path}}/current_sky_wheel_hash || exit 1);
     sudo bash -c 'rm -rf /etc/security/limits.d; echo "* soft nofile 1048576" >> /etc/security/limits.conf; echo "* hard nofile 1048576" >> /etc/security/limits.conf';
     sudo grep -e '^DefaultTasksMax' /etc/systemd/system.conf || (sudo bash -c 'echo "DefaultTasksMax=infinity" >> /etc/systemd/system.conf'); sudo systemctl set-property user-$(id -u $(whoami)).slice TasksMax=infinity; sudo systemctl daemon-reload;
     mkdir -p ~/.ssh; (grep -Pzo -q "Host \*\n  StrictHostKeyChecking no" ~/.ssh/config) || printf "Host *\n  StrictHostKeyChecking no\n" >> ~/.ssh/config;
     python3 -c "from sky.skylet.ray_patches import patch; patch()" || exit 1;
     [ -f /etc/fuse.conf ] && sudo sed -i 's/#user_allow_other/user_allow_other/g' /etc/fuse.conf || (sudo sh -c 'echo "user_allow_other" > /etc/fuse.conf');
 
 # Command to start ray on the head node. You don't need to change this.
@@ -91,20 +91,21 @@
 # items! The same comment applies for worker_start_ray_commands.
 #
 # Increment the following for catching performance bugs easier:
 #   current num items (num SSH connections): 2
 head_start_ray_commands:
   # Start skylet daemon. (Should not place it in the head_setup_commands, otherwise it will run before skypilot is installed.)
   - ((ps aux | grep -v nohup | grep -v grep | grep -q -- "python3 -m sky.skylet.skylet") || nohup python3 -m sky.skylet.skylet >> ~/.sky/skylet.log 2>&1 &);
-    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --head --port=6379 --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} || exit 1;
+    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
+    {{dump_port_command}};
 
 {%- if num_nodes > 1 %}
 worker_start_ray_commands:
-  - ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:6379 --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} || exit 1;
+  - ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
 {%- else %}
 worker_start_ray_commands: []
 {%- endif %}
 
 head_node: {}
 worker_nodes: {}
```

### Comparing `skypilot-0.2.5/sky/templates/local-ray.yml.j2` & `skypilot-0.3.0/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/templates/spot-controller.yaml.j2` & `skypilot-0.3.0/sky/templates/spot-controller.yaml.j2`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # The template for the spot controller
 
 name: {{task_name}}
 
 resources:
   disk_size: 50
 # It is now using default CPU instance type hard-coded in code for spot controller,
-# i.e. m6i.2xlarge (8vCPUs, 32 GB) for AWS, Standard_D8_v4 (8vCPUs, 32 GB) for Azure, and n1-highmem-8 (8 vCPUs, 52 GB) for GCP.
+# i.e. m6i.2xlarge (8vCPUs, 32 GB) for AWS, Standard_D8s_v4 (8vCPUs, 32 GB) for Azure, and n1-highmem-8 (8 vCPUs, 52 GB) for GCP.
 # This allows users without the credits for some of the clouds available to use managed spot instances.
 # TODO(zhwu): Fix this to be able to failvoer across clouds with cheaper instance.
 #  instance_type: t3.xlarge
 
 file_mounts:
   {{remote_user_yaml_prefix}}/{{task_name}}-{{uuid}}.yaml: {{user_yaml_path}}
 {% if user_config_path is not none %}
@@ -47,10 +47,13 @@
   SKYPILOT_USER: {{user}}
 {% if user_config_path is not none %}
   {{env_var_skypilot_config}}: {{remote_user_yaml_prefix}}/{{task_name}}-{{uuid}}.config_yaml
 {% endif %}
 {% if is_dev %}
   SKYPILOT_DEV: 1
 {% endif %}
+{% if is_debug %}
+  SKYPILOT_DEBUG: 1
+{% endif %}
 {% if disable_logging %}
   SKYPILOT_DISABLE_USAGE_COLLECTION: 1
 {% endif %}
```

### Comparing `skypilot-0.2.5/sky/usage/constants.py` & `skypilot-0.3.0/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/usage/usage_lib.py` & `skypilot-0.3.0/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/utils/accelerator_registry.py` & `skypilot-0.3.0/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/utils/cli_utils/status_utils.py` & `skypilot-0.3.0/sky/utils/cli_utils/status_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from sky import global_user_state
 from sky import spot
 from sky.backends import backend_utils
 from sky.utils import common_utils
 from sky.utils import log_utils
 
 _COMMAND_TRUNC_LENGTH = 25
+NUM_COST_REPORT_LINES = 5
 
 # A record in global_user_state's 'clusters' table.
 _ClusterRecord = Dict[str, Any]
 # A record returned by core.cost_report(); see its docstr for all fields.
 _ClusterCostReportRecord = Dict[str, Any]
 
 
@@ -100,19 +101,48 @@
     if cluster_records:
         click.echo(cluster_table)
     else:
         click.echo('No existing clusters.')
     return num_pending_autostop
 
 
+def get_total_cost_of_displayed_records(
+        cluster_records: List[_ClusterCostReportRecord], display_all: bool):
+    """Compute total cost of records to be displayed in cost report."""
+    cluster_records.sort(
+        key=lambda report: -_get_status_value_for_cost_report(report))
+
+    displayed_records = cluster_records[:NUM_COST_REPORT_LINES]
+    if display_all:
+        displayed_records = cluster_records
+
+    total_cost = sum(record['total_cost'] for record in displayed_records)
+    return total_cost
+
+
 def show_cost_report_table(cluster_records: List[_ClusterCostReportRecord],
                            show_all: bool,
                            reserved_group_name: Optional[str] = None):
     """Compute cluster table values and display for cost report.
 
+    For each cluster, this shows: cluster name, resources, launched time,
+    duration that cluster was up, and total estimated cost.
+
+    The estimated cost column indicates the price for the cluster based on the
+    type of resources being used and the duration of use up until now. This
+    means if the cluster is UP, successive calls to cost-report will show
+    increasing price.
+
+    The estimated cost is calculated based on the local cache of the cluster
+    status, and may not be accurate for:
+
+      - clusters with autostop/use_spot set; or
+
+      - clusters that were terminated/stopped on the cloud console.
+
     Returns:
         Number of pending auto{stop,down} clusters.
     """
     # TODO(zhwu): Update the information for autostop clusters.
 
     status_columns = [
         StatusColumn('NAME', _get_name),
@@ -120,29 +150,37 @@
         StatusColumn('DURATION', _get_duration, trunc_length=20),
         StatusColumn('RESOURCES',
                      _get_resources_for_cost_report,
                      trunc_length=70 if not show_all else 0),
         StatusColumn('STATUS',
                      _get_status_for_cost_report,
                      show_by_default=True),
-        StatusColumn('HOURLY_PRICE',
+        StatusColumn('COST/hr',
                      _get_price_for_cost_report,
                      show_by_default=True),
         StatusColumn('COST (est.)',
                      _get_estimated_cost_for_cost_report,
                      show_by_default=True),
     ]
 
     columns = []
     for status_column in status_columns:
         if status_column.show_by_default or show_all:
             columns.append(status_column.name)
     cluster_table = log_utils.create_table(columns)
 
-    for record in cluster_records:
+    num_lines_to_display = NUM_COST_REPORT_LINES
+    if show_all:
+        num_lines_to_display = len(cluster_records)
+
+    # prioritize showing non-terminated clusters in table
+    cluster_records.sort(
+        key=lambda report: -_get_status_value_for_cost_report(report))
+
+    for record in cluster_records[:num_lines_to_display]:
         row = []
         for status_column in status_columns:
             if status_column.show_by_default or show_all:
                 row.append(status_column.calc(record))
         cluster_table.add_row(row)
 
     if cluster_records:
@@ -321,14 +359,22 @@
     return cluster_record['autostop'] >= 0 and _get_status(
         cluster_record) != global_user_state.ClusterStatus.STOPPED
 
 
 # ---- 'sky cost-report' helper functions below ----
 
 
+def _get_status_value_for_cost_report(
+        cluster_cost_report_record: _ClusterCostReportRecord) -> int:
+    status = cluster_cost_report_record['status']
+    if status is None:
+        return -1
+    return 1
+
+
 def _get_status_for_cost_report(
         cluster_cost_report_record: _ClusterCostReportRecord) -> str:
     status = cluster_cost_report_record['status']
     if status is None:
         return f'{colorama.Style.DIM}TERMINATED{colorama.Style.RESET_ALL}'
     return status.colored_str()
 
@@ -347,19 +393,19 @@
 
 def _get_price_for_cost_report(
         cluster_cost_report_record: _ClusterCostReportRecord) -> str:
     launched_nodes = cluster_cost_report_record['num_nodes']
     launched_resources = cluster_cost_report_record['resources']
 
     hourly_cost = (launched_resources.get_cost(3600) * launched_nodes)
-    price_str = f'$ {hourly_cost:.3f}'
+    price_str = f'$ {hourly_cost:.2f}'
     return price_str
 
 
 def _get_estimated_cost_for_cost_report(
         cluster_cost_report_record: _ClusterCostReportRecord) -> str:
     cost = cluster_cost_report_record['total_cost']
 
     if not cost:
         return '-'
 
-    return f'${cost:.3f}'
+    return f'$ {cost:.2f}'
```

### Comparing `skypilot-0.2.5/sky/utils/command_runner.py` & `skypilot-0.3.0/sky/utils/command_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Runner for commands to be executed on the cluster."""
 import getpass
 import enum
 import hashlib
 import os
 import pathlib
 import shlex
+import time
 from typing import List, Optional, Tuple, Union
 
 from sky import sky_logging
-from sky.utils import subprocess_utils
+from sky.utils import common_utils, subprocess_utils
 from sky.skylet import log_lib
 
 logger = sky_logging.init_logger(__name__)
 
 # The git exclude file to support.
 GIT_EXCLUDE = '.git/info/exclude'
 # Rsync options
@@ -288,24 +289,27 @@
         source: str,
         target: str,
         *,
         up: bool,
         # Advanced options.
         log_path: str = os.devnull,
         stream_logs: bool = True,
+        max_retry: int = 1,
     ) -> None:
         """Uses 'rsync' to sync 'source' to 'target'.
 
         Args:
             source: The source path.
             target: The target path.
             up: The direction of the sync, True for local to cluster, False
               for cluster to local.
             log_path: Redirect stdout/stderr to the log_path.
             stream_logs: Stream logs to the stdout/stderr.
+            max_retry: The maximum number of retries for the rsync command.
+              This value should be non-negative.
 
         Raises:
             exceptions.CommandError: rsync command failed.
         """
         # Build command.
         # TODO(zhwu): This will print a per-file progress bar (with -P),
         # shooting a lot of messages to the output. --info=progress2 is used
@@ -347,20 +351,28 @@
         else:
             rsync_command.extend([
                 f'{self.ssh_user}@{self.ip}:{source!r}',
                 f'{os.path.expanduser(target)!r}',
             ])
         command = ' '.join(rsync_command)
 
-        returncode, _, stderr = log_lib.run_with_log(command,
-                                                     log_path=log_path,
-                                                     stream_logs=stream_logs,
-                                                     shell=True,
-                                                     require_outputs=True)
+        backoff = common_utils.Backoff(initial_backoff=5, max_backoff_factor=5)
+        while max_retry >= 0:
+            returncode, _, stderr = log_lib.run_with_log(
+                command,
+                log_path=log_path,
+                stream_logs=stream_logs,
+                shell=True,
+                require_outputs=True)
+            if returncode == 0:
+                break
+            max_retry -= 1
+            time.sleep(backoff.current_backoff())
 
         direction = 'up' if up else 'down'
-        subprocess_utils.handle_returncode(
-            returncode,
-            command,
-            f'Failed to rsync {direction}: {source} -> {target}',
-            stderr=stderr,
-            stream_logs=stream_logs)
+        error_msg = (f'Failed to rsync {direction}: {source} -> {target}. '
+                     'Ensure that the network is stable, then retry.')
+        subprocess_utils.handle_returncode(returncode,
+                                           command,
+                                           error_msg,
+                                           stderr=stderr,
+                                           stream_logs=stream_logs)
```

### Comparing `skypilot-0.2.5/sky/utils/common_utils.py` & `skypilot-0.3.0/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/utils/db_utils.py` & `skypilot-0.3.0/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/utils/env_options.py` & `skypilot-0.3.0/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/utils/log_utils.py` & `skypilot-0.3.0/sky/utils/log_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Logging utils."""
 import enum
 import threading
-from typing import List, Optional
+from typing import Optional, List
 
 import rich.console as rich_console
 
 import colorama
 import pendulum
 import prettytable
 
@@ -141,14 +141,20 @@
             diff = '< 1 second'
         diff = diff.replace(' seconds', 's')
         diff = diff.replace(' second', 's')
         diff = diff.replace(' minutes', 'm')
         diff = diff.replace(' minute', 'm')
         diff = diff.replace(' hours', 'h')
         diff = diff.replace(' hour', 'h')
+        diff = diff.replace(' days', 'd')
+        diff = diff.replace(' day', 'd')
+        diff = diff.replace(' weeks', 'w')
+        diff = diff.replace(' week', 'w')
+        diff = diff.replace(' months', 'mo')
+        diff = diff.replace(' month', 'mo')
     else:
         diff = start_time.diff_for_humans(end)
         if duration.in_seconds() < 1:
             diff = '< 1 second'
         diff = diff.replace('second', 'sec')
         diff = diff.replace('minute', 'min')
         diff = diff.replace('hour', 'hr')
```

### Comparing `skypilot-0.2.5/sky/utils/schemas.py` & `skypilot-0.3.0/sky/utils/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,17 @@
             },
             'spot_recovery': {
                 'type': 'string',
             },
             'disk_size': {
                 'type': 'integer',
             },
+            'disk_tier': {
+                'type': 'string',
+            },
             'accelerator_args': {
                 'type': 'object',
                 'required': [],
                 'additionalProperties': False,
                 'properties': {
                     'runtime_version': {
                         'type': 'string',
```

### Comparing `skypilot-0.2.5/sky/utils/subprocess_utils.py` & `skypilot-0.3.0/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/utils/timeline.py` & `skypilot-0.3.0/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/utils/tpu_utils.py` & `skypilot-0.3.0/sky/utils/tpu_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/sky/utils/validator.py` & `skypilot-0.3.0/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/skypilot.egg-info/PKG-INFO` & `skypilot-0.3.0/skypilot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: skypilot
-Version: 0.2.5
+Version: 0.3.0
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
 Description-Content-Type: text/markdown
 Provides-Extra: aws
 Provides-Extra: azure
 Provides-Extra: gcp
+Provides-Extra: ibm
 Provides-Extra: docker
 Provides-Extra: lambda
+Provides-Extra: cloudflare
 Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
   <img alt="SkyPilot" src="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/skypilot-wide-light-1k.png" width=55%>
 </p>
 
@@ -46,14 +47,21 @@
 </p>
 
 
 <h3 align="center">
     Run jobs on any cloud, easily and cost effectively
 </h3>
 
+----
+:fire: :dromedary_camel: *News* :dromedary_camel: :fire: 
+- [April, 2023] **[**SkyPilot YAMLs released**](./llm/vicuna/) for finetuning & serving the Vicuna model with a single command**!
+- [March, 2023] **[Vicuna LLM chatbot](https://lmsys.org/blog/2023-03-30-vicuna/) trained** [**using SkyPilot**](./llm/vicuna/) **for $300 on spot instances!** 
+- [March, 2023] *Serve* your own LLaMA LLM chatbot (not finetuned) on any cloud: [**example**](./llm/llama-chatbots/), [**repo**](https://github.com/skypilot-org/sky-llama)
+----
+
 SkyPilot is a framework for easily and cost effectively running ML workloads<sup>[1]</sup> on any cloud. 
 
 SkyPilot abstracts away the cloud infra burden:
 - Launch jobs & clusters on any cloud (AWS, Azure, GCP, Lambda Cloud)
 - Find scarce resources across zones/regions/clouds
 - Queue jobs & use cloud object stores
 
@@ -135,15 +143,17 @@
 - [Documentation](https://skypilot.readthedocs.io/en/latest/)
 - [Example: HuggingFace](https://skypilot.readthedocs.io/en/latest/getting-started/tutorial.html) 
 - [Tutorials](https://github.com/skypilot-org/skypilot-tutorial) 
 - [YAML reference](https://skypilot.readthedocs.io/en/latest/reference/yaml-spec.html)
 - Framework examples: [PyTorch DDP](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_torch.yaml),  [Distributed](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_tf_app.py) [TensorFlow](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_app_storage.yaml), [JAX/Flax on TPU](https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/tree/master/examples/stable_diffusion), [Detectron2](https://github.com/skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml), [programmatic grid search](https://github.com/skypilot-org/skypilot/blob/master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml), and [many more](./examples).
 
 More information:
-- [Introductory blog post](https://medium.com/@zongheng_yang/skypilot-ml-and-data-science-on-any-cloud-with-massive-cost-savings-244189cc7c0f)
+- [SkyPilot Blog](https://blog.skypilot.co/)
+  - [Introductory blog post](https://blog.skypilot.co/introducing-skypilot/)
+- [NSDI 2023 paper & talk](https://www.usenix.org/conference/nsdi23/presentation/yang-zongheng)
 
 ## Issues, feature requests, and questions
 We are excited to hear your feedback! 
 * For issues and feature requests, please [open a GitHub issue](https://github.com/skypilot-org/skypilot/issues/new).
 * For questions, please use [GitHub Discussions](https://github.com/skypilot-org/skypilot/discussions).
 
 For general discussions, join us on the [SkyPilot Slack](http://slack.skypilot.co).
```

#### html2text {}

```diff
@@ -1,31 +1,38 @@
-Metadata-Version: 2.1 Name: skypilot Version: 0.2.5 Summary: SkyPilot: An
+Metadata-Version: 2.1 Name: skypilot Version: 0.3.0 Summary: SkyPilot: An
 intercloud broker for the clouds Author: SkyPilot Team License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot Project-URL:
 Issues, https://github.com/skypilot-org/skypilot/issues Project-URL:
 Discussion, https://github.com/skypilot-org/skypilot/discussions Project-URL:
 Documentation, https://skypilot.readthedocs.io/en/latest/ Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: System ::
-Distributed Computing Description-Content-Type: text/markdown Provides-Extra:
-aws Provides-Extra: azure Provides-Extra: gcp Provides-Extra: docker Provides-
-Extra: lambda Provides-Extra: all License-File: LICENSE
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Distributed Computing Description-Content-Type:
+text/markdown Provides-Extra: aws Provides-Extra: azure Provides-Extra: gcp
+Provides-Extra: ibm Provides-Extra: docker Provides-Extra: lambda Provides-
+Extra: cloudflare Provides-Extra: all License-File: LICENSE
                                   [SkyPilot]
                  [Documentation] [GitHub_Release] [Join_Slack]
          **** Run jobs on any cloud, easily and cost effectively ****
-SkyPilot is a framework for easily and cost effectively running ML workloads[1]
-on any cloud. SkyPilot abstracts away the cloud infra burden: - Launch jobs &
-clusters on any cloud (AWS, Azure, GCP, Lambda Cloud) - Find scarce resources
-across zones/regions/clouds - Queue jobs & use cloud object stores SkyPilot
-cuts your cloud costs: * [Managed Spot](https://skypilot.readthedocs.io/en/
-latest/examples/spot-jobs.html): **3x cost savings** using spot VMs, with auto-
+---- :fire: :dromedary_camel: *News* :dromedary_camel: :fire: - [April, 2023]
+**[**SkyPilot YAMLs released**](./llm/vicuna/) for finetuning & serving the
+Vicuna model with a single command**! - [March, 2023] **[Vicuna LLM chatbot]
+(https://lmsys.org/blog/2023-03-30-vicuna/) trained** [**using SkyPilot**](./
+llm/vicuna/) **for $300 on spot instances!** - [March, 2023] *Serve* your own
+LLaMA LLM chatbot (not finetuned) on any cloud: [**example**](./llm/llama-
+chatbots/), [**repo**](https://github.com/skypilot-org/sky-llama) ---- SkyPilot
+is a framework for easily and cost effectively running ML workloads[1] on any
+cloud. SkyPilot abstracts away the cloud infra burden: - Launch jobs & clusters
+on any cloud (AWS, Azure, GCP, Lambda Cloud) - Find scarce resources across
+zones/regions/clouds - Queue jobs & use cloud object stores SkyPilot cuts your
+cloud costs: * [Managed Spot](https://skypilot.readthedocs.io/en/latest/
+examples/spot-jobs.html): **3x cost savings** using spot VMs, with auto-
 recovery from preemptions * [Autostop](https://skypilot.readthedocs.io/en/
 latest/reference/auto-stop.html): hands-free cleanup of idle clusters *
 [Benchmark](https://skypilot.readthedocs.io/en/latest/reference/benchmark/
 index.html): find best VM types for your jobs * Optimizer: **2x cost savings**
 by auto-picking best prices across zones/regions/clouds SkyPilot supports your
 existing GPU, TPU, and CPU workloads, with no code changes. Install with pip
 (choose your clouds) or [from source](https://skypilot.readthedocs.io/en/
@@ -72,17 +79,18 @@
 (https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/
 tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/
 tree/master/examples/stable_diffusion), [Detectron2](https://github.com/
 skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml),
 [programmatic grid search](https://github.com/skypilot-org/skypilot/blob/
 master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://
 github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml),
-and [many more](./examples). More information: - [Introductory blog post]
-(https://medium.com/@zongheng_yang/skypilot-ml-and-data-science-on-any-cloud-
-with-massive-cost-savings-244189cc7c0f) ## Issues, feature requests, and
+and [many more](./examples). More information: - [SkyPilot Blog](https://
+blog.skypilot.co/) - [Introductory blog post](https://blog.skypilot.co/
+introducing-skypilot/) - [NSDI 2023 paper & talk](https://www.usenix.org/
+conference/nsdi23/presentation/yang-zongheng) ## Issues, feature requests, and
 questions We are excited to hear your feedback! * For issues and feature
 requests, please [open a GitHub issue](https://github.com/skypilot-org/
 skypilot/issues/new). * For questions, please use [GitHub Discussions](https://
 github.com/skypilot-org/skypilot/discussions). For general discussions, join us
 on the [SkyPilot Slack](http://slack.skypilot.co). ## Contributing We welcome
 and value all contributions to the project! Please refer to [CONTRIBUTING]
 (CONTRIBUTING.md) for how to get involved. # [1]: While SkyPilot is currently
```

### Comparing `skypilot-0.2.5/skypilot.egg-info/SOURCES.txt` & `skypilot-0.3.0/skypilot.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 pyproject.toml
 setup.py
 sky/__init__.py
 sky/authentication.py
 sky/check.py
 sky/cli.py
 sky/cloud_stores.py
+sky/config.py
 sky/core.py
 sky/dag.py
 sky/exceptions.py
 sky/execution.py
 sky/global_user_state.py
 sky/optimizer.py
 sky/resources.py
 sky/sky_logging.py
 sky/skypilot_config.py
 sky/task.py
 sky/adaptors/__init__.py
 sky/adaptors/aws.py
 sky/adaptors/azure.py
+sky/adaptors/cloudflare.py
 sky/adaptors/docker.py
 sky/adaptors/gcp.py
+sky/adaptors/ibm.py
 sky/backends/__init__.py
 sky/backends/backend.py
 sky/backends/backend_utils.py
 sky/backends/cloud_vm_ray_backend.py
 sky/backends/docker_utils.py
 sky/backends/local_docker_backend.py
 sky/backends/onprem_utils.py
@@ -36,38 +39,40 @@
 sky/benchmark/benchmark_state.py
 sky/benchmark/benchmark_utils.py
 sky/clouds/__init__.py
 sky/clouds/aws.py
 sky/clouds/azure.py
 sky/clouds/cloud.py
 sky/clouds/gcp.py
+sky/clouds/ibm.py
 sky/clouds/lambda_cloud.py
 sky/clouds/local.py
 sky/clouds/service_catalog/__init__.py
 sky/clouds/service_catalog/aws_catalog.py
 sky/clouds/service_catalog/azure_catalog.py
 sky/clouds/service_catalog/common.py
 sky/clouds/service_catalog/config.py
 sky/clouds/service_catalog/constants.py
 sky/clouds/service_catalog/gcp_catalog.py
+sky/clouds/service_catalog/ibm_catalog.py
 sky/clouds/service_catalog/lambda_catalog.py
 sky/clouds/service_catalog/data_fetchers/__init__.py
 sky/clouds/service_catalog/data_fetchers/fetch_aws.py
 sky/clouds/service_catalog/data_fetchers/fetch_azure.py
 sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
 sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
 sky/data/__init__.py
 sky/data/data_transfer.py
 sky/data/data_utils.py
 sky/data/mounting_utils.py
 sky/data/storage.py
 sky/data/storage_utils.py
 sky/setup_files/MANIFEST.in
 sky/setup_files/setup.py
-sky/skylet/LICENCE
+sky/skylet/LICENSE
 sky/skylet/__init__.py
 sky/skylet/autostop_lib.py
 sky/skylet/configs.py
 sky/skylet/constants.py
 sky/skylet/events.py
 sky/skylet/job_lib.py
 sky/skylet/log_lib.py
@@ -85,23 +90,25 @@
 sky/skylet/providers/azure/config.py
 sky/skylet/providers/azure/node_provider.py
 sky/skylet/providers/gcp/__init__.py
 sky/skylet/providers/gcp/config.py
 sky/skylet/providers/gcp/constants.py
 sky/skylet/providers/gcp/node.py
 sky/skylet/providers/gcp/node_provider.py
+sky/skylet/providers/ibm/__init__.py
+sky/skylet/providers/ibm/node_provider.py
+sky/skylet/providers/ibm/utils.py
+sky/skylet/providers/ibm/vpc_provider.py
 sky/skylet/providers/lambda_cloud/__init__.py
 sky/skylet/providers/lambda_cloud/lambda_utils.py
 sky/skylet/providers/lambda_cloud/node_provider.py
 sky/skylet/ray_patches/__init__.py
 sky/skylet/ray_patches/autoscaler.py.patch
-sky/skylet/ray_patches/azure_cli.py.patch
 sky/skylet/ray_patches/cli.py.patch
 sky/skylet/ray_patches/command_runner.py.patch
-sky/skylet/ray_patches/job_manager.py.patch
 sky/skylet/ray_patches/log_monitor.py.patch
 sky/skylet/ray_patches/resource_demand_scheduler.py.patch
 sky/skylet/ray_patches/updater.py.patch
 sky/skylet/ray_patches/worker.py.patch
 sky/spot/__init__.py
 sky/spot/constants.py
 sky/spot/controller.py
@@ -109,14 +116,15 @@
 sky/spot/spot_state.py
 sky/spot/spot_utils.py
 sky/templates/aws-ray.yml.j2
 sky/templates/azure-ray.yml.j2
 sky/templates/gcp-ray.yml.j2
 sky/templates/gcp-tpu-create.sh.j2
 sky/templates/gcp-tpu-delete.sh.j2
+sky/templates/ibm-ray.yml.j2
 sky/templates/lambda-ray.yml.j2
 sky/templates/local-ray.yml.j2
 sky/templates/spot-controller.yaml.j2
 sky/usage/__init__.py
 sky/usage/constants.py
 sky/usage/usage_lib.py
 sky/utils/__init__.py
@@ -137,14 +145,16 @@
 skypilot.egg-info/PKG-INFO
 skypilot.egg-info/SOURCES.txt
 skypilot.egg-info/dependency_links.txt
 skypilot.egg-info/entry_points.txt
 skypilot.egg-info/requires.txt
 skypilot.egg-info/top_level.txt
 tests/test_cli.py
+tests/test_config.py
+tests/test_file_mount_helper.py
 tests/test_global_user_state.py
 tests/test_list_accelerators.py
 tests/test_onprem.py
 tests/test_optimizer_dryruns.py
 tests/test_optimizer_random_dag.py
 tests/test_pycryptodome_version.py
 tests/test_smoke.py
```

### Comparing `skypilot-0.2.5/tests/test_cli.py` & `skypilot-0.3.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import tempfile
 import textwrap
 
 from click import testing as cli_testing
 
 import sky
-from sky import clouds
 import sky.cli as cli
 
 
 def test_infer_gpunode_type():
     resources = [
         sky.Resources(cloud=sky.AWS(), instance_type='p3.2xlarge'),
         sky.Resources(cloud=sky.GCP(), accelerators='K80'),
```

### Comparing `skypilot-0.2.5/tests/test_list_accelerators.py` & `skypilot-0.3.0/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/tests/test_onprem.py` & `skypilot-0.3.0/tests/test_onprem.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/tests/test_optimizer_dryruns.py` & `skypilot-0.3.0/tests/test_optimizer_dryruns.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,30 +249,30 @@
 
 
 def test_instance_type_from_cpu_memory(monkeypatch, capfd):
     _test_resources_launch(monkeypatch, cpus=8)
     stdout, _ = capfd.readouterr()
     # Choose General Purpose instance types
     assert 'm6i.2xlarge' in stdout  # AWS, 8 vCPUs, 32 GB memory
-    assert 'Standard_D8_v5' in stdout  # Azure, 8 vCPUs, 32 GB memory
+    assert 'Standard_D8s_v5' in stdout  # Azure, 8 vCPUs, 32 GB memory
     assert 'n2-standard-8' in stdout  # GCP, 8 vCPUs, 32 GB memory
 
     _test_resources_launch(monkeypatch, memory=32)
     stdout, _ = capfd.readouterr()
     # Choose memory-optimized instance types, when the memory
     # is specified
     assert 'r6i.xlarge' in stdout  # AWS, 4 vCPUs, 32 GB memory
-    assert 'Standard_E4_v5' in stdout  # Azure, 4 vCPUs, 32 GB memory
+    assert 'Standard_E4s_v5' in stdout  # Azure, 4 vCPUs, 32 GB memory
     assert 'n2-highmem-4' in stdout  # GCP, 4 vCPUs, 32 GB memory
 
     _test_resources_launch(monkeypatch, memory='64+')
     stdout, _ = capfd.readouterr()
     # Choose memory-optimized instance types
     assert 'r6i.2xlarge' in stdout  # AWS, 8 vCPUs, 64 GB memory
-    assert 'Standard_E8_v5' in stdout  # Azure, 8 vCPUs, 64 GB memory
+    assert 'Standard_E8s_v5' in stdout  # Azure, 8 vCPUs, 64 GB memory
     assert 'n2-highmem-8' in stdout  # GCP, 8 vCPUs, 64 GB memory
     assert 'gpu_1x_a6000' in stdout  # Lambda, 14 vCPUs, 100 GB memory
 
     _test_resources_launch(monkeypatch, cpus='4+', memory='4+')
     stdout, _ = capfd.readouterr()
     # Choose compute-optimized instance types, when the memory
     # requirement is less than the memory of General Purpose
@@ -433,15 +433,15 @@
 
     with pytest.raises(ValueError) as e:
         _test_resources(monkeypatch, image_id='ami-0868a20f5a3bf9702')
     assert 'Cloud must be specified' in str(e.value)
 
     with pytest.raises(ValueError) as e:
         _test_resources(monkeypatch, cloud=sky.Azure(), image_id='some-image')
-    assert 'only supported for AWS and GCP' in str(e.value)
+    assert 'only supported for AWS, GCP and IBM' in str(e.value)
 
 
 def test_valid_image(monkeypatch):
     _test_resources(monkeypatch,
                     cloud=sky.AWS(),
                     region='us-east-1',
                     image_id='ami-0868a20f5a3bf9702')
```

### Comparing `skypilot-0.2.5/tests/test_optimizer_random_dag.py` & `skypilot-0.3.0/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/tests/test_smoke.py` & `skypilot-0.3.0/tests/test_smoke.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,25 +28,28 @@
 import subprocess
 import sys
 import tempfile
 import time
 from typing import Dict, List, NamedTuple, Optional, Tuple
 import urllib.parse
 import uuid
+import os
 
 import colorama
 import jinja2
 import pytest
 
 import sky
 from sky import global_user_state
 from sky.data import storage as storage_lib
+from sky.adaptors import cloudflare
 from sky.skylet import events
 from sky.utils import common_utils
 from sky.utils import subprocess_utils
+from sky.clouds import AWS, GCP, Azure
 
 # For uniquefying users on shared-account cloud providers. Used as part of the
 # cluster names.
 _smoke_test_hash = hashlib.md5(
     common_utils.user_and_hostname_hash().encode()).hexdigest()[:4]
 
 # To avoid the second smoke test reusing the cluster launched in the first
@@ -233,14 +236,31 @@
             f'sky status --all | grep {name} | grep us-central1',  # Ensure the region is correct.
         ],
         f'sky down -y {name}',
     )
     run_one_test(test)
 
 
+@pytest.mark.ibm
+def test_ibm_region():
+    name = _get_cluster_name()
+    region = 'eu-de'
+    test = Test(
+        'region',
+        [
+            f'sky launch -y -c {name} --cloud ibm --region {region} examples/minimal.yaml',
+            f'sky exec {name} --cloud ibm examples/minimal.yaml',
+            f'sky logs {name} 1 --status',  # Ensure the job succeeded.
+            f'sky status --all | grep {name} | grep {region}',  # Ensure the region is correct.
+        ],
+        f'sky down -y {name}',
+    )
+    run_one_test(test)
+
+
 @pytest.mark.azure
 def test_azure_region():
     name = _get_cluster_name()
     test = Test(
         'azure_region',
         [
             f'sky launch -y -c {name} --region eastus2 --cloud azure tests/test_yamls/minimal.yaml',
@@ -266,14 +286,31 @@
             f'sky status --all | grep {name} | grep us-west-2b',  # Ensure the zone is correct.
         ],
         f'sky down -y {name}',
     )
     run_one_test(test)
 
 
+@pytest.mark.ibm
+def test_ibm_zone():
+    name = _get_cluster_name()
+    zone = 'eu-de-2'
+    test = Test(
+        'zone',
+        [
+            f'sky launch -y -c {name} --cloud ibm examples/minimal.yaml --zone {zone}',
+            f'sky exec {name} --cloud ibm examples/minimal.yaml --zone {zone}',
+            f'sky logs {name} 1 --status',  # Ensure the job succeeded.
+            f'sky status --all | grep {name} | grep {zone}',  # Ensure the zone is correct.
+        ],
+        f'sky down -y {name} {name}-2 {name}-3',
+    )
+    run_one_test(test)
+
+
 @pytest.mark.gcp
 def test_gcp_zone():
     name = _get_cluster_name()
     test = Test(
         'gcp_zone',
         [
             f'sky launch -y -c {name} --zone us-central1-a --cloud gcp tests/test_yamls/minimal.yaml',
@@ -674,14 +711,43 @@
             test_commands,
             f'sky down -y {name}; sky storage delete {storage_name}',
             timeout=20 * 60,  # 20 mins
         )
         run_one_test(test)
 
 
+@pytest.mark.cloudflare
+def test_cloudflare_storage_mounts(generic_cloud: str):
+    name = _get_cluster_name()
+    storage_name = f'sky-test-{int(time.time())}'
+    template_str = pathlib.Path(
+        'tests/test_yamls/test_r2_storage_mounting.yaml').read_text()
+    template = jinja2.Template(template_str)
+    content = template.render(storage_name=storage_name)
+    endpoint_url = cloudflare.create_endpoint()
+    with tempfile.NamedTemporaryFile(suffix='.yaml', mode='w') as f:
+        f.write(content)
+        f.flush()
+        file_path = f.name
+        test_commands = [
+            *storage_setup_commands,
+            f'sky launch -y -c {name} --cloud {generic_cloud} {file_path}',
+            f'sky logs {name} 1 --status',  # Ensure job succeeded.
+            f'AWS_SHARED_CREDENTIALS_FILE={cloudflare.R2_CREDENTIALS_PATH} aws s3 ls s3://{storage_name}/hello.txt --endpoint {endpoint_url} --profile=r2'
+        ]
+
+        test = Test(
+            'cloudflare_storage_mounts',
+            test_commands,
+            f'sky down -y {name}; sky storage delete {storage_name}',
+            timeout=20 * 60,  # 20 mins
+        )
+        run_one_test(test)
+
+
 # ---------- CLI logs ----------
 def test_cli_logs(generic_cloud: str):
     name = _get_cluster_name()
     timestamp = time.time()
     test = Test(
         'cli_logs',
         [
@@ -698,29 +764,30 @@
         f'sky down -y {name}',
     )
     run_one_test(test)
 
 
 # ---------- Job Queue. ----------
 @pytest.mark.no_lambda_cloud  # Lambda Cloud does not have K80 gpus
+@pytest.mark.no_ibm  # IBM Cloud does not have K80 gpus. run test_ibm_job_queue instead
 def test_job_queue(generic_cloud: str):
     name = _get_cluster_name()
     test = Test(
         'job_queue',
         [
             f'sky launch -y -c {name} --cloud {generic_cloud} examples/job_queue/cluster.yaml',
             f'sky exec {name} -n {name}-1 -d examples/job_queue/job.yaml',
             f'sky exec {name} -n {name}-2 -d examples/job_queue/job.yaml',
             f'sky exec {name} -n {name}-3 -d examples/job_queue/job.yaml',
-            f'sky queue {name} | grep {name}-1 | grep RUNNING',
-            f'sky queue {name} | grep {name}-2 | grep RUNNING',
-            f'sky queue {name} | grep {name}-3 | grep PENDING',
+            f's=$(sky queue {name}); echo "$s"; echo; echo; echo "$s" | grep {name}-1 | grep RUNNING',
+            f's=$(sky queue {name}); echo "$s"; echo; echo; echo "$s" | grep {name}-2 | grep RUNNING',
+            f's=$(sky queue {name}); echo "$s"; echo; echo; echo "$s" | grep {name}-3 | grep PENDING',
             f'sky cancel -y {name} 2',
             'sleep 5',
-            f'sky queue {name} | grep {name}-3 | grep RUNNING',
+            f's=$(sky queue {name}); echo "$s"; echo; echo; echo "$s" | grep {name}-3 | grep RUNNING',
             f'sky cancel -y {name} 3',
             f'sky exec {name} --gpus K80:0.2 "[[ \$SKYPILOT_NUM_GPUS_PER_NODE -eq 1 ]] || exit 1"',
             f'sky exec {name} --gpus K80:1 "[[ \$SKYPILOT_NUM_GPUS_PER_NODE -eq 1 ]] || exit 1"',
             f'sky logs {name} 4 --status',
             f'sky logs {name} 5 --status',
         ],
         f'sky down -y {name}',
@@ -747,15 +814,39 @@
             f'sky cancel -y {name} 3',
         ],
         f'sky down -y {name}',
     )
     run_one_test(test)
 
 
+@pytest.mark.ibm
+def test_ibm_job_queue():
+    name = _get_cluster_name()
+    test = Test(
+        'ibm_job_queue',
+        [
+            f'sky launch -y -c {name} --cloud ibm --gpus v100',
+            f'sky exec {name} -n {name}-1 --cloud ibm -d examples/job_queue/job_ibm.yaml',
+            f'sky exec {name} -n {name}-2 --cloud ibm -d examples/job_queue/job_ibm.yaml',
+            f'sky exec {name} -n {name}-3 --cloud ibm -d examples/job_queue/job_ibm.yaml',
+            f'sky queue {name} | grep {name}-1 | grep RUNNING',
+            f'sky queue {name} | grep {name}-2 | grep RUNNING',
+            f'sky queue {name} | grep {name}-3 | grep PENDING',
+            f'sky cancel -y {name} 2',
+            'sleep 5',
+            f'sky queue {name} | grep {name}-3 | grep RUNNING',
+            f'sky cancel -y {name} 3',
+        ],
+        f'sky down -y {name}',
+    )
+    run_one_test(test)
+
+
 @pytest.mark.no_lambda_cloud  # Lambda Cloud does not have T4 gpus
+@pytest.mark.no_ibm  # IBM Cloud does not have T4 gpus. run test_ibm_job_queue_multinode instead
 def test_job_queue_multinode(generic_cloud: str):
     name = _get_cluster_name()
     test = Test(
         'job_queue_multinode',
         [
             f'sky launch -y -c {name} --cloud {generic_cloud} examples/job_queue/cluster_multinode.yaml',
             f'sky exec {name} -n {name}-1 -d examples/job_queue/job_multinode.yaml',
@@ -764,15 +855,15 @@
             f's=$(sky queue {name}) && echo "$s" && (echo "$s" | grep {name}-1 | grep RUNNING)',
             f's=$(sky queue {name}) && echo "$s" && (echo "$s" | grep {name}-2 | grep RUNNING)',
             f's=$(sky queue {name}) && echo "$s" && (echo "$s" | grep {name}-3 | grep SETTING_UP)',
             'sleep 90',
             f's=$(sky queue {name}) && echo "$s" && (echo "$s" | grep {name}-3 | grep PENDING)',
             f'sky cancel -y {name} 1',
             'sleep 5',
-            f'sky queue {name} | grep {name}-3 | grep RUNNING',
+            f's=$(sky queue {name}); echo "$s"; echo; echo; echo "$s" | grep {name}-3 | grep RUNNING',
             f'sky cancel -y {name} 1 2 3',
             f'sky launch -c {name} -n {name}-4 --detach-setup -d examples/job_queue/job_multinode.yaml',
             # Test the job status is correctly set to SETTING_UP, during the setup is running,
             # and the job can be cancelled during the setup.
             f's=$(sky queue {name}) && echo "$s" && (echo "$s" | grep {name}-4 | grep SETTING_UP)',
             f'sky cancel -y {name} 4',
             f's=$(sky queue {name}) && echo "$s" && (echo "$s" | grep {name}-4 | grep CANCELLED)',
@@ -796,45 +887,85 @@
         [
             f'sky launch -y -c {name} --cloud {generic_cloud}',
             f'for i in `seq 1 75`; do sky exec {name} -d "echo $i; sleep 100000000"; done',
             f'sky cancel -y {name} 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16',
             'sleep 20',
             # Each job takes 0.5 CPU and the default VM has 8 CPUs, so there should be 8 / 0.5 = 16 jobs running.
             # The first 16 jobs are canceled, so there should be 75 - 32 = 43 jobs PENDING.
-            f'sky queue {name} | grep -v grep | grep PENDING | wc -l | grep 43',
+            f's=$(sky queue {name}); echo "$s"; echo; echo; echo "$s" | grep -v grep | grep PENDING | wc -l | grep 43',
         ],
         f'sky down -y {name}',
         timeout=20 * 60,
     )
     run_one_test(test)
 
 
+@pytest.mark.ibm
+def test_ibm_job_queue_multinode():
+    name = _get_cluster_name()
+    task_file = 'examples/job_queue/job_multinode_ibm.yaml'
+    test = Test(
+        'ibm_job_queue_multinode',
+        [
+            f'sky launch -y -c {name} --cloud ibm --gpus v100 --num-nodes 2',
+            f'sky exec {name} -n {name}-1 -d {task_file}',
+            f'sky exec {name} -n {name}-2 -d {task_file}',
+            f'sky launch -y -c {name} -n {name}-3 --detach-setup -d {task_file}',
+            f's=$(sky queue {name}) && printf "$s" && (echo "$s" | grep {name}-1 | grep RUNNING)',
+            f's=$(sky queue {name}) && printf "$s" && (echo "$s" | grep {name}-2 | grep RUNNING)',
+            f's=$(sky queue {name}) && printf "$s" && (echo "$s" | grep {name}-3 | grep SETTING_UP)',
+            'sleep 90',
+            f's=$(sky queue {name}) && printf "$s" && (echo "$s" | grep {name}-3 | grep PENDING)',
+            f'sky cancel -y {name} 1',
+            'sleep 5',
+            f'sky queue {name} | grep {name}-3 | grep RUNNING',
+            f'sky cancel -y {name} 1 2 3',
+            f'sky launch -c {name} -n {name}-4 --detach-setup -d {task_file}',
+            # Test the job status is correctly set to SETTING_UP, during the setup is running,
+            # and the job can be cancelled during the setup.
+            f's=$(sky queue {name}) && printf "$s" && (echo "$s" | grep {name}-4 | grep SETTING_UP)',
+            f'sky cancel -y {name} 4',
+            f's=$(sky queue {name}) && printf "$s" && (echo "$s" | grep {name}-4 | grep CANCELLED)',
+            f'sky exec {name} --gpus v100:0.2 "[[ \$SKYPILOT_NUM_GPUS_PER_NODE -eq 1 ]] || exit 1"',
+            f'sky exec {name} --gpus v100:0.2 --num-nodes 2 "[[ \$SKYPILOT_NUM_GPUS_PER_NODE -eq 1 ]] || exit 1"',
+            f'sky exec {name} --gpus v100:1 --num-nodes 2 "[[ \$SKYPILOT_NUM_GPUS_PER_NODE -eq 1 ]] || exit 1"',
+            f'sky logs {name} 5 --status',
+            f'sky logs {name} 6 --status',
+            f'sky logs {name} 7 --status',
+        ],
+        f'sky down -y {name}',
+    )
+    run_one_test(test)
+
+
 # ---------- Submitting multiple tasks to the same cluster. ----------
 @pytest.mark.no_lambda_cloud  # Lambda Cloud does not have K80 gpus
+@pytest.mark.no_ibm  # IBM Cloud does not have K80 gpus
 def test_multi_echo(generic_cloud: str):
     name = _get_cluster_name()
     test = Test(
         'multi_echo',
         [
             f'python examples/multi_echo.py {name} {generic_cloud}',
-            'sleep 70',
+            'sleep 90',
         ] +
         # Ensure jobs succeeded.
         [f'sky logs {name} {i + 1} --status' for i in range(32)] +
         # Ensure monitor/autoscaler didn't crash on the 'assert not
         # unfulfilled' error.  If process not found, grep->ssh returns 1.
         [f'ssh {name} \'ps aux | grep "[/]"monitor.py\''],
         f'sky down -y {name}',
         timeout=20 * 60,
     )
     run_one_test(test)
 
 
 # ---------- Task: 1 node training. ----------
 @pytest.mark.no_lambda_cloud  # Lambda Cloud does not have V100 gpus
+@pytest.mark.no_ibm  # IBM cloud currently doesn't provide public image with CUDA
 def test_huggingface(generic_cloud: str):
     name = _get_cluster_name()
     test = Test(
         'huggingface_glue_imdb_app',
         [
             f'sky launch -y -c {name} --cloud {generic_cloud} examples/huggingface_glue_imdb_app.yaml',
             f'sky logs {name} 1 --status',  # Ensure the job succeeded.
@@ -936,14 +1067,15 @@
         f'sky down -y {name}',
     )
     run_one_test(test)
 
 
 # ---------- Task: n=2 nodes with setups. ----------
 @pytest.mark.no_lambda_cloud  # Lambda Cloud does not have V100 gpus
+@pytest.mark.no_ibm  # IBM cloud currently doesn't provide public image with CUDA
 def test_distributed_tf(generic_cloud: str):
     name = _get_cluster_name()
     test = Test(
         'resnet_distributed_tf_app',
         [
             # NOTE: running it twice will hang (sometimes?) - an app-level bug.
             f'python examples/resnet_distributed_tf_app.py {name} {generic_cloud}',
@@ -1000,14 +1132,15 @@
         timeout=30 * 60,  # 30 mins
     )
     run_one_test(test)
 
 
 # ---------- Testing Autostopping ----------
 @pytest.mark.no_lambda_cloud  # Lambda Cloud does not support stopping instances
+@pytest.mark.no_ibm  # FIX(IBM) sporadically fails, as restarted workers stay uninitialized indefinitely
 def test_autostop(generic_cloud: str):
     name = _get_cluster_name()
     test = Test(
         'autostop',
         [
             f'sky launch -y -d -c {name} --num-nodes 2 --cloud {generic_cloud} tests/test_yamls/minimal.yaml',
             f'sky autostop -y {name} -i 1',
@@ -1133,14 +1266,15 @@
 def test_cancel_azure():
     name = _get_cluster_name()
     test = _get_cancel_task_with_cloud(name, 'azure', timeout=30 * 60)
     run_one_test(test)
 
 
 @pytest.mark.no_lambda_cloud  # Lambda Cloud does not have V100 gpus
+@pytest.mark.no_ibm  # IBM cloud currently doesn't provide public image with CUDA
 def test_cancel_pytorch(generic_cloud: str):
     name = _get_cluster_name()
     test = Test(
         'cancel-pytorch',
         [
             f'sky launch -c {name} --cloud {generic_cloud} examples/resnet_distributed_torch.yaml -y -d',
             # Wait the GPU process to start.
@@ -1151,20 +1285,43 @@
             'sleep 60',
             f'sky exec {name} "(nvidia-smi | grep \'No running process\') || '
             # Ensure Xorg is the only process running.
             '[ \$(nvidia-smi | grep -A 10 Processes | grep -A 10 === | grep -v Xorg) -eq 2 ]"',
             f'sky logs {name} 3 --status',  # Ensure the job succeeded.
         ],
         f'sky down -y {name}',
+        timeout=20 * 60,
+    )
+    run_one_test(test)
+
+
+# can't use `_get_cancel_task_with_cloud()`, as command `nvidia-smi`
+# requires a CUDA public image, which IBM doesn't offer
+@pytest.mark.ibm
+def test_cancel_ibm():
+    name = _get_cluster_name()
+    test = Test(
+        'ibm-cancel-task',
+        [
+            f'sky launch -y -c {name} --cloud ibm examples/minimal.yaml',
+            f'sky exec {name} -n {name}-1 -d  "while true; do echo \'Hello SkyPilot\'; sleep 2; done"',
+            'sleep 20',
+            f'sky queue {name} | grep {name}-1 | grep RUNNING',
+            f'sky cancel -y {name} 2',
+            f'sleep 5',
+            f'sky queue {name} | grep {name}-1 | grep CANCELLED',
+        ],
+        f'sky down -y {name}',
     )
     run_one_test(test)
 
 
 # ---------- Testing use-spot option ----------
 @pytest.mark.no_lambda_cloud  # Lambda Cloud does not support spot instances
+@pytest.mark.no_ibm  # IBM Cloud does not support spot instances
 def test_use_spot(generic_cloud: str):
     """Test use-spot and sky exec."""
     name = _get_cluster_name()
     test = Test(
         'use-spot',
         [
             f'sky launch -c {name} --cloud {generic_cloud} tests/test_yamls/minimal.yaml --use-spot -y',
@@ -1175,14 +1332,15 @@
         f'sky down -y {name}',
     )
     run_one_test(test)
 
 
 # ---------- Testing managed spot ----------
 @pytest.mark.no_lambda_cloud  # Lambda Cloud does not support spot instances
+@pytest.mark.no_ibm  # IBM Cloud does not support spot instances
 @pytest.mark.managed_spot
 def test_spot(generic_cloud: str):
     """Test the spot yaml."""
     name = _get_cluster_name()
     test = Test(
         'managed-spot',
         [
@@ -1190,55 +1348,56 @@
             f'sky spot launch -n {name}-2 --cloud {generic_cloud} examples/managed_spot.yaml -y -d',
             'sleep 5',
             f'{_SPOT_QUEUE_WAIT}| grep {name}-1 | head -n1 | grep "STARTING\|RUNNING"',
             f'{_SPOT_QUEUE_WAIT}| grep {name}-2 | head -n1 | grep "STARTING\|RUNNING"',
             _SPOT_CANCEL_WAIT.format(job_name=f'{name}-1'),
             'sleep 5',
             f'{_SPOT_QUEUE_WAIT}| grep {name}-1 | head -n1 | grep "CANCELLING\|CANCELLED"',
-            'sleep 120',
+            'sleep 200',
             f'{_SPOT_QUEUE_WAIT}| grep {name}-1 | head -n1 | grep CANCELLED',
             f'{_SPOT_QUEUE_WAIT}| grep {name}-2 | head -n1 | grep "RUNNING\|SUCCEEDED"',
         ],
         # TODO(zhwu): Change to _SPOT_CANCEL_WAIT.format(job_name=f'{name}-1 -n {name}-2') when
         # canceling multiple job names is supported.
         (_SPOT_CANCEL_WAIT.format(job_name=f'{name}-1') + '; ' +
          _SPOT_CANCEL_WAIT.format(job_name=f'{name}-2')),
         # Increase timeout since sky spot queue -r can be blocked by other spot tests.
         timeout=20 * 60,
     )
     run_one_test(test)
 
 
 @pytest.mark.no_lambda_cloud  # Lambda Cloud does not support spot instances
+@pytest.mark.no_ibm  # IBM Cloud does not support spot instances
 @pytest.mark.managed_spot
 def test_spot_failed_setup(generic_cloud: str):
     """Test managed spot job with failed setup."""
     name = _get_cluster_name()
     test = Test(
         'spot-failed-setup',
         [
             f'sky spot launch -n {name} --cloud {generic_cloud} -y -d tests/test_yamls/failed_setup.yaml',
-            'sleep 300',
+            'sleep 330',
             # Make sure the job failed quickly.
             f'{_SPOT_QUEUE_WAIT} | grep {name} | head -n1 | grep "FAILED_SETUP"',
         ],
         _SPOT_CANCEL_WAIT.format(job_name=name),
         # Increase timeout since sky spot queue -r can be blocked by other spot tests.
         timeout=20 * 60,
     )
     run_one_test(test)
 
 
 # ---------- Testing managed spot recovery ----------
 @pytest.mark.aws
 @pytest.mark.managed_spot
-def test_spot_recovery_aws():
+def test_spot_recovery_aws(aws_config_region):
     """Test managed spot recovery."""
     name = _get_cluster_name()
-    region = 'us-west-2'
+    region = aws_config_region
     test = Test(
         'spot_recovery_aws',
         [
             f'sky spot launch --cloud aws --region {region} -n {name} "echo SKYPILOT_JOB_ID: \$SKYPILOT_JOB_ID; sleep 1800"  -y -d',
             'sleep 360',
             f'{_SPOT_QUEUE_WAIT}| grep {name} | head -n1 | grep "RUNNING"',
             f'RUN_ID=$(sky spot logs -n {name} --no-follow | grep SKYPILOT_JOB_ID | cut -d: -f2); echo "$RUN_ID" | tee /tmp/{name}-run-id',
@@ -1289,14 +1448,15 @@
         _SPOT_CANCEL_WAIT.format(job_name=name),
         timeout=25 * 60,
     )
     run_one_test(test)
 
 
 @pytest.mark.no_lambda_cloud  # Lambda Cloud does not support spot instances
+@pytest.mark.no_ibm  # IBM Cloud does not support spot instances
 @pytest.mark.managed_spot
 def test_spot_recovery_default_resources(generic_cloud: str):
     """Test managed spot recovery for default resources."""
     name = _get_cluster_name()
     test = Test(
         'managed-spot-recovery-default-resources',
         [
@@ -1308,18 +1468,18 @@
         timeout=25 * 60,
     )
     run_one_test(test)
 
 
 @pytest.mark.aws
 @pytest.mark.managed_spot
-def test_spot_recovery_multi_node_aws():
+def test_spot_recovery_multi_node_aws(aws_config_region):
     """Test managed spot recovery."""
     name = _get_cluster_name()
-    region = 'us-west-2'
+    region = aws_config_region
     test = Test(
         'spot_recovery_multi_node_aws',
         [
             f'sky spot launch --cloud aws --region {region} -n {name} --num-nodes 2 "echo SKYPILOT_JOB_ID: \$SKYPILOT_JOB_ID; sleep 1800"  -y -d',
             'sleep 450',
             f'{_SPOT_QUEUE_WAIT}| grep {name} | head -n1 | grep "RUNNING"',
             f'RUN_ID=$(sky spot logs -n {name} --no-follow | grep SKYPILOT_JOB_ID | cut -d: -f2); echo "$RUN_ID" | tee /tmp/{name}-run-id',
@@ -1333,15 +1493,15 @@
             'sleep 50',
             f'{_SPOT_QUEUE_WAIT}| grep {name} | head -n1 | grep "RECOVERING"',
             'sleep 560',
             f'{_SPOT_QUEUE_WAIT}| grep {name} | head -n1 | grep "RUNNING"',
             f'RUN_ID=$(cat /tmp/{name}-run-id); echo $RUN_ID; sky spot logs -n {name} --no-follow | grep SKYPILOT_JOB_ID | cut -d: -f2 | grep "$RUN_ID"',
         ],
         _SPOT_CANCEL_WAIT.format(job_name=name),
-        timeout=25 * 60,
+        timeout=30 * 60,
     )
     run_one_test(test)
 
 
 @pytest.mark.gcp
 @pytest.mark.managed_spot
 def test_spot_recovery_multi_node_gcp():
@@ -1374,17 +1534,17 @@
         timeout=25 * 60,
     )
     run_one_test(test)
 
 
 @pytest.mark.aws
 @pytest.mark.managed_spot
-def test_spot_cancellation_aws():
+def test_spot_cancellation_aws(aws_config_region):
     name = _get_cluster_name()
-    region = 'us-east-2'
+    region = aws_config_region
     test = Test(
         'spot_cancellation_aws',
         [
             # Test cancellation during spot cluster being launched.
             f'sky spot launch --cloud aws --region {region} -n {name} "sleep 1000"  -y -d',
             'sleep 60',
             f'{_SPOT_QUEUE_WAIT}| grep {name} | head -n1 | grep "STARTING"',
@@ -1417,15 +1577,15 @@
             f'{_SPOT_QUEUE_WAIT}| grep {name}-3 | head -n1 | grep "RUNNING"',
             # Terminate the cluster manually.
             (f'aws ec2 terminate-instances --region {region} --instance-ids $('
              f'aws ec2 describe-instances --region {region} '
              f'--filters Name=tag:ray-cluster-name,Values={name}-3-* '
              f'--query Reservations[].Instances[].InstanceId '
              '--output text)'),
-            'sleep 100',
+            'sleep 120',
             f'{_SPOT_QUEUE_WAIT}| grep {name}-3 | head -n1 | grep "RECOVERING"',
             _SPOT_CANCEL_WAIT.format(job_name=f'{name}-3'),
             'sleep 5',
             f'{_SPOT_QUEUE_WAIT}| grep {name}-3 | head -n1 | grep "CANCELLING\|CANCELLED"',
             'sleep 120',
             f'{_SPOT_QUEUE_WAIT}| grep {name}-3 | head -n1 | grep "CANCELLED"',
             # The cluster should be terminated (shutting-down) after cancellation. We don't use the `=` operator here because
@@ -1493,14 +1653,15 @@
         ],
         timeout=25 * 60)
     run_one_test(test)
 
 
 # ---------- Testing storage for managed spot ----------
 @pytest.mark.no_lambda_cloud  # Lambda Cloud does not support spot instances
+@pytest.mark.no_ibm  # IBM Cloud does not support spot instances
 @pytest.mark.managed_spot
 def test_spot_storage(generic_cloud: str):
     """Test storage with managed spot"""
     name = _get_cluster_name()
     yaml_str = pathlib.Path(
         'examples/managed_spot_with_storage.yaml').read_text()
     storage_name = f'sky-test-{int(time.time())}'
@@ -1545,14 +1706,15 @@
         timeout=20 * 60,
     )
     run_one_test(test)
 
 
 # ---------- Testing env for spot ----------
 @pytest.mark.no_lambda_cloud  # Lambda Cloud does not support spot instances
+@pytest.mark.no_ibm  # IBM Cloud does not support spot instances
 @pytest.mark.managed_spot
 def test_spot_inline_env(generic_cloud: str):
     """Test spot env"""
     name = _get_cluster_name()
     test = Test(
         'test-spot-inline-env',
         [
@@ -1617,27 +1779,177 @@
         ],
         f'sky down -y {name}',
         timeout=30 * 60,  # 30 mins  (it takes around ~23 mins)
     )
     run_one_test(test)
 
 
+# ---------- Testing env for disk tier ----------
+def test_aws_disk_tier():
+
+    def _get_aws_query_command(region, instance_id, field, expected):
+        return (f'aws ec2 describe-volumes --region {region} '
+                f'--filters Name=attachment.instance-id,Values={instance_id} '
+                f'--query Volumes[*].{field} | grep {expected} ; ')
+
+    for disk_tier in ['low', 'medium', 'high']:
+        specs = AWS._get_disk_specs(disk_tier)
+        name = _get_cluster_name() + '-' + disk_tier
+        region = 'us-west-2'
+        test = Test(
+            'aws-disk-tier',
+            [
+                f'sky launch -y -c {name} --cloud aws --region {region} '
+                f'--disk-tier {disk_tier} echo "hello sky"',
+                f'id=`aws ec2 describe-instances --region {region} --filters '
+                f'Name=tag:ray-cluster-name,Values={name} --query '
+                f'Reservations[].Instances[].InstanceId --output text`; ' +
+                _get_aws_query_command(region, '$id', 'VolumeType',
+                                       specs['disk_tier']) +
+                ('' if disk_tier == 'low' else
+                 (_get_aws_query_command(region, '$id', 'Iops',
+                                         specs['disk_iops']) +
+                  _get_aws_query_command(region, '$id', 'Throughput',
+                                         specs['disk_throughput']))),
+            ],
+            f'sky down -y {name}',
+            timeout=10 * 60,  # 10 mins  (it takes around ~6 mins)
+        )
+        run_one_test(test)
+
+
+def test_gcp_disk_tier():
+    for disk_tier in ['low', 'medium', 'high']:
+        type = GCP._get_disk_type(disk_tier)
+        name = _get_cluster_name() + '-' + disk_tier
+        region = 'us-west2'
+        test = Test(
+            'gcp-disk-tier',
+            [
+                f'sky launch -y -c {name} --cloud gcp --region {region} '
+                f'--disk-tier {disk_tier} echo "hello sky"',
+                f'name=`gcloud compute instances list --filter='
+                f'"labels.ray-cluster-name:{name}" --format="value(name)"`; '
+                f'gcloud compute disks list --filter="name=$name" '
+                f'--format="value(type)" | grep {type} '
+            ],
+            f'sky down -y {name}',
+            timeout=6 * 60,  # 6 mins  (it takes around ~3 mins)
+        )
+        run_one_test(test)
+
+
+def test_azure_disk_tier():
+    for disk_tier in ['low', 'medium']:
+        type = Azure._get_disk_type(disk_tier)
+        name = _get_cluster_name() + '-' + disk_tier
+        region = 'westus2'
+        test = Test(
+            'azure-disk-tier',
+            [
+                f'sky launch -y -c {name} --cloud azure --region {region} '
+                f'--disk-tier {disk_tier} echo "hello sky"',
+                f'az resource list --tag ray-cluster-name={name} --query '
+                f'"[?type==\'Microsoft.Compute/disks\'].sku.name" '
+                f'--output tsv | grep {type}'
+            ],
+            f'sky down -y {name}',
+            timeout=20 * 60,  # 20 mins  (it takes around ~12 mins)
+        )
+        run_one_test(test)
+
+
 # ------- Testing the core API --------
 # Most of the core APIs have been tested in the CLI tests.
 # These tests are for testing the return value of the APIs not fully used in CLI.
 def test_core_api():
     name = _get_cluster_name()
     sky.launch
     # TODO(zhwu): Add a test for core api.
 
 
 # ---------- Testing Storage ----------
 class TestStorageWithCredentials:
     """Storage tests which require credentials and network connection"""
 
+    AWS_INVALID_NAMES = [
+        'ab',  # less than 3 characters
+        'abcdefghijklmnopqrstuvwxyzabcdefghijklmnopqrstuvwxyzabcdefghijklmnopqrstuvwxyz1',
+        # more than 63 characters
+        'Abcdef',  # contains an uppercase letter
+        'abc def',  # contains a space
+        'abc..def',  # two adjacent periods
+        '192.168.5.4',  # formatted as an IP address
+        'xn--bucket',  # starts with 'xn--' prefix
+        'bucket-s3alias',  # ends with '-s3alias' suffix
+        'bucket--ol-s3',  # ends with '--ol-s3' suffix
+        '.abc',  # starts with a dot
+        'abc.',  # ends with a dot
+        '-abc',  # starts with a hyphen
+        'abc-',  # ends with a hyphen
+    ]
+
+    GCS_INVALID_NAMES = [
+        'ab',  # less than 3 characters
+        'abcdefghijklmnopqrstuvwxyzabcdefghijklmnopqrstuvwxyzabcdefghijklmnopqrstuvwxyz1',
+        # more than 63 characters (without dots)
+        'Abcdef',  # contains an uppercase letter
+        'abc def',  # contains a space
+        'abc..def',  # two adjacent periods
+        'abc_.def.ghi.jklmnopqrstuvwxyzabcdefghijklmnopqrstuvwxyzabcdefghijklmnopqrstuvwxyz1'
+        # More than 63 characters between dots
+        'abc_.def.ghi.jklmnopqrstuvwxyzabcdefghijklmnopqfghijklmnopqrstuvw' * 5,
+        # more than 222 characters (with dots)
+        '192.168.5.4',  # formatted as an IP address
+        'googbucket',  # starts with 'goog' prefix
+        'googlebucket',  # contains 'google'
+        'g00glebucket',  # variant of 'google'
+        'go0glebucket',  # variant of 'google'
+        'g0oglebucket',  # variant of 'google'
+        '.abc',  # starts with a dot
+        'abc.',  # ends with a dot
+        '_abc',  # starts with an underscore
+        'abc_',  # ends with an underscore
+    ]
+
+    @staticmethod
+    def cli_delete_cmd(store_type, bucket_name):
+        if store_type == storage_lib.StoreType.S3:
+            url = f's3://{bucket_name}'
+            return f'aws s3 rb {url} --force'
+        if store_type == storage_lib.StoreType.GCS:
+            url = f'gs://{bucket_name}'
+            return f'gsutil -m rm -r {url}'
+        if store_type == storage_lib.StoreType.R2:
+            endpoint_url = cloudflare.create_endpoint()
+            url = f's3://{bucket_name}'
+            return f'AWS_SHARED_CREDENTIALS_FILE={cloudflare.R2_CREDENTIALS_PATH} aws s3 rb {url} --force --endpoint {endpoint_url} --profile=r2'
+
+    @staticmethod
+    def cli_ls_cmd(store_type, bucket_name, suffix=''):
+        if store_type == storage_lib.StoreType.S3:
+            if suffix:
+                url = f's3://{bucket_name}/{suffix}'
+            else:
+                url = f's3://{bucket_name}'
+            return f'aws s3 ls {url}'
+        if store_type == storage_lib.StoreType.GCS:
+            if suffix:
+                url = f'gs://{bucket_name}/{suffix}'
+            else:
+                url = f'gs://{bucket_name}'
+            return f'gsutil ls {url}'
+        if store_type == storage_lib.StoreType.R2:
+            endpoint_url = cloudflare.create_endpoint()
+            if suffix:
+                url = f's3://{bucket_name}/{suffix}'
+            else:
+                url = f's3://{bucket_name}'
+            return f'AWS_SHARED_CREDENTIALS_FILE={cloudflare.R2_CREDENTIALS_PATH} aws s3 ls {url} --endpoint {endpoint_url} --profile=r2'
+
     @pytest.fixture
     def tmp_source(self, tmp_path):
         # Creates a temporary directory with a file in it
         tmp_dir = tmp_path / 'tmp-source'
         tmp_dir.mkdir()
         tmp_file = tmp_dir / 'tmp-file'
         tmp_file.write_text('test')
@@ -1722,23 +2034,37 @@
     def tmp_gsutil_bucket(self, tmp_bucket_name):
         # Creates a temporary bucket using gsutil
         subprocess.check_call(['gsutil', 'mb', f'gs://{tmp_bucket_name}'])
         yield tmp_bucket_name
         subprocess.check_call(['gsutil', 'rm', '-r', f'gs://{tmp_bucket_name}'])
 
     @pytest.fixture
+    def tmp_awscli_bucket_r2(self, tmp_bucket_name):
+        # Creates a temporary bucket using awscli
+        endpoint_url = cloudflare.create_endpoint()
+        subprocess.check_call(
+            f'AWS_SHARED_CREDENTIALS_FILE={cloudflare.R2_CREDENTIALS_PATH} aws s3 mb s3://{tmp_bucket_name} --endpoint {endpoint_url} --profile=r2',
+            shell=True)
+        yield tmp_bucket_name
+        subprocess.check_call(
+            f'AWS_SHARED_CREDENTIALS_FILE={cloudflare.R2_CREDENTIALS_PATH} aws s3 rb s3://{tmp_bucket_name} --force --endpoint {endpoint_url} --profile=r2',
+            shell=True)
+
+    @pytest.fixture
     def tmp_public_storage_obj(self, request):
         # Initializes a storage object with a public bucket
         storage_obj = storage_lib.Storage(source=request.param)
         yield storage_obj
         # This does not require any deletion logic because it is a public bucket
         # and should not get added to global_user_state.
 
-    @pytest.mark.parametrize(
-        'store_type', [storage_lib.StoreType.S3, storage_lib.StoreType.GCS])
+    @pytest.mark.parametrize('store_type', [
+        storage_lib.StoreType.S3, storage_lib.StoreType.GCS,
+        pytest.param(storage_lib.StoreType.R2, marks=pytest.mark.cloudflare)
+    ])
     def test_new_bucket_creation_and_deletion(self, tmp_local_storage_obj,
                                               store_type):
         # Creates a new bucket with a local source, uploads files to it
         # and deletes it.
         tmp_local_storage_obj.add_store(store_type)
 
         # Run sky storage ls to check if storage object exists in the output
@@ -1749,16 +2075,46 @@
         subprocess.check_output(
             ['sky', 'storage', 'delete', tmp_local_storage_obj.name])
 
         # Run sky storage ls to check if storage object is deleted
         out = subprocess.check_output(['sky', 'storage', 'ls'])
         assert tmp_local_storage_obj.name not in out.decode('utf-8')
 
-    @pytest.mark.parametrize(
-        'store_type', [storage_lib.StoreType.S3, storage_lib.StoreType.GCS])
+    @pytest.mark.parametrize('store_type', [
+        storage_lib.StoreType.S3, storage_lib.StoreType.GCS,
+        pytest.param(storage_lib.StoreType.R2, marks=pytest.mark.cloudflare)
+    ])
+    def test_bucket_external_deletion(self, tmp_scratch_storage_obj,
+                                      store_type):
+        # Creates a bucket, deletes it externally using cloud cli commands
+        # and then tries to delete it using sky storage delete.
+        tmp_scratch_storage_obj.add_store(store_type)
+
+        # Run sky storage ls to check if storage object exists in the output
+        out = subprocess.check_output(['sky', 'storage', 'ls'])
+        assert tmp_scratch_storage_obj.name in out.decode('utf-8')
+
+        # Delete bucket externally
+        cmd = self.cli_delete_cmd(store_type, tmp_scratch_storage_obj.name)
+        subprocess.check_output(cmd, shell=True)
+
+        # Run sky storage delete to delete the storage object
+        out = subprocess.check_output(
+            ['sky', 'storage', 'delete', tmp_scratch_storage_obj.name])
+        # Make sure bucket was not created during deletion (see issue #1322)
+        assert 'created' not in out.decode('utf-8').lower()
+
+        # Run sky storage ls to check if storage object is deleted
+        out = subprocess.check_output(['sky', 'storage', 'ls'])
+        assert tmp_scratch_storage_obj.name not in out.decode('utf-8')
+
+    @pytest.mark.parametrize('store_type', [
+        storage_lib.StoreType.S3, storage_lib.StoreType.GCS,
+        pytest.param(storage_lib.StoreType.R2, marks=pytest.mark.cloudflare)
+    ])
     def test_bucket_bulk_deletion(self, store_type):
         # Create a temp folder with over 256 files and folders, upload
         # files and folders to a new bucket, then delete bucket.
         with tempfile.TemporaryDirectory() as tmpdir:
             subprocess.check_output(f'mkdir -p {tmpdir}/folder{{000..255}}',
                                     shell=True)
             subprocess.check_output(f'touch {tmpdir}/test{{000..255}}.txt',
@@ -1787,41 +2143,43 @@
         # added to global_user_state.
         tmp_public_storage_obj.add_store(store_type)
 
         # Run sky storage ls to check if storage object exists in the output
         out = subprocess.check_output(['sky', 'storage', 'ls'])
         assert tmp_public_storage_obj.name not in out.decode('utf-8')
 
-    @pytest.mark.parametrize('nonexist_bucket_url',
-                             ['s3://{random_name}', 'gs://{random_name}'])
+    @pytest.mark.parametrize('nonexist_bucket_url', [
+        's3://{random_name}', 'gs://{random_name}',
+        pytest.param('r2://{random_name}', marks=pytest.mark.cloudflare)
+    ])
     def test_nonexistent_bucket(self, nonexist_bucket_url):
         # Attempts to create fetch a stroage with a non-existent source.
         # Generate a random bucket name and verify it doesn't exist:
         retry_count = 0
         while True:
             nonexist_bucket_name = str(uuid.uuid4())
             if nonexist_bucket_url.startswith('s3'):
-                command = [
-                    'aws', 's3api', 'head-bucket', '--bucket',
-                    nonexist_bucket_name
-                ]
+                command = f'aws s3api head-bucket --bucket {nonexist_bucket_name}'
                 expected_output = '404'
             elif nonexist_bucket_url.startswith('gs'):
-                command = [
-                    'gsutil', 'ls',
-                    nonexist_bucket_url.format(random_name=nonexist_bucket_name)
-                ]
+                command = f'gsutil ls {nonexist_bucket_url.format(random_name=nonexist_bucket_name)}'
                 expected_output = 'BucketNotFoundException'
+            elif nonexist_bucket_url.startswith('r2'):
+                endpoint_url = cloudflare.create_endpoint()
+                command = f'AWS_SHARED_CREDENTIALS_FILE={cloudflare.R2_CREDENTIALS_PATH} aws s3api head-bucket --bucket {nonexist_bucket_name} --endpoint {endpoint_url} --profile=r2'
+                expected_output = '404'
             else:
                 raise ValueError('Unsupported bucket type '
                                  f'{nonexist_bucket_url}')
 
             # Check if bucket exists using the cli:
             try:
-                out = subprocess.check_output(command, stderr=subprocess.STDOUT)
+                out = subprocess.check_output(command,
+                                              stderr=subprocess.STDOUT,
+                                              shell=True)
             except subprocess.CalledProcessError as e:
                 out = e.output
             out = out.decode('utf-8')
             if expected_output in out:
                 break
             else:
                 retry_count += 1
@@ -1845,42 +2203,31 @@
         private_bucket_name = urllib.parse.urlsplit(private_bucket).netloc
         with pytest.raises(
                 sky.exceptions.StorageBucketGetError,
                 match=storage_lib._BUCKET_FAIL_TO_CONNECT_MESSAGE.format(
                     name=private_bucket_name)):
             storage_obj = storage_lib.Storage(source=private_bucket)
 
-    @staticmethod
-    def cli_ls_cmd(store_type, bucket_name, suffix=''):
-        if store_type == storage_lib.StoreType.S3:
-            if suffix:
-                url = f's3://{bucket_name}/{suffix}'
-            else:
-                url = f's3://{bucket_name}'
-            return ['aws', 's3', 'ls', url]
-        if store_type == storage_lib.StoreType.GCS:
-            if suffix:
-                url = f'gs://{bucket_name}/{suffix}'
-            else:
-                url = f'gs://{bucket_name}'
-            return ['gsutil', 'ls', url]
-
     @pytest.mark.parametrize('ext_bucket_fixture, store_type',
                              [('tmp_awscli_bucket', storage_lib.StoreType.S3),
-                              ('tmp_gsutil_bucket', storage_lib.StoreType.GCS)])
+                              ('tmp_gsutil_bucket', storage_lib.StoreType.GCS),
+                              pytest.param('tmp_awscli_bucket_r2',
+                                           storage_lib.StoreType.R2,
+                                           marks=pytest.mark.cloudflare)])
     def test_upload_to_existing_bucket(self, ext_bucket_fixture, request,
                                        tmp_source, store_type):
         # Tries uploading existing files to newly created bucket (outside of
         # sky) and verifies that files are written.
         bucket_name = request.getfixturevalue(ext_bucket_fixture)
         storage_obj = storage_lib.Storage(name=bucket_name, source=tmp_source)
         storage_obj.add_store(store_type)
 
         # Check if tmp_source/tmp-file exists in the bucket using aws cli
-        out = subprocess.check_output(self.cli_ls_cmd(store_type, bucket_name))
+        out = subprocess.check_output(self.cli_ls_cmd(store_type, bucket_name),
+                                      shell=True)
         assert 'tmp-file' in out.decode('utf-8'), \
             'File not found in bucket - output was : {}'.format(out.decode
                                                                 ('utf-8'))
 
         # Check symlinks - symlinks don't get copied by sky storage
         assert (pathlib.Path(tmp_source) / 'circle-link').is_symlink(), (
             'circle-link was not found in the upload source - '
@@ -1901,36 +2248,53 @@
         tmp_copy_mnt_existing_storage_obj.add_store(storage_lib.StoreType.S3)
         storage_name = tmp_copy_mnt_existing_storage_obj.name
 
         # Check `sky storage ls` to ensure storage object exists
         out = subprocess.check_output(['sky', 'storage', 'ls']).decode('utf-8')
         assert storage_name in out, f'Storage {storage_name} not found in sky storage ls.'
 
-    @pytest.mark.parametrize(
-        'store_type', [storage_lib.StoreType.S3, storage_lib.StoreType.GCS])
+    @pytest.mark.parametrize('store_type', [
+        storage_lib.StoreType.S3, storage_lib.StoreType.GCS,
+        pytest.param(storage_lib.StoreType.R2, marks=pytest.mark.cloudflare)
+    ])
     def test_list_source(self, tmp_local_list_storage_obj, store_type):
         # Uses a list in the source field to specify a file and a directory to
         # be uploaded to the storage object.
         tmp_local_list_storage_obj.add_store(store_type)
 
         # Check if tmp-file exists in the bucket root using cli
-        out = subprocess.check_output(
-            self.cli_ls_cmd(store_type, tmp_local_list_storage_obj.name))
+        out = subprocess.check_output(self.cli_ls_cmd(
+            store_type, tmp_local_list_storage_obj.name),
+                                      shell=True)
         assert 'tmp-file' in out.decode('utf-8'), \
             'File not found in bucket - output was : {}'.format(out.decode
                                                                 ('utf-8'))
 
         # Check if tmp-file exists in the bucket/tmp-source using cli
-        out = subprocess.check_output(
-            self.cli_ls_cmd(store_type, tmp_local_list_storage_obj.name,
-                            'tmp-source/'))
+        out = subprocess.check_output(self.cli_ls_cmd(
+            store_type, tmp_local_list_storage_obj.name, 'tmp-source/'),
+                                      shell=True)
         assert 'tmp-file' in out.decode('utf-8'), \
             'File not found in bucket - output was : {}'.format(out.decode
                                                                 ('utf-8'))
 
+    @pytest.mark.parametrize('invalid_name_list, store_type',
+                             [(AWS_INVALID_NAMES, storage_lib.StoreType.S3),
+                              (GCS_INVALID_NAMES, storage_lib.StoreType.GCS),
+                              pytest.param(AWS_INVALID_NAMES,
+                                           storage_lib.StoreType.R2,
+                                           marks=pytest.mark.cloudflare)])
+    def test_invalid_names(self, invalid_name_list, store_type):
+        # Uses a list in the source field to specify a file and a directory to
+        # be uploaded to the storage object.
+        for name in invalid_name_list:
+            with pytest.raises(sky.exceptions.StorageNameError):
+                storage_obj = storage_lib.Storage(name=name)
+                storage_obj.add_store(store_type)
+
 
 # ---------- Testing YAML Specs ----------
 # Our sky storage requires credentials to check the bucket existance when
 # loading a task from the yaml file, so we cannot make it a unit test.
 class TestYamlSpecs:
     # TODO(zhwu): Add test for `to_yaml_config` for the Storage object.
     #  We should not use `examples/storage_demo.yaml` here, since it requires
```

### Comparing `skypilot-0.2.5/tests/test_spot.py` & `skypilot-0.3.0/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.2.5/tests/test_storage.py` & `skypilot-0.3.0/tests/test_storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -79,7 +79,24 @@
     def test_noname_and_nosource(self):
         """Tests when neither name nor source is specified"""
         # Storage cannot be specified without name or source - invalid spec
         with pytest.raises(exceptions.StorageSpecError) as e:
             storage_lib.Storage()
 
         assert 'Storage source or storage name must be specified' in str(e)
+
+    def test_uri_in_name(self):
+        """Tests when name is a URI.
+
+        Other tests for invalid names require store-specific test cases, and
+        are in test_smoke.py::TestStorageWithCredentials"""
+        invalid_names = [
+            's3://mybucket',
+            'gs://mybucket',
+            'r2://mybucket',
+        ]
+
+        for n in invalid_names:
+            with pytest.raises(exceptions.StorageNameError) as e:
+                storage_lib.Storage(name=n)
+
+            assert 'Prefix detected' in str(e)
```

### Comparing `skypilot-0.2.5/tests/test_wheels.py` & `skypilot-0.3.0/tests/test_wheels.py`

 * *Files identical despite different names*

