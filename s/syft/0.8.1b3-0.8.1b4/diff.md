# Comparing `tmp/syft-0.8.1b3.tar.gz` & `tmp/syft-0.8.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.1b3.tar", last modified: Sun May 21 12:44:53 2023, max compression
+gzip compressed data, was "syft-0.8.1b4.tar", last modified: Tue May 30 06:02:09 2023, max compression
```

## Comparing `syft-0.8.1b3.tar` & `syft-0.8.1b4.tar`

### file list

```diff
@@ -1,192 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.624683 syft-0.8.1b3/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-05-21 12:41:56.000000 syft-0.8.1b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 12:41:56.000000 syft-0.8.1b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-21 12:44:53.624683 syft-0.8.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-21 12:41:55.000000 syft-0.8.1b3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-21 12:41:56.000000 syft-0.8.1b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-21 12:44:53.628682 syft-0.8.1b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-21 12:41:56.000000 syft-0.8.1b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.588681 syft-0.8.1b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.592681 syft-0.8.1b3/src/syft/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-21 12:42:13.000000 syft-0.8.1b3/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-21 12:42:13.000000 syft-0.8.1b3/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.596681 syft-0.8.1b3/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.596681 syft-0.8.1b3/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24303 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.588681 syft-0.8.1b3/src/syft/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.588681 syft-0.8.1b3/src/syft/core/node/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.596681 syft-0.8.1b3/src/syft/core/node/new/
--rw-r--r--   0 runner    (1001) docker     (123)    26990 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/core/node/new/action_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.596681 syft-0.8.1b3/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.600682 syft-0.8.1b3/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15930 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.604682 syft-0.8.1b3/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.604682 syft-0.8.1b3/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/third_party.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.604682 syft-0.8.1b3/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.608682 syft-0.8.1b3/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    46598 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27045 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.608682 syft-0.8.1b3/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    21458 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.612682 syft-0.8.1b3/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.612682 syft-0.8.1b3/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.612682 syft-0.8.1b3/src/syft/service/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/message/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/message/message_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/message/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.612682 syft-0.8.1b3/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/metadata/metadata_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.612682 syft-0.8.1b3/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (123)    20283 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/network/network_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.616682 syft-0.8.1b3/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.616682 syft-0.8.1b3/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22709 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.616682 syft-0.8.1b3/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.616682 syft-0.8.1b3/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.616682 syft-0.8.1b3/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.620682 syft-0.8.1b3/src/syft/service/vpn/
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/vpn/headscale_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/vpn/tailscale_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/vpn/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.620682 syft-0.8.1b3/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.624683 syft-0.8.1b3/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.624683 syft-0.8.1b3/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23269 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.596681 syft-0.8.1b3/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.360423 syft-0.8.1b4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-05-30 05:59:36.000000 syft-0.8.1b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 05:59:36.000000 syft-0.8.1b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-30 06:02:09.360423 syft-0.8.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-30 05:59:36.000000 syft-0.8.1b4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-30 05:59:36.000000 syft-0.8.1b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-30 06:02:09.360423 syft-0.8.1b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-30 05:59:36.000000 syft-0.8.1b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.320423 syft-0.8.1b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.324422 syft-0.8.1b4/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-30 05:59:49.000000 syft-0.8.1b4/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-30 05:59:49.000000 syft-0.8.1b4/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.328423 syft-0.8.1b4/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.328423 syft-0.8.1b4/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24407 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23720 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.328423 syft-0.8.1b4/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.332423 syft-0.8.1b4/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15930 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.332423 syft-0.8.1b4/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28362 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.336423 syft-0.8.1b4/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/third_party.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.336423 syft-0.8.1b4/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.340423 syft-0.8.1b4/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46765 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26970 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.340423 syft-0.8.1b4/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22217 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.344423 syft-0.8.1b4/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.344423 syft-0.8.1b4/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.344423 syft-0.8.1b4/src/syft/service/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/message/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/message/message_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/message/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.344423 syft-0.8.1b4/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.344423 syft-0.8.1b4/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/network/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/network/node_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/network/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.348423 syft-0.8.1b4/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21242 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.348423 syft-0.8.1b4/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42329 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.348423 syft-0.8.1b4/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.348423 syft-0.8.1b4/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.348423 syft-0.8.1b4/src/syft/service/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.352423 syft-0.8.1b4/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.352423 syft-0.8.1b4/src/syft/service/vpn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/vpn/headscale_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/vpn/tailscale_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/vpn/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.352423 syft-0.8.1b4/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.356423 syft-0.8.1b4/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18931 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.360423 syft-0.8.1b4/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23579 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.328423 syft-0.8.1b4/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.1b3/LICENSE` & `syft-0.8.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/PKG-INFO` & `syft-0.8.1b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b3
+Version: 0.8.1b4
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b3 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b4 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.1b3/README.md` & `syft-0.8.1b4/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/setup.cfg` & `syft-0.8.1b4/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.1-beta.3"
+version = attr: "0.8.1-beta.4"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -29,15 +29,15 @@
 	forbiddenfruit==0.1.4
 	gevent==22.10.2
 	gipc==1.5.0
 	jax==0.3.14
 	jaxlib==0.3.14
 	loguru==0.7.0
 	networkx==2.8
-	numpy==1.24.2
+	numpy==1.24.3
 	opendp==0.6.2
 	packaging>=21.0
 	pandas==1.5.3
 	pyarrow==11.0.0
 	pycapnp==1.3.0
 	pydantic[email]==1.10.7
 	pymongo==4.3.3
```

### Comparing `syft-0.8.1b3/src/syft/VERSION` & `syft-0.8.1b4/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.1-beta.3"
+__version__ = "0.8.1-beta.4"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.1b3/src/syft/__init__.py` & `syft-0.8.1b4/src/syft/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.1-beta.3"
+__version__ = "0.8.1-beta.4"
 
 # stdlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
 
@@ -25,14 +25,15 @@
 from .node.server import serve_node  # noqa: F401
 from .node.server import serve_node as bind_worker  # noqa: F401
 from .node.worker import Worker  # noqa: F401
 from .serde import NOTHING  # noqa: F401
 from .serde.deserialize import _deserialize as deserialize  # noqa: F401
 from .serde.serializable import serializable  # noqa: F401
 from .serde.serialize import _serialize as serialize  # noqa: F401
+from .service.action.action_data_empty import ActionDataEmpty  # noqa: F401
 from .service.action.action_object import ActionObject  # noqa: F401
 from .service.action.plan import Plan  # noqa: F401
 from .service.action.plan import planify  # noqa: F401
 from .service.code.user_code import UserCodeStatus  # noqa: F401
 from .service.code.user_code import syft_function  # noqa: F401
 from .service.data_subject import DataSubjectCreate as DataSubject  # noqa: F401
 from .service.dataset.dataset import CreateAsset as Asset  # noqa: F401
```

### Comparing `syft-0.8.1b3/src/syft/abstract_node.py` & `syft-0.8.1b4/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/client/api.py` & `syft-0.8.1b4/src/syft/client/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def set_api_for(cls, node_uid: Union[UID, str], api: SyftAPI) -> None:
         if isinstance(node_uid, str):
             node_uid = UID.from_string(node_uid)
         cls.__api_registry__[node_uid] = api
 
     @classmethod
     def api_for(cls, node_uid: UID) -> SyftAPI:
-        return cls.__api_registry__[node_uid]
+        return cls.__api_registry__.get(node_uid, None)
 
     @classmethod
     def get_all_api(cls) -> List[SyftAPI]:
         return list(cls.__api_registry__.values())
 
 
 @serializable()
@@ -318,15 +318,18 @@
         if isinstance(key, int) and hasattr(self, "get_all"):
             return self.get_all()[key]
         raise NotImplementedError
 
     def _repr_html_(self) -> Any:
         if not hasattr(self, "get_all"):
             return NotImplementedError
-        results = self.get_all()
+        if hasattr(self, "get_all_unread"):
+            results = self.get_all_unread()
+        else:
+            results = self.get_all()
         return results._repr_html_()
 
 
 @instrument
 @serializable(attrs=["endpoints", "node_uid", "node_name", "lib_endpoints"])
 class SyftAPI(SyftObject):
     # version
@@ -591,15 +594,15 @@
         return None
 
 
 def monkey_patch_getdef(self, obj, oname="") -> Union[str, None]:
     try:
         if hasattr(obj, "__ipython_inspector_signature_override__"):
             return _render_signature(
-                getattr(obj, "__ipython_inspector_signature_override__"), oname
+                obj.__ipython_inspector_signature_override__, oname
             )
         return _getdef(self, obj, oname)
     except Exception:
         return None
 
 
 # try to monkeypatch IPython
```

### Comparing `syft-0.8.1b3/src/syft/client/client.py` & `syft-0.8.1b4/src/syft/client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # stdlib
 from enum import Enum
 import hashlib
 import json
 from typing import Any
-from typing import Callable
 from typing import Dict
 from typing import Optional
 from typing import Type
 from typing import Union
 from typing import cast
 
 # third party
@@ -19,31 +18,34 @@
 from tqdm import tqdm
 from typing_extensions import Self
 
 # relative
 from .. import __version__
 from ..abstract_node import AbstractNode
 from ..node.credentials import SyftSigningKey
+from ..node.credentials import SyftVerifyKey
 from ..node.credentials import UserLoginCredentials
 from ..serde.deserialize import _deserialize
 from ..serde.serializable import serializable
 from ..serde.serialize import _serialize
 from ..service.context import NodeServiceContext
 from ..service.dataset.dataset import CreateDataset
+from ..service.metadata.node_metadata import NodeMetadata
 from ..service.metadata.node_metadata import NodeMetadataJSON
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
 from ..service.user.user import UserCreate
 from ..service.user.user import UserPrivateKey
 from ..service.user.user_service import UserService
 from ..types.grid_url import GridURL
 from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.uid import UID
 from ..util.logger import debug
 from ..util.telemetry import instrument
+from ..util.util import thread_ident
 from ..util.util import verify_tls
 from .api import APIModule
 from .api import APIRegistry
 from .api import SignedSyftAPICall
 from .api import SyftAPI
 from .api import SyftAPICall
 from .connection import NodeConnection
@@ -61,15 +63,15 @@
             debug(f"GridURL Upgraded to HTTPS. {https_url}")
             return https_url
     except Exception as e:
         print(f"Failed to upgrade to HTTPS. {e}")
     return url
 
 
-API_PATH = "/api/v1/new"
+API_PATH = "/api/v2"
 
 
 class Routes(Enum):
     ROUTE_METADATA = f"{API_PATH}/metadata"
     ROUTE_API = f"{API_PATH}/api"
     ROUTE_LOGIN = f"{API_PATH}/login"
     ROUTE_REGISTER = f"{API_PATH}/register"
@@ -321,14 +323,20 @@
         if self.metadata is None:
             self._fetch_node_metadata(self.credentials)
 
     @property
     def authed(self) -> bool:
         return bool(self.credentials)
 
+    @property
+    def verify_key(self) -> SyftVerifyKey:
+        if self.credentials is None:
+            raise ValueError("SigningKey not set on client")
+        return self.credentials.verify_key
+
     @staticmethod
     def from_url(url: Union[str, GridURL]) -> Self:
         return SyftClient(connection=HTTPConnection(GridURL.from_url(url)))
 
     @staticmethod
     def from_node(node: AbstractNode) -> Self:
         return SyftClient(connection=PythonConnection(node=node))
@@ -377,47 +385,58 @@
             return self.api.services.dataset.add(dataset=dataset)
         else:
             if len(valid.err()) > 0:
                 return tuple(valid.err())
             return valid.err()
 
     def exchange_route(self, client: Self) -> None:
-        result = self.api.services.network.exchange_credentials_with(client=client)
-        if result:
-            # relative
-            from ..service.network.network_service import connection_to_route
+        # relative
+        from ..service.network.routes import connection_to_route
+
+        self_node_route = connection_to_route(self.connection)
+        remote_node_route = connection_to_route(client.connection)
+
+        result = self.api.services.network.exchange_credentials_with(
+            self_node_route=self_node_route,
+            remote_node_route=remote_node_route,
+            remote_node_verify_key=client.metadata.to(NodeMetadata).verify_key,
+        )
 
-            route = connection_to_route(self.connection)
-            result = self.api.services.network.add_route_for(route=route, client=client)
         return result
 
     def apply_to_gateway(self, client: Self) -> None:
         return self.exchange_route(client)
 
     @property
     def data_subject_registry(self) -> Optional[APIModule]:
         if self.api is not None and hasattr(self.api.services, "data_subject"):
             return self.api.services.data_subject
         return None
 
     @property
+    def users(self) -> Optional[APIModule]:
+        if self.api is not None and hasattr(self.api.services, "user"):
+            return self.api.services.user
+        return None
+
+    @property
     def code(self) -> Optional[APIModule]:
         if self.api is not None and hasattr(self.api.services, "code"):
             return self.api.services.code
 
     @property
-    def datasets(self) -> Optional[APIModule]:
-        if self.api is not None and hasattr(self.api.services, "dataset"):
-            return self.api.services.dataset
+    def requests(self) -> Optional[APIModule]:
+        if self.api is not None and hasattr(self.api.services, "request"):
+            return self.api.services.request
         return None
 
     @property
-    def submit_project(self) -> Callable:
-        if self.api is not None and hasattr(self.api.services, "project"):
-            return self.api.services.project.submit
+    def datasets(self) -> Optional[APIModule]:
+        if self.api is not None and hasattr(self.api.services, "dataset"):
+            return self.api.services.dataset
         return None
 
     @property
     def notifications(self) -> Optional[APIModule]:
         if self.api is not None and hasattr(self.api.services, "messages"):
             return self.api.services.messages
         return None
@@ -436,16 +455,41 @@
             if cache:
                 SyftClientSessionCache.add_client(
                     email=email,
                     password=password,
                     connection=self.connection,
                     syft_client=self,
                 )
+                # Adding another cache storage
+                # as this would be useful in retrieving unique clients
+                # node uid and verify key are not individually unique
+                # both the combination of node uid and verify key are unique
+                # which could be used to identity a client uniquely of any given node
+                # TODO: It would be better to have a single cache storage
+                # combining both email, password and verify key and uid
+                SyftClientSessionCache.add_client_by_uid_and_verify_key(
+                    verify_key=signing_key.verify_key,
+                    node_uid=self.id,
+                    syft_client=self,
+                )
+
+        # relative
+        from ..node.node import CODE_RELOADER
+
+        CODE_RELOADER[thread_ident()] = self._reload_user_code
+
         return self
 
+    def _reload_user_code(self):
+        # relative
+        from ..service.code.user_code import load_approved_policy_code
+
+        user_code_items = self.code.get_all_for_user()
+        load_approved_policy_code(user_code_items)
+
     def register(
         self,
         name: str,
         email: str,
         password: str,
         institution: Optional[str] = None,
         website: Optional[str] = None,
@@ -483,14 +527,26 @@
         connection = self.connection.with_proxy(peer.id)
         client = SyftClient(
             connection=connection,
             credentials=self.credentials,
         )
         return client
 
+    def __getattr__(self, name):
+        if (
+            hasattr(self, "api")
+            and hasattr(self.api, "lib")
+            and hasattr(self.api.lib, name)
+        ):
+            return getattr(self.api.lib, name)
+        else:
+            raise AttributeError(
+                f"{self.__class__.__name__} object has no attribute {name}"
+            )
+
     def __hash__(self) -> int:
         return hash(self.id) + hash(self.connection)
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, SyftClient):
             return False
         return (
@@ -608,14 +664,31 @@
         syft_client: SyftClient,
     ):
         hash_key = cls._get_key(email, password, connection.get_cache_key())
         cls.__credentials_store__[hash_key] = syft_client
         cls.__client_cache__[syft_client.id] = syft_client
 
     @classmethod
+    def add_client_by_uid_and_verify_key(
+        cls,
+        verify_key: SyftVerifyKey,
+        node_uid: UID,
+        syft_client: SyftClient,
+    ):
+        hash_key = str(node_uid) + str(verify_key)
+        cls.__client_cache__[hash_key] = syft_client
+
+    @classmethod
+    def get_client_by_uid_and_verify_key(
+        cls, verify_key: SyftVerifyKey, node_uid: UID
+    ) -> Optional[SyftClient]:
+        hash_key = str(node_uid) + str(verify_key)
+        return cls.__client_cache__.get(hash_key, None)
+
+    @classmethod
     def get_client(
         cls, email: str, password: str, connection: NodeConnection
     ) -> Optional[SyftClient]:
         # we have some bugs here so lets disable until they are fixed
         return None
         hash_key = cls._get_key(email, password, connection.get_cache_key())
         return cls.__credentials_store__.get(hash_key, None)
```

### Comparing `syft-0.8.1b3/src/syft/client/deploy.py` & `syft-0.8.1b4/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/client/registry.py` & `syft-0.8.1b4/src/syft/client/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             if online:
                 version = network.get("version", None)
                 # Check if syft version was described in NetworkRegistry
                 # If it's unknown, try to update it to an available version.
                 if not version or version == "unknown":
                     # If not defined, try to ask in /syft/version endpoint (supported by 0.7.0)
                     try:
-                        version_url = url + "api/v1/new/metadata"
+                        version_url = url + "api/v2/metadata"
                         res = requests.get(version_url, timeout=0.5)  # nosec
                         if res.status_code == 200:
                             network["version"] = res.json()["syft_version"]
                         else:
                             network["version"] = "unknown"
                     except Exception:
                         network["version"] = "unknown"
@@ -172,15 +172,15 @@
             if online:
                 version = network.get("version", None)
                 # Check if syft version was described in NetworkRegistry
                 # If it's unknown, try to update it to an available version.
                 if not version or version == "unknown":
                     # If not defined, try to ask in /syft/version endpoint (supported by 0.7.0)
                     try:
-                        version_url = url + "api/v1/new/metadata"
+                        version_url = url + "api/v2/metadata"
                         res = requests.get(version_url, timeout=0.5)
                         if res.status_code == 200:
                             network["version"] = res.json()["syft_version"]
                         else:
                             network["version"] = "unknown"
                     except Exception:
                         network["version"] = "unknown"
```

### Comparing `syft-0.8.1b3/src/syft/client/search.py` & `syft-0.8.1b4/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/client/user_settings.py` & `syft-0.8.1b4/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/core/node/new/action_object.py` & `syft-0.8.1b4/src/syft/service/action/action_object.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,121 @@
 # future
 from __future__ import annotations
 
 # stdlib
+from enum import Enum
 import inspect
+import traceback
 import types
 from typing import Any
 from typing import Callable
 from typing import ClassVar
 from typing import Dict
 from typing import KeysView
 from typing import List
 from typing import Optional
-from typing import Set
 from typing import Tuple
 from typing import Type
 from typing import Union
 
 # third party
 import pydantic
+from result import Err
+from result import Ok
+from result import Result
 from typing_extensions import Self
 
 # relative
+from ...client.api import SyftAPI
+from ...client.client import SyftClient
+from ...serde.serializable import serializable
+from ...store.linked_obj import LinkedObject
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftBaseObject
+from ...types.syft_object import SyftObject
+from ...types.uid import LineageID
+from ...types.uid import UID
+from ...util.logger import debug
+from ..response import SyftException
 from .action_data_empty import ActionDataEmpty
+from .action_permissions import ActionPermission
+from .action_types import action_type_for_object
 from .action_types import action_type_for_type
 from .action_types import action_types
-from .client import SyftClient
-from .response import SyftException
-from .serializable import serializable
-from .syft_object import SYFT_OBJECT_VERSION_1
-from .syft_object import SyftBaseObject
-from .syft_object import SyftObject
-from .uid import LineageID
-from .uid import UID
+
+NoneType = type(None)
+
+
+@serializable()
+class TwinMode(Enum):
+    NONE = 0
+    PRIVATE = 1
+    MOCK = 2
+
+
+@serializable()
+class ActionType(Enum):
+    GETATTRIBUTE = 1
+    METHOD = 2
+    SETATTRIBUTE = 4
+    FUNCTION = 8
+    CREATEOBJECT = 16
 
 
 @serializable()
 class Action(SyftObject):
+    """Serializable Action object.
+
+    Parameters:
+        path: str
+            The path of the Type of the remote object.
+        op: str
+            The method to be executed from the remote object.
+        remote_self: Optional[LineageID]
+            The extended UID of the SyftObject
+        args: List[LineageID]
+            `op` args
+        kwargs: Dict[str, LineageID]
+            `op` kwargs
+        result_id: Optional[LineageID]
+            Extended UID of the resulted SyftObject
+    """
+
     __canonical_name__ = "Action"
     __version__ = SYFT_OBJECT_VERSION_1
 
     __attr_searchable__: List[str] = []
 
     path: str
     op: str
     remote_self: Optional[LineageID]
     args: List[LineageID]
     kwargs: Dict[str, LineageID]
     result_id: Optional[LineageID]
+    action_type: Optional[ActionType]
+    create_object: Optional[SyftObject] = None
 
     @pydantic.validator("id", pre=True, always=True)
     def make_id(cls, v: Optional[UID]) -> UID:
+        """Generate or reuse an UID"""
         return v if isinstance(v, UID) else UID()
 
     @pydantic.validator("result_id", pre=True, always=True)
     def make_result_id(cls, v: Optional[Union[UID, LineageID]]) -> UID:
+        """Generate or reuse a LineageID"""
         return v if isinstance(v, LineageID) else LineageID(v)
 
     @property
     def full_path(self) -> str:
+        """Action path and operation"""
         return f"{self.path}.{self.op}"
 
     @property
     def syft_history_hash(self) -> int:
+        """Create a unique hash for the operations applied on the object."""
         hashes = 0
         if self.remote_self:
             hashes += hash(self.remote_self.syft_history_hash)
         # 🔵 TODO: resolve this
         # if the object is ActionDataEmpty then the type might not be equal to the
         # real thing. This is the same issue with determining the result type from
         # a pointer operation in the past, so we should think about what we want here
@@ -74,20 +124,37 @@
         for arg in self.args:
             hashes += hash(arg.syft_history_hash)
         for k, arg in self.kwargs.items():
             hashes += hash(k)
             hashes += hash(arg.syft_history_hash)
         return hashes
 
+    def __repr__(self):
+        def repr_uid(_id):
+            return f"{str(_id)[:3]}..{str(_id)[-1]}"
+
+        arg_repr = ", ".join([repr_uid(x) for x in self.args])
+        kwargs_repr = ", ".join(
+            [f"{key}={repr_uid(value)}" for key, value in self.kwargs.items()]
+        )
+        self_repr = (
+            f"[{repr_uid(self.remote_self)}]" if self.remote_self is not None else ""
+        )
+        return (
+            f"ActionObject {self.path}{self_repr}.{self.op}({arg_repr},{kwargs_repr})"
+        )
+
 
 class ActionObjectPointer:
     pass
 
 
+# Hooks
 HOOK_ALWAYS = "ALWAYS"
+HOOK_ON_POINTERS = "ON_POINTERS"
 
 passthrough_attrs = [
     "__dict__",  # python
     "__class__",  # python
     "__repr_name__",  # python
     "__annotations__",  # python
     "_init_private_attributes",  # pydantic
@@ -130,119 +197,188 @@
     "__getitem__",
     "__setitem__",
     "__len__",
     "shape",
 ]
 action_data_empty_must_run = [
     "__repr__",
+    "__str__",
 ]
-show_print = False
 
 
-def debug_original_func(name: str, func: Callable) -> None:
-    print(f"{name} func is:")
-    print("inspect.isdatadescriptor", inspect.isdatadescriptor(func))
-    print("inspect.isgetsetdescriptor", inspect.isgetsetdescriptor(func))
-    print("inspect.isfunction", inspect.isfunction(func))
-    print("inspect.isbuiltin", inspect.isbuiltin(func))
-    print("inspect.ismethod", inspect.ismethod(func))
-    print("inspect.ismethoddescriptor", inspect.ismethoddescriptor(func))
+class PreHookContext(SyftBaseObject):
+    """Hook context
+
+    Parameters:
+        obj: Any
+            The ActionObject to use for the action
+        op_name: str
+            The method name to use for the action
+        node_uid: Optional[UID]
+            Optional Syft node UID
+        result_id: Optional[Union[UID, LineageID]]
+            Optional result Syft UID
+        action: Optional[Action]
+            The action generated by the current hook
+    """
+
+    obj: Any
+    op_name: str
+    node_uid: Optional[UID]
+    result_id: Optional[Union[UID, LineageID]]
+    result_twin_type: Optional[TwinMode]
+    action: Optional[Action]
+    action_type: Optional[ActionType]
 
 
-def make_action_side_effect(context: PreHookContext, *args: Any, **kwargs: Any) -> Any:
+def make_action_side_effect(
+    context: PreHookContext, *args: List[Any, ...], **kwargs: Dict[str, Any]
+) -> Result[Ok[Tuple[PreHookContext, Tuple[Any, ...], Dict[str, Any]]], Err[str]]:
+    """Create a new action from context_op_name, and add it to the PreHookContext
+
+    Parameters:
+        context: PreHookContext
+            PreHookContext object
+        *args:
+            Operation *args
+        **kwargs
+            Operation *kwargs
+    Returns:
+        - Ok[[Tuple[PreHookContext, Tuple[Any, ...], Dict[str, Any]]] on success
+        - Err[str] on failure
+    """
+    # relative
+
     try:
