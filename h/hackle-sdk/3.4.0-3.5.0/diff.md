# Comparing `tmp/hackle-sdk-3.4.0.tar.gz` & `tmp/hackle-sdk-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hackle-sdk-3.4.0.tar", last modified: Tue Mar  7 04:02:05 2023, max compression
+gzip compressed data, was "dist/hackle-sdk-3.5.0.tar", last modified: Tue May 30 07:20:39 2023, max compression
```

## Comparing `hackle-sdk-3.4.0.tar` & `hackle-sdk-3.5.0.tar`

### file list

```diff
@@ -1,74 +1,215 @@
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.122788 hackle-sdk-3.4.0/
--rw-r--r--   0 teddykwon   (501) staff       (20)     1500 2023-03-07 04:02:05.122456 hackle-sdk-3.4.0/PKG-INFO
--rw-r--r--   0 teddykwon   (501) staff       (20)      776 2020-12-02 08:27:28.000000 hackle-sdk-3.4.0/README.md
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.093960 hackle-sdk-3.4.0/hackle/
--rw-r--r--   0 teddykwon   (501) staff       (20)        0 2020-08-06 09:08:29.000000 hackle-sdk-3.4.0/hackle/__init__.py
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.096643 hackle-sdk-3.4.0/hackle/commons/
--rw-r--r--   0 teddykwon   (501) staff       (20)        0 2020-08-07 04:13:28.000000 hackle-sdk-3.4.0/hackle/commons/__init__.py
--rw-r--r--   0 teddykwon   (501) staff       (20)      905 2022-06-28 01:10:31.000000 hackle-sdk-3.4.0/hackle/commons/enums.py
--rw-r--r--   0 teddykwon   (501) staff       (20)      165 2021-06-22 12:41:01.000000 hackle-sdk-3.4.0/hackle/commons/utils.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     2768 2022-12-23 04:15:15.000000 hackle-sdk-3.4.0/hackle/commons/validator.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     2732 2022-12-23 04:15:15.000000 hackle-sdk-3.4.0/hackle/decision.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     6752 2022-12-23 04:15:15.000000 hackle-sdk-3.4.0/hackle/entities.py
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.097847 hackle-sdk-3.4.0/hackle/evaluation/
--rw-r--r--   0 teddykwon   (501) staff       (20)        0 2021-09-15 05:07:09.000000 hackle-sdk-3.4.0/hackle/evaluation/__init__.py
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.098965 hackle-sdk-3.4.0/hackle/evaluation/action/
--rw-r--r--   0 teddykwon   (501) staff       (20)        0 2021-09-15 05:07:09.000000 hackle-sdk-3.4.0/hackle/evaluation/action/__init__.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     1493 2022-08-29 05:43:50.000000 hackle-sdk-3.4.0/hackle/evaluation/action/action_resolver.py
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.100244 hackle-sdk-3.4.0/hackle/evaluation/bucket/
--rw-r--r--   0 teddykwon   (501) staff       (20)        0 2021-09-15 05:07:09.000000 hackle-sdk-3.4.0/hackle/evaluation/bucket/__init__.py
--rw-r--r--   0 teddykwon   (501) staff       (20)      497 2022-08-29 05:43:50.000000 hackle-sdk-3.4.0/hackle/evaluation/bucket/bucketer.py
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.101509 hackle-sdk-3.4.0/hackle/evaluation/container/
--rw-r--r--   0 teddykwon   (501) staff       (20)        0 2022-08-29 05:43:50.000000 hackle-sdk-3.4.0/hackle/evaluation/container/__init__.py
--rw-r--r--   0 teddykwon   (501) staff       (20)      664 2022-08-29 05:43:50.000000 hackle-sdk-3.4.0/hackle/evaluation/container/container_resolver.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     5283 2022-12-23 04:15:15.000000 hackle-sdk-3.4.0/hackle/evaluation/evaluator.py
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.104587 hackle-sdk-3.4.0/hackle/evaluation/flow/
--rw-r--r--   0 teddykwon   (501) staff       (20)        0 2021-09-15 05:07:09.000000 hackle-sdk-3.4.0/hackle/evaluation/flow/__init__.py
--rw-r--r--   0 teddykwon   (501) staff       (20)      924 2022-12-12 08:49:23.000000 hackle-sdk-3.4.0/hackle/evaluation/flow/evaluation_flow.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     2544 2022-12-23 04:15:15.000000 hackle-sdk-3.4.0/hackle/evaluation/flow/evaluation_flow_factory.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     8659 2022-12-12 08:49:23.000000 hackle-sdk-3.4.0/hackle/evaluation/flow/flow_evaluator.py
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.108980 hackle-sdk-3.4.0/hackle/evaluation/match/
--rw-r--r--   0 teddykwon   (501) staff       (20)        0 2021-09-15 05:07:09.000000 hackle-sdk-3.4.0/hackle/evaluation/match/__init__.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     4685 2022-10-31 08:30:32.000000 hackle-sdk-3.4.0/hackle/evaluation/match/condition_matcher.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     6369 2023-03-07 03:59:53.000000 hackle-sdk-3.4.0/hackle/evaluation/match/operator_matcher.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     4046 2022-06-28 01:10:31.000000 hackle-sdk-3.4.0/hackle/evaluation/match/semantic_version.py
--rw-r--r--   0 teddykwon   (501) staff       (20)      894 2021-09-15 05:07:09.000000 hackle-sdk-3.4.0/hackle/evaluation/match/target_matcher.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     2741 2023-03-07 03:59:53.000000 hackle-sdk-3.4.0/hackle/evaluation/match/value_matcher.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     2431 2022-12-23 04:15:15.000000 hackle-sdk-3.4.0/hackle/evaluation/match/value_operator_matcher.py
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.112075 hackle-sdk-3.4.0/hackle/evaluation/target/
--rw-r--r--   0 teddykwon   (501) staff       (20)        0 2021-09-15 05:07:09.000000 hackle-sdk-3.4.0/hackle/evaluation/target/__init__.py
--rw-r--r--   0 teddykwon   (501) staff       (20)      440 2022-06-28 01:10:31.000000 hackle-sdk-3.4.0/hackle/evaluation/target/experiment_target_determiner.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     1269 2022-08-29 05:43:50.000000 hackle-sdk-3.4.0/hackle/evaluation/target/override_resolver.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     1076 2022-12-23 04:15:15.000000 hackle-sdk-3.4.0/hackle/evaluation/target/remote_config_target_rule_determiner.py
--rw-r--r--   0 teddykwon   (501) staff       (20)      364 2022-06-28 01:10:31.000000 hackle-sdk-3.4.0/hackle/evaluation/target/target_rule_determiner.py
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.114526 hackle-sdk-3.4.0/hackle/event/
--rw-r--r--   0 teddykwon   (501) staff       (20)        0 2020-08-10 11:06:13.000000 hackle-sdk-3.4.0/hackle/event/__init__.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     1329 2022-06-28 01:10:31.000000 hackle-sdk-3.4.0/hackle/event/event_dispatcher.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     6427 2022-12-23 04:15:15.000000 hackle-sdk-3.4.0/hackle/event/event_processor.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     2213 2022-12-23 04:15:15.000000 hackle-sdk-3.4.0/hackle/event/user_event.py
--rw-r--r--   0 teddykwon   (501) staff       (20)       54 2020-08-07 09:09:52.000000 hackle-sdk-3.4.0/hackle/exceptions.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     7208 2022-12-23 04:15:15.000000 hackle-sdk-3.4.0/hackle/hackle.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     3312 2022-12-23 04:15:15.000000 hackle-sdk-3.4.0/hackle/internal_client.py
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.115656 hackle-sdk-3.4.0/hackle/lib/
--rw-r--r--   0 teddykwon   (501) staff       (20)        0 2020-08-10 07:03:38.000000 hackle-sdk-3.4.0/hackle/lib/__init__.py
--rwxr-xr-x   0 teddykwon   (501) staff       (20)    13699 2020-08-06 09:00:23.000000 hackle-sdk-3.4.0/hackle/lib/pymmh3.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     1392 2022-10-26 10:37:30.000000 hackle-sdk-3.4.0/hackle/logger.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     3457 2023-01-12 07:23:38.000000 hackle-sdk-3.4.0/hackle/model.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     1408 2022-12-23 04:15:15.000000 hackle-sdk-3.4.0/hackle/remote_config.py
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.118855 hackle-sdk-3.4.0/hackle/user/
--rw-r--r--   0 teddykwon   (501) staff       (20)        0 2022-08-29 05:43:50.000000 hackle-sdk-3.4.0/hackle/user/__init__.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     1933 2022-08-29 05:43:50.000000 hackle-sdk-3.4.0/hackle/user/hackle_user_resolver.py
--rw-r--r--   0 teddykwon   (501) staff       (20)       91 2022-08-29 05:43:50.000000 hackle-sdk-3.4.0/hackle/user/identifier_type.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     1648 2022-11-01 11:15:54.000000 hackle-sdk-3.4.0/hackle/user/identifiers_builder.py
--rw-r--r--   0 teddykwon   (501) staff       (20)      429 2022-08-29 05:43:50.000000 hackle-sdk-3.4.0/hackle/user/internal_hackle_user.py
--rw-r--r--   0 teddykwon   (501) staff       (20)       78 2023-03-07 04:01:58.000000 hackle-sdk-3.4.0/hackle/version.py
--rw-r--r--   0 teddykwon   (501) staff       (20)    12322 2022-12-23 04:15:15.000000 hackle-sdk-3.4.0/hackle/workspace.py
--rw-r--r--   0 teddykwon   (501) staff       (20)     2921 2022-10-26 10:37:47.000000 hackle-sdk-3.4.0/hackle/workspace_fetcher.py
-drwxr-xr-x   0 teddykwon   (501) staff       (20)        0 2023-03-07 04:02:05.121860 hackle-sdk-3.4.0/hackle_sdk.egg-info/
--rw-r--r--   0 teddykwon   (501) staff       (20)     1500 2023-03-07 04:02:05.000000 hackle-sdk-3.4.0/hackle_sdk.egg-info/PKG-INFO
--rw-r--r--   0 teddykwon   (501) staff       (20)     1889 2023-03-07 04:02:05.000000 hackle-sdk-3.4.0/hackle_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 teddykwon   (501) staff       (20)        1 2023-03-07 04:02:05.000000 hackle-sdk-3.4.0/hackle_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 teddykwon   (501) staff       (20)       56 2023-03-07 04:02:05.000000 hackle-sdk-3.4.0/hackle_sdk.egg-info/requires.txt
--rw-r--r--   0 teddykwon   (501) staff       (20)        7 2023-03-07 04:02:05.000000 hackle-sdk-3.4.0/hackle_sdk.egg-info/top_level.txt
--rw-r--r--   0 teddykwon   (501) staff       (20)       38 2023-03-07 04:02:05.122883 hackle-sdk-3.4.0/setup.cfg
--rw-r--r--   0 teddykwon   (501) staff       (20)     1283 2022-11-03 09:04:20.000000 hackle-sdk-3.4.0/setup.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.473806 hackle-sdk-3.5.0/
+-rw-r--r--   0 yong       (501) staff       (20)     1895 2023-05-30 07:20:39.473114 hackle-sdk-3.5.0/PKG-INFO
+-rw-r--r--   0 yong       (501) staff       (20)      776 2020-12-16 04:01:56.000000 hackle-sdk-3.5.0/README.md
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.320122 hackle-sdk-3.5.0/hackle/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2020-11-02 11:39:11.000000 hackle-sdk-3.5.0/hackle/__init__.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.321202 hackle-sdk-3.5.0/hackle/commons/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2020-11-02 11:26:30.000000 hackle-sdk-3.5.0/hackle/commons/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)      313 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/commons/enums.py
+-rw-r--r--   0 yong       (501) staff       (20)     2802 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/decision.py
+-rw-r--r--   0 yong       (501) staff       (20)       54 2020-11-02 11:26:30.000000 hackle-sdk-3.5.0/hackle/exceptions.py
+-rw-r--r--   0 yong       (501) staff       (20)     8273 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/hackle.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.322373 hackle-sdk-3.5.0/hackle/internal/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/__init__.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.322985 hackle-sdk-3.5.0/hackle/internal/concurrent/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/concurrent/__init__.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.323852 hackle-sdk-3.5.0/hackle/internal/concurrent/atomic/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/concurrent/atomic/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)      700 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/concurrent/atomic/atomic_integer.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.325783 hackle-sdk-3.5.0/hackle/internal/concurrent/schedule/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/concurrent/schedule/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)      598 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/concurrent/schedule/scheduler.py
+-rw-r--r--   0 yong       (501) staff       (20)     1564 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/concurrent/schedule/thread_scheduler.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.326408 hackle-sdk-3.5.0/hackle/internal/evaluation/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/__init__.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.327423 hackle-sdk-3.5.0/hackle/internal/evaluation/action/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/action/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     2117 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/action/action_resolver.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.328554 hackle-sdk-3.5.0/hackle/internal/evaluation/bucket/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/bucket/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)      536 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/bucket/bucketer.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.329571 hackle-sdk-3.5.0/hackle/internal/evaluation/container/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/container/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     1247 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/container/container_resolver.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.331340 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)      652 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/delegating_evaluator.py
+-rw-r--r--   0 yong       (501) staff       (20)     6054 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/evaluator.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.333938 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/experiment/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/experiment/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     3432 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/experiment/experiment_evaluation.py
+-rw-r--r--   0 yong       (501) staff       (20)     1129 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/experiment/experiment_evaluator.py
+-rw-r--r--   0 yong       (501) staff       (20)     1901 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/experiment/experiment_request.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.336223 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/remoteconfig/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/remoteconfig/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     2494 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/remoteconfig/remote_config_evaluation.py
+-rw-r--r--   0 yong       (501) staff       (20)     3604 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/remoteconfig/remote_config_evaluator.py
+-rw-r--r--   0 yong       (501) staff       (20)     1409 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/evaluator/remoteconfig/remote_config_request.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.339118 hackle-sdk-3.5.0/hackle/internal/evaluation/flow/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/flow/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     1778 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/flow/evaluation_flow.py
+-rw-r--r--   0 yong       (501) staff       (20)     2762 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/flow/evaluation_flow_factory.py
+-rw-r--r--   0 yong       (501) staff       (20)     9350 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/flow/flow_evaluator.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.350866 hackle-sdk-3.5.0/hackle/internal/evaluation/match/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/match/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)      495 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/match/condition_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     2111 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/match/condition_matcher_factory.py
+-rw-r--r--   0 yong       (501) staff       (20)     5713 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/match/experiment_condition_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     6417 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/match/operator_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     3006 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/match/segment_condition_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     4046 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/match/semantic_version.py
+-rw-r--r--   0 yong       (501) staff       (20)     1469 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/match/target_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     1794 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/match/user_condition_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     2764 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/match/value_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     3200 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/match/value_operator_matcher.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.356011 hackle-sdk-3.5.0/hackle/internal/evaluation/target/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/target/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)      890 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/target/experiment_target_determiner.py
+-rw-r--r--   0 yong       (501) staff       (20)      901 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/target/experiment_target_rule_determiner.py
+-rw-r--r--   0 yong       (501) staff       (20)     2179 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/target/override_resolver.py
+-rw-r--r--   0 yong       (501) staff       (20)     2000 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/evaluation/target/remote_config_target_rule_determiner.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.361726 hackle-sdk-3.5.0/hackle/internal/event/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/event/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     4127 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/event/event_dispatcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     4475 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/event/event_processor.py
+-rw-r--r--   0 yong       (501) staff       (20)     4587 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/event/user_event.py
+-rw-r--r--   0 yong       (501) staff       (20)     2500 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/event/user_event_factory.py
+-rw-r--r--   0 yong       (501) staff       (20)     6996 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/hackle_core.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.363561 hackle-sdk-3.5.0/hackle/internal/http/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/http/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     1408 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/http/http_client.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.365428 hackle-sdk-3.5.0/hackle/internal/logger/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/logger/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)      372 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/logger/log.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.369594 hackle-sdk-3.5.0/hackle/internal/model/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/model/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     7329 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/model/entities.py
+-rw-r--r--   0 yong       (501) staff       (20)     3307 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/model/properties_builder.py
+-rw-r--r--   0 yong       (501) staff       (20)      572 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/model/sdk.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.372073 hackle-sdk-3.5.0/hackle/internal/time/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/time/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)      375 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/time/clock.py
+-rw-r--r--   0 yong       (501) staff       (20)      706 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/time/time_unit.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.373217 hackle-sdk-3.5.0/hackle/internal/type/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/type/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     1252 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/type/hackle_types.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.376716 hackle-sdk-3.5.0/hackle/internal/user/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/user/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     1525 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/user/hackle_user_resolver.py
+-rw-r--r--   0 yong       (501) staff       (20)       91 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/user/identifier_type.py
+-rw-r--r--   0 yong       (501) staff       (20)     2034 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/user/identifiers_builder.py
+-rw-r--r--   0 yong       (501) staff       (20)     2705 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/user/internal_hackle_user.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.378970 hackle-sdk-3.5.0/hackle/internal/workspace/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/workspace/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)    12343 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/workspace/workspace.py
+-rw-r--r--   0 yong       (501) staff       (20)     1640 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/internal/workspace/workspace_fetcher.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.380175 hackle-sdk-3.5.0/hackle/lib/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2020-11-02 11:26:30.000000 hackle-sdk-3.5.0/hackle/lib/__init__.py
+-rwxr-xr-x   0 yong       (501) staff       (20)    13699 2023-05-19 11:36:28.000000 hackle-sdk-3.5.0/hackle/lib/pymmh3.py
+-rw-r--r--   0 yong       (501) staff       (20)     1392 2023-03-07 10:58:13.000000 hackle-sdk-3.5.0/hackle/logger.py
+-rw-r--r--   0 yong       (501) staff       (20)    11701 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/model.py
+-rw-r--r--   0 yong       (501) staff       (20)     1662 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/hackle/remote_config.py
+-rw-r--r--   0 yong       (501) staff       (20)       78 2023-05-30 07:15:55.000000 hackle-sdk-3.5.0/hackle/version.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.383980 hackle-sdk-3.5.0/hackle_sdk.egg-info/
+-rw-r--r--   0 yong       (501) staff       (20)     1895 2023-05-30 07:20:39.000000 hackle-sdk-3.5.0/hackle_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yong       (501) staff       (20)     7732 2023-05-30 07:20:39.000000 hackle-sdk-3.5.0/hackle_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yong       (501) staff       (20)        1 2023-05-30 07:20:39.000000 hackle-sdk-3.5.0/hackle_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yong       (501) staff       (20)       56 2023-05-30 07:20:39.000000 hackle-sdk-3.5.0/hackle_sdk.egg-info/requires.txt
+-rw-r--r--   0 yong       (501) staff       (20)       13 2023-05-30 07:20:39.000000 hackle-sdk-3.5.0/hackle_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yong       (501) staff       (20)       38 2023-05-30 07:20:39.473977 hackle-sdk-3.5.0/setup.cfg
+-rw-r--r--   0 yong       (501) staff       (20)     1283 2023-03-07 10:58:13.000000 hackle-sdk-3.5.0/setup.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.312985 hackle-sdk-3.5.0/tests/
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.386220 hackle-sdk-3.5.0/tests/internal/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/__init__.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.387791 hackle-sdk-3.5.0/tests/internal/concurrent/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/concurrent/__init__.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.389779 hackle-sdk-3.5.0/tests/internal/concurrent/schedule/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/concurrent/schedule/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     1642 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/concurrent/schedule/test_threading_scheduler.py
+-rw-r--r--   0 yong       (501) staff       (20)      373 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/concurrent/test_concurrent_supports.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.390810 hackle-sdk-3.5.0/tests/internal/evaluation/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/__init__.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.392496 hackle-sdk-3.5.0/tests/internal/evaluation/action/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/action/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     5961 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/action/test_action_resolver.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.396944 hackle-sdk-3.5.0/tests/internal/evaluation/bucket/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/bucket/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     1065 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/bucket/test_buckter.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.399934 hackle-sdk-3.5.0/tests/internal/evaluation/container/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/container/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     4265 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/container/test_container_resolver_test.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.404300 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/__init__.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.410575 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/experiment/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/experiment/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     5540 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/experiment/test_experiment_evaluation.py
+-rw-r--r--   0 yong       (501) staff       (20)     2069 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/experiment/test_experiment_evaluator.py
+-rw-r--r--   0 yong       (501) staff       (20)      675 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/experiment/test_experiment_request.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.416950 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/remoteconfig/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/remoteconfig/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     2058 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/remoteconfig/test_remote_config_evaluation.py
+-rw-r--r--   0 yong       (501) staff       (20)     7600 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/remoteconfig/test_remote_config_evaluator.py
+-rw-r--r--   0 yong       (501) staff       (20)      993 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/remoteconfig/test_remote_config_request.py
+-rw-r--r--   0 yong       (501) staff       (20)     1259 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/test_delegating_evaluator.py
+-rw-r--r--   0 yong       (501) staff       (20)     2290 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/test_evaluator_context.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.421268 hackle-sdk-3.5.0/tests/internal/evaluation/flow/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/flow/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     1965 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/flow/test_evaluation_flow.py
+-rw-r--r--   0 yong       (501) staff       (20)     1740 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/flow/test_evaluation_flow_factory.py
+-rw-r--r--   0 yong       (501) staff       (20)    24560 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/flow/test_flow_evaluator.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.438520 hackle-sdk-3.5.0/tests/internal/evaluation/match/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     7738 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/test_ab_test_condition_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     1262 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/test_condition_matcher_factory.py
+-rw-r--r--   0 yong       (501) staff       (20)     2487 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/test_experiment_condition_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     4188 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/test_feature_flag_condition_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)    13764 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/test_operator_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     4159 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/test_segment_condition_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     2056 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/test_segment_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     5233 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/test_semantic_version.py
+-rw-r--r--   0 yong       (501) staff       (20)     2092 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/test_target_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     2569 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/test_user_condition_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     1788 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/test_user_value_resolver.py
+-rw-r--r--   0 yong       (501) staff       (20)     5287 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/test_value_matcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     4541 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/match/test_value_operator_matcer.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.444415 hackle-sdk-3.5.0/tests/internal/evaluation/target/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/target/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     2469 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/target/test_experiment_target_determiner.py
+-rw-r--r--   0 yong       (501) staff       (20)     2704 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/target/test_experiment_target_rule_determiner.py
+-rw-r--r--   0 yong       (501) staff       (20)     6807 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/target/test_override_resolver.py
+-rw-r--r--   0 yong       (501) staff       (20)     5240 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/evaluation/target/test_remote_target_rule_determiner.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.452383 hackle-sdk-3.5.0/tests/internal/event/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/event/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     2539 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/event/test_event_dispatcher.py
+-rw-r--r--   0 yong       (501) staff       (20)     3767 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/event/test_event_processor.py
+-rw-r--r--   0 yong       (501) staff       (20)      238 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/event/test_in_memory_event_processor.py
+-rw-r--r--   0 yong       (501) staff       (20)     2936 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/event/test_user_event.py
+-rw-r--r--   0 yong       (501) staff       (20)     3688 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/event/test_user_event_factory.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.454345 hackle-sdk-3.5.0/tests/internal/http/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/http/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     1862 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/http/test_http_client.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.458811 hackle-sdk-3.5.0/tests/internal/model/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/model/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     1793 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/model/test_entities.py
+-rw-r--r--   0 yong       (501) staff       (20)     2746 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/model/test_properties_builder.py
+-rw-r--r--   0 yong       (501) staff       (20)      302 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/model/test_sdk.py
+-rw-r--r--   0 yong       (501) staff       (20)    14776 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/test_hackle_core.py
+-rw-r--r--   0 yong       (501) staff       (20)     5180 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/test_hackle_core_2.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.460873 hackle-sdk-3.5.0/tests/internal/time/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/time/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)      717 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/time/test_clock.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.462831 hackle-sdk-3.5.0/tests/internal/type/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/type/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     4355 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/type/test_hackle_types.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.467136 hackle-sdk-3.5.0/tests/internal/workspace/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/workspace/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)      336 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/workspace/test_resource_workspace_fetcher.py
+-rw-r--r--   0 yong       (501) staff       (20)      810 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/workspace/test_workspace.py
+-rw-r--r--   0 yong       (501) staff       (20)     2578 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/internal/workspace/test_workspace_fetcher.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.469005 hackle-sdk-3.5.0/tests/resources/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/resources/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)      143 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/resources/test_resource_reader.py
+drwxr-xr-x   0 yong       (501) staff       (20)        0 2023-05-30 07:20:39.471920 hackle-sdk-3.5.0/tests/user/
+-rw-r--r--   0 yong       (501) staff       (20)        0 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/user/__init__.py
+-rw-r--r--   0 yong       (501) staff       (20)     6650 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/user/test_hackle_user_resolver.py
+-rw-r--r--   0 yong       (501) staff       (20)     2300 2023-05-30 07:12:34.000000 hackle-sdk-3.5.0/tests/user/test_identifier_builder.py
```

### Comparing `hackle-sdk-3.4.0/README.md` & `hackle-sdk-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hackle-sdk-3.4.0/hackle/decision.py` & `hackle-sdk-3.5.0/hackle/decision.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     EXPERIMENT_NOT_FOUND = 'EXPERIMENT_NOT_FOUND'
     EXPERIMENT_DRAFT = 'EXPERIMENT_DRAFT'
     EXPERIMENT_PAUSED = 'EXPERIMENT_PAUSED'
     EXPERIMENT_COMPLETED = 'EXPERIMENT_COMPLETED'
     OVERRIDDEN = 'OVERRIDDEN'
     TRAFFIC_NOT_ALLOCATED = 'TRAFFIC_NOT_ALLOCATED'
     TRAFFIC_ALLOCATED = 'TRAFFIC_ALLOCATED'
