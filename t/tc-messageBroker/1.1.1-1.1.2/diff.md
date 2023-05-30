# Comparing `tmp/tc-messageBroker-1.1.1.tar.gz` & `tmp/tc-messageBroker-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc-messageBroker-1.1.1.tar", last modified: Mon May 29 12:02:49 2023, max compression
+gzip compressed data, was "tc-messageBroker-1.1.2.tar", last modified: Tue May 30 15:45:40 2023, max compression
```

## Comparing `tc-messageBroker-1.1.1.tar` & `tc-messageBroker-1.1.2.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.197578 tc-messageBroker-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-29 12:02:49.197578 tc-messageBroker-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 12:02:49.197578 tc-messageBroker-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.189578 tc-messageBroker-1.1.1/tc_messageBroker/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/message_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/db_operations/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/db_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/event/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/event/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/event/events_microservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/queue/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/queue/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/choreography.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/choreography_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/saga.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/transaction_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-29 12:02:49.000000 tc-messageBroker-1.1.1/tc_messageBroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-29 12:02:49.000000 tc-messageBroker-1.1.1/tc_messageBroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:02:49.000000 tc-messageBroker-1.1.1/tc_messageBroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-29 12:02:49.000000 tc-messageBroker-1.1.1/tc_messageBroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 12:02:49.000000 tc-messageBroker-1.1.1/tc_messageBroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/integration/test_message_broker_exchange_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/integration/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/integration/test_saga.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.197578 tc-messageBroker-1.1.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_choreagraphy_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_enum_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_message_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_predefined_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_saga_next.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_saga_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.622549 tc-messageBroker-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-30 15:45:40.622549 tc-messageBroker-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:45:40.622549 tc-messageBroker-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.614549 tc-messageBroker-1.1.2/tc_messageBroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/message_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.614549 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/db_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/db_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/event/events_microservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/queue/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/choreography.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/choreography_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/saga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/transaction_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.614549 tc-messageBroker-1.1.2/tc_messageBroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-30 15:45:40.000000 tc-messageBroker-1.1.2/tc_messageBroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-30 15:45:40.000000 tc-messageBroker-1.1.2/tc_messageBroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:45:40.000000 tc-messageBroker-1.1.2/tc_messageBroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-30 15:45:40.000000 tc-messageBroker-1.1.2/tc_messageBroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 15:45:40.000000 tc-messageBroker-1.1.2/tc_messageBroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/integration/test_message_broker_exchange_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/integration/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/integration/test_saga.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.622549 tc-messageBroker-1.1.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_choreagraphy_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_enum_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_message_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_predefined_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_saga_next.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_saga_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_transactions.py
```

### Comparing `tc-messageBroker-1.1.1/PKG-INFO` & `tc-messageBroker-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.1.1
+Version: 1.1.2
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.1.1/README.md` & `tc-messageBroker-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.1/setup.py` & `tc-messageBroker-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="tc-messageBroker",
-    version="1.1.1",
+    version="1.1.2",
     author="Mohammad Amin Dadgar, RnDAO",
     maintainer="Mohammad Amin Dadgar",
     maintainer_email="dadgaramin96@gmail.com",
     packages=find_packages(),
     description="Shared library for message broker in Python",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `tc-messageBroker-1.1.1/tc_messageBroker/message_broker.py` & `tc-messageBroker-1.1.2/tc_messageBroker/message_broker.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/db_operations/mongodb.py` & `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/db_operations/mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/choreography.py` & `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/choreography.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/saga.py` & `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/saga.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/saga_base.py` & `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/saga_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from .choreography_base import IChoreography
 from .transaction_base import ITransaction
+from .utils.saga_base_utils import get_transactions, convert_tx_dict
 from tc_messageBroker.rabbit_mq.status import Status
 import uuid
 from datetime import datetime
 import numpy as np
 from tc_messageBroker.rabbit_mq.db_operations import MongoDB
+import logging
 
 
 class Saga:
     def __init__(
         self,
         choreography: IChoreography,
         status: str,
@@ -21,55 +23,56 @@
         self.status = status
         self.data = data
         self.created_at = created_at
 
     def start(
         self,
         publish_method: callable,
-        mongo_connection: str,
+        mongo_creds: dict[str, any],
         test_mode=False,
     ):
         """
         just publish the first transaction
         """
         tx_sorted, _ = self._sort_transactions(self.choreography.transactions)
         current_tx = tx_sorted[0]
         self.status = Status.IN_PROGRESS
 
         self._update_save(
             transactions=tx_sorted,
-            mongo_connection=mongo_connection,
+            mongo_creds=mongo_creds,
             test=test_mode,
         )
 
         publish_method(
             queue_name=current_tx.queue,
             event=current_tx.event,
             content={"uuid": self.uuid},
         )
 
     def next(
         self,
         publish_method: callable,
         call_function: callable,
-        mongo_connection: str,
+        mongo_creds: dict[str, any],
         test_mode=False,
     ):
         """
         calling the next transaction within the saga
         and updating the saga state in db
 
         Parameters:
         ------------
         publish_method : RabbitMQ.publish | RabbitMQ.publish_on_exchange
             the publish methods that are from the RabbitMQ
         call_function : callable
             a function to be called when the message recieved
-        mongo_connection : str
-            the mongodb connection url to update the db
+        mongo_creds : dict[str, any]
+            the mongodb credentials to update the db
+            the keys must be `connection_str`, `db_name`, and `collection_name`
         test_mode : bool
             testing the function indicates that we wouldn't read or write on DB
             default is False
         """
         tx_sorted, tx_not_started_count = self._sort_transactions(
             self.choreography.transactions
         )
@@ -79,15 +82,15 @@
         ## get the first order transaction
         current_tx = tx_sorted[0]
 
         current_tx.status = Status.IN_PROGRESS
         current_tx.start = datetime.now()
 
         self._update_save(
-            transactions=tx_sorted, mongo_connection=mongo_connection, test=test_mode
+            transactions=tx_sorted, mongo_creds=mongo_creds, test=test_mode
         )
 
         try:
             ## the function we would call
             result = call_function()
 
             current_tx.status = Status.SUCCESS
@@ -104,29 +107,29 @@
                     queue_name=next_tx.queue,
                     event=next_tx.event,
                     content={"uuid": self.uuid, "data": result},
                 )
 
             self._update_save(
                 transactions=tx_sorted,
-                mongo_connection=mongo_connection,
+                mongo_creds=mongo_creds,
                 test=test_mode,
             )
 
         except Exception as exp:
             current_tx.error = str(exp)
 
             if current_tx.status != Status.SUCCESS:
                 current_tx.status = Status.FAILED
 
             self.status = Status.FAILED
 
             self._update_save(
                 transactions=tx_sorted,
-                mongo_connection=mongo_connection,
+                mongo_creds=mongo_creds,
                 test=test_mode,
             )
 
     def _sort_transactions(self, transactions: list[ITransaction]):
         """
         sort transactions by their order and status
         the NOT_STARTED ones would be at the first of the list
@@ -180,26 +183,27 @@
         """
         orders = [tx.order for tx in transactions]
         sorted_indices = np.argsort(orders)
 
         return np.array(transactions)[sorted_indices]
 
     def _update_save(
-        self, transactions: list[ITransaction], mongo_connection, test=False
+        self, transactions: list[ITransaction], mongo_creds: dict[str, any], test=False
     ):
         """
         update the transactions in saga choreography and then save data to db
 
         test is the test mode which it does not interact with db.
         default is False meaning we have to have an interaction with db
         """
         if not test:
             ## save the status into DB
-            mongodb = MongoDB(mongo_connection)
-            mongodb.connect()
+            mongodb = self._get_mongo_db(
+                mongo_creds=mongo_creds,
+            )
             data = self._create_data()
 
             ## creating a duplicate choreography to avoid shallow copy
             choreography = IChoreography(
                 name=self.choreography.name, transactions=transactions
             )
 
@@ -217,23 +221,42 @@
         ---------
         data : dict[str, any]
             the dictionary representing the current saga document
 
         """
         data = {}
 
-        data["choreography"] = self.choreography
+        data["choreography"] = {}
+        data["choreography"]["name"] = self.choreography.name
+        data["choreography"]["transactions"] = {}
+        for idx, tx in enumerate(self.choreography.transactions):
+            transaction = convert_tx_dict(tx)
+            data["choreography"]["transactions"][str(idx)] = transaction
+
         data["status"] = self.status
         data["data"] = self.data
         data["sagaId"] = self.uuid
         data["createdAt"] = self.created_at
         data["updatedAt"] = datetime.now()
 
         return data
 
+    def _get_mongo_db(self, mongo_creds: dict[str, any], test=False):
+        """
+        get mongodb instance
+        """
+        ## save the status into DB
+        mongodb = MongoDB(
+            connection_str=mongo_creds["connection_str"],
+            db_name=mongo_creds["db_name"],
+            collection_name=mongo_creds["collection_name"],
+        )
+        mongodb.connect()
+        return mongodb
+
 
 def get_saga(guildId: str, connection_url: str, db_name: str, collection: str):
     """
     get saga object for a special guild
 
     Parameters:
     ------------
@@ -254,16 +277,27 @@
     mongodb = MongoDB(
         connection_str=connection_url, db_name=db_name, collection_name=collection
     )
     mongodb.connect()
 
     data = mongodb.read(query={"data.guildId": guildId}, count=1)
 
-    saga_obj = Saga(
-        choreography=data["choreography"],
-        status=data["status"],
-        created_at=data["createdAt"],
-        sagaId=data["sagaId"],
-        data=data["data"],
+    transactions = get_transactions(data["choreography"]["transactions"])
+
+    choreography = IChoreography(
+        name=data["choreography"]["name"],
+        transactions=transactions,
     )
 
+    saga_obj = None
+    if data is not None:
+        saga_obj = Saga(
+            choreography=choreography,
+            status=data["status"],
+            created_at=data["createdAt"],
+            sagaId=data["sagaId"],
+            data=data["data"],
+        )
+    else:
+        logging.error("Error! no saga available for this!")
+
     return saga_obj
```