-        action = context.obj.syft_make_method_action(
-            op=context.op_name, args=args, kwargs=kwargs
+        action = context.obj.syft_make_action_with_self(
+            op=context.op_name,
+            args=args,
+            kwargs=kwargs,
+            action_type=context.action_type,
         )
         context.action = action
-    except Exception:  # nosec
-        # print(
-        #     "Exception detected in make_action_side_effect", e
-        # )  # TODO: Put this Exception back
-        pass
-    return context, args, kwargs
-
-
-def send_action_side_effect(context: PreHookContext, *args: Any, **kwargs: Any) -> Any:
+    except Exception:
+        print(f"make_action_side_effect failed with {traceback.format_exc()}")
+        return Err(f"make_action_side_effect failed with {traceback.format_exc()}")
+    return Ok((context, args, kwargs))
+
+
+class TraceResult:
+    result = []
+    _client = None
+
+    @classmethod
+    def reset(cls):
+        cls.result = []
+        cls._client = None
+
+
+def trace_action_side_effect(
+    context: PreHookContext, *args: Any, **kwargs: Any
+) -> Result[Ok[Tuple[PreHookContext, Tuple[Any, ...], Dict[str, Any]]], Err[str]]:
+    action = context.action
+    if action is not None:
+        TraceResult.result += [action]
+    return Ok((context, args, kwargs))
+
+
+def convert_to_pointers(
+    api: SyftAPI,
+    node_uid: Optional[UID] = None,
+    args: Optional[List] = None,
+    kwargs: Optional[Dict] = None,
+) -> Tuple[List, Dict]:
+    arg_list = []
+    kwarg_dict = {}
+    if args is not None:
+        for arg in args:
+            if not isinstance(arg, ActionObject):
+                arg = ActionObject.from_obj(arg)
+                arg.syft_node_uid = node_uid
+                arg = api.services.action.set(arg)
+                # arg = action_obj.send(
+                #     client
+                # )  # make sure this doesn't break things later on in send_method_action
+            arg_list.append(arg)
+
+    if kwargs is not None:
+        for k, arg in kwargs.items():
+            if not isinstance(arg, ActionObject):
+                arg = ActionObject.from_obj(arg)
+                arg.syft_node_uid = node_uid
+                arg = api.services.action.set(arg)
+                # arg = action_obj.send(client)
+
+            kwarg_dict[k] = arg
+
+    return arg_list, kwarg_dict
+
+
+def send_action_side_effect(
+    context: PreHookContext, *args: Any, **kwargs: Any
+) -> Result[Ok[Tuple[PreHookContext, Tuple[Any, ...], Dict[str, Any]]], Err[str]]:
+    """Create a new action from the context.op_name, and execute it on the remote node."""
     try:
-        if context.op_name not in dont_make_side_effects and hasattr(
-            context.obj, "syft_node_uid"
-        ):
-            if getattr(context.obj, "syft_node_uid", None):
-                if context.action is not None:
-                    action = context.obj.syft_make_method_action(
-                        op=context.op_name, args=args, kwargs=kwargs
-                    )
-                    context.action = action
-
-                action_result = context.obj.syft_execute_action(action, sync=True)
-                if not isinstance(action_result, ActionObject):
-                    # print("Got back unexpected response", action_result)
-                    pass
-                else:
-                    context.node_uid = action_result.syft_node_uid
-                    context.result_id = action.result_id
-                    # print("IGNORING: got action result", action_result)
-            else:
-                # 🟡 TODO
-                pass
-                # print(
-                #     "Can't Send Action without a target node. Use .point_to(node_uid: UID)"
-                # )
-    except Exception:  # nosec
-        # print(
-        #     "Exception in send_action_side_effect", e
-        # )  # TODO: Put this Exception back
-        pass
-    return context, args, kwargs
+        if context.action is None:
+            result = make_action_side_effect(context, *args, **kwargs)
+            if result.is_err():
+                raise RuntimeError(result.err())
 
+            context, _, _ = result.ok()
 
-def propagate_node_uid(context: PreHookContext, op: str, result: Any) -> Any:
-    try:
-        if context.op_name not in dont_make_side_effects and hasattr(
-            context.obj, "syft_node_uid"
-        ):
-            syft_node_uid = getattr(context.obj, "syft_node_uid", None)
-            if syft_node_uid:
-                if not hasattr(result, "syft_node_uid"):
-                    # print("result doesnt have a syft_node_uid attr")
-                    pass
-                if op not in context.obj._syft_dont_wrap_attrs():
-                    if hasattr(result, "syft_node_uid"):
-                        setattr(result, "syft_node_uid", syft_node_uid)
-                else:
-                    # print("dont propogate node_uid because output isnt wrapped")
-                    pass
-            else:
-                # 🟡 TODO
-                # print("Can't proagate node_uid because parent doesnt have one")
-                pass
-    except Exception:  # nosec
-        # print("Exception in propagate_node_uid", e)
-        pass
-    return result
+        action_result = context.obj.syft_execute_action(context.action, sync=True)
 
+        if not isinstance(action_result, ActionObject):
+            raise RuntimeError(f"Got back unexpected response : {action_result}")
+        else:
+            context.node_uid = action_result.syft_node_uid
+            context.result_id = action_result.id
+            context.result_twin_type = action_result.syft_twin_type
+    except Exception as e:
+        return Err(
+            f"send_action_side_effect failed with {e}\n {traceback.format_exc()}"
+        )
+    return Ok((context, args, kwargs))
 
-def is_action_data_empty(obj: Any) -> bool:
-    if hasattr(obj, "syft_action_data"):
-        obj = obj.syft_action_data
-    if isinstance(obj, ActionDataEmpty):
-        return True
-    return False
 
+def propagate_node_uid(
+    context: PreHookContext, op: str, result: Any
+) -> Result[Ok[Any], Err[str]]:
+    """Patch the result to include the syft_node_uid
+
+    Parameters:
+        context: PreHookContext
+            PreHookContext object
+        op: str
+            Which operation was executed
+        result: Any
+            The result to patch
+    Returns:
+        - Ok[[result] on success
+        - Err[str] on failure
+    """
+    if context.op_name in dont_make_side_effects or not hasattr(
+        context.obj, "syft_node_uid"
+    ):
+        return Ok(result)
 
-def has_action_data_empty(args: Any, kwargs: Any) -> bool:
-    for a in args:
-        if is_action_data_empty(a):
-            return True
+    try:
+        syft_node_uid = getattr(context.obj, "syft_node_uid", None)
+        if syft_node_uid is None:
+            raise RuntimeError("Can't proagate node_uid because parent doesnt have one")
+
+        if op not in context.obj._syft_dont_wrap_attrs():
+            if hasattr(result, "syft_node_uid"):
+                result.syft_node_uid = syft_node_uid
+        else:
+            raise RuntimeError("dont propogate node_uid because output isnt wrapped")
+    except Exception:
+        return Err(f"propagate_node_uid failed with {traceback.format_exc()}")
 
-    for _, a in kwargs.items():
-        if is_action_data_empty(a):
-            return True
-    return False
+    return Ok(result)
 
 
 def debox_args_and_kwargs(args: Any, kwargs: Any) -> Tuple[Any, Any]:
     filtered_args = []
     filtered_kwargs = {}
     for a in args:
         value = a
@@ -255,23 +391,30 @@
         if hasattr(value, "syft_action_data"):
             value = value.syft_action_data
         filtered_kwargs[k] = a
 
     return tuple(filtered_args), filtered_kwargs
 
 
-class PreHookContext(SyftBaseObject):
-    obj: Any
-    op_name: str
-    node_uid: Optional[UID]
-    result_id: Optional[Union[UID, LineageID]]
-    action: Optional[Action]
+BASE_PASSTHROUGH_ATTRS = [
+    "is_mock",
+    "is_real",
+    "is_twin",
+    "is_pointer",
+    "request",
+    "__repr__",
+    "_repr_markdown_",
+    "syft_twin_type",
+    "_repr_debug_",
+]
 
 
 class ActionObject(SyftObject):
+    """Action object for remote execution."""
+
     __canonical_name__ = "ActionObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     __attr_searchable__: List[str] = []
     syft_action_data: Optional[Any] = None
     syft_pointer_type: ClassVar[Type[ActionObjectPointer]]
 
@@ -279,394 +422,765 @@
     syft_parent_hashes: Optional[Union[int, List[int]]]
     syft_parent_op: Optional[str]
     syft_parent_args: Optional[Any]
     syft_parent_kwargs: Optional[Any]
     syft_history_hash: Optional[int]
     syft_internal_type: ClassVar[Type[Any]]
     syft_node_uid: Optional[UID]
-    _syft_pre_hooks__: Dict[str, Set] = {}
-    _syft_post_hooks__: Dict[str, Set] = {}
+    _syft_pre_hooks__: Dict[str, List] = {}
+    _syft_post_hooks__: Dict[str, List] = {}
+    syft_twin_type: TwinMode = TwinMode.NONE
+    syft_passthrough_attrs = BASE_PASSTHROUGH_ATTRS
+    # syft_dont_wrap_attrs = ["shape"]
+
+    @property
+    def is_pointer(self) -> bool:
+        return self.syft_node_uid is not None
 
     @property
     def syft_lineage_id(self) -> LineageID:
+        """Compute the LineageID of the ActionObject, using the `id` and the `syft_history_hash` memebers"""
         return LineageID(self.id, self.syft_history_hash)
 
     @pydantic.validator("id", pre=True, always=True)
     def make_id(cls, v: Optional[UID]) -> UID:
-        return v if isinstance(v, UID) else UID()
+        """Generate or reuse an UID"""
+        return Action.make_id(v)
+
+    @property
+    def is_mock(self):
+        return self.syft_twin_type == TwinMode.MOCK
+
+    @property
+    def is_real(self):
+        return self.syft_twin_type == TwinMode.PRIVATE
+
+    @property
+    def is_twin(self):
+        return self.syft_twin_type != TwinMode.NONE
 
     @pydantic.validator("syft_action_data", pre=True, always=True)
     def check_action_data(
         cls, v: ActionObject.syft_pointer_type
     ) -> ActionObject.syft_pointer_type:
         if cls == AnyActionObject or isinstance(
             v, (cls.syft_internal_type, ActionDataEmpty)
         ):
             return v
-        # third party
         raise SyftException(
             f"Must init {cls} with {cls.syft_internal_type} not {type(v)}"
         )
 
-    def syft_point_to(self, node_uid: UID) -> None:
+    def syft_point_to(self, node_uid: UID) -> "ActionObject":
+        """Set the syft_node_uid, used in the post hooks"""
         self.syft_node_uid = node_uid
 
+        return self
+
     def syft_get_property(self, obj: Any, method: str) -> Any:
         klass_method = getattr(type(obj), method, None)
         if klass_method is None:
             raise Exception(f"{type(obj)} has no {method} attribute")
         return klass_method.__get__(obj)
 
     def syft_is_property(self, obj: Any, method: str) -> bool:
         klass_method = getattr(type(obj), method, None)
         return isinstance(klass_method, property) or inspect.isdatadescriptor(
             klass_method
         )
 
+    def syft_execute_action(
+        self, action: Action, sync: bool = True
+    ) -> ActionObjectPointer:
+        """Execute a remote action
+
+        Parameters:
+            action: Action
+                Which action to execute
+            sync: bool
+                Run sync/async
+
+        Returns:
+            ActionObjectPointer
+        """
+        if self.syft_node_uid is None:
+            raise SyftException("Pointers can't execute without a node_uid.")
+
+        # relative
+        from ...client.api import APIRegistry
+        from ...client.api import SyftAPICall
+
+        api = APIRegistry.api_for(node_uid=self.syft_node_uid)
+
+        kwargs = {"action": action}
+        api_call = SyftAPICall(
+            node_uid=self.syft_node_uid, path="action.execute", args=[], kwargs=kwargs
+        )
+        return api.make_call(api_call)
+
+    def request(self, client):
+        # relative
+        from ..request.request import ActionStoreChange
+        from ..request.request import SubmitRequest
+
+        action_object_link = LinkedObject.from_obj(self, node_uid=self.syft_node_uid)
+        permission_change = ActionStoreChange(
+            linked_obj=action_object_link, apply_permission_type=ActionPermission.READ
+        )
+
+        submit_request = SubmitRequest(
+            changes=[permission_change],
+            requesting_user_verify_key=client.credentials.verify_key,
+        )
+        return client.api.services.request.submit(submit_request)
+
+    def _syft_try_to_save_to_store(self, obj) -> None:
+        if self.syft_node_uid is None:
+            return
+        elif obj.syft_node_uid is not None:
+            return
+        # TODO fix: the APIRegistry often gets the wrong client
+        # if you have 2 clients in memory
+        # therefore the following happens if you call a method
+        # with a pointer to a twin (mock version)
+        # 1) it gets the wrong credentials
+        # 2) it uses the mock version to overwrite the real version
+        # 3) it shouldnt send in the first place as it already exists
+
+        # relative
+        from ...client.api import APIRegistry
+
+        action = Action(
+            path="",
+            op="",
+            remote_self=None,
+            result_id=obj.id,
+            args=[],
+            kwargs=dict(),
+            action_type=ActionType.CREATEOBJECT,
+            create_object=obj,
+        )
+
+        if TraceResult._client is not None:
+            api = TraceResult._client.api
+            TraceResult.result += [action]
+        else:
+            api = APIRegistry.api_for(node_uid=self.syft_node_uid)
+
+        api.services.action.execute(action)
+
+    def _syft_prepare_obj_uid(self, obj) -> LineageID:
+        # We got the UID
+        if isinstance(obj, (UID, LineageID)):
+            return LineageID(obj.id)
+
+        # We got the ActionObjectPointer
+        if isinstance(obj, ActionObjectPointer):
+            return obj.syft_lineage_id
+
+        # We got the ActionObject. We need to save it in the store.
+        if isinstance(obj, ActionObject):
+            self._syft_try_to_save_to_store(obj)
+            return obj.syft_lineage_id
+
+        # We got a raw object. We need to create the ActionObject from scratch and save it in the store.
+        obj_id = Action.make_id(None)
+        lin_obj_id = Action.make_result_id(obj_id)
+        act_obj = ActionObject.from_obj(obj, id=obj_id, syft_lineage_id=lin_obj_id)
+
+        self._syft_try_to_save_to_store(act_obj)
+
+        return act_obj.syft_lineage_id
+
+    def syft_make_action(
+        self,
+        path: str,
+        op: str,
+        remote_self: Optional[Union[UID, LineageID]] = None,
+        args: Optional[
+            List[Union[UID, LineageID, ActionObjectPointer, ActionObject, Any]]
+        ] = None,
+        kwargs: Optional[
+            Dict[str, Union[UID, LineageID, ActionObjectPointer, ActionObject, Any]]
+        ] = None,
+        action_type: Optional[ActionType] = None,
+    ) -> Action:
+        """Generate new action from the information
+
+        Parameters:
+            path: str
+                The path of the Type of the remote object.
+            op: str
+                The method to be executed from the remote object.
+            remote_self: Optional[Union[UID, LineageID]]
+                The extended UID of the SyftObject
+            args: Optional[List[Union[UID, LineageID, ActionObjectPointer, ActionObject]]]
+                `op` args
+            kwargs: Optional[Dict[str, Union[UID, LineageID, ActionObjectPointer, ActionObject]]]
+                `op` kwargs
+        Returns:
+            Action object
+
+        Raises:
+            ValueError: For invalid args or kwargs
+            PydanticValidationError: For args and kwargs
+        """
+        if args is None:
+            args = []
+        if kwargs is None:
+            kwargs = {}
+
+        arg_ids = []
+        kwarg_ids = {}
+
+        for obj in args:
+            arg_ids.append(self._syft_prepare_obj_uid(obj))
+
+        for k, obj in kwargs.items():
+            kwarg_ids[k] = self._syft_prepare_obj_uid(obj)
+
+        action = Action(
+            path=path,
+            op=op,
+            remote_self=LineageID(remote_self),
+            args=arg_ids,
+            kwargs=kwarg_ids,
+            action_type=action_type,
+        )
+        return action
+
+    def syft_make_action_with_self(
+        self,
+        op: str,
+        args: Optional[List[Union[UID, ActionObjectPointer]]] = None,
+        kwargs: Optional[Dict[str, Union[UID, ActionObjectPointer]]] = None,
+        action_type: Optional[ActionType] = None,
+    ) -> Action:
+        """Generate new method action from the current object.
+
+        Parameters:
+            op: str
+                The method to be executed from the remote object.
+            args: List[LineageID]
+                `op` args
+            kwargs: Dict[str, LineageID]
+                `op` kwargs
+        Returns:
+            Action object
+
+        Raises:
+            ValueError: For invalid args or kwargs
+            PydanticValidationError: For args and kwargs
+        """
+        path = self.syft_get_path()
+        return self.syft_make_action(
+            path=path,
+            op=op,
+            remote_self=self.syft_lineage_id,
+            args=args,
+            kwargs=kwargs,
+            action_type=action_type,
+        )
+
+    def syft_get_path(self) -> str:
+        """Get the type path of the underlying object"""
+        if isinstance(self, AnyActionObject) and self.syft_internal_type:
+            return f"{type(self.syft_action_data).__name__}"  # avoids AnyActionObject errors
+        return f"{type(self).__name__}"
+
+    def syft_remote_method(
+        self,
+        op: str,
+    ) -> Callable:
+        """Generate a Callable object for remote calls.
+
+        Parameters:
+            op: str
+                he method to be executed from the remote object.
+
+        Returns:
+            A function
+        """
+
+        def wrapper(
+            *args: Optional[List[Union[UID, ActionObjectPointer]]],
+            **kwargs: Optional[Dict[str, Union[UID, ActionObjectPointer]]],
+        ) -> Action:
+            return self.syft_make_action_with_self(op=op, args=args, kwargs=kwargs)
+
+        return wrapper
+
     def send(self, client: SyftClient) -> Self:
+        """Send the object to a Syft Client"""
+
         return client.api.services.action.set(self)
 
     def get_from(self, client: SyftClient) -> Any:
-        return client.api.services.action.get(self.id).syft_action_data
+        """Get the object from a Syft Client"""
+        res = client.api.services.action.get(self.id)
+        if not isinstance(res, ActionObject):
+            return Err(res)
+        else:
+            return res.syft_action_data
 
     @staticmethod
     def from_obj(
         syft_action_data: Any,
         id: Optional[UID] = None,
         syft_lineage_id: Optional[LineageID] = None,
     ) -> ActionObject:
-        if isinstance(syft_action_data, ActionObject):
-            return syft_action_data
+        """Create an ActionObject from an existing object.
+
+        Parameters:
+            syft_action_data: Any
+                The object to be converted to a Syft ActionObject
+            id: Optional[UID]
+                Which ID to use for the ActionObject. Optional
+            syft_lineage_id: Optional[LineageID]
+                Which LineageID to use for the ActionObject. Optional
+        """
         if id and syft_lineage_id and id != syft_lineage_id.id:
-            raise Exception("UID and LineageID should match")
-        action_type = action_type_for_type(syft_action_data)
-        if action_type is None:
-            raise Exception(f"{type(syft_action_data)} not in action_types")
+            raise ValueError("UID and LineageID should match")
+
+        action_type = action_type_for_object(syft_action_data)
         action_object = action_type(syft_action_data=syft_action_data)
+
         if id:
             action_object.id = id
+
         if syft_lineage_id:
             action_object.id = syft_lineage_id.id
             action_object.syft_history_hash = syft_lineage_id.syft_history_hash
         elif id:
             action_object.syft_history_hash = hash(id)
 
         return action_object
 
+    @classmethod
+    def add_trace_hook(cls):
+        return True
+        # if trace_action_side_effect not in self._syft_pre_hooks__[HOOK_ALWAYS]:
+        #     self._syft_pre_hooks__[HOOK_ALWAYS].append(trace_action_side_effect)
+
+    @classmethod
+    def remove_trace_hook(cls):
+        return True
+        # self._syft_pre_hooks__[HOOK_ALWAYS].pop(trace_action_side_effct, None)
+
     @staticmethod
     def empty(
-        syft_internal_type: Optional[Any] = Any,
+        syft_internal_type: Type[Any] = NoneType,
         id: Optional[UID] = None,
         syft_lineage_id: Optional[LineageID] = None,
     ) -> ActionObject:
+        """Create an ActionObject from a type, using a ActionDataEmpty object
+
+        Parameters:
+            syft_internal_type: Type
+                The Type for which to create a ActionDataEmpty object
+            id: Optional[UID]
+                Which ID to use for the ActionObject. Optional
+            syft_lineage_id: Optional[LineageID]
+                Which LineageID to use for the ActionObject. Optional
+        """
+
         empty = ActionDataEmpty(syft_internal_type=syft_internal_type)
-        action_object = ActionObject.from_obj(
+        res = ActionObject.from_obj(
             syft_action_data=empty, id=id, syft_lineage_id=syft_lineage_id
         )
-        return action_object
+        res.__dict__["syft_internal_type"] = syft_internal_type
+        return res
 
     def __post_init__(self) -> None:
+        """Add pre/post hooks."""
         if HOOK_ALWAYS not in self._syft_pre_hooks__:
-            self._syft_pre_hooks__[HOOK_ALWAYS] = set()
-        self._syft_pre_hooks__[HOOK_ALWAYS].add(make_action_side_effect)
-        self._syft_pre_hooks__[HOOK_ALWAYS].add(send_action_side_effect)
+            self._syft_pre_hooks__[HOOK_ALWAYS] = []
+
+        if HOOK_ON_POINTERS not in self._syft_post_hooks__:
+            self._syft_pre_hooks__[HOOK_ON_POINTERS] = []
+
+        # this should be a list as orders matters
+        for side_effect in [make_action_side_effect]:
+            if side_effect not in self._syft_pre_hooks__[HOOK_ALWAYS]:
+                self._syft_pre_hooks__[HOOK_ALWAYS].append(side_effect)
+
+        for side_effect in [send_action_side_effect]:
+            if side_effect not in self._syft_pre_hooks__[HOOK_ON_POINTERS]:
+                self._syft_pre_hooks__[HOOK_ON_POINTERS].append(side_effect)
+
+        if trace_action_side_effect not in self._syft_pre_hooks__[HOOK_ALWAYS]:
+            self._syft_pre_hooks__[HOOK_ALWAYS].append(trace_action_side_effect)
 
         if HOOK_ALWAYS not in self._syft_post_hooks__:
-            self._syft_post_hooks__[HOOK_ALWAYS] = set()
-        self._syft_post_hooks__[HOOK_ALWAYS].add(propagate_node_uid)
+            self._syft_post_hooks__[HOOK_ALWAYS] = []
+
+        if HOOK_ON_POINTERS not in self._syft_post_hooks__:
+            self._syft_post_hooks__[HOOK_ON_POINTERS] = []
+
+        for side_effect in [propagate_node_uid]:
+            if side_effect not in self._syft_post_hooks__[HOOK_ALWAYS]:
+                self._syft_post_hooks__[HOOK_ALWAYS].append(side_effect)
 
         if isinstance(self.syft_action_data, ActionObject):
             raise Exception("Nested ActionObjects", self.syft_action_data)
 
         self.syft_history_hash = hash(self.id)
 
     def _syft_run_pre_hooks__(
         self, context: PreHookContext, name: str, args: Any, kwargs: Any
     ) -> Tuple[PreHookContext, Tuple[Any, ...], Dict[str, Any]]:
-        try:
-            result_args, result_kwargs = args, kwargs
-            if name in self._syft_pre_hooks__:
-                for hook in self._syft_pre_hooks__[name]:
-                    context, result_args, result_kwargs = hook(
-                        context, *result_args, **result_kwargs
-                    )
+        """Hooks executed before the actual call"""
+        result_args, result_kwargs = args, kwargs
+        if name in self._syft_pre_hooks__:
+            for hook in self._syft_pre_hooks__[name]:
+                result = hook(context, *result_args, **result_kwargs)
+                if result.is_ok():
+                    context, result_args, result_kwargs = result.ok()
+                else:
+                    debug(f"Pre-hook failed with {result.err()}")
+        if name not in self._syft_dont_wrap_attrs():
+            if HOOK_ALWAYS in self._syft_pre_hooks__:
+                for hook in self._syft_pre_hooks__[HOOK_ALWAYS]:
+                    result = hook(context, *result_args, **result_kwargs)
+                    if result.is_ok():
+                        context, result_args, result_kwargs = result.ok()
+                    else:
+                        msg = result.err().replace("\\n", "\n")
+                        debug(f"Pre-hook failed with {msg}")
 
+        if self.is_pointer:
             if name not in self._syft_dont_wrap_attrs():
                 if HOOK_ALWAYS in self._syft_pre_hooks__:
-                    for hook in self._syft_pre_hooks__[HOOK_ALWAYS]:
-                        context, result_args, result_kwargs = hook(
-                            context, *result_args, **result_kwargs
-                        )
-        except Exception as e:
-            print("Exception in pre hooks", e)
+                    for hook in self._syft_pre_hooks__[HOOK_ON_POINTERS]:
+                        result = hook(context, *result_args, **result_kwargs)
+                        if result.is_ok():
+                            context, result_args, result_kwargs = result.ok()
+                        else:
+                            msg = result.err().replace("\\n", "\n")
+                            debug(f"Pre-hook failed with {msg}")
+
         return context, result_args, result_kwargs
 
     def _syft_run_post_hooks__(
         self, context: PreHookContext, name: str, result: Any
     ) -> Any:
+        """Hooks executed after the actual call"""
         new_result = result
         if name in self._syft_post_hooks__:
             for hook in self._syft_post_hooks__[name]:
-                new_result = hook(context, name, new_result)
+                result = hook(context, name, new_result)
+                if result.is_ok():
+                    new_result = result.ok()
+                else:
+                    debug(f"Post hook failed with {result.err()}")
 
         if name not in self._syft_dont_wrap_attrs():
             if HOOK_ALWAYS in self._syft_post_hooks__:
                 for hook in self._syft_post_hooks__[HOOK_ALWAYS]:
-                    new_result = hook(context, name, new_result)
+                    result = hook(context, name, new_result)
+                    if result.is_ok():
+                        new_result = result.ok()
+                    else:
+                        debug(f"Post hook failed with {result.err()}")
+
+        if self.is_pointer:
+            if name not in self._syft_dont_wrap_attrs():
+                if HOOK_ALWAYS in self._syft_post_hooks__:
+                    for hook in self._syft_post_hooks__[HOOK_ON_POINTERS]:
+                        result = hook(context, name, new_result)
+                        if result.is_ok():
+                            new_result = result.ok()
+                        else:
+                            debug(f"Post hook failed with {result.err()}")
+
         return new_result
 
     def _syft_output_action_object(
-        self,
-        result: Any,
+        self, result: Any, context: Optional[PreHookContext] = None
     ) -> Any:
-        # can check types here
-        if not issubclass(type(result), ActionObject):
-            constructor = action_type_for_type(result)
-            if not constructor:
-                raise Exception(f"output: {type(result)} no in action_types")
-            result = constructor(syft_action_data=result)
+        """Wrap the result in an ActionObject"""
+        if issubclass(type(result), ActionObject):
+            return result
+
+        constructor = action_type_for_type(result)
+        syft_twin_type = TwinMode.NONE
+        if context.result_twin_type is not None:
+            syft_twin_type = context.result_twin_type
+        result = constructor(syft_action_data=result, syft_twin_type=syft_twin_type)
 
         return result
 
     def _syft_passthrough_attrs(self) -> List[str]:
+        """These attributes are forwarded to the `object` base class."""
         return passthrough_attrs + getattr(self, "syft_passthrough_attrs", [])
 
     def _syft_dont_wrap_attrs(self) -> List[str]:
+        """The results from these attributes are ignored from UID patching."""
         return dont_wrap_output_attrs + getattr(self, "syft_dont_wrap_attrs", [])
 
-    def __getattribute__(self, name: str) -> Any:
-        # bypass certain attrs to prevent recursion issues
-        if name.startswith("_syft") or name.startswith("syft"):
-            return object.__getattribute__(self, name)
-
-        if name in self._syft_passthrough_attrs():
-            return object.__getattribute__(self, name)
+    def _syft_get_attr_context(self, name: str) -> Any:
+        """Find which instance - Syft ActionObject or the original object - has the requested attribute."""
         defined_on_self = name in self.__dict__ or name in self.__private_attributes__
-        if show_print:
-            print(">> ", name, ", defined_on_self = ", defined_on_self)
 
-        # use the custom definied version
+        debug(">> ", name, ", defined_on_self = ", defined_on_self)
+
+        # use the custom defined version
         context_self = self
         if not defined_on_self:
             context_self = self.syft_action_data  # type: ignore
 
-        # TODO: weird edge cases here for things like tuples
-        if name == "__bool__" and not hasattr(self.syft_action_data, "__bool__"):
-            context = PreHookContext(obj=self, op_name=name)
-            context, _, _ = self._syft_run_pre_hooks__(context, name, (), {})
-            # no input needs to propagate
-            result = self._syft_run_post_hooks__(
-                context, name, bool(self.syft_action_data)
+        return context_self
+
+    def _syft_attr_propagate_ids(self, context, name: str, result: Any) -> Any:
+        """Patch the results with the syft_history_hash, node_uid, and result_id."""
+        if name in self._syft_dont_wrap_attrs():
+            return result
+
+        # Wrap as Syft Object
+        result = self._syft_output_action_object(result, context)
+
+        # Propagate History
+        if context.action is not None:
+            result.syft_history_hash = context.action.syft_history_hash
+
+        # Propagate Syft Node UID
+        result.syft_node_uid = context.node_uid
+
+        # Propagate Result ID
+        if context.result_id is not None:
+            result.id = context.result_id
+
+        return result
+
+    def _syft_wrap_attribute_for_bool_on_nonbools(self, name: str) -> Any:
+        """Handle `__getattribute__` for bool casting."""
+        if name != "__bool__":
+            raise RuntimeError(
+                "[_wrap_attribute_for_bool_on_nonbools] Use this only for the __bool__ operator"
             )
-            if name not in self._syft_dont_wrap_attrs():
-                result = self._syft_output_action_object(result)
-                if context.action is not None:
-                    result.syft_history_hash = context.action.syft_history_hash
 
-            def __wrapper__bool__() -> bool:
-                return result
+        if hasattr(self.syft_action_data, "__bool__"):
+            raise RuntimeError(
+                "[_wrap_attribute_for_bool_on_nonbools] self.syft_action_data already implements the bool operator"
+            )
 
-            return __wrapper__bool__
+        debug("[__getattribute__] Handling bool on nonbools")
+        context = PreHookContext(obj=self, op_name=name)
+        context, _, _ = self._syft_run_pre_hooks__(context, name, (), {})
+
+        # no input needs to propagate
+        result = self._syft_run_post_hooks__(context, name, bool(self.syft_action_data))
+        result = self._syft_attr_propagate_ids(context, name, result)
+
+        def __wrapper__bool__() -> bool:
+            return result
+
+        return __wrapper__bool__
+
+    def _syft_wrap_attribute_for_properties(self, name: str) -> Any:
+        """Handle `__getattribute__` for properties."""
+        context_self = self._syft_get_attr_context(name)
+
+        if not self.syft_is_property(context_self, name):
+            raise RuntimeError(
+                "[_wrap_attribute_for_properties] Use this only on properties"
+            )
+        debug(f"[__getattribute__] Handling property {name} ")
 
-        if self.syft_is_property(context_self, name):
-            if show_print:
-                print("Property detected: ", name)
-            if self.syft_is_property(context_self, name):
-                context = PreHookContext(obj=self, op_name=name)
-                context, _, _ = self._syft_run_pre_hooks__(context, name, (), {})
-                # no input needs to propagate
-                result = self._syft_run_post_hooks__(
-                    context, name, self.syft_get_property(context_self, name)
-                )
-                if name not in self._syft_dont_wrap_attrs():
-                    result = self._syft_output_action_object(result)
-                    if context.action is not None:
-                        result.syft_history_hash = context.action.syft_history_hash
-                return result
+        context = PreHookContext(
+            obj=self, op_name=name, action_type=ActionType.GETATTRIBUTE
+        )
+        context, _, _ = self._syft_run_pre_hooks__(context, name, (), {})
+        # no input needs to propagate
+        result = self._syft_run_post_hooks__(
+            context, name, self.syft_get_property(context_self, name)
+        )
+
+        return self._syft_attr_propagate_ids(context, name, result)
+
+    def _syft_wrap_attribute_for_methods(self, name: str) -> Any:
+        """Handle `__getattribute__` for methods."""
 
         # check for other types that aren't methods, functions etc
         def fake_func(*args: Any, **kwargs: Any) -> Any:
             return ActionDataEmpty(syft_internal_type=self.syft_internal_type)
 
+        debug(f"[__getattribute__] Handling method {name} ")
         if (
             isinstance(self.syft_action_data, ActionDataEmpty)
             and name not in action_data_empty_must_run
         ):
             original_func = fake_func
         else:
             original_func = getattr(self.syft_action_data, name)
 
-        if show_print:
-            debug_original_func(name, original_func)
+        debug_original_func(name, original_func)
 
-        if inspect.ismethod(original_func) or inspect.ismethoddescriptor(original_func):
-            if show_print:
-                print("Running method: ", name)
+        def _base_wrapper(*args: Any, **kwargs: Any) -> Any:
+            context = PreHookContext(
+                obj=self, op_name=name, action_type=ActionType.METHOD
+            )
+            context, pre_hook_args, pre_hook_kwargs = self._syft_run_pre_hooks__(
+                context, name, args, kwargs
+            )
 
-            def wrapper(_self: Any, *args: Any, **kwargs: Any) -> Any:
-                context = PreHookContext(obj=self, op_name=name)
-                context, pre_hook_args, pre_hook_kwargs = self._syft_run_pre_hooks__(
-                    context, name, args, kwargs
+            if has_action_data_empty(args=args, kwargs=kwargs):
+                result = fake_func(*args, **kwargs)
+            else:
+                original_args, original_kwargs = debox_args_and_kwargs(
+                    pre_hook_args, pre_hook_kwargs
                 )
+                result = original_func(*original_args, **original_kwargs)
 
-                if not has_action_data_empty(args=args, kwargs=kwargs):
-                    original_args, original_kwargs = debox_args_and_kwargs(
-                        pre_hook_args, pre_hook_kwargs
-                    )
+            post_result = self._syft_run_post_hooks__(context, name, result)
+            post_result = self._syft_attr_propagate_ids(context, name, post_result)
 
-                    result = original_func(*original_args, **original_kwargs)
-                else:
-                    result = fake_func(*args, **kwargs)
+            return post_result
 
-                post_result = self._syft_run_post_hooks__(context, name, result)
-                if name not in self._syft_dont_wrap_attrs():
-                    post_result = self._syft_output_action_object(
-                        post_result,
-                    )
-                    if context.action is not None:
-                        post_result.syft_history_hash = context.action.syft_history_hash
-                    post_result.syft_node_uid = context.node_uid
-                    if context.result_id is not None:
-                        post_result.id = context.result_id
-                return post_result
+        if inspect.ismethod(original_func) or inspect.ismethoddescriptor(original_func):
+            debug("Running method: ", name)
+
+            def wrapper(_self: Any, *args: Any, **kwargs: Any):
+                return _base_wrapper(*args, **kwargs)
 
             wrapper = types.MethodType(wrapper, type(self))
         else:
-            if show_print:
-                print("Running non-method: ", name)
-
-            def wrapper(*args: Any, **kwargs: Any) -> Any:
-                context = PreHookContext(obj=self, op_name=name)
-                context, pre_hook_args, pre_hook_kwargs = self._syft_run_pre_hooks__(
-                    context, name, args, kwargs
-                )
+            debug("Running non-method: ", name)
 
-                if not has_action_data_empty(args=args, kwargs=kwargs):
-                    original_args, original_kwargs = debox_args_and_kwargs(
-                        pre_hook_args, pre_hook_kwargs
-                    )
-
-                    result = original_func(*original_args, **original_kwargs)
-                else:
-                    result = fake_func(*args, **kwargs)
-
-                post_result = self._syft_run_post_hooks__(context, name, result)
-                if name not in self._syft_dont_wrap_attrs():
-                    post_result = self._syft_output_action_object(post_result)
-                    if context.action is not None:
-                        post_result.syft_history_hash = context.action.syft_history_hash
-                    post_result.syft_node_uid = context.node_uid
-                    if context.result_id is not None:
-                        post_result.id = context.result_id
-                return post_result
+            wrapper = _base_wrapper
 
         try:
             wrapper.__doc__ = original_func.__doc__
-            if show_print:
-                print(
-                    "Found original signature for ",
-                    name,
-                    inspect.signature(original_func),
-                )
+            debug(
+                "Found original signature for ",
+                name,
+                inspect.signature(original_func),
+            )
             wrapper.__ipython_inspector_signature_override__ = inspect.signature(
                 original_func
             )
         except Exception:
-            if show_print:
-                print("name", name, "has no signature")
+            debug("name", name, "has no signature")
 
         return wrapper
 
-    def syft_execute_action(
-        self, action: Action, sync: bool = True
-    ) -> ActionObjectPointer:
-        if self.syft_node_uid is None:
-            raise SyftException("Pointers can't execute without a node_uid.")
-        # relative
-        from .api import APIRegistry
-        from .api import SyftAPICall
+    def _syft_setattr(self, name, value):
+        args = (name, value)
+        kwargs = dict()
+        op_name = "__setattr__"
 
-        api = APIRegistry.api_for(node_uid=self.syft_node_uid)
+        def fake_func(*args: Any, **kwargs: Any) -> Any:
+            return ActionDataEmpty(syft_internal_type=self.syft_internal_type)
 
-        kwargs = {"action": action}
-        api_call = SyftAPICall(
-            node_uid=self.syft_node_uid, path="action.execute", args=[], kwargs=kwargs
-        )
-        return api.make_call(api_call)
+        if isinstance(self.syft_action_data, ActionDataEmpty) or has_action_data_empty(
+            args=args, kwargs=kwargs
+        ):
+            local_func = fake_func
+        else:
+            local_func = getattr(self.syft_action_data, op_name)
 
-    def syft_make_action(
-        self,
-        path: str,
-        op: str,
-        remote_self: Optional[Union[UID, LineageID]] = None,
-        args: Optional[List[Union[UID, ActionObjectPointer, LineageID]]] = None,
-        kwargs: Optional[Dict[str, Union[UID, ActionObjectPointer, LineageID]]] = None,
-    ) -> Action:
-        if args is None:
-            args = []
-        if kwargs is None:
-            kwargs = {}
-        arg_ids = [
-            LineageID(uid) if isinstance(uid, (UID, LineageID)) else uid.syft_lineage_id
-            for uid in args
-        ]
-        kwarg_ids = {
-            k: LineageID(uid)
-            if isinstance(uid, (LineageID, UID))
-            else uid.syft_lineage_id
-            for k, uid in kwargs.items()
-        }
-        action = Action(
-            path=path,
-            op=op,
-            remote_self=LineageID(remote_self),
-            args=arg_ids,
-            kwargs=kwarg_ids,
+        context = PreHookContext(
+            obj=self, op_name=op_name, action_type=ActionType.SETATTRIBUTE
         )
-        return action
-
-    def syft_make_method_action(
-        self,
-        op: str,
-        args: Optional[List[Union[UID, ActionObjectPointer]]] = None,
-        kwargs: Optional[Dict[str, Union[UID, ActionObjectPointer]]] = None,
-    ) -> Action:
-        path = self.syft_get_path()
-        return self.syft_make_action(
-            path=path, op=op, remote_self=self.syft_lineage_id, args=args, kwargs=kwargs
+        context, pre_hook_args, pre_hook_kwargs = self._syft_run_pre_hooks__(
+            context, "__setattr__", args, kwargs
         )
 
-    def syft_get_path(self) -> str:
-        if isinstance(self, AnyActionObject) and self.syft_internal_type:
-            return f"{self.syft_internal_type.__name__}"
-        return f"{type(self).__name__}"
+        original_args, _ = debox_args_and_kwargs(pre_hook_args, pre_hook_kwargs)
+        val = original_args[1]
+        local_func(name, val)
+        local_result = self
+
+        post_result = self._syft_run_post_hooks__(context, op_name, local_result)
+        post_result = self._syft_attr_propagate_ids(context, op_name, post_result)
+        return post_result
 
-    def syft_remote_method(
-        self,
-        op: str,
-    ) -> Callable:
-        def wrapper(
-            *args: Optional[List[Union[UID, ActionObjectPointer]]],
-            **kwargs: Optional[Dict[str, Union[UID, ActionObjectPointer]]],
-        ) -> Action:
-            return self.syft_make_method_action(op=op, args=args, kwargs=kwargs)
+    def __getattribute__(self, name: str) -> Any:
+        """Called unconditionally to implement attribute accesses for instances of the class.
+        If the class also defines __getattr__(), the latter will not be called unless __getattribute__()
+        either calls it explicitly or raises an AttributeError.
+        This method should return the (computed) attribute value or raise an AttributeError exception.
+        In order to avoid infinite recursion in this method, its implementation should always:
+         * call the base class method with the same name to access any attributes it needs
+            for example : object.__getattribute__(self, name).
+         * use the syft/_syft prefix for internal methods.
+         * add the method name to the passthrough_attrs.
+
+        Parameters:
+            name: str
+                The name of the attribute to access.
+        """
+        # bypass certain attrs to prevent recursion issues
+        if name.startswith("_syft") or name.startswith("syft"):
+            return object.__getattribute__(self, name)
 
-        return wrapper
+        # third party
+        if name in self._syft_passthrough_attrs():
+            return object.__getattribute__(self, name)
+        context_self = self._syft_get_attr_context(name)
+
+        # Handle bool operator on nonbools
+        if name == "__bool__" and not hasattr(self.syft_action_data, "__bool__"):
+            return self._syft_wrap_attribute_for_bool_on_nonbools(name)
+
+        # Handle Properties
+        if self.syft_is_property(context_self, name):
+            return self._syft_wrap_attribute_for_properties(name)
+
+        # Handle anything else
+        return self._syft_wrap_attribute_for_methods(name)
+
+    def __setattr__(self, name: str, value: Any) -> Any:
+        defined_on_self = name in self.__dict__ or name in self.__private_attributes__
+
+        debug(">> ", name, ", defined_on_self = ", defined_on_self)
+
+        # use the custom defined version
+        if defined_on_self:
+            self.__dict__[name] = value
+            return value
+        else:
+            self._syft_setattr(name, value)
+            context_self = self.syft_action_data  # type: ignore
+            return context_self.__setattr__(name, value)
 
     def keys(self) -> KeysView[str]:
         return self.syft_action_data.keys()  # type: ignore
 
     ###### __DUNDER_MIFFLIN__
 
     # if we do not implement these boiler plate __method__'s then special infix
     # operations like x + y won't trigger __getattribute__
     # unless there is a super special reason we should write no code in these functions
+    def _repr_markdown_(self) -> str:
+        if self.is_mock:
+            res = "TwinPointer(Mock)"
+        elif self.is_real:
+            res = "TwinPointer(Real)"
+        elif not self.is_twin:
+            res = "Pointer"
+        child_repr = (
+            self.syft_action_data._repr_markdown_()
+            if hasattr(self.syft_action_data, "_repr_markdown_")
+            else self.syft_action_data.__repr__()
+        )
+
+        return f"```python\n{res}\n```\n{child_repr}"
 
     def __repr__(self) -> str:
-        return self.__repr__()
+        if self.is_mock:
+            res = "TwinPointer(Mock)"
+        elif self.is_real:
+            res = "TwinPointer(Real)"
+        if not self.is_twin:
+            res = "Pointer"
+        return f"{res}:\n{str(self.syft_action_data)}"
+
+    def __call__(self, *args: Any, **kwds: Any) -> Any:
+        return self.__call__(*args, **kwds)
 
     def __str__(self) -> str:
         return self.__str__()
 
     def __len__(self) -> int:
         return self.__len__()
 
@@ -711,54 +1225,149 @@
 
     def __delattr__(self, key: Any) -> None:
         self.__delattr__(key)
 
     def __delitem__(self, key: Any) -> None:
         self.__delitem__(key)
 
-    def __invert__(self, other: Any) -> Any:
-        return self._syft_output_action_object(self.__invert__(other))
+    def __invert__(self) -> Any:
+        return self._syft_output_action_object(self.__invert__())
 
-    def __divmod__(self, other: Any) -> Any:
-        return self._syft_output_action_object(self.__divmod__(other))
+    def __round__(self) -> Any:
+        return self._syft_output_action_object(self.__round__())
 
-    def __truediv__(self, other: Any) -> Any:
-        return self._syft_output_action_object(self.__truediv__(other))
+    def __pos__(self) -> Any:
+        return self._syft_output_action_object(self.__pos__())
 
-    def __and__(self, other: Any) -> Any:
-        return self._syft_output_action_object(self.__and__(other))
+    def __trunc__(self) -> Any:
+        return self._syft_output_action_object(self.__trunc__())
+
+    def __divmod__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__divmod__(other))
 
     def __floordiv__(self, other: Any) -> Any:
         return self._syft_output_action_object(self.__floordiv__(other))
 
     def __mod__(self, other: Any) -> Any:
         return self._syft_output_action_object(self.__mod__(other))
 
+    def __abs__(self) -> Any:
+        return self._syft_output_action_object(self.__abs__())
+
+    def __neg__(self) -> Any:
+        return self._syft_output_action_object(self.__neg__())
+
+    def __or__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__or__(other))
+
+    def __and__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__and__(other))
+
+    def __xor__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__xor__(other))
+
+    def __pow__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__pow__(other))
+
+    def __truediv__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__truediv__(other))
+
+    def __lshift__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__lshift__(other))
+
+    def __rshift__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rshift__(other))
+
+    def __iter__(self):
+        return self._syft_output_action_object(self.__iter__())
+
+    def __next__(self):
+        return self._syft_output_action_object(self.__next__())
+
     # r ops
     # we want the underlying implementation so we should just call into __getattribute__
     def __radd__(self, other: Any) -> Any:
         return self.__radd__(other)
 
     def __rsub__(self, other: Any) -> Any:
         return self.__rsub__(other)
 
