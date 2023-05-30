# Comparing `tmp/flytekit-1.6.1b0.tar.gz` & `tmp/flytekit-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.6.1b0.tar", last modified: Mon May 15 22:06:54 2023, max compression
+gzip compressed data, was "flytekit-1.6.2.tar", last modified: Tue May 30 15:24:06 2023, max compression
```

## Comparing `flytekit-1.6.1b0.tar` & `flytekit-1.6.2.tar`

### file list

```diff
@@ -1,253 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.715864 flytekit-1.6.1b0/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-15 22:06:53.000000 flytekit-1.6.1b0/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50556 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28484 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    30303 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.723864 flytekit-1.6.1b0/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    35947 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    31127 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    36181 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    46418 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    77129 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extend/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extend/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extend/backend/base_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extend/backend/external_plugin_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interfaces/stats/taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/lazy_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/lazy_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/lazy_import/lazy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.731864 flytekit-1.6.1b0/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.731864 flytekit-1.6.1b0/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.731864 flytekit-1.6.1b0/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    84835 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44537 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.715864 flytekit-1.6.1b0/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-15 22:06:54.000000 flytekit-1.6.1b0/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-15 22:06:54.000000 flytekit-1.6.1b0/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:06:54.000000 flytekit-1.6.1b0/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-15 22:06:54.000000 flytekit-1.6.1b0/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-15 22:06:54.000000 flytekit-1.6.1b0/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 22:06:54.000000 flytekit-1.6.1b0/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-15 22:06:53.000000 flytekit-1.6.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-30 15:23:56.000000 flytekit-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-30 15:23:56.000000 flytekit-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-30 15:24:06.901439 flytekit-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-30 15:23:56.000000 flytekit-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.881439 flytekit-1.6.2/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-05-30 15:24:05.000000 flytekit-1.6.2/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.889439 flytekit-1.6.2/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.889439 flytekit-1.6.2/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    36184 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31127 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36181 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46442 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77072 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extend/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extend/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extend/backend/base_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extend/backend/external_plugin_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.893439 flytekit-1.6.2/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/interfaces/stats/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/lazy_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/lazy_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/lazy_import/lazy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.897439 flytekit-1.6.2/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87310 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44537 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.885439 flytekit-1.6.2/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-30 15:24:06.000000 flytekit-1.6.2/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-30 15:24:06.000000 flytekit-1.6.2/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:24:06.000000 flytekit-1.6.2/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-30 15:24:06.000000 flytekit-1.6.2/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-30 15:24:06.000000 flytekit-1.6.2/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 15:24:06.000000 flytekit-1.6.2/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:06.901439 flytekit-1.6.2/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-30 15:23:56.000000 flytekit-1.6.2/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-30 15:23:56.000000 flytekit-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-30 15:24:06.905439 flytekit-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-30 15:24:05.000000 flytekit-1.6.2/setup.py
```

### Comparing `flytekit-1.6.1b0/LICENSE` & `flytekit-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/MANIFEST.in` & `flytekit-1.6.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/PKG-INFO` & `flytekit-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.1b0
+Version: 1.6.2
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.1b0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.2 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.1b0/README.md` & `flytekit-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/__init__.py` & `flytekit-1.6.2/flytekit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.6.1b0"
+__version__ = "1.6.2"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
```

### Comparing `flytekit-1.6.1b0/flytekit/bin/entrypoint.py` & `flytekit-1.6.2/flytekit/bin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clients/auth/auth_client.py` & `flytekit-1.6.2/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clients/auth/authenticator.py` & `flytekit-1.6.2/flytekit/clients/auth/authenticator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import subprocess
 import typing
 from abc import abstractmethod
 from dataclasses import dataclass
 
+import click
+
 from . import token_client
 from .auth_client import AuthorizationClient
 from .exceptions import AccessTokenNotFoundError, AuthenticationError
 from .keyring import Credentials, KeyringStore
 
 
 @dataclass
@@ -44,18 +46,27 @@
 
 
 class Authenticator(object):
     """
     Base authenticator for all authentication flows
     """
 
-    def __init__(self, endpoint: str, header_key: str, credentials: Credentials = None):
+    def __init__(
+        self,
+        endpoint: str,
+        header_key: str,
+        credentials: Credentials = None,
+        http_proxy_url: typing.Optional[str] = None,
+        verify: typing.Optional[typing.Union[bool, str]] = None,
+    ):
         self._endpoint = endpoint
         self._creds = credentials
         self._header_key = header_key if header_key else "authorization"
+        self._http_proxy_url = http_proxy_url
+        self._verify = verify
 
     def get_credentials(self) -> Credentials:
         return self._creds
 
     def _set_credentials(self, creds):
         self._creds = creds
 
@@ -83,18 +94,17 @@
         cfg_store: ClientConfigStore,
         header_key: typing.Optional[str] = None,
         verify: typing.Optional[typing.Union[bool, str]] = None,
     ):
         """
         Initialize with default creds from KeyStore using the endpoint name
         """
-        super().__init__(endpoint, header_key, KeyringStore.retrieve(endpoint))
+        super().__init__(endpoint, header_key, KeyringStore.retrieve(endpoint), verify=verify)
         self._cfg_store = cfg_store
         self._auth_client = None
-        self._verify = verify
 
     def _initialize_auth_client(self):
         if not self._auth_client:
             cfg = self._cfg_store.get_client_config()
             self._set_header_key(cfg.header_key)
             self._auth_client = AuthorizationClient(
                 endpoint=self._endpoint,
@@ -158,24 +168,26 @@
         self,
         endpoint: str,
         client_id: str,
         client_secret: str,
         cfg_store: ClientConfigStore,
         header_key: typing.Optional[str] = None,
         scopes: typing.Optional[typing.List[str]] = None,
+        http_proxy_url: typing.Optional[str] = None,
+        verify: typing.Optional[typing.Union[bool, str]] = None,
     ):
         if not client_id or not client_secret:
             raise ValueError("Client ID and Client SECRET both are required.")
         cfg = cfg_store.get_client_config()
         self._token_endpoint = cfg.token_endpoint
         # Use scopes from `flytekit.configuration.PlatformConfig` if passed
         self._scopes = scopes or cfg.scopes
         self._client_id = client_id
         self._client_secret = client_secret
-        super().__init__(endpoint, cfg.header_key or header_key)
+        super().__init__(endpoint, cfg.header_key or header_key, http_proxy_url=http_proxy_url, verify=verify)
 
     def refresh_credentials(self):
         """
         This function is used by the _handle_rpc_error() decorator, depending on the AUTH_MODE config object. This handler
         is meant for SDK use-cases of auth (like pyflyte, or when users call SDK functions that require access to Admin,
         like when waiting for another workflow to complete from within a task). This function uses basic auth, which means
         the credentials for basic auth must be present from wherever this code is running.
@@ -183,15 +195,18 @@
         """
         token_endpoint = self._token_endpoint
         scopes = self._scopes
 
         # Note that unlike the Pkce flow, the client ID does not come from Admin.
         logging.debug(f"Basic authorization flow with client id {self._client_id} scope {scopes}")
         authorization_header = token_client.get_basic_authorization_header(self._client_id, self._client_secret)
