# Comparing `tmp/prism-dev-0.1.1.tar.gz` & `tmp/prism-dev-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prism-dev-0.1.1.tar", last modified: Wed May 17 12:13:42 2023, max compression
+gzip compressed data, was "prism-dev-0.1.2.tar", last modified: Tue May 30 14:17:42 2023, max compression
```

## Comparing `prism-dev-0.1.1.tar` & `prism-dev-0.1.2.tar`

### file list

```diff
@@ -1,409 +1,440 @@
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.550318 prism-dev-0.1.1/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11312 2022-08-08 04:50:27.000000 prism-dev-0.1.1/LICENSE
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      219 2023-05-16 12:01:01.000000 prism-dev-0.1.1/MANIFEST.in
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5534 2023-05-17 12:13:42.550425 prism-dev-0.1.1/PKG-INFO
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4572 2023-05-16 12:50:41.000000 prism-dev-0.1.1/README.md
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.439597 prism-dev-0.1.1/prism/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:34:22.000000 prism-dev-0.1.1/prism/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/admin.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.444039 prism-dev-0.1.1/prism/agents/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/agents/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7778 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/agents/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    18475 2023-05-15 14:21:16.000000 prism-dev-0.1.1/prism/agents/docker_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    37139 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/agents/ec2.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      533 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/agents/meta.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.446648 prism-dev-0.1.1/prism/agents/scripts/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-16 12:00:13.000000 prism-dev-0.1.1/prism/agents/scripts/__init__.py
--rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)     3276 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/agents/scripts/apply.sh
--rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)      680 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/agents/scripts/run.sh
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.449398 prism-dev-0.1.1/prism/cli/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/cli/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9886 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/cli/agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6974 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/cli/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6235 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/cli/compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4391 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/cli/connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4186 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/cli/create_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4548 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/cli/create_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4408 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/cli/create_trigger.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5415 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/cli/graph.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5452 2023-05-04 13:05:27.000000 prism-dev-0.1.1/prism/cli/init.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9372 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/cli/run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      724 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/cli/spark_submit.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.449660 prism-dev-0.1.1/prism/client/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    12158 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/client/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4973 2023-05-16 03:01:00.000000 prism-dev-0.1.1/prism/constants.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6480 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/decorators.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.449843 prism-dev-0.1.1/prism/docs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/docs/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.455189 prism-dev-0.1.1/prism/docs/build/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    50665 2023-03-25 19:27:00.000000 prism-dev-0.1.1/prism/docs/build/311ea03002abadcdcaba.png
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6035 2023-03-25 19:27:00.000000 prism-dev-0.1.1/prism/docs/build/54968a39190c43d592b9.svg
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15406 2023-03-25 19:27:00.000000 prism-dev-0.1.1/prism/docs/build/737ad70b3f2d3a9b5f6e.ico
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       86 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/docs/build/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4653 2023-03-25 19:27:00.000000 prism-dev-0.1.1/prism/docs/build/ce188596011a8fa32931.png
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)   560665 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/docs/build/index.html
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      961 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/docs/build/main.js.LICENSE.txt
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.455567 prism-dev-0.1.1/prism/event_managers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/event_managers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5985 2023-05-04 14:38:23.000000 prism-dev-0.1.1/prism/event_managers/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6544 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/exceptions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.460701 prism-dev-0.1.1/prism/infra/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/infra/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13452 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/infra/compiler.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    12699 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/infra/executor.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2395 2023-05-04 13:05:27.000000 prism-dev-0.1.1/prism/infra/hooks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2811 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/infra/manifest.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6433 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/infra/module.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3629 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/infra/pipeline.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    17123 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/infra/project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1673 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/infra/sys_path.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      719 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/infra/task_manager.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    21250 2023-05-15 14:21:16.000000 prism-dev-0.1.1/prism/logging.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    22073 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/main.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.463633 prism-dev-0.1.1/prism/mixins/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-dev-0.1.1/prism/mixins/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2405 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/mixins/agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2823 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/mixins/aws.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1124 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/mixins/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8170 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/mixins/compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7300 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/mixins/connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2306 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/mixins/create_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4713 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/mixins/create_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5422 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/mixins/create_trigger.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2438 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/mixins/graph.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1107 2023-04-02 17:52:18.000000 prism-dev-0.1.1/prism/mixins/run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4244 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/mixins/sys_handler.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.464283 prism-dev-0.1.1/prism/parsers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/parsers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15219 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/parsers/ast_parser.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2206 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/parsers/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3049 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/parsers/yml_parser.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.468775 prism-dev-0.1.1/prism/profiles/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/profiles/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2745 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/profiles/adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3611 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/profiles/bigquery.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15601 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/profiles/dbt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      539 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/profiles/meta.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4501 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/profiles/postgres.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9047 2023-05-04 13:05:27.000000 prism-dev-0.1.1/prism/profiles/profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4089 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/profiles/pyspark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4491 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/profiles/redshift.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4077 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/profiles/snowflake.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6292 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/profiles/trino.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.469581 prism-dev-0.1.1/prism/spark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/spark/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      439 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/spark/script.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2889 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/spark/wrapper.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1180 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4676 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.469788 prism-dev-0.1.1/prism/templates/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:55:51.000000 prism-dev-0.1.1/prism/templates/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.470267 prism-dev-0.1.1/prism/templates/agents/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       59 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/agents/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      233 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/agents/docker.yml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      191 2023-05-16 03:00:05.000000 prism-dev-0.1.1/prism/templates/agents/ec2.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.471219 prism-dev-0.1.1/prism/templates/minimal_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-16 12:31:03.000000 prism-dev-0.1.1/prism/templates/minimal_project/.gitignore
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/minimal_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.471419 prism-dev-0.1.1/prism/templates/minimal_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/minimal_project/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1323 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/minimal_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.471612 prism-dev-0.1.1/prism/templates/profile/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/profile/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.471858 prism-dev-0.1.1/prism/templates/profile/bigquery/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      153 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/bigquery/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.473508 prism-dev-0.1.1/prism/templates/profile/dbt/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/dbt/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.473803 prism-dev-0.1.1/prism/templates/profile/postgres/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/postgres/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.473996 prism-dev-0.1.1/prism/templates/profile/pyspark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      483 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/pyspark/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.474183 prism-dev-0.1.1/prism/templates/profile/redshift/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/redshift/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.474388 prism-dev-0.1.1/prism/templates/profile/snowflake/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/snowflake/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.474558 prism-dev-0.1.1/prism/templates/profile/trino/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      194 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/profile/trino/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.476260 prism-dev-0.1.1/prism/templates/starter_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/templates/starter_project/.gitignore
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/starter_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.477202 prism-dev-0.1.1/prism/templates/starter_project/data/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-dev-0.1.1/prism/templates/starter_project/data/.exists
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.477364 prism-dev-0.1.1/prism/templates/starter_project/dev/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      788 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/templates/starter_project/dev/dev.ipynb
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.477793 prism-dev-0.1.1/prism/templates/starter_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/starter_project/modules/module01.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.478036 prism-dev-0.1.1/prism/templates/starter_project/output/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-dev-0.1.1/prism/templates/starter_project/output/.exists
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1109 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/starter_project/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/starter_project/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.478577 prism-dev-0.1.1/prism/templates/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      430 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/tasks/pyspark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      430 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/tasks/python.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      155 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/tasks/sql.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.480730 prism-dev-0.1.1/prism/templates/triggers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/templates/triggers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      267 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/triggers/function.yml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      208 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/templates/triggers/prism_project.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.480899 prism-dev-0.1.1/prism/tests/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.487213 prism-dev-0.1.1/prism/tests/integration/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/integration/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7910 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/integration_test_class.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14197 2023-05-15 03:40:20.000000 prism-dev-0.1.1/prism/tests/integration/test_client.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7755 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10275 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4524 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_create.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4010 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_dbt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5729 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_hooks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4601 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_init.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.429699 prism-dev-0.1.1/prism/tests/integration/test_projects/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.494853 prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.495306 prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1117 2023-05-15 12:58:47.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.495883 prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.496119 prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1340 2023-05-15 12:58:47.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.499058 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/functions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.501910 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      835 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.504024 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.504573 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      888 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      921 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.504854 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.505342 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      917 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1035 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.506511 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.507160 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1031 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1152 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.508678 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.509702 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1104 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1264 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.510049 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.510957 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1790 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1176 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1051 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      622 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.511444 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.512697 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      973 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/csv.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1535 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1589 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1796 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/parquet.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      494 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/txt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.512984 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.513125 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.513527 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      576 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      583 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.513843 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.514127 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.514528 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1112 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.514734 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.515036 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.515237 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.515629 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1120 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.515819 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.516087 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.517173 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1242 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1245 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1188 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.521927 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.524749 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1359 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1090 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1838 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2154 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1080 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.525119 prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.526009 prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      347 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.526450 prism-dev-0.1.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.526621 prism-dev-0.1.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1153 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.527099 prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.527614 prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.529180 prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.529645 prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.530148 prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.530322 prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.530613 prism-dev-0.1.1/prism/tests/integration/test_projects/common/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/common/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      376 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_projects/common/functions.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    31080 2023-05-04 22:20:29.000000 prism-dev-0.1.1/prism/tests/integration/test_run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11844 2023-03-26 19:43:45.000000 prism-dev-0.1.1/prism/tests/integration/test_spark_submit.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5358 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/integration/test_targets.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.534336 prism-dev-0.1.1/prism/tests/unit/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/unit/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.534625 prism-dev-0.1.1/prism/tests/unit/dummy_modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/dummy_modules/dummy_module1.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13709 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_adapter_profile.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.534741 prism-dev-0.1.1/prism/tests/unit/test_agent/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1232 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_agent/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10137 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_agents.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    26210 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_dag_fns.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.534930 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       77 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.536177 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      224 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.539908 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      436 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module05.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module06.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module07.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module08.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module09.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module10.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module11.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module12.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module13.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module14.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module15.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.540691 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      134 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      183 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      210 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module03.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.541930 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.542968 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.544196 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      175 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleE.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      405 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/unit/test_import.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5017 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_jinja.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10636 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_module_parser.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.546809 prism-dev-0.1.1/prism/tests/unit/test_modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      143 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/bad_run_extra_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      127 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/bad_run_missing_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      135 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/bad_run_no_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/diff_import_structure.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/if_name_main.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      226 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/multiple_prism_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      120 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/no_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      121 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/no_run_func.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/one_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      199 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/other_classes.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      332 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/task_with_target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      345 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_modules/tasks_refs.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.548379 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/bad_trigger_key.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      915 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/multiple_profiles.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      879 2022-08-08 04:50:27.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/no_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      909 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/non_null_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      894 2023-03-01 23:08:44.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/null_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      998 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/triggers_normal.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7556 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8920 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_trigger.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.548728 prism-dev-0.1.1/prism/tests/unit/test_trigger_yml/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_trigger_yml/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-04-04 01:59:51.000000 prism-dev-0.1.1/prism/tests/unit/test_trigger_yml/test_fn.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.548895 prism-dev-0.1.1/prism/triggers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19434 2023-05-04 14:37:27.000000 prism-dev-0.1.1/prism/triggers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      810 2023-05-04 14:39:42.000000 prism-dev-0.1.1/prism/ui.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-17 12:13:42.550204 prism-dev-0.1.1/prism_dev.egg-info/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5534 2023-05-17 12:13:42.000000 prism-dev-0.1.1/prism_dev.egg-info/PKG-INFO
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15970 2023-05-17 12:13:42.000000 prism-dev-0.1.1/prism_dev.egg-info/SOURCES.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-05-17 12:13:42.000000 prism-dev-0.1.1/prism_dev.egg-info/dependency_links.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       42 2023-05-17 12:13:42.000000 prism-dev-0.1.1/prism_dev.egg-info/entry_points.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-05-05 11:34:30.000000 prism-dev-0.1.1/prism_dev.egg-info/not-zip-safe
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      553 2023-05-17 12:13:42.000000 prism-dev-0.1.1/prism_dev.egg-info/requires.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       15 2023-05-17 12:13:42.000000 prism-dev-0.1.1/prism_dev.egg-info/top_level.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      743 2022-11-12 14:33:04.000000 prism-dev-0.1.1/pyproject.toml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1753 2023-05-17 12:13:42.550827 prism-dev-0.1.1/setup.cfg
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       70 2023-05-04 13:05:27.000000 prism-dev-0.1.1/setup.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.915129 prism-dev-0.1.2/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11312 2022-08-08 04:50:27.000000 prism-dev-0.1.2/LICENSE
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      219 2023-05-16 12:01:01.000000 prism-dev-0.1.2/MANIFEST.in
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5534 2023-05-30 14:17:42.915227 prism-dev-0.1.2/PKG-INFO
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4572 2023-05-16 12:50:41.000000 prism-dev-0.1.2/README.md
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.823563 prism-dev-0.1.2/prism/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:34:22.000000 prism-dev-0.1.2/prism/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/admin.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.825376 prism-dev-0.1.2/prism/agents/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/agents/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7778 2023-05-15 03:40:20.000000 prism-dev-0.1.2/prism/agents/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    18475 2023-05-15 14:21:16.000000 prism-dev-0.1.2/prism/agents/docker_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    37114 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/agents/ec2.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      533 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/agents/meta.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.826158 prism-dev-0.1.2/prism/agents/scripts/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-16 12:00:13.000000 prism-dev-0.1.2/prism/agents/scripts/__init__.py
+-rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)     3276 2023-05-15 03:40:20.000000 prism-dev-0.1.2/prism/agents/scripts/apply.sh
+-rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)      680 2023-05-15 03:40:20.000000 prism-dev-0.1.2/prism/agents/scripts/run.sh
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.830491 prism-dev-0.1.2/prism/cli/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/cli/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9886 2023-05-15 03:40:20.000000 prism-dev-0.1.2/prism/cli/agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6974 2023-04-02 17:52:18.000000 prism-dev-0.1.2/prism/cli/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6235 2023-04-02 17:52:18.000000 prism-dev-0.1.2/prism/cli/compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4391 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/cli/connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4186 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/cli/create_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4805 2023-05-27 16:07:03.000000 prism-dev-0.1.2/prism/cli/create_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4408 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/cli/create_trigger.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5415 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/cli/graph.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5452 2023-05-04 13:05:27.000000 prism-dev-0.1.2/prism/cli/init.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9372 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/cli/run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      724 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/cli/spark_submit.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.830759 prism-dev-0.1.2/prism/client/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    12158 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/client/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4973 2023-05-26 22:34:14.000000 prism-dev-0.1.2/prism/constants.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.832759 prism-dev-0.1.2/prism/decorators/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/decorators/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7124 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/decorators/target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3116 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/decorators/task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.832924 prism-dev-0.1.2/prism/docs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/docs/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.837485 prism-dev-0.1.2/prism/docs/build/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    50665 2023-03-25 19:27:00.000000 prism-dev-0.1.2/prism/docs/build/311ea03002abadcdcaba.png
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6035 2023-03-25 19:27:00.000000 prism-dev-0.1.2/prism/docs/build/54968a39190c43d592b9.svg
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15406 2023-03-25 19:27:00.000000 prism-dev-0.1.2/prism/docs/build/737ad70b3f2d3a9b5f6e.ico
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       86 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/docs/build/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4653 2023-03-25 19:27:00.000000 prism-dev-0.1.2/prism/docs/build/ce188596011a8fa32931.png
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)   560665 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/docs/build/index.html
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      961 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/docs/build/main.js.LICENSE.txt
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.837837 prism-dev-0.1.2/prism/event_managers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/event_managers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5985 2023-05-04 14:38:23.000000 prism-dev-0.1.2/prism/event_managers/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7320 2023-05-27 16:07:03.000000 prism-dev-0.1.2/prism/exceptions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.840243 prism-dev-0.1.2/prism/infra/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/infra/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13452 2023-04-02 17:52:18.000000 prism-dev-0.1.2/prism/infra/compiler.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13001 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/infra/executor.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2395 2023-05-04 13:05:27.000000 prism-dev-0.1.2/prism/infra/hooks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2811 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/infra/manifest.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7801 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/infra/module.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3629 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/infra/pipeline.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    17123 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/infra/project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1673 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/infra/sys_path.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      719 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/infra/task_manager.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    21250 2023-05-15 14:21:16.000000 prism-dev-0.1.2/prism/logging.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    22347 2023-05-27 16:07:03.000000 prism-dev-0.1.2/prism/main.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.843855 prism-dev-0.1.2/prism/mixins/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-dev-0.1.2/prism/mixins/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2405 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/mixins/agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2823 2023-05-15 03:40:20.000000 prism-dev-0.1.2/prism/mixins/aws.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1124 2023-04-02 17:52:18.000000 prism-dev-0.1.2/prism/mixins/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8170 2023-04-02 17:52:18.000000 prism-dev-0.1.2/prism/mixins/compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7295 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/mixins/connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2306 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/mixins/create_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5710 2023-05-27 16:07:03.000000 prism-dev-0.1.2/prism/mixins/create_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5422 2023-05-15 03:40:20.000000 prism-dev-0.1.2/prism/mixins/create_trigger.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2438 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/mixins/graph.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1107 2023-04-02 17:52:18.000000 prism-dev-0.1.2/prism/mixins/run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4244 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/mixins/sys_handler.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.845615 prism-dev-0.1.2/prism/parsers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/parsers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    23861 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/parsers/ast_parser.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2206 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/parsers/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3049 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/parsers/yml_parser.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.848972 prism-dev-0.1.2/prism/profiles/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/profiles/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2745 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/profiles/adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3611 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/profiles/bigquery.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15601 2023-05-15 03:40:20.000000 prism-dev-0.1.2/prism/profiles/dbt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      539 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/profiles/meta.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4501 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/profiles/postgres.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9047 2023-05-04 13:05:27.000000 prism-dev-0.1.2/prism/profiles/profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4089 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/profiles/pyspark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4491 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/profiles/redshift.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4077 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/profiles/snowflake.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6292 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/profiles/trino.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.849509 prism-dev-0.1.2/prism/spark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/spark/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      439 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/spark/script.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2889 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/spark/wrapper.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1582 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5145 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.850304 prism-dev-0.1.2/prism/templates/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:55:51.000000 prism-dev-0.1.2/prism/templates/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.851943 prism-dev-0.1.2/prism/templates/agents/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       59 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/templates/agents/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      233 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/templates/agents/docker.yml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      191 2023-05-20 15:36:38.000000 prism-dev-0.1.2/prism/templates/agents/ec2.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.852545 prism-dev-0.1.2/prism/templates/minimal_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-16 12:31:03.000000 prism-dev-0.1.2/prism/templates/minimal_project/.gitignore
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/templates/minimal_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.853797 prism-dev-0.1.2/prism/templates/minimal_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-05-30 01:38:51.000000 prism-dev-0.1.2/prism/templates/minimal_project/modules/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-05-30 01:39:48.000000 prism-dev-0.1.2/prism/templates/minimal_project/modules/decorated_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1328 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/templates/minimal_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.854112 prism-dev-0.1.2/prism/templates/profile/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/templates/profile/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.854285 prism-dev-0.1.2/prism/templates/profile/bigquery/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/templates/profile/bigquery/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.854459 prism-dev-0.1.2/prism/templates/profile/dbt/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      141 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/templates/profile/dbt/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.854637 prism-dev-0.1.2/prism/templates/profile/postgres/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/templates/profile/postgres/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.854823 prism-dev-0.1.2/prism/templates/profile/pyspark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      478 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/templates/profile/pyspark/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.855001 prism-dev-0.1.2/prism/templates/profile/redshift/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/templates/profile/redshift/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.855227 prism-dev-0.1.2/prism/templates/profile/snowflake/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      193 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/templates/profile/snowflake/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.855403 prism-dev-0.1.2/prism/templates/profile/trino/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      189 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/templates/profile/trino/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.857595 prism-dev-0.1.2/prism/templates/starter_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/templates/starter_project/.gitignore
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/templates/starter_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.857865 prism-dev-0.1.2/prism/templates/starter_project/data/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-dev-0.1.2/prism/templates/starter_project/data/.exists
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.857967 prism-dev-0.1.2/prism/templates/starter_project/dev/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      788 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/templates/starter_project/dev/dev.ipynb
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.859766 prism-dev-0.1.2/prism/templates/starter_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-05-30 01:39:55.000000 prism-dev-0.1.2/prism/templates/starter_project/modules/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-05-30 01:39:55.000000 prism-dev-0.1.2/prism/templates/starter_project/modules/decorated_task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.860043 prism-dev-0.1.2/prism/templates/starter_project/output/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-dev-0.1.2/prism/templates/starter_project/output/.exists
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1114 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/templates/starter_project/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/templates/starter_project/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.861496 prism-dev-0.1.2/prism/templates/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-dev-0.1.2/prism/templates/tasks/pyspark_cls.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-dev-0.1.2/prism/templates/tasks/pyspark_dec.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-dev-0.1.2/prism/templates/tasks/python_cls.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-dev-0.1.2/prism/templates/tasks/python_dec.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      155 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/templates/tasks/sql.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.862278 prism-dev-0.1.2/prism/templates/triggers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/templates/triggers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      267 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/templates/triggers/function.yml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      208 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/templates/triggers/prism_project.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.862456 prism-dev-0.1.2/prism/tests/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/tests/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.866663 prism-dev-0.1.2/prism/tests/integration/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/tests/integration/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7910 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/integration_test_class.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14197 2023-05-15 03:40:20.000000 prism-dev-0.1.2/prism/tests/integration/test_client.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7755 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10260 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/integration/test_connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6520 2023-05-27 16:07:03.000000 prism-dev-0.1.2/prism/tests/integration/test_create.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4010 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_dbt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5729 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_hooks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4539 2023-05-30 01:42:39.000000 prism-dev-0.1.2/prism/tests/integration/test_init.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.817488 prism-dev-0.1.2/prism/tests/integration/test_projects/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.869148 prism-dev-0.1.2/prism/tests/integration/test_projects/001_init/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/001_init/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.869487 prism-dev-0.1.2/prism/tests/integration/test_projects/001_init/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/001_init/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1122 2023-05-27 15:46:27.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/001_init/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/001_init/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.871024 prism-dev-0.1.2/prism/tests/integration/test_projects/001a_init_minimal/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/001a_init_minimal/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.871346 prism-dev-0.1.2/prism/tests/integration/test_projects/001a_init_minimal/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1008 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/001a_init_minimal/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1345 2023-05-27 15:46:27.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.871790 prism-dev-0.1.2/prism/tests/integration/test_projects/002_no_project_py/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/002_no_project_py/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/002_no_project_py/functions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.872617 prism-dev-0.1.2/prism/tests/integration/test_projects/002_no_project_py/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      835 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      867 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.872933 prism-dev-0.1.2/prism/tests/integration/test_projects/003_project_with_cycle/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/003_project_with_cycle/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.873592 prism-dev-0.1.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      888 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      921 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.873893 prism-dev-0.1.2/prism/tests/integration/test_projects/004_simple_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/004_simple_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.874425 prism-dev-0.1.2/prism/tests/integration/test_projects/004_simple_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/004_simple_project/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/004_simple_project/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      917 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/004_simple_project/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1035 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/004_simple_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.875052 prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.875773 prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1031 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1152 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.876064 prism-dev-0.1.2/prism/tests/integration/test_projects/006_simple_project_with_profile/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/006_simple_project_with_profile/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.876973 prism-dev-0.1.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1104 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      986 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1259 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.877335 prism-dev-0.1.2/prism/tests/integration/test_projects/007_spark_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/007_spark_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.878037 prism-dev-0.1.2/prism/tests/integration/test_projects/007_spark_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1790 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/007_spark_project/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1176 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/007_spark_project/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1051 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/007_spark_project/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      622 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/007_spark_project/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/007_spark_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.878414 prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.879404 prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      973 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/modules/csv.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1535 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1589 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1796 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/modules/parquet.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      494 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/modules/txt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.879595 prism-dev-0.1.2/prism/tests/integration/test_projects/009_simple_dbt_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/009_simple_dbt_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.879710 prism-dev-0.1.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.880100 prism-dev-0.1.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      576 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      583 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.880383 prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.880662 prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.881008 prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1112 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.881194 prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.881466 prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.881637 prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.881992 prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1120 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.882189 prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      994 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.882456 prism-dev-0.1.2/prism/tests/integration/test_projects/012_concurrency/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/012_concurrency/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.883353 prism-dev-0.1.2/prism/tests/integration/test_projects/012_concurrency/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1242 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/012_concurrency/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1245 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/012_concurrency/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1188 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/012_concurrency/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      922 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/012_concurrency/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/012_concurrency/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.883645 prism-dev-0.1.2/prism/tests/integration/test_projects/013_hooks_sql_spark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/013_hooks_sql_spark/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.884348 prism-dev-0.1.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1359 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1090 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1838 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2154 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1075 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.884622 prism-dev-0.1.2/prism/tests/integration/test_projects/014_test_triggers_normal/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/014_test_triggers_normal/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.885156 prism-dev-0.1.2/prism/tests/integration/test_projects/014_test_triggers_normal/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      347 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/014_test_triggers_normal/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.885542 prism-dev-0.1.2/prism/tests/integration/test_projects/015_test_triggers_no_dir/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/015_test_triggers_no_dir/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.885783 prism-dev-0.1.2/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      362 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/015_test_triggers_no_dir/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1153 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.886335 prism-dev-0.1.2/prism/tests/integration/test_projects/016_test_triggers_error/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/016_test_triggers_error/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.886516 prism-dev-0.1.2/prism/tests/integration/test_projects/016_test_triggers_error/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/016_test_triggers_error/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.886966 prism-dev-0.1.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.887192 prism-dev-0.1.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.887690 prism-dev-0.1.2/prism/tests/integration/test_projects/018_test_triggers_no_include/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/018_test_triggers_no_include/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.887866 prism-dev-0.1.2/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      930 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/018_test_triggers_no_include/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.888145 prism-dev-0.1.2/prism/tests/integration/test_projects/019_dec_targets/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/019_dec_targets/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.888627 prism-dev-0.1.2/prism/tests/integration/test_projects/019_dec_targets/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      578 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/019_dec_targets/modules/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      620 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/019_dec_targets/modules/load.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/019_dec_targets/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.889213 prism-dev-0.1.2/prism/tests/integration/test_projects/020_dec_retries/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/020_dec_retries/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.889603 prism-dev-0.1.2/prism/tests/integration/test_projects/020_dec_retries/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      399 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/020_dec_retries/modules/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      703 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/020_dec_retries/modules/load.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1213 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/020_dec_retries/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/020_dec_retries/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.889930 prism-dev-0.1.2/prism/tests/integration/test_projects/common/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/common/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      376 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_projects/common/functions.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    36004 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/integration/test_run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11844 2023-03-26 19:43:45.000000 prism-dev-0.1.2/prism/tests/integration/test_spark_submit.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5358 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/integration/test_targets.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.892737 prism-dev-0.1.2/prism/tests/unit/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/tests/unit/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.893131 prism-dev-0.1.2/prism/tests/unit/dummy_modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/unit/dummy_modules/dummy_module1.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13709 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/unit/test_adapter_profile.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.893286 prism-dev-0.1.2/prism/tests/unit/test_agent/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1232 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/unit/test_agent/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10137 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/unit/test_agents.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    26210 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_dag_fns.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.893483 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       77 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.894691 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/dag_cycle/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/dag_cycle/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      224 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.897817 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      436 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module05.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module06.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module07.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module08.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module09.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module10.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module11.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module12.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module13.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module14.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/module15.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.898975 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      134 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      183 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      211 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      210 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/module03.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.902903 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      250 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.904173 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.905129 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      175 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      171 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleE.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      405 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/tests/unit/test_import.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4992 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/unit/test_jinja.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10289 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/unit/test_module_parser_cls.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9472 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/unit/test_module_parser_dec.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.911744 prism-dev-0.1.2/prism/tests/unit/test_modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      143 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/bad_run_extra_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      127 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/bad_run_missing_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      135 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/bad_run_no_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       92 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/dec_bad_dec_no_parentheses.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      105 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/dec_bad_run_extra_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       87 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/dec_bad_run_missing_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      124 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/dec_diff_decorator_structure.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      156 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/dec_multiple_prism_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       49 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/dec_no_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       93 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/dec_one_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/dec_other_functions.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      301 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/dec_task_with_target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      451 2023-05-26 22:30:47.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/dec_tasks_refs.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/diff_import_structure.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/if_name_main.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      226 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/multiple_prism_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      120 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/no_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      121 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/no_run_func.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/one_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      199 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/other_classes.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      332 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/task_with_target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      345 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_modules/tasks_refs.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.913212 prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/bad_trigger_key.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      915 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/multiple_profiles.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      879 2022-08-08 04:50:27.000000 prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/no_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      909 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/non_null_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      894 2023-03-01 23:08:44.000000 prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/null_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1002 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      998 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/triggers_normal.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7556 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/unit/test_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8920 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/unit/test_trigger.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.913537 prism-dev-0.1.2/prism/tests/unit/test_trigger_yml/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      931 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/unit/test_trigger_yml/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-04-04 01:59:51.000000 prism-dev-0.1.2/prism/tests/unit/test_trigger_yml/test_fn.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.913688 prism-dev-0.1.2/prism/triggers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19434 2023-05-04 14:37:27.000000 prism-dev-0.1.2/prism/triggers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      810 2023-05-04 14:39:42.000000 prism-dev-0.1.2/prism/ui.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-05-30 14:17:42.915017 prism-dev-0.1.2/prism_dev.egg-info/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5534 2023-05-30 14:17:42.000000 prism-dev-0.1.2/prism_dev.egg-info/PKG-INFO
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    17452 2023-05-30 14:17:42.000000 prism-dev-0.1.2/prism_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-05-30 14:17:42.000000 prism-dev-0.1.2/prism_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       42 2023-05-30 14:17:42.000000 prism-dev-0.1.2/prism_dev.egg-info/entry_points.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-05-05 11:34:30.000000 prism-dev-0.1.2/prism_dev.egg-info/not-zip-safe
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      553 2023-05-30 14:17:42.000000 prism-dev-0.1.2/prism_dev.egg-info/requires.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       15 2023-05-30 14:17:42.000000 prism-dev-0.1.2/prism_dev.egg-info/top_level.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      743 2022-11-12 14:33:04.000000 prism-dev-0.1.2/pyproject.toml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1753 2023-05-30 14:17:42.915619 prism-dev-0.1.2/setup.cfg
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       70 2023-05-04 13:05:27.000000 prism-dev-0.1.2/setup.py
```

### Comparing `prism-dev-0.1.1/LICENSE` & `prism-dev-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/PKG-INFO` & `prism-dev-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prism-dev
-Version: 0.1.1
+Version: 0.1.2
 Summary: The easiest way to create data pipelines in Python.
 Author: prism founders
 Author-email: hello@runprism.com
 License: Apache-2.0
 Project-URL: homepage, https://www.runprism.com
 Project-URL: documentation, https://docs.runprism.com
 Project-URL: repository, https://github.com/runprism/prism
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prism-dev Version: 0.1.1 Summary: The easiest way
+Metadata-Version: 2.1 Name: prism-dev Version: 0.1.2 Summary: The easiest way
 to create data pipelines in Python. Author: prism founders Author-email:
 hello@runprism.com License: Apache-2.0 Project-URL: homepage, https://
 www.runprism.com Project-URL: documentation, https://docs.runprism.com Project-
 URL: repository, https://github.com/runprism/prism Platform: unix Platform:
 linux Platform: osx Platform: win32 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `prism-dev-0.1.1/README.md` & `prism-dev-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/admin.py` & `prism-dev-0.1.2/prism/admin.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/agents/base.py` & `prism-dev-0.1.2/prism/agents/base.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/agents/docker_agent.py` & `prism-dev-0.1.2/prism/agents/docker_agent.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/agents/ec2.py` & `prism-dev-0.1.2/prism/agents/ec2.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,14 @@
         """
         required_keys = {
             "type": str,
             "instance_type": str,
             "requirements": str,
         }
         optional_keys = {
-            "user": str,
             "env": dict
         }
 
         return self.check_conf_keys(
             agent_conf,
             required_keys,
             optional_keys
```