-    def __hash__(self) -> Any:
-        return self.__hash__().syft_action_data
+    def __rmul__(self, other: Any) -> Any:
+        return self.__rmul__(other)
 
     def __rmatmul__(self, other: Any) -> Any:
         return self.__rmatmul__(other)
 
+    def __rmod__(self, other: Any) -> Any:
+        return self.__rmod__(other)
+
+    def __ror__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__ror__(other))
+
+    def __rand__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rand__(other))
+
+    def __rxor__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rxor__(other))
+
+    def __rpow__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rpow__(other))
+
+    def __rtruediv__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rtruediv__(other))
+
+    def __rfloordiv__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rfloordiv__(other))
+
+    def __rlshift__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rlshift__(other))
+
+    def __rrshift__(self, other: Any) -> Any:
+        return self._syft_output_action_object(self.__rrshift__(other))
+
 
 @serializable()
 class AnyActionObject(ActionObject):
     __canonical_name__ = "AnyActionObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
-    syft_internal_type: ClassVar[Type[Any]] = Any  # type: ignore
-    syft_passthrough_attrs: List[str] = []
-    syft_dont_wrap_attrs: List[str] = []
+    syft_internal_type: ClassVar[Type[Any]] = NoneType  # type: ignore
+    # syft_passthrough_attrs: List[str] = []
+    syft_dont_wrap_attrs: List[str] = ["__str__", "__repr__"]
 
     def __float__(self) -> float:
         return float(self.syft_action_data)
 
+    def __int__(self) -> float:
+        return int(self.syft_action_data)
+
 
 action_types[Any] = AnyActionObject
+
+
+def debug_original_func(name: str, func: Callable) -> None:
+    debug(f"{name} func is:")
+    debug("inspect.isdatadescriptor", inspect.isdatadescriptor(func))
+    debug("inspect.isgetsetdescriptor", inspect.isgetsetdescriptor(func))
+    debug("inspect.isfunction", inspect.isfunction(func))
+    debug("inspect.isbuiltin", inspect.isbuiltin(func))
+    debug("inspect.ismethod", inspect.ismethod(func))
+    debug("inspect.ismethoddescriptor", inspect.ismethoddescriptor(func))
+
+
+def is_action_data_empty(obj: Any) -> bool:
+    if hasattr(obj, "syft_action_data"):
+        obj = obj.syft_action_data
+    if isinstance(obj, ActionDataEmpty):
+        return True
+    return False
+
+
+def has_action_data_empty(args: Any, kwargs: Any) -> bool:
+    for a in args:
+        if is_action_data_empty(a):
+            return True
+
+    for _, a in kwargs.items():
+        if is_action_data_empty(a):
+            return True
+    return False
```

### Comparing `syft-0.8.1b3/src/syft/external/__init__.py` & `syft-0.8.1b4/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/external/oblv/__init__.py` & `syft-0.8.1b4/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/external/oblv/deployment.py` & `syft-0.8.1b4/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/external/oblv/deployment_client.py` & `syft-0.8.1b4/src/syft/external/oblv/deployment_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,24 +69,24 @@
             )
         return oblv_client
 
 
 class DeploymentClient:
     deployment_id: str
     key_name: str