### Comparing `tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/transaction_base.py` & `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/transaction_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/transactions.py` & `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/transactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,11 +37,11 @@
     #     Event.DISCORD_BOT.FETCH,
     #     order=1,
     #     status=Status.NOT_STARTED,
     # ),
     ITransaction(
         Queue.DISCORD_ANALYZER,
         Event.DISCORD_ANALYZER.RUN_ONCE,
-        order=2,
+        order=1,
         status=Status.NOT_STARTED,
     ),
 ]
```

### Comparing `tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py` & `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,16 @@
                                         Status.IN_PROGRESS,
                                         Status.SUCCESS,
                                         Status.FAILED,
                                         Status.CANCELLED,
                                     ],
                                 },
                                 "message": {"type": "string"},
-                                "start": {"type": "string"},
-                                "end": {"type": "string"},
+                                "start": {},
+                                "end": {},
                                 "runtime": {"type": "number"},
                                 "error": {"type": "string"},
                             },
                             "required": ["queue", "event", "order", "status"],
                             "additionalProperties": False,
                         }
                     },
@@ -52,13 +52,13 @@
                 Status.IN_PROGRESS,
                 Status.SUCCESS,
                 Status.FAILED,
                 Status.CANCELLED,
             ],
         },
         "data": {"type": "object"},