### Comparing `prism-dev-0.1.1/prism/agents/meta.py` & `prism-dev-0.1.2/prism/agents/meta.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/agents/scripts/apply.sh` & `prism-dev-0.1.2/prism/agents/scripts/apply.sh`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/agents/scripts/run.sh` & `prism-dev-0.1.2/prism/agents/scripts/run.sh`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/cli/agent.py` & `prism-dev-0.1.2/prism/cli/agent.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/cli/base.py` & `prism-dev-0.1.2/prism/cli/base.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/cli/compile.py` & `prism-dev-0.1.2/prism/cli/compile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/cli/connect.py` & `prism-dev-0.1.2/prism/cli/connect.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/cli/create_agent.py` & `prism-dev-0.1.2/prism/cli/create_agent.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/cli/create_task.py` & `prism-dev-0.1.2/prism/cli/create_task.py`

 * *Files 15% similar despite different names*

```diff
@@ -53,29 +53,35 @@
         event_list = task_return_result.event_list
         event_list = fire_empty_line_event(event_list)
 
         # ------------------------------------------------------------------------------
         # Define task type, task number, and task name
 
         task_type = self.args.type
+        decorated = self.args.decorated
 
         # If adapter type is None, throw an error
         if task_type is None:
             e = prism.logging.InvalidType(
                 "task",
                 prism.constants.VALID_TASK_TYPES
             )
             event_list = fire_console_event(e, event_list, 0, log_level='error')
             event_list = self.fire_tail_event(event_list)
             return prism.cli.base.TaskRunReturnResult(event_list)
 
         # Grab the template
-        template_module = importlib.import_module(
-            name=f"prism.templates.tasks.{task_type}"
-        )
+        if decorated:
+            template_module = importlib.import_module(
+                name=f"prism.templates.tasks.{task_type}_dec"
+            )
+        else:
+            template_module = importlib.import_module(
+                name=f"prism.templates.tasks.{task_type}_cls"
+            )
         template = template_module.TEMPLATE
         task_template = Environment(loader=BaseLoader).from_string(template)  # type: ignore # noqa: E501
 
         # Get the number of tasks to create and the task name
         task_number = self.args.number
         user_task_name = self.args.name
 
@@ -108,15 +114,16 @@
         task_manager_output: EventManagerOutput = task_manager.manage_events_during_run(
             event_list=event_list,
             fire_exec_events=False,
             task_number=task_number,
             task_type=task_type,
             user_task_name=user_task_name,
             task_template=task_template,
-            task_dir=task_dir
+            task_dir=task_dir,
+            decorated=decorated,
         )
         output = task_manager_output.outputs
         event_to_fire = task_manager_output.event_to_fire
         event_list = task_manager_output.event_list
         if output == 0:
             event_list = fire_console_event(
                 event_to_fire,
```