-    domain_clients: List[SyftClient] = []  # List of domain client objects
+    domain_clients: List[SyftClient]  # List of domain client objects
     oblv_client: OblvClient = None
     __conn_string: str
     __logs: Any
     __process: Any
     __enclave_client: SyftClient
 
     def __init__(
         self,
-        domain_clients: List[Any],
+        domain_clients: List[SyftClient],
         deployment_id: str,
         oblv_client: Optional[OblvClient] = None,
         key_name: Optional[str] = None,
         api: Optional[SyftAPI] = None,
     ):
         if not domain_clients:
             raise Exception(
```

### Comparing `syft-0.8.1b3/src/syft/external/oblv/exceptions.py` & `syft-0.8.1b4/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.1b4/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.1b4/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/external/oblv/oblv_service.py` & `syft-0.8.1b4/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/gevent_patch.py` & `syft-0.8.1b4/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/node/credentials.py` & `syft-0.8.1b4/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/node/gateway.py` & `syft-0.8.1b4/src/syft/node/gateway.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/node/node.py` & `syft-0.8.1b4/src/syft/node/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # future
 from __future__ import annotations
 
 # stdlib
+import binascii
 import contextlib
 from datetime import datetime
 from functools import partial
 import hashlib
 from multiprocessing import current_process
 import os
-import threading
 import traceback
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
+import uuid
 
 # third party
 import gevent
 import gipc
 from gipc.gipc import _GIPCDuplexHandle
 from nacl.signing import SigningKey
 from result import Err
@@ -47,32 +48,32 @@
 from ..service.context import NodeServiceContext
 from ..service.context import UnauthedServiceContext
 from ..service.context import UserLoginCredentials
 from ..service.data_subject.data_subject_member_service import DataSubjectMemberService
 from ..service.data_subject.data_subject_service import DataSubjectService
 from ..service.dataset.dataset_service import DatasetService
 from ..service.message.message_service import MessageService
-from ..service.metadata.metadata_service import MetadataService
-from ..service.metadata.metadata_stash import MetadataStash
 from ..service.metadata.node_metadata import NodeMetadata
 from ..service.network.network_service import NetworkService
 from ..service.policy.policy_service import PolicyService
-from ..service.project.project_service import NewProjectService
 from ..service.project.project_service import ProjectService
 from ..service.queue.queue import APICallMessageHandler
 from ..service.queue.queue import QueueManager
 from ..service.queue.queue_stash import QueueItem
 from ..service.queue.queue_stash import QueueStash
 from ..service.queue.zmq_queue import QueueConfig
 from ..service.queue.zmq_queue import ZMQQueueConfig
 from ..service.request.request_service import RequestService
 from ..service.response import SyftError
 from ..service.service import AbstractService
 from ..service.service import ServiceConfigRegistry
 from ..service.service import UserServiceConfigRegistry
+from ..service.settings.settings import NodeSettings
+from ..service.settings.settings_service import SettingsService
+from ..service.settings.settings_stash import SettingsStash
 from ..service.user.user import User
 from ..service.user.user import UserCreate
 from ..service.user.user_roles import ServiceRole
 from ..service.user.user_service import UserService
 from ..service.user.user_stash import UserStash
 from ..store.dict_document_store import DictStoreConfig
 from ..store.document_store import StoreConfig
@@ -80,23 +81,19 @@
 from ..store.sqlite_document_store import SQLiteStoreConfig
 from ..types.syft_object import HIGHEST_SYFT_OBJECT_VERSION
 from ..types.syft_object import LOWEST_SYFT_OBJECT_VERSION
 from ..types.syft_object import SyftObject
 from ..types.uid import UID
 from ..util.telemetry import instrument
 from ..util.util import random_name
+from ..util.util import thread_ident
 from .credentials import SyftSigningKey
 from .credentials import SyftVerifyKey
 from .worker_settings import WorkerSettings
 
-
-def thread_ident() -> int:
-    return threading.current_thread().ident
-
-
 # if user code needs to be serded and its not available we can call this to refresh
 # the code for a specific node UID and thread
 CODE_RELOADER: Dict[int, Callable] = {}
 
 
 def gipc_encoder(obj):
     return _serialize(obj, to_bytes=True)
@@ -193,26 +190,25 @@
 
         if name is None:
             name = random_name()
         self.name = name
         services = (
             [
                 UserService,
-                MetadataService,
+                SettingsService,
                 ActionService,
                 DatasetService,
                 UserCodeService,
                 RequestService,
                 DataSubjectService,
                 NetworkService,
                 PolicyService,
                 MessageService,
-                ProjectService,
                 DataSubjectMemberService,
-                NewProjectService,
+                ProjectService,
             ]
             if services is None
             else services
         )
 
         self.service_config = ServiceConfigRegistry.get_registered_configs()
         self.local_db = local_db
@@ -239,14 +235,15 @@
             node=self,
         )
 
         self.client_cache = {}
         self.node_type = node_type
 
         self.post_init()
+        self.create_initial_settings()
         if not (self.is_subprocess or self.processes == 0):
             self.init_queue_manager(queue_config=queue_config)
 
     def init_queue_manager(self, queue_config: QueueConfig):
         MessageHandlers = [APICallMessageHandler]
 
         self.queue_manager = QueueManager(queue_config)
@@ -266,15 +263,24 @@
         name: str,
         processes: int = 0,
         reset: bool = False,
         local_db: bool = False,
         sqlite_path: Optional[str] = None,
     ) -> Self:
         name_hash = hashlib.sha256(name.encode("utf8")).digest()
-        uid = UID(name_hash[0:16])
+        name_hash_uuid = name_hash[0:16]
+        name_hash_uuid = bytearray(name_hash_uuid)
+        name_hash_uuid[6] = (
+            name_hash_uuid[6] & 0x0F
+        ) | 0x40  # Set version to 4 (uuid4)
+        name_hash_uuid[8] = (name_hash_uuid[8] & 0x3F) | 0x80  # Set variant to RFC 4122
+        name_hash_string = binascii.hexlify(bytearray(name_hash_uuid)).decode("utf-8")
+        if uuid.UUID(name_hash_string).version != 4:
+            raise Exception(f"Invalid UID: {name_hash_string} for name: {name}")
+        uid = UID(name_hash_string)
         key = SyftSigningKey(SigningKey(name_hash))
         if reset:
             store_config = SQLiteStoreClientConfig()
             store_config.filename = f"{uid}.sqlite"
 
             # stdlib
             import sqlite3
@@ -410,25 +416,24 @@
 
         for service_klass in self.services:
             kwargs = {}
             if service_klass == ActionService:
                 kwargs["store"] = self.action_store
             store_services = [
                 UserService,
-                MetadataService,
+                SettingsService,
                 DatasetService,
                 UserCodeService,
                 RequestService,
                 DataSubjectService,
                 NetworkService,
                 PolicyService,
                 MessageService,
-                ProjectService,
                 DataSubjectMemberService,
-                NewProjectService,
+                ProjectService,
             ]
 
             if OBLV:
                 # relative
                 from ..external.oblv.oblv_service import OblvService
 
                 store_services += [OblvService]
@@ -461,21 +466,27 @@
         method_name = path_list.pop()
         service_obj = self._get_service_from_path(path=path)
 
         return getattr(service_obj, method_name)
 
     @property
     def metadata(self) -> NodeMetadata:
+        settings_stash = SettingsStash(store=self.document_store)
+        settings = settings_stash.get_all(self.signing_key.verify_key).ok()[0]
         return NodeMetadata(
-            name=self.name,
+            name=settings.name,
             id=self.id,
             verify_key=self.verify_key,
             highest_object_version=HIGHEST_SYFT_OBJECT_VERSION,
             lowest_object_version=LOWEST_SYFT_OBJECT_VERSION,
             syft_version=__version__,
+            deployed_on=settings.deployed_on,
+            description=settings.description,
+            organization=settings.organization,
+            on_board=settings.on_board,
         )
 
     @property
     def icon(self) -> str:
         return "🦾"
 
     @property
@@ -494,14 +505,15 @@
 
         return True
 
     def resolve_future(
         self, credentials: SyftVerifyKey, uid: UID
     ) -> Union[Optional[QueueItem], SyftError]:
         result = self.queue_stash.pop_on_complete(credentials, uid)
+
         if result.is_ok():
             return result.ok()
         return result.err()
 
     def forward_message(
         self, api_call: Union[SyftAPICall, SignedSyftAPICall]
     ) -> Result[Union[QueueItem, SyftObject], Err]:
@@ -515,15 +527,15 @@
             )
 
         client = None
         if node_uid in self.client_cache:
             client = self.client_cache[node_uid]
         else:
             network_service = self.get_service(NetworkService)
-            peer = network_service.stash.get_by_uid(node_uid)
+            peer = network_service.stash.get_by_uid(self.verify_key, node_uid)
 
             if peer.is_ok() and peer.ok():
                 peer = peer.ok()
                 context = NodeServiceContext(node=self)
                 client = peer.client_with_context(context=context)
                 self.client_cache[node_uid] = client
 
@@ -557,15 +569,14 @@
             )
         else:
             if not api_call.is_valid:
                 return SyftError(message="Your message signature is invalid")  # type: ignore
 
         if api_call.message.node_uid != self.id:
             return self.forward_message(api_call=api_call)
-
         if api_call.message.path == "queue":
             return self.resolve_future(
                 credentials=api_call.credentials, uid=api_call.message.kwargs["uid"]
             )
 
         if api_call.message.path == "metadata":
             return self.metadata
@@ -628,14 +639,34 @@
         return partial(method, context=context)
 
     def get_unauthed_context(
         self, login_credentials: UserLoginCredentials
     ) -> NodeServiceContext:
         return UnauthedServiceContext(node=self, login_credentials=login_credentials)
 
+    def create_initial_settings(self) -> Optional[NodeSettings]:
+        try:
+            settings_stash = SettingsStash(store=self.document_store)
+            settings_exists = settings_stash.get_all(self.signing_key.verify_key).ok()
+            if settings_exists:
+                return None
+            else:
+                new_settings = NodeSettings(
+                    name=self.name,
+                    deployed_on=datetime.now().date().strftime("%m/%d/%Y"),
+                )
+                result = settings_stash.set(
+                    credentials=self.signing_key.verify_key, settings=new_settings
+                )
+                if result.is_ok():
+                    return result.ok()
+                return None
+        except Exception as e:
+            print("create_worker_metadata failed", e)
+
 
 def task_producer(
     pipe: _GIPCDuplexHandle, api_call: SyftAPICall, blocking: bool
 ) -> Any:
     try:
         result = None
         with pipe:
@@ -676,15 +707,15 @@
             result = worker.handle_api_call(api_call)
             if blocking:
                 pipe.put(result)
             else:
                 item = QueueItem(
                     node_uid=worker.id, id=task_uid, result=result, resolved=True
                 )
-                worker.queue_stash.set_result(item)
+                worker.queue_stash.set_result(worker.verify_key, item)
                 worker.queue_stash.partition.close()
             pipe.close()
     except Exception as e:
         print("Exception in task_runner", e)
         raise e
 
 
@@ -710,42 +741,14 @@
         process.join()
 
     if blocking:
         return producer.value
     return None
 
 
-def create_worker_metadata(
-    worker: AbstractNode,
-) -> Optional[NodeMetadata]:
-    try:
-        metadata_stash = MetadataStash(store=worker.document_store)
-        metadata_exists = metadata_stash.get_all(worker.signing_key.verify_key).ok()
-        if metadata_exists:
-            return None
-        else:
-            new_metadata = NodeMetadata(
-                name=worker.name,
-                id=worker.id,
-                verify_key=worker.signing_key.verify_key,
-                highest_object_version=HIGHEST_SYFT_OBJECT_VERSION,
-                lowest_object_version=LOWEST_SYFT_OBJECT_VERSION,
-                syft_version=__version__,
-                deployed_on=datetime.now().date().strftime("%m/%d/%Y"),
-            )
-            result = metadata_stash.set(
-                credentials=worker.signing_key.verify_key, metadata=new_metadata
-            )
-            if result.is_ok():
-                return result.ok()
-            return None
-    except Exception as e:
-        print("create_worker_metadata failed", e)
-
-
 def create_admin_new(
     name: str,
     email: str,
     password: str,
     node: AbstractNode,
 ) -> Optional[User]:
     try:
```

### Comparing `syft-0.8.1b3/src/syft/node/routes.py` & `syft-0.8.1b4/src/syft/node/routes.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 # relative
 from ..abstract_node import AbstractNode
 from ..serde.deserialize import _deserialize as deserialize
 from ..serde.serialize import _serialize as serialize
 from ..service.context import NodeServiceContext
 from ..service.context import UnauthedServiceContext
-from ..service.metadata.metadata_service import MetadataService
 from ..service.metadata.node_metadata import NodeMetadataJSON
 from ..service.response import SyftError
 from ..service.user.user import UserCreate
 from ..service.user.user import UserPrivateKey
 from ..service.user.user_service import UserService
 from ..util.telemetry import TRACE_MODE
 from .credentials import SyftVerifyKey
@@ -59,19 +58,17 @@
     # provide information about the node in JSON
     @router.get("/metadata", response_class=JSONResponse)
     def syft_metadata() -> JSONResponse:
         return worker.metadata.to(NodeMetadataJSON)
 
     @router.get("/metadata_capnp")
     def syft_metadata_capnp() -> Response:
-        context = NodeServiceContext(node=worker)
-        method = worker.get_method_with_context(MetadataService.get, context)
-        result = method()
+        result = worker.metadata
         return Response(
-            serialize(result.ok(), to_bytes=True),
+            serialize(result, to_bytes=True),
             media_type="application/octet-stream",
         )
 
     def handle_syft_new_api(user_verify_key: SyftVerifyKey) -> Response:
         return Response(
             serialize(worker.get_api(user_verify_key), to_bytes=True),
             media_type="application/octet-stream",
@@ -98,15 +95,15 @@
             serialize(result, to_bytes=True),
             media_type="application/octet-stream",
         )
 
     # make a request to the SyftAPI
     @router.post("/api_call")
     def syft_new_api_call(
-        request: Request, data: bytes = Depends(get_body)
+        request: Request, data: bytes = Depends(get_body)  # noqa: B008
     ) -> Response:
         if TRACE_MODE:
             with trace.get_tracer(syft_new_api_call.__module__).start_as_current_span(
                 syft_new_api_call.__qualname__,
                 context=extract(request.headers),
                 kind=trace.SpanKind.SERVER,
             ):
@@ -160,29 +157,31 @@
             media_type="application/octet-stream",
         )
 
     # exchange email and password for a SyftSigningKey
     @router.post("/login", name="login", status_code=200)
     def login(
         request: Request,
-        email: str = Body(..., example="info@openmined.org"),
-        password: str = Body(..., example="changethis"),
+        email: str = Body(..., example="info@openmined.org"),  # noqa: B008
+        password: str = Body(..., example="changethis"),  # noqa: B008
     ) -> Any:
         if TRACE_MODE:
             with trace.get_tracer(login.__module__).start_as_current_span(
                 login.__qualname__,
                 context=extract(request.headers),
                 kind=trace.SpanKind.SERVER,
             ):
                 return handle_login(email, password, worker)
         else:
             return handle_login(email, password, worker)
 
     @router.post("/register", name="register", status_code=200)
-    def register(request: Request, data: bytes = Depends(get_body)) -> Any:
+    def register(
+        request: Request, data: bytes = Depends(get_body)  # noqa: B008
+    ) -> Any:
         if TRACE_MODE:
             with trace.get_tracer(register.__module__).start_as_current_span(
                 register.__qualname__,
                 context=extract(request.headers),
                 kind=trace.SpanKind.SERVER,
             ):
                 return handle_register(data, worker)
```

### Comparing `syft-0.8.1b3/src/syft/node/run.py` & `syft-0.8.1b4/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/node/server.py` & `syft-0.8.1b4/src/syft/node/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,31 +10,41 @@
 from typing import Callable
 from typing import List
 from typing import Tuple
 
 # third party
 from fastapi import APIRouter
 from fastapi import FastAPI
+import requests
 from starlette.middleware.cors import CORSMiddleware
 import uvicorn
 
 # relative
+from ..client.client import API_PATH
+from ..util.util import os_name
 from .domain import Domain
 from .routes import make_routes
 
+if os_name() == "macOS":
+    # needed on MacOS to prevent [__NSCFConstantString initialize] may have been in
+    # progress in another thread when fork() was called.
+    multiprocessing.set_start_method("spawn", True)
+
+WAIT_TIME_SECONDS = 20
+
 
 def make_app(name: str, router: APIRouter) -> FastAPI:
     app = FastAPI(
         title=name,
     )
 
     api_router = APIRouter()
-    api_router.include_router(router, prefix="/new", tags=["new"])
 
-    app.include_router(api_router, prefix="/api/v1")
+    api_router.include_router(router)
+    app.include_router(api_router, prefix="/api/v2")
 
     app.add_middleware(
         CORSMiddleware,
         allow_origins=["*"],
         allow_credentials=True,
         allow_methods=["*"],
         allow_headers=["*"],
@@ -69,15 +79,17 @@
                 print(f"Failed to kill python process on port: {port}")
 
         log_level = "critical"
         if dev_mode:
             log_level = "info"
             logging.getLogger("uvicorn").setLevel(logging.CRITICAL)
             logging.getLogger("uvicorn.access").setLevel(logging.CRITICAL)
-        config = uvicorn.Config(app, host=host, port=port, log_level=log_level)
+        config = uvicorn.Config(
+            app, host=host, port=port, log_level=log_level, reload=dev_mode
+        )
         server = uvicorn.Server(config)
 
         await server.serve()
         asyncio.get_running_loop().stop()
 
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
@@ -101,23 +113,36 @@
         print(f"Stopping {name}")
         server_process.terminate()
         server_process.join()
 
     def start():
         print(f"Starting {name} server on {host}:{port}")
         server_process.start()
+
         if tail:
             try:
                 while True:
                     time.sleep(1)
             except KeyboardInterrupt:
                 try:
                     stop()
                 except SystemExit:
                     os._exit(130)
+        else:
+            for _ in range(WAIT_TIME_SECONDS):
+                try:
+                    req = requests.get(
+                        f"http://{host}:{port}{API_PATH}/metadata", timeout=0.5
+                    )
+                    if req.status_code == 200:
+                        print("Server Started")
+                        break
+                except Exception:
+                    time.sleep(1)
+                    print("Waiting for server to start")
 
     return start, stop
 
 
 def find_python_processes_on_port(port: int) -> List[int]:
     system = platform.system()
```

### Comparing `syft-0.8.1b3/src/syft/node/worker_settings.py` & `syft-0.8.1b4/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/serde/array.py` & `syft-0.8.1b4/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/serde/arrow.py` & `syft-0.8.1b4/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/serde/deserialize.py` & `syft-0.8.1b4/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/serde/lib_permissions.py` & `syft-0.8.1b4/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/serde/lib_service_registry.py` & `syft-0.8.1b4/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/serde/mock.py` & `syft-0.8.1b4/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/serde/recursive.py` & `syft-0.8.1b4/src/syft/serde/recursive.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # stdlib
 from enum import Enum
 import sys
-import threading
 import types
 from typing import Any
 from typing import Callable
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Type
@@ -24,16 +23,33 @@
 from .capnp import get_capnp_schema
 
 TYPE_BANK = {}
 
 recursive_scheme = get_capnp_schema("recursive_serde.capnp").RecursiveSerde  # type: ignore
 
 
-def thread_ident() -> int:
-    return int(threading.current_thread().ident)
+def get_types(cls: Type, keys: Optional[List[str]] = None) -> Optional[List[Type]]:
+    if keys is None:
+        return None
+    types = []
+    for key in keys:
+        _type = None
+        annotations = getattr(cls, "__annotations__", None)
+        if annotations and key in annotations:
+            _type = annotations[key]
+        else:
+            for parent_cls in cls.mro():
+                sub_annotations = getattr(parent_cls, "__annotations__", None)
+                if sub_annotations and key in sub_annotations:
+                    _type = sub_annotations[key]
+        if _type is None:
+            print(f"Failed to find type for key: {key} in {cls}")
+            return None
+        types.append(_type)
+    return types
 
 
 def recursive_serde_register(
     cls: Union[object, type],
     serialize: Optional[Callable] = None,
     deserialize: Optional[Callable] = None,
     serialize_attrs: Optional[List] = None,
@@ -77,28 +93,30 @@
 
     exclude_attrs = [] if exclude_attrs is None else exclude_attrs
     attribute_list = attribute_list - set(exclude_attrs)
 
     if inheritable_attrs and attribute_list and not is_pydantic:
         # only set __syft_serializable__ for non-pydantic classes because
         # pydantic objects inherit by default
-        setattr(cls, "__syft_serializable__", attribute_list)
+        cls.__syft_serializable__ = attribute_list
 
     attributes = set(list(attribute_list)) if attribute_list else None
+    attribute_types = get_types(cls, attributes)
     serde_overrides = getattr(cls, "__serde_overrides__", {})
 
     # without fqn duplicate class names overwrite
     TYPE_BANK[fqn] = (
         nonrecursive,
         _serialize,
         _deserialize,
         attributes,
         exclude_attrs,
         serde_overrides,
         cls,
+        attribute_types,
     )
 
 
 def chunk_bytes(
     data: bytes, field_name: Union[str, int], builder: _DynamicStructBuilder
 ) -> None:
     CHUNK_SIZE = int(5.12e8)  # capnp max for a List(Data) field
@@ -136,14 +154,15 @@
         nonrecursive,
         serialize,
         deserialize,
         attribute_list,
         exclude_attrs_list,
         serde_overrides,
         cls,
+        attribute_types,
     ) = TYPE_BANK[fqn]
 
     if nonrecursive or is_type:
         if serialize is None:
             raise Exception(
                 f"Cant serialize {type(self)} nonrecursive without serialize."
             )
@@ -228,14 +247,15 @@
         nonrecursive,
         serialize,
         deserialize,
         attribute_list,
         exclude_attrs_list,
         serde_overrides,
         cls,
+        attribute_types,
     ) = TYPE_BANK[proto.fullyQualifiedName]
 
     if class_type == type(None):
         # yes this looks stupid but it works and the opposite breaks
         class_type = cls
 
     if nonrecursive:
@@ -255,15 +275,15 @@
             transforms = serde_overrides.get(attr_name, None)
 
             if transforms is not None:
                 attr_value = transforms[1](attr_value)
             kwargs[attr_name] = attr_value
 
     if hasattr(class_type, "serde_constructor"):
-        return getattr(class_type, "serde_constructor")(kwargs)
+        return class_type.serde_constructor(kwargs)
 
     if issubclass(class_type, Enum) and "value" in kwargs:
         obj = class_type.__new__(class_type, kwargs["value"])  # type: ignore
     elif issubclass(class_type, BaseModel):
         # if we skip the __new__ flow of BaseModel we get the error
         # AttributeError: object has no attribute '__fields_set__'