+    TRAFFIC_ALLOCATED_BY_TARGETING = 'TRAFFIC_ALLOCATED_BY_TARGETING'
     VARIATION_DROPPED = 'VARIATION_DROPPED'
     NOT_IN_EXPERIMENT_TARGET = 'NOT_IN_EXPERIMENT_TARGET'
     NOT_IN_MUTUAL_EXCLUSION_EXPERIMENT = 'NOT_IN_MUTUAL_EXCLUSION_EXPERIMENT'
     IDENTIFIER_NOT_FOUND = 'IDENTIFIER_NOT_FOUND'
 
     FEATURE_FLAG_NOT_FOUND = 'FEATURE_FLAG_NOT_FOUND'
     FEATURE_FLAG_INACTIVE = 'FEATURE_FLAG_INACTIVE'
```

### Comparing `hackle-sdk-3.4.0/hackle/entities.py` & `hackle-sdk-3.5.0/hackle/internal/model/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,30 @@
             return False
 
 
 class Experiment(BaseEntity):
 
     def __init__(self, id, key, type, identifier_type, status, version, variations, user_overrides, segment_overrides,
                  target_audiences, target_rules, default_rule, container_id, winner_variation_id):
+        """
+        :param int id:
+        :param int key:
+        :param str type:
+        :param str identifier_type:
+        :param str status:
+        :param int version:
+        :param list[Variation] variations:
+        :param dict[str, int] user_overrides:
+        :param list[TargetRule] segment_overrides:
+        :param list[Target] target_audiences:
+        :param list[TargetRule] target_rules:
+        :param TargetAction default_rule:
+        :param int or None container_id:
+        :param int or None winner_variation_id:
+        """
         self.id = id
         self.key = key
         self.type = type
         self.identifier_type = identifier_type
         self.status = status
         self.version = version
         self.variations = variations