-        token, expires_in = token_client.get_token(token_endpoint, scopes, authorization_header)
+
+        token, expires_in = token_client.get_token(
+            token_endpoint, scopes, authorization_header, http_proxy_url=self._http_proxy_url, verify=self._verify
+        )
         logging.info("Retrieved new token, expires in {}".format(expires_in))
         self._creds = Credentials(token)
 
 
 class DeviceCodeAuthenticator(Authenticator):
     """
     This Authenticator implements the Device Code authorization flow useful for headless user authentication.
@@ -203,39 +218,49 @@
 
     def __init__(
         self,
         endpoint: str,
         cfg_store: ClientConfigStore,
         header_key: typing.Optional[str] = None,
         audience: typing.Optional[str] = None,
+        http_proxy_url: typing.Optional[str] = None,
+        verify: typing.Optional[typing.Union[bool, str]] = None,
     ):
         self._audience = audience
         cfg = cfg_store.get_client_config()
         self._client_id = cfg.client_id
         self._device_auth_endpoint = cfg.device_authorization_endpoint
         self._scope = cfg.scopes
         self._token_endpoint = cfg.token_endpoint
         if self._device_auth_endpoint is None:
             raise AuthenticationError(
                 "Device Authentication is not available on the Flyte backend / authentication server"
             )
         super().__init__(
-            endpoint=endpoint, header_key=header_key or cfg.header_key, credentials=KeyringStore.retrieve(endpoint)
+            endpoint=endpoint,
+            header_key=header_key or cfg.header_key,
+            credentials=KeyringStore.retrieve(endpoint),
+            http_proxy_url=http_proxy_url,
+            verify=verify,
         )
 
     def refresh_credentials(self):
-        resp = token_client.get_device_code(self._device_auth_endpoint, self._client_id, self._audience, self._scope)
-        print(
-            f"""
-To Authenticate navigate in a browser to the following URL: {resp.verification_uri} and enter code: {resp.user_code}
-OR copy paste the following URL: {resp.verification_uri_complete}
-        """
+        resp = token_client.get_device_code(
+            self._device_auth_endpoint, self._client_id, self._audience, self._scope, self._http_proxy_url, self._verify
         )
+        text = f"To Authenticate, navigate in a browser to the following URL: {click.style(resp.verification_uri, fg='blue', underline=True)} and enter code: {click.style(resp.user_code, fg='blue')}"
+        click.secho(text)
         try:
             # Currently the refresh token is not retreived. We may want to add support for refreshTokens so that
             # access tokens can be refreshed for once authenticated machines
-            token, expires_in = token_client.poll_token_endpoint(resp, self._token_endpoint, client_id=self._client_id)
+            token, expires_in = token_client.poll_token_endpoint(
+                resp,
+                self._token_endpoint,
+                client_id=self._client_id,
+                http_proxy_url=self._http_proxy_url,
+                verify=self._verify,
+            )
             self._creds = Credentials(access_token=token, expires_in=expires_in, for_endpoint=self._endpoint)
             KeyringStore.store(self._creds)
         except Exception:
             KeyringStore.delete(self._endpoint)
             raise
```

### Comparing `flytekit-1.6.1b0/flytekit/clients/auth/keyring.py` & `flytekit-1.6.2/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clients/auth/token_client.py` & `flytekit-1.6.2/flytekit/clients/auth/token_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import typing
 import urllib.parse
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 
 import requests
 
+from flytekit import logger
 from flytekit.clients.auth.exceptions import AuthenticationError, AuthenticationPending
 
 utf_8 = "utf-8"
 
 # Errors that Token endpoint will return
 error_slow_down = "slow_down"
 error_auth_pending = "authorization_pending"
@@ -27,33 +28,30 @@
 @dataclass
 class DeviceCodeResponse:
     """
     Response from device auth flow endpoint
     {'device_code': 'code',
          'user_code': 'BNDJJFXL',
          'verification_uri': 'url',
-         'verification_uri_complete': 'url',
          'expires_in': 600,
          'interval': 5}
     """
 
     device_code: str
     user_code: str
     verification_uri: str
-    verification_uri_complete: str
     expires_in: int
     interval: int
 
     @classmethod
     def from_json_response(cls, j: typing.Dict) -> "DeviceCodeResponse":
         return cls(
             device_code=j["device_code"],
             user_code=j["user_code"],
             verification_uri=j["verification_uri"],
-            verification_uri_complete=j["verification_uri_complete"],
             expires_in=j["expires_in"],
             interval=j["interval"],
         )
 
 
 def get_basic_authorization_header(client_id: str, client_secret: str) -> str:
     """