```

### Comparing `syft-0.8.1b3/src/syft/serde/recursive_primitives.py` & `syft-0.8.1b4/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/serde/serializable.py` & `syft-0.8.1b4/src/syft/serde/serializable.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 def serializable(
     attrs: Optional[List[str]] = None,
     without: Optional[List[str]] = None,
     inherit: Optional[bool] = True,
     inheritable: Optional[bool] = True,
-) -> Callable:
+) -> Callable[[T], T]:
     """
     Recursively serialize attributes of the class.
 
     Args:
         `attrs`       : List of attributes to serialize
         `without`     : List of attributes to exclude from serialization
         `inherit`     : Whether to inherit serializable attribute list from base class
```

### Comparing `syft-0.8.1b3/src/syft/serde/signature.py` & `syft-0.8.1b4/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/serde/third_party.py` & `syft-0.8.1b4/src/syft/serde/third_party.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,20 @@
     ),
 )
 
 # unsure why we have to register the object not the type but this works
 recursive_serde_register(np.core._ufunc_config._unspecified())
 
 recursive_serde_register(
+    pydantic.networks.EmailStr,
+    serialize=lambda x: x.encode(),
+    deserialize=lambda x: pydantic.networks.EmailStr(x.decode()),
+)
+
+recursive_serde_register(
     zmq._Socket,
     serialize_attrs=[
         "_shadow",
         "_monitor_socket",
         "_type_name",
     ],
 )
```

### Comparing `syft-0.8.1b3/src/syft/service/action/action_graph.py` & `syft-0.8.1b4/src/syft/service/action/action_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from typing import Type
 from typing import Union
 
 # third party
 import matplotlib.pyplot as plt
 import networkx as nx
 import pydantic
+from pydantic import Field
+from pydantic import validator
 from result import Err
 from result import Ok
 from result import Result
 from typing_extensions import Self
 
 # relative
 from ...node.credentials import SyftVerifyKey
@@ -184,31 +186,28 @@
 
     def topological_sort(self, subgraph: Any) -> Any:
         raise NotImplementedError
 
 
 @serializable()
 class InMemoryStoreClientConfig(StoreClientConfig):
-    filename: Optional[str] = None
-    path: Union[str, Path]
+    filename: str = "action_graph.bytes"
+    path: Union[str, Path] = Field(default_factory=tempfile.gettempdir)
 
-    def __init__(
-        self,
-        filename: Optional[str] = None,
-        path: Optional[Union[str, Path]] = None,
-        *args,
-        **kwargs,
-    ):
-        path_ = tempfile.gettempdir() if path is None else path
-        filename_ = "action_graph.bytes" if filename is None else filename
-        super().__init__(filename=filename_, path=path_, *args, **kwargs)
+    # We need this in addition to Field(default_factory=...)
+    # so users can still do InMemoryStoreClientConfig(path=None)
+    @validator("path", pre=True)
+    def __default_path(cls, path: Optional[Union[str, Path]]) -> Union[str, Path]:
+        if path is None:
+            return tempfile.gettempdir()
+        return path
 
     @property
-    def file_path(self) -> Optional[Path]:
-        return Path(self.path) / self.filename if self.filename is not None else None
+    def file_path(self) -> Path:
+        return Path(self.path) / self.filename
 
 
 @serializable(without=["_lock"])
 class NetworkXBackingStore(BaseGraphStore):
     def __init__(self, store_config: StoreConfig, reset: bool = False) -> None:
         self.path_str = store_config.client_config.file_path.as_posix()
 
@@ -363,20 +362,24 @@
             self.store_config, reset
         )
 
     def set(
         self,
         node: NodeActionData,
         credentials: SyftVerifyKey,
-        parent_uids: List[UID] = [],
+        parent_uids: Optional[List[UID]] = None,
     ) -> Result[NodeActionData, str]:
         if self.graph.exists(uid=node.id):
             return Err(f"Node already exists in the graph: {node}")
 
         self.graph.set(uid=node.id, data=node)
+
+        if parent_uids is None:
+            parent_uids = []
+
         for parent_uid in parent_uids:
             result = self.add_edge(
                 parent=parent_uid,
                 child=node.id,
                 credentials=credentials,
             )
             if result.is_err():
```

### Comparing `syft-0.8.1b3/src/syft/service/action/action_graph_service.py` & `syft-0.8.1b4/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/action/action_permissions.py` & `syft-0.8.1b4/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/action/action_service.py` & `syft-0.8.1b4/src/syft/service/action/action_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,15 @@
     def _get(
         self,
         context: AuthedServiceContext,
         uid: UID,
         twin_mode: TwinMode = TwinMode.PRIVATE,
         has_permission=False,
     ) -> Result[ActionObject, str]:
-        # TODO 🟣 Temporarily added skip permission arguments for enclave
-        # until permissions are fully integrated
+        """Get an object from the action store"""
         result = self.store.get(
             uid=uid, credentials=context.credentials, has_permission=has_permission
         )
         if result.is_ok():
             obj = result.ok()
             if isinstance(obj, TwinObject):
                 if twin_mode == TwinMode.PRIVATE:
```

### Comparing `syft-0.8.1b3/src/syft/service/action/action_store.py` & `syft-0.8.1b4/src/syft/service/action/action_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,16 +62,14 @@
         self.root_verify_key = root_verify_key
 
     def get(
         self, uid: UID, credentials: SyftVerifyKey, has_permission=False
     ) -> Result[SyftObject, str]:
         uid = uid.id  # We only need the UID from LineageID or UID
 
-        # TODO 🟣 Temporarily added skip permission argument for enclave
-        # until permissions are fully integrated
         # if you get something you need READ permission
         read_permission = ActionObjectREAD(uid=uid, credentials=credentials)
         if has_permission or self.has_permission(read_permission):
             try:
                 if isinstance(uid, LineageID):
                     syft_object = self.data[uid.id]
                 elif isinstance(uid, UID):
```

### Comparing `syft-0.8.1b3/src/syft/service/action/action_types.py` & `syft-0.8.1b4/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/action/numpy.py` & `syft-0.8.1b4/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/action/pandas.py` & `syft-0.8.1b4/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/action/plan.py` & `syft-0.8.1b4/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/action/verification.py` & `syft-0.8.1b4/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/code/unparse.py` & `syft-0.8.1b4/src/syft/service/code/unparse.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # this fixes the bug in ast.unparse https://github.com/IBM/lale/pull/738/files
 
 
 class FixUnparser(astunparse.Unparser):
     def _Constant(self, t: _ast.expr) -> None:
         if not hasattr(t, "kind"):
-            setattr(t, "kind", None)
+            t.kind = None
 
         super()._Constant(t)
 
 
 def unparse(tree: _ast.Module) -> str:
     if sys.version_info >= (3, 9):
         return ast.unparse(tree)
```

### Comparing `syft-0.8.1b3/src/syft/service/code/user_code.py` & `syft-0.8.1b4/src/syft/service/code/user_code.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,28 +28,30 @@
 from ...serde.deserialize import _deserialize
 from ...serde.serializable import serializable
 from ...serde.serialize import _serialize
 from ...store.document_store import PartitionKey
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
+from ...types.transforms import add_node_uid_for_key
 from ...types.transforms import generate_id
 from ...types.transforms import transform
 from ...types.uid import UID
 from ..context import AuthedServiceContext
 from ..dataset.dataset import Asset
 from ..metadata.node_metadata import EnclaveMetadata
 from ..policy.policy import CustomInputPolicy
 from ..policy.policy import CustomOutputPolicy
 from ..policy.policy import InputPolicy
 from ..policy.policy import OutputPolicy
 from ..policy.policy import Policy
 from ..policy.policy import SubmitUserPolicy
 from ..policy.policy import UserPolicy
 from ..policy.policy import init_policy
+from ..policy.policy import load_policy_code
 from ..policy.policy_service import PolicyService
 from ..response import SyftError
 from .code_parse import GlobalsVisitor
 from .unparse import unparse
 
 UserVerifyKeyPartitionKey = PartitionKey(key="user_verify_key", type_=SyftVerifyKey)
 CodeHashPartitionKey = PartitionKey(key="code_hash", type_=int)
@@ -145,15 +147,15 @@
     def mutate(
         self, value: UserCodeStatus, node_name: str, verify_key: SyftVerifyKey
     ) -> Result[Ok, Err]:
         node_view = NodeView(node_name=node_name, verify_key=verify_key)
         base_dict = self.base_dict
         if node_view in base_dict:
             base_dict[node_view] = value
-            setattr(self, "base_dict", base_dict)
+            self.base_dict = base_dict
             return Ok(self)
         else:
             return Err(
                 "Cannot Modify Status as the Domain's data is not included in the request"
             )
 
 
@@ -304,15 +306,15 @@
             return SyftError(message=f"You must login to {self.node_uid}")
 
         node_view = NodeView(
             node_name=api.node_name, verify_key=api.signing_key.verify_key
         )
         inputs = self.input_policy_init_kwargs[node_view]
         all_assets = []
-        for k, uid in inputs.items():
+        for uid in inputs.values():
             if isinstance(uid, UID):
                 assets = api.services.dataset.get_assets_by_action_id(uid)
                 if not isinstance(assets, list):
                     return assets
 
                 all_assets += assets
         return all_assets
@@ -476,15 +478,15 @@
     return unparse(wrapper_function)
 
 
 def new_check_code(context: TransformContext) -> TransformContext:
     # TODO remove this tech debt hack
     input_kwargs = context.output["input_policy_init_kwargs"]
     node_view_workaround = False
-    for k, v in input_kwargs.items():
+    for k in input_kwargs.keys():
         if isinstance(k, NodeView):
             node_view_workaround = True
 
     if not node_view_workaround:
         input_keys = list(input_kwargs.keys())
     else:
         input_keys = []
@@ -565,15 +567,15 @@
 
 def add_custom_status(context: TransformContext) -> TransformContext:
     input_keys = list(context.output["input_policy_init_kwargs"].keys())
     if context.node.node_type == NodeType.DOMAIN:
         node_view = NodeView(
             node_name=context.node.name, verify_key=context.node.signing_key.verify_key
         )
-        if node_view in input_keys:
+        if node_view in input_keys or len(input_keys) == 0:
             context.output["status"] = UserCodeStatusContext(
                 base_dict={node_view: UserCodeStatus.SUBMITTED}
             )
         else:
             raise NotImplementedError
     elif context.node.node_type == NodeType.ENCLAVE:
         base_dict = {key: UserCodeStatus.SUBMITTED for key in input_keys}
@@ -591,14 +593,15 @@
         hash_code,
         generate_unique_func_name,
         check_input_policy,
         check_output_policy,
         new_check_code,
         add_credentials_for_key("user_verify_key"),
         add_custom_status,
+        add_node_uid_for_key("node_uid"),
     ]
 
 
 @serializable()
 class UserCodeExecutionResult(SyftObject):
     # version
     __canonical_name__ = "UserCodeExecutionResult"
@@ -642,7 +645,20 @@
         )
 
     except Exception as e:
         print("execute_byte_code failed", e, file=stderr_)
     finally:
         sys.stdout = stdout_
         sys.stderr = stderr_
+
+
+def load_approved_policy_code(user_code_items: List[UserCode]) -> Any:
+    """Reload the policy code in memory for user code that is approved."""
+    try:
+        for user_code in user_code_items:
+            if user_code.status.approved:
+                if isinstance(user_code.input_policy_type, UserPolicy):
+                    load_policy_code(user_code.input_policy_type)
+                if isinstance(user_code.output_policy_type, UserPolicy):
+                    load_policy_code(user_code.output_policy_type)
+    except Exception as e:
+        raise Exception(f"Failed to load code: {user_code}: {e}")
```

### Comparing `syft-0.8.1b3/src/syft/service/code/user_code_parse.py` & `syft-0.8.1b4/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/code/user_code_service.py` & `syft-0.8.1b4/src/syft/service/code/user_code_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,44 +12,43 @@
 from ...store.document_store import DocumentStore
 from ...store.linked_obj import LinkedObject
 from ...types.twin_object import TwinObject
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..context import AuthedServiceContext
 from ..policy.policy import OutputHistory
-from ..policy.policy import UserPolicy
-from ..policy.policy import load_policy_code
 from ..request.request import SubmitRequest
 from ..request.request import UserCodeStatusChange
 from ..request.request_service import RequestService
 from ..response import SyftError
 from ..response import SyftNotReady
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from .user_code import SubmitUserCode
 from .user_code import UserCode
 from .user_code import UserCodeStatus
+from .user_code import load_approved_policy_code
 from .user_code_stash import UserCodeStash
 
 
 @instrument
 @serializable()
 class UserCodeService(AbstractService):
     store: DocumentStore
     stash: UserCodeStash
 
     def __init__(self, store: DocumentStore) -> None:
         self.store = store
         self.stash = UserCodeStash(store=store)
 
-    @service_method(path="code.submit", name="submit")
+    @service_method(path="code.submit", name="submit", roles=GUEST_ROLE_LEVEL)
     def submit(
         self, context: AuthedServiceContext, code: SubmitUserCode
     ) -> Union[UserCode, SyftError]:
         """Add User Code"""
         result = self.stash.set(context.credentials, code.to(UserCode, context=context))
         if result.is_err():
             return SyftError(message=str(result.err()))
@@ -133,20 +132,15 @@
             return SyftSuccess(message="Code State Updated")
         return SyftError(message="Unable to Update Code State")
 
     def load_user_code(self, context: AuthedServiceContext) -> None:
         result = self.stash.get_all(credentials=context.credentials)
         if result.is_ok():
             user_code_items = result.ok()
-            for user_code in user_code_items:
-                if user_code.status.approved:
-                    if isinstance(user_code.input_policy_type, UserPolicy):
-                        load_policy_code(user_code.input_policy_type)
-                    if isinstance(user_code.output_policy_type, UserPolicy):
-                        load_policy_code(user_code.output_policy_type)
+            load_approved_policy_code(user_code_items=user_code_items)
 
     @service_method(path="code.call", name="call", roles=GUEST_ROLE_LEVEL)
     def call(
         self, context: AuthedServiceContext, uid: UID, **kwargs: Any
     ) -> Union[SyftSuccess, SyftError]:
         """Call a User Code Function"""
         try:
```

### Comparing `syft-0.8.1b3/src/syft/service/code/user_code_stash.py` & `syft-0.8.1b4/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/context.py` & `syft-0.8.1b4/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/data_subject/data_subject.py` & `syft-0.8.1b4/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.1b4/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.1b4/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.1b4/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/dataset/dataset.py` & `syft-0.8.1b4/src/syft/service/dataset/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     action_id: UID
     node_uid: UID
     name: str
     description: Optional[str]
     contributors: List[Contributor] = []
     data_subjects: List[DataSubject] = []
     mock_is_real: bool = False
-    shape: Tuple
+    shape: Optional[Tuple]
 
     # @property
     # def pointer(self) -> ActionObjectPointer:
     #     api = APIRegistry.api_for(node_uid=self.node_uid)
     #     obj_ptr = api.services.action.get_pointer(uid=self.action_id)
     #     return obj_ptr
 
@@ -87,14 +87,30 @@
         _repr_str += f"Shape: {self.shape}\n"
         _repr_str += f"Contributors: {len(self.contributors)}\n"
         for contributor in self.contributors:
             _repr_str += f"\t{contributor.name}: {contributor.email}\n"
         return "```python\n" + _repr_str + "\n```"
 
     @property
+    def pointer(self) -> Any:
+        # relative
+        from ...client.api import APIRegistry
+
+        api = APIRegistry.api_for(node_uid=self.node_uid)
+        return api.services.action.get_pointer(self.action_id)
+
+    @property
+    def mock_data(self) -> Any:
+        # relative
+        from ...client.api import APIRegistry
+
+        api = APIRegistry.api_for(node_uid=self.node_uid)
+        return api.services.action.get_pointer(self.action_id).syft_action_data
+
+    @property
     def mock(self) -> Any:
         # relative
         from ...client.api import APIRegistry
 
         api = APIRegistry.api_for(node_uid=self.node_uid)
         return api.services.action.get_pointer(self.action_id)
 
@@ -103,14 +119,33 @@
         # relative
         from ...client.api import APIRegistry
 
         api = APIRegistry.api_for(node_uid=self.node_uid)
         return api.services.action.get(self.action_id)
 
 
+def is_action_data_empty(mock: Any) -> bool:
+    # relative
+    from ...service.action.action_data_empty import ActionDataEmpty
+    from ...service.action.action_object import AnyActionObject
+
+    if isinstance(mock, AnyActionObject) and isinstance(
+        mock.syft_action_data, ActionDataEmpty
+    ):
+        return True
+    return False
+
+
+def check_mock(data: Any, mock: Any) -> bool:
+    if type(data) == type(mock):
+        return True
+
+    return is_action_data_empty(mock)
+
+
 @serializable()
 class CreateAsset(SyftObject):
     # version
     __canonical_name__ = "CreateAsset"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: Optional[UID] = None
@@ -156,24 +191,25 @@
         self.mock = mock_data
         self.mock_is_real = mock_is_real
 
     def set_shape(self, shape: Tuple) -> None:
         self.shape = shape
 
     def check(self) -> Union[SyftSuccess, SyftError]:
-        if type(self.data) != type(self.mock):  # noqa: E721
+        if not check_mock(self.data, self.mock):
             return SyftError(
                 message=f"set_obj type {type(self.data)} must match set_mock type {type(self.mock)}"
             )
-        data_shape = get_shape_or_len(self.data)
-        mock_shape = get_shape_or_len(self.mock)
-        if data_shape != mock_shape:
-            return SyftError(
-                message=f"set_obj shape {data_shape} must match set_mock shape {mock_shape}"
-            )
+        if not is_action_data_empty(self.mock):
+            data_shape = get_shape_or_len(self.data)
+            mock_shape = get_shape_or_len(self.mock)
+            if data_shape != mock_shape:
+                return SyftError(
+                    message=f"set_obj shape {data_shape} must match set_mock shape {mock_shape}"
+                )
 
         return SyftSuccess(message="Dataset is Valid")
 
 
 def get_shape_or_len(obj: Any) -> Optional[Union[Tuple[int, ...], int]]:
     if hasattr(obj, "shape"):
         shape = getattr(obj, "shape", None)
@@ -331,15 +367,16 @@
         private_obj = context.output.pop("data", None)
         mock_obj = context.output.pop("mock", None)
     return context
 
 
 def infer_shape(context: TransformContext) -> TransformContext:
     if context.output["shape"] is None:
-        context.output["shape"] = get_shape_or_len(context.obj.mock)
+        if not is_action_data_empty(context.obj.mock):
+            context.output["shape"] = get_shape_or_len(context.obj.mock)
     return context
 
 
 def set_data_subjects(context: TransformContext) -> TransformContext:
     data_subjects = context.output["data_subjects"]
     get_data_subject = context.node.get_service_method(DataSubjectService.get_by_name)
```

### Comparing `syft-0.8.1b3/src/syft/service/dataset/dataset_service.py` & `syft-0.8.1b4/src/syft/service/dataset/dataset_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # stdlib
 from typing import List
+from typing import Optional
 from typing import Union
 
 # relative
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...types.uid import UID
 from ...util.telemetry import instrument
@@ -50,38 +51,66 @@
             ],
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="Dataset Added")
 
     @service_method(path="dataset.get_all", name="get_all", roles=GUEST_ROLE_LEVEL)
-    def get_all(self, context: AuthedServiceContext) -> Union[List[Dataset], SyftError]:
+    def get_all(
+        self,
+        context: AuthedServiceContext,
+        page_size: Optional[int] = 0,
+        page_index: Optional[int] = 0,
+    ) -> Union[List[Dataset], SyftError]:
         """Get a Dataset"""
         result = self.stash.get_all(context.credentials)
         if result.is_ok():
             datasets = result.ok()
             results = []
             for dataset in datasets:
                 dataset.node_uid = context.node.id
                 results.append(dataset)
+
+            # If chunk size is defined, then split list into evenly sized chunks
+            if page_size:
+                results = [
+                    results[i : i + page_size]
+                    for i in range(0, len(results), page_size)
+                ]
+                # Return the proper slice using chunk_index
+                results = results[page_index]
+
             return results
         return SyftError(message=result.err())
 
     @service_method(path="dataset.search", name="search")
     def search(
-        self, context: AuthedServiceContext, name: str
+        self,
+        context: AuthedServiceContext,
+        name: str,
+        page_size: Optional[int] = 0,
+        page_index: Optional[int] = 0,
     ) -> Union[List[Dataset], SyftError]:
         """Search a Dataset by name"""
         results = self.get_all(context)
 
-        return (
-            results
-            if isinstance(results, SyftError)
-            else [dataset for dataset in results if name in dataset.name]
-        )
+        if not isinstance(results, SyftError):
+            results = [dataset for dataset in results if name in dataset.name]
+
+            # If chunk size is defined, then split list into evenly sized chunks
+
+            if page_size:
+                results = [
+                    results[i : i + page_size]
+                    for i in range(0, len(results), page_size)
+                ]
+                # Return the proper slice using chunk_index
+                results = results[page_index]
+
+        return results
 
     @service_method(path="dataset.get_by_id", name="get_by_id")
     def get_by_id(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[SyftSuccess, SyftError]:
         """Get a Dataset"""
         result = self.stash.get_by_uid(context.credentials, uid=uid)
```

### Comparing `syft-0.8.1b3/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.1b4/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/message/message_service.py` & `syft-0.8.1b4/src/syft/service/message/message_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ..context import AuthedServiceContext
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
+from ..user.user_roles import DATA_SCIENTIST_ROLE_LEVEL
 from .message_stash import MessageStash
 from .messages import CreateMessage
 from .messages import LinkedObject
 from .messages import Message
 from .messages import MessageStatus
 
 
@@ -49,53 +50,84 @@
             context.credentials, verify_key=context.credentials
         )
         if result.err():
             return SyftError(message=str(result.err()))
         messages = result.ok()
         return messages
 
-    @service_method(path="messages.get_all_sent", name="outbox")
+    @service_method(
+        path="messages.get_all_sent", name="outbox", roles=DATA_SCIENTIST_ROLE_LEVEL
+    )
     def get_all_sent(
         self, context: AuthedServiceContext
     ) -> Union[List[Message], SyftError]:
         result = self.stash.get_all_sent_for_verify_key(
             context.credentials, context.credentials
         )
         if result.err():
             return SyftError(message=str(result.err()))
         messages = result.ok()
         return messages
 
-    @service_method(
-        path="messages.get_all_for_status",
-        name="get_all_for_status",
-    )
+    # get_all_read and unread cover the same functionality currently as
+    # get_all_for_status. However, there may be more statuses added in the future,
+    # so we are keeping the more generic get_all_for_status method.
     def get_all_for_status(
         self,
         context: AuthedServiceContext,
         status: MessageStatus,
     ) -> Union[List[Message], SyftError]:
         result = self.stash.get_all_by_verify_key_for_status(
             context.credentials, verify_key=context.credentials, status=status
         )
         if result.err():
             return SyftError(message=str(result.err()))
         messages = result.ok()
         return messages
 
-    @service_method(path="messages.mark_as_delivered", name="mark_as_delivered")
-    def mark_as_delivered(
+    @service_method(path="messages.get_all_read", name="get_all_read")
+    def get_all_read(
+        self,
+        context: AuthedServiceContext,
+    ) -> Union[List[Message], SyftError]:
+        return self.get_all_for_status(
+            context=context,
+            status=MessageStatus.READ,
+        )
+
+    @service_method(path="messages.get_all_unread", name="get_all_unread")
+    def get_all_unread(
+        self,
+        context: AuthedServiceContext,
+    ) -> Union[List[Message], SyftError]:
+        return self.get_all_for_status(
+            context=context,
+            status=MessageStatus.UNREAD,
+        )
+
+    @service_method(path="messages.mark_as_read", name="mark_as_read")
+    def mark_as_read(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[Message, SyftError]:
         result = self.stash.update_message_status(
-            context.credentials, uid=uid, status=MessageStatus.DELIVERED
+            context.credentials, uid=uid, status=MessageStatus.READ
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
+        return result.ok()
 
+    @service_method(path="messages.mark_as_unread", name="mark_as_unread")
+    def mark_as_unread(
+        self, context: AuthedServiceContext, uid: UID
+    ) -> Union[Message, SyftError]:
+        result = self.stash.update_message_status(
+            context.credentials, uid=uid, status=MessageStatus.UNREAD
+        )
+        if result.is_err():
+            return SyftError(message=str(result.err()))
         return result.ok()
 
     @service_method(path="messages.resolve_object", name="resolve_object")
     def resolve_object(
         self, context: AuthedServiceContext, linked_obj: LinkedObject
     ) -> Union[Message, SyftError]:
         service = context.node.get_service(linked_obj.service_type)
```

### Comparing `syft-0.8.1b3/src/syft/service/message/message_stash.py` & `syft-0.8.1b4/src/syft/service/message/message_stash.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 # relative
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
+from ...types.datetime import DateTime
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from .messages import Message
 from .messages import MessageStatus
 
 FromUserVerifyKeyPartitionKey = PartitionKey(
     key="from_user_verify_key", type_=SyftVerifyKey
 )
 ToUserVerifyKeyPartitionKey = PartitionKey(
     key="to_user_verify_key", type_=SyftVerifyKey
 )
 StatusPartitionKey = PartitionKey(key="status", type_=MessageStatus)
 
+OrderByCreatedAtTimeStampPartitionKey = PartitionKey(key="created_at", type_=DateTime)
+
 
 @instrument
 @serializable()
 class MessageStash(BaseUIDStoreStash):
     object_type = Message
     settings: PartitionSettings = PartitionSettings(
         name=Message.__canonical_name__,
@@ -59,29 +62,37 @@
         return self.get_all_for_verify_key(credentials, verify_key=verify_key, qks=qks)
 
     def get_all_for_verify_key(
         self, credentials: SyftVerifyKey, verify_key: SyftVerifyKey, qks: QueryKeys
     ) -> Result[List[Message], str]:
         if isinstance(verify_key, str):
             verify_key = SyftVerifyKey.from_string(verify_key)
-        return self.query_all(credentials, qks=qks)
+        return self.query_all(
+            credentials,
+            qks=qks,
+            order_by=OrderByCreatedAtTimeStampPartitionKey,
+        )
 
     def get_all_by_verify_key_for_status(
         self,
         credentials: SyftVerifyKey,
         verify_key: SyftVerifyKey,
         status: MessageStatus,
     ) -> Result[List[Message], str]:
         qks = QueryKeys(
             qks=[
                 ToUserVerifyKeyPartitionKey.with_obj(verify_key),
                 StatusPartitionKey.with_obj(status),
             ]
         )
-        return self.query_all(credentials, qks=qks)
+        return self.query_all(
+            credentials,
+            qks=qks,
+            order_by=OrderByCreatedAtTimeStampPartitionKey,
+        )
 
     def update_message_status(
         self, credentials: SyftVerifyKey, uid: UID, status: MessageStatus
     ) -> Result[Message, str]:
         result = self.get_by_uid(credentials, uid=uid)
         if result.is_err():
             return result.err()
@@ -91,15 +102,18 @@
             return Err(f"No message exists for id: {uid}")
         message.status = status
         return self.update(credentials, obj=message)
 
     def delete_all_for_verify_key(
         self, credentials: SyftVerifyKey, verify_key: SyftVerifyKey
     ) -> Result[bool, str]:
-        result = self.get_all_inbox_for_verify_key(credentials, verify_key=verify_key)
+        result = self.get_all_inbox_for_verify_key(
+            credentials,
+            verify_key=verify_key,
+        )
         # If result is an error then return the error
         if result.is_err():
             return result
 
         # get the list of messages
         messages = result.ok()
```

### Comparing `syft-0.8.1b3/src/syft/service/message/messages.py` & `syft-0.8.1b4/src/syft/service/message/messages.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # stdlib
 from enum import Enum
 from typing import Optional
 
 # relative
+from ...client.api import APIRegistry
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...store.linked_obj import LinkedObject
 from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
@@ -15,16 +16,16 @@
 from ...types.transforms import generate_id
 from ...types.transforms import transform
 from ...types.uid import UID
 
 
 @serializable()
 class MessageStatus(Enum):
-    UNDELIVERED = 0
-    DELIVERED = 1
+    UNREAD = 0
+    READ = 1
 
 
 class MessageExpiryStatus(Enum):
     AUTO = 0
     NEVER = 1
 
 
@@ -34,15 +35,15 @@
     __version__ = SYFT_OBJECT_VERSION_1
 
     subject: str
     node_uid: UID
     from_user_verify_key: SyftVerifyKey
     to_user_verify_key: SyftVerifyKey
     created_at: DateTime
-    status: MessageStatus = MessageStatus.UNDELIVERED
+    status: MessageStatus = MessageStatus.UNREAD
     linked_obj: Optional[LinkedObject]
 
     __attr_searchable__ = [
         "from_user_verify_key",
         "to_user_verify_key",
         "status",
     ]
@@ -50,14 +51,22 @@
 
     @property
     def link(self) -> Optional[SyftObject]:
         if self.linked_obj:
             return self.linked_obj.resolve
         return None
 
+    def mark_read(self) -> None:
+        api = APIRegistry.api_for(self.node_uid)
+        return api.services.messages.mark_as_read(uid=self.id)
+
+    def mark_unread(self) -> None:
+        api = APIRegistry.api_for(self.node_uid)
+        return api.services.messages.mark_as_unread(uid=self.id)
+
 
 @serializable()
 class CreateMessage(Message):
     __canonical_name__ = "CreateMessage"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: Optional[UID]
```

### Comparing `syft-0.8.1b3/src/syft/service/metadata/metadata_service.py` & `syft-0.8.1b4/src/syft/service/settings/settings_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,66 +9,67 @@
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ..context import AuthedServiceContext
 from ..context import UnauthedServiceContext
 from ..response import SyftError
 from ..service import AbstractService
 from ..service import service_method
-from .metadata_stash import MetadataStash
-from .node_metadata import NodeMetadata
-from .node_metadata import NodeMetadataUpdate
+from .settings import NodeSettings
+from .settings import NodeSettingsUpdate
+from .settings_stash import SettingsStash
 
 
 @serializable()
-class MetadataService(AbstractService):
+class SettingsService(AbstractService):
     store: DocumentStore
-    stash: MetadataStash
+    stash: SettingsStash
 
     def __init__(self, store: DocumentStore) -> None:
         self.store = store
-        self.stash = MetadataStash(store=store)
+        self.stash = SettingsStash(store=store)
 
-    @service_method(path="metadata.get", name="get")
+    @service_method(path="settings.get", name="get")
     def get(self, context: UnauthedServiceContext) -> Result[Ok, Err]:
-        """Get Metadata"""
+        """Get Settings"""
         result = self.stash.get_all(context.node.signing_key.verify_key)
         if result.is_ok():
-            metadata = result.ok()
-            # check if the metadata list is empty
-            if len(metadata) == 0:
-                return SyftError(message="No metadata found")
-            result = metadata[0]
+            settings = result.ok()
+            # check if the settings list is empty
+            if len(settings) == 0:
+                return SyftError(message="No settings found")
+            result = settings[0]
             return Ok(result)
         else:
             return SyftError(message=result.err())
 
-    @service_method(path="metadata.set", name="set")
+    @service_method(path="settings.set", name="set")
     def set(
-        self, context: AuthedServiceContext, metadata: NodeMetadata
+        self, context: AuthedServiceContext, settings: NodeSettings
     ) -> Result[Ok, Err]:
-        """Set a new the Node Metadata"""
-        result = self.stash.set(context.credentials, metadata)
+        """Set a new the Node Settings"""
+        print("Here!")
+        result = self.stash.set(context.credentials, settings)
         if result.is_ok():
             return result
         else:
             return SyftError(message=result.err())
 
-    @service_method(path="metadata.update", name="update")
+    @service_method(path="settings.update", name="update")
     def update(
-        self, context: AuthedServiceContext, metadata: NodeMetadataUpdate
+        self, context: AuthedServiceContext, settings: NodeSettingsUpdate
     ) -> Result[Ok, Err]:
         result = self.stash.get_all(context.credentials)
         if result.is_ok():
-            current_metadata = result.ok()
-            if len(current_metadata) > 0:
-                new_metadata = current_metadata[0].copy(
-                    update=metadata.dict(exclude_unset=True)
+            current_settings = result.ok()
+            if len(current_settings) > 0:
+                new_settings = current_settings[0].copy(
+                    update=settings.dict(exclude_unset=True)
                 )
-                update_result = self.stash.update(context.credentials, new_metadata)
+                update_result = self.stash.update(context.credentials, new_settings)
                 if update_result.is_ok():
                     return result
                 else:
                     return SyftError(message=update_result.err())
             else:
-                return SyftError(message="No metadata found")
+                return SyftError(message="No settings found")
         else:
             return SyftError(message=result.err())
```

### Comparing `syft-0.8.1b3/src/syft/service/metadata/metadata_stash.py` & `syft-0.8.1b4/src/syft/service/settings/settings_stash.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,41 +9,41 @@
 from ...serde.serializable import serializable
 from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...types.uid import UID
 from ...util.telemetry import instrument
-from .node_metadata import NodeMetadata
+from .settings import NodeSettings
 
 NamePartitionKey = PartitionKey(key="name", type_=str)
 ActionIDsPartitionKey = PartitionKey(key="action_ids", type_=List[UID])
 
 
 @instrument
 @serializable()
-class MetadataStash(BaseUIDStoreStash):
-    object_type = NodeMetadata
+class SettingsStash(BaseUIDStoreStash):
+    object_type = NodeSettings
     settings: PartitionSettings = PartitionSettings(
-        name=NodeMetadata.__canonical_name__, object_type=NodeMetadata
+        name=NodeSettings.__canonical_name__, object_type=NodeSettings
     )
 
     def __init__(self, store: DocumentStore) -> None:
         super().__init__(store=store)
 
     def set(
-        self, credentials: SyftVerifyKey, metadata: NodeMetadata
-    ) -> Result[NodeMetadata, str]:
-        res = self.check_type(metadata, self.object_type)
+        self, credentials: SyftVerifyKey, settings: NodeSettings
+    ) -> Result[NodeSettings, str]:
+        res = self.check_type(settings, self.object_type)
         # we dont use and_then logic here as it is hard because of the order of the arguments
         if res.is_err():
             return res
         return super().set(credentials=credentials, obj=res.ok())
 
     def update(
-        self, credentials: SyftVerifyKey, metadata: NodeMetadata
-    ) -> Result[NodeMetadata, str]:
-        res = self.check_type(metadata, self.object_type)
+        self, credentials: SyftVerifyKey, settings: NodeSettings
+    ) -> Result[NodeSettings, str]:
+        res = self.check_type(settings, self.object_type)
         # we dont use and_then logic here as it is hard because of the order of the arguments
         if res.is_err():
             return res
         return super().update(credentials=credentials, obj=res.ok())
```

### Comparing `syft-0.8.1b3/src/syft/service/metadata/node_metadata.py` & `syft-0.8.1b4/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/network/network_service.py` & `syft-0.8.1b4/src/syft/service/network/network_service.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,37 @@
 # stdlib
+import secrets
 from typing import Any
 from typing import Callable
 from typing import List
 from typing import Optional
 from typing import Union
 
 # third party
 from result import Result
-from typing_extensions import Self
 
 # relative
-from ...abstract_node import AbstractNode
 from ...client.client import HTTPConnection
-from ...client.client import NodeConnection
 from ...client.client import PythonConnection
 from ...client.client import SyftClient
-from ...node.credentials import SyftSigningKey
 from ...node.credentials import SyftVerifyKey
 from ...node.worker_settings import WorkerSettings
 from ...serde.serializable import serializable
 from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
 from ...types.grid_url import GridURL
-from ...types.syft_object import SYFT_OBJECT_VERSION_1
-from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import keep
 from ...types.transforms import transform
 from ...types.transforms import transform_method
-from ...types.uid import UID
 from ...util.telemetry import instrument
-from ...util.util import recursive_hash
 from ..context import AuthedServiceContext
-from ..context import NodeServiceContext
 from ..data_subject.data_subject import NamePartitionKey
 from ..metadata.node_metadata import NodeMetadata
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
@@ -47,219 +39,22 @@
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from ..vpn.headscale_client import HeadscaleAuthToken
 from ..vpn.headscale_client import HeadscaleClient
 from ..vpn.tailscale_client import TailscaleClient
 from ..vpn.tailscale_client import TailscaleState
 from ..vpn.tailscale_client import TailscaleStatus
 from ..vpn.tailscale_client import get_vpn_client
+from .node_peer import NodePeer
+from .routes import HTTPNodeRoute
+from .routes import NodeRoute
+from .routes import PythonNodeRoute
 
 VerifyKeyPartitionKey = PartitionKey(key="verify_key", type_=SyftVerifyKey)
 
 
-class NodeRoute:
-    def client_with_context(self, context: NodeServiceContext) -> SyftClient:
-        connection = route_to_connection(route=self, context=context)
-        return SyftClient(connection=connection, credentials=context.node.signing_key)
-
-
-@serializable()
-class HTTPNodeRoute(SyftObject, NodeRoute):
-    __canonical_name__ = "HTTPNodeRoute"
-    __version__ = SYFT_OBJECT_VERSION_1
-
-    host_or_ip: str
-    private: bool = False
-    protocol: str = "http"
-    port: int = 80
-
-    def __hash__(self) -> int:
-        return (
-            hash(self.host_or_ip)
-            + hash(self.private)
-            + hash(self.protocol)
-            + hash(self.port)
-        )
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, HTTPNodeRoute):
-            return hash(self) == hash(other)
-        return self == other
-
-
-@serializable()
-class PythonNodeRoute(SyftObject, NodeRoute):
-    __canonical_name__ = "PythonNodeRoute"
-    __version__ = SYFT_OBJECT_VERSION_1
-
-    worker_settings: WorkerSettings
-
-    @property
-    def node(self) -> Optional[AbstractNode]:
-        # relative
-        from ...node.worker import Worker
-
-        node = Worker(
-            id=self.worker_settings.id,
-            name=self.worker_settings.name,
-            signing_key=self.worker_settings.signing_key,
-            document_store_config=self.worker_settings.document_store_config,
-            action_store_config=self.worker_settings.action_store_config,
-            processes=1,
-        )
-        return node
-
-    @staticmethod
-    def with_node(self, node: AbstractNode) -> Self:
-        worker_settings = WorkerSettings.from_node(node)
-        return PythonNodeRoute(id=worker_settings.id, worker_settings=worker_settings)
-
-    def __hash__(self) -> int:
-        return (
-            hash(self.worker_settings.id)
-            + hash(self.worker_settings.name)
-            + hash(self.worker_settings.signing_key)
-        )
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, PythonNodeRoute):
-            return hash(self) == hash(other)
-        return self == other
-
-
-def route_to_connection(
-    route: NodeRoute, context: Optional[TransformContext] = None
-) -> NodeConnection:
-    if isinstance(route, HTTPNodeRoute):
-        return route.to(HTTPConnection, context=context)
-    else:
-        return route.to(PythonConnection, context=context)
-
-
-def connection_to_route(connection: NodeConnection) -> NodeRoute:
-    if isinstance(connection, HTTPConnection):
-        return connection.to(HTTPNodeRoute)
-    else:
-        return connection.to(PythonNodeRoute)
-
-
-@serializable()
-class NodePeer(SyftObject):
-    # version
-    __canonical_name__ = "NodePeer"
-    __version__ = SYFT_OBJECT_VERSION_1
-
-    id: Optional[UID]
-    name: str
-    verify_key: SyftVerifyKey
-    is_vpn: bool = False
-    vpn_auth_key: Optional[str] = None
-    node_routes: List[NodeRoute] = []
-
-    __attr_searchable__ = ["name"]
-    __attr_unique__ = ["verify_key"]
-    __attr_repr_cols__ = ["name"]
-
-    def __hash__(self) -> int:
-        hashes = 0
-        hashes += recursive_hash(self.id)
-        hashes += recursive_hash(self.name)
-        hashes += recursive_hash(self.verify_key)
-        hashes += recursive_hash(self.node_routes)
-        return hashes
-
-    def update_routes(self, new_routes: List[NodeRoute]) -> None:
-        add_routes = []
-        existing_routes = set(self.node_routes)
-        for new_route in new_routes:
-            if new_route not in existing_routes:
-                add_routes.append(new_route)
-        self.node_routes += add_routes
-
-    @staticmethod
-    def from_client(client: SyftClient) -> Self:
-        if not client.metadata:
-            raise Exception("Client has have metadata first")
-
-        peer = client.metadata.to(NodeMetadata).to(NodePeer)
-        route = connection_to_route(client.connection)
-        peer.node_routes.append(route)
-        return peer
-
-    def client_with_context(self, context: NodeServiceContext) -> SyftClient:
-        if len(self.node_routes) < 1:
-            raise Exception(f"No routes to peer: {self}")
-        route = self.node_routes[0]
-        connection = route_to_connection(route=route)
-        return SyftClient(connection=connection, credentials=context.node.signing_key)
-
-    def client_with_key(self, credentials: SyftSigningKey) -> SyftClient:
-        if len(self.node_routes) < 1:
-            raise Exception(f"No routes to peer: {self}")
-        route = self.node_routes[0]
-        connection = route_to_connection(route=route)
-        return SyftClient(connection=connection, credentials=credentials)
-
-    @property
-    def guest_client(self) -> SyftClient:
-        guest_key = SyftSigningKey.generate()
-        return self.client_with_key(credentials=guest_key)
-
-    def proxy_from(self, client: SyftClient) -> SyftClient:
-        return client.proxy_to(self)
-
-
-def from_grid_url(context: TransformContext) -> TransformContext:
-    url = context.obj.url.as_container_host()
-    context.output["host_or_ip"] = url.host_or_ip
-    context.output["protocol"] = url.protocol
-    context.output["port"] = url.port
-    context.output["private"] = False
-    return context
-
-
-@transform(HTTPConnection, HTTPNodeRoute)
-def http_connection_to_node_route() -> List[Callable]:
-    return [from_grid_url]
-
-
-def get_python_node_route(context: TransformContext) -> TransformContext:
-    context.output["id"] = context.obj.node.id
-    context.output["worker_settings"] = WorkerSettings.from_node(context.obj.node)
-    return context
-
-
-@transform(PythonConnection, PythonNodeRoute)
-def python_connection_to_node_route() -> List[Callable]:
-    return [get_python_node_route]
-
-
-@transform_method(PythonNodeRoute, PythonConnection)
-def node_route_to_python_connection(
-    obj: Any, context: Optional[TransformContext] = None
-) -> List[Callable]:
-    return PythonConnection(node=obj.node)
-
-
-@transform_method(HTTPNodeRoute, HTTPConnection)
-def node_route_to_http_connection(
-    obj: Any, context: Optional[TransformContext] = None
-) -> List[Callable]:
-    url = GridURL(
-        protocol=obj.protocol, host_or_ip=obj.host_or_ip, port=obj.port
-    ).as_container_host()
-    return HTTPConnection(url=url)
-
-
-@transform(NodeMetadata, NodePeer)
-def metadata_to_peer() -> List[Callable]:
-    return [
-        keep(["id", "name", "verify_key"]),
-    ]
-
-
 @instrument
 @serializable()
 class NetworkStash(BaseUIDStoreStash):
     object_type = NodePeer
     settings: PartitionSettings = PartitionSettings(
         name=NodePeer.__canonical_name__, object_type=NodePeer
     )
@@ -310,98 +105,138 @@
     store: DocumentStore
     stash: NetworkStash
 
     def __init__(self, store: DocumentStore) -> None:
         self.store = store
         self.stash = NetworkStash(store=store)
 
+    # TODO: Check with MADHAVA, can we even allow guest user to introduce routes to
+    # domain nodes?
     @service_method(
-        path="network.exchange_credentials_with", name="exchange_credentials_with"
+        path="network.exchange_credentials_with",
+        name="exchange_credentials_with",
+        roles=GUEST_ROLE_LEVEL,
     )
     def exchange_credentials_with(
         self,
         context: AuthedServiceContext,
-        peer: Optional[NodePeer] = None,
-        client: Optional[SyftClient] = None,
+        self_node_route: NodeRoute,
+        remote_node_route: NodeRoute,
+        remote_node_verify_key: SyftVerifyKey,
     ) -> Union[SyftSuccess, SyftError]:
-        """Exchange Credentials With Another Node"""
-        # check root user is asking for the exchange
-        if isinstance(client, SyftClient):
-            remote_peer = NodePeer.from_client(client)
-        else:
-            remote_peer = peer
-        if remote_peer is None:
-            return SyftError("exchange_credentials_with requires peer or client")
+        """Exchange Route With Another Node"""
 
-        # tell the remote peer our details
-        if not context.node:
-            return SyftError(f"{type(context)} has no node")
-        self_metadata = context.node.metadata
-        self_node_peer = self_metadata.to(NodePeer)
+        # Step 1: Validate the Route
+        self_node_peer = self_node_route.validate_with_context(context=context)
 
-        # switch to the nodes signing key
-        client = remote_peer.client_with_context(context=context)
-        remote_peer_metadata = client.api.services.network.add_peer(self_node_peer)
+        if isinstance(self_node_peer, SyftError):
+            return self_node_peer
 
-        if remote_peer_metadata.verify_key != remote_peer.verify_key:
-            return SyftError(
-                (
-                    f"Response from remote peer {remote_peer_metadata} "
-                    f"does not match initial peer {remote_peer}"
-                )
-            )
+        # Step 2: Send the Node Peer to the remote node
+        # Also give them their own to validate that it belongs to them
+        # random challenge prevents replay attacks
+        remote_client = remote_node_route.client_with_context(context=context)
+        random_challenge = secrets.token_bytes(16)
+
+        remote_res = remote_client.api.services.network.add_peer(
+            peer=self_node_peer,
+            challenge=random_challenge,
+            self_node_route=remote_node_route,
+            verify_key=remote_node_verify_key,
+        )
+
+        if isinstance(remote_res, SyftError):
+            return remote_res
+
+        challenge_signature, remote_node_peer = remote_res
+
+        # Verifying if the challenge is valid
+        remote_node_verify_key.verify_key.verify(random_challenge, challenge_signature)
 
         # save the remote peer for later
-        result = self.stash.update_peer(context.node.verify_key, remote_peer)
+        result = self.stash.update_peer(context.node.verify_key, remote_node_peer)
         if result.is_err():
             return SyftError(message=str(result.err()))
 
-        if result.is_err():
-            return SyftError(message=str(result.err()))
-        return SyftSuccess(message="Credentials Exchanged")
+        return SyftSuccess(message="Routes Exchanged")
 
     @service_method(path="network.add_peer", name="add_peer", roles=GUEST_ROLE_LEVEL)
     def add_peer(
-        self, context: AuthedServiceContext, peer: NodePeer
-    ) -> Union[NodeMetadata, SyftError]:
+        self,
+        context: AuthedServiceContext,
+        peer: NodePeer,
+        challenge: bytes,
+        self_node_route: NodeRoute,
+        verify_key: SyftVerifyKey,
+    ) -> Union[bytes, SyftError]:
         """Add a Network Node Peer"""
-        # save the peer and verify the key matches the message signer
+
+        # Using the verify_key of the peer to verify the signature
+        # It is also our single source of truth for the peer
         if peer.verify_key != context.credentials:
             return SyftError(
                 message=(
                     f"The {type(peer)}.verify_key: "
                     f"{peer.verify_key} does not match the signature of the message"
                 )
             )
 
-        result = self.stash.update_peer(context.credentials, peer)
+        if verify_key != context.node.verify_key:
+            return SyftError(
+                message="verify_key does not match the remote node's verify_key for add_peer"
+            )
+
+        result = self.stash.update_peer(context.node.verify_key, peer)
         if result.is_err():
             return SyftError(message=str(result.err()))
+
+        # this way they can match up who we are with who they think we are
+        # Sending a signed messages for the peer to verify
+        self_node_peer = self_node_route.validate_with_context(context=context)
+
+        if isinstance(self_node_peer, SyftError):
+            return self_node_peer
+
+        # Q,TODO: Should the returned node peer also be signed
+        # as the challenge is already signed
+
+        challenge_signature = context.node.signing_key.signing_key.sign(
+            challenge
+        ).signature
+
+        return [challenge_signature, self_node_peer]
+
+    @service_method(path="network.ping", name="ping")
+    def ping(
+        self, context: AuthedServiceContext, challenge: bytes
+    ) -> Union[bytes, SyftError]:
+        """To check alivesness/authenticity of a peer"""
+
+        # Only the root user can ping the node to check its state
+        if context.node.verify_key != context.credentials:
+            return SyftError(message=("Only the root user can access ping endpoint"))
+
         # this way they can match up who we are with who they think we are
-        metadata = context.node.metadata
-        return metadata
+        # Sending a signed messages for the peer to verify
+        challenge_signature = context.node.signing_key.signing_key.sign(
+            challenge
+        ).signature
+
+        return challenge_signature
 
     @service_method(path="network.add_route_for", name="add_route_for")
     def add_route_for(
         self,
         context: AuthedServiceContext,
         route: NodeRoute,
-        peer: Optional[NodePeer] = None,
-        client: Optional[SyftClient] = None,
+        peer: NodePeer,
     ) -> Union[SyftSuccess, SyftError]:
         """Add Route for this Node to another Node"""
         # check root user is asking for the exchange
-        if isinstance(client, SyftClient):
-            remote_peer = NodePeer.from_client(client)
-        else:
-            remote_peer = peer
-        if remote_peer is None:
-            return SyftError("exchange_credentials_with requires peer or client")
-
-        client = remote_peer.client_with_context(context=context)
+        client = peer.client_with_context(context=context)
         result = client.api.services.network.verify_route(route)
 
         if not isinstance(result, SyftSuccess):
             return result
         return SyftSuccess(message="Route Verified")
 
     @service_method(
@@ -415,20 +250,18 @@
         peer = self.stash.get_for_verify_key(
             context.node.verify_key, context.credentials
         )
         if peer.is_err():
             return SyftError(message=peer.err())
         peer = peer.ok()
 
-        client = route.client_with_context(context=context)
-        metadata = client.metadata.to(NodeMetadata)
-        if peer.verify_key != metadata.verify_key:
+        if peer.verify_key != context.credentials:
             return SyftError(
                 message=(
-                    f"verify_key: {metadata.verify_key} at route {route} "
+                    f"verify_key: {context.credentials} at route {route} "
                     f"does not match listed peer: {peer}"
                 )
             )
         peer.update_routes([route])
         result = self.stash.update_peer(context.node.verify_key, peer)
         if result.is_err():
             return SyftError(message=str(result.err()))
@@ -600,7 +433,56 @@
             return result
 
         return SyftSuccess(message="Successfully joined VPN !!!")
 
 
 TYPE_TO_SERVICE[NodePeer] = NetworkService
 SERVICE_TO_TYPES[NetworkService].update({NodePeer})
+
+
+def from_grid_url(context: TransformContext) -> TransformContext:
+    url = context.obj.url.as_container_host()
+    context.output["host_or_ip"] = url.host_or_ip
+    context.output["protocol"] = url.protocol
+    context.output["port"] = url.port
+    context.output["private"] = False
+    return context
+
+
+@transform(HTTPConnection, HTTPNodeRoute)
+def http_connection_to_node_route() -> List[Callable]:
+    return [from_grid_url]
+
+
+def get_python_node_route(context: TransformContext) -> TransformContext:
+    context.output["id"] = context.obj.node.id
+    context.output["worker_settings"] = WorkerSettings.from_node(context.obj.node)
+    return context
+
+
+@transform(PythonConnection, PythonNodeRoute)
+def python_connection_to_node_route() -> List[Callable]:
+    return [get_python_node_route]
+
+
+@transform_method(PythonNodeRoute, PythonConnection)
+def node_route_to_python_connection(
+    obj: Any, context: Optional[TransformContext] = None
+) -> List[Callable]:
+    return PythonConnection(node=obj.node)
+
+
+@transform_method(HTTPNodeRoute, HTTPConnection)
+def node_route_to_http_connection(
+    obj: Any, context: Optional[TransformContext] = None
+) -> List[Callable]:
+    url = GridURL(
+        protocol=obj.protocol, host_or_ip=obj.host_or_ip, port=obj.port
+    ).as_container_host()
+    return HTTPConnection(url=url)
+
+
+@transform(NodeMetadata, NodePeer)
+def metadata_to_peer() -> List[Callable]:
+    return [
+        keep(["id", "name", "verify_key"]),
+    ]
```

### Comparing `syft-0.8.1b3/src/syft/service/policy/policy.py` & `syft-0.8.1b4/src/syft/service/policy/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from RestrictedPython import compile_restricted
 from result import Ok
 
 # relative
 from ...abstract_node import NodeType
 from ...client.api import NodeView
 from ...node.credentials import SyftVerifyKey
+from ...serde.recursive_primitives import recursive_serde_register_type
 from ...serde.serializable import serializable
 from ...store.document_store import PartitionKey
 from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import generate_id
@@ -94,15 +95,15 @@
         if "init_kwargs" in kwargs:
             init_kwargs = kwargs["init_kwargs"]
             del kwargs["init_kwargs"]
         else:
             init_kwargs = deepcopy(kwargs)
             if "id" in init_kwargs:
                 del init_kwargs["id"]
-        super().__init__(init_kwargs=init_kwargs, *args, **kwargs)
+        super().__init__(init_kwargs=init_kwargs, *args, **kwargs)  # noqa: B026
 
     @classmethod
     @property
     def policy_code(cls) -> str:
         mro = reversed(cls.mro())
         op_code = ""
         for klass in mro:
@@ -204,16 +205,14 @@
                 context=context, uid=arg_id, twin_mode=TwinMode.NONE
             )
             if kwarg_value.is_err():
                 return kwarg_value
             code_inputs[var_name] = kwarg_value.ok()
 
     elif context.node.node_type == NodeType.ENCLAVE:
-        # TODO 🟣 Temporarily added skip permission arguments for enclave
-        # until permissions are fully integrated
         dict_object = action_service.get(context=context, uid=code_item_id)
         if dict_object.is_err():
             return dict_object
         for value in dict_object.ok().base_dict.values():
             code_inputs.update(value)
 
     else:
@@ -358,22 +357,27 @@
 
     limit: int = 1
 
 
 SingleExecutionExactOutput = OutputPolicyExecuteOnce
 
 
+@serializable()
 class CustomPolicy(type):
     # capture the init_kwargs transparently
     def __call__(cls, *args: Any, **kwargs: Any) -> None:
         obj = super().__call__(*args, **kwargs)
-        setattr(obj, "init_kwargs", kwargs)
+        obj.init_kwargs = kwargs
         return obj
 
 
+recursive_serde_register_type(CustomPolicy)
+
+
+@serializable()
 class CustomOutputPolicy(metaclass=CustomPolicy):
     def apply_output(
         self,
         context: NodeServiceContext,
         outputs: Any,
     ) -> Optional[Any]:
         return outputs
@@ -656,18 +660,18 @@
     klass.__module__ = "syft.user"
     klass.__name__ = unique_name
     # syft absolute
     import syft as sy
 
     if not hasattr(sy, "user"):
         user_module = types.ModuleType("user")
-        setattr(sys.modules["syft"], "user", user_module)
+        sys.modules["syft"].user = user_module
     user_module = sy.user
     setattr(user_module, unique_name, klass)
-    setattr(sys.modules["syft"], "user", user_module)
+    sys.modules["syft"].user = user_module
     return klass
 
 
 def execute_policy_code(user_policy: UserPolicy):
     stdout_ = sys.stdout
     stderr_ = sys.stderr
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `syft-0.8.1b3/src/syft/service/policy/policy_service.py` & `syft-0.8.1b4/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.1b4/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/queue/base_queue.py` & `syft-0.8.1b4/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/queue/queue.py` & `syft-0.8.1b4/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/queue/queue_stash.py` & `syft-0.8.1b4/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/queue/zmq_queue.py` & `syft-0.8.1b4/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/request/request.py` & `syft-0.8.1b4/src/syft/service/request/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,14 +211,16 @@
         )
 
         submit_request = SubmitRequest(
             changes=[policy_state_mutation, permission_change],
             requesting_user_verify_key=self.requesting_user_verify_key,
         )
 
+        self.status = RequestStatus.APPROVED
+
         new_request = api.services.request.submit(submit_request)
         if not new_request:
             return new_request
         new_request_result = api.services.request.apply(new_request.id)
         if not new_request_result:
             return new_request_result
         result = api.services.request.apply(self.id)
```

### Comparing `syft-0.8.1b3/src/syft/service/request/request_service.py` & `syft-0.8.1b4/src/syft/service/request/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/request/request_stash.py` & `syft-0.8.1b4/src/syft/service/request/request_stash.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 # relative
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
+from ...types.datetime import DateTime
 from ...util.telemetry import instrument
 from .request import Request
 from .request import RequestStatus
 
 RequestingUserVerifyKeyPartitionKey = PartitionKey(
     key="requesting_user_verify_key", type_=SyftVerifyKey
 )
 StatusPartitionKey = PartitionKey(key="status", type_=RequestStatus)
 
+OrderByRequestTimeStampPartitionKey = PartitionKey(key="request_time", type_=DateTime)
+
 
 @instrument
 @serializable()
 class RequestStash(BaseUIDStoreStash):
     object_type = Request
     settings: PartitionSettings = PartitionSettings(
         name=Request.__canonical_name__, object_type=Request
@@ -33,14 +36,22 @@
         self,
         credentials: SyftVerifyKey,
         verify_key: SyftVerifyKey,
     ) -> Result[List[Request], str]:
         if isinstance(verify_key, str):
             verify_key = SyftVerifyKey.from_string(verify_key)
         qks = QueryKeys(qks=[RequestingUserVerifyKeyPartitionKey.with_obj(verify_key)])
-        return self.query_all(credentials=credentials, qks=qks)
+        return self.query_all(
+            credentials=credentials,
+            qks=qks,
+            order_by=OrderByRequestTimeStampPartitionKey,
+        )
 
     def get_all_for_status(
         self, credentials: SyftVerifyKey, status: RequestStatus
     ) -> Result[List[Request], str]:
         qks = QueryKeys(qks=[StatusPartitionKey.with_obj(status)])
-        return self.query_all(credentials=credentials, qks=qks)
+        return self.query_all(
+            credentials=credentials,
+            qks=qks,
+            order_by=OrderByRequestTimeStampPartitionKey,
+        )
```

### Comparing `syft-0.8.1b3/src/syft/service/response.py` & `syft-0.8.1b4/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/service.py` & `syft-0.8.1b4/src/syft/service/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,19 +255,21 @@
         keys = autosplat_type.__fields__.keys()
         for key in keys:
             if key in kwargs:
                 init_kwargs[key] = kwargs.pop(key)
         autosplat_objs[autosplat_key] = autosplat_type(**init_kwargs)
 
     final_kwargs = {}
-    for param_key, _ in signature.parameters.items():
+    for param_key, param in signature.parameters.items():
         if param_key in kwargs:
             final_kwargs[param_key] = kwargs[param_key]
         elif param_key in autosplat_objs:
             final_kwargs[param_key] = autosplat_objs[param_key]
+        elif not isinstance(param.default, type(Parameter.empty)):
+            final_kwargs[param_key] = param.default
         else:
             raise Exception(f"Missing {param_key} not in kwargs.")
     return (args, final_kwargs)
 
 
 def expand_signature(signature: Signature, autosplat: List[str]) -> Signature:
     new_mapping = {}
```

### Comparing `syft-0.8.1b3/src/syft/service/user/user.py` & `syft-0.8.1b4/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/user/user_roles.py` & `syft-0.8.1b4/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/user/user_service.py` & `syft-0.8.1b4/src/syft/service/user/user_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,19 +89,33 @@
                 return SyftError(message=f"No user exists for given: {uid}")
             return user.to(UserView)
 
         return SyftError(message=str(result.err()))
 
     @service_method(path="user.get_all", name="get_all", roles=DATA_OWNER_ROLE_LEVEL)
     def get_all(
-        self, context: AuthedServiceContext
+        self,
+        context: AuthedServiceContext,
+        page_size: Optional[int] = 0,
+        page_index: Optional[int] = 0,
     ) -> Union[Optional[UserView], SyftError]:
         result = self.stash.get_all(context.credentials)
         if result.is_ok():
-            return [user.to(UserView) for user in result.ok()]
+            results = [user.to(UserView) for user in result.ok()]
+
+            # If chunk size is defined, then split list into evenly sized chunks
+            if page_size:
+                results = [
+                    results[i : i + page_size]
+                    for i in range(0, len(results), page_size)
+                ]
+                # Return the proper slice using chunk_index
+                results = results[page_index]
+
+            return results
 
         # 🟡 TODO: No user exists will happen when result.ok() is empty list
         return SyftError(message="No users exists")
 
     def get_role_for_credentials(
         self, credentials: SyftVerifyKey
     ) -> Union[Optional[ServiceRole], SyftError]:
@@ -117,28 +131,41 @@
         return ServiceRole.GUEST
 
     @service_method(path="user.search", name="search", autosplat=["user_search"])
     def search(
         self,
         context: AuthedServiceContext,
         user_search: UserSearch,
+        page_size: Optional[int] = 0,
+        page_index: Optional[int] = 0,
     ) -> Union[List[UserView], SyftError]:
         kwargs = user_search.to_dict(exclude_empty=True)
 
         if len(kwargs) == 0:
             valid_search_params = list(UserSearch.__fields__.keys())
             return SyftError(
                 message=f"Invalid Search parameters. \
                 Allowed params: {valid_search_params}"
             )
         result = self.stash.find_all(credentials=context.credentials, **kwargs)
+
         if result.is_err():
             return SyftError(message=str(result.err()))
         users = result.ok()
-        return [user.to(UserView) for user in users] if users is not None else []
+        results = [user.to(UserView) for user in users] if users is not None else []
+
+        # If page size is defined, then split list into evenly sized chunks
+        if page_size:
+            results = [
+                results[i : i + page_size] for i in range(0, len(results), page_size)
+            ]
+            # Return the proper slice using page_index
+            results = results[page_index]
+
+        return results
 
     @service_method(path="user.update", name="update", roles=GUEST_ROLE_LEVEL)
     def update(
         self, context: AuthedServiceContext, uid: UID, user_update: UserUpdate
     ) -> Union[UserView, SyftError]:
         updates_role = user_update.role is not Empty
```

### Comparing `syft-0.8.1b3/src/syft/service/user/user_stash.py` & `syft-0.8.1b4/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/vpn/headscale_client.py` & `syft-0.8.1b4/src/syft/service/vpn/headscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/vpn/tailscale_client.py` & `syft-0.8.1b4/src/syft/service/vpn/tailscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/service/vpn/vpn.py` & `syft-0.8.1b4/src/syft/service/vpn/vpn.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,17 +83,17 @@
     __canonical_name__ = "VPNClientConnection"
     __version__ = SYFT_OBJECT_VERSION_1
 
     url: GridURL
     session_cache: Optional[Session]
     routes: Type[VPNRoutes]
 
-    def __init__(self, url: Union[GridURL, str], *args, **kwargs) -> None:
-        url = GridURL.from_url(url)
-        super().__init__(url=url, *args, **kwargs)
+    @validator("url", pre=True)
+    def __make_grid_url(cls, url: Union[GridURL, str]) -> GridURL:
+        return GridURL.from_url(url)
 
     @property
     def session(self) -> Session:
         if self.session_cache is None:
             session = requests.Session()
             retry = Retry(total=3, backoff_factor=0.5)
             adapter = HTTPAdapter(max_retries=retry)
@@ -152,17 +152,19 @@
 
         return response.content
 
     def send_command(
         self,
         path: str,
         api_key: str,
-        command_args: dict = {},
+        command_args: Optional[dict] = None,
         timeout: int = DEFAULT_TIMEOUT,
     ) -> Result[CommandReport, str]:
+        if command_args is None:
+            command_args = {}
         command_args.update({"timeout": timeout, "force_unique_key": True})
         headers = {"X-STACK-API-KEY": api_key}
         result = self._make_post(
             path=path,
             json=command_args,
             headers=headers,
         )
```

### Comparing `syft-0.8.1b3/src/syft/store/dict_document_store.py` & `syft-0.8.1b4/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/store/document_store.py` & `syft-0.8.1b4/src/syft/store/document_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -387,21 +387,26 @@
         return self._thread_safe_cbk(
             self._get,
             uid=uid,
             credentials=credentials,
         )
 
     def find_index_or_search_keys(
-        self, credentials: SyftVerifyKey, index_qks: QueryKeys, search_qks: QueryKeys
+        self,
+        credentials: SyftVerifyKey,
+        index_qks: QueryKeys,
+        search_qks: QueryKeys,
+        order_by: Optional[PartitionKey] = None,
     ) -> Result[List[SyftObject], str]:
         return self._thread_safe_cbk(
             self._find_index_or_search_keys,
             credentials,
             index_qks=index_qks,
             search_qks=search_qks,
+            order_by=order_by,
         )
 
     def remove_keys(
         self,
         unique_query_keys: QueryKeys,
         searchable_query_keys: QueryKeys,
     ) -> None:
@@ -423,29 +428,34 @@
             credentials=credentials,
             qk=qk,
             obj=obj,
             has_permission=has_permission,
         )
 
     def get_all_from_store(
-        self, credentials: SyftVerifyKey, qks: QueryKeys
+        self,
+        credentials: SyftVerifyKey,
+        qks: QueryKeys,
+        order_by: Optional[PartitionKey] = None,
     ) -> Result[List[SyftObject], str]:
-        return self._thread_safe_cbk(self._get_all_from_store, credentials, qks)
+        return self._thread_safe_cbk(
+            self._get_all_from_store, credentials, qks, order_by
+        )
 
     def delete(
         self, credentials: SyftVerifyKey, qk: QueryKey, has_permission=False
     ) -> Result[SyftSuccess, Err]:
         return self._thread_safe_cbk(
             self._delete, credentials, qk, has_permission=has_permission
         )
 
     def all(
-        self, credentials: SyftVerifyKey
+        self, credentials: SyftVerifyKey, order_by: Optional[PartitionKey] = None
     ) -> Result[List[BaseStash.object_type], str]:
-        return self._thread_safe_cbk(self._all, credentials)
+        return self._thread_safe_cbk(self._all, credentials, order_by)
 
     # Potentially thread-unsafe methods.
     # CAUTION:
     #       * Don't use self.lock here.
     #       * Do not call the public thread-safe methods here(with locking).
     # These methods are called from the public thread-safe API, and will hang the process.
     def _set(
@@ -455,15 +465,18 @@
     ) -> Result[SyftObject, str]:
         raise NotImplementedError
 
     def _update(self, qk: QueryKey, obj: SyftObject) -> Result[SyftObject, str]:
         raise NotImplementedError
 
     def _get_all_from_store(
-        self, credentials: SyftVerifyKey, qks: QueryKeys
+        self,
+        credentials: SyftVerifyKey,
+        qks: QueryKeys,
+        order_by: Optional[PartitionKey] = None,
     ) -> Result[List[SyftObject], str]:
         raise NotImplementedError
 
     def _delete(self, qk: QueryKey) -> Result[SyftSuccess, Err]:
         raise NotImplementedError
 
     def _all(self) -> Result[List[BaseStash.object_type], str]:
@@ -516,17 +529,17 @@
         return (
             Ok(obj)
             if isinstance(obj, type_)
             else Err(f"{type(obj)} does not match required type: {type_}")
         )
 
     def get_all(
-        self, credentials: SyftVerifyKey
+        self, credentials: SyftVerifyKey, order_by: Optional[PartitionKey] = None
     ) -> Result[List[BaseStash.object_type], str]:
-        return self.partition.all(credentials)
+        return self.partition.all(credentials, order_by)
 
     def __len__(self) -> int:
         return len(self.partition)
 
     def set(
         self,
         credentials: SyftVerifyKey,
@@ -538,15 +551,18 @@
             credentials=credentials,
             obj=obj,
             ignore_duplicates=ignore_duplicates,
             add_permissions=add_permissions,
         )
 
     def query_all(
-        self, credentials: SyftVerifyKey, qks: Union[QueryKey, QueryKeys]
+        self,
+        credentials: SyftVerifyKey,
+        qks: Union[QueryKey, QueryKeys],
+        order_by: Optional[PartitionKey] = None,
     ) -> Result[List[BaseStash.object_type], str]:
         if isinstance(qks, QueryKey):
             qks = QueryKeys(qks=qks)
 
         unique_keys = []
         searchable_keys = []
 
@@ -561,27 +577,38 @@
                     f"{qk} not in {type(self.partition)} unique or searchable keys"
                 )
 
         index_qks = QueryKeys(qks=unique_keys)
         search_qks = QueryKeys(qks=searchable_keys)
 
         return self.partition.find_index_or_search_keys(
-            credentials=credentials, index_qks=index_qks, search_qks=search_qks
+            credentials=credentials,
+            index_qks=index_qks,
+            search_qks=search_qks,
+            order_by=order_by,
         )
 
     def query_all_kwargs(
-        self, credentials: SyftVerifyKey, **kwargs: Dict[str, Any]
+        self,
+        credentials: SyftVerifyKey,
+        **kwargs: Dict[str, Any],
     ) -> Result[List[BaseStash.object_type], str]:
+        order_by = kwargs.pop("order_by", None)
         qks = QueryKeys.from_dict(kwargs)
-        return self.query_all(credentials=credentials, qks=qks)
+        return self.query_all(credentials=credentials, qks=qks, order_by=order_by)
 
     def query_one(
-        self, credentials: SyftVerifyKey, qks: Union[QueryKey, QueryKeys]
+        self,
+        credentials: SyftVerifyKey,
+        qks: Union[QueryKey, QueryKeys],
+        order_by: Optional[PartitionKey] = None,
     ) -> Result[Optional[BaseStash.object_type], str]:
-        return self.query_all(credentials=credentials, qks=qks).and_then(first_or_none)
+        return self.query_all(
+            credentials=credentials, qks=qks, order_by=order_by
+        ).and_then(first_or_none)
 
     def query_one_kwargs(
         self,
         credentials: SyftVerifyKey,
         **kwargs: Dict[str, Any],
     ) -> Result[Optional[BaseStash.object_type], str]:
         return self.query_all_kwargs(credentials, **kwargs).and_then(first_or_none)
```

### Comparing `syft-0.8.1b3/src/syft/store/kv_document_store.py` & `syft-0.8.1b4/src/syft/store/kv_document_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from ..service.action.action_permissions import ActionObjectREAD
 from ..service.action.action_permissions import ActionObjectWRITE
 from ..service.action.action_permissions import ActionPermission
 from ..service.response import SyftSuccess
 from ..types.syft_object import SyftObject
 from ..types.uid import UID
 from .document_store import BaseStash
+from .document_store import PartitionKey
 from .document_store import PartitionSettings
 from .document_store import QueryKey
 from .document_store import QueryKeys
 from .document_store import StoreConfig
 from .document_store import StorePartition
 
 
@@ -142,19 +143,17 @@
     def __len__(self) -> int:
         return len(self.data)
 
     def _get(self, uid: UID, credentials: SyftVerifyKey) -> Result[SyftObject, str]:
         # relative
         from ..service.action.action_store import ActionObjectREAD
 
-        # TODO 🟣 Temporarily added skip permission argument for enclave
-        # until permissions are fully integrated
         # if you get something you need READ permission
         read_permission = ActionObjectREAD(uid=uid, credentials=credentials)
-        # if True:
+
         if self.has_permission(read_permission):
             syft_object = self.data[uid]
             return Ok(syft_object)
         return Err(f"Permission: {read_permission} denied")
 
     # Potentially thread-unsafe methods.
     # CAUTION:
@@ -279,39 +278,50 @@
             pass
         elif permission.permission == ActionPermission.EXECUTE:
             pass
 
         return False
 
     def _all(
-        self, credentials: SyftVerifyKey
+        self, credentials: SyftVerifyKey, order_by: Optional[PartitionKey] = None
     ) -> Result[List[BaseStash.object_type], str]:
         # this checks permissions
         res = [self._get(uid, credentials) for uid in self.data.keys()]
-        return Ok([x.ok() for x in res if x.is_ok()])
+        result = [x.ok() for x in res if x.is_ok()]
+        if order_by is not None:
+            result = sorted(result, key=lambda x: getattr(x, order_by.key, ""))
+        return Ok(result)
 
     def _remove_keys(
         self,
+        store_key: QueryKey,
         unique_query_keys: QueryKeys,
         searchable_query_keys: QueryKeys,
     ) -> None:
         uqks = unique_query_keys.all
         for qk in uqks:
             pk_key, pk_value = qk.key, qk.value
             ck_col = self.unique_keys[pk_key]
-            ck_col.pop(pk_value, None)
+            ck_col.pop(store_key.value, None)
+            self.unique_keys[pk_key] = ck_col
 
         sqks = searchable_query_keys.all
         for qk in sqks:
             pk_key, pk_value = qk.key, qk.value
             ck_col = self.searchable_keys[pk_key]
-            ck_col.pop(pk_value, None)
+            if pk_value in ck_col and (store_key.value in ck_col[pk_value]):
+                ck_col[pk_value].remove(store_key.value)
+            self.searchable_keys[pk_key] = ck_col
 
     def _find_index_or_search_keys(
-        self, credentials: SyftVerifyKey, index_qks: QueryKeys, search_qks: QueryKeys
+        self,
+        credentials: SyftVerifyKey,
+        index_qks: QueryKeys,
+        search_qks: QueryKeys,
+        order_by: Optional[PartitionKey] = None,
     ) -> Result[List[SyftObject], str]:
         ids: Optional[Set] = None
         errors = []
         # third party
         if len(index_qks.all) > 0:
             index_results = self._get_keys_index(qks=index_qks)
             if index_results.is_ok():
@@ -335,32 +345,17 @@
         if len(errors) > 0:
             return Err(" ".join(errors))
 
         if ids is None:
             return Ok([])
 
         qks: QueryKeys = self.store_query_keys(ids)
-        return self._get_all_from_store(credentials=credentials, qks=qks)
-
-    def remove_keys(
-        self,
-        unique_query_keys: QueryKeys,
-        searchable_query_keys: QueryKeys,
-    ) -> None:
-        uqks = unique_query_keys.all
-        for qk in uqks:
-            pk_key, pk_value = qk.key, qk.value
-            ck_col = self.unique_keys[pk_key]
-            ck_col.pop(pk_value, None)
-
-        sqks = searchable_query_keys.all
-        for qk in sqks:
-            pk_key, pk_value = qk.key, qk.value
-            ck_col = self.searchable_keys[pk_key]
-            ck_col.pop(pk_value, None)
+        return self._get_all_from_store(
+            credentials=credentials, qks=qks, order_by=order_by
+        )
 
     def _update(
         self,
         credentials: SyftVerifyKey,
         qk: QueryKey,
         obj: SyftObject,
         has_permission=False,
@@ -376,64 +371,65 @@
                 _original_unique_keys = self.settings.unique_keys.with_obj(
                     _original_obj
                 )
                 _original_searchable_keys = self.settings.searchable_keys.with_obj(
                     _original_obj
                 )
 
+                store_query_key = self.settings.store_key.with_obj(_original_obj)
+
                 # remove old keys
                 self._remove_keys(
+                    store_key=store_query_key,
                     unique_query_keys=_original_unique_keys,
                     searchable_query_keys=_original_searchable_keys,
                 )
 
                 # update the object with new data
-                for key, value in obj.to_dict(exclude_none=True).items():
+                for key, value in obj.to_dict(exclude_empty=True).items():
                     if key == "id":
                         # protected field
                         continue
                     setattr(_original_obj, key, value)
 
                 # update data and keys
                 self._set_data_and_keys(
-                    store_query_key=qk,
+                    store_query_key=store_query_key,
                     unique_query_keys=self.settings.unique_keys.with_obj(_original_obj),
                     searchable_query_keys=self.settings.searchable_keys.with_obj(
                         _original_obj
                     ),
                     # has been updated
                     obj=_original_obj,
                 )
 
                 # 🟡 TODO 28: Add locking in this transaction
 
-                # update the object with new data
-                for key, value in obj.to_dict(exclude_none=True).items():
-                    if key == "id":
-                        # protected field
-                        continue
-                    setattr(_original_obj, key, value)
-
                 return Ok(_original_obj)
             else:
                 return Err(f"Failed to update obj {obj}, you have no permission")
 
         except Exception as e:
             return Err(f"Failed to update obj {obj} with error: {e}")
 
     def _get_all_from_store(
-        self, credentials: SyftVerifyKey, qks: QueryKeys
+        self,
+        credentials: SyftVerifyKey,
+        qks: QueryKeys,
+        order_by: Optional[PartitionKey] = None,
     ) -> Result[List[SyftObject], str]:
         matches = []
         for qk in qks.all:
             if qk.value in self.data:
                 if self.has_permission(
                     ActionObjectREAD(uid=qk.value, credentials=credentials)
                 ):
                     matches.append(self.data[qk.value])
+        if order_by is not None:
+            matches = sorted(matches, key=lambda x: getattr(x, order_by.key, ""))
         return Ok(matches)
 
     def create(self, obj: SyftObject) -> Result[SyftObject, str]:
         pass
 
     def _delete(
         self, credentials: SyftVerifyKey, qk: QueryKey, has_permission=False
@@ -586,11 +582,17 @@
         for qk in sqks:
             pk_key, pk_value = qk.key, qk.value
             ck_col = self.searchable_keys[pk_key]
             if qk.type_list:
                 # coerce the list of objects to strings for a single key
                 pk_value = " ".join([str(obj) for obj in pk_value])
 
-            ck_col[pk_value].append(store_query_key.value)
+            # check if key is present, then add to existing key
+            if pk_value in ck_col:
+                ck_col[pk_value].append(store_query_key.value)
+            else:
+                # else create the key with a list
+                ck_col[pk_value] = [store_query_key.value]
+
             self.searchable_keys[pk_key] = ck_col
 
         self.data[store_query_key.value] = obj
```

### Comparing `syft-0.8.1b3/src/syft/store/linked_obj.py` & `syft-0.8.1b4/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/store/locks.py` & `syft-0.8.1b4/src/syft/store/locks.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
             return True
 
         owner = str(uuid.uuid4())
 
         # Acquire lock at OS level
         with self._lock_file:
             if self._data_file.exists():
-                for retry in range(10):
+                for _retry in range(10):
                     try:
                         data = json.loads(self._data_file.read_text())
                         break
                     except BaseException:
                         time.sleep(0.1)
 
                 now = self._now()
@@ -252,15 +252,15 @@
 
         if not self._data_file.exists():
             # File doesn't exist so can't be locked.
             return False
 
         with self._lock_file:
             data = None
-            for retry in range(10):
+            for _retry in range(10):
                 try:
                     data = json.loads(self._data_file.read_text())
                     break
                 except BaseException:
                     time.sleep(0.1)
 
         if data is None:
@@ -281,15 +281,15 @@
             return
 
         if not self._data_file.exists():
             return
 
         with self._lock_file:
             data = None
-            for retry in range(10):
+            for _retry in range(10):
                 try:
                     data = json.loads(self._data_file.read_text())
                     break
                 except BaseException:
                     time.sleep(0.1)
 
             if data is None:
```

### Comparing `syft-0.8.1b3/src/syft/store/mongo_client.py` & `syft-0.8.1b4/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/store/mongo_codecs.py` & `syft-0.8.1b4/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/store/mongo_document_store.py` & `syft-0.8.1b4/src/syft/store/mongo_document_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftObject
 from ..types.syft_object import SyftObjectRegistry
 from ..types.transforms import TransformContext
 from ..types.transforms import transform
 from ..types.transforms import transform_method
 from .document_store import DocumentStore
+from .document_store import PartitionKey
 from .document_store import QueryKey
 from .document_store import QueryKeys
 from .document_store import StoreConfig
 from .document_store import StorePartition
 from .locks import LockingConfig
 from .locks import NoLockingConfig
 from .mongo_client import MongoClient
@@ -270,49 +271,62 @@
         if has_permission or self.has_permission(
             ActionObjectWRITE(uid=prev_obj.id, credentials=credentials)
         ):
             # we don't want to overwrite Mongo's "id_" or Syft's "id" on update
             obj_id = obj["id"]
 
             # Set ID to the updated object value
-            setattr(obj, "id", prev_obj["id"])
+            obj.id = prev_obj["id"]
 
             # Create the Mongo object
             storage_obj = obj.to(self.storage_type)
 
             # revert the ID
-            setattr(obj, "id", obj_id)
+            obj.id = obj_id
 
             try:
                 collection.update_one(
                     filter=qk.as_dict_mongo, update={"$set": storage_obj}
                 )
             except Exception as e:
                 return Err(f"Failed to update obj: {obj} with qk: {qk}. Error: {e}")
 
             return Ok(obj)
         else:
             return Err(f"Failed to update obj {obj}, you have no permission")
 
     def _find_index_or_search_keys(
-        self, credentials: SyftVerifyKey, index_qks: QueryKeys, search_qks: QueryKeys
+        self,
+        credentials: SyftVerifyKey,
+        index_qks: QueryKeys,
+        search_qks: QueryKeys,
+        order_by: Optional[PartitionKey] = None,
     ) -> Result[List[SyftObject], str]:
         # TODO: pass index as hint to find method
         qks = QueryKeys(qks=(index_qks.all + search_qks.all))
-        return self._get_all_from_store(credentials=credentials, qks=qks)
+        return self._get_all_from_store(
+            credentials=credentials, qks=qks, order_by=order_by
+        )
 
     def _get_all_from_store(
-        self, credentials: SyftVerifyKey, qks: QueryKeys
+        self,
+        credentials: SyftVerifyKey,
+        qks: QueryKeys,
+        order_by: Optional[PartitionKey] = None,
     ) -> Result[List[SyftObject], str]:
         collection_status = self.collection
         if collection_status.is_err():
             return collection_status
         collection = collection_status.ok()
 
-        storage_objs = collection.find(filter=qks.as_dict_mongo)
+        if order_by is not None:
+            storage_objs = collection.find(filter=qks.as_dict_mongo).sort(order_by.key)
+        else:
+            _default_key = "_id"
+            storage_objs = collection.find(filter=qks.as_dict_mongo).sort(_default_key)
         syft_objs = []
         for storage_obj in storage_objs:
             obj = self.storage_type(storage_obj)
             transform_context = TransformContext(output={}, obj=obj)
             syft_objs.append(obj.to(self.settings.object_type, transform_context))
 
         # TODO: maybe do this in loop before this
@@ -341,17 +355,19 @@
 
         return Err(f"Failed to delete object with qk: {qk}")
 
     def has_permission(self, permission: ActionObjectPermission) -> bool:
         # TODO: implement
         return True
 
-    def _all(self, credentials: SyftVerifyKey):
+    def _all(self, credentials: SyftVerifyKey, order_by: Optional[PartitionKey] = None):
         qks = QueryKeys(qks=())
-        return self._get_all_from_store(credentials=credentials, qks=qks)
+        return self._get_all_from_store(
+            credentials=credentials, qks=qks, order_by=order_by
+        )
 
     def __len__(self):
         collection_status = self.collection
         if collection_status.is_err():
             return 0
         collection = collection_status.ok()
         return collection.count_documents(filter={})
```

### Comparing `syft-0.8.1b3/src/syft/store/sqlite_document_store.py` & `syft-0.8.1b4/src/syft/store/sqlite_document_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,33 +2,35 @@
 from __future__ import annotations
 
 # stdlib
 from copy import deepcopy
 from pathlib import Path
 import sqlite3
 import tempfile
-import threading
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
 
 # third party
+from pydantic import Field
+from pydantic import validator
 from result import Err
 from result import Ok
 from result import Result
 from typing_extensions import Self
 
 # relative
 from ..serde.deserialize import _deserialize
 from ..serde.serializable import serializable
 from ..serde.serialize import _serialize
 from ..types.uid import UID
+from ..util.util import thread_ident
 from .document_store import DocumentStore
 from .document_store import PartitionSettings
 from .document_store import StoreClientConfig
 from .document_store import StoreConfig
 from .kv_document_store import KeyValueBackingStore
 from .kv_document_store import KeyValueStorePartition
 from .locks import FileLockingConfig
@@ -37,18 +39,14 @@
 
 def _repr_debug_(value: Any) -> str:
     if hasattr(value, "_repr_debug_"):
         return str(value._repr_debug_())
     return repr(value)
 
 
-def thread_ident() -> int:
-    return threading.current_thread().ident
-
-
 @serializable(attrs=["index_name", "settings", "store_config"])
 class SQLiteBackingStore(KeyValueBackingStore):
     """Core Store logic for the SQLite stores.
 
     Parameters:
         `index_name`: str
             Index name