### Comparing `prism-dev-0.1.1/prism/cli/create_trigger.py` & `prism-dev-0.1.2/prism/cli/create_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/cli/graph.py` & `prism-dev-0.1.2/prism/cli/graph.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/cli/init.py` & `prism-dev-0.1.2/prism/cli/init.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/cli/run.py` & `prism-dev-0.1.2/prism/cli/run.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/cli/spark_submit.py` & `prism-dev-0.1.2/prism/cli/spark_submit.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/client/__init__.py` & `prism-dev-0.1.2/prism/client/__init__.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/constants.py` & `prism-dev-0.1.2/prism/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 #############
 # Constants #
 #############
 
 # Version number
-VERSION = '0.1.9rc1'
+VERSION = '0.1.9rc2'
 
 # Root directory of project
 ROOT_DIR = str(Path(os.path.dirname(__file__)).parent)
 
 # Files to ignore when instantiating Prism project
 IGNORE_FILES = ["__pycache__", '*checkpoint.ipynb', '.ipynb_checkpoints']
```

### Comparing `prism-dev-0.1.1/prism/decorators.py` & `prism-dev-0.1.2/prism/decorators/target.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,68 +14,79 @@
 from pathlib import Path
 
 # Prism imports
 import prism.exceptions
 from prism.task import PrismTask
 import prism.infra.hooks
 import prism.infra.task_manager