-        "createdAt": {"type": "string", "format": "date-time"},
-        "updatedAt": {"type": "string", "format": "date-time"},
+        "createdAt": {},
+        "updatedAt": {},
     },
     "required": ["sagaId", "choreography", "status", "createdAt", "updatedAt"],
     "additionalProperties": False,
 }
```

### Comparing `tc-messageBroker-1.1.1/tc_messageBroker.egg-info/PKG-INFO` & `tc-messageBroker-1.1.2/tc_messageBroker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.1.1
+Version: 1.1.2
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.1.1/tc_messageBroker.egg-info/SOURCES.txt` & `tc-messageBroker-1.1.2/tc_messageBroker.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 tc_messageBroker/rabbit_mq/saga/choreography_base.py
 tc_messageBroker/rabbit_mq/saga/saga.py
 tc_messageBroker/rabbit_mq/saga/saga_base.py
 tc_messageBroker/rabbit_mq/saga/transaction_base.py
 tc_messageBroker/rabbit_mq/saga/transactions.py
 tc_messageBroker/rabbit_mq/saga/utils/__init__.py
 tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
+tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
 tests/__init__.py
 tests/integration/__init__.py
 tests/integration/test_message_broker_exchange_points.py
 tests/integration/test_mongodb.py
 tests/integration/test_saga.py
 tests/unit/__init__.py
 tests/unit/test_choreagraphy_base.py
 tests/unit/test_enum_status.py
 tests/unit/test_event.py
 tests/unit/test_message_broker.py
 tests/unit/test_predefined_transactions.py
 tests/unit/test_queue.py
 tests/unit/test_saga_base.py
+tests/unit/test_saga_base_utils.py
 tests/unit/test_saga_next.py
 tests/unit/test_saga_start.py
 tests/unit/test_transactions.py