@@ -96,15 +94,16 @@
         # Set journal mode to WAL.
         # self._db[thread_ident()].execute("pragma journal_mode=wal")
 
     def create_table(self):
         try:
             self.cur.execute(
                 f"create table {self.table_name} (uid VARCHAR(32) NOT NULL PRIMARY KEY, "  # nosec
-                + "repr TEXT NOT NULL, value BLOB NOT NULL)"  # nosec
+                + "repr TEXT NOT NULL, value BLOB NOT NULL, "  # nosec
+                + "sqltime TIMESTAMP DEFAULT CURRENT_TIMESTAMP NOT NULL)"  # nosec
             )
             self.db.commit()
         except sqlite3.OperationalError as e:
             if f"table {self.table_name} already exists" not in str(e):
                 raise e
 
     @property
@@ -159,15 +158,17 @@
         insert_sql = f"update {self.table_name} set uid = ?, repr = ?, value = ? where uid = ?"  # nosec
         data = _serialize(value, to_bytes=True)
         res = self._execute(insert_sql, [str(key), _repr_debug_(value), data, str(key)])
         if res.is_err():
             raise ValueError(res.err())
 
     def _get(self, key: UID) -> Any:
-        select_sql = f"select * from {self.table_name} where uid = ?"  # nosec
+        select_sql = (
+            f"select * from {self.table_name} where uid = ? order by sqltime"  # nosec
+        )
         res = self._execute(select_sql, [str(key)])
         if res.is_err():
             raise KeyError(f"Query {select_sql} failed")
         cursor = res.ok()
 
         row = cursor.fetchone()
         if row is None or len(row) == 0:
@@ -186,15 +187,15 @@
         row = cursor.fetchone()
         if row is None:
             return False
 
         return bool(row)
 
     def _get_all(self) -> Any:
-        select_sql = f"select * from {self.table_name}"  # nosec
+        select_sql = f"select * from {self.table_name} order by sqltime"  # nosec
         keys = []
         data = []
 
         res = self._execute(select_sql)
         if res.is_err():
             return {}
         cursor = res.ok()
@@ -205,15 +206,15 @@
 
         for row in rows:
             keys.append(UID(row[0]))
             data.append(_deserialize(row[2], from_bytes=True))
         return dict(zip(keys, data))
 
     def _get_all_keys(self) -> Any:
-        select_sql = f"select uid from {self.table_name}"  # nosec
+        select_sql = f"select uid from {self.table_name} order by sqltime"  # nosec
         keys = []
 
         res = self._execute(select_sql)
         if res.is_err():
             return []
         cursor = res.ok()
 
@@ -362,27 +363,25 @@
         `timeout`: int
             How many seconds the connection should wait before raising an exception, if the database
             is locked by another connection. If another connection opens a transaction to modify the
             database, it will be locked until that transaction is committed. Default five seconds.
     """
 
     filename: Optional[str] = None
-    path: Union[str, Path]
+    path: Union[str, Path] = Field(default_factory=tempfile.gettempdir)
     check_same_thread: bool = True
     timeout: int = 5
 
-    def __init__(
-        self,
-        filename: Optional[str] = None,
-        path: Optional[Union[str, Path]] = None,
-        *args,
-        **kwargs,
-    ):
-        path_ = tempfile.gettempdir() if path is None else path
-        super().__init__(filename=filename, path=path_, *args, **kwargs)
+    # We need this in addition to Field(default_factory=...)
+    # so users can still do SQLiteStoreClientConfig(path=None)
+    @validator("path", pre=True)
+    def __default_path(cls, path: Optional[Union[str, Path]]) -> Union[str, Path]:
+        if path is None:
+            return tempfile.gettempdir()
+        return path
 
     @property
     def file_path(self) -> Optional[Path]:
         return Path(self.path) / self.filename if self.filename is not None else None
 
 
 @serializable()
```

### Comparing `syft-0.8.1b3/src/syft/types/datetime.py` & `syft-0.8.1b4/src/syft/types/datetime.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,7 +26,16 @@
 
     def __str__(self) -> str:
         utc_datetime = datetime.utcfromtimestamp(self.utc_timestamp)
         return utc_datetime.strftime("%Y-%m-%d %H:%M:%S")
 
     def __hash__(self) -> int:
         return hash(self.utc_timestamp)
+
+    def __eq__(self, other: Self) -> bool:
+        return self.utc_timestamp == other.utc_timestamp
+
+    def __lt__(self, other: Self) -> bool:
+        return self.utc_timestamp < other.utc_timestamp
+
+    def __gt__(self, other: Self) -> bool:
+        return self.utc_timestamp > other.utc_timestamp
```

### Comparing `syft-0.8.1b3/src/syft/types/grid_url.py` & `syft-0.8.1b4/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/types/syft_metaclass.py` & `syft-0.8.1b4/src/syft/types/syft_metaclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                         )
 
                 # Validation is performed in __init__, for which all fields are now optional
                 cls_init(self, *args, **kwargs)
                 # Restore requiredness
                 optionalize(fields, restore=True)
 
-        setattr(cls, "__init__", __init__)
+        cls.__init__ = __init__
 
         def iter_exclude_empty(self) -> TupleGenerator:
             for key, value in self.__dict__.items():
                 if value is not Empty:
                     yield key, value
 
         cls.__iter__ = iter_exclude_empty
```

### Comparing `syft-0.8.1b3/src/syft/types/syft_object.py` & `syft-0.8.1b4/src/syft/types/syft_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # stdlib
 from collections import defaultdict
 import inspect
 from inspect import Signature
 import types
 from typing import Any
 from typing import Callable
+from typing import ClassVar
 from typing import Dict
 from typing import KeysView
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Type
@@ -153,23 +154,25 @@
     @pydantic.root_validator(pre=True)
     def make_id(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         id_field = cls.__fields__["id"]
         if "id" not in values and id_field.required:
             values["id"] = id_field.type_()
         return values
 
-    __attr_searchable__: List[str] = []  # keys which can be searched in the ORM
-    __attr_unique__: List[str] = []
+    __attr_searchable__: ClassVar[
+        List[str]
+    ] = []  # keys which can be searched in the ORM
+    __attr_unique__: ClassVar[List[str]] = []
     # the unique keys for the particular Collection the objects will be stored in
     __serde_overrides__: Dict[
         str, Sequence[Callable]
     ] = {}  # List of attributes names which require a serde override.
     __owner__: str
 
-    __attr_repr_cols__: List[str] = []  # show these in html repr collections
+    __attr_repr_cols__: ClassVar[List[str]] = []  # show these in html repr collections
 
     def to_mongo(self) -> Dict[str, Any]:
         warnings.warn(
             "`SyftObject.to_mongo` is deprecated and will be removed in a future version",
             PendingDeprecationWarning,
         )
```

### Comparing `syft-0.8.1b3/src/syft/types/transforms.py` & `syft-0.8.1b4/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/types/twin_object.py` & `syft-0.8.1b4/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/types/uid.py` & `syft-0.8.1b4/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/util/autoreload.py` & `syft-0.8.1b4/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/util/decorators.py` & `syft-0.8.1b4/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/util/experimental_flags.py` & `syft-0.8.1b4/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/util/filterwarnings.py` & `syft-0.8.1b4/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/util/logger.py` & `syft-0.8.1b4/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/util/telemetry.py` & `syft-0.8.1b4/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft/util/trace_decorator.py` & `syft-0.8.1b4/src/syft/util/trace_decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,58 +2,64 @@
 # https://github.com/digma-ai/opentelemetry-instrumentation-digma/pull/41
 
 # stdlib
 import asyncio
 from functools import wraps
 import inspect
 from typing import Callable
+from typing import ClassVar
 from typing import Dict
 from typing import Optional
 from typing import TypeVar
 from typing import Union
+from typing import cast
 
 # third party
 from opentelemetry import trace
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import Tracer
+from opentelemetry.trace.span import Span
 
 
 class TracingDecoratorOptions:
     class NamingSchemes:
         @staticmethod
-        def function_qualified_name(func: Callable):
+        def function_qualified_name(func: Callable) -> str:
             return func.__qualname__
 
         default_scheme = function_qualified_name
 
-    naming_scheme: Callable[[Callable], str] = NamingSchemes.default_scheme
-    default_attributes: Dict[str, str] = {}
+    naming_scheme: ClassVar[Callable[[Callable], str]] = NamingSchemes.default_scheme
+    default_attributes: ClassVar[Dict[str, str]] = {}
 
-    @staticmethod
-    def set_naming_scheme(naming_scheme: Callable[[Callable], str]):
-        TracingDecoratorOptions.naming_scheme = naming_scheme
+    @classmethod
+    def set_naming_scheme(cls, naming_scheme: Callable[[Callable], str]) -> None:
+        cls.naming_scheme = naming_scheme
+
+    @classmethod
+    def set_default_attributes(
+        cls, attributes: Optional[Dict[str, str]] = None
+    ) -> None:
+        if attributes is not None:
+            for att in attributes:
+                cls.default_attributes[att] = attributes[att]
 
-    @staticmethod
-    def set_default_attributes(attributes: Dict[str, str] = None):
-        for att in attributes:
-            TracingDecoratorOptions.default_attributes[att] = attributes[att]
 
-
-T = TypeVar("T", bound=Optional[Union[Callable, type]])
+T = TypeVar("T", bound=Union[Callable, type])
 
 
 def instrument(
-    _func_or_class: T = None,
+    _func_or_class: T,
     *,
     span_name: str = "",
     record_exception: bool = True,
     attributes: Optional[Dict[str, str]] = None,
     existing_tracer: Optional[Tracer] = None,
-    ignore=False,
-):
+    ignore: bool = False,
+) -> T:
     """
     A decorator to instrument a class or function with an OTEL tracing span.
     :param cls: internal, used to specify scope of instrumentation
     :param _func_or_class: The function or span to instrument, this is automatically assigned
     :param span_name: Specify the span name explicitly, rather than use the naming convention.
     This parameter has no effect for class decorators: str
     :param record_exception: Sets whether any exceptions occurring in the span and the stacktrace are recorded