@@ -128,15 +144,15 @@
 
     def supports(self, target_key_type):
         return target_key_type in self.supported_key_types
 
 
 class TargetingTypes(object):
     IDENTIFIER = TargetingType('SEGMENT')
-    PROPERTY = TargetingType('SEGMENT', 'USER_PROPERTY', 'HACKLE_PROPERTY')
+    PROPERTY = TargetingType('SEGMENT', 'USER_PROPERTY', 'HACKLE_PROPERTY', 'AB_TEST', 'FEATURE_FLAG')
     SEGMENT = TargetingType('USER_ID', 'USER_PROPERTY', 'HACKLE_PROPERTY')
 
 
 class Container(object):
 
     def __init__(self, id, bucket_id, groups):
         self.id = id
```

### Comparing `hackle-sdk-3.4.0/hackle/evaluation/flow/evaluation_flow.py` & `hackle-sdk-3.5.0/tests/internal/evaluation/evaluator/test_delegating_evaluator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,41 @@
-from hackle.decision import DecisionReason
-from hackle.evaluation.evaluator import Evaluation
+from unittest import TestCase
+from unittest.mock import Mock
 
+from hackle.internal.evaluation.evaluator.delegating_evaluator import DelegatingEvaluator
+from hackle.internal.evaluation.evaluator.evaluator import Evaluator, ContextualEvaluator
 