```

### Comparing `tc-messageBroker-1.1.1/tests/integration/test_message_broker_exchange_points.py` & `tc-messageBroker-1.1.2/tests/integration/test_message_broker_exchange_points.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.1/tests/integration/test_mongodb.py` & `tc-messageBroker-1.1.2/tests/integration/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.1/tests/integration/test_saga.py` & `tc-messageBroker-1.1.2/tests/integration/test_saga.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.1/tests/unit/test_choreagraphy_base.py` & `tc-messageBroker-1.1.2/tests/unit/test_choreagraphy_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.1/tests/unit/test_message_broker.py` & `tc-messageBroker-1.1.2/tests/unit/test_message_broker.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.1/tests/unit/test_predefined_transactions.py` & `tc-messageBroker-1.1.2/tests/unit/test_predefined_transactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,11 +27,11 @@
 
     assert len(tx) == 1
     # assert tx[0].order == 1
     # assert tx[0].queue == Queue.DISCORD_BOT
     # assert tx[0].event == Event.DISCORD_BOT.FETCH
     # assert tx[0].status == Status.NOT_STARTED
 
-    assert tx[0].order == 2
+    assert tx[0].order == 1
     assert tx[0].queue == Queue.DISCORD_ANALYZER
     assert tx[0].event == Event.DISCORD_ANALYZER.RUN_ONCE
     assert tx[0].status == Status.NOT_STARTED
```

### Comparing `tc-messageBroker-1.1.1/tests/unit/test_saga_base.py` & `tc-messageBroker-1.1.2/tests/unit/test_saga_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.1/tests/unit/test_saga_next.py` & `tc-messageBroker-1.1.2/tests/unit/test_saga_next.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         return calculations
 
     saga = Saga(choreography, Status.NOT_STARTED, data=None, created_at=datetime.now())
 
     saga.next(
         publish_method=sample_publish,
         call_function=sample_call,
-        mongo_connection="",
+        mongo_creds={},
         test_mode=True,
     )
 
     assert saga.status == Status.SUCCESS
     assert saga.choreography.transactions[1].status == Status.SUCCESS
 
 
@@ -62,15 +62,15 @@
         return calculations
 
     saga = Saga(choreography, Status.NOT_STARTED, data=None, created_at=datetime.now())
 
     saga.next(
         publish_method=sample_publish,
         call_function=sample_call,
-        mongo_connection="",
+        mongo_creds={},
         test_mode=True,
     )
 
     assert saga.status == Status.IN_PROGRESS
     assert saga.choreography.transactions[1].status == Status.SUCCESS
 
 
@@ -96,15 +96,15 @@
         return calculations
 
     saga = Saga(choreography, Status.NOT_STARTED, data=None, created_at=datetime.now())
 
     saga.next(
         publish_method=sample_publish,
         call_function=sample_call,
-        mongo_connection="",
+        mongo_creds={},
         test_mode=True,
     )
 
     assert saga.status == Status.FAILED
     assert saga.choreography.transactions[1].status == Status.SUCCESS
 
 
@@ -130,13 +130,13 @@
         return calculations
 
     saga = Saga(choreography, Status.NOT_STARTED, data=None, created_at=datetime.now())
 
     saga.next(
         publish_method=sample_publish,
         call_function=sample_call,
-        mongo_connection="",
+        mongo_creds={},
         test_mode=True,
     )
 
     assert saga.status == Status.FAILED
     assert saga.choreography.transactions[1].status == Status.FAILED
```

### Comparing `tc-messageBroker-1.1.1/tests/unit/test_saga_start.py` & `tc-messageBroker-1.1.2/tests/unit/test_saga_start.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def sample_publish(**kwargs):
         assert kwargs["queue_name"] == choreography.transactions[1].queue
         assert kwargs["event"] == choreography.transactions[1].event
         assert kwargs["content"]["uuid"] == saga.uuid
 
     saga.start(
         publish_method=sample_publish,
-        mongo_connection="",
+        mongo_creds={},
         test_mode=True,
     )
 
     assert saga.status == Status.IN_PROGRESS
     assert saga.choreography.transactions[0].status == Status.NOT_STARTED
     assert saga.choreography.transactions[1].status == Status.NOT_STARTED
     assert saga.choreography.transactions[2].status == Status.SUCCESS
```

### Comparing `tc-messageBroker-1.1.1/tests/unit/test_transactions.py` & `tc-messageBroker-1.1.2/tests/unit/test_transactions.py`

 * *Files identical despite different names*