@@ -71,29 +77,31 @@
             if not name.startswith("_"):
                 if isinstance(inspect.getattr_static(cls, name), staticmethod):
                     setattr(
                         cls,
                         name,
                         staticmethod(
                             instrument(
+                                method,
                                 record_exception=record_exception,
                                 attributes=attributes,
                                 existing_tracer=existing_tracer,
-                            )(method)
+                            )
                         ),
                     )
                 else:
                     setattr(
                         cls,
                         name,
                         instrument(
+                            method,
                             record_exception=record_exception,
                             attributes=attributes,
                             existing_tracer=existing_tracer,
-                        )(method),
+                        ),
                     )
 
         return cls
 
     # Check if this is a span or class decorator
     if inspect.isclass(_func_or_class):
         return decorate_class(_func_or_class)
@@ -107,42 +115,44 @@
         # Check if already decorated (happens if both class and function
         # decorated). If so, we keep the function decorator settings only
         undecorated_func = getattr(func_or_class, "__tracing_unwrapped__", None)
         if undecorated_func:
             # We have already decorated this function, override
             return func_or_class
 
-        setattr(func_or_class, "__tracing_unwrapped__", func_or_class)
+        func_or_class.__tracing_unwrapped__ = func_or_class
 
         tracer = existing_tracer or trace.get_tracer(func_or_class.__module__)
 
-        def _set_semantic_attributes(span, func: Callable):
+        def _set_semantic_attributes(span: Span, func: Callable) -> None:
             span.set_attribute(SpanAttributes.CODE_NAMESPACE, func.__module__)
             span.set_attribute(SpanAttributes.CODE_FUNCTION, func.__qualname__)
             span.set_attribute(SpanAttributes.CODE_FILEPATH, func.__code__.co_filename)
             span.set_attribute(SpanAttributes.CODE_LINENO, func.__code__.co_firstlineno)
 
-        def _set_attributes(span, attributes_dict):
-            if attributes_dict:
+        def _set_attributes(
+            span: Span, attributes_dict: Optional[Dict[str, str]] = None
+        ) -> None:
+            if attributes_dict is not None:
                 for att in attributes_dict:
                     span.set_attribute(att, attributes_dict[att])
 
         @wraps(func_or_class)
-        def wrap_with_span_sync(*args, **kwargs):
+        def wrap_with_span_sync(*args, **kwargs):  # type: ignore
             name = span_name or TracingDecoratorOptions.naming_scheme(func_or_class)
             with tracer.start_as_current_span(
                 name, record_exception=record_exception
             ) as span:
                 _set_semantic_attributes(span, func_or_class)
                 _set_attributes(span, TracingDecoratorOptions.default_attributes)
                 _set_attributes(span, attributes)
                 return func_or_class(*args, **kwargs)
 
         @wraps(func_or_class)
-        async def wrap_with_span_async(*args, **kwargs):
+        async def wrap_with_span_async(*args, **kwargs):  # type: ignore
             name = span_name or TracingDecoratorOptions.naming_scheme(func_or_class)
             with tracer.start_as_current_span(
                 name, record_exception=record_exception
             ) as span:
                 _set_semantic_attributes(span, func_or_class)
                 _set_attributes(span, TracingDecoratorOptions.default_attributes)
                 _set_attributes(span, attributes)
@@ -154,13 +164,10 @@
         wrapper = (
             wrap_with_span_async
             if asyncio.iscoroutinefunction(func_or_class)
             else wrap_with_span_sync
         )
         wrapper.__signature__ = inspect.signature(func_or_class)
 
-        return wrapper
+        return cast(T, wrapper)
 
-    if _func_or_class is None:
-        return span_decorator
-    else:
-        return span_decorator(_func_or_class)
+    return span_decorator(_func_or_class)
```

### Comparing `syft-0.8.1b3/src/syft/util/util.py` & `syft-0.8.1b4/src/syft/util/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import os
 from pathlib import Path
 import platform
 import re
 from secrets import randbelow
 import socket
 import sys
+import threading
 import time
 from types import ModuleType
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterator
 from typing import List
@@ -849,7 +850,17 @@
         # and also for different python versions
         # to be modified in the hashing PR
         # Adding a temp fix for now
         serde_bytes = _serialize(obj, to_bytes=True)
         hash_bytes = hashlib.sha256(serde_bytes).digest()
         hashes += int.from_bytes(hash_bytes, byteorder="big")
     return hashes
+
+
+if os_name() == "macOS":
+    # needed on MacOS to prevent [__NSCFConstantString initialize] may have been in
+    # progress in another thread when fork() was called.
+    multiprocessing.set_start_method("spawn", True)
+
+
+def thread_ident() -> int:
+    return threading.current_thread().ident
```

### Comparing `syft-0.8.1b3/src/syft/util/version_compare.py` & `syft-0.8.1b4/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b3/src/syft.egg-info/PKG-INFO` & `syft-0.8.1b4/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b3
+Version: 0.8.1b4
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b3 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b4 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.1b3/src/syft.egg-info/SOURCES.txt` & `syft-0.8.1b4/src/syft.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 src/syft/client/api.py
 src/syft/client/client.py
 src/syft/client/connection.py
 src/syft/client/deploy.py
 src/syft/client/registry.py
 src/syft/client/search.py
 src/syft/client/user_settings.py
-src/syft/core/node/new/action_object.py
 src/syft/external/__init__.py
 src/syft/external/oblv/__init__.py
 src/syft/external/oblv/auth.py
 src/syft/external/oblv/constants.py
 src/syft/external/oblv/deployment.py
 src/syft/external/oblv/deployment_client.py
 src/syft/external/oblv/exceptions.py
@@ -96,18 +95,18 @@
 src/syft/service/dataset/dataset.py
 src/syft/service/dataset/dataset_service.py
 src/syft/service/dataset/dataset_stash.py
 src/syft/service/message/__init__.py
 src/syft/service/message/message_service.py
 src/syft/service/message/message_stash.py
 src/syft/service/message/messages.py
-src/syft/service/metadata/metadata_service.py
-src/syft/service/metadata/metadata_stash.py
 src/syft/service/metadata/node_metadata.py
 src/syft/service/network/network_service.py
+src/syft/service/network/node_peer.py
+src/syft/service/network/routes.py
 src/syft/service/policy/__init__.py
 src/syft/service/policy/policy.py
 src/syft/service/policy/policy_service.py
 src/syft/service/policy/user_policy_stash.py
 src/syft/service/project/__init__.py
 src/syft/service/project/project.py
 src/syft/service/project/project_service.py
@@ -116,14 +115,17 @@
 src/syft/service/queue/queue.py
 src/syft/service/queue/queue_stash.py
 src/syft/service/queue/zmq_queue.py
 src/syft/service/request/__init__.py
 src/syft/service/request/request.py
 src/syft/service/request/request_service.py
 src/syft/service/request/request_stash.py
+src/syft/service/settings/settings.py
+src/syft/service/settings/settings_service.py
+src/syft/service/settings/settings_stash.py
 src/syft/service/user/__init__.py
 src/syft/service/user/roles.py
 src/syft/service/user/user.py
 src/syft/service/user/user_roles.py
 src/syft/service/user/user_service.py
 src/syft/service/user/user_stash.py
 src/syft/service/vpn/headscale_client.py
@@ -151,11 +153,12 @@
 src/syft/util/__init__.py
 src/syft/util/autoreload.py
 src/syft/util/decorators.py
 src/syft/util/experimental_flags.py
 src/syft/util/filterwarnings.py
 src/syft/util/jax_settings.py
 src/syft/util/logger.py
+src/syft/util/schema.py
 src/syft/util/telemetry.py
 src/syft/util/trace_decorator.py
 src/syft/util/util.py
 src/syft/util/version_compare.py
```

### Comparing `syft-0.8.1b3/src/syft.egg-info/requires.txt` & `syft-0.8.1b4/src/syft.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 forbiddenfruit==0.1.4
 gevent==22.10.2
 gipc==1.5.0
 jax==0.3.14
 jaxlib==0.3.14
 loguru==0.7.0
 networkx==2.8
-numpy==1.24.2
+numpy==1.24.3
 opendp==0.6.2
 packaging>=21.0
 pandas==1.5.3
 pyarrow==11.0.0
 pycapnp==1.3.0
 pydantic[email]==1.10.7
 pymongo==4.3.3
```