@@ -73,14 +71,16 @@
 def get_token(
     token_endpoint: str,
     scopes: typing.Optional[typing.List[str]] = None,
     authorization_header: typing.Optional[str] = None,
     client_id: typing.Optional[str] = None,
     device_code: typing.Optional[str] = None,
     grant_type: GrantType = GrantType.CLIENT_CREDS,
+    http_proxy_url: typing.Optional[str] = None,
+    verify: typing.Optional[typing.Union[bool, str]] = None,
 ) -> typing.Tuple[str, int]:
     """
     :rtype: (Text,Int) The first element is the access token retrieved from the IDP, the second is the expiration
             in seconds
     """
     headers = {
         "Cache-Control": "no-cache",
@@ -95,15 +95,16 @@
     if client_id:
         body["client_id"] = client_id
     if device_code:
         body["device_code"] = device_code
     if scopes is not None:
         body["scope"] = ",".join(scopes)
 
-    response = requests.post(token_endpoint, data=body, headers=headers)
+    proxies = {"https": http_proxy_url, "http": http_proxy_url} if http_proxy_url else None
+    response = requests.post(token_endpoint, data=body, headers=headers, proxies=proxies, verify=verify)
     if not response.ok:
         j = response.json()
         if "error" in j:
             err = j["error"]
             if err == error_auth_pending or err == error_slow_down:
                 raise AuthenticationPending(f"Token not yet available, try again in some time {err}")
         logging.error("Status Code ({}) received from IDP: {}".format(response.status_code, response.text))
@@ -114,41 +115,54 @@
 
 
 def get_device_code(
     device_auth_endpoint: str,
     client_id: str,
     audience: typing.Optional[str] = None,
     scope: typing.Optional[typing.List[str]] = None,
+    http_proxy_url: typing.Optional[str] = None,
+    verify: typing.Optional[typing.Union[bool, str]] = None,
 ) -> DeviceCodeResponse:
     """
     Retrieves the device Authentication code that can be done to authenticate the request using a browser on a
     separate device
     """
-    payload = {"client_id": client_id, "scope": scope, "audience": audience}
-    resp = requests.post(device_auth_endpoint, payload)
+    _scope = " ".join(scope) if scope is not None else ""
+    payload = {"client_id": client_id, "scope": _scope, "audience": audience}
+    proxies = {"https": http_proxy_url, "http": http_proxy_url} if http_proxy_url else None
+    resp = requests.post(device_auth_endpoint, payload, proxies=proxies, verify=verify)
     if not resp.ok:
         raise AuthenticationError(f"Unable to retrieve Device Authentication Code for {payload}, Reason {resp.reason}")
     return DeviceCodeResponse.from_json_response(resp.json())
 
 
-def poll_token_endpoint(resp: DeviceCodeResponse, token_endpoint: str, client_id: str) -> typing.Tuple[str, int]:
+def poll_token_endpoint(
+    resp: DeviceCodeResponse,
+    token_endpoint: str,
+    client_id: str,
+    http_proxy_url: typing.Optional[str] = None,
+    verify: typing.Optional[typing.Union[bool, str]] = None,
+) -> typing.Tuple[str, int]:
     tick = datetime.now()
     interval = timedelta(seconds=resp.interval)
     end_time = tick + timedelta(seconds=resp.expires_in)
     while tick < end_time:
         try:
             access_token, expires_in = get_token(
                 token_endpoint,
                 grant_type=GrantType.DEVICE_CODE,
                 client_id=client_id,
                 device_code=resp.device_code,
+                http_proxy_url=http_proxy_url,
+                verify=verify,
             )
             print("Authentication successful!")
             return access_token, expires_in
         except AuthenticationPending:
             ...
-        except Exception:
-            raise
+        except Exception as e:
+            logger.error("Authentication attempt failed: ", e)
+            raise e
         print("Authentication Pending...")
         time.sleep(interval.total_seconds())
         tick = tick + interval
     raise AuthenticationError("Authentication failed!")
```

### Comparing `flytekit-1.6.1b0/flytekit/clients/auth_helper.py` & `flytekit-1.6.2/flytekit/clients/auth_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,39 +54,48 @@
     if type(cfg_auth) is str:
         try:
             cfg_auth = AuthType[cfg_auth.upper()]
         except KeyError:
             logging.warning(f"Authentication type {cfg_auth} does not exist, defaulting to standard")
             cfg_auth = AuthType.STANDARD
 
+    verify = None
+    if cfg.insecure_skip_verify:
+        verify = False
+    elif cfg.ca_cert_file_path:
+        verify = cfg.ca_cert_file_path
+
     if cfg_auth == AuthType.STANDARD or cfg_auth == AuthType.PKCE:
-        verify = None
-        if cfg.insecure_skip_verify:
-            verify = False
-        elif cfg.ca_cert_file_path:
-            verify = cfg.ca_cert_file_path
         return PKCEAuthenticator(cfg.endpoint, cfg_store, verify=verify)
     elif cfg_auth == AuthType.BASIC or cfg_auth == AuthType.CLIENT_CREDENTIALS or cfg_auth == AuthType.CLIENTSECRET:
         return ClientCredentialsAuthenticator(
             endpoint=cfg.endpoint,
             client_id=cfg.client_id,
             client_secret=cfg.client_credentials_secret,
             cfg_store=cfg_store,
             scopes=cfg.scopes,
+            http_proxy_url=cfg.http_proxy_url,
+            verify=verify,
         )
     elif cfg_auth == AuthType.EXTERNAL_PROCESS or cfg_auth == AuthType.EXTERNALCOMMAND:
         client_cfg = None
         if cfg_store:
             client_cfg = cfg_store.get_client_config()
         return CommandAuthenticator(
             command=cfg.command,
             header_key=client_cfg.header_key if client_cfg else None,
         )
     elif cfg_auth == AuthType.DEVICEFLOW:
-        return DeviceCodeAuthenticator(endpoint=cfg.endpoint, cfg_store=cfg_store, audience=cfg.audience)
+        return DeviceCodeAuthenticator(
+            endpoint=cfg.endpoint,
+            cfg_store=cfg_store,
+            audience=cfg.audience,
+            http_proxy_url=cfg.http_proxy_url,
+            verify=verify,
+        )
     else:
         raise ValueError(
             f"Invalid auth mode [{cfg_auth}] specified." f"Please update the creds config to use a valid value"
         )
 
 
 def upgrade_channel_to_authenticated(cfg: PlatformConfig, in_channel: grpc.Channel) -> grpc.Channel:
```

### Comparing `flytekit-1.6.1b0/flytekit/clients/friendly.py` & `flytekit-1.6.2/flytekit/clients/friendly.py`

 * *Files 1% similar despite different names*

```diff
@@ -1014,7 +1014,13 @@
             expires_in_pb.FromTimedelta(expires_in)
         return super(SynchronousFlyteClient, self).create_download_location(
             _data_proxy_pb2.CreateDownloadLocationRequest(
                 native_url=native_url,
                 expires_in=expires_in_pb,
             )
         )
+
+    def get_data(self, flyte_uri: str) -> _data_proxy_pb2.GetDataResponse:
+        req = _data_proxy_pb2.GetDataRequest(flyte_url=flyte_uri)
+
+        resp = self._dataproxy_stub.GetData(req, metadata=self._metadata)
+        return resp
```

### Comparing `flytekit-1.6.1b0/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.6.2/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.6.2/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clients/helpers.py` & `flytekit-1.6.2/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clients/raw.py` & `flytekit-1.6.2/flytekit/clients/raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,13 +575,13 @@
         :rtype: flyteidl.service.dataproxy_pb2.CreateUploadLocationResponse
         """
         return self._dataproxy_stub.CreateUploadLocation(create_upload_location_request, metadata=self._metadata)
 
     def create_download_location(
         self, create_download_location_request: _dataproxy_pb2.CreateDownloadLocationRequest
     ) -> _dataproxy_pb2.CreateDownloadLocationResponse:
-        """
-        Get a signed url to be used during fast registration
-        :param flyteidl.service.dataproxy_pb2.CreateDownloadLocationRequest create_download_location_request:
-        :rtype: flyteidl.service.dataproxy_pb2.CreateDownloadLocationResponse
-        """
         return self._dataproxy_stub.CreateDownloadLocation(create_download_location_request, metadata=self._metadata)
+
+    def create_download_link(
+        self, create_download_link_request: _dataproxy_pb2.CreateDownloadLinkRequest
+    ) -> _dataproxy_pb2.CreateDownloadLinkResponse:
+        return self._dataproxy_stub.CreateDownloadLink(create_download_link_request, metadata=self._metadata)
```

### Comparing `flytekit-1.6.1b0/flytekit/clis/flyte_cli/main.py` & `flytekit-1.6.2/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clis/helpers.py` & `flytekit-1.6.2/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.6.2/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.6.2/flytekit/clis/sdk_in_container/build.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.6.2/flytekit/clis/sdk_in_container/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.6.2/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.6.2/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.6.2/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/metrics.py` & `flytekit-1.6.2/flytekit/clis/sdk_in_container/metrics.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.6.2/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.6.2/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.6.2/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.6.2/flytekit/clis/sdk_in_container/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 import os
 import pathlib
 import typing
 from dataclasses import dataclass
 from typing import cast
 
+import cloudpickle
 import rich_click as click
 import yaml
 from dataclasses_json import DataClassJsonMixin
 from pytimeparse import parse
 from typing_extensions import get_args
 
 from flytekit import BlobType, Literal, Scalar
@@ -29,26 +30,27 @@
     get_and_save_remote_with_click_context,
     patch_image_config,
 )
 from flytekit.configuration import ImageConfig
 from flytekit.configuration.default_images import DefaultImages
 from flytekit.core import context_manager
 from flytekit.core.base_task import PythonTask
-from flytekit.core.context_manager import FlyteContext
+from flytekit.core.context_manager import FlyteContext, FlyteContextManager
 from flytekit.core.data_persistence import FileAccessProvider
 from flytekit.core.type_engine import TypeEngine
 from flytekit.core.workflow import PythonFunctionWorkflow, WorkflowBase
 from flytekit.models import literals
 from flytekit.models.interface import Variable
 from flytekit.models.literals import Blob, BlobMetadata, LiteralCollection, LiteralMap, Primitive, Union
 from flytekit.models.types import LiteralType, SimpleType
 from flytekit.remote.executions import FlyteWorkflowExecution
 from flytekit.tools import module_loader, script_mode
 from flytekit.tools.script_mode import _find_project_root
 from flytekit.tools.translator import Options
+from flytekit.types.pickle.pickle import FlytePickleTransformer
 
 REMOTE_FLAG_KEY = "remote"
 RUN_LEVEL_PARAMS_KEY = "run_level_params"
 DATA_PROXY_CALLBACK_KEY = "data_proxy"
 
 
 def remove_prefix(text, prefix):
@@ -99,14 +101,27 @@
             return FileParam(filepath=value, local=False)
         p = pathlib.Path(value)
         if p.exists() and p.is_file():
             return FileParam(filepath=str(p.resolve()))
         raise click.BadParameter(f"parameter should be a valid file path, {value}")
 
 
+class PickleParamType(click.ParamType):
+    name = "pickle"
+
+    def convert(
+        self, value: typing.Any, param: typing.Optional[click.Parameter], ctx: typing.Optional[click.Context]
+    ) -> typing.Any:
+
+        uri = FlyteContextManager.current_context().file_access.get_random_local_path()
+        with open(uri, "w+b") as outfile:
+            cloudpickle.dump(value, outfile)
+        return FileParam(filepath=str(pathlib.Path(uri).resolve()))
+
+
 class DateTimeType(click.DateTime):
 
     _NOW_FMT = "now"
     _ADDITONAL_FORMATS = [_NOW_FMT]
 
     def __init__(self):
         super().__init__()
@@ -223,15 +238,18 @@
             if self._literal_type.collection_type:
                 self._click_type.name = "json list"
             else:
                 self._click_type.name = "json dictionary"
 
         if self._literal_type.blob:
             if self._literal_type.blob.dimensionality == BlobType.BlobDimensionality.SINGLE:
-                self._click_type = FileParamType()
+                if self._literal_type.blob.format == FlytePickleTransformer.PYTHON_PICKLE_FORMAT:
+                    self._click_type = PickleParamType()
+                else:
+                    self._click_type = FileParamType()
             else:
                 self._click_type = DirParamType()
 
     @property
     def click_type(self) -> click.ParamType:
         return self._click_type
```

### Comparing `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.6.2/flytekit/clis/sdk_in_container/serialize.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/serve.py` & `flytekit-1.6.2/flytekit/clis/sdk_in_container/serve.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/configuration/__init__.py` & `flytekit-1.6.2/flytekit/configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,28 +372,30 @@
       More details here: https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/.
     :param client_credentials_secret: Used for service auth, which is automatically called during pyflyte. This will
       allow the Flyte engine to read the password directly from the environment variable. Note that this is
       less secure! Please only use this if mounting the secret as a file is impossible
     :param scopes: List of scopes to request. This is only applicable to the client credentials flow
     :param auth_mode: The OAuth mode to use. Defaults to pkce flow
     :param ca_cert_file_path: [optional] str Root Cert to be loaded and used to verify admin
+    :param http_proxy_url: [optional] HTTP Proxy to be used for OAuth requests
     """
 
     endpoint: str = "localhost:30080"
     insecure: bool = False
     insecure_skip_verify: bool = False
     ca_cert_file_path: typing.Optional[str] = None
     console_endpoint: typing.Optional[str] = None
     command: typing.Optional[typing.List[str]] = None
     client_id: typing.Optional[str] = None
     client_credentials_secret: typing.Optional[str] = None
     scopes: List[str] = field(default_factory=list)
     auth_mode: AuthType = AuthType.STANDARD
     audience: typing.Optional[str] = None
     rpc_retries: int = 3
+    http_proxy_url: typing.Optional[str] = None
 
     @classmethod
     def auto(cls, config_file: typing.Optional[typing.Union[str, ConfigFile]] = None) -> PlatformConfig:
         """
         Reads from Config file, and overrides from Environment variables. Refer to ConfigEntry for details
         :param config_file:
         :return:
@@ -422,14 +424,15 @@
             "client_credentials_secret",
             client_credentials_secret,
         )
         kwargs = set_if_exists(kwargs, "scopes", _internal.Credentials.SCOPES.read(config_file))
         kwargs = set_if_exists(kwargs, "auth_mode", _internal.Credentials.AUTH_MODE.read(config_file))
         kwargs = set_if_exists(kwargs, "endpoint", _internal.Platform.URL.read(config_file))
         kwargs = set_if_exists(kwargs, "console_endpoint", _internal.Platform.CONSOLE_ENDPOINT.read(config_file))
+        kwargs = set_if_exists(kwargs, "http_proxy_url", _internal.Platform.HTTP_PROXY_URL.read(config_file))
         return PlatformConfig(**kwargs)
 
     @classmethod
     def for_endpoint(cls, endpoint: str, insecure: bool = False) -> PlatformConfig:
         return PlatformConfig(endpoint=endpoint, insecure=insecure)
```

### Comparing `flytekit-1.6.1b0/flytekit/configuration/default_images.py` & `flytekit-1.6.2/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/configuration/feature_flags.py` & `flytekit-1.6.2/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/configuration/file.py` & `flytekit-1.6.2/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/configuration/internal.py` & `flytekit-1.6.2/flytekit/configuration/internal.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     INSECURE_SKIP_VERIFY = ConfigEntry(
         LegacyConfigEntry(SECTION, "insecure_skip_verify", bool), YamlConfigEntry("admin.insecureSkipVerify", bool)
     )
     CONSOLE_ENDPOINT = ConfigEntry(LegacyConfigEntry(SECTION, "console_endpoint"), YamlConfigEntry("console.endpoint"))
     CA_CERT_FILE_PATH = ConfigEntry(
         LegacyConfigEntry(SECTION, "ca_cert_file_path"), YamlConfigEntry("admin.caCertFilePath")
     )
+    HTTP_PROXY_URL = ConfigEntry(LegacyConfigEntry(SECTION, "http_proxy_url"), YamlConfigEntry("admin.httpProxyURL"))
 
 
 class LocalSDK(object):
     SECTION = "sdk"
     WORKFLOW_PACKAGES = ConfigEntry(LegacyConfigEntry(SECTION, "workflow_packages", list))
     """
     This is a comma-delimited list of packages that SDK tools will use to discover entities for the purpose of registration
```

### Comparing `flytekit-1.6.1b0/flytekit/core/annotation.py` & `flytekit-1.6.2/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/base_sql_task.py` & `flytekit-1.6.2/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/base_task.py` & `flytekit-1.6.2/flytekit/core/base_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/checkpointer.py` & `flytekit-1.6.2/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/class_based_resolver.py` & `flytekit-1.6.2/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/condition.py` & `flytekit-1.6.2/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/constants.py` & `flytekit-1.6.2/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/container_task.py` & `flytekit-1.6.2/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/context_manager.py` & `flytekit-1.6.2/flytekit/core/context_manager.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/data_persistence.py` & `flytekit-1.6.2/flytekit/core/data_persistence.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/docstring.py` & `flytekit-1.6.2/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.6.2/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/gate.py` & `flytekit-1.6.2/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/interface.py` & `flytekit-1.6.2/flytekit/core/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/launch_plan.py` & `flytekit-1.6.2/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/local_cache.py` & `flytekit-1.6.2/flytekit/core/local_cache.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/map_task.py` & `flytekit-1.6.2/flytekit/core/map_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from flytekit.configuration import SerializationSettings
 from flytekit.core import tracker
 from flytekit.core.base_task import PythonTask, Task, TaskResolverMixin
 from flytekit.core.constants import SdkTaskType
 from flytekit.core.context_manager import ExecutionState, FlyteContext, FlyteContextManager
 from flytekit.core.interface import transform_interface_to_list_interface
-from flytekit.core.python_function_task import PythonFunctionTask
+from flytekit.core.python_function_task import PythonFunctionTask, PythonInstanceTask
 from flytekit.core.tracker import TrackedInstance
 from flytekit.core.utils import timeit
 from flytekit.exceptions import scopes as exception_scopes
 from flytekit.models.array_job import ArrayJob
 from flytekit.models.interface import Variable
 from flytekit.models.task import Container, K8sPod, Sql
 from flytekit.tools.module_loader import load_object_from_module
@@ -30,15 +30,15 @@
     """
     A MapPythonTask defines a :py:class:`flytekit.PythonTask` which specifies how to run
     an inner :py:class:`flytekit.PythonFunctionTask` across a range of inputs in parallel.
     """
 
     def __init__(
         self,
-        python_function_task: typing.Union[PythonFunctionTask, functools.partial],
+        python_function_task: typing.Union[PythonFunctionTask, PythonInstanceTask, functools.partial],
         concurrency: Optional[int] = None,
         min_success_ratio: Optional[float] = None,
         bound_inputs: Optional[Set[str]] = None,
         **kwargs,
     ):
         """
         Wrapper that creates a MapPythonTask
@@ -61,26 +61,33 @@
                     raise ValueError("Map tasks do not support partial tasks with lists as inputs. ")
             self._partial = python_function_task
             actual_task = self._partial.func
         else:
             actual_task = python_function_task
 
         if not isinstance(actual_task, PythonFunctionTask):
-            raise ValueError("Map tasks can only compose of Python Functon Tasks currently")
+            if isinstance(actual_task, PythonInstanceTask):
+                pass
+            else:
+                raise ValueError("Map tasks can only compose of PythonFuncton and PythonInstanceTasks currently")
 
         if len(actual_task.python_interface.outputs.keys()) > 1:
             raise ValueError("Map tasks only accept python function tasks with 0 or 1 outputs")
 
         self._bound_inputs: typing.Set[str] = set(bound_inputs) if bound_inputs else set()
         if self._partial:
             self._bound_inputs = set(self._partial.keywords.keys())
 
         collection_interface = transform_interface_to_list_interface(actual_task.python_interface, self._bound_inputs)
         self._run_task: PythonFunctionTask = actual_task
-        _, mod, f, _ = tracker.extract_task_module(actual_task.task_function)
+        if isinstance(actual_task, PythonInstanceTask):
+            mod = actual_task.task_type
+            f = actual_task.lhs
+        else:
+            _, mod, f, _ = tracker.extract_task_module(actual_task.task_function)
         h = hashlib.md5(collection_interface.__str__().encode("utf-8")).hexdigest()
         name = f"{mod}.map_{f}_{h}"
 
         self._cmd_prefix: typing.Optional[typing.List[str]] = None
         self._max_concurrency: typing.Optional[int] = concurrency
         self._min_success_ratio: typing.Optional[float] = min_success_ratio
         self._array_task_interface = actual_task.python_interface
@@ -267,15 +274,15 @@
             if outputs_expected:
                 outputs.append(o)
 
         return outputs
 
 
 def map_task(
-    task_function: typing.Union[PythonFunctionTask, functools.partial],
+    task_function: typing.Union[PythonFunctionTask, PythonInstanceTask, functools.partial],
     concurrency: int = 0,
     min_success_ratio: float = 1.0,
     **kwargs,
 ):
     """
     Use a map task for parallelizable tasks that run across a list of an input type. A map task can be composed of
     any individual :py:class:`flytekit.PythonFunctionTask`.
```

### Comparing `flytekit-1.6.1b0/flytekit/core/mock_stats.py` & `flytekit-1.6.2/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/node.py` & `flytekit-1.6.2/flytekit/core/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,16 @@
             self._metadata._name = kwargs["name"]
         if "task_config" in kwargs:
             logger.warning("This override is beta. We may want to revisit this in the future.")
             new_task_config = kwargs["task_config"]
             if not isinstance(new_task_config, type(self.flyte_entity._task_config)):
                 raise ValueError("can't change the type of the task config")
             self.flyte_entity._task_config = new_task_config
+        if "container_image" in kwargs:
+            self.flyte_entity._container_image = kwargs["container_image"]
         return self
 
 
 def _convert_resource_overrides(
     resources: typing.Optional[Resources], resource_name: str
 ) -> typing.List[_resources_model.ResourceEntry]:
     if resources is None:
```

### Comparing `flytekit-1.6.1b0/flytekit/core/node_creation.py` & `flytekit-1.6.2/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/notification.py` & `flytekit-1.6.2/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/pod_template.py` & `flytekit-1.6.2/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/promise.py` & `flytekit-1.6.2/flytekit/core/promise.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,15 +615,15 @@
             return _literals_models.BindingData(promise=t_value.ref)
 
     elif isinstance(t_value, VoidPromise):
         raise AssertionError(
             f"Cannot pass output from task {t_value.task_name} that produces no outputs to a downstream task"
         )
 
-    elif expected_literal_type.union_type is not None:
+    elif t_value is not None and expected_literal_type.union_type is not None:
         for i in range(len(expected_literal_type.union_type.variants)):
             try:
                 lt_type = expected_literal_type.union_type.variants[i]
                 python_type = get_args(t_value_type)[i] if t_value_type else None
                 return binding_data_from_python_std(ctx, lt_type, t_value, python_type)
             except Exception:
                 logger.debug(
```

### Comparing `flytekit-1.6.1b0/flytekit/core/python_auto_container.py` & `flytekit-1.6.2/flytekit/core/python_auto_container.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/python_customized_container_task.py` & `flytekit-1.6.2/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/python_function_task.py` & `flytekit-1.6.2/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/reference.py` & `flytekit-1.6.2/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/reference_entity.py` & `flytekit-1.6.2/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/resources.py` & `flytekit-1.6.2/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/schedule.py` & `flytekit-1.6.2/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/shim_task.py` & `flytekit-1.6.2/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/task.py` & `flytekit-1.6.2/flytekit/core/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/testing.py` & `flytekit-1.6.2/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/tracker.py` & `flytekit-1.6.2/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/type_engine.py` & `flytekit-1.6.2/flytekit/core/type_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,16 +169,15 @@
         if type(python_val) != self._type:
             raise TypeTransformerFailedError(
                 f"Expected value of type {self._type} but got '{python_val}' of type {type(python_val)}"
             )
         return self._to_literal_transformer(python_val)
 
     def to_python_value(self, ctx: FlyteContext, lv: Literal, expected_python_type: Type[T]) -> T:
-        if get_origin(expected_python_type) is Annotated:
-            expected_python_type = get_args(expected_python_type)[0]
+        expected_python_type = get_underlying_type(expected_python_type)
 
         if expected_python_type != self._type:
             raise TypeTransformerFailedError(
                 f"Cannot convert to type {expected_python_type}, only {self._type} is supported"
             )
 
         try:  # todo(maximsmol): this is quite ugly and each transformer should really check their Literal
@@ -307,15 +306,15 @@
                 raise TypeTransformerFailedError(f"Type of Val '{original_type}' is not an instance of {expected_type}")
 
     def get_literal_type(self, t: Type[T]) -> LiteralType:
         """
         Extracts the Literal type definition for a Dataclass and returns a type Struct.
         If possible also extracts the JSONSchema for the dataclass.
         """
-        if get_origin(t) is Annotated:
+        if is_annotated(t):
             raise ValueError(
                 "Flytekit does not currently have support for FlyteAnnotations applied to Dataclass."
                 f"Type {t} cannot be parsed."
             )
 
         if not issubclass(t, DataClassJsonMixin):
             raise AssertionError(
@@ -364,15 +363,15 @@
         if get_origin(python_type) is list:
             return typing.List[self._get_origin_type_in_annotation(get_args(python_type)[0])]  # type: ignore
         elif get_origin(python_type) is dict:
             return typing.Dict[  # type: ignore
                 self._get_origin_type_in_annotation(get_args(python_type)[0]),
                 self._get_origin_type_in_annotation(get_args(python_type)[1]),
             ]
-        elif get_origin(python_type) is Annotated:
+        elif is_annotated(python_type):
             return get_args(python_type)[0]
         elif dataclasses.is_dataclass(python_type):
             for field in dataclasses.fields(copy.deepcopy(python_type)):
                 field.type = self._get_origin_type_in_annotation(field.type)
         return python_type
 
     def _fix_structured_dataset_type(self, python_type: Type[T], python_val: typing.Any) -> T:
@@ -733,30 +732,30 @@
             TODO lets make this deterministic by using an ordered dict
 
         Step 5:
             if v is of type data class, use the dataclass transformer
         """
         cls.lazy_import_transformers()
         # Step 1
-        if get_origin(python_type) is Annotated:
+        if is_annotated(python_type):
             args = get_args(python_type)
             for annotation in args:
                 if isinstance(annotation, TypeTransformer):
                     return annotation
 
             python_type = args[0]
 
         if python_type in cls._REGISTRY:
             return cls._REGISTRY[python_type]
 
         # Step 2
         if hasattr(python_type, "__origin__"):
             # Handling of annotated generics, eg:
             # Annotated[typing.List[int], 'foo']
-            if get_origin(python_type) is Annotated:
+            if is_annotated(python_type):
                 return cls.get_transformer(get_args(python_type)[0])
 
             if python_type.__origin__ in cls._REGISTRY:
                 return cls._REGISTRY[python_type.__origin__]
 
             raise ValueError(f"Generic Type {python_type.__origin__} not supported currently in Flytekit.")
 
@@ -819,15 +818,15 @@
     def to_literal_type(cls, python_type: Type) -> LiteralType:
         """
         Converts a python type into a flyte specific ``LiteralType``
         """
         transformer = cls.get_transformer(python_type)
         res = transformer.get_literal_type(python_type)
         data = None
-        if get_origin(python_type) is Annotated:
+        if is_annotated(python_type):
             for x in get_args(python_type)[1:]:
                 if not isinstance(x, FlyteAnnotation):
                     continue
                 if data is not None:
                     raise ValueError(
                         f"More than one FlyteAnnotation used within {python_type} typehint. Flytekit requires a max of one."
                     )
@@ -847,17 +846,17 @@
             raise TypeTransformerFailedError(f"Python value cannot be None, expected {python_type}/{expected}")
         transformer = cls.get_transformer(python_type)
         if transformer.type_assertions_enabled:
             transformer.assert_type(python_type, python_val)
 
         # In case the value is an annotated type we inspect the annotations and look for hash-related annotations.
         hash = None
-        if get_origin(python_type) is Annotated:
+        if is_annotated(python_type):
             # We are now dealing with one of two cases:
-            # 1. The annotated type is a `HashMethod`, which indicates that we should we should produce the hash using
+            # 1. The annotated type is a `HashMethod`, which indicates that we should produce the hash using
             #    the method indicated in the annotation.
             # 2. The annotated type is being used for a different purpose other than calculating hash values, in which case
             #    we should just continue.
             for annotation in get_args(python_type)[1:]:
                 if not isinstance(annotation, HashMethod):
                     continue
                 hash = annotation.calculate(python_val)
@@ -876,15 +875,15 @@
         """
         transformer = cls.get_transformer(expected_python_type)
         return transformer.to_python_value(ctx, lv, expected_python_type)
 
     @classmethod
     def to_html(cls, ctx: FlyteContext, python_val: typing.Any, expected_python_type: Type[typing.Any]) -> str:
         transformer = cls.get_transformer(expected_python_type)
-        if get_origin(expected_python_type) is Annotated:
+        if is_annotated(expected_python_type):
             expected_python_type, *annotate_args = get_args(expected_python_type)
             from flytekit.deck.renderer import Renderable
 
             for arg in annotate_args:
                 if isinstance(arg, Renderable):
                     return arg.to_html(python_val)
         return transformer.to_html(ctx, python_val, expected_python_type)
@@ -1000,15 +999,15 @@
     def get_sub_type(t: Type[T]) -> Type[T]:
         """
         Return the generic Type T of the List
         """
         if hasattr(t, "__origin__"):
             # Handle annotation on list generic, eg:
             # Annotated[typing.List[int], 'foo']
-            if get_origin(t) is Annotated:
+            if is_annotated(t):
                 return ListTransformer.get_sub_type(get_args(t)[0])
 
             if getattr(t, "__origin__") is list and hasattr(t, "__args__"):
                 return getattr(t, "__args__")[0]
 
         raise ValueError("Only generic univariate typing.List[T] type is supported.")
 
@@ -1026,15 +1025,15 @@
     def is_batchable(t: Type):
         """
         This function evaluates whether the provided type is batchable or not.
         It returns True only if the type is either List or Annotated(List) and the List subtype is FlytePickle.
         """
         from flytekit.types.pickle import FlytePickle
 
-        if get_origin(t) is Annotated:
+        if is_annotated(t):
             return ListTransformer.is_batchable(get_args(t)[0])
         if get_origin(t) is list:
             subtype = get_args(t)[0]
             if subtype == FlytePickle or (hasattr(subtype, "__origin__") and subtype.__origin__ == FlytePickle):
                 return True
         return False
 
@@ -1043,15 +1042,15 @@
             raise TypeTransformerFailedError("Expected a list")
 
         if ListTransformer.is_batchable(python_type):
             from flytekit.types.pickle.pickle import BatchSize, FlytePickle
 
             batch_size = len(python_val)  # default batch size
             # parse annotated to get the number of items saved in a pickle file.
-            if get_origin(python_type) is Annotated:
+            if is_annotated(python_type):
                 for annotation in get_args(python_type)[1:]:
                     if isinstance(annotation, BatchSize):
                         batch_size = annotation.val
                         break
             if batch_size > 0:
                 lit_list = [TypeEngine.to_literal(ctx, python_val[i : i + batch_size], FlytePickle, expected.collection_type) for i in range(0, len(python_val), batch_size)]  # type: ignore
             else:
@@ -1187,31 +1186,29 @@
     def get_sub_type_in_optional(t: Type[T]) -> Type[T]:
         """
         Return the generic Type T of the Optional type
         """
         return get_args(t)[0]
 
     def get_literal_type(self, t: Type[T]) -> Optional[LiteralType]:
-        if get_origin(t) is Annotated:
-            t = get_args(t)[0]
+        t = get_underlying_type(t)
 
         try:
             trans: typing.List[typing.Tuple[TypeTransformer, typing.Any]] = [
                 (TypeEngine.get_transformer(x), x) for x in get_args(t)
             ]
             # must go through TypeEngine.to_literal_type instead of trans.get_literal_type
             # to handle Annotated
             variants = [_add_tag_to_type(TypeEngine.to_literal_type(x), t.name) for (t, x) in trans]
             return _type_models.LiteralType(union_type=UnionType(variants))
         except Exception as e:
             raise ValueError(f"Type of Generic Union type is not supported, {e}")
 
     def to_literal(self, ctx: FlyteContext, python_val: T, python_type: Type[T], expected: LiteralType) -> Literal:
-        if get_origin(python_type) is Annotated:
-            python_type = get_args(python_type)[0]
+        python_type = get_underlying_type(python_type)
 
         found_res = False
         res = None
         res_type = None
         for t in get_args(python_type):
             try:
                 trans: TypeTransformer[T] = TypeEngine.get_transformer(t)
@@ -1228,16 +1225,15 @@
 
         if found_res:
             return Literal(scalar=Scalar(union=Union(value=res, stored_type=res_type)))
 
         raise TypeTransformerFailedError(f"Cannot convert from {python_val} to {python_type}")
 
     def to_python_value(self, ctx: FlyteContext, lv: Literal, expected_python_type: Type[T]) -> Optional[typing.Any]:
-        if get_origin(expected_python_type) is Annotated:
-            expected_python_type = get_args(expected_python_type)[0]
+        expected_python_type = get_underlying_type(expected_python_type)
 
         union_tag = None
         union_type = None
         if lv.scalar is not None and lv.scalar.union is not None:
             union_type = lv.scalar.union.stored_type
             if union_type.structure is not None:
                 union_tag = union_type.structure.tag
@@ -1464,15 +1460,15 @@
     Enables converting a python type enum.Enum to LiteralType.EnumType
     """
 
     def __init__(self):
         super().__init__(name="DefaultEnumTransformer", t=enum.Enum)
 
     def get_literal_type(self, t: Type[T]) -> LiteralType:
-        if get_origin(t) is Annotated:
+        if is_annotated(t):
             raise ValueError(
                 f"Flytekit does not currently have support \
                     for FlyteAnnotations applied to enums. {t} cannot be \
                     parsed."
             )
 
         values = [v.value for v in t]  # type: ignore
@@ -1778,7 +1774,18 @@
             self._ctx or FlyteContext.current_context(), self._literals[attr], cast(Type, as_type)
         )
         self._native_values[attr] = val
         return val
 
 
 _register_default_type_transformers()
+
+
+def is_annotated(t: Type) -> bool:
+    return get_origin(t) is Annotated
+
+
+def get_underlying_type(t: Type) -> Type:
+    """Return the underlying type for annotated types or the type itself"""
+    if is_annotated(t):
+        return get_args(t)[0]
+    return t
```

### Comparing `flytekit-1.6.1b0/flytekit/core/type_helpers.py` & `flytekit-1.6.2/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/utils.py` & `flytekit-1.6.2/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/core/workflow.py` & `flytekit-1.6.2/flytekit/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/deck/deck.py` & `flytekit-1.6.2/flytekit/deck/deck.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import typing
 from typing import Optional
 
 from flytekit.core.context_manager import ExecutionParameters, ExecutionState, FlyteContext, FlyteContextManager
 from flytekit.loggers import logger
+from flytekit.tools.interactive import ipython_check
 
 OUTPUT_DIR_JUPYTER_PREFIX = "jupyter"
 DECK_FILE_NAME = "deck.html"
 
 
 class Deck:
     """
@@ -120,40 +121,24 @@
             df[["Name", "WallTime", "ProcessTime"]],
             header_labels=["Name", "Wall Time(s)", "Process Time(s)"],
             table_width=width,
         )
         return gantt_chart_html + time_table_html + note
 
 
-def _ipython_check() -> bool:
-    """
-    Check if interface is launching from iPython (not colab)
-    :return is_ipython (bool): True or False
-    """
-    is_ipython = False
-    try:  # Check if running interactively using ipython.
-        from IPython import get_ipython
-
-        if get_ipython() is not None:
-            is_ipython = True
-    except (ImportError, NameError):
-        pass
-    return is_ipython
-
-
 def _get_deck(
     new_user_params: ExecutionParameters, ignore_jupyter: bool = False
 ) -> typing.Union[str, "IPython.core.display.HTML"]:  # type:ignore
     """
     Get flyte deck html string
     If ignore_jupyter is set to True, then it will return a str even in a jupyter environment.
     """
     deck_map = {deck.name: deck.html for deck in new_user_params.decks}
     raw_html = get_deck_template().render(metadata=deck_map)
-    if not ignore_jupyter and _ipython_check():
+    if not ignore_jupyter and ipython_check():
         try:
             from IPython.core.display import HTML
         except ImportError:
             ...
         return HTML(raw_html)
     return raw_html
```

### Comparing `flytekit-1.6.1b0/flytekit/deck/html/template.html` & `flytekit-1.6.2/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/deck/renderer.py` & `flytekit-1.6.2/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/exceptions/scopes.py` & `flytekit-1.6.2/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/exceptions/system.py` & `flytekit-1.6.2/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/exceptions/user.py` & `flytekit-1.6.2/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extend/__init__.py` & `flytekit-1.6.2/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extend/backend/base_plugin.py` & `flytekit-1.6.2/flytekit/extend/backend/base_plugin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extend/backend/external_plugin_service.py` & `flytekit-1.6.2/flytekit/extend/backend/external_plugin_service.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.6.2/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extras/pytorch/__init__.py` & `flytekit-1.6.2/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.6.2/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extras/pytorch/native.py` & `flytekit-1.6.2/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extras/sklearn/__init__.py` & `flytekit-1.6.2/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extras/sklearn/native.py` & `flytekit-1.6.2/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extras/sqlite3/task.py` & `flytekit-1.6.2/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extras/tasks/shell.py` & `flytekit-1.6.2/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.6.2/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extras/tensorflow/model.py` & `flytekit-1.6.2/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/extras/tensorflow/record.py` & `flytekit-1.6.2/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/image_spec/image_spec.py` & `flytekit-1.6.2/flytekit/image_spec/image_spec.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/interaction/parse_stdin.py` & `flytekit-1.6.2/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.6.2/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/interfaces/random.py` & `flytekit-1.6.2/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/interfaces/stats/client.py` & `flytekit-1.6.2/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/interfaces/stats/taggable.py` & `flytekit-1.6.2/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/lazy_import/lazy_module.py` & `flytekit-1.6.2/flytekit/lazy_import/lazy_module.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/loggers.py` & `flytekit-1.6.2/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/admin/common.py` & `flytekit-1.6.2/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/admin/task_execution.py` & `flytekit-1.6.2/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/admin/workflow.py` & `flytekit-1.6.2/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/annotation.py` & `flytekit-1.6.2/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/array_job.py` & `flytekit-1.6.2/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/common.py` & `flytekit-1.6.2/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/core/catalog.py` & `flytekit-1.6.2/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/core/compiler.py` & `flytekit-1.6.2/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/core/condition.py` & `flytekit-1.6.2/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/core/errors.py` & `flytekit-1.6.2/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/core/execution.py` & `flytekit-1.6.2/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/core/identifier.py` & `flytekit-1.6.2/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/core/types.py` & `flytekit-1.6.2/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/core/workflow.py` & `flytekit-1.6.2/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/documentation.py` & `flytekit-1.6.2/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/dynamic_job.py` & `flytekit-1.6.2/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/execution.py` & `flytekit-1.6.2/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/filters.py` & `flytekit-1.6.2/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/interface.py` & `flytekit-1.6.2/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/launch_plan.py` & `flytekit-1.6.2/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/literals.py` & `flytekit-1.6.2/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/matchable_resource.py` & `flytekit-1.6.2/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/named_entity.py` & `flytekit-1.6.2/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/node_execution.py` & `flytekit-1.6.2/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/presto.py` & `flytekit-1.6.2/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/project.py` & `flytekit-1.6.2/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/qubole.py` & `flytekit-1.6.2/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/schedule.py` & `flytekit-1.6.2/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/security.py` & `flytekit-1.6.2/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/task.py` & `flytekit-1.6.2/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/types.py` & `flytekit-1.6.2/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/models/workflow_closure.py` & `flytekit-1.6.2/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/remote/__init__.py` & `flytekit-1.6.2/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/remote/backfill.py` & `flytekit-1.6.2/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/remote/entities.py` & `flytekit-1.6.2/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/remote/executions.py` & `flytekit-1.6.2/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/remote/lazy_entity.py` & `flytekit-1.6.2/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/remote/remote.py` & `flytekit-1.6.2/flytekit/remote/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from dataclasses import asdict, dataclass
 from datetime import datetime, timedelta
 
 import requests
 from flyteidl.admin.signal_pb2 import Signal, SignalListRequest, SignalSetRequest
 from flyteidl.core import literals_pb2 as literals_pb2
 
-from flytekit import Literal
 from flytekit.clients.friendly import SynchronousFlyteClient
 from flytekit.clients.helpers import iterate_node_executions, iterate_task_executions
 from flytekit.configuration import Config, FastSerializationSettings, ImageConfig, SerializationSettings
 from flytekit.core import constants, utils
 from flytekit.core.base_task import PythonTask
 from flytekit.core.context_manager import FlyteContext, FlyteContextManager
 from flytekit.core.data_persistence import FileAccessProvider
@@ -57,30 +56,37 @@
 from flytekit.models.execution import (
     ExecutionMetadata,
     ExecutionSpec,
     NodeExecutionGetDataResponse,
     NotificationList,
     WorkflowExecutionGetDataResponse,
 )
+from flytekit.models.literals import Literal, LiteralMap
 from flytekit.remote.backfill import create_backfill_workflow
 from flytekit.remote.entities import FlyteLaunchPlan, FlyteNode, FlyteTask, FlyteTaskNode, FlyteWorkflow
 from flytekit.remote.executions import FlyteNodeExecution, FlyteTaskExecution, FlyteWorkflowExecution
 from flytekit.remote.interface import TypedInterface
 from flytekit.remote.lazy_entity import LazyEntity
 from flytekit.remote.remote_callable import RemoteEntity
 from flytekit.tools.fast_registration import fast_package
+from flytekit.tools.interactive import ipython_check
 from flytekit.tools.script_mode import compress_scripts, hash_file
 from flytekit.tools.translator import (
     FlyteControlPlaneEntity,
     FlyteLocalEntity,
     Options,
     get_serializable,
     get_serializable_launch_plan,
 )
 
+try:
+    from IPython.core.display import HTML
+except ImportError:
+    ...
+
 ExecutionDataResponse = typing.Union[WorkflowExecutionGetDataResponse, NodeExecutionGetDataResponse]
 
 MOST_RECENT_FIRST = admin_common_models.Sort("created_at", admin_common_models.Sort.Direction.DESCENDING)
 
 
 class RegistrationSkipped(Exception):
     """
@@ -215,14 +221,56 @@
         return self._config
 
     @property
     def file_access(self) -> FileAccessProvider:
         """File access provider to use for offloading non-literal inputs/outputs."""
         return self._file_access
 
+    def get(
+        self, flyte_uri: typing.Optional[str] = None
+    ) -> typing.Optional[typing.Union[LiteralsResolver, Literal, HTML, bytes]]:
+        """
+        General function that works with flyte tiny urls. This can return outputs (in the form of LiteralsResolver, or
+        individual Literals for singular requests), or HTML if passed a deck link, or bytes containing HTML,
+        if ipython is not available locally.
+        """
+        if flyte_uri is None:
+            raise user_exceptions.FlyteUserException("flyte_uri cannot be empty")
+        ctx = self._ctx or FlyteContextManager.current_context()
+        try:
+            data_response = self.client.get_data(flyte_uri)
+
+            if data_response.HasField("literal_map"):
+                lm = LiteralMap.from_flyte_idl(data_response.literal_map)
+                return LiteralsResolver(lm.literals)
+            elif data_response.HasField("literal"):
+                return data_response.literal
+            elif data_response.HasField("pre_signed_urls"):
+                if len(data_response.pre_signed_urls.signed_url) == 0:
+                    raise ValueError(f"Flyte url {flyte_uri} resolved to empty download link")
+                d = data_response.pre_signed_urls.signed_url[0]
+                remote_logger.debug(f"Download link is {d}")
+                fs = ctx.file_access.get_filesystem_for_path(d)
+
+                # If the venv has IPython, then return IPython's HTML
+                if ipython_check():
+                    remote_logger.debug(f"IPython found, returning HTML from {flyte_uri}")
+                    with fs.open(d, "rb") as r:
+                        html = HTML(str(r.read()))
+                        return html
+                # If not return bytes
+                else:
+                    remote_logger.debug(f"IPython not found, returning HTML as bytes from {flyte_uri}")
+                    return fs.open(d, "rb").read()
+
+        except user_exceptions.FlyteUserException as e:
+            remote_logger.info(f"Error from Flyte backend when trying to fetch data: {e.__cause__}")
+
+        remote_logger.info(f"Nothing found from {flyte_uri}")
+
     def remote_context(self):
         """Context manager with remote-specific configuration."""
         return FlyteContextManager.with_context(
             FlyteContextManager.current_context().with_file_access(self.file_access)
         )
 
     def fetch_task_lazy(
@@ -743,14 +791,17 @@
         with open(str(to_upload), "+rb") as local_file:
             content = local_file.read()
             content_length = len(content)
             rsp = requests.put(
                 upload_location.signed_url,
                 data=content,
                 headers={"Content-Length": str(content_length), "Content-MD5": encoded_md5},
+                verify=False
+                if self._config.platform.insecure_skip_verify is True
+                else self._config.platform.ca_cert_file_path,
             )
 
             if rsp.status_code != requests.codes["OK"]:
                 raise FlyteValueException(
                     rsp.status_code,
                     f"Request to send data {upload_location.signed_url} failed.",
                 )
```

### Comparing `flytekit-1.6.1b0/flytekit/remote/remote_callable.py` & `flytekit-1.6.2/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/testing/__init__.py` & `flytekit-1.6.2/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/tools/fast_registration.py` & `flytekit-1.6.2/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/tools/ignore.py` & `flytekit-1.6.2/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/tools/module_loader.py` & `flytekit-1.6.2/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/tools/repo.py` & `flytekit-1.6.2/flytekit/tools/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,28 +250,28 @@
     b = serialization_settings.new_builder()
     b.version = version
     serialization_settings = b.build()
 
     options = Options.default_from(k8s_service_account=service_account, raw_data_prefix=raw_data_prefix)
 
     # Load all the entities
-    serializable_entities = load_packages_and_modules(
+    registrable_entities = load_packages_and_modules(
         serialization_settings, detected_root, list(package_or_module), options
     )
-    if len(serializable_entities) == 0:
+    if len(registrable_entities) == 0:
         click.secho("No Flyte entities were detected. Aborting!", fg="red")
         return
 
-    for cp_entity in serializable_entities:
+    for cp_entity in registrable_entities:
         og_id = cp_entity.id if isinstance(cp_entity, launch_plan.LaunchPlan) else cp_entity.template.id
         secho(og_id, "")
         try:
             if not dry_run:
                 i = remote.raw_register(
                     cp_entity, serialization_settings, version=version, create_default_launchplan=False
                 )
                 secho(i)
             else:
                 secho(og_id, reason="Dry run Mode!")
         except RegistrationSkipped:
             secho(og_id, "failed")
-    click.secho(f"Successfully registered {len(serializable_entities)} entities", fg="green")
+    click.secho(f"Successfully registered {len(registrable_entities)} entities", fg="green")
```

### Comparing `flytekit-1.6.1b0/flytekit/tools/script_mode.py` & `flytekit-1.6.2/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/tools/serialize_helpers.py` & `flytekit-1.6.2/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/tools/subprocess.py` & `flytekit-1.6.2/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/tools/translator.py` & `flytekit-1.6.2/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/types/directory/__init__.py` & `flytekit-1.6.2/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/types/directory/types.py` & `flytekit-1.6.2/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/types/file/__init__.py` & `flytekit-1.6.2/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/types/file/file.py` & `flytekit-1.6.2/flytekit/types/file/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 import pathlib
 import typing
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 
 from dataclasses_json import config, dataclass_json
 from marshmallow import fields
-from typing_extensions import Annotated, get_args, get_origin
 
 from flytekit.core.context_manager import FlyteContext, FlyteContextManager
-from flytekit.core.type_engine import TypeEngine, TypeTransformer, TypeTransformerFailedError
+from flytekit.core.type_engine import TypeEngine, TypeTransformer, TypeTransformerFailedError, get_underlying_type
 from flytekit.loggers import logger
 from flytekit.models.core.types import BlobType
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
 from flytekit.types.pickle.pickle import FlytePickleTransformer
 
 
@@ -333,16 +332,15 @@
         remote_path = None
         should_upload = True
 
         if python_val is None:
             raise TypeTransformerFailedError("None value cannot be converted to a file.")
 
         # Correctly handle `Annotated[FlyteFile, ...]` by extracting the origin type
-        if get_origin(python_type) is Annotated:
-            python_type = get_args(python_type)[0]
+        python_type = get_underlying_type(python_type)
 
         if not (python_type is os.PathLike or issubclass(python_type, FlyteFile)):
             raise ValueError(f"Incorrect type {python_type}, must be either a FlyteFile or os.PathLike")
 
         # information used by all cases
         meta = BlobMetadata(type=self._blob_type(format=FlyteFilePathTransformer.get_format(python_type)))
 
@@ -409,14 +407,17 @@
         except AttributeError:
             raise TypeTransformerFailedError(f"Cannot convert from {lv} to {expected_python_type}")
         # In this condition, we still return a FlyteFile instance, but it's a simple one that has no downloading tricks
         # Using is instead of issubclass because FlyteFile does actually subclass it
         if expected_python_type is os.PathLike:
             return FlyteFile(uri)
 
+        # Correctly handle `Annotated[FlyteFile, ...]` by extracting the origin type
+        expected_python_type = get_underlying_type(expected_python_type)
+
         # The rest of the logic is only for FlyteFile types.
         if not issubclass(expected_python_type, FlyteFile):  # type: ignore
             raise TypeError(f"Neither os.PathLike nor FlyteFile specified {expected_python_type}")
 
         # This is a local file path, like /usr/local/my_file, don't mess with it. Certainly, downloading it doesn't
         # make any sense.
         if not ctx.file_access.is_remote(uri):
```

### Comparing `flytekit-1.6.1b0/flytekit/types/numpy/ndarray.py` & `flytekit-1.6.2/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/types/pickle/pickle.py` & `flytekit-1.6.2/flytekit/types/pickle/pickle.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/types/schema/types.py` & `flytekit-1.6.2/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/types/schema/types_pandas.py` & `flytekit-1.6.2/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/types/structured/__init__.py` & `flytekit-1.6.2/flytekit/types/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/types/structured/basic_dfs.py` & `flytekit-1.6.2/flytekit/types/structured/basic_dfs.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/types/structured/bigquery.py` & `flytekit-1.6.2/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit/types/structured/structured_dataset.py` & `flytekit-1.6.2/flytekit/types/structured/structured_dataset.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/flytekit.egg-info/PKG-INFO` & `flytekit-1.6.2/flytekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.1b0
+Version: 1.6.2
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.1b0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.2 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.1b0/flytekit.egg-info/SOURCES.txt` & `flytekit-1.6.2/flytekit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -179,14 +179,15 @@
 flytekit/remote/lazy_entity.py
 flytekit/remote/remote.py
 flytekit/remote/remote_callable.py
 flytekit/testing/__init__.py
 flytekit/tools/__init__.py
 flytekit/tools/fast_registration.py
 flytekit/tools/ignore.py
+flytekit/tools/interactive.py
 flytekit/tools/module_loader.py
 flytekit/tools/repo.py
 flytekit/tools/script_mode.py
 flytekit/tools/serialize_helpers.py
 flytekit/tools/subprocess.py
 flytekit/tools/translator.py
 flytekit/types/__init__.py
```

### Comparing `flytekit-1.6.1b0/flytekit.egg-info/requires.txt` & `flytekit-1.6.2/flytekit.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 googleapis-common-protos>=1.57
-flyteidl>=1.5.4
+flyteidl>=1.5.6
 wheel<1.0.0,>=0.30.0
 pandas<2.0.0,>=1.0.0
 pyarrow<11.0.0,>=4.0.0
 click<9.0,>=6.6
 croniter<4.0.0,>=0.3.20
 deprecated<2.0,>=1.0
 docker<7.0.0,>=4.0.0
 python-dateutil>=2.1
-grpcio<2.0,>=1.50.0
-grpcio-status<2.0,>=1.50.0
+grpcio!=1.55.0,<2.0,>=1.50.0
+grpcio-status!=1.55.0,<2.0,>=1.50.0
 importlib-metadata
 fsspec>=2023.3.0
 adlfs
 s3fs>=0.6.0
 gcsfs
 pyopenssl
 joblib
@@ -38,10 +38,7 @@
 cloudpickle>=2.0.0
 cookiecutter>=1.7.3
 numpy
 gitpython
 kubernetes>=12.0.1
 rich
 rich_click
-
-[:python_version < "3.8.0"]
-singledispatchmethod
```

### Comparing `flytekit-1.6.1b0/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.6.2/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.1b0/setup.py` & `flytekit-1.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.6.1b0"
+__version__ = "1.6.2"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
@@ -25,27 +25,27 @@
             "pyflyte-map-execute=flytekit.bin.entrypoint:map_execute_task_cmd",
             "pyflyte=flytekit.clis.sdk_in_container.pyflyte:main",
             "flyte-cli=flytekit.clis.flyte_cli.main:_flyte_cli",
         ]
     },
     install_requires=[
         "googleapis-common-protos>=1.57",
-        "flyteidl>=1.5.4",
+        "flyteidl>=1.5.6",
         "wheel>=0.30.0,<1.0.0",
         "pandas>=1.0.0,<2.0.0",
         "pyarrow>=4.0.0,<11.0.0",
         "click>=6.6,<9.0",
         "croniter>=0.3.20,<4.0.0",
         "deprecated>=1.0,<2.0",
         "docker>=4.0.0,<7.0.0",
         "python-dateutil>=2.1",
         # Restrict grpcio and grpcio-status.  Version 1.50.0 pulls in a version of protobuf that is not compatible
         # with the old protobuf library (as described in https://developers.google.com/protocol-buffers/docs/news/2022-05-06)
-        "grpcio>=1.50.0,<2.0",
-        "grpcio-status>=1.50.0,<2.0",
+        "grpcio>=1.50.0,!=1.55.0,<2.0",
+        "grpcio-status>=1.50.0,!=1.55.0,<2.0",
         "importlib-metadata",
         "fsspec>=2023.3.0",
         "adlfs",
         "s3fs>=0.6.0",
         "gcsfs",
         "pyopenssl",
         "joblib",
@@ -60,15 +60,14 @@
         "statsd>=3.0.0,<4.0.0",
         "urllib3>=1.22,<2.0.0",
         "wrapt>=1.0.0,<2.0.0",
         "dataclasses-json>=0.5.2",
         "marshmallow-jsonschema>=0.12.0",
         "natsort>=7.0.1",
         "docker-image-py>=0.1.10",
-        "singledispatchmethod; python_version < '3.8.0'",
         "typing_extensions",
         "docstring-parser>=0.9.0",
         "diskcache>=5.2.1",
         "cloudpickle>=2.0.0",
         "cookiecutter>=1.7.3",
         "numpy",
         "gitpython",
```