-class EvaluationFlow(object):
 
-    def __init__(self, flow_evaluator=None, next_flow=None):
-        self.flow_evaluator = flow_evaluator
-        self.next_flow = next_flow
-
-    def evaluate(self, workspace, experiment, user, default_variation_key):
-        if self.is_end():
-            return Evaluation.of(workspace, experiment, default_variation_key, DecisionReason.TRAFFIC_NOT_ALLOCATED)
-        else:
-            return self.flow_evaluator.evaluate(workspace, experiment, user, default_variation_key, self.next_flow)
-
-    def is_end(self):
-        return self.flow_evaluator is None or self.next_flow is None
-
-    @staticmethod
-    def of(*flow_evaluators):
-        flow = EvaluationFlow()
-        for flow_evaluator in reversed(flow_evaluators):
-            flow = EvaluationFlow(flow_evaluator, flow)
-        return flow
+class DelegatingEvaluatorTest(TestCase):
+
+    def test_evaluate(self):
+        sut = DelegatingEvaluator()
+
+        r1 = Mock(spec=Evaluator.Request)
+        e1 = Mock(spec=Evaluator.Evaluation)
+        evaluator1 = MockEvaluator(r1, e1)
+
+        sut.add(evaluator1)
+        with self.assertRaises(Exception):
+            sut.evaluate(Mock(), Mock())
+        self.assertEqual(e1, sut.evaluate(r1, Evaluator.context()))
+
+        r2 = Mock(spec=Evaluator.Request)
+        e2 = Mock(spec=Evaluator.Evaluation)
+        evaluator2 = MockEvaluator(r2, e2)
+
+        sut.add(evaluator2)
+        self.assertEqual(e2, sut.evaluate(r2, Evaluator.context()))
+
+
+class MockEvaluator(ContextualEvaluator):
+
+    def __init__(self, request, evaluation):
+        super(MockEvaluator, self).__init__()
+        self.__request = request
+        self.__evaluation = evaluation
+
+    def supports(self, request):
+        return request == self.__request
+
+    def evaluate_internal(self, request, context):
+        return self.__evaluation
```

### Comparing `hackle-sdk-3.4.0/hackle/evaluation/flow/evaluation_flow_factory.py` & `hackle-sdk-3.5.0/hackle/internal/evaluation/flow/evaluation_flow_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,62 @@
-from hackle import logger as _logging
-from hackle.evaluation.action.action_resolver import ActionResolver
-from hackle.evaluation.bucket.bucketer import Bucketer
-from hackle.evaluation.container.container_resolver import ContainerResolver
-from hackle.evaluation.flow.evaluation_flow import EvaluationFlow
-from hackle.evaluation.flow.flow_evaluator import *
-from hackle.evaluation.match.condition_matcher import ConditionMatcherFactory
-from hackle.evaluation.match.target_matcher import TargetMatcher
-from hackle.evaluation.target.experiment_target_determiner import ExperimentTargetDeterminer
-from hackle.evaluation.target.override_resolver import OverrideResolver
-from hackle.evaluation.target.remote_config_target_rule_determiner import RemoteConfigTargetRuleDeterminer
-from hackle.evaluation.target.target_rule_determiner import TargetRuleDeterminer
+from hackle.internal.evaluation.bucket.bucketer import Bucketer
+from hackle.internal.evaluation.evaluator.evaluator import Evaluator
+from hackle.internal.evaluation.flow.flow_evaluator import *
+from hackle.internal.evaluation.match.condition_matcher_factory import ConditionMatcherFactory
+from hackle.internal.evaluation.match.target_matcher import TargetMatcher
+from hackle.internal.evaluation.target.experiment_target_determiner import ExperimentTargetDeterminer
+from hackle.internal.evaluation.target.experiment_target_rule_determiner import ExperimentTargetRuleDeterminer
+from hackle.internal.evaluation.target.override_resolver import OverrideResolver
+from hackle.internal.evaluation.target.remote_config_target_rule_determiner import RemoteConfigTargetRuleDeterminer, \
+    RemoteConfigTargetRuleMatcher
 
 
 class EvaluationFlowFactory(object):
 