+import inspect
 
 
 #####################
 # Target decorators #
 #####################
 
 def target(*, type, loc, **kwargs):
     """
     Decorator to use if user wishes to save the output of a task to an external location
     (e.g., a data warehouse, an S3 bucket, or a local filepath).
     """
 
     def decorator_target(func):
 
-        def wrapper_target(self,
+        def wrapper_target_dec(self,
             task_manager: prism.infra.task_manager.PrismTaskManager,
             hooks: prism.infra.hooks.PrismHooks
         ):
 
             # This will only ever be called inside a PrismTask
             if not isinstance(self, PrismTask):
                 raise prism.exceptions.RuntimeException(
                     message="`target` decorator can only be called within a Prism task"
                 )
 
             # In cases with multiple decorators, we don't want to "chain" the
             # decorators. Rather, we want each target declaration to apply to each
             # object returned. In this case, keep track of the target types, locs, and
             # kwargs.
-            if func.__name__ == "wrapper_target":
+            if func.__name__ == "wrapper_target_dec":
                 self.types.append(type)
                 self.locs.append(loc)
                 try:
                     self.kwargs.append(kwargs)
                 except TypeError:
                     self.kwargs.append({})
 
                 # Return the next wrapper_target function with the same arguments as
                 # this one. If a function has `n` targets, then this will happen n-1
                 # times until the `run` function is reached.
-                return func(self, task_manager, hooks)
+                if not inspect.ismethod(func):
+                    return func(self, task_manager, hooks)
+                else:
+                    return func(task_manager, hooks)
 
             # Now, we've hit the `run` function
             else:
 
                 # Confirm function name
                 if func.__name__ != "run":
                     raise prism.exceptions.RuntimeException(
                         message="`target` decorator can only be called on `run` function"  # noqa: E501
                     )
 
                 # If the task should be run in full, then call the run function
                 if self.bool_run:
-                    obj = func(self, task_manager, hooks)
+
+                    # When using `target` as a decorator, `run` is a function. When
+                    # using `target` as an argument to the `task()` decorator, `run` is
+                    # a bound method.
+                    if not inspect.ismethod(func):
+                        obj = func(self, task_manager, hooks)
+                    else:
+                        obj = func(task_manager, hooks)
                     self.types.append(type)
                     self.locs.append(loc)
                     try:
                         self.kwargs.append(kwargs)
                     except TypeError:
                         self.kwargs.append({})
 
@@ -83,15 +94,15 @@
                     if isinstance(obj, tuple):
                         objects_to_save = zip(obj, self.types, self.locs, self.kwargs)
                         for zipped in objects_to_save:
                             temp_o = zipped[0]
                             temp_t = zipped[1]
                             temp_l = zipped[2]
                             temp_k = zipped[3]
-                            target = temp_t(temp_o, temp_l, hooks)
+                            target = temp_t(temp_o, temp_l, hooks)  # type: ignore
                             target.save(**temp_k)
 
                         # If a target is set, just assume that the user wants to
                         # reference the location of the target when they call `mod`
                         return self.locs
 
                     # If return type is not a Tuple, we expect a single target
@@ -115,15 +126,16 @@
                     # If multiple targets, then return all locs
                     if len(self.locs) > 1:
                         return self.locs
 
                     # For single-target case, return single loc
                     else:
                         return loc
-        return wrapper_target
+
+        return wrapper_target_dec
 
     return decorator_target
 
 
 def target_iterator(*, type, loc, **kwargs):
     """
     Decorator to use if task requires user to iterate through several different objects
@@ -146,15 +158,18 @@
             # Confirm function name
             if func.__name__ != "run":
                 raise prism.exceptions.RuntimeException(
                     message="`target iterator` decorator can only be called on `run` function"  # noqa: E501
                 )
 
             if self.bool_run:
-                objs = func(self, task_manager, hooks)
+                if not inspect.ismethod(func):
+                    objs = func(self, task_manager, hooks)
+                else:
+                    objs = func(task_manager, hooks)
                 if not isinstance(objs, dict):
                     raise prism.exceptions.RuntimeException(
                         message="output of run function should be dict mapping name --> object to save"  # noqa: E501
                     )
                 for k, _ in objs.items():
                     if not isinstance(k, str):
                         raise prism.exceptions.RuntimeException(
```

### Comparing `prism-dev-0.1.1/prism/docs/build/311ea03002abadcdcaba.png` & `prism-dev-0.1.2/prism/docs/build/311ea03002abadcdcaba.png`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/docs/build/54968a39190c43d592b9.svg` & `prism-dev-0.1.2/prism/docs/build/54968a39190c43d592b9.svg`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/docs/build/737ad70b3f2d3a9b5f6e.ico` & `prism-dev-0.1.2/prism/docs/build/737ad70b3f2d3a9b5f6e.ico`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/docs/build/ce188596011a8fa32931.png` & `prism-dev-0.1.2/prism/docs/build/ce188596011a8fa32931.png`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/docs/build/index.html` & `prism-dev-0.1.2/prism/docs/build/index.html`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/docs/build/main.js.LICENSE.txt` & `prism-dev-0.1.2/prism/docs/build/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/event_managers/base.py` & `prism-dev-0.1.2/prism/event_managers/base.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/exceptions.py` & `prism-dev-0.1.2/prism/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,7 +302,33 @@
 
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
 
     def __str__(self):
         return self.message
+
+
+class UnsupportedTaskTypeException(PrismException):
+    """
+    Exception raised when an unsupported task is requested
+    """
+
+    def __init__(self, task_type):
+        self.message = f"{task_type} tasks aren't currently supported by Prism...be patient, we're working on it! :)"  # noqa: E501
+        super().__init__(self.message)
+
+    def __str__(self):
+        return self.message
+
+
+class InvalidTaskNameException(PrismException):
+    """
+    Exception raised when an unsupported task is requested
+    """
+
+    def __init__(self, task_name):
+        self.message = f"invalid task name `{task_name}`...task names should only have lowercase letters and underscores"  # noqa: E501
+        super().__init__(self.message)
+
+    def __str__(self):
+        return self.message
```

### Comparing `prism-dev-0.1.1/prism/infra/compiler.py` & `prism-dev-0.1.2/prism/infra/compiler.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/infra/executor.py` & `prism-dev-0.1.2/prism/infra/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,18 @@
 
         # Execute the module with appropriate number of retries
         retries, retry_delay_seconds = module.grab_retries_metadata()
         num_runs = 0
         num_expected_runs = retries + 1
         outputs = 0
         name = module.name
+
+        # For testing, keep track of all events
+        all_events = []
+
         while num_runs != num_expected_runs and outputs == 0:
             num_runs += 1
             if num_runs > 1:
                 event_list = fire_console_event(
                     prism.logging.DelayEvent(name, retry_delay_seconds),
                     log_level='warn'
                 )
@@ -193,16 +197,23 @@
                 fire_empty_line_events,
                 run_context=self.run_context,
                 task_manager=task_manager,
                 hooks=hooks,
                 explicit_run=relative_path not in self.nodes_not_explicitly_run,
                 user_context=user_context
             )
+
+            # All events
+            all_events += script_event_manager_result.event_list
+
+            # Set output
             outputs = script_event_manager_result.outputs
 
+        # Now, update the event list of the output
+        script_event_manager_result.event_list = all_events
         return script_event_manager_result
 
     def _cancel_connections(self, pool):
         """
         Given a pool, cancel all adapter connections and wait until all
         runners gentle terminates.
         """
```

### Comparing `prism-dev-0.1.1/prism/infra/hooks.py` & `prism-dev-0.1.2/prism/infra/hooks.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/infra/manifest.py` & `prism-dev-0.1.2/prism/infra/manifest.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/infra/pipeline.py` & `prism-dev-0.1.2/prism/infra/pipeline.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/infra/project.py` & `prism-dev-0.1.2/prism/infra/project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/infra/sys_path.py` & `prism-dev-0.1.2/prism/infra/sys_path.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/infra/task_manager.py` & `prism-dev-0.1.2/prism/infra/task_manager.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/logging.py` & `prism-dev-0.1.2/prism/logging.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/main.py` & `prism-dev-0.1.2/prism/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,14 +347,23 @@
         required=False,
         default="python",
         help=f"""
         Task type. One of {valid_tasks_str}. Default is `python`
         """
     )
 
+    # Add argument for whether the task should be a decorated function or a full class.
+    subcommand_options.add_argument(
+        '--decorated',
+        action='store_true',
+        help="""
+        If specified, the task will be a decorated function.
+        """
+    )
+
     # Add argument for number of tasks to create
     subcommand_options.add_argument(
         '-n',
         '--number',
         type=int,
         required=False,
         metavar="N",
```

### Comparing `prism-dev-0.1.1/prism/mixins/agent.py` & `prism-dev-0.1.2/prism/mixins/agent.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/mixins/aws.py` & `prism-dev-0.1.2/prism/mixins/aws.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/mixins/base.py` & `prism-dev-0.1.2/prism/mixins/base.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/mixins/compile.py` & `prism-dev-0.1.2/prism/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/mixins/connect.py` & `prism-dev-0.1.2/prism/mixins/connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
             base_yml = yaml.safe_load(f)
         f.close()
 
         template_path = Path(profiles_template_dir) / profile_type / 'profile.yml'
         with open(template_path, 'r') as f:
             template_yml = yaml.safe_load(f)
         f.close()
-        new_connection = template_yml['profile_name']
+        new_connection = template_yml['default']
 
         if profile_type in prism.constants.VALID_ADAPTERS:
             new_connection = new_connection['adapters']
         else:
             msg = f"new profile_type is invalid; must be one of `{prism.constants.VALID_ADAPTERS}`"  # noqa: E501
             raise prism.exceptions.InvalidProfileException(message=msg)
```

### Comparing `prism-dev-0.1.1/prism/mixins/create_agent.py` & `prism-dev-0.1.2/prism/mixins/create_agent.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/mixins/create_task.py` & `prism-dev-0.1.2/prism/mixins/create_task.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,54 +20,73 @@
 import prism.cli.compile
 import prism.exceptions
 import prism.constants
 import prism.logging
 
 # Other imports
 from jinja2 import Template
+import re
 
 
 ####################
 # Class definition #
 ####################
 
 class CreateTaskMixins:
     """
     Mixin for CreateTask task
     """
 
-    def user_task_name_to_classname(self,
+    def is_valid_user_task_name(self,
+        user_task_name: str
+    ):
+        """
+        Check if the user task name is valid. A user's task name should only have
+        letters and underscores.
+        """
+        if not bool(re.match(r'^[a-z\_]$', user_task_name)):
+            raise prism.exceptions.InvalidTaskNameException(user_task_name)
+        return True
+
+    def process_user_task_name(self,
         task_type: str,
         user_task_name: str,
+        decorated: bool = False
     ):
         f"""
         The user-inputted `task_name` corresponds to the file name for the new task. We
         want to use this same `task_name` to populate the class name associated with the
         new task.
 
         args:
             task_type: one of {','.join(prism.constants.VALID_TASK_TYPES)}
             user_task_name: user-inputted `task_name` argument
+            decorated: True if the task is a decorated function, False otherwise.
+                Defaults to False
         returns:
             class name
         """
         if task_type == "sql":
-            return ""
+            raise prism.exceptions.UnsupportedTaskTypeException(task_type)
 
         else:
-            # Convert to proper case
-            delim = "_"
-            new_sections = []
-            for name_section in user_task_name.split(delim):
-                new_sections.append(name_section[0].upper() + name_section[1:])
-            name_proper_case = delim.join(new_sections)
-
-            # Remove "_"
-            class_name = name_proper_case.replace("_", "")
-            return class_name
+            # If the user wishes to create a class task, then convert the inputted task
+            # name to proper case and remove the underscores.
+            if not decorated:
+                delim = "_"
+                new_sections = []
+                for name_section in user_task_name.split(delim):
+                    new_sections.append(name_section[0].upper() + name_section[1:])
+                name_proper_case = delim.join(new_sections)
+
+                # Remove "_"
+                class_name = name_proper_case.replace("_", "")
+                return class_name
+            else:
+                return user_task_name
 
     def create_task_module(self,
         task_type: str,
         task_template: Template,
         args: Dict[str, str],
         user_task_name: str,
         task_dir: Path,
@@ -111,32 +130,35 @@
 
     def create_tasks(self,
         task_number: int,
         task_type: str,
         user_task_name: str,
         task_template: Template,
         task_dir: Path,
+        decorated: bool = False
     ):
         f"""
         Create new tasks
 
         args:
             task_number: number of tasks to create
             task_type: one of {','.join(prism.constants.VALID_TASK_TYPES)}
             user_task_name: user-inputted task name
             task_template: unrendered Jinja2 template
             task_dir: directory to place new tasks in
+            decorated: True if the task is a decorated function, False otherwise.
+                Defaults to False
         returns:
             None
         """
         # Only one task is requested
         if task_number == 1:
             template_args = {
-                "task_cls_name": self.user_task_name_to_classname(
-                    task_type, user_task_name
+                "task_name": self.process_user_task_name(
+                    task_type, user_task_name, decorated
                 )
             }
             self.create_task_module(
                 task_type,
                 task_template,
                 template_args,
                 user_task_name,
@@ -144,18 +166,20 @@
             )
 
         # Multiple tasks are requested
         else:
             for i in range(1, task_number + 1):
 
                 # Add the task number to the class name and the user task name
-                cls_name = self.user_task_name_to_classname(task_type, user_task_name)
+                cls_name = self.process_user_task_name(
+                    task_type, user_task_name, decorated
+                )
                 cls_name += str(i)
                 template_args = {
-                    "task_cls_name": cls_name
+                    "task_name": cls_name
                 }
                 new_user_task_name = user_task_name + f"_{i}"
 
                 # Create task modules
                 self.create_task_module(
                     task_type,
                     task_template,
```

### Comparing `prism-dev-0.1.1/prism/mixins/create_trigger.py` & `prism-dev-0.1.2/prism/mixins/create_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/mixins/graph.py` & `prism-dev-0.1.2/prism/mixins/graph.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/mixins/run.py` & `prism-dev-0.1.2/prism/mixins/run.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/mixins/sys_handler.py` & `prism-dev-0.1.2/prism/mixins/sys_handler.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/parsers/base.py` & `prism-dev-0.1.2/prism/parsers/base.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/parsers/yml_parser.py` & `prism-dev-0.1.2/prism/parsers/yml_parser.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/profiles/adapter.py` & `prism-dev-0.1.2/prism/profiles/adapter.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/profiles/bigquery.py` & `prism-dev-0.1.2/prism/profiles/bigquery.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/profiles/dbt.py` & `prism-dev-0.1.2/prism/profiles/dbt.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/profiles/meta.py` & `prism-dev-0.1.2/prism/profiles/meta.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/profiles/postgres.py` & `prism-dev-0.1.2/prism/profiles/postgres.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/profiles/profile.py` & `prism-dev-0.1.2/prism/profiles/profile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/profiles/pyspark.py` & `prism-dev-0.1.2/prism/profiles/pyspark.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/profiles/redshift.py` & `prism-dev-0.1.2/prism/profiles/redshift.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/profiles/snowflake.py` & `prism-dev-0.1.2/prism/profiles/snowflake.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/profiles/trino.py` & `prism-dev-0.1.2/prism/profiles/trino.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/spark/wrapper.py` & `prism-dev-0.1.2/prism/spark/wrapper.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/target.py` & `prism-dev-0.1.2/prism/target.py`

 * *Files 21% similar despite different names*

```diff
@@ -59,7 +59,26 @@
         f.close()
 
 
 class MatplotlibPNG(PrismTarget):
 
     def save(self, **kwargs):
         self.obj.savefig(self.loc, **kwargs)
+
+
+class JSON(PrismTarget):
+
+    def save(self, **kwargs):
+
+        # Imports
+        import json
+
+        # Check object type
+        if not isinstance(self.obj, dict):
+            raise ValueError(
+                "object must be a dictionary!"
+            )
+        json_object = json.dumps(self.obj, **kwargs)
+
+        # Write
+        with open(self.loc, "w") as f:
+            f.write(json_object)
```

### Comparing `prism-dev-0.1.1/prism/task.py` & `prism-dev-0.1.2/prism/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,39 +6,51 @@
 - Class definition
 """
 
 ###########
 # Imports #
 ###########
 
-import prism.exceptions
+# Standard library imports
+from pathlib import Path
+from typing import Any, Callable, List, Optional, Union
 
-# Prism logging
+# Prism imports
+import prism.exceptions
 import prism.logging
 import prism.infra.hooks
 import prism.infra.task_manager
+import prism.target
 
 
 ####################
 # Class definition #
 ####################
 
 class PrismTask:
 
-    def __init__(self, bool_run=True):
+    def __init__(self,
+        bool_run: bool = True,
+        func: Optional[Callable[..., Any]] = None
+    ):
         """
         Create an instance of the PrismTask. The class immediately calls the `run`
         function and assigns the result to the `output` attribute.
         """
         self.bool_run = bool_run
+        self.func = func
 
         # Tyeps, locs, and kwargs for target
-        self.types = []
-        self.locs = []
-        self.kwargs = []
+        self.types: List[prism.target.PrismTarget] = []
+        self.locs: List[Union[str, Path]] = []
+        self.kwargs: List[Any] = []
+
+        # Retries
+        self.RETRIES = 0
+        self.RETRY_DELAY_SECONDS = 0
 
     def set_task_manager(self, task_manager: prism.infra.task_manager.PrismTaskManager):
         self.task_manager = task_manager
 
     def set_hooks(self, hooks: prism.infra.hooks.PrismHooks):
         self.hooks = hooks
 
@@ -69,21 +81,24 @@
             if self.output is None:
                 raise prism.exceptions.RuntimeException(
                     "`run` method must produce a non-null output"
                 )
 
     def run(self,
         tasks: prism.infra.task_manager.PrismTaskManager,
-        hooks: prism.infra.hooks.PrismHooks
+        hooks: prism.infra.hooks.PrismHooks,
     ):
         """
         Run the task. The user should override this function definition when creating
         their own tasks.
         """
-        raise prism.exceptions.RuntimeException("`run` method not implemented")
+        if self.func is not None:
+            return self.func(tasks, hooks)
+        else:
+            raise prism.exceptions.RuntimeException("`run` method not implemented")
 
     @prism.logging.deprecated('prism.task.PrismTask.target', 'prism.decorators.target')
     def target(type, loc, **kwargs):
         """
         Decorator to use if task requires user to iterate through several different
         objects and save each object to an external location
         """
```

### Comparing `prism-dev-0.1.1/prism/templates/minimal_project/modules/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/001_init/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/templates/minimal_project/prism_project.py` & `prism-dev-0.1.2/prism/templates/minimal_project/prism_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 1
 
 
 # Profile directory and name
 PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
-PROFILE = None  # name of profile within `profiles.yml`
+PROFILE = "default"  # name of profile within `profiles.yml`
 
 
 # Logger
 PRISM_LOGGER = logging.getLogger("PRISM_LOGGER")
 
 
 # Triggers
```

### Comparing `prism-dev-0.1.1/prism/templates/starter_project/dev/dev.ipynb` & `prism-dev-0.1.2/prism/templates/starter_project/dev/dev.ipynb`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/templates/starter_project/modules/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/001a_init_minimal/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/templates/starter_project/prism_project.py` & `prism-dev-0.1.2/prism/templates/starter_project/prism_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 1
 
 
 # Profile directory and name
 PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
-PROFILE = None
+PROFILE = "default"
 
 
 # Logger
 PRISM_LOGGER = logging.getLogger("PRISM_LOGGER")
 
 
 # Triggers
```

### Comparing `prism-dev-0.1.1/prism/tests/integration/integration_test_class.py` & `prism-dev-0.1.2/prism/tests/integration/integration_test_class.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_client.py` & `prism-dev-0.1.2/prism/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_compile.py` & `prism-dev-0.1.2/prism/tests/integration/test_compile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_connect.py` & `prism-dev-0.1.2/prism/tests/integration/test_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 connect_task_invalid_expected_events = header_events + [
     'InvalidType',
     'SeparatorEvent'
 ]
 
 # Snowflake profile as a dict
 expected_snowflake_dict = {
-    'profile_name': {
+    'default': {
         'adapters': {
             'snowflake_adapter_name_here': {
                 'type': 'snowflake',
                 'user': None,
                 'password': None,
                 'account': None,
                 'role': None,
@@ -75,15 +75,15 @@
             }
         }
     }
 }
 
 # PySpark profile as a dict
 expected_pyspark_dict = {
-    'profile_name': {
+    'default': {
         'adapters': {
             'pyspark_adapter_name_here': {
                 'type': 'pyspark',
                 'alias': 'spark',
                 'loglevel': 'WARN',
                 'config': {
                     'spark.driver.cores': None,
@@ -99,15 +99,15 @@
             }
         }
     }
 }
 
 # Snowflake + PySpark profile
 expected_snowflake_pyspark_dict = {
-    'profile_name': {
+    'default': {
         'adapters': {
             'snowflake_adapter_name_here': {
                 'type': 'snowflake',
                 'user': None,
                 'password': None,
                 'account': None,
                 'role': None,
```

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_create.py` & `prism-dev-0.1.2/prism/tests/integration/test_create.py`

 * *Files 21% similar despite different names*

```diff
@@ -145,7 +145,60 @@
         self.assertEqual(' | '.join(expected_events), run_twice.get_results())
 
         # Remove task
         os.unlink(Path(wkdir / 'modules' / 'dummy_task.py'))
 
         # Set up wkdir for the next test case
         self._set_up_wkdir()
+
+    def test_create_decorated_task(self):
+        """
+        Created a task using the --decorated flag. This will create a class that has
+        a decorated function rather than a class.
+        """
+        # Change directory to 005_simple_project_with_profile
+        self.maxDiff = None
+
+        # Set working directory
+        wkdir = Path(TEST_PROJECTS) / '005_simple_project_no_null'
+        os.chdir(wkdir)
+
+        # First, check that `dummy_task.py` does not exist in the project
+        self.assertFalse(Path(wkdir / 'modules' / 'dummy_task.py').is_file())
+
+        # ------------------------------------------------------------------------------
+        # Run
+        args = [
+            'create', 'task', '--type', 'python', '--name', 'dummy_task', '--decorated'
+        ]
+        create_task_run = self._run_prism(args)
+
+        # `triggers.yml` file was found
+        self.assertTrue(Path(wkdir / 'modules' / 'dummy_task.py').is_file())
+
+        # Expected events
+        expected_events = SUCCESS_EXPECTED_CREATE_START_EVENTS \
+            + SUCCESS_EXPECTED_CREATE_TASK_EVENTS \
+            + SUCCESS_EXPECTED_CREATE_END_EVENTS
+        self.assertEqual(' | '.join(expected_events), create_task_run.get_results())
+
+        # Get the class name
+        with open(Path(wkdir / 'modules' / 'dummy_task.py'), 'r') as f:
+            dummy_task_py = f.read()
+        self.assertTrue("class DummyTask(prism.task.PrismTask):" not in dummy_task_py)
+        decorated_string = "\n".join([
+            "@task(",
+            "    retries=0,",
+            "    retry_delay_seconds=0,",
+            "    targets=[",
+            "        target(...)",
+            "    ]",
+            ")"
+        ])
+        self.assertTrue(decorated_string in dummy_task_py)
+        self.assertTrue("def dummy_task(tasks, hooks):" in dummy_task_py)
+
+        # Remove task
+        os.unlink(Path(wkdir / 'modules' / 'dummy_task.py'))
+
+        # Set up wkdir for the next test case
+        self._set_up_wkdir()
```

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_dbt.py` & `prism-dev-0.1.2/prism/tests/integration/test_dbt.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_hooks.py` & `prism-dev-0.1.2/prism/tests/integration/test_hooks.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_init.py` & `prism-dev-0.1.2/prism/tests/integration/test_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,88 +12,86 @@
 # Imports #
 ###########
 
 # Standard library imports
 import os
 from pathlib import Path
 import shutil
-import unittest
 
 # Prism imports
-import prism.cli.base
-from prism.main import main
-import prism.logging
 import prism.tests.integration.integration_test_class as integration_test_class
 
 
 #################################
 # Test case directory and paths #
 #################################
 
 # Directory containing all prism_project.py test cases
 TEST_CASE_WKDIR = os.path.dirname(__file__)
 TEST_PROJECTS = Path(TEST_CASE_WKDIR) / 'test_projects'
 
 
-################################
-## Test case class definition ##
-################################
+##############################
+# Test case class definition #
+##############################
 
 class TestInitIntegration(integration_test_class.IntegrationTestCase):
 
-
     def test_init(self):
         """
         `prism init`
         """
-        
+
         # Set working directory
         os.chdir(TEST_PROJECTS)
 
         # Remove folder '001_init' if it already exists
         init_path = Path(TEST_PROJECTS) / '001_init'
         if init_path.is_dir():
             shutil.rmtree(init_path)
 
         # Execute init command
         args = ['init', '--project-name', '001_init']
         init_run = self._run_prism(args)
         init_run_results = init_run.get_results()
-        
-        # Since project has not been created, the events should align with a successful task creation
+
+        # Since project has not been created, the events should align with a successful
+        # task creation
         expected_events = ' | '.join([
             'SeparatorEvent',
             'TaskRunEvent',
             'EmptyLineEvent',
             'CreatingProjectDirEvent',
             'EmptyLineEvent',
             'InitSuccessfulEvent',
             'SeparatorEvent',
         ])
         self.assertEqual(expected_events, init_run_results)
         self.assertTrue(init_path.is_dir())
         self._is_valid_project(init_path)
 
-        # Try creating the project again. This time, we should see a `ProjectAlreadyExistsEvent`
+        # Try creating the project again. This time, we should see a
+        # `ProjectAlreadyExistsEvent`
         os.chdir(TEST_PROJECTS)
         init_run_already_exists = self._run_prism(args)
         init_run_already_exists_results = init_run_already_exists.get_results()
         expected_events_already_exists = ' | '.join([
             'SeparatorEvent',
             'TaskRunEvent',
             'EmptyLineEvent',
             'ProjectAlreadyExistsEvent',
             'SeparatorEvent',
         ])
-        self.assertEqual(expected_events_already_exists, init_run_already_exists_results)
-        
+        self.assertEqual(
+            expected_events_already_exists, init_run_already_exists_results
+        )
+
         # Set up wkdir for the next test case
         self._set_up_wkdir()
 
-    
     def test_init_minimal(self):
         """
         `prism init --minimal`
         """
         # Set working directory
         os.chdir(TEST_PROJECTS)
 
@@ -102,16 +100,17 @@
         if init_path.is_dir():
             shutil.rmtree(init_path)
 
         # Execute init command
         args = ['init', '--project-name', '001a_init_minimal', '--minimal']
         init_run = self._run_prism(args)
         init_run_results = init_run.get_results()
-        
-        # Since project has not been created, the events should align with a successful task creation
+
+        # Since project has not been created, the events should align with a successful
+        # task creation
         expected_events = ' | '.join([
             'SeparatorEvent',
             'TaskRunEvent',
             'EmptyLineEvent',
             'CreatingProjectDirEvent',
             'EmptyLineEvent',
             'InitSuccessfulEvent',
@@ -122,25 +121,25 @@
         self._is_valid_project(init_path)
 
         # Check that data and output directory do not exist
         self.assertFalse(Path(init_path / 'data').is_dir())
         self.assertFalse(Path(init_path / 'output').is_dir())
         self.assertFalse(Path(init_path / 'functions.py').is_file())
 
-        # Try creating the project again. This time, we should see a `ProjectAlreadyExistsEvent`
+        # Try creating the project again. This time, we should see a
+        # `ProjectAlreadyExistsEvent`
         os.chdir(TEST_PROJECTS)
         init_run_already_exists = self._run_prism(args)
         init_run_already_exists_results = init_run_already_exists.get_results()
         expected_events_already_exists = ' | '.join([
             'SeparatorEvent',
             'TaskRunEvent',
             'EmptyLineEvent',
             'ProjectAlreadyExistsEvent',
             'SeparatorEvent',
         ])
-        self.assertEqual(expected_events_already_exists, init_run_already_exists_results)
-        
+        self.assertEqual(
+            expected_events_already_exists, init_run_already_exists_results
+        )
+
         # Set up wkdir for the next test case
         self._set_up_wkdir()
-
-
-# EOF
```

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/modules/module01.py` & `prism-dev-0.1.2/prism/templates/minimal_project/modules/class_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import prism_project
 
 
 ###################
 # Task definition #
 ###################
 
-class Module01(prism.task.PrismTask):
+class ExampleTask(prism.task.PrismTask):
 
     # Run
     @prism.decorators.target(type=prism.target.Txt, loc=prism_project.OUTPUT / 'hello_world.txt')
     def run(self, tasks, hooks):
         """
         Execute task.
```

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/001_init/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/001_init/prism_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 1
 
 
 # Profile directory and name
 PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
-PROFILE = None
+PROFILE = "default"
 
 
 # Logger
 PRISM_LOGGER = logging.getLogger("PRISM_LOGGER")
 
 
 # Triggers
```

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/modules/module01.py` & `prism-dev-0.1.2/prism/templates/starter_project/modules/class_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import prism_project
 
 
 ###################
 # Task definition #
 ###################
 
-class Module01(prism.task.PrismTask):
+class ExampleTask(prism.task.PrismTask):
 
     # Run
     @prism.decorators.target(type=prism.target.Txt, loc=prism_project.OUTPUT / 'hello_world.txt')
     def run(self, tasks, hooks):
         """
         Execute task.
```

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 1
 
 
 # Profile directory and name
 PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
-PROFILE = None  # name of profile within `profiles.yml`
+PROFILE = "default"  # name of profile within `profiles.yml`
 
 
 # Logger
 PRISM_LOGGER = logging.getLogger("PRISM_LOGGER")
 
 
 # Triggers
```

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/functions.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/002_no_project_py/functions.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/004_simple_project/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/module02.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/004_simple_project/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/modules/module03.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/004_simple_project/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/004_simple_project/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/004_simple_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/functions.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/005_simple_project_no_null/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 1
 
 
 # Profile directory and name
 PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
-PROFILE = 'profile_name'  # name of profile within `profiles.yml`
+PROFILE = 'default'  # name of profile within `profiles.yml`
 
 
 # Logger
 PRISM_LOGGER = logging.getLogger("PRISM_LOGGER")
 
 
 # Other variables / parameters. Make sure to capitalize all of these!
```

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/007_spark_project/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module02.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/007_spark_project/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module03.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/007_spark_project/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/modules/module04.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/007_spark_project/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/007_spark_project/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/007_spark_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/csv.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/modules/csv.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/modules/csv_iter.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/modules/csv_mult.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/modules/parquet.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/modules/parquet.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/008_targets/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/008_targets/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/bad_adapter.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/modules/filter_customers.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/012_concurrency/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module02.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/012_concurrency/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module03.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/012_concurrency/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/modules/module04.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/012_concurrency/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/012_concurrency/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/012_concurrency/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # Thread count: number of workers to use to execute tasks concurrently. If set to 1,
 # then 1 task is run at a time.
 THREADS = 2
 
 
 # Profile directory and name
 PROFILE_YML_PATH = Path(__file__).parent / 'profile.yml'
-PROFILE = 'profile_name'  # name of profile within `profiles.yml`
+PROFILE = 'default'  # name of profile within `profiles.yml`
 
 
 # Logger
 PRISM_LOGGER = logging.getLogger("PRISM_LOGGER")
 
 
 # Other variables / parameters. Make sure to capitalize all of these!
```

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/016_test_triggers_error/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py` & `prism-dev-0.1.2/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_run.py` & `prism-dev-0.1.2/prism/tests/integration/test_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 ###########
 # Imports #
 ###########
 
 # Standard library imports
+import json
 import pandas as pd
 import os
 from pathlib import Path
 import shutil
 from typing import Dict, List
 
 # Prism imports
@@ -848,7 +849,150 @@
         self.assertEqual(' | '.join(expected_events), run_results)
 
         # Remove the .compiled directory, if it exists
         self._remove_compiled_dir(wkdir)
 
         # Set up wkdir for the next test case
         self._set_up_wkdir()
+
+    def test_decorator_tasks_with_targets(self):
+        """
+        `prism run` on a project where all the tasks are functions decorated with
+        `@task`
+        """
+        self.maxDiff = None
+
+        # Set working directory
+        wkdir = Path(TEST_PROJECTS) / '019_dec_targets'
+        os.chdir(wkdir)
+
+        # Remove the .compiled directory, if it exists
+        self._remove_compiled_dir(wkdir)
+
+        # Remove all files in the output directory
+        self._remove_files_in_output(wkdir)
+
+        # Run
+        args = ['run']
+        runtask_run = self._run_prism(args)
+        runtask_run_results = runtask_run.get_results()
+        expected_events = self._check_trigger_events(
+            {
+                'extract.py': 'DONE',
+                'load.py': 'DONE'
+            },
+        ) + _run_task_end_events('TaskSuccessfulEndEvent')
+        self.assertEqual(' | '.join(expected_events), runtask_run_results)
+
+        # Check output of 'extract' task
+        self.assertTrue(Path(wkdir / 'output' / 'astros.json').is_file())
+        self.assertTrue(Path(wkdir / 'output' / 'second_target.txt').is_file())
+
+        # Astros JSON file
+        with open(Path(wkdir / 'output' / 'astros.json'), 'r') as f:
+            astros_str = f.read()
+        astros_dict = json.loads(astros_str)
+        self.assertEqual(astros_dict["message"], "success")
+
+        # Dummy second target text file
+        with open(Path(wkdir / 'output' / 'second_target.txt'), 'r') as f:
+            second_target = f.read()
+        self.assertEqual(second_target, "second target")
+
+        # Check output of 'load' task
+        names = [
+            "Andrey Fedyaev",
+            "Deng Qingming",
+            "Dmitry Petelin",
+            "Fei Junlong",
+            "Frank Rubio",
+            "Sergey Prokopyev",
+            "Stephen Bowen",
+            "Sultan Alneyadi",
+            "Warren Hoburg",
+            "Zhang Lu",
+        ]
+        for n in names:
+            formatted_name = n.lower().replace(" ", "_")
+            self.assertTrue(Path(wkdir / 'output' / f'{formatted_name}.txt').is_file())
+            with open(Path(wkdir / 'output' / f'{formatted_name}.txt'), 'r') as f:
+                contents = f.read()
+            self.assertEqual(contents, n)
+
+        # Remove the .compiled directory, if it exists
+        self._remove_compiled_dir(wkdir)
+
+        # Set up the working directory
+        self._set_up_wkdir()
+
+    def test_decorator_tasks_with_retries(self):
+        """
+        `prism run` on a project where all the tasks are functions decorated with
+        `@task` and the user wants to retry a task
+        """
+        self.maxDiff = None
+
+        # Set working directory
+        wkdir = Path(TEST_PROJECTS) / '020_dec_retries'
+        os.chdir(wkdir)
+
+        # Remove the .compiled directory, if it exists
+        self._remove_compiled_dir(wkdir)
+
+        # Remove all files in the output directory
+        self._remove_files_in_output(wkdir)
+
+        # Run
+        args = ['run']
+        runtask_run = self._run_prism(args)
+        runtask_run_results = runtask_run.get_results()
+        expected_events = run_success_starting_events + \
+            ['TasksHeaderEvent'] + \
+            _execution_events_modules(
+                {
+                    'extract.py': 'DONE',
+                    'load.py': 'ERROR'
+                },
+            ) + \
+            ['DelayEvent'] + \
+            _execution_events_modules(
+                {'load.py (RETRY 1)': 'ERROR'}
+            ) + \
+            [
+                "EmptyLineEvent",
+                "ExecutionErrorEvent",
+                "TriggersHeaderEvent",
+                "ExecutionEvent - test_trigger_function - RUN",
+                "ExecutionEvent - test_trigger_function - DONE",
+                "SeparatorEvent"
+            ]
+        self.assertEqual(' | '.join(expected_events), runtask_run_results)
+
+        # Check output of 'extract' task
+        self.assertTrue(Path(wkdir / 'output' / 'astros.json').is_file())
+        with open(Path(wkdir / 'output' / 'astros.json'), 'r') as f:
+            astros_str = f.read()
+        astros_dict = json.loads(astros_str)
+        self.assertEqual(astros_dict["message"], "success")
+
+        # Output of 'load' task was not created
+        names = [
+            "Andrey Fedyaev",
+            "Deng Qingming",
+            "Dmitry Petelin",
+            "Fei Junlong",
+            "Frank Rubio",
+            "Sergey Prokopyev",
+            "Stephen Bowen",
+            "Sultan Alneyadi",
+            "Warren Hoburg",
+            "Zhang Lu",
+        ]
+        for n in names:
+            formatted_name = n.lower().replace(" ", "_")
+            self.assertFalse(Path(wkdir / 'output' / f'{formatted_name}.txt').is_file())
+
+        # Remove the .compiled directory, if it exists
+        self._remove_compiled_dir(wkdir)
+
+        # Set up the working directory
+        self._set_up_wkdir()
```

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_spark_submit.py` & `prism-dev-0.1.2/prism/tests/integration/test_spark_submit.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/integration/test_targets.py` & `prism-dev-0.1.2/prism/tests/integration/test_targets.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_adapter_profile.py` & `prism-dev-0.1.2/prism/tests/unit/test_adapter_profile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_agent/prism_project.py` & `prism-dev-0.1.2/prism/tests/unit/test_agent/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_agents.py` & `prism-dev-0.1.2/prism/tests/unit/test_agents.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_all_dag_fns.py` & `prism-dev-0.1.2/prism/tests/unit/test_all_dag_fns.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_jinja.py` & `prism-dev-0.1.2/prism/tests/unit/test_jinja.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
     def test_env_exists(self):
         """
         env() function returns an environment variable
         """
         yml = self._load_profile_yml(ENV_EXISTS)
         expected_user = "/bin/bash"
-        actual_user = yml['profile_name']['adapters']['snowflake_adapter_name_here']['user']  # noqa: E501
+        actual_user = yml['default']['adapters']['snowflake_adapter_name_here']['user']  # noqa: E501
         self.assertEqual(expected_user, actual_user)
 
     def test_env_doesnt_exist(self):
         """
         env() function returns a blank string if the environment variable doesn't exist
         """
         with self.assertRaises(prism.exceptions.EnvironmentVariableNotFoundException) as cm:  # noqa: E501
@@ -124,31 +124,31 @@
 
     def test_parent(self):
         """
         parent() function returns the parent directory for the inputted path
         """
         yml = self._load_profile_yml(PARENT)
         expected_profiles_dir = PARENT.parent.parent
-        actual_profiles_dir = yml['profile_name']['adapters']['dbt']['profiles_dir']
+        actual_profiles_dir = yml['default']['adapters']['dbt']['profiles_dir']
         self.assertEqual(str(expected_profiles_dir), actual_profiles_dir)
 
     def test_wkdir(self):
         """
         wkdir() function returns the current directory
         """
         yml = self._load_profile_yml(WKDIR)
         expected_profiles_dir = WKDIR.parent
-        actual_profiles_dir = yml['profile_name']['adapters']['dbt']['profiles_dir']
+        actual_profiles_dir = yml['default']['adapters']['dbt']['profiles_dir']
         self.assertEqual(str(expected_profiles_dir), actual_profiles_dir)
 
     def test_path(self):
         """
         Path(__file__) returns the path of the YAML file and can be manipulated like
         Pathlib's Path object.
         """
         yml = self._load_profile_yml(PATH_STUFF)
         expected_project_dir = PATH_STUFF
         expected_profiles_dir = PATH_STUFF.parent
-        actual_project_dir = yml['profile_name']['adapters']['dbt']['project_dir']
-        actual_profiles_dir = yml['profile_name']['adapters']['dbt']['profiles_dir']
+        actual_project_dir = yml['default']['adapters']['dbt']['project_dir']
+        actual_profiles_dir = yml['default']['adapters']['dbt']['profiles_dir']
         self.assertEqual(str(expected_project_dir), str(actual_project_dir))
         self.assertEqual(str(expected_profiles_dir), str(actual_profiles_dir))
```

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_module_parser.py` & `prism-dev-0.1.2/prism/tests/unit/test_module_parser_cls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Unit testing for functions for PythonModuleParser class.
+Unit testing for parsing modules with tasks created via the PrismTask class.
 
 Table of Contents:
 - Imports
 - Test case directory and paths
 - Test case class definition
 """
 
@@ -44,15 +44,15 @@
 NO_RUN_FUNC = Path('no_run_func.py')
 
 
 ##############################
 # Test case class definition #
 ##############################
 
-class TestModuleParsing(unittest.TestCase):
+class TestModuleClassParsing(unittest.TestCase):
 
     def test_one_prism_task(self):
         """
         Test behavior of parser with just one Prism task
         """
         # Prism task
         parser = ast_parser.AstParser(ONE_PRISM_TASK, MODULE_TEST_CASES)
@@ -62,15 +62,15 @@
         prism_task_name = prism_task_class.name
 
         # Run function
         run_func = parser.get_run_func(prism_task_class)
         run_func_args = parser.get_func_args(run_func)
 
         # Number of prism tasks
-        num_prism_tasks = parser.get_num_prism_tasks(parser.bases)
+        num_prism_tasks = parser.get_num_prism_task_classes(parser.bases)
 
         self.assertEqual("NormalPrismTask", prism_task_name)
         self.assertEqual(1, num_prism_tasks)
         self.assertEqual(['self', 'tasks', 'hooks'], run_func_args)
 
         # Calling `parse` shouldn't throw an error
         self.assertEqual([], parser.parse())
@@ -81,15 +81,15 @@
         """
         parser = ast_parser.AstParser(NO_PRISM_TASK, MODULE_TEST_CASES)
 
         # Prism task name
         prism_task_class = parser.get_prism_task_node(parser.classes, parser.bases)
 
         # Number of prism tasks
-        num_prism_tasks = parser.get_num_prism_tasks(parser.bases)
+        num_prism_tasks = parser.get_num_prism_task_classes(parser.bases)
 
         self.assertIsNone(prism_task_class)
         self.assertEqual(0, num_prism_tasks)
 
         # Calling `parse` should throw an error
         with self.assertRaises(prism.exceptions.ParserException) as cm:
             parser.parse()
@@ -99,33 +99,22 @@
     def test_multiple_prism_task(self):
         """
         Test behavior of parser when module has multiple Prism tasks
         """
         parser = ast_parser.AstParser(MULTIPLE_PRISM_TASKS, MODULE_TEST_CASES)
 
         # Number of prism tasks
-        num_prism_tasks = parser.get_num_prism_tasks(parser.bases)
-
-        # Prism task name -- it should return the first one
-        first_prism_task_class = parser.get_prism_task_node(
-            parser.classes, parser.bases
-        )
-        first_prism_task_class_name = first_prism_task_class.name
-
-        # Run function
-        run_func = parser.get_run_func(first_prism_task_class)
-        run_func_args = parser.get_func_args(run_func)
-
+        num_prism_tasks = parser.get_num_prism_task_classes(parser.bases)
         self.assertEqual(2, num_prism_tasks)
-        self.assertEqual("FirstPrismTask", first_prism_task_class_name)
-        self.assertEqual(['self', 'tasks', 'hooks'], run_func_args)
 
-        # Calling `parse` should throw an error
-        with self.assertRaises(prism.exceptions.ParserException) as cm:
-            parser.parse()
+        # Prism task name -- it should return the first one
+        with self.assertRaises(prism.exceptions.RuntimeException) as cm:
+            _ = parser.get_prism_task_node(
+                parser.classes, parser.bases
+            )
         expected_msg = f"too many PrismTasks in `{str(MULTIPLE_PRISM_TASKS)}`"
         self.assertEqual(expected_msg, str(cm.exception))
 
     def test_diff_import_structure(self):
         """
         Different PrismTask import structure (i.e., import prism.task.PrismTask) should
         not affect the behavior of the parser
@@ -138,15 +127,15 @@
         prism_task_name = prism_task_class.name
 
         # Run function
         run_func = parser.get_run_func(prism_task_class)
         run_func_args = parser.get_func_args(run_func)
 
         # Number of prism tasks
-        num_prism_tasks = parser.get_num_prism_tasks(parser.bases)
+        num_prism_tasks = parser.get_num_prism_task_classes(parser.bases)
 
         self.assertEqual("DiffImportStructure", prism_task_name)
         self.assertEqual(1, num_prism_tasks)
         self.assertEqual(['self', 'tasks', 'hooks'], run_func_args)
 
         # Calling `parse` shouldn't throw an error
         self.assertEqual([], parser.parse())
@@ -164,15 +153,15 @@
         prism_task_name = prism_task_class.name
 
         # Run function
         run_func = parser.get_run_func(prism_task_class)
         run_func_args = parser.get_func_args(run_func)
 
         # Number of prism tasks
-        num_prism_tasks = parser.get_num_prism_tasks(parser.bases)
+        num_prism_tasks = parser.get_num_prism_task_classes(parser.bases)
 
         self.assertEqual("OnlyPrismTask", prism_task_name)
         self.assertEqual(1, num_prism_tasks)
         self.assertEqual(['self', 'tasks', 'hooks'], run_func_args)
 
         # Calling `parse` shouldn't throw an error
         self.assertEqual([], parser.parse())
@@ -189,25 +178,25 @@
         prism_task_name = prism_task_class.name
 
         # Run function
         run_func = parser.get_run_func(prism_task_class)
         run_func_args = parser.get_func_args(run_func)
 
         # Number of prism tasks
-        num_prism_tasks = parser.get_num_prism_tasks(parser.bases)
+        num_prism_tasks = parser.get_num_prism_task_classes(parser.bases)
 
         self.assertEqual("TaskWithTarget", prism_task_name)
         self.assertEqual(1, num_prism_tasks)
         self.assertEqual(['self', 'tasks', 'hooks'], run_func_args)
 
         # Calling `parse` shouldn't throw an error
         self.assertEqual([Path('hello.py'), Path('world.py')], parser.parse())
 
         # Get target
-        targets = parser.get_targets(run_func)
+        targets = parser.get_targets(prism_task_class, run_func)
         expected_targets = "os.path.join(os.getcwd(), 'temp')"
         self.assertEqual(targets, expected_targets)
 
     def test_tasks_refs(self):
         """
         Test behavior of parse when there are mod references
         """
@@ -219,15 +208,15 @@
         prism_task_name = prism_task_class.name
 
         # Run function
         run_func = parser.get_run_func(prism_task_class)
         run_func_args = parser.get_func_args(run_func)
 
         # Number of prism tasks
-        num_prism_tasks = parser.get_num_prism_tasks(parser.bases)
+        num_prism_tasks = parser.get_num_prism_task_classes(parser.bases)
 
         self.assertEqual("TasksRefs", prism_task_name)
         self.assertEqual(1, num_prism_tasks)
         self.assertEqual(['self', 'tasks', 'hooks'], run_func_args)
 
         # Calling `parse` shouldn't throw an error
         expected_tasks = [
@@ -285,9 +274,9 @@
         ]:
             with self.assertRaises(prism.exceptions.ParserException) as cm:
                 parser = ast_parser.AstParser(module, MODULE_TEST_CASES)
                 parser.parse()
             if module == NO_RUN_FUNC:
                 expected_msg = f"no `run` function in PrismTask in `{str(module)}`"
             else:
-                expected_msg = f'invalid arguments in `run` function in PrismTask in {str(module)}; should only be "self", "tasks", and "hooks"'  # noqa: E501
+                expected_msg = f'invalid arguments in `run` function in PrismTask in {str(module)}; should only be `self`,`tasks`,`hooks`'  # noqa: E501
             self.assertEqual(expected_msg, str(cm.exception))
```

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/bad_trigger_key.py` & `prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/bad_trigger_key.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/multiple_profiles.py` & `prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/multiple_profiles.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/no_profile.py` & `prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/no_profile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/non_null_profile.py` & `prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/non_null_profile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/null_profile.py` & `prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/null_profile.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py` & `prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py` & `prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_prism_project_py/triggers_normal.py` & `prism-dev-0.1.2/prism/tests/unit/test_prism_project_py/triggers_normal.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_project.py` & `prism-dev-0.1.2/prism/tests/unit/test_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_trigger.py` & `prism-dev-0.1.2/prism/tests/unit/test_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/tests/unit/test_trigger_yml/prism_project.py` & `prism-dev-0.1.2/prism/tests/unit/test_trigger_yml/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/triggers/__init__.py` & `prism-dev-0.1.2/prism/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism/ui.py` & `prism-dev-0.1.2/prism/ui.py`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/prism_dev.egg-info/PKG-INFO` & `prism-dev-0.1.2/prism_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prism-dev
-Version: 0.1.1
+Version: 0.1.2
 Summary: The easiest way to create data pipelines in Python.
 Author: prism founders
 Author-email: hello@runprism.com
 License: Apache-2.0
 Project-URL: homepage, https://www.runprism.com
 Project-URL: documentation, https://docs.runprism.com
 Project-URL: repository, https://github.com/runprism/prism
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prism-dev Version: 0.1.1 Summary: The easiest way
+Metadata-Version: 2.1 Name: prism-dev Version: 0.1.2 Summary: The easiest way
 to create data pipelines in Python. Author: prism founders Author-email:
 hello@runprism.com License: Apache-2.0 Project-URL: homepage, https://
 www.runprism.com Project-URL: documentation, https://docs.runprism.com Project-
 URL: repository, https://github.com/runprism/prism Platform: unix Platform:
 linux Platform: osx Platform: win32 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `prism-dev-0.1.1/prism_dev.egg-info/SOURCES.txt` & `prism-dev-0.1.2/prism_dev.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 prism/__init__.py
 prism/admin.py
 prism/constants.py
-prism/decorators.py
 prism/exceptions.py
 prism/logging.py
 prism/main.py
 prism/target.py
 prism/task.py
 prism/ui.py
 prism/agents/__init__.py
@@ -31,14 +30,17 @@
 prism/cli/create_task.py
 prism/cli/create_trigger.py
 prism/cli/graph.py
 prism/cli/init.py
 prism/cli/run.py
 prism/cli/spark_submit.py
 prism/client/__init__.py
+prism/decorators/__init__.py
+prism/decorators/target.py
+prism/decorators/task.py
 prism/docs/__init__.py
 prism/docs/build/311ea03002abadcdcaba.png
 prism/docs/build/54968a39190c43d592b9.svg
 prism/docs/build/737ad70b3f2d3a9b5f6e.ico
 prism/docs/build/__init__.py
 prism/docs/build/ce188596011a8fa32931.png
 prism/docs/build/index.html
@@ -88,33 +90,37 @@
 prism/templates/__init__.py
 prism/templates/agents/__init__.py
 prism/templates/agents/docker.yml
 prism/templates/agents/ec2.yml
 prism/templates/minimal_project/.gitignore
 prism/templates/minimal_project/__init__.py
 prism/templates/minimal_project/prism_project.py
-prism/templates/minimal_project/modules/module01.py
+prism/templates/minimal_project/modules/class_task.py
+prism/templates/minimal_project/modules/decorated_task.py
 prism/templates/profile/__init__.py
 prism/templates/profile/bigquery/profile.yml
 prism/templates/profile/dbt/profile.yml
 prism/templates/profile/postgres/profile.yml
 prism/templates/profile/pyspark/profile.yml
 prism/templates/profile/redshift/profile.yml
 prism/templates/profile/snowflake/profile.yml
 prism/templates/profile/trino/profile.yml
 prism/templates/starter_project/.gitignore
 prism/templates/starter_project/__init__.py
 prism/templates/starter_project/prism_project.py
 prism/templates/starter_project/utils.py
 prism/templates/starter_project/data/.exists
 prism/templates/starter_project/dev/dev.ipynb
-prism/templates/starter_project/modules/module01.py
+prism/templates/starter_project/modules/class_task.py
+prism/templates/starter_project/modules/decorated_task.py
 prism/templates/starter_project/output/.exists
-prism/templates/tasks/pyspark.py
-prism/templates/tasks/python.py
+prism/templates/tasks/pyspark_cls.py
+prism/templates/tasks/pyspark_dec.py
+prism/templates/tasks/python_cls.py
+prism/templates/tasks/python_dec.py
 prism/templates/tasks/sql.py
 prism/templates/triggers/__init__.py
 prism/templates/triggers/function.yml
 prism/templates/triggers/prism_project.yml
 prism/tests/__init__.py
 prism/tests/integration/__init__.py
 prism/tests/integration/integration_test_class.py
@@ -219,23 +225,33 @@
 prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py
 prism/tests/integration/test_projects/017_test_triggers_extra_key/utils.py
 prism/tests/integration/test_projects/017_test_triggers_extra_key/modules/module01.py
 prism/tests/integration/test_projects/018_test_triggers_no_include/__init__.py
 prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py
 prism/tests/integration/test_projects/018_test_triggers_no_include/utils.py
 prism/tests/integration/test_projects/018_test_triggers_no_include/modules/module01.py
+prism/tests/integration/test_projects/019_dec_targets/__init__.py
+prism/tests/integration/test_projects/019_dec_targets/prism_project.py
+prism/tests/integration/test_projects/019_dec_targets/modules/extract.py
+prism/tests/integration/test_projects/019_dec_targets/modules/load.py
+prism/tests/integration/test_projects/020_dec_retries/__init__.py
+prism/tests/integration/test_projects/020_dec_retries/prism_project.py
+prism/tests/integration/test_projects/020_dec_retries/utils.py
+prism/tests/integration/test_projects/020_dec_retries/modules/extract.py
+prism/tests/integration/test_projects/020_dec_retries/modules/load.py
 prism/tests/integration/test_projects/common/__init__.py
 prism/tests/integration/test_projects/common/functions.py
 prism/tests/unit/__init__.py
 prism/tests/unit/test_adapter_profile.py
 prism/tests/unit/test_agents.py
 prism/tests/unit/test_all_dag_fns.py
 prism/tests/unit/test_import.py
 prism/tests/unit/test_jinja.py
-prism/tests/unit/test_module_parser.py
+prism/tests/unit/test_module_parser_cls.py
+prism/tests/unit/test_module_parser_dec.py
 prism/tests/unit/test_project.py
 prism/tests/unit/test_trigger.py
 prism/tests/unit/dummy_modules/dummy_module1.py
 prism/tests/unit/test_agent/prism_project.py
 prism/tests/unit/test_all_things_dag/__init__.py
 prism/tests/unit/test_all_things_dag/dag_cycle/__init__.py
 prism/tests/unit/test_all_things_dag/dag_cycle/moduleA.py
@@ -280,14 +296,24 @@
 prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleB.py
 prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleC.py
 prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleD.py
 prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleE.py
 prism/tests/unit/test_modules/bad_run_extra_arg.py
 prism/tests/unit/test_modules/bad_run_missing_arg.py
 prism/tests/unit/test_modules/bad_run_no_tasks.py
+prism/tests/unit/test_modules/dec_bad_dec_no_parentheses.py
+prism/tests/unit/test_modules/dec_bad_run_extra_arg.py
+prism/tests/unit/test_modules/dec_bad_run_missing_arg.py
+prism/tests/unit/test_modules/dec_diff_decorator_structure.py
+prism/tests/unit/test_modules/dec_multiple_prism_tasks.py
+prism/tests/unit/test_modules/dec_no_prism_task.py
+prism/tests/unit/test_modules/dec_one_prism_task.py
+prism/tests/unit/test_modules/dec_other_functions.py
+prism/tests/unit/test_modules/dec_task_with_target.py
+prism/tests/unit/test_modules/dec_tasks_refs.py
 prism/tests/unit/test_modules/diff_import_structure.py
 prism/tests/unit/test_modules/if_name_main.py
 prism/tests/unit/test_modules/multiple_prism_tasks.py
 prism/tests/unit/test_modules/no_prism_task.py
 prism/tests/unit/test_modules/no_run_func.py
 prism/tests/unit/test_modules/one_prism_task.py
 prism/tests/unit/test_modules/other_classes.py
```

### Comparing `prism-dev-0.1.1/prism_dev.egg-info/requires.txt` & `prism-dev-0.1.2/prism_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/pyproject.toml` & `prism-dev-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prism-dev-0.1.1/setup.cfg` & `prism-dev-0.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = prism-dev
 description = The easiest way to create data pipelines in Python.
 long_description_content_type = text/markdown
 long_description = file: README.md
-version = 0.1.1
+version = 0.1.2
 author = prism founders
 author_email = hello@runprism.com
 license = Apache-2.0
 license_file = LICENSE
 platforms = unix, linux, osx, win32
 classifiers = 
 	Programming Language :: Python :: 3
```