-    def __init__(self, logger=None):
-        self.logger = _logging.adapt_logger(logger or _logging.NoOpLogger())
-
+    def __init__(self, evaluator):
+        """
+        :param Evaluator evaluator:
+        """
         bucketer = Bucketer()
-        target_matcher = TargetMatcher(ConditionMatcherFactory())
-        action_resolver = ActionResolver(bucketer, self.logger)
+        target_matcher = TargetMatcher(ConditionMatcherFactory(evaluator))
+        action_resolver = ActionResolver(bucketer)
         override_resolver = OverrideResolver(target_matcher, action_resolver)
         container_resolver = ContainerResolver(bucketer)
 
-        self.ab_test_flow = EvaluationFlow.of(
+        self.__ab_test_flow = EvaluationFlow.of(
             OverrideEvaluator(override_resolver),
             IdentifierEvaluator(),
             ContainerEvaluator(container_resolver),
             ExperimentTargetEvaluator(ExperimentTargetDeterminer(target_matcher)),
             DraftEvaluator(),
             PausedEvaluator(),
             CompletedEvaluator(),
             TrafficAllocateEvaluator(action_resolver)
         )
 
-        self.feature_flag_flow = EvaluationFlow.of(
+        self.__feature_flag_flow = EvaluationFlow.of(
             DraftEvaluator(),
             PausedEvaluator(),
             CompletedEvaluator(),
             OverrideEvaluator(override_resolver),
             IdentifierEvaluator(),
-            TargetRuleEvaluator(TargetRuleDeterminer(target_matcher), action_resolver),
+            TargetRuleEvaluator(ExperimentTargetRuleDeterminer(target_matcher), action_resolver),
             DefaultRuleEvaluator(action_resolver)
         )
 
-        self.remote_config_parameter_target_rule_determiner = RemoteConfigTargetRuleDeterminer(target_matcher, bucketer)
+        self.__remote_config_parameter_target_rule_determiner = RemoteConfigTargetRuleDeterminer(
+            RemoteConfigTargetRuleMatcher(target_matcher, bucketer))
 
     def get_evaluation_flow(self, experiment_type):
         if experiment_type == 'AB_TEST':
-            return self.ab_test_flow
+            return self.__ab_test_flow
         elif experiment_type == 'FEATURE_FLAG':
-            return self.feature_flag_flow
+            return self.__feature_flag_flow
         else:
             raise Exception('Unsupported type [{}]'.format(experiment_type))
+
+    @property
+    def remote_config_parameter_target_rule_determiner(self):
+        """
+        :rtype: RemoteConfigTargetRuleDeterminer 
+        """
+        return self.__remote_config_parameter_target_rule_determiner
```

### Comparing `hackle-sdk-3.4.0/hackle/evaluation/match/operator_matcher.py` & `hackle-sdk-3.5.0/hackle/internal/evaluation/match/operator_matcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 
 from six import add_metaclass, string_types
 
-from hackle.commons import validator
-from hackle.evaluation.match.semantic_version import SemanticVersion
+from hackle.internal.evaluation.match.semantic_version import SemanticVersion
+from hackle.internal.type import hackle_types
 
 
 @add_metaclass(abc.ABCMeta)
 class OperatorMatcher(object):
 
     @abc.abstractmethod
     def string_matches(self, user_value, match_value):
@@ -30,15 +30,15 @@
     def string_matches(self, user_value, match_value):
         if isinstance(user_value, string_types) and isinstance(match_value, string_types):
             return user_value == match_value
         else:
             return False
 
     def number_matches(self, user_value, match_value):
-        if validator.is_finite_number(user_value) and validator.is_finite_number(match_value):
+        if hackle_types.is_finite_number(user_value) and hackle_types.is_finite_number(match_value):
             return user_value == match_value
         else:
             return False
 
     def bool_matches(self, user_value, match_value):
         if isinstance(user_value, bool) and isinstance(match_value, bool):
             return user_value == match_value
@@ -107,15 +107,15 @@
     def string_matches(self, user_value, match_value):
         if isinstance(user_value, string_types) and isinstance(match_value, string_types):
             return user_value > match_value
         else:
             return False
 
     def number_matches(self, user_value, match_value):
-        if validator.is_finite_number(user_value) and validator.is_finite_number(match_value):
+        if hackle_types.is_finite_number(user_value) and hackle_types.is_finite_number(match_value):
             return user_value > match_value
         else:
             return False
 
     def bool_matches(self, user_value, match_value):
         return False
 
@@ -130,15 +130,15 @@
     def string_matches(self, user_value, match_value):
         if isinstance(user_value, string_types) and isinstance(match_value, string_types):
             return user_value >= match_value
         else:
             return False
 
     def number_matches(self, user_value, match_value):
-        if validator.is_finite_number(user_value) and validator.is_finite_number(match_value):
+        if hackle_types.is_finite_number(user_value) and hackle_types.is_finite_number(match_value):
             return user_value >= match_value
         else:
             return False
 
     def bool_matches(self, user_value, match_value):
         return False
 
@@ -153,15 +153,15 @@
     def string_matches(self, user_value, match_value):
         if isinstance(user_value, string_types) and isinstance(match_value, string_types):
             return user_value < match_value
         else:
             return False
 
     def number_matches(self, user_value, match_value):
-        if validator.is_finite_number(user_value) and validator.is_finite_number(match_value):
+        if hackle_types.is_finite_number(user_value) and hackle_types.is_finite_number(match_value):
             return user_value < match_value
         else:
             return False
 
     def bool_matches(self, user_value, match_value):
         return False
 
@@ -176,15 +176,15 @@
     def string_matches(self, user_value, match_value):
         if isinstance(user_value, string_types) and isinstance(match_value, string_types):
             return user_value <= match_value
         else:
             return False
 
     def number_matches(self, user_value, match_value):
-        if validator.is_finite_number(user_value) and validator.is_finite_number(match_value):
+        if hackle_types.is_finite_number(user_value) and hackle_types.is_finite_number(match_value):
             return user_value <= match_value
         else:
             return False
 
     def bool_matches(self, user_value, match_value):
         return False
```

### Comparing `hackle-sdk-3.4.0/hackle/evaluation/match/semantic_version.py` & `hackle-sdk-3.5.0/hackle/internal/evaluation/match/semantic_version.py`

 * *Files identical despite different names*

### Comparing `hackle-sdk-3.4.0/hackle/evaluation/match/value_matcher.py` & `hackle-sdk-3.5.0/hackle/internal/evaluation/match/value_matcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 
 from six import add_metaclass, string_types
 
-from hackle.commons import validator
-from hackle.evaluation.match.semantic_version import SemanticVersion
+from hackle.internal.evaluation.match.semantic_version import SemanticVersion
+from hackle.internal.type import hackle_types
 
 
 @add_metaclass(abc.ABCMeta)
 class ValueMatcher(object):
 
     @abc.abstractmethod
     def matches(self, operator_matcher, user_value, match_value):
@@ -23,15 +23,15 @@
         else:
             return False
 
     @staticmethod
     def __string_or_none(value):
         if isinstance(value, string_types):
             return value
-        elif validator.is_finite_number(value):
+        elif hackle_types.is_finite_number(value):
             return str(value)
         else:
             return None
 
 
 class NumberValueMatcher(ValueMatcher):
     def matches(self, operator_matcher, user_value, match_value):
@@ -40,20 +40,20 @@
         if number_user_value is not None and number_match_value is not None:
             return operator_matcher.number_matches(number_user_value, number_match_value)
         else:
             return False
 
     @staticmethod
     def __number_or_none(value):
-        if validator.is_finite_number(value):
+        if hackle_types.is_finite_number(value):
             return value
         elif isinstance(value, string_types):
             try:
                 number = float(value)
-                if validator.is_finite_number(number):
+                if hackle_types.is_finite_number(number):
                     return number
                 else:
                     return None
             except ValueError:
                 return None
         else:
             return None
@@ -76,8 +76,7 @@
         else:
             return False
 
 
 class NoneValueMatcher(ValueMatcher):
     def matches(self, operator_matcher, user_value, match_value):
         return False
-
```

### Comparing `hackle-sdk-3.4.0/hackle/evaluation/match/value_operator_matcher.py` & `hackle-sdk-3.5.0/hackle/internal/evaluation/match/value_operator_matcher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,58 @@
-from hackle import logger as _logging
-from hackle.evaluation.match.operator_matcher import *
-from hackle.evaluation.match.value_matcher import *
+from hackle.internal.evaluation.match.operator_matcher import *
+from hackle.internal.evaluation.match.value_matcher import *
+from hackle.internal.logger.log import Log
 
 
 class ValueOperatorMatcher(object):
 
-    def __init__(self, factory, logger=None):
+    def __init__(self, factory):
         self.factory = factory
-        self.logger = _logging.adapt_logger(logger or _logging.NoOpLogger())
 
     def matches(self, user_value, match):
         value_matcher = self.factory.get_value_matcher_or_none(match.value_type)
         if not value_matcher:
-            self.logger.debug('Unsupported type[{}]. Please use the latest version of sdk.'.format(match.value_type))
+            Log.get().debug('Unsupported type[{}]. Please use the latest version of sdk.'.format(match.value_type))
             return False
 
         operator_matcher = self.factory.get_operator_matcher_or_none(match.operator)
         if not operator_matcher:
-            self.logger.debug('Unsupported type[{}]. Please use the latest version of sdk.'.format(match.operator))
+            Log.get().debug('Unsupported type[{}]. Please use the latest version of sdk.'.format(match.operator))
             return False
 
+        is_matched = self.__matches(user_value, match, value_matcher, operator_matcher)
+        return self.__type_matches(match.type, is_matched)
+
+    def __matches(self, user_value, match, value_matcher, operator_matcher):
+        if isinstance(user_value, list):
+            return self.__array_matches(user_value, match, value_matcher, operator_matcher)
+        else:
+            return self.__single_matches(user_value, match, value_matcher, operator_matcher)
+
+    # noinspection PyMethodMayBeStatic
+    def __single_matches(self, user_value, match, value_matcher, operator_matcher):
         for match_value in match.values:
             if value_matcher.matches(operator_matcher, user_value, match_value):
-                return self._matches(match.type, True)
+                return True
+        return False
 
-        return self._matches(match.type, False)
+    def __array_matches(self, user_values, match, value_matcher, operator_matcher):
+        for user_value in user_values:
+            if self.__single_matches(user_value, match, value_matcher, operator_matcher):
+                return True
+        return False
 
-    def _matches(self, match_type, is_matched):
+    # noinspection PyMethodMayBeStatic
+    def __type_matches(self, match_type, is_matched):
         if match_type == 'MATCH':
             return is_matched
         elif match_type == 'NOT_MATCH':
             return not is_matched
         else:
-            self.logger.debug('Unsupported type[{}]. Please use the latest version of sdk.'.format(match_type))
+            Log.get().debug('Unsupported type[{}]. Please use the latest version of sdk.'.format(match_type))
             return False
 
 
 class ValueOperatorMatcherFactory(object):
 
     def __init__(self):
         self._value_matchers = {
```

### Comparing `hackle-sdk-3.4.0/hackle/hackle.py` & `hackle-sdk-3.5.0/hackle/hackle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+from six.moves.queue import Queue
+
 from . import exceptions as hackle_exceptions
 from . import logger as _logging
-from .commons import utils
-from .commons import validator
+from . import version
+from .commons.enums import Default
 from .decision import ExperimentDecision, DecisionReason, FeatureFlagDecision
-from .evaluation.evaluator import Evaluator
-from .evaluation.flow.evaluation_flow_factory import EvaluationFlowFactory
-from .event.event_dispatcher import EventDispatcher
-from .event.event_processor import BatchEventProcessor
-from .internal_client import InternalClient
+from .internal.concurrent.schedule.thread_scheduler import ThreadScheduler
+from .internal.event.event_dispatcher import EventDispatcher
+from .internal.event.event_processor import EventProcessor
+from .internal.hackle_core import HackleCore
+from .internal.http.http_client import HttpClient
+from .internal.logger.log import Log
+from .internal.model.sdk import Sdk
+from .internal.type import hackle_types
+from .internal.user.hackle_user_resolver import HackleUserResolver
+from .internal.workspace.workspace_fetcher import WorkspaceFetcher
+from .model import HackleEvent, HackleRemoteConfig, PropertyOperations
 from .remote_config import HackleRemoteConfigImpl
-from .user.hackle_user_resolver import HackleUserResolver
-from .workspace_fetcher import WorkspaceFetcher
 
 
 def __singleton(cls):
     instance = [None]
 
     def wrapper(*args, **kwargs):
         if instance[0] is None:
@@ -26,27 +32,44 @@
 
 @__singleton
 class Client(object):
     def __init__(self, sdk_key=None, logger=None, timeout=None):
         if sdk_key is None:
             raise hackle_exceptions.RequiredParameterException('sdk_key must not be empty.')
 
-        self.logger = _logging.adapt_logger(logger or _logging.NoOpLogger())
+        Log.initialize(_logging.adapt_logger(logger or _logging.NoOpLogger()))
+
+        sdk = Sdk(sdk_key, "python-sdk", version.__version__)
+
+        http_client = HttpClient(sdk)
 
-        self.internal_client = InternalClient(
-            evaluator=Evaluator(EvaluationFlowFactory(self.logger)),
-            workspace_fetcher=WorkspaceFetcher(sdk_key, logger=self.logger, timeout=timeout),
-            event_processor=BatchEventProcessor(sdk_key, EventDispatcher(), self.logger),
-            logger=self.logger
+        workspace_fetcher = WorkspaceFetcher(
+            sdk_base_url=Default.SDK_URL,
+            http_client=http_client,
+            polling_interval_seconds=10,
+            scheduler=ThreadScheduler()
         )
 
-        self.hackle_user_resolver = HackleUserResolver(logger)
+        event_processor = EventProcessor(
+            queue=Queue(maxsize=1000),
+            event_dispatcher=EventDispatcher(Default.EVENT_URL, http_client),
+            event_dispatch_size=500,
+            flush_scheduler=ThreadScheduler(),
+            flush_interval_seconds=10,
+            shutdown_timeout_seconds=10
+        )
+
+        workspace_fetcher.start()
+        event_processor.start()
+
+        self._core = HackleCore.create(workspace_fetcher, event_processor)
+        self._user_resolver = HackleUserResolver()
 
     def close(self):
-        self.internal_client.close()
+        self._core.close()
 
     def __exit__(self):
         self.close()
 
     def variation(self, experiment_key, user, default_variation='A'):
         """
         Decide the variation to expose to the user for experiment.
@@ -57,108 +80,124 @@
             - The user is not allocated to the experiment
             - The decided variation has been dropped
 
         :param int experiment_key: the unique key of the experiment.
         :param hackle.model.User or hackle.model.HackleUser user: the user to participate in the experiment.
         :param str default_variation: the default variation of the experiment.
 
+        :rtype: str
         :return: the decided variation for the user, or the default variation.
         """
         return self.variation_detail(experiment_key, user, default_variation).variation
 
     def variation_detail(self, experiment_key, user, default_variation='A'):
         """
         Decide the variation to expose to the user for experiment, and returns an object that
         describes the way the variation was decided.
 
         :param int experiment_key: the unique key of the experiment.
         :param hackle.model.User or hackle.model.HackleUser user: the user to participate in the experiment.
         :param str default_variation: the default variation of the experiment.
 
-        :return: a object describing the result
+        :rtype: hackle.decision.ExperimentDecision
+        :return: an object describing the result
         """
         try:
-            if not validator.is_non_zero_and_empty_int(experiment_key):
-                self.logger.error('Experiment Key must not be empty. : {}'.format(experiment_key))
+            if not hackle_types.is_positive_int(experiment_key):
+                Log.get().warning('Invalid experiment_key: {} (expected: positive integer)'.format(experiment_key))
                 return ExperimentDecision(default_variation, DecisionReason.INVALID_INPUT)
 
-            hackle_user = self.hackle_user_resolver.resolve_or_none(user)
+            hackle_user = self._user_resolver.resolve_or_none(user)
             if hackle_user is None:
                 return ExperimentDecision(default_variation, DecisionReason.INVALID_INPUT)
 
-            return self.internal_client.experiment(experiment_key, hackle_user, default_variation)
+            return self._core.experiment(experiment_key, hackle_user, default_variation)
         except Exception as e:
-            self.logger.error(
-                "Unexpected error while deciding variation of experiment[{}]: {}".format(experiment_key, str(e)))
+            Log.get().error(
+                'Unexpected error while deciding variation of experiment[{}]: {}'.format(experiment_key, str(e)))
             return ExperimentDecision(default_variation, DecisionReason.EXCEPTION)
 
     def is_feature_on(self, feature_key, user):
         """
         Decide whether the feature is turned on to the user.
 
-        :param int feature_key: the unique key of the feature.
-        :param hackle.model.User or hackle.model.HackleUser user: the user to participate in the experiment.
+        :param int feature_key: the unique key for the feature.
+        :param hackle.model.User or hackle.model.HackleUser user: the user requesting the feature.
+
+        :rtype: bool
         :return: True if the feature is on
-                  False if the feature is off
+                 False if the feature is off
         """
         return self.feature_flag_detail(feature_key, user).is_on
 
     def feature_flag_detail(self, feature_key, user):
         """
         Decide whether the feature is turned on to the user, and returns an object that
         describes the way the value was decided.
 
         :param int feature_key: the unique key of the feature.
-        :param hackle.model.User or hackle.model.HackleUser user: the user to participate in the experiment.
+        :param hackle.model.User or hackle.model.HackleUser user: the user requesting the feature.
 
-        :return: a object describing the result
+        :rtype: hackle.decision.FeatureFlagDecision
+        :return: an object describing the result
         """
         try:
-
-            if not validator.is_non_zero_and_empty_int(feature_key):
-                self.logger.error('Experiment Key must not be empty. : {}'.format(feature_key))
+            if not hackle_types.is_positive_int(feature_key):
+                Log.get().warning('Invalid feature_key: {} (expected: positive integer)'.format(feature_key))
                 return FeatureFlagDecision(False, DecisionReason.INVALID_INPUT)
 
-            hackle_user = self.hackle_user_resolver.resolve_or_none(user)
+            hackle_user = self._user_resolver.resolve_or_none(user)
             if hackle_user is None:
                 return FeatureFlagDecision(False, DecisionReason.INVALID_INPUT)
 
-            return self.internal_client.feature_flag(feature_key, hackle_user)
+            return self._core.feature_flag(feature_key, hackle_user)
         except Exception as e:
-            self.logger.error("Unexpected error while deciding feature flag[{}]: {}".format(feature_key, str(e)))
+            Log.get().error('Unexpected error while deciding feature flag[{}]: {}'.format(feature_key, str(e)))
             return FeatureFlagDecision(False, DecisionReason.EXCEPTION)
 
     def track(self, event, user):
         """
-        Records the event performed by the user with additional numeric value.
+        Records the event that occurred by the user.
 
-        :param hackle.model.Event event: the unique key of the event. MUST NOT be null.
-        :param hackle.model.User or hackle.model.HackleUser user: the user to participate in the experiment.
+        :param hackle.model.Event or hackle.model.HackleEvent event: the event that occurred.
+        :param hackle.model.User or hackle.model.HackleUser user: the user that occurred the event.
         """
         try:
-            if not validator.is_valid_event(event):
-                self.logger.error('Event is not valid. Event must be hackle.model.event and event.id\'s type must be '
-                                  'string_types. value\'s type must be numeric. '
-                                  ': {}'.format(event))
+            hackle_event = HackleEvent.from_event(event)
+            if not hackle_event.is_valid:
+                Log.get().warning('Invalid event for track: [{}]'.format(hackle_event.error_or_none))
                 return
 
-            if not validator.is_valid_properties(event.properties):
-                self.logger.warning(
-                    'Event properties is not valid. Event properties must be not dic types and items types must be string_types, number, bool.'
-                    ': {}'.format(event.properties))
-                event.properties = utils.filter_properties(event.properties)
-
-            hackle_user = self.hackle_user_resolver.resolve_or_none(user)
+            hackle_user = self._user_resolver.resolve_or_none(user)
             if hackle_user is None:
                 return
 
-            self.internal_client.track_event(event, hackle_user)
+            self._core.track(hackle_event, hackle_user)
         except Exception as e:
-            self.logger.error('Unexpected error while tracking event: {}'.format(str(e)))
+            Log.get().error('Unexpected error while tracking event: {}'.format(str(e)))
 
     def remote_config(self, user):
         """
         Returns a instance of Hackle Remote Config.
 
         :param hackle.model.User or hackle.model.HackleUser user: the identifier of user.
+        :rtype: HackleRemoteConfig
+        """
+        return HackleRemoteConfigImpl(user, self._core, self._user_resolver)
+
+    def update_user_properties(self, operations, user):
+        """
+        Updates the user's properties.
+
+        :param hackle.model.PropertyOperations operations: Property operations to update user properties.
+        :param hackle.model.HackleUser user: the user whos properties will be updated.
         """
-        return HackleRemoteConfigImpl(user, self.internal_client, self.hackle_user_resolver)
+        try:
+            if not isinstance(operations, PropertyOperations):
+                Log.get().warning(
+                    'Invalid user property update operations: {} (expected: PropertyOperations)'.format(operations))
+                return
+
+            event = operations.to_event()
+            self.track(event, user)
+        except Exception as e:
+            Log.get().error('Unexpected exception while update user properties: {}'.format(str(e)))
```

### Comparing `hackle-sdk-3.4.0/hackle/lib/pymmh3.py` & `hackle-sdk-3.5.0/hackle/lib/pymmh3.py`

 * *Files identical despite different names*

### Comparing `hackle-sdk-3.4.0/hackle/logger.py` & `hackle-sdk-3.5.0/hackle/logger.py`

 * *Files identical despite different names*

### Comparing `hackle-sdk-3.4.0/hackle/remote_config.py` & `hackle-sdk-3.5.0/hackle/remote_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 from .decision import RemoteConfigDecision, DecisionReason
-from .commons import validator
-from .model import HackleRemoteConfig
+from .internal.hackle_core import HackleCore
+from .internal.type import hackle_types
+from .internal.user.hackle_user_resolver import HackleUserResolver
+from .model import HackleRemoteConfig, HackleUser
 
 
 class HackleRemoteConfigImpl(HackleRemoteConfig):
-    def __init__(self, user, internal_client, hackle_user_resolver):
-        self.user = user
-        self.internal_client = internal_client
-        self.hackle_user_resolver = hackle_user_resolver
+    def __init__(self, user, core, hackle_user_resolver):
+        """
+        :param HackleUser user:
+        :param HackleCore core:
+        :param HackleUserResolver hackle_user_resolver:
+        """
+        self.__user = user
+        self.__core = core
+        self.__hackle_user_resolver = hackle_user_resolver
 
     def get(self, key, default=None):
-        if validator.is_string(default):
+        if hackle_types.is_string(default):
             parameter_value = self.__get(key, 'STRING', default).value
-        elif validator.is_number(default):
+        elif hackle_types.is_number(default):
             parameter_value = self.__get(key, 'NUMBER', default).value
-        elif validator.is_bool(default):
+        elif hackle_types.is_bool(default):
             parameter_value = self.__get(key, 'BOOLEAN', default).value
         elif default is None:
             parameter_value = self.__get(key, 'NULL', default).value
         else:
             parameter_value = self.__get(key, 'UNKNOWN', default).value
 
         return parameter_value
 
     def __get(self, key, required_type, default):
-        hackle_user = self.hackle_user_resolver.resolve_or_none(self.user)
+        hackle_user = self.__hackle_user_resolver.resolve_or_none(self.__user)
 
         if hackle_user is None:
             return RemoteConfigDecision(default, DecisionReason.INVALID_INPUT)
 
         if key is None:
             return RemoteConfigDecision(default, DecisionReason.INVALID_INPUT)
 
-        return self.internal_client.remote_config(hackle_user, key, required_type, default)
+        return self.__core.remote_config(key, hackle_user, required_type, default)
```

### Comparing `hackle-sdk-3.4.0/hackle/user/identifiers_builder.py` & `hackle-sdk-3.5.0/hackle/internal/user/identifiers_builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,64 @@
-from six import string_types
-
-from hackle import logger as _logging
+from hackle.internal.logger.log import Log
+from hackle.internal.type import hackle_types
 
 
 class IdentifiersBuilder(object):
+    __MAX_IDENTIFIER_TYPE_LENGTH = 128
+    __MAX_IDENTIFIER_VALUE_LENGTH = 512
+
+    def __init__(self):
+        self.__identifiers = {}
 
-    def __init__(self, logger=None):
-        self.logger = _logging.adapt_logger(logger or _logging.NoOpLogger())
-        self.identifiers = {}
+    def build(self):
+        return self.__identifiers
 
     def add_identifiers(self, identifiers):
         if identifiers is None:
             return self
 
         if not isinstance(identifiers, dict):
-            self.logger.warning('Identifiers must be dictionary.')
+            Log.get().warning('Identifiers MUST be dictionary [Request Type={}]'.format(type(identifiers)))
             return self
 
         for identifier_type in identifiers:
             self.add(identifier_type, identifiers[identifier_type])
 
         return self
 
     def add(self, identifier_type, identifier_value):
-        if self._is_valid(identifier_type, identifier_value):
-            self.identifiers[identifier_type] = identifier_value
+
+        sanitized_identifier_value = self.sanitize_value_or_none(identifier_value)
+        if self.__is_value_type(identifier_type) and sanitized_identifier_value is not None:
+            self.__identifiers[identifier_type] = sanitized_identifier_value
         else:
-            self.logger.warning('Invalid user identifier [type={}, value={}]'.format(identifier_type, identifier_value))
+            Log.get().warning('Invalid user identifier [type={}, value={}]'.format(identifier_type, identifier_value))
         return self
 
-    def _is_valid(self, identifier_type, identifier_value):
-        if identifier_type is None:
-            return False
+    @staticmethod
+    def sanitize_value_or_none(identifier_value):
+        if identifier_value is None:
+            return None
 
-        if not isinstance(identifier_type, string_types):
-            return False
+        if hackle_types.is_not_empty_string(identifier_value) \
+                and len(identifier_value) <= IdentifiersBuilder.__MAX_IDENTIFIER_VALUE_LENGTH:
+            return identifier_value
 
-        if len(identifier_type) == 0:
-            return False
+        if hackle_types.is_finite_number(identifier_value):
+            return str(identifier_value)
 
-        if len(identifier_type) > 128:
-            return False
+        return None
 
-        if identifier_value is None:
+    def __is_value_type(self, identifier_type):
+        if identifier_type is None:
             return False
 
-        if not isinstance(identifier_value, string_types):
+        if not hackle_types.is_string(identifier_type):
             return False
 
-        if len(identifier_value) == 0:
+        if hackle_types.is_empty_string(identifier_type):
             return False
 
-        if len(identifier_value) > 512:
+        if len(identifier_type) > self.__MAX_IDENTIFIER_TYPE_LENGTH:
             return False
 
         return True
-
-    def build(self):
-        return self.identifiers
```

### Comparing `hackle-sdk-3.4.0/hackle/workspace.py` & `hackle-sdk-3.5.0/hackle/internal/workspace/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-from .entities import *
+from hackle.internal.model.entities import *
 
 
 class Workspace(object):
     def __init__(self, data):
         json_data = json.loads(data)
 
         self.bucket_id_map = self._bucket_id_map(json_data.get('buckets', []))
```

### Comparing `hackle-sdk-3.4.0/setup.py` & `hackle-sdk-3.5.0/setup.py`

 * *Files identical despite different names*

