# Comparing `tmp/mpyl-0.0.9-py3-none-any.whl.zip` & `tmp/mpyl-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,72 +1,87 @@
-Zip file size: 74388 bytes, number of entries: 70
--rw-r--r--  2.0 unx     1927 b- defN 23-Mar-16 09:26 mpyl/__init__.py
--rw-r--r--  2.0 unx      215 b- defN 23-Mar-16 09:26 mpyl/__main__.py
--rw-r--r--  2.0 unx    11538 b- defN 23-Mar-16 09:26 mpyl/project.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Mar-16 09:26 mpyl/validation.py
--rw-r--r--  2.0 unx      568 b- defN 23-Mar-16 09:26 mpyl/cli/__init__.py
--rw-r--r--  2.0 unx       51 b- defN 23-Mar-16 09:26 mpyl/cli/build/__init__.py
--rw-r--r--  2.0 unx     2250 b- defN 23-Mar-16 09:26 mpyl/cli/build/jenkins.py
--rw-r--r--  2.0 unx     4542 b- defN 23-Mar-16 09:26 mpyl/cli/build/mpyl.py
--rw-r--r--  2.0 unx      471 b- defN 23-Mar-16 09:26 mpyl/cli/commands/__init__.py
--rw-r--r--  2.0 unx     4539 b- defN 23-Mar-16 09:26 mpyl/cli/commands/build.py
--rw-r--r--  2.0 unx     2170 b- defN 23-Mar-16 09:26 mpyl/cli/commands/meta_info.py
--rw-r--r--  2.0 unx     1756 b- defN 23-Mar-16 09:26 mpyl/cli/commands/projects.py
--rw-r--r--  2.0 unx       39 b- defN 23-Mar-16 09:26 mpyl/cli/projects/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-16 09:26 mpyl/projects/__init__.py
--rw-r--r--  2.0 unx      265 b- defN 23-Mar-16 09:26 mpyl/projects/find.py
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-16 09:26 mpyl/reporting/__init__.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-16 09:26 mpyl/reporting/formatting/__init__.py
--rw-r--r--  2.0 unx     2622 b- defN 23-Mar-16 09:26 mpyl/reporting/formatting/markdown.py
--rw-r--r--  2.0 unx     1148 b- defN 23-Mar-16 09:26 mpyl/reporting/formatting/text.py
--rw-r--r--  2.0 unx      488 b- defN 23-Mar-16 09:26 mpyl/reporting/targets/__init__.py
--rw-r--r--  2.0 unx     5538 b- defN 23-Mar-16 09:26 mpyl/reporting/targets/github.py
--rw-r--r--  2.0 unx     4656 b- defN 23-Mar-16 09:26 mpyl/reporting/targets/jira.py
--rw-r--r--  2.0 unx     5755 b- defN 23-Mar-16 09:26 mpyl/reporting/targets/slack.py
--rw-r--r--  2.0 unx     5920 b- defN 23-Mar-16 09:26 mpyl/schema/mpyl_config.schema.yml
--rw-r--r--  2.0 unx    24999 b- defN 23-Mar-16 09:26 mpyl/schema/project.schema.yml
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-16 09:26 mpyl/stages/__init__.py
--rw-r--r--  2.0 unx     2408 b- defN 23-Mar-16 09:26 mpyl/stages/discovery.py
--rw-r--r--  2.0 unx     6135 b- defN 23-Mar-16 09:26 mpyl/steps/__init__.py
--rw-r--r--  2.0 unx     4839 b- defN 23-Mar-16 09:26 mpyl/steps/models.py
--rw-r--r--  2.0 unx     2166 b- defN 23-Mar-16 09:26 mpyl/steps/run.py
--rw-r--r--  2.0 unx     5815 b- defN 23-Mar-16 09:26 mpyl/steps/steps.py
--rw-r--r--  2.0 unx       59 b- defN 23-Mar-16 09:26 mpyl/steps/build/__init__.py
--rw-r--r--  2.0 unx     2255 b- defN 23-Mar-16 09:26 mpyl/steps/build/docker_after_build.py
--rw-r--r--  2.0 unx     2032 b- defN 23-Mar-16 09:26 mpyl/steps/build/dockerbuild.py
--rw-r--r--  2.0 unx      765 b- defN 23-Mar-16 09:26 mpyl/steps/build/echo.py
--rw-r--r--  2.0 unx     2402 b- defN 23-Mar-16 09:26 mpyl/steps/build/sbt.py
--rw-r--r--  2.0 unx       60 b- defN 23-Mar-16 09:26 mpyl/steps/deploy/__init__.py
--rw-r--r--  2.0 unx     1001 b- defN 23-Mar-16 09:26 mpyl/steps/deploy/echo.py
--rw-r--r--  2.0 unx      876 b- defN 23-Mar-16 09:26 mpyl/steps/deploy/kubernetes.py
--rw-r--r--  2.0 unx     1008 b- defN 23-Mar-16 09:26 mpyl/steps/deploy/kubernetes_job.py
--rw-r--r--  2.0 unx     1491 b- defN 23-Mar-16 09:26 mpyl/steps/deploy/k8s/__init__.py
--rw-r--r--  2.0 unx    13565 b- defN 23-Mar-16 09:26 mpyl/steps/deploy/k8s/chart.py
--rw-r--r--  2.0 unx     2097 b- defN 23-Mar-16 09:26 mpyl/steps/deploy/k8s/helm.py
--rw-r--r--  2.0 unx     1431 b- defN 23-Mar-16 09:26 mpyl/steps/deploy/k8s/rancher.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-16 09:26 mpyl/steps/deploy/k8s/resources/__init__.py
--rw-r--r--  2.0 unx     4418 b- defN 23-Mar-16 09:26 mpyl/steps/deploy/k8s/resources/crd.py
--rw-r--r--  2.0 unx     1330 b- defN 23-Mar-16 09:26 mpyl/steps/deploy/k8s/resources/customresources.py
--rw-r--r--  2.0 unx    11697 b- defN 23-Mar-16 09:26 mpyl/steps/deploy/k8s/resources/schema/traeffik.schema.yml
--rw-r--r--  2.0 unx       58 b- defN 23-Mar-16 09:26 mpyl/steps/test/__init__.py
--rw-r--r--  2.0 unx     1428 b- defN 23-Mar-16 09:26 mpyl/steps/test/after_test.py
--rw-r--r--  2.0 unx     2453 b- defN 23-Mar-16 09:26 mpyl/steps/test/before_test.py
--rw-r--r--  2.0 unx     2830 b- defN 23-Mar-16 09:26 mpyl/steps/test/dockertest.py
--rw-r--r--  2.0 unx      724 b- defN 23-Mar-16 09:26 mpyl/steps/test/echo.py
--rw-r--r--  2.0 unx     4669 b- defN 23-Mar-16 09:26 mpyl/steps/test/sbt.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-16 09:26 mpyl/utilities/__init__.py
--rw-r--r--  2.0 unx     3315 b- defN 23-Mar-16 09:26 mpyl/utilities/docker/__init__.py
--rw-r--r--  2.0 unx     1547 b- defN 23-Mar-16 09:26 mpyl/utilities/github/__init__.py
--rw-r--r--  2.0 unx     1542 b- defN 23-Mar-16 09:26 mpyl/utilities/jenkins/__init__.py
--rw-r--r--  2.0 unx     5016 b- defN 23-Mar-16 09:26 mpyl/utilities/jenkins/runner.py
--rw-r--r--  2.0 unx     1280 b- defN 23-Mar-16 09:26 mpyl/utilities/junit/__init__.py
--rw-r--r--  2.0 unx      754 b- defN 23-Mar-16 09:26 mpyl/utilities/pyaml_env/__init__.py
--rw-r--r--  2.0 unx     2708 b- defN 23-Mar-16 09:26 mpyl/utilities/repo/__init__.py
--rw-r--r--  2.0 unx     1520 b- defN 23-Mar-16 09:26 mpyl/utilities/sbt/__init__.py
--rw-r--r--  2.0 unx     1338 b- defN 23-Mar-16 09:26 mpyl/utilities/subprocess/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-16 09:27 mpyl-0.0.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     2914 b- defN 23-Mar-16 09:27 mpyl-0.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-16 09:27 mpyl-0.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       35 b- defN 23-Mar-16 09:27 mpyl-0.0.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Mar-16 09:27 mpyl-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5937 b- defN 23-Mar-16 09:27 mpyl-0.0.9.dist-info/RECORD
-70 files, 202066 bytes uncompressed, 64970 bytes compressed:  67.8%
+Zip file size: 126146 bytes, number of entries: 85
+-rw-r--r--  2.0 unx      766 b- defN 23-May-30 02:46 mpyl/__init__.py
+-rw-r--r--  2.0 unx      215 b- defN 23-May-30 02:46 mpyl/__main__.py
+-rw-r--r--  2.0 unx      129 b- defN 23-May-30 02:46 mpyl/constants.py
+-rw-r--r--  2.0 unx    12783 b- defN 23-May-30 02:46 mpyl/project.py
+-rw-r--r--  2.0 unx     1708 b- defN 23-May-30 02:46 mpyl/validation.py
+-rw-r--r--  2.0 unx     2138 b- defN 23-May-30 02:46 mpyl/cli/__init__.py
+-rw-r--r--  2.0 unx    10143 b- defN 23-May-30 02:46 mpyl/cli/build.py
+-rw-r--r--  2.0 unx      341 b- defN 23-May-30 02:46 mpyl/cli/health.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-May-30 02:46 mpyl/cli/meta_info.py
+-rw-r--r--  2.0 unx     3896 b- defN 23-May-30 02:46 mpyl/cli/projects.py
+-rw-r--r--  2.0 unx       34 b- defN 23-May-30 02:46 mpyl/cli/commands/__init__.py
+-rw-r--r--  2.0 unx       51 b- defN 23-May-30 02:46 mpyl/cli/commands/build/__init__.py
+-rw-r--r--  2.0 unx     3705 b- defN 23-May-30 02:46 mpyl/cli/commands/build/jenkins.py
+-rw-r--r--  2.0 unx     5565 b- defN 23-May-30 02:46 mpyl/cli/commands/build/mpyl.py
+-rw-r--r--  2.0 unx       38 b- defN 23-May-30 02:46 mpyl/cli/commands/health/__init__.py
+-rw-r--r--  2.0 unx     5090 b- defN 23-May-30 02:46 mpyl/cli/commands/health/checks.py
+-rw-r--r--  2.0 unx       46 b- defN 23-May-30 02:46 mpyl/cli/commands/projects/__init__.py
+-rw-r--r--  2.0 unx     1039 b- defN 23-May-30 02:46 mpyl/cli/commands/projects/formatting.py
+-rw-r--r--  2.0 unx      620 b- defN 23-May-30 02:46 mpyl/projects/__init__.py
+-rw-r--r--  2.0 unx     1993 b- defN 23-May-30 02:46 mpyl/projects/find.py
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 02:46 mpyl/reporting/__init__.py
+-rw-r--r--  2.0 unx       76 b- defN 23-May-30 02:46 mpyl/reporting/formatting/__init__.py
+-rw-r--r--  2.0 unx     3197 b- defN 23-May-30 02:46 mpyl/reporting/formatting/markdown.py
+-rw-r--r--  2.0 unx     1148 b- defN 23-May-30 02:46 mpyl/reporting/formatting/text.py
+-rw-r--r--  2.0 unx     1096 b- defN 23-May-30 02:46 mpyl/reporting/targets/__init__.py
+-rw-r--r--  2.0 unx     6735 b- defN 23-May-30 02:46 mpyl/reporting/targets/github.py
+-rw-r--r--  2.0 unx     8955 b- defN 23-May-30 02:46 mpyl/reporting/targets/jira.py
+-rw-r--r--  2.0 unx     7106 b- defN 23-May-30 02:46 mpyl/reporting/targets/slack.py
+-rw-r--r--  2.0 unx     7834 b- defN 23-May-30 02:46 mpyl/schema/mpyl_config.schema.yml
+-rw-r--r--  2.0 unx    25500 b- defN 23-May-30 02:46 mpyl/schema/project.schema.yml
+-rw-r--r--  2.0 unx     2954 b- defN 23-May-30 02:46 mpyl/schema/run_properties.schema.yml
+-rw-r--r--  2.0 unx        0 b- defN 23-May-30 02:46 mpyl/stages/__init__.py
+-rw-r--r--  2.0 unx     3439 b- defN 23-May-30 02:46 mpyl/stages/discovery.py
+-rw-r--r--  2.0 unx     6135 b- defN 23-May-30 02:46 mpyl/steps/__init__.py
+-rw-r--r--  2.0 unx     6103 b- defN 23-May-30 02:46 mpyl/steps/models.py
+-rw-r--r--  2.0 unx     3429 b- defN 23-May-30 02:46 mpyl/steps/run.py
+-rw-r--r--  2.0 unx     8800 b- defN 23-May-30 02:46 mpyl/steps/steps.py
+-rw-r--r--  2.0 unx       59 b- defN 23-May-30 02:46 mpyl/steps/build/__init__.py
+-rw-r--r--  2.0 unx     2093 b- defN 23-May-30 02:46 mpyl/steps/build/docker_after_build.py
+-rw-r--r--  2.0 unx     2221 b- defN 23-May-30 02:46 mpyl/steps/build/dockerbuild.py
+-rw-r--r--  2.0 unx      765 b- defN 23-May-30 02:46 mpyl/steps/build/echo.py
+-rw-r--r--  2.0 unx     2402 b- defN 23-May-30 02:46 mpyl/steps/build/sbt.py
+-rw-r--r--  2.0 unx       60 b- defN 23-May-30 02:46 mpyl/steps/deploy/__init__.py
+-rw-r--r--  2.0 unx     1001 b- defN 23-May-30 02:46 mpyl/steps/deploy/echo.py
+-rw-r--r--  2.0 unx     1310 b- defN 23-May-30 02:46 mpyl/steps/deploy/ephemeral_docker_deploy.py
+-rw-r--r--  2.0 unx     2432 b- defN 23-May-30 02:46 mpyl/steps/deploy/kubernetes.py
+-rw-r--r--  2.0 unx     1111 b- defN 23-May-30 02:46 mpyl/steps/deploy/kubernetes_job.py
+-rw-r--r--  2.0 unx     1118 b- defN 23-May-30 02:46 mpyl/steps/deploy/kubernetes_spark_job.py
+-rw-r--r--  2.0 unx     3341 b- defN 23-May-30 02:46 mpyl/steps/deploy/k8s/__init__.py
+-rw-r--r--  2.0 unx    18616 b- defN 23-May-30 02:46 mpyl/steps/deploy/k8s/chart.py
+-rw-r--r--  2.0 unx     2856 b- defN 23-May-30 02:46 mpyl/steps/deploy/k8s/helm.py
+-rw-r--r--  2.0 unx     1579 b- defN 23-May-30 02:46 mpyl/steps/deploy/k8s/rancher.py
+-rw-r--r--  2.0 unx     4467 b- defN 23-May-30 02:46 mpyl/steps/deploy/k8s/resources/__init__.py
+-rw-r--r--  2.0 unx      591 b- defN 23-May-30 02:46 mpyl/steps/deploy/k8s/resources/sealed_secret.py
+-rw-r--r--  2.0 unx     6143 b- defN 23-May-30 02:46 mpyl/steps/deploy/k8s/resources/spark.py
+-rw-r--r--  2.0 unx     1948 b- defN 23-May-30 02:46 mpyl/steps/deploy/k8s/resources/traefik.py
+-rw-r--r--  2.0 unx   168371 b- defN 23-May-30 02:46 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml
+-rw-r--r--  2.0 unx   151469 b- defN 23-May-30 02:46 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml
+-rw-r--r--  2.0 unx    11703 b- defN 23-May-30 02:46 mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml
+-rw-r--r--  2.0 unx    42950 b- defN 23-May-30 02:46 mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml
+-rw-r--r--  2.0 unx       64 b- defN 23-May-30 02:46 mpyl/steps/postdeploy/__init__.py
+-rw-r--r--  2.0 unx     2827 b- defN 23-May-30 02:46 mpyl/steps/postdeploy/cypress_test.py
+-rw-r--r--  2.0 unx       58 b- defN 23-May-30 02:46 mpyl/steps/test/__init__.py
+-rw-r--r--  2.0 unx     1428 b- defN 23-May-30 02:46 mpyl/steps/test/after_test.py
+-rw-r--r--  2.0 unx     2453 b- defN 23-May-30 02:46 mpyl/steps/test/before_test.py
+-rw-r--r--  2.0 unx     2830 b- defN 23-May-30 02:46 mpyl/steps/test/dockertest.py
+-rw-r--r--  2.0 unx     1657 b- defN 23-May-30 02:46 mpyl/steps/test/echo.py
+-rw-r--r--  2.0 unx     4885 b- defN 23-May-30 02:46 mpyl/steps/test/sbt.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-30 02:46 mpyl/utilities/__init__.py
+-rw-r--r--  2.0 unx      612 b- defN 23-May-30 02:46 mpyl/utilities/cypress/__init__.py
+-rw-r--r--  2.0 unx     4239 b- defN 23-May-30 02:46 mpyl/utilities/docker/__init__.py
+-rw-r--r--  2.0 unx     1739 b- defN 23-May-30 02:46 mpyl/utilities/github/__init__.py
+-rw-r--r--  2.0 unx     1533 b- defN 23-May-30 02:46 mpyl/utilities/jenkins/__init__.py
+-rw-r--r--  2.0 unx     6220 b- defN 23-May-30 02:46 mpyl/utilities/jenkins/runner.py
+-rw-r--r--  2.0 unx     1288 b- defN 23-May-30 02:46 mpyl/utilities/junit/__init__.py
+-rw-r--r--  2.0 unx      847 b- defN 23-May-30 02:46 mpyl/utilities/pyaml_env/__init__.py
+-rw-r--r--  2.0 unx     5708 b- defN 23-May-30 02:46 mpyl/utilities/repo/__init__.py
+-rw-r--r--  2.0 unx     1551 b- defN 23-May-30 02:46 mpyl/utilities/sbt/__init__.py
+-rw-r--r--  2.0 unx     2110 b- defN 23-May-30 02:46 mpyl/utilities/subprocess/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-30 02:47 mpyl-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5820 b- defN 23-May-30 02:47 mpyl-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 02:47 mpyl-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       35 b- defN 23-May-30 02:47 mpyl-1.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-May-30 02:47 mpyl-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7480 b- defN 23-May-30 02:47 mpyl-1.0.0.dist-info/RECORD
+85 files, 640513 bytes uncompressed, 114224 bytes compressed:  82.2%
```

## zipnote {}

```diff
@@ -1,44 +1,59 @@
 Filename: mpyl/__init__.py
 Comment: 
 
 Filename: mpyl/__main__.py
 Comment: 
 
+Filename: mpyl/constants.py
+Comment: 
+
 Filename: mpyl/project.py
 Comment: 
 
 Filename: mpyl/validation.py
 Comment: 
 
 Filename: mpyl/cli/__init__.py
 Comment: 
 
-Filename: mpyl/cli/build/__init__.py
+Filename: mpyl/cli/build.py
+Comment: 
+
+Filename: mpyl/cli/health.py
 Comment: 
 
-Filename: mpyl/cli/build/jenkins.py
+Filename: mpyl/cli/meta_info.py
 Comment: 
 
-Filename: mpyl/cli/build/mpyl.py
+Filename: mpyl/cli/projects.py
 Comment: 
 
 Filename: mpyl/cli/commands/__init__.py
 Comment: 
 
-Filename: mpyl/cli/commands/build.py
+Filename: mpyl/cli/commands/build/__init__.py
+Comment: 
+
+Filename: mpyl/cli/commands/build/jenkins.py
+Comment: 
+
+Filename: mpyl/cli/commands/build/mpyl.py
 Comment: 
 
-Filename: mpyl/cli/commands/meta_info.py
+Filename: mpyl/cli/commands/health/__init__.py
 Comment: 
 
-Filename: mpyl/cli/commands/projects.py
+Filename: mpyl/cli/commands/health/checks.py
 Comment: 
 
-Filename: mpyl/cli/projects/__init__.py
+Filename: mpyl/cli/commands/projects/__init__.py
+Comment: 
+
+Filename: mpyl/cli/commands/projects/formatting.py
 Comment: 
 
 Filename: mpyl/projects/__init__.py
 Comment: 
 
 Filename: mpyl/projects/find.py
 Comment: 
@@ -69,14 +84,17 @@
 
 Filename: mpyl/schema/mpyl_config.schema.yml
 Comment: 
 
 Filename: mpyl/schema/project.schema.yml
 Comment: 
 
+Filename: mpyl/schema/run_properties.schema.yml
+Comment: 
+
 Filename: mpyl/stages/__init__.py
 Comment: 
 
 Filename: mpyl/stages/discovery.py
 Comment: 
 
 Filename: mpyl/steps/__init__.py
@@ -108,20 +126,26 @@
 
 Filename: mpyl/steps/deploy/__init__.py
 Comment: 
 
 Filename: mpyl/steps/deploy/echo.py
 Comment: 
 
+Filename: mpyl/steps/deploy/ephemeral_docker_deploy.py
+Comment: 
+
 Filename: mpyl/steps/deploy/kubernetes.py
 Comment: 
 
 Filename: mpyl/steps/deploy/kubernetes_job.py
 Comment: 
 
+Filename: mpyl/steps/deploy/kubernetes_spark_job.py
+Comment: 
+
 Filename: mpyl/steps/deploy/k8s/__init__.py
 Comment: 
 
 Filename: mpyl/steps/deploy/k8s/chart.py
 Comment: 
 
 Filename: mpyl/steps/deploy/k8s/helm.py
@@ -129,21 +153,39 @@
 
 Filename: mpyl/steps/deploy/k8s/rancher.py
 Comment: 
 
 Filename: mpyl/steps/deploy/k8s/resources/__init__.py
 Comment: 
 
-Filename: mpyl/steps/deploy/k8s/resources/crd.py
+Filename: mpyl/steps/deploy/k8s/resources/sealed_secret.py
+Comment: 
+
+Filename: mpyl/steps/deploy/k8s/resources/spark.py
+Comment: 
+
+Filename: mpyl/steps/deploy/k8s/resources/traefik.py
+Comment: 
+
+Filename: mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml
 Comment: 
 
-Filename: mpyl/steps/deploy/k8s/resources/customresources.py
+Filename: mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml
 Comment: 
 
-Filename: mpyl/steps/deploy/k8s/resources/schema/traeffik.schema.yml
+Filename: mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml
+Comment: 
+
+Filename: mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml
+Comment: 
+
+Filename: mpyl/steps/postdeploy/__init__.py
+Comment: 
+
+Filename: mpyl/steps/postdeploy/cypress_test.py
 Comment: 
 
 Filename: mpyl/steps/test/__init__.py
 Comment: 
 
 Filename: mpyl/steps/test/after_test.py
 Comment: 
@@ -159,14 +201,17 @@
 
 Filename: mpyl/steps/test/sbt.py
 Comment: 
 
 Filename: mpyl/utilities/__init__.py
 Comment: 
 
+Filename: mpyl/utilities/cypress/__init__.py
+Comment: 
+
 Filename: mpyl/utilities/docker/__init__.py
 Comment: 
 
 Filename: mpyl/utilities/github/__init__.py
 Comment: 
 
 Filename: mpyl/utilities/jenkins/__init__.py
@@ -186,26 +231,26 @@
 
 Filename: mpyl/utilities/sbt/__init__.py
 Comment: 
 
 Filename: mpyl/utilities/subprocess/__init__.py
 Comment: 
 
-Filename: mpyl-0.0.9.dist-info/LICENSE
+Filename: mpyl-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: mpyl-0.0.9.dist-info/METADATA
+Filename: mpyl-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: mpyl-0.0.9.dist-info/WHEEL
+Filename: mpyl-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: mpyl-0.0.9.dist-info/entry_points.txt
+Filename: mpyl-1.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: mpyl-0.0.9.dist-info/top_level.txt
+Filename: mpyl-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mpyl-0.0.9.dist-info/RECORD
+Filename: mpyl-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mpyl/__init__.py

```diff
@@ -1,61 +1,31 @@
 """
 .. include:: ../../README.md
 
-## Technologies
-
-### Requirements
-The following technologies are expected to be present on the local OS:
- - [Python](https://www.python.org/) >= 3.9
- - [Pip](https://pypi.org/project/pip/) >= 23.0.1
- - [Pipenv](https://pypi.org/project/pipenv/) >= 2023.2.18
- - [Docker](https://www.docker.com/) > 20
- - [Docker compose](https://docs.docker.com/compose/install/linux/)
- installed as plugin (`docker compose version`) >= v2.2.3
- - [Git](https://git-scm.com/) SCM
-
-### Bundled
-MPyL is extensible and has a minimal footprint. Having said that, batteries for the following technologies are included.
-
-##### CI/CD
-###### Build
- - [Docker](https://www.docker.com/) `mpyl.steps.build.dockerbuild`
- - [Scala (SBT)](https://www.scala-sbt.org/) `mpyl.steps.build.sbt`
-
-###### Testing
- - [Junit](https://junit.org/) `mpyl.steps.models.ArtifactType.JUNIT_TESTS`
-
-###### Deployment
- - [K8S](https://kubernetes.io/) `mpyl.steps.deploy.kubernetes`
- - [Helm](https://helm.sh/) `mpyl.steps.deploy.k8s.helm`
-
-##### Reporting
- - [Jira](https://www.atlassian.com) `mpyl.reporting.targets.jira`
- - [Github](https://github.com/) `mpyl.reporting.targets.github`
- - [Slack](https://slack.com/) `mpyl.reporting.targets.slack`
-
 .. include:: ../../README-usage.md
 
 .. include:: ../../README-dev.md
 """
 
 import click
 
-from .cli.commands import get_version
-from .cli.commands.build import build
-from .cli.commands.meta_info import version
-from .cli.commands.projects import projects
+from .cli.build import build
+from .cli.health import health
+from .cli.meta_info import get_version
+from .cli.meta_info import version
+from .cli.projects import projects
 from .utilities.pyaml_env import parse_config
 from .utilities.repo import RepoConfig, Repository
 
 
 @click.group(name='mpyl')
 def main_group():
     """Command Line Interface for MPyL"""
 
 
 def main():
     main_group.help = f"Command Line Interface for MPyL {get_version()}"
     main_group.add_command(projects)
     main_group.add_command(build)
     main_group.add_command(version)
+    main_group.add_command(health)
     main_group()  # pylint: disable = no-value-for-parameter
```

## mpyl/project.py

```diff
@@ -27,14 +27,18 @@
 from ruamel.yaml import YAML
 
 from .validation import validate
 
 T = TypeVar('T')
 
 
+def without_keys(dictionary: dict, keys: set[str]):
+    return {k: dictionary[k] for k in dictionary.keys() - keys}
+
+
 @dataclass(frozen=True)
 class Target(Enum):
     def __eq__(self, other):
         return self.value == other.value
 
     PULL_REQUEST = 'PullRequest'
     PULL_REQUEST_BASE = 'PullRequestBase'
@@ -72,14 +76,16 @@
             return self.acceptance
         if target == Target.PRODUCTION:
             return self.production
         return None
 
     @staticmethod
     def from_config(values: dict):
+        if not values:
+            return None
         return TargetProperty(pr=values.get('pr'), test=values.get('test'), acceptance=values.get('acceptance'),
                               production=values.get('production'), all=values.get('all'))
 
 
 @dataclass(frozen=True)
 class KeyValueProperty(TargetProperty[str]):
     key: str
@@ -152,88 +158,98 @@
 @dataclass(frozen=True)
 class Probe:
     path: TargetProperty[str]
     values: dict
 
     @staticmethod
     def from_config(values: dict):
-        path = values['path']
-        return Probe(path=TargetProperty.from_config(path), values=values)
+        if not values:
+            return None
+        return Probe(path=TargetProperty.from_config(values['path']), values=values)
 
 
 @dataclass(frozen=True)
 class Metrics:
     path: str
     enabled: bool
 
     @staticmethod
     def from_config(values: dict):
+        if not values:
+            return None
         return Metrics(path=values.get('path', '/metrics'), enabled=values.get('enabled', False))
 
 
 @dataclass(frozen=True)
 class Resources:
     instances: Optional[TargetProperty[int]]
     cpus: Optional[TargetProperty[float]]
     mem: Optional[TargetProperty[int]]
     disk: Optional[TargetProperty[int]]
 
     @staticmethod
     def from_config(values: dict):
-        instances = values.get('instances')
         limits = values.get('limit', {})
-        cpus = limits.get('cpus')
-        mem = limits.get('mem')
-        disk = limits.get('disk')
-        return Resources(instances=TargetProperty.from_config(instances) if instances else None,
-                         cpus=TargetProperty.from_config(cpus) if cpus else None,
-                         mem=TargetProperty.from_config(mem) if mem else None,
-                         disk=TargetProperty.from_config(disk) if disk else None)
+        return Resources(
+            instances=TargetProperty.from_config(limits.get('instances', {})),
+            cpus=TargetProperty.from_config(limits.get('cpus', {})),
+            mem=TargetProperty.from_config(limits.get('mem', {})),
+            disk=TargetProperty.from_config(limits.get('disk', {}))
+        )
+
+
+@dataclass(frozen=True)
+class Job:
+    cron: dict
+    job: dict
+    spark: dict
+
+    @staticmethod
+    def from_config(values: dict):
+        if not values:
+            return None
+        return Job(cron=values.get('cron', {}), job=without_keys(values, {'cron'}), spark=values.get('spark', {}))
 
 
 @dataclass(frozen=True)
 class Kubernetes:
     port_mappings: dict[int, int]
     liveness_probe: Optional[Probe]
     startup_probe: Optional[Probe]
     metrics: Optional[Metrics]
     resources: Resources
-    cron: dict
+    job: Optional[Job]
 
     @staticmethod
     def from_config(values: dict):
-        mappings = values.get('portMappings')
-        liveness_probe = values.get('livenessProbe')
-        startup_probe = values.get('startupProbe')
-        metrics = values.get('metrics', None)
-        resources = values.get('resources')
         return Kubernetes(
-            port_mappings=mappings if mappings else {},
-            liveness_probe=Probe.from_config(liveness_probe) if liveness_probe else None,
-            startup_probe=Probe.from_config(startup_probe) if startup_probe else None,
-            metrics=Metrics.from_config(metrics) if metrics else None,
-            resources=Resources.from_config(resources) if resources else None,
-            cron=values.get('cron', {})
+            port_mappings=values.get('portMappings', {}),
+            liveness_probe=Probe.from_config(values.get('livenessProbe', {})),
+            startup_probe=Probe.from_config(values.get('startupProbe', {})),
+            metrics=Metrics.from_config(values.get('metrics', {})),
+            resources=Resources.from_config(values.get('resources', {})),
+            job=Job.from_config(values.get('job', {}))
         )
 
 
 @dataclass(frozen=True)
 class Host:
     host: TargetProperty[str]
+    service_port: Optional[int]
     tls: TargetProperty[str]
     whitelists: TargetProperty[list[str]]
 
     @staticmethod
     def from_config(values: dict):
-        host = values.get('host')
-        tls = values.get('tls')
-        whitelists = values.get('whitelists')
-        return Host(host=TargetProperty.from_config(host) if host else None,
-                    tls=TargetProperty.from_config(tls) if tls else None,
-                    whitelists=TargetProperty.from_config(whitelists) if whitelists else None)
+        return Host(
+            host=TargetProperty.from_config(values.get('host', {})),
+            service_port=values.get('servicePort'),
+            tls=TargetProperty.from_config(values.get('tls', {})),
+            whitelists=TargetProperty.from_config(values.get('whitelists', {}))
+        )
 
 
 @dataclass(frozen=True)
 class Traefik:
     hosts: list[Host]
 
     @staticmethod
@@ -250,21 +266,28 @@
     traefik: Optional[Traefik]
 
     @staticmethod
     def from_config(values: dict):
         props = values.get('properties')
         kubernetes = values.get('kubernetes')
         traefik = values.get('traefik')
+
         return Deployment(namespace=values.get('namespace'),
                           properties=Properties.from_config(props) if props else None,
                           kubernetes=Kubernetes.from_config(kubernetes) if kubernetes else None,
                           traefik=Traefik.from_config(traefik) if traefik else None)
 
 
 @dataclass(frozen=True)
+class ProjectName:
+    name: str
+    namespace: Optional[str]
+
+
+@dataclass(frozen=True)
 class Project:
     name: str
     description: str
     path: str
     stages: Stages
     maintainer: list[str]
     deployment: Optional[Deployment]
@@ -276,19 +299,36 @@
     def __eq__(self, other):
         return self.path == other.path
 
     def __hash__(self):
         return hash(self.path)
 
     @property
+    def to_name(self) -> ProjectName:
+        return ProjectName(
+            name=self.name,
+            namespace=self.deployment.namespace if self.deployment and self.deployment.namespace else None
+        )
+
+    @property
     def kubernetes(self) -> Kubernetes:
         if self.deployment is None or self.deployment.kubernetes is None:
-            raise AttributeError(f"Project '{self.name}' does not have kubernetes configuration")
+            raise KeyError(f"Project '{self.name}' does not have kubernetes configuration")
         return self.deployment.kubernetes
 
+    @property
+    def resources(self) -> Resources:
+        return self.kubernetes.resources
+
+    @property
+    def job(self) -> Job:
+        if self.kubernetes.job is None:
+            raise KeyError(f"Project '{self.name}' does not have kubernetes.job configuration")
+        return self.kubernetes.job
+
     @staticmethod
     def project_yaml_path() -> str:
         return 'deployment/project.yml'
 
     @property
     def root_path(self) -> str:
         return self.path.replace(Project.project_yaml_path(), '')
@@ -355,7 +395,21 @@
         except TypeError:
             traceback.print_exc()
             logging.warning('Type error', exc_info=True)
             raise
         except Exception:
             logging.warning(f'Failed to load {project_path}', exc_info=True)
             raise
+
+
+def get_env_variables(project: Project, target: Target) -> dict[str, str]:
+    if project.deployment is None:
+        raise KeyError(f'No deployment information was found for project: {project.name}')
+    if len(project.deployment.properties.env) == 0:
+        raise KeyError(f'No properties.env is defined for project: {project.name}')
+
+    env_variables: dict[str, str] = {
+        env_variable.key: env_variable.get_value(target) for env_variable in
+        project.deployment.properties.env
+    }
+
+    return env_variables
```

## mpyl/validation.py

```diff
@@ -1,14 +1,14 @@
 """ Function used to validate the project.schema.yml against the local schema."""
 
 import pkgutil
 from functools import lru_cache
 
 import jsonschema
-from jsonschema import RefResolver, Draft7Validator
+from jsonschema import RefResolver, Draft7Validator, validators
 from ruamel.yaml import YAML
 
 yaml = YAML()
 
 
 @lru_cache(maxsize=10)
 def load_schema(schema_string: str) -> Draft7Validator:
@@ -21,13 +21,28 @@
 
     def load_schema_from_local(uri):
         if 'project.schema.yml' in uri:
             return project_schema
         return {}
 
     resolver = RefResolver(referrer=schema, base_uri="", handlers={"": load_schema_from_local})
-    return jsonschema.validators.Draft7Validator(schema=schema, resolver=resolver)
+    all_validators = dict(Draft7Validator.VALIDATORS)
+    existing_validator = all_validators['type']
+
+    def allow_none_validator(validator, types, instance, yaml_schema):
+        for field_type in types:
+            if field_type is None and instance is None:
+                return None
+
+        return existing_validator(validator, types, instance, yaml_schema)
+
+    all_validators['type'] = allow_none_validator
+    type_checker = Draft7Validator.TYPE_CHECKER
+
+    extended_validator = validators.extend(jsonschema.validators.Draft7Validator, validators=all_validators,
+                                           type_checker=type_checker)
+    return extended_validator(schema=schema, resolver=resolver)
 
 
 def validate(values: dict, schema_string: str):
     schema = load_schema(schema_string)
     return schema.validate(values)
```

## mpyl/cli/__init__.py

```diff
@@ -1,17 +1,72 @@
-"""Command Line Interface for MPyL"""
+"""Command Line Interface parsing for MPyL"""
+import asyncio
+import importlib
 import logging
+from dataclasses import dataclass
+from importlib.metadata import version as version_meta
+from typing import Optional
+
+import aiohttp
+import requests
+from aiohttp import ClientConnectorError, ClientTimeout
 
 from rich.console import Console
 from rich.logging import RichHandler
 
+from ..utilities.repo import Repository
+
+CONFIG_PATH_HELP = 'Path to the config.yml. Needs to comply with schema at ' \
+                   'https://vandebron.github.io/mpyl/schema/mpyl_config.schema.yml ' \
+                   'Can be set via `MPYL_CONFIG_PATH` env var. '
+
+
+@dataclass(frozen=True)
+class CliContext:
+    config: dict
+    repo: Repository
+    console: Console
+    verbose: bool
+
+
+async def fetch_latest_version() -> Optional[str]:
+    try:
+        async with aiohttp.ClientSession(timeout=ClientTimeout(total=10)) as session:
+            async with session.get("https://pypi.org/pypi/mpyl/json") as response:
+                body = await response.json()
+                return body.get('info', {}).get('version')
+    except (asyncio.exceptions.TimeoutError, ClientConnectorError, requests.exceptions.RequestException):
+        return None
+
+
+def get_meta_version():
+    try:
+        return version_meta('mpyl')
+    except importlib.metadata.PackageNotFoundError:
+        return None
+
+
+async def check_updates(meta: str) -> Optional[str]:
+    latest = await fetch_latest_version()
+    if latest and meta != latest:
+        return latest
+    return None
+
+
+def get_version():
+    try:
+        return f"v{version_meta('mpyl')}"
+    except importlib.metadata.PackageNotFoundError:
+        return '(local)'
+
+
 FORMAT = "%(message)s"
 
 
 def create_console_logger(local: bool, verbose: bool) -> Console:
-    console = Console(markup=True, width=None if local else 135, no_color=False, log_path=False, color_system='256')
+    console = Console(markup=True, width=None if local else 135, no_color=False, log_path=False, log_time=False,
+                      color_system='256')
     logging.basicConfig(
         level="DEBUG" if verbose else "INFO", format=FORMAT, datefmt="[%X]",
-        handlers=[RichHandler(markup=True,
-                              console=console, show_path=local)]
+        handlers=[RichHandler(markup=True, console=console, show_path=local)]
     )
     return console
```

## mpyl/cli/commands/__init__.py

```diff
@@ -1,23 +1 @@
-"""CLI commands"""
-import importlib
-from dataclasses import dataclass
-from importlib.metadata import version as version_meta
-
-from rich.console import Console
-
-from ...utilities.repo import Repository
-
-
-@dataclass(frozen=True)
-class CliContext:
-    config: dict
-    repo: Repository
-    console: Console
-    verbose: bool
-
-
-def get_version():
-    try:
-        return f"v{version_meta('mpyl')}"
-    except importlib.metadata.PackageNotFoundError:
-        return '(local)'
+"""CLI command implementations"""
```

## mpyl/projects/__init__.py

```diff
@@ -0,0 +1,39 @@
+00000000: 2222 2250 726f 6a65 6374 7320 616e 6420  """Projects and 
+00000010: 686f 7720 7468 6579 2072 656c 6174 6520  how they relate 
+00000020: 746f 2065 6163 6820 6f74 6865 7222 2222  to each other"""
+00000030: 0a66 726f 6d20 6461 7461 636c 6173 7365  .from dataclasse
+00000040: 7320 696d 706f 7274 2064 6174 6163 6c61  s import datacla
+00000050: 7373 0a66 726f 6d20 656e 756d 2069 6d70  ss.from enum imp
+00000060: 6f72 7420 456e 756d 0a66 726f 6d20 7479  ort Enum.from ty
+00000070: 7069 6e67 2069 6d70 6f72 7420 4f70 7469  ping import Opti
+00000080: 6f6e 616c 0a0a 6672 6f6d 202e 2e70 726f  onal..from ..pro
+00000090: 6a65 6374 2069 6d70 6f72 7420 5072 6f6a  ject import Proj
+000000a0: 6563 740a 0a0a 4064 6174 6163 6c61 7373  ect...@dataclass
+000000b0: 2866 726f 7a65 6e3d 5472 7565 290a 636c  (frozen=True).cl
+000000c0: 6173 7320 5072 6f74 6f63 6f6c 2845 6e75  ass Protocol(Enu
+000000d0: 6d29 3a0a 2020 2020 554e 4b4e 4f57 4e20  m):.    UNKNOWN 
+000000e0: 3d20 310a 2020 2020 5245 5354 203d 2032  = 1.    REST = 2
+000000f0: 0a20 2020 204b 4146 4b41 203d 2033 0a0a  .    KAFKA = 3..
+00000100: 0a40 6461 7461 636c 6173 7328 6672 6f7a  .@dataclass(froz
+00000110: 656e 3d54 7275 6529 0a63 6c61 7373 2043  en=True).class C
+00000120: 6f6e 7472 6163 743a 0a20 2020 2074 7970  ontract:.    typ
+00000130: 653a 2050 726f 746f 636f 6c0a 2020 2020  e: Protocol.    
+00000140: 636f 6e74 7261 6374 5f66 696c 653a 204f  contract_file: O
+00000150: 7074 696f 6e61 6c5b 7374 725d 0a0a 0a40  ptional[str]...@
+00000160: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
+00000170: 3d54 7275 6529 0a63 6c61 7373 2044 6570  =True).class Dep
+00000180: 656e 6465 6e63 793a 0a20 2020 2070 726f  endency:.    pro
+00000190: 6a65 6374 3a20 5072 6f6a 6563 740a 2020  ject: Project.  
+000001a0: 2020 636f 6e74 7261 6374 733a 2073 6574    contracts: set
+000001b0: 5b43 6f6e 7472 6163 745d 0a0a 0a40 6461  [Contract]...@da
+000001c0: 7461 636c 6173 730a 636c 6173 7320 5072  taclass.class Pr
+000001d0: 6f6a 6563 7457 6974 6844 6570 656e 6465  ojectWithDepende
+000001e0: 6e74 733a 0a20 2020 2070 726f 6a65 6374  nts:.    project
+000001f0: 3a20 5072 6f6a 6563 740a 2020 2020 6465  : Project.    de
+00000200: 7065 6e64 656e 745f 7072 6f6a 6563 7473  pendent_projects
+00000210: 3a20 6469 6374 5b73 7472 2c20 4465 7065  : dict[str, Depe
+00000220: 6e64 656e 6379 5d0a 0a20 2020 2040 7072  ndency]..    @pr
+00000230: 6f70 6572 7479 0a20 2020 2064 6566 206e  operty.    def n
+00000240: 616d 6528 7365 6c66 293a 0a20 2020 2020  ame(self):.     
+00000250: 2020 2072 6574 7572 6e20 7365 6c66 2e70     return self.p
+00000260: 726f 6a65 6374 2e6e 616d 650a            roject.name.
```

## mpyl/projects/find.py

```diff
@@ -1,8 +1,43 @@
 """ Loads all projects inside a repository. """
 from pathlib import Path
+from typing import Optional
 
-from ..project import Project, load_project
+from . import ProjectWithDependents, Protocol, Contract, Dependency
+from ..project import Project, load_project, Stage
 
 
-def load_projects(root_dir: Path, paths: set[str]) -> set[Project]:
-    return set(map(lambda p: load_project(root_dir, Path(p), False), paths))
+def load_projects(root_dir: Path, paths: list[str], strict: bool = False) -> set[Project]:
+    return set(map(lambda p: load_project(root_dir, Path(p), strict), paths))
+
+
+def find_by_contract_dep(dep: str, projects: list[ProjectWithDependents]) -> Optional[ProjectWithDependents]:
+    for project in projects:
+        if project.project.root_path.replace('./', '') in dep:
+            return project
+    return None
+
+
+def find_dependencies(project: Project, other_projects: set[Project]) -> ProjectWithDependents:
+    mapped = list(map(lambda p: ProjectWithDependents(p, {}), other_projects))
+
+    def recursively_find(proj: ProjectWithDependents, other: list[ProjectWithDependents], discovery_stack: list[str]):
+        dependent_projects = {}
+        for dep in proj.project.dependencies.set_for_stage(Stage.TEST) if proj.project.dependencies else set():
+            found = find_by_contract_dep(dep, other)
+            if found:
+                if found.name not in discovery_stack:
+                    discovery_stack.append(found.name)
+                    recursively_find(found, other, discovery_stack[:])
+                    dependent_projects[found.name] = Dependency(found.project, {Contract(Protocol.UNKNOWN, dep)})
+                elif found.name in dependent_projects:
+                    dependent_projects[found.name].contracts.add(Contract(Protocol.UNKNOWN, dep))
+
+        proj.dependent_projects = dependent_projects
+        return proj
+
+    return recursively_find(ProjectWithDependents(project=project, dependent_projects={}), mapped, [])
+
+
+def find_all_dependencies(root_dir: Path, paths: list[str]) -> list[ProjectWithDependents]:
+    projects = load_projects(root_dir, paths)
+    return list(map(lambda p: find_dependencies(p, projects), projects))
```

## mpyl/reporting/formatting/markdown.py

```diff
@@ -1,73 +1,96 @@
 """
 Markdown run result formatters
 """
-import itertools
+import operator
 
 from junitparser import TestSuite
 
 from ...project import Stage, Project
-from ...steps.models import ArtifactType
+from ...steps import Output, ArtifactType
 from ...steps.run import RunResult
-from ...steps.steps import StepResult
-from ...utilities.junit import TestRunSummary, to_test_suites, sum_suites
+from ...steps.steps import StepResult, collect_test_results
+from ...utilities.junit import TestRunSummary, sum_suites
 
 
 def summary_to_markdown(summary: TestRunSummary):
-    return f":test_tube: {summary.tests} :x: {summary.failures} " \
-           f":broken_heart: {summary.errors} :see_no_evil: {summary.skipped}"
+    return f"🧪 {summary.tests} ❌ {summary.failures} " \
+           f"💔 {summary.errors} 🙈 {summary.skipped}"
+
+
+def __add_link_if_service(name: str, output: Output) -> str:
+    if output.produced_artifact and output.produced_artifact.artifact_type == ArtifactType.DEPLOYED_HELM_APP:
+        url = output.produced_artifact.spec.get('url')
+        if url:
+            return f'[{name}]({url})'
+
+    return name
+
+
+def wrap_project_name(proj: Project, result: list[StepResult]):
+    project_name = proj.name
+    encapsulation = '_'
+    found_result = next((r for r in result if r.project.name == project_name), None)
+    if found_result:
+        project_name = __add_link_if_service(project_name, found_result.output)
+        encapsulation = '*' if found_result.output.success else '~~'
+
+    return f'{encapsulation}{project_name}{encapsulation}'
 
 
 def __to_oneliner(result: list[StepResult], plan: set[Project]) -> str:
     project_names: list[str] = []
     if plan:
-        for proj in plan:
-            found_result = next((r for r in result if r.project.name == proj.name), None)
-            if found_result:
-                project_names.append(f'*{proj.name}*' if found_result.output.success else f'~~{proj.name}~~')
-            else:
-                project_names.append(f'_{proj.name}_')
+        sorted_plan = sorted(plan, key=operator.attrgetter('name'))
+        for proj in sorted_plan:
+            project_names.append(wrap_project_name(proj, result))
     else:
         project_names = list(map(lambda r: f'_{r.project.name}_', result))
 
-    return f'{", ".join(sorted(project_names))}'
-
-
-def __collect_test_results(step_results: list[StepResult]) -> list[TestSuite]:
-    test_artifacts = [res.output.produced_artifact for res in step_results if
-                      (res.output.produced_artifact and
-                       res.output.produced_artifact.artifact_type == ArtifactType.JUNIT_TESTS)]
-
-    suites: list[list[TestSuite]] = list(map(to_test_suites, test_artifacts))
-    flattened = list(itertools.chain(*suites))
-    return flattened
+    return f'{", ".join(project_names)}'
 
 
 def stage_to_icon(stage: Stage):
     if stage == Stage.BUILD:
         return '🏗️ '
     if stage == Stage.TEST:
         return '🧪'
     if stage == Stage.DEPLOY:
         return '🚀'
     return '➡️'
 
 
+def markdown_for_stage(run_result: RunResult, stage: Stage):
+    step_results: list[StepResult] = run_result.results_for_stage(stage)
+    plan: set[Project] = run_result.plan_for_stage(stage)
+    if not step_results and not plan:
+        return ''
+
+    result = f"{stage_to_icon(stage)}  {__to_oneliner(step_results, plan)}  \n"
+    test_results = collect_test_results(step_results)
+    if test_results:
+        result += to_markdown_test_report(
+            test_results) + f' [link]({run_result.run_properties.details.tests_url}) \n'
+
+    return result
+
+
 def run_result_to_markdown(run_result: RunResult) -> str:
-    result: str = f'❗Exception: \n```\n{run_result.exception}\n```\n' if run_result.exception else ""
+    result: str = f'{run_result.status_line}  \n'
+    exception = run_result.exception
+    if exception:
+        result += f"For _{exception.executor}_ on _{exception.project_name}_ at _{exception.stage}_ \n"
+        result += f"\n```\n{exception}\n```\n"
+    elif run_result.failed_result:
+        failed = run_result.failed_result
+        result += f"For _{failed.project.name}_ at _{failed.stage}_ \n"
+        result += f"\n```\n{run_result.failed_result.output.message}\n```\n"
 
     for stage in Stage:
-        step_results: list[StepResult] = run_result.results_for_stage(stage)
-        plan: set[Project] = run_result.plan_for_stage(stage)
-        if step_results or plan:
-            result += f"{stage_to_icon(stage)}  {__to_oneliner(step_results, plan)}  \n"
-            test_results = __collect_test_results(step_results)
-            if test_results:
-                result += to_markdown_test_report(
-                    test_results) + f' [link]({run_result.run_properties.details.tests_url}) \n'
+        result += markdown_for_stage(run_result, stage)
 
     return result
 
 
 def to_markdown_test_report(suites: list[TestSuite]):
     total_tests = sum_suites(suites)
     return f"{summary_to_markdown(total_tests)}"
```

## mpyl/reporting/targets/__init__.py

```diff
@@ -3,16 +3,39 @@
 To create a new reporter, implement `Reporter.send_report`.
 You can transform `mpyl.steps.run.RunResult` to a report using any of the standard formatters under
 `mpyl.reporting.formatting` and send it to target of your choice.
 
 See the **Submodules** for built-in reporters.
 """
 from abc import abstractmethod
+from dataclasses import dataclass
+from typing import Optional
 
 from ...steps.run import RunResult
 
 
+@dataclass(frozen=True)
+class ReportOutcome:
+    success: bool
+    exception: Optional[Exception] = None
+
+
+class ReportAccumulator:
+    outcomes: list[ReportOutcome]
+
+    def __init__(self):
+        self.outcomes = []
+
+    def add(self, outcome: ReportOutcome):
+        self.outcomes.append(outcome)
+
+    @property
+    def failures(self) -> list[str]:
+        return [f'{type(outcome).__name__} failed with exception {outcome.exception}' for outcome in self.outcomes if
+                not outcome.success]
+
+
 class Reporter:
 
     @abstractmethod
-    def send_report(self, results: RunResult) -> None:
+    def send_report(self, results: RunResult, text: Optional[str] = None) -> ReportOutcome:
         pass
```

## mpyl/reporting/targets/github.py

```diff
@@ -27,100 +27,122 @@
  2. Go to your repository's *Setting* -> *Integrations* -> *Github Apps* and click **Configure** for*_MPyL Pipeline*
  3. In the app's settings page, scroll down and click **Generate a private key**
  4. The private key needs to be made available at the location configured in `csv.targets.app.privateKeyPath` at
   runtime.
 
 """
 import base64
+import typing
 from datetime import datetime
 from logging import Logger
 from pathlib import Path
 from typing import Dict, Optional
 
-from github import Github, GithubIntegration
+from github import Github, GithubIntegration, GithubException
 from github.IssueComment import IssueComment
+from github.PullRequest import PullRequest
 from github.Repository import Repository as GithubRepository
 
-from . import Reporter
+from . import Reporter, ReportOutcome
 from ...reporting.formatting.markdown import run_result_to_markdown
 from ...reporting.formatting.text import to_string
 from ...steps.models import RunProperties
 from ...steps.run import RunResult
-from ...utilities.github import GithubConfig, get_pr_for_branch
+from ...utilities.github import GithubConfig, get_pr_for_branch, GithubAppConfig
 from ...utilities.repo import Repository, RepoConfig
 
 
+def compose_message_body(results: RunResult, _unused_config: Optional[Dict] = None) -> str:
+    return run_result_to_markdown(results)
+
+
+class GithubOutcome(ReportOutcome):
+    pass
+
+
 class PullRequestComment(Reporter):
     _config: GithubConfig
 
-    def __init__(self, config: Dict):
-        self._config = GithubConfig(config)
-        self.git_repository = Repository(RepoConfig(config))
+    def __init__(self, config: Dict,
+                 compose_function: typing.Callable[[RunResult, Optional[Dict]], str] = compose_message_body):
+        self._raw_config = config
+        self._config = GithubConfig.from_config(config)
+        self.git_repository = Repository(RepoConfig.from_config(config))
+        self.compose_function = compose_function
 
-    def _get_pull_request(self, repo: GithubRepository, run_properties: RunProperties):
+    def _get_pull_request(self, repo: GithubRepository, run_properties: RunProperties) -> Optional[PullRequest]:
         if run_properties.versioning.pr_number:
             return repo.get_pull(run_properties.versioning.pr_number)
 
         current_branch = self.git_repository.get_branch
-        return get_pr_for_branch(repo, current_branch)
+        if current_branch:
+            return get_pr_for_branch(repo, current_branch)
+        return None
 
-    def send_report(self, results: RunResult) -> None:
-        github = Github(self._config.token)
-        repo = github.get_repo(self._config.repository)
-
-        pull_request = self._get_pull_request(repo, results.run_properties)
-
-        comments = pull_request.get_issue_comments()
-        authenticated_user = github.get_user()
-        comments_for_user = [c for c in comments if c.user.id == authenticated_user.id]
-        if comments_for_user:
-            comment_to_update: IssueComment = comments_for_user.pop()
-            comment_to_update.edit(run_result_to_markdown(results))
-        else:
-            pull_request.create_issue_comment(run_result_to_markdown(results))
+    def send_report(self, results: RunResult, text: Optional[str] = None) -> GithubOutcome:
+        try:
+            github = Github(self._config.token)
+            repo = github.get_repo(self._config.repository)
+
+            pull_request = self._get_pull_request(repo, results.run_properties)
+            if not pull_request:
+                return GithubOutcome(success=False, exception=Exception('No pull request found'))
+
+            comments = pull_request.get_issue_comments()
+            authenticated_user = github.get_user()
+            comments_for_user = [c for c in comments if c.user.id == authenticated_user.id]
+            if comments_for_user:
+                comment_to_update: IssueComment = comments_for_user.pop()
+                comment_to_update.edit(self.compose_function(results, self._raw_config))
+            else:
+                pull_request.create_issue_comment(self.compose_function(results, self._raw_config))
+            return GithubOutcome(success=True)
+        except GithubException as exc:
+            return GithubOutcome(success=False, exception=exc)
 
 
 class CommitCheck(Reporter):
     _github_config: GithubConfig
     _check_run_id: Optional[int]
 
     def __init__(self, config: Dict, logger: Logger):
         self._config = config
-        self._github_config = GithubConfig(config)
+        self._github_config = GithubConfig.from_config(config)
         self._check_run_id = None
         self._logger = logger
 
     @staticmethod
     def _to_output(results: RunResult) -> dict:
         build_id = results.run_properties.details.build_id
         summary = ':white_check_mark: Build successful' if results.is_success else ':x: Build failed'
         return {'title': f'Build {build_id}', 'summary': summary + '\n' + run_result_to_markdown(results),
                 'text': to_string(results)}
 
-    def send_report(self, results: RunResult) -> None:
+    def send_report(self, results: RunResult, text: Optional[str] = None) -> GithubOutcome:
         try:
-            config = self._github_config.app_config
+            config: GithubAppConfig = self._github_config.get_app_config
             if not config:
                 raise KeyError("github.app config needs to be defined")
 
             private_key = Path(config.private_app_key_path or '').read_text(
                 encoding='utf-8') if config.private_app_key_path else base64.b64decode(
                 config.private_key_base_64_encoded or '').decode('utf-8')
 
             integration = GithubIntegration(integration_id=config.app_key, private_key=private_key)
 
             install = integration.get_installation(self._github_config.owner, self._github_config.repo_name)
             access_token = integration.get_access_token(install.id)
             github = Github(login_or_token=access_token.token)
             repo = github.get_repo(self._github_config.repository)
-            if self._check_run_id:
+            if self._check_run_id and results:
                 run = repo.get_check_run(self._check_run_id)
-                conclusion = 'success' if results.is_success else 'failure'
+                conclusion = 'success' if results is None or results.is_success else 'failure'
                 self._logger.info(f'Setting check to {conclusion}')
                 run.edit(completed_at=datetime.now(), conclusion=conclusion, output=self._to_output(results))
             else:
-                with Repository(RepoConfig(self._config)) as git_repository:
+                with Repository(RepoConfig.from_config(self._config)) as git_repository:
                     self._check_run_id = repo.create_check_run(name='Pipeline build', head_sha=git_repository.get_sha,
                                                                status='in_progress').id
-        except Exception as exc:
+            return GithubOutcome(success=True)
+        except GithubException as exc:
             self._logger.warning(f'Unexpected exception: {exc}', exc_info=True)
-            raise exc
+            return GithubOutcome(success=False, exception=exc)
```

## mpyl/reporting/targets/jira.py

```diff
@@ -1,112 +1,204 @@
 """
 Jira result reporter.
 
 ### Usage
 
 To determine which `Jira` ticket a pipeline run relates to, the branch is parsed.
-The following pattern is assumed `[A-Za-z]{3}-\\d+` to signify the Jira ticket key.
+The following pattern is assumed unless otherwise specified: `[A-Za-z]{3,}-` to signify the Jira ticket key.
 If a Jira ticket key cannot be extracted from the branch, this reporter will fail silently.
 
 ### Actions
  - If the ticket is still in its initial stage, it transitioned to the following stage. For example:
 `To Do` -> `In progress`
  - If the ticket hasn't been assigned to any particular person, it will be assigned to whoever triggered
  the pipeline run.
 
 ### Configuration
 Configure hostname and credentials under `jira` in the `config.yml`
+
+.. note:: Use API token as password
+   You need to create a regular Jira account to represent the MPyL system integration.
+   The username is the email address of the account. Log in as this user and create an
+   [API token](https://id.atlassian.com/manage-profile/security/api-tokens) to be used as the password.
 """
 import re
 from dataclasses import dataclass
 from logging import Logger
+from re import Pattern
 from typing import Optional
+from urllib.parse import urlsplit
 
+import requests
 from atlassian import Jira
 
-from . import Reporter
+from . import Reporter, ReportOutcome
+from ..formatting.markdown import markdown_for_stage
+from ...constants import DEFAULT_CONFIG_FILE_NAME
+from ...project import Stage
 from ...steps.run import RunResult
 
 
 @dataclass(frozen=True)
 class JiraTicket:
+    jira_url: str
     ticket_id: str
+    ticket_url: str
     issue_type: str
     summary: str
     description: str
     status_name: str
     user_avatar: str
     user_email: str
     assignee_email: Optional[str]
 
     @staticmethod
     def from_issue_response(response):
+        jira_url = "{uri.scheme}://{uri.netloc}".format(uri=urlsplit(response['self']))
         fields = response['fields']
+        ticket_id = response['key']
         assignee = fields.get('assignee')
         user = assignee or fields.get('reporter') or fields.get('creator')
-        avatar = user['avatarUrls']['48x48'] if user else ''
+        avatar = user['avatarUrls']['24x24'] if user else ''
         status_name = fields['status']['name']
         assignee_email = assignee['emailAddress'] if assignee else None
+        ticket_url = f"{jira_url}/browse/{ticket_id}"
 
-        return JiraTicket(ticket_id=response['key'], issue_type=fields['issuetype']['name'], summary=fields['summary'],
-                          status_name=status_name, description=fields['description'], user_avatar=avatar,
-                          user_email=user['emailAddress'], assignee_email=assignee_email)
+        return JiraTicket(jira_url=jira_url, ticket_id=ticket_id, ticket_url=ticket_url,
+                          issue_type=fields['issuetype']['name'], summary=fields['summary'], status_name=status_name,
+                          description=fields['description'], user_avatar=avatar, user_email=user['emailAddress'],
+                          assignee_email=assignee_email)
 
 
-def extract_ticket_from_branch(branch: str) -> Optional[str]:
-    pattern = r'[A-Za-z]{3}-\d+'
+def extract_ticket_from_branch(branch: str, pattern: Pattern) -> Optional[str]:
     ticket: Optional[str] = next(iter(re.findall(pattern, branch)), None)
     if ticket:
         return ticket.upper()
     return None
 
 
 @dataclass(frozen=True)
 class JiraConfig:
     site: str
     user_name: str
     password: str
+    ticket_pattern: Pattern
     token: Optional[str]
 
     @staticmethod
     def from_config(config: dict):
-        return JiraConfig(site=config['site'], user_name=config['userName'], password=config['password'],
-                          token=config.get('token'))
+        jira_config = config.get('jira')
+        if not jira_config:
+            raise KeyError(f'jira section needs to be defined in {DEFAULT_CONFIG_FILE_NAME}')
+        return JiraConfig(site=jira_config['site'], user_name=jira_config['userName'], password=jira_config['password'],
+                          ticket_pattern=re.compile(jira_config.get('ticketPattern', '[A-Za-z]{2,}-\\d+')),
+                          token=jira_config.get('token'))
+
+
+def create_jira_for_config(jira_config: JiraConfig):
+    return Jira(
+        url=jira_config.site,
+        token=jira_config.token,
+        api_version='2',
+        cloud=True
+    ) if jira_config.token else Jira(
+        url=jira_config.site,
+        username=jira_config.user_name,
+        password=jira_config.password,
+        api_version='2',
+        cloud=True
+    )
+
+
+def to_github_markdown(jira_markdown: str, jira_url: str) -> str:
+    jira_markdown = re.sub(r'\[(.*)/(.*)\|(.*)\|smart-link\]', r'[\2](\3)', jira_markdown)
+    jira_markdown = re.sub(r'\[(.*)\|(.*)\]', r'[\1](\2)', jira_markdown)
+    jira_markdown = re.sub(r'\[~accountid:(.*)\]', rf'[👩‍💻]({jira_url}/jira/people/\1)', jira_markdown)
+    jira_markdown = re.sub(r'\{\{(.*)\}\}', r'`\1`', jira_markdown)
+    jira_markdown = re.sub(r'\{quote}(.*)\{quote}', r'> \1', jira_markdown)
+    jira_markdown = re.sub(r'\{noformat\}((.|\n)*)\{noformat\}', r'```\n\1\n```', jira_markdown)
+    jira_markdown = re.sub(r'\{code:+(.*)\}((.|\n)*)\{code\}', r'```\1\n\2\n```', jira_markdown)
+    jira_markdown = re.sub(r'\{noformat\}((.|\n)*)', r'```\n\1\n```', jira_markdown)
+    jira_markdown = re.sub(r'\*(.*)\*', r'**\1**', jira_markdown)
+    jira_markdown = re.sub(r'_(.*)_', r'*\1*', jira_markdown)
+    jira_markdown = re.sub(r'!.*\|.*!', r'', jira_markdown)
+
+    jira_markdown = jira_markdown.replace('h1. ', '### ')
+    jira_markdown = jira_markdown.replace('h2. ', '#### ')
+    jira_markdown = jira_markdown.replace('h3. ', '##### ')
+    jira_markdown = jira_markdown.replace('h4. ', '###### ')
+    jira_markdown = jira_markdown.replace('h5. ', '###### ')
+    jira_markdown = jira_markdown.replace('h6. ', '###### ')
+    return jira_markdown
+
+
+def to_markdown_summary(ticket: JiraTicket, run_result: RunResult) -> str:
+    description_markdown = to_github_markdown(ticket.description, ticket.ticket_url) if ticket.description else ""
+    lines = description_markdown.splitlines()
+    max_message_length = 288
+    if len(lines) > max_message_length:
+        description_markdown = "\n".join(lines[:max_message_length]) + "\n..."
+
+    details = run_result.run_properties.details
+
+    build_status = f"🏗️ Build [{details.build_id}]({details.run_url}) {run_result.status_line}, " \
+                   f"started by _{details.user}_  \n{markdown_for_stage(run_result, Stage.DEPLOY)}"
+    return f"## 📕 [{ticket.ticket_id}]({ticket.ticket_url}) {ticket.summary} " \
+           f"![{ticket.user_email}]({ticket.user_avatar}) \n" \
+           f"{description_markdown}\n" \
+           f"{build_status}"
+
+
+def compose_build_status(result: RunResult, config: dict) -> str:
+    jira_config = JiraConfig.from_config(config=config)
+    jira_client = create_jira_for_config(jira_config)
+    branch = result.run_properties.versioning.branch
+    if not branch:
+        return " # ⚠️ `versioning.branch` not set, cannot find corresponding ticket"
+    ticket_id = extract_ticket_from_branch(branch, jira_config.ticket_pattern)
+    if not ticket_id:
+        return f" # ⚠️ Could not find ticket corresponding to `{branch}. " \
+               f"Does your branch name follow the correct pattern?"
+    issue = jira_client.get_issue(ticket_id)
+    jira_ticket = JiraTicket.from_issue_response(issue)
+    return to_markdown_summary(jira_ticket, result)
+
+
+class JiraOutcome(ReportOutcome):
+    pass
 
 
 class JiraReporter(Reporter):
 
     def __init__(self, config: dict, branch: str, logger: Logger):
-        jira_config = config.get('jira')
-        if not jira_config:
-            raise ValueError('jira section needs to be defined in config.yml')
-        self._ticket = extract_ticket_from_branch(branch)
-
-        jira_config = JiraConfig.from_config(jira_config)
+        jira_config = JiraConfig.from_config(config)
+        self._ticket = extract_ticket_from_branch(branch, jira_config.ticket_pattern) if branch else None
         self._config = jira_config
-        self._jira = Jira(url=jira_config.site, token=jira_config.token, api_version='3',
-                          cloud=True) if jira_config.token else Jira(url=jira_config.site,
-                                                                     username=jira_config.user_name,
-                                                                     password=jira_config.password,
-                                                                     api_version='3', cloud=True)
+        self._jira = create_jira_for_config(jira_config)
         self._logger = logger
 
-    def send_report(self, results: RunResult) -> None:
+    def send_report(self, results: RunResult, text: Optional[str] = None) -> JiraOutcome:
         if not self._ticket:
-            return None
+            return JiraOutcome(success=True)
+
+        try:
+            issue_response = self._jira.get_issue(self._ticket)
+
+            ticket = JiraTicket.from_issue_response(issue_response)
 
-        issue_response = self._jira.get_issue(self._ticket)
-        ticket = JiraTicket.from_issue_response(issue_response)
+            self.__move_ticket_forward(ticket)
 
-        self.__move_ticket_forward(ticket)
+            user_email = results.run_properties.details.user_email
+            if user_email:
+                self.__assign_ticket(user_email, ticket)
+            return JiraOutcome(success=True)
 
-        user_email = results.run_properties.details.user_email
-        if user_email:
-            self.__assign_ticket(user_email, ticket)
-        return None
+        except requests.exceptions.HTTPError as exc:
+            self._logger.warning(f'Could not handle Jira ticket {self._ticket}: {exc}')
+            return JiraOutcome(success=False, exception=exc)
 
     def __assign_ticket(self, run_user_email: str, ticket: JiraTicket):
         if ticket.assignee_email is None or ticket.assignee_email != run_user_email:
             jira_user = self._jira.user_find_by_user_string(query=run_user_email)
             if jira_user:
                 account_id = jira_user.pop().get('accountId')
                 self._logger.info(f'Assigning {ticket.ticket_id} to {account_id}')
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## mpyl/reporting/targets/slack.py

```diff
@@ -31,40 +31,42 @@
 ```
 """
 import re
 from dataclasses import dataclass
 from typing import Dict, Optional
 
 from slack_sdk import WebClient
+from slack_sdk.errors import SlackClientError
 from slack_sdk.models.blocks import HeaderBlock, SectionBlock, MarkdownTextObject, ContextBlock, ImageElement, Block
 
-from . import Reporter
+from . import Reporter, ReportOutcome
 from ..formatting.markdown import run_result_to_markdown
 from ...steps.models import RunProperties
 from ...steps.run import RunResult
 
 
 def to_slack_markdown(markdown: str) -> str:
     regex_replace = (
-        (re.compile(r'\[(.*)\]\((.*)\)', flags=re.M), r'<\2|\1>'),
+        (re.compile(r'\[(.*?)\]\((.*?)\)'), r'<\2|\1>'),
         (re.compile(r'^- ', flags=re.M), '• '),
         (re.compile(r'^  - ', flags=re.M), '  ◦ '),
         (re.compile(r'^    - ', flags=re.M), '    ⬩ '),
         (re.compile(r'^      - ', flags=re.M), '    ◽ '),
         (re.compile(r'^#+ (.+)$', flags=re.M), r'*\1*'),
         (re.compile(r'\*\*'), '*'),
         (re.compile(r'~~'), '~'),
     )
-    for regex, replacement in regex_replace:
-        markdown = regex.sub(replacement, markdown)
+    for pattern, replacement in regex_replace:
+        markdown = re.sub(pattern, replacement, markdown)
     return markdown
 
 
 @dataclass(frozen=True)
 class SlackIcons:
+    building: str
     success: str
     failure: str
 
 
 @dataclass(frozen=True)
 class MessageIdentifier:
     channel_id: str
@@ -74,51 +76,69 @@
 @dataclass(frozen=True)
 class UserInfo:
     user_name: str
     profile_image: str
     initiator: Optional[str]
 
 
+class SlackOutcome(ReportOutcome):
+    pass
+
+
 class SlackReporter(Reporter):
     _icons: SlackIcons
     _message_identifier: Optional[MessageIdentifier]
 
     def __init__(self, config: Dict, channel: Optional[str], title: str,
                  message_identifier: Optional[MessageIdentifier] = None):
         slack_config = config.get('slack')
         if not slack_config:
             raise ValueError('slack config not set')
         self._client = WebClient(token=slack_config['botToken'])
         self._channel = channel
         self._title = title
         icons = slack_config['icons']
-        self._icons = SlackIcons(success=icons['success'], failure=icons['failure'])
+        self._icons = SlackIcons(success=icons['success'], failure=icons['failure'], building=icons['building'])
         self._message_identifier = message_identifier
 
-    def send_report(self, results: RunResult) -> None:
-        user_info = self.__get_user_info(results.run_properties.details.user_email)
-
-        if not self._channel and user_info.initiator:
-            self._channel = self.__open_conversation_with_user(user_info.initiator)
-
-        if not self._channel:
-            raise ValueError('Channel not explicitly set and initiator could not be determined')
-
-        text = to_slack_markdown(run_result_to_markdown(results))
-        blocks = self.__compose_blocks(results, text, user_info)
-
-        if self._message_identifier:
-            self._client.chat_update(channel=self._message_identifier.channel_id,
-                                     ts=self._message_identifier.time_stamp,
-                                     icon_emoji=':robot_face:', mrkdwn=True, blocks=blocks, text=text)
-            return
-
-        response = self._client.chat_postMessage(channel=self._channel, icon_emoji=':robot_face:', mrkdwn=True,
-                                                 blocks=blocks, text=text)
-        self._message_identifier = MessageIdentifier(channel_id=response['channel'], time_stamp=response['ts'])
+    def send_report(self, results: RunResult, text: Optional[str] = None) -> ReportOutcome:
+        try:
+            user_info = self.__get_user_info(results.run_properties.details.user_email)
+
+            if not self._channel and user_info.initiator:
+                self._channel = self.__open_conversation_with_user(user_info.initiator)
+
+            if not self._channel:
+                raise ValueError('Channel not explicitly set and initiator could not be determined')
+
+            body = to_slack_markdown(text if text else run_result_to_markdown(results))
+            blocks = self.__compose_blocks(results, body, user_info)
+
+            if self._message_identifier:
+                self._client.chat_update(channel=self._message_identifier.channel_id,
+                                         ts=self._message_identifier.time_stamp,
+                                         icon_emoji=':robot_face:', mrkdwn=True, blocks=blocks, text=body)
+                return SlackOutcome(success=True)
+
+            response = self._client.chat_postMessage(channel=self._channel, icon_emoji=':robot_face:', mrkdwn=True,
+                                                     blocks=blocks, text=body)
+            self._message_identifier = MessageIdentifier(channel_id=response['channel'], time_stamp=response['ts'])
+            return SlackOutcome(success=True)
+        except SlackClientError as slack_exception:
+            return SlackOutcome(success=False, exception=slack_exception)
+
+    def send_progress_update(self, results: RunResult, text: Optional[str]):
+        if not self._message_identifier:
+            raise ValueError('Message identifier not set. Cannot call update before `send_report` has been called')
+
+        result_markdown = text if text else run_result_to_markdown(results)
+        body = to_slack_markdown(result_markdown)
+        blocks = self.__compose_blocks(results, body, self.__get_user_info(results.run_properties.details.user_email))
+        self._client.chat_update(channel=self._message_identifier.channel_id, ts=self._message_identifier.time_stamp,
+                                 icon_emoji=':robot_face:', mrkdwn=True, blocks=blocks, text=body)
 
     def __open_conversation_with_user(self, user_id: str):
         opened_channel = self._client.conversations_open(users=[user_id])
         return opened_channel['channel']['id']
 
     def __get_user_info(self, user_email: Optional[str]):
         profile_data: dict[str, str] = {}
@@ -130,23 +150,31 @@
             profile_data = resp.get('profile', {})
 
         return UserInfo(user_name=profile_data.get('real_name_normalized', 'Anonymous'),
                         profile_image=profile_data.get('image_24',
                                                        'https://avatars.githubusercontent.com/u/18010732'),
                         initiator=user_id)
 
+    def __get_icon(self, results: RunResult):
+        if results.is_in_progress:
+            return self._icons.building
+        if results.is_success:
+            return self._icons.success
+        return self._icons.failure
+
     def __compose_blocks(self, results: RunResult, text: str, user_info: UserInfo) -> list[Block]:
-        icon = self._icons.success if results.is_success else self._icons.failure
+        icon = self.__get_icon(results)
+
         context = self.compose_context(results.run_properties, icon, user_info.user_name)
         return [HeaderBlock(text=self._title),
                 SectionBlock(text=MarkdownTextObject(text=text)),
                 ContextBlock(elements=[MarkdownTextObject(text=context),
                                        ImageElement(image_url=user_info.profile_image, alt_text=user_info.user_name)])
                 ]
 
     @staticmethod
     def compose_context(build_props: RunProperties, icon: str, user: Optional[str]) -> str:
         details = build_props.details
         user_name = user if user else details.user
-        return f":{icon}: Build <{details.run_url}|{details.build_id.upper()}> and changes in " \
+        return f":{icon}: Build <{details.run_url}|{details.build_id.upper()}> for " \
                f"<{details.change_url}|{build_props.versioning.identifier.upper()}> " \
                f"started by _{user_name}_"
```

## mpyl/schema/mpyl_config.schema.yml

```diff
@@ -5,14 +5,18 @@
     type: object
     additionalProperties: false
     properties:
       cvs:
         "$ref": "#/definitions/CVS"
       docker:
         "$ref": "#/definitions/Docker"
+      whiteLists:
+        "$ref": "#/definitions/Whitelists"
+      cypress:
+        "$ref": "#/definitions/Cypress"
       kubernetes:
         "$ref": "#/definitions/Kubernetes"
       project:
         "$ref": "#/definitions/Project"
       jenkins:
         "$ref": "#/definitions/Jenkins"
       sbt:
@@ -21,14 +25,55 @@
         "$ref": "#/definitions/Slack"
       jira:
         "$ref": "#/definitions/Jira"
     required:
       - cvs
       - docker
     title: MPyL global configuration
+  Whitelists:
+    type: object
+    required:
+      - default
+      - addresses
+    properties:
+      default:
+        description: "Default whitelist for all environments"
+        type: array
+        items:
+          minItems: 1
+          type: string
+      addresses:
+        type: array
+        minItems: 1
+        items:
+          type: object
+          additionalProperties: false
+          required:
+            - name
+            - values
+          properties:
+            name:
+              type: string
+            values:
+              type: array
+              items:
+                minItems: 1
+                type: string
+  Cypress:
+    type: object
+    additionalProperties: false
+    properties:
+      recordKey:
+        type: string
+        description: 'Key for recording runs to cypress dashboard'
+      cypressSourceCodePath:
+        type: string
+        description: 'Path to cypress source code'
+    required:
+      - cypressSourceCodePath
   Kubernetes:
     type: object
     additionalProperties: false
     properties:
       rancher:
         type: object
         additionalProperties: false
@@ -70,45 +115,54 @@
       - git
       - github
     title: CVS
   Git:
     type: object
     additionalProperties: false
     properties:
+      remote:
+        type: object
+        additionalProperties: false
+        properties:
+          url:
+            type: [ string, null ]
+          userName:
+            type: [ string, null ]
+          password:
+            type: [ string, null ]
       mainBranch:
         type: string
     required:
       - mainBranch
     title: Git
   Github:
     type: object
     additionalProperties: false
     properties:
       repository:
         type: string
       token:
-        type: string
+        type: [ string, null ]
       app:
         type: object
         properties:
           privateKeyPath:
             description: Used to authenticate with github if the app is used (https://github.com/apps/mpyl-pipeline)
             type: string
           privateKeyBase64Encoded:
             description: Used to authenticate with github if the app is used (https://github.com/apps/mpyl-pipeline)
-            type: string
+            type: [ string, null ]
           appId:
             description: The id of the github app (https://github.com/apps/mpyl-pipeline) that has permission to update checks
             type: string
             default: 295700
         required:
           - appId
     required:
       - repository
-      - token
     title: Github
   Docker:
     type: object
     additionalProperties: false
     properties:
       registry:
         "$ref": "#/definitions/Registry"
@@ -121,15 +175,15 @@
             description: "Polling interval for checking if containers are up"
             type: integer
             default: 2
           failureThreshold:
             description: "Maximum number of times to poll before considering 'docker-compose up' failed"
             type: integer
             default: 20
-        required: ['periodSeconds', 'failureThreshold']
+        required: [ 'periodSeconds', 'failureThreshold' ]
     required:
       - registry
     title: Docker
   Build:
     type: object
     additionalProperties: false
     properties:
@@ -145,15 +199,15 @@
         type: string
     required: [ rootFolder, buildTarget, dockerFileName ]
   Registry:
     type: object
     additionalProperties: false
     properties:
       hostName:
-        type: string
+        type: [ string, null ]
       userName:
         type: string
       password:
         type: string
     required:
       - hostName
       - password
@@ -161,14 +215,16 @@
     title: Registry
   Sbt:
     type: object
     additionalProperties: false
     properties:
       command:
         type: string
+      clientCommand:
+        type: string
       verbose:
         default: false
         type: boolean
       testWithCoverage:
         type: string
       javaOpts:
         type: string
@@ -182,65 +238,82 @@
             type: boolean
             default: true
           test:
             type: boolean
             default: true
     required:
       - command
+      - clientCommand
       - javaOpts
       - sbtOpts
     title: Sbt
   Project:
     type: object
     additionalProperties: false
+    required:
+      - allowedMaintainers
+      - deployment
     properties:
+      allowedMaintainers:
+        type: array
+        items:
+          type: string
       deployment:
         type: object
         additionalProperties: false
         properties:
+          traefik:
+            "$ref": "project.schema.yml#/definitions/traefik"
           kubernetes:
-             "$ref": "project.schema.yml#/definitions/kubernetes"
+            "$ref": "project.schema.yml#/definitions/kubernetes"
   Slack:
     type: object
     additionalProperties: false
     properties:
       botToken:
-          type: string
+        type: [ string, null ]
       icons:
         type: object
         properties:
+          building:
+            type: string
           success:
             type: string
           failure:
             type: string
-        required: ['success', 'failure']
+        required: [ 'success', 'failure', 'building' ]
     required:
       - botToken
       - icons
   Jenkins:
     type: object
     additionalProperties: false
+    required: [ 'url' ]
     properties:
       url:
-        type: string
+        type: [ string ]
         format: url
       pipelines:
         type: object
-        additionalProperties: {"type": "string"}
+        additionalProperties: { "type": "string" }
       defaultPipeline:
         type: string
   Jira:
     type: object
     additionalProperties: false
     properties:
       site:
         description: "Only works with the cloud version of Jira"
-        type: string
+        type: [ string, null ]
         format: uri
       userName:
         type: string
       password:
         type: string
       token:
         type: string
+      ticketPattern:
+        type: [ string, null ]
+        default: '[A-Za-z]{2,}-\d+'
+        description: 'A pattern that extracts a ticket number from the branch name'
     required:
       - site
```

## mpyl/schema/project.schema.yml

```diff
@@ -24,26 +24,14 @@
   maintainer:
     description: >-
       Describes which team or guild is ultimately responsible for the life cycle
       of this particular project
     type: array
     items:
       type: string
-      enum:
-        - Energy Trading
-        - Big Data
-        - Flex IoT
-        - Marketplace
-        - EV Home
-        - Data Analytics
-        - Salesforce
-        - Commercial Analytics
-        - Energy Services And Flex Analytics
-        - Finance
-        - Portfolio Management
     uniqueItems: true
     minItems: 1
   stages:
     $id: '#/properties/stages'
     description: Defines which steps should be executed at each stage
     type: object
     additionalProperties: false
@@ -76,15 +64,15 @@
         $id: '#/properties/stages/deploy'
         description: Deploys the artifacts created in the build stage
         examples:
           - Kubernetes Deploy
         type: string
         enum:
           - Docker Deploy
-          - Ephemeral Docker Deploy
+          - Deploy From Docker Container
           - Echo Deploy
           - NUC Deploy
           - Kubernetes Deploy
           - Echo Kubernetes Deploy
           - Kubernetes Job Deploy
           - Kubernetes Job Template Deploy
           - Kubernetes Spark Job Deploy
@@ -95,14 +83,15 @@
       postdeploy:
         description: Additional steps that can be done after the project has been deployed.
         examples:
           - TriggerJenkinsJob PostDeploy
         type: string
         enum:
           - TriggerJenkinsJob PostDeploy
+          - Cypress Test
     minProperties: 1
   docker:
     description: Defines docker repository and it's credentials
     type: object
     additionalProperties: false
     properties:
       credentialsId:
@@ -224,23 +213,15 @@
           bucket:
             $ref: '#/definitions/dtapValue'
           path:
             $ref: '#/definitions/dtapValue'
       kubernetes:
         $ref: '#/definitions/kubernetes'
       traefik:
-        additionalProperties: false
-        type: object
-        properties:
-          enabled:
-            type: boolean
-          hosts:
-            type: array
-            items:
-              $ref: '#/definitions/traefikHost'
+        $ref: '#/definitions/traefik'
       nuc:
         type: object
         required:
           - path
         properties:
           config:
             type: string
@@ -305,16 +286,29 @@
         minItems: 1
       test:
         type: array
         minItems: 1
       deploy:
         type: array
         minItems: 1
+      postdeploy:
+        type: array
+        minItems: 1
     additionalProperties: false
 definitions:
+  traefik:
+    additionalProperties: false
+    type: object
+    properties:
+      enabled:
+        type: boolean
+      hosts:
+        type: array
+        items:
+          $ref: '#/definitions/traefikHost'
   dtapValue:
     type: object
     additionalProperties: false
     oneOf:
       - required:
           - pr
           - test
@@ -422,15 +416,15 @@
   livenessProbe:
     type: object
     additionalProperties: true
     required:
       - path
     properties:
       path:
-        description: URL to be used called for liveness probes
+        description: URL to be called for liveness probes
         $ref: '#/definitions/dtapValue'
       periodSeconds:
         description: >-
           How often to perform the probe. Period needs to be > than timeout, or
           requests will overlap
         type: integer
       timeoutSeconds:
@@ -449,15 +443,15 @@
   startupProbe:
     type: object
     additionalProperties: true
     required:
       - path
     properties:
       path:
-        description: URL to be used called for startup probes
+        description: URL to be called for startup probes
         $ref: '#/definitions/dtapValue'
       initialDelaySeconds:
         description: >-
           Number of seconds after the container has started before probe is
           started.
         type: integer
       periodSeconds:
@@ -767,54 +761,14 @@
         type: object
         additionalItems: false
         required:
           - name
         properties:
           name:
             type: string
-      cron:
-        description: 'CronJobSpec describes how the job execution will look like and when it
-          will actually run. Identical to See https://kubernetesjsonschema.dev/v1.14.0/_definitions.json#/definitions/io.k8s.api.batch.v1beta1.CronJobSpec
-          but without jobTemplate'
-        additionalProperties: false
-        properties:
-          concurrencyPolicy:
-            description: 'Specifies how to treat concurrent executions of a Job. Valid values
-              are: - "Allow" (default): allows CronJobs to run concurrently; - "Forbid": forbids
-              concurrent runs, skipping next run if previous run hasn''t finished yet; - "Replace":
-              cancels currently running job and replaces it with a new one
-              See https://kubernetes.io/docs/tasks/job/automated-tasks-with-cron-jobs/#concurrency-policy
-              '
-            type: string
-            enum:
-              - Allow
-              - Forbid
-              - Replace
-          failedJobsHistoryLimit:
-            description: The number of failed finished jobs to retain. This is a pointer to
-              distinguish between explicit zero and not specified. Defaults to 1.
-            format: int32
-            type: integer
-          schedule:
-            description: The schedule in Cron format, see https://en.wikipedia.org/wiki/Cron.
-            type: string
-          startingDeadlineSeconds:
-            description: Optional deadline in seconds for starting the job if it misses scheduled
-              time for any reason.  Missed jobs executions will be counted as failed ones.
-            format: int64
-            type: integer
-          successfulJobsHistoryLimit:
-            description: The number of successful finished jobs to retain. This is a pointer
-              to distinguish between explicit zero and not specified. Defaults to 3.
-            format: int32
-            type: integer
-          suspend:
-            description: This flag tells the controller to suspend subsequent executions,
-              it does not apply to already started executions.  Defaults to false.
-            type: boolean
       policies:
         type: array
         minItems: 1
       labels:
         type: array
         items:
           $ref: '#/definitions/label'
@@ -870,18 +824,72 @@
           limit:
             $ref: '#/definitions/limitResources'
           request:
             $ref: '#/definitions/requestResources'
         additionalProperties: false
       portMappings:
         type: object
-      ttlSecondsAfterFinished:
-        $ref: '#/definitions/dtapNumberValue'
-      activeDeadlineSeconds:
-        $ref: '#/definitions/dtapNumberValue'
+      job:
+        type: object
+        additionalProperties: true
+        properties:
+          ttlSecondsAfterFinished:
+            $ref: '#/definitions/dtapNumberValue'
+          activeDeadlineSeconds:
+            $ref: '#/definitions/dtapNumberValue'
+          cron:
+            description: 'CronJobSpec describes how the job execution will look like and when it
+              will actually run. Identical to See https://kubernetesjsonschema.dev/v1.14.0/_definitions.json#/definitions/io.k8s.api.batch.v1beta1.CronJobSpec
+              but without jobTemplate'
+            additionalProperties: false
+            properties:
+              concurrencyPolicy:
+                description: 'Specifies how to treat concurrent executions of a Job. Valid values
+                  are: - "Allow" (default): allows CronJobs to run concurrently; - "Forbid": forbids
+                  concurrent runs, skipping next run if previous run hasn''t finished yet; - "Replace":
+                  cancels currently running job and replaces it with a new one
+                  See https://kubernetes.io/docs/tasks/job/automated-tasks-with-cron-jobs/#concurrency-policy
+                  '
+                type: string
+                enum:
+                  - Allow
+                  - Forbid
+                  - Replace
+              failedJobsHistoryLimit:
+                description: The number of failed finished jobs to retain. This is a pointer to
+                  distinguish between explicit zero and not specified. Defaults to 1.
+                format: int32
+                type: integer
+              schedule:
+                description: The schedule in Cron format, see https://en.wikipedia.org/wiki/Cron.
+                type: string
+              startingDeadlineSeconds:
+                description: Optional deadline in seconds for starting the job if it misses scheduled
+                  time for any reason.  Missed jobs executions will be counted as failed ones.
+                format: int64
+                type: integer
+              successfulJobsHistoryLimit:
+                description: The number of successful finished jobs to retain. This is a pointer
+                  to distinguish between explicit zero and not specified. Defaults to 3.
+                format: int32
+                type: integer
+              suspend:
+                description: This flag tells the controller to suspend subsequent executions,
+                  it does not apply to already started executions.  Defaults to false.
+                type: boolean
+          spark:
+            type: object
+            additionalProperties: false
+            properties:
+              mainClass:
+                description: 'MainClass is the fully-qualified main class of the Spark application.'
+                type: string
+              mainApplicationFile:
+                description: 'MainFile is the path to a bundled JAR, Python, or R file of the application.'
+                type: string
       role:
         type: object
         additionalProperties: false
         required:
           - resources
           - verbs
         properties:
```

## mpyl/stages/discovery.py

```diff
@@ -1,32 +1,55 @@
 """ Discovery of projects that are relevant to a specific `mpyl.stage.Stage` . Determine which of the
 discovered projects have been invalidated due to changes in the source code since the last build of the project's
 output artifact."""
+import operator
+from dataclasses import dataclass
+from pathlib import Path
+from typing import Optional
 
-from ..project import Project
+from ..project import Project, load_project
 from ..project import Stage
 from ..steps.models import Output
-from ..utilities.repo import Revision
+from ..utilities.repo import Revision, RepoConfig, Repository
+
+
+@dataclass(frozen=True)
+class DeploySet:
+    all_projects: set[Project]
+    projects_to_deploy: set[Project]
 
 
 def is_invalidated(project: Project, stage: Stage, path: str) -> bool:
     deps = project.dependencies
     deps_for_stage = deps.set_for_stage(stage) if deps else {}
 
     touched_dependency = next(filter(path.startswith, deps_for_stage), None) if deps else None
     startswith: bool = path.startswith(project.root_path)
     return startswith or touched_dependency is not None
 
 
+def output_invalidated(output: Optional[Output], revision_hash: str) -> bool:
+    if output is None:
+        return True
+    if not output.success:
+        return True
+    if output.produced_artifact is None:
+        return True
+    artifact = output.produced_artifact
+    if artifact.revision != revision_hash:
+        return True
+
+    return False
+
+
 def _to_relevant_changes(project: Project, stage: Stage, change_history: list[Revision]) -> set[str]:
     output: Output = Output.try_read(project.target_path, stage)
     relevant = set()
     for history in reversed(sorted(change_history, key=lambda c: c.ord)):
-        if stage == Stage.DEPLOY or output is None or output.produced_artifact is None \
-                or output.produced_artifact.revision != history.hash:
+        if stage == Stage.DEPLOY or output_invalidated(output, history.hash):
             relevant.update(history.files_touched)
         else:
             return relevant
 
     return relevant
 
 
@@ -39,19 +62,28 @@
 
 
 def find_invalidated_projects_for_stage(all_projects: set[Project], stage: Stage,
                                         change_history: list[Revision]) -> set[Project]:
     return set(filter(lambda p: are_invalidated(p, stage, change_history), all_projects))
 
 
+def find_deploy_set(repo_config: RepoConfig) -> DeploySet:
+    with Repository(repo_config) as repo:
+        changes_in_branch = repo.changes_in_branch_including_local()
+        project_paths = repo.find_projects()
+        all_projects = set(map(lambda p: load_project(Path(""), Path(p), False), project_paths))
+        return DeploySet(all_projects,
+                         find_invalidated_projects_for_stage(all_projects, Stage.DEPLOY, changes_in_branch))
+
+
 def find_invalidated_projects_per_stage(all_projects: set[Project], change_history: list[Revision]) \
         -> dict[Stage, set[Project]]:
     projects_for_stage = {}
     for stage in Stage:
         projects = find_invalidated_projects_for_stage(all_projects, stage, change_history)
         if projects:
-            projects_for_stage[stage] = projects
+            projects_for_stage[stage] = set(sorted(projects, key=operator.attrgetter('name')))
     return projects_for_stage
 
 
 def for_stage(projects: set[Project], stage: Stage) -> set[Project]:
     return set(filter(lambda p: p.stages.for_stage(stage), projects))
```

## mpyl/steps/models.py

```diff
@@ -1,17 +1,19 @@
 """ Model representation of run-specific configuration. """
 
+import pkgutil
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from typing import Optional, Dict
 
 from ruamel.yaml import YAML, yaml_object  # type: ignore
 
 from ..project import Project, Stage, Target
+from ..validation import validate
 
 yaml = YAML()
 
 
 @dataclass(frozen=True)
 class VersioningProperties:
     revision: str
@@ -24,14 +26,15 @@
             raise ValueError('Either pr_number or tag need to be set')
 
     @property
     def identifier(self):
         return f'pr-{self.pr_number}' if self.pr_number else self.tag
 
 
+
 @dataclass(frozen=True)
 class RunContext:
     build_id: str
     """Uniquely identifies the run. Typically a monotonically increasing number"""
     run_url: str
     """Link back to the run executor"""
     change_url: str
@@ -46,42 +49,77 @@
     @staticmethod
     def from_configuration(run_details: Dict):
         return RunContext(build_id=run_details['id'], run_url=run_details['run_url'],
                           change_url=run_details['change_url'], tests_url=run_details['tests_url'],
                           user=run_details['user'], user_email=run_details['user_email'])
 
 
+@dataclass(frozen=True)
+class ConsoleProperties:
+    log_level: str
+    width: Optional[int]
+
+    @staticmethod
+    def from_configuration(build_config: Dict):
+        console_config = build_config['console']
+        width = console_config.get('width', 130)
+        return ConsoleProperties(console_config.get('logLevel', 'INFO'), None if width == 0 else width)
+
+
 @yaml_object(yaml)
 @dataclass(frozen=True)
 class RunProperties:
     """ Contains information that is specific to a particular run of the pipeline"""
     details: RunContext
     """Run specific details"""
     target: Target
     """The deploy target"""
     versioning: VersioningProperties
     config: dict
     """Globally specified configuration, to be used by specific steps. Complies with the schema as
     specified in `mpyl_config.schema.yml`
      """
+    console: ConsoleProperties
+    """Settings for the console output"""
+    local: bool
+    """Whether the run is local or not"""
 
     @staticmethod
-    def for_local_run(config: Dict, revision: str, branch: Optional[str]):
+    def for_local_run(config: Dict, revision: str, branch: Optional[str], tag: Optional[str]):
         return RunProperties(details=RunContext("", "", "", "", "", None), target=Target.PULL_REQUEST,
-                             versioning=VersioningProperties(revision, branch, 123, None), config=config)
+                             versioning=VersioningProperties(revision, branch, 123, tag), config=config,
+                             console=ConsoleProperties("INFO", 130), local=True)
 
     @staticmethod
     def from_configuration(run_properties: Dict, config: Dict):
+        build_dict = pkgutil.get_data(__name__, "../schema/run_properties.schema.yml")
+
+        if build_dict:
+            validate(run_properties, build_dict.decode('utf-8'))
+
         build = run_properties['build']
-        versioning = build['versioning']
-        versioning = VersioningProperties(revision=versioning['revision'], branch=versioning['branch'],
-                                          pr_number=int(versioning.get('pr_number')), tag=versioning.get('tag'))
+        versioning_config = build['versioning']
+
+        pr_num: str = versioning_config.get('pr_number')
+        tag: str = versioning_config.get('tag')
 
-        return RunProperties(details=RunContext.from_configuration(build['run']),
-                             target=Target(build['parameters']['deploy_target']), versioning=versioning, config=config)
+        versioning = VersioningProperties(revision=versioning_config['revision'],
+                                          branch=versioning_config['branch'],
+                                          pr_number=int(pr_num) if pr_num else None,
+                                          tag=tag)
+        console = ConsoleProperties.from_configuration(build)
+
+        return RunProperties(
+            details=RunContext.from_configuration(build['run']),
+            target=Target(build['parameters']['deploy_target']),
+            versioning=versioning,
+            config=config,
+            console=console,
+            local=str(build['local']).lower() == 'true'
+        )
 
 
 @yaml_object(yaml)
 @dataclass(frozen=True)
 class ArtifactType(Enum):
     def __eq__(self, other):
         return self.value == other.value
@@ -95,15 +133,17 @@
         return representer.represent_scalar('!ArtifactType',
                                             f'{node._name_}-{node._value_}')  # pylint: disable=protected-access
 
     DOCKER_IMAGE = 1
     """A docker image"""
     JUNIT_TESTS = 2
     """A test suite in junit compatible `.xml` format"""
-    NONE = 3
+    DEPLOYED_HELM_APP = 3
+    """A helm chart deployed to kubernetes"""
+    NONE = 4
 
 
 @yaml_object(yaml)
 @dataclass(frozen=True)
 class Artifact:
     artifact_type: ArtifactType
     revision: str
```

## mpyl/steps/run.py

```diff
@@ -3,44 +3,72 @@
 """
 
 import operator
 from typing import Optional
 
 from .models import RunProperties
 from ..project import Stage, Project
-from .steps import StepResult
+from .steps import StepResult, ExecutionException
 
 
 class RunResult:
     _run_plan: dict[Stage, set[Project]]
-    _results: list[StepResult] = []
+    _results: list[StepResult]
     _run_properties: RunProperties
-    _exception: Optional[Exception]
+    _exception: Optional[ExecutionException]
 
     def __init__(self, run_properties: RunProperties, run_plan=None):
         if run_plan is None:
             run_plan = {}
         self._run_properties = run_properties
         self._run_plan = run_plan
         self._exception = None
+        self._results = []
 
     @property
     def status_line(self) -> str:
         if self._exception:
-            return '❗Failed with exception'
+            return '❗ Failed with exception'
+        if self.is_in_progress:
+            return '🏗️ Building'
+        if not self.has_results:
+            return '🦥 Nothing to do'
         if self._results_success():
-            return '✅Successful'
-        return '❌Failed'
+            return '✅ Successful'
+
+        return '❌ Failed'
+
+    @property
+    def failed_result(self) -> Optional[StepResult]:
+        return next((r for r in self._results if not r.output.success), None)
+
+    @property
+    def progress_fraction(self) -> float:
+        unfinished = 0
+        finished = 0
+        for stage, projects in self.run_plan.items():
+            finished_project_names = set(map(lambda r: r.project.name, self.results_for_stage(stage)))
+            for project in projects:
+                if project.name in finished_project_names:
+                    finished += 1
+                else:
+                    unfinished += 1
+
+        total = unfinished + finished
+        if total == 0:
+            return 0.0
+
+        return 1.0 - (unfinished / total)
 
     @property
-    def exception(self) -> Optional[Exception]:
+    def exception(self) -> Optional[ExecutionException]:
         return self._exception
 
     @exception.setter
-    def exception(self, exception: Exception):
+    def exception(self, exception: ExecutionException):
         self._exception = exception
 
     @property
     def run_properties(self) -> RunProperties:
         return self._run_properties
 
     @property
@@ -55,16 +83,28 @@
 
     @property
     def is_success(self):
         if self._exception:
             return False
         return self._results_success()
 
+    @property
+    def is_finished(self):
+        return self.progress_fraction == 1.0
+
+    @property
+    def has_results(self):
+        return len(self._results) > 0
+
+    @property
+    def is_in_progress(self):
+        return len(self.run_plan.items()) > 0 and self.is_success and not self.is_finished
+
     def _results_success(self):
-        return all(r.output.success for r in self._results)
+        return not self.has_results or all(r.output.success for r in self._results)
 
     @staticmethod
     def sort_chronologically(results: list[StepResult]) -> list[StepResult]:
         return sorted(results, key=operator.attrgetter('timestamp'))
 
     def results_for_stage(self, stage: Stage) -> list[StepResult]:
         return RunResult.sort_chronologically([res for res in self._results if res.stage == stage])
```

## mpyl/steps/steps.py

```diff
@@ -1,45 +1,70 @@
 """ Entry point of MPyL. Loads all available Step implementations and triggers their execution based on the specified
 Project and Stage.
 """
-
+import itertools
 import pkgutil
 from dataclasses import dataclass
 from datetime import datetime
 from logging import Logger
 from typing import Optional
+from unittest import TestSuite
 
 from ruamel.yaml import YAML  # type: ignore
 
 from . import Step
 from .build.dockerbuild import BuildDocker
 from .build.echo import BuildEcho
 from .build.sbt import BuildSbt
 from .deploy.echo import DeployEcho
+from .deploy.ephemeral_docker_deploy import EphemeralDockerDeploy
 from .deploy.kubernetes import DeployKubernetes
 from .deploy.kubernetes_job import DeployKubernetesJob
+from .deploy.kubernetes_spark_job import DeployKubernetesSparkJob
 from .models import Output, Input, RunProperties, ArtifactType, Artifact
+from .postdeploy.cypress_test import CypressTest
 from .test.dockertest import TestDocker
 from .test.echo import TestEcho
 from .test.sbt import TestSbt
 from ..project import Project
 from ..project import Stage
+from ..utilities.junit import to_test_suites
 from ..validation import validate
 
 yaml = YAML()
 
 
+class ExecutionException(Exception):
+    """ Exception thrown when a step execution fails. """
+
+    def __init__(self, project_name: str, executor: str, stage: str, message: str):
+        self.project_name = project_name
+        self.executor = executor
+        self.stage = stage
+        self.message = message
+        super().__init__(self.message)
+
+
 @dataclass(frozen=True)
 class StepResult:
     stage: Stage
     project: Project
     output: Output
     timestamp: datetime = datetime.now()
 
 
+def collect_test_results(step_results: list[StepResult]) -> list[TestSuite]:
+    test_artifacts = [res.output.produced_artifact for res in step_results if
+                      (res.output.produced_artifact and
+                       res.output.produced_artifact.artifact_type == ArtifactType.JUNIT_TESTS)]
+
+    suites: list[list[TestSuite]] = list(map(to_test_suites, test_artifacts))
+    return list(itertools.chain(*suites))
+
+
 class Steps:
     """ Executor of individual steps within a pipeline. """
     _step_executors: dict[Stage, set[Step]]
     _logger: Logger
     _properties: RunProperties
 
     def __init__(self, logger: Logger, properties: RunProperties) -> None:
@@ -60,21 +85,26 @@
                 TestEcho(logger),
                 TestSbt(logger),
                 TestDocker(logger)
             },
             Stage.DEPLOY: {
                 DeployEcho(logger),
                 DeployKubernetes(logger),
-                DeployKubernetesJob(logger)
+                DeployKubernetesJob(logger),
+                DeployKubernetesSparkJob(logger),
+                EphemeralDockerDeploy(logger)
+            },
+            Stage.POST_DEPLOY: {
+                CypressTest(logger)
             }
         }
 
         self._properties = properties
         for stage, steps in self._step_executors.items():
-            self._logger.debug(f"Registered executors for stage {stage.name}: "
+            self._logger.debug(f"Registered executors for stage {stage.name}: "  # pylint: disable=E1101
                                f"{[step.meta.name for step in steps]}")
 
     def _find_executor(self, stage: Stage, step_name: str) -> Optional[Step]:
         executors = filter(lambda e: e.meta.stage == stage and step_name == e.meta.name, self._step_executors[stage])
         return next(executors, None)
 
     def _execute(self, executor: Step, project: Project, properties: RunProperties,
@@ -96,42 +126,79 @@
         for stage in Stage:
             output: Optional[Output] = Output.try_read(project.target_path, stage)
             if output and output.produced_artifact and output.produced_artifact.artifact_type == required_artifact:
                 return output.produced_artifact
 
         raise ValueError(f"Artifact {required_artifact} required for {project.name} not found")
 
+    def _execute_after_(self, main_result: Output, step: Step, project: Project, stage: Stage,
+                        dry_run: bool = False) -> Output:
+        main_step_artifact = main_result.produced_artifact
+        after_result = self._execute(step, project, self._properties, main_step_artifact, dry_run)
+        if after_result.produced_artifact and after_result.produced_artifact.artifact_type != ArtifactType.NONE:
+            after_result.write(project.target_path, stage)
+        else:
+            after_result.produced_artifact = main_step_artifact
+
+        if not main_result.success:
+            after_result.message = main_result.message
+            after_result.success = False
+
+        return after_result
+
+    def _validate_project_against_config(self, project: Project) -> Optional[Output]:
+        allowed_maintainers = set(self._properties.config.get('project', {}).get('allowedMaintainers', []))
+        not_allowed = set(project.maintainer).difference(allowed_maintainers)
+        if not_allowed:
+            return Output(success=False, message=f"Maintainer(s) '{', '.join(not_allowed)}' not defined in config")
+        return None
+
     def _execute_stage(self, stage: Stage, project: Project, dry_run: bool = False) -> Output:
         stage_name = project.stages.for_stage(stage)
         if stage_name is None:
             return Output(success=False, message=f"Stage '{stage.value}' not defined on project '{project.name}'")
 
-        executor = self._find_executor(stage, stage_name)
+        invalid_maintainers = self._validate_project_against_config(project)
+        if invalid_maintainers:
+            return invalid_maintainers
+
+        executor: Optional[Step] = self._find_executor(stage, stage_name)
         if executor:
             try:
                 self._logger.info(f'Executing {stage} for {project.name}')
                 artifact: Optional[Artifact] = self._find_required_artifact(project, executor.required_artifact)
-                result = Output(success=True, message='')
                 if executor.before:
-                    result = self._execute(executor.before, project, self._properties,
-                                           self._find_required_artifact(project, executor.before.required_artifact),
-                                           dry_run)
-                if result.success:
-                    result = self._execute(executor, project, self._properties, artifact, dry_run)
-                if executor.after:
-                    executor = executor.after
-                    result = self._execute(executor, project, self._properties, result.produced_artifact, dry_run)
+                    before_result = self._execute(executor.before, project, self._properties,
+                                                  self._find_required_artifact(project,
+                                                                               executor.before.required_artifact),
+                                                  dry_run)
+                    if not before_result.success:
+                        return before_result
+
+                result = self._execute(executor, project, self._properties, artifact, dry_run)
                 result.write(project.target_path, stage)
+
+                if executor.after:
+                    return self._execute_after_(result, executor.after, project, stage, dry_run)
+
                 return result
             except Exception as exc:
+                message = str(exc)
                 self._logger.warning(
                     f"Execution of '{executor.meta.name}' for project '{project.name}' in stage {stage} "
-                    f"failed with exception: {str(exc)}", exc_info=True)
-                raise ValueError from exc
+                    f"failed with exception: {message}", exc_info=True)
+                raise ExecutionException(project.name, executor.meta.name, stage.name, message) from exc
         else:
             self._logger.warning(f"No executor found for {stage_name} in stage {stage}")
 
         return Output(success=False, message=f"Executor '{stage_name}' for '{stage.value}' not known or registered")
 
     def execute(self, stage: Stage, project: Project, dry_run: bool = False) -> StepResult:
+        """
+        :param stage: the stage to execute
+        :param project: the project metadata
+        :param dry_run: indicates whether artifacts should be submitted or deployed for real
+        :return: StepResult
+        :raise ExecutionException
+        """
         step_output = self._execute_stage(stage, project, dry_run)
         return StepResult(stage=stage, project=project, output=step_output)
```

## mpyl/steps/build/docker_after_build.py

```diff
@@ -5,15 +5,15 @@
 from logging import Logger
 
 from python_on_whales import docker
 
 from .. import Step, Meta
 from ..models import Input, Output, Artifact, ArtifactType
 from ...project import Stage
-from ...utilities.docker import DockerConfig
+from ...utilities.docker import DockerConfig, login
 
 
 class AfterBuildDocker(Step):
 
     def __init__(self, logger: Logger) -> None:
         super().__init__(logger, Meta(
             name='After Docker Build',
@@ -37,17 +37,15 @@
         artifact = Artifact(ArtifactType.DOCKER_IMAGE, step_input.run_properties.versioning.revision, self.meta.name,
                             {'image': full_image_path})
 
         if step_input.dry_run:
             return Output(success=True, message=f"Dry run. Not pushing {image_name} to {docker_config.host_name}",
                           produced_artifact=artifact)
 
-        self._logger.info(f"Logging in with user '{docker_config.user_name}'")
-        docker.login(server=f'https://{docker_config.host_name}', username=docker_config.user_name,
-                     password=docker_config.password)
+        login(logger=self._logger, docker_config=docker_config)
         image = docker.image.inspect(image_name)
         self._logger.debug(f'Found image {image}')
         docker.image.tag(image, full_image_path)
 
         docker.image.push(full_image_path, quiet=False)
 
         return Output(success=True, message=f"Pushed {full_image_path}", produced_artifact=artifact)
```

## mpyl/steps/build/dockerbuild.py

```diff
@@ -2,15 +2,15 @@
 
 from logging import Logger
 
 from .docker_after_build import AfterBuildDocker
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType, input_to_artifact
 from ...project import Stage
-from ...utilities.docker import DockerConfig, build, docker_image_tag, docker_file_path
+from ...utilities.docker import DockerConfig, build, docker_image_tag, docker_file_path, login
 
 DOCKER_IGNORE_DEFAULT = ['**/target/*', '**/.mpl/*']
 
 
 class BuildDocker(Step):
 
     def __init__(self, logger: Logger) -> None:
@@ -27,14 +27,18 @@
         build_target = docker_config.build_target
         if not build_target:
             raise ValueError('docker.buildTarget must be specified')
 
         image_tag = docker_image_tag(step_input)
         dockerfile = docker_file_path(project=step_input.project, docker_config=docker_config)
 
+        if not step_input.dry_run:
+            # log in to registry, because we may need to pull in a base image
+            login(logger=self._logger, docker_config=docker_config)
+
         success = build(logger=self._logger, root_path=docker_config.root_folder,
                         file_path=dockerfile, image_tag=image_tag,
                         target=build_target)
         artifact = input_to_artifact(ArtifactType.DOCKER_IMAGE, step_input, spec={'image': image_tag})
 
         with open('.dockerignore', 'w+', encoding='utf-8') as ignore_file:
             contents = '\n'.join(DOCKER_IGNORE_DEFAULT)
```

## mpyl/steps/deploy/kubernetes.py

```diff
@@ -1,24 +1,58 @@
 """ Step that deploys the docker image produced in the build stage to Kubernetes, using HELM. """
-
+import re
 from logging import Logger
+from typing import Optional
 
-from .k8s import deploy_helm_chart
+from .k8s import deploy_helm_chart, CustomResourceDefinition
 from .k8s.chart import ChartBuilder, to_service_chart
 from .. import Step, Meta
-from ..models import Input, Output, ArtifactType
+from ..models import Input, Output, ArtifactType, input_to_artifact
 from ...project import Stage
+from ...stages.discovery import find_deploy_set
+from ...utilities.repo import RepoConfig
+
+DEPLOYED_SERVICE_KEY = 'url'
 
 
 class DeployKubernetes(Step):
 
     def __init__(self, logger: Logger) -> None:
         super().__init__(logger, Meta(
             name='Kubernetes Deploy',
             description='Deploy to k8s',
             version='0.0.1',
             stage=Stage.DEPLOY
         ), produced_artifact=ArtifactType.NONE, required_artifact=ArtifactType.DOCKER_IMAGE)
 
+    @staticmethod
+    def match_to_url(match: str) -> str:
+        return 'https://' + next(iter(re.findall(r'`(.*)`', match.split(',')[-1])))
+
+    @staticmethod
+    def try_extract_hostname(chart: dict[str, CustomResourceDefinition]) -> Optional[str]:
+        ingress = chart.get('ingress-https-route')
+        if ingress:
+            routes = ingress.spec.get('routes', {})
+            if routes:
+                match = routes[0].get('match')
+                return DeployKubernetes.match_to_url(match)
+        return None
+
     def execute(self, step_input: Input) -> Output:
-        builder = ChartBuilder(step_input)
-        return deploy_helm_chart(self._logger, to_service_chart(builder), step_input, builder.release_name)
+        builder = ChartBuilder(step_input, find_deploy_set(RepoConfig.from_config(step_input.run_properties.config)))
+        chart = to_service_chart(builder)
+
+        deploy_result = deploy_helm_chart(self._logger, chart, step_input, builder.release_name)
+        if deploy_result.success:
+            hostname = self.try_extract_hostname(chart)
+            spec = {}
+            if hostname:
+                has_specific_routes_configured: bool = bool(builder.deployment.traefik is not None)
+                self._logger.info(f"Service {step_input.project.name} reachable at: {hostname}")
+
+                endpoint = '/' if has_specific_routes_configured else '/swagger/index.html'
+                spec[DEPLOYED_SERVICE_KEY] = f'{hostname}{endpoint}'
+            artifact = input_to_artifact(ArtifactType.DEPLOYED_HELM_APP, step_input, spec=spec)
+            return Output(success=True, message=deploy_result.message, produced_artifact=artifact)
+
+        return deploy_result
```

## mpyl/steps/deploy/kubernetes_job.py

```diff
@@ -1,26 +1,27 @@
 """ A step to deploy a job to kubernetes. """
 
 from logging import Logger
 
 from .k8s import deploy_helm_chart
-from .k8s.chart import ChartBuilder, to_job_chart, to_cron_job_chart
+from .k8s.chart import ChartBuilder, to_cron_job_chart, to_job_chart
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType
 from ...project import Stage
+from ...stages.discovery import find_deploy_set
+from ...utilities.repo import RepoConfig
 
 
 class DeployKubernetesJob(Step):
 
     def __init__(self, logger: Logger) -> None:
         super().__init__(logger, Meta(
             name='Kubernetes Job Deploy',
             description='Deploy a job to k8s',
             version='0.0.1',
             stage=Stage.DEPLOY
         ), produced_artifact=ArtifactType.NONE, required_artifact=ArtifactType.DOCKER_IMAGE)
 
     def execute(self, step_input: Input) -> Output:
-        builder = ChartBuilder(step_input)
-        is_cron_job = builder.deployment.kubernetes and builder.deployment.kubernetes.cron
-        chart = to_cron_job_chart(builder) if is_cron_job else to_job_chart(builder)
-        return deploy_helm_chart(self._logger, chart, step_input, builder.release_name)
+        builder = ChartBuilder(step_input, find_deploy_set(RepoConfig.from_config(step_input.run_properties.config)))
+        chart = to_cron_job_chart(builder) if builder.is_cron_job else to_job_chart(builder)
+        return deploy_helm_chart(self._logger, chart, step_input, builder.release_name, delete_existing=True)
```

## mpyl/steps/deploy/k8s/__init__.py

```diff
@@ -1,36 +1,80 @@
 """Kubernetes deployment related helper methods"""
 from logging import Logger
+from typing import Optional
 
 from kubernetes import config, client
 
-from ...deploy.k8s.resources.crd import CustomResourceDefinition
+from ...deploy.k8s.resources import CustomResourceDefinition
+from ...models import RunProperties
+from ....project import Project, Target, ProjectName
 from ....steps import Input, Output
 from ....steps.deploy.k8s import helm
 from ....steps.deploy.k8s.rancher import cluster_config, rancher_namespace_metadata
 
 
+def get_namespace(run_properties: RunProperties, project: Project) -> Optional[str]:
+    if run_properties.target == Target.PULL_REQUEST:
+        return run_properties.versioning.identifier
+
+    return get_namespace_from_project(project)
+
+
+def get_namespace_from_project(project: Project) -> Optional[str]:
+    if project.deployment and project.deployment.namespace:
+        return project.deployment.namespace
+
+    return None
+
+
 def upsert_namespace(logger: Logger, step_input: Input, context: str):
     properties = step_input.run_properties
 
     config.load_kube_config(context=context)
     logger.info(f"Deploying target {properties.target} and k8s context {context}")
     api = client.CoreV1Api()
 
-    namespace = f'pr-{properties.versioning.pr_number}'
-    meta_data = rancher_namespace_metadata(namespace, properties.target)
-
+    namespace = get_namespace(properties, step_input.project)
+    meta_data = rancher_namespace_metadata(namespace or step_input.project.name, step_input)
     namespaces = api.list_namespace(field_selector=f'metadata.name={namespace}')
+
     if len(namespaces.items) == 0 and not step_input.dry_run:
-        api.create_namespace(
-            client.V1Namespace(api_version='v1', kind='Namespace', metadata=meta_data))
+        api.create_namespace(client.V1Namespace(api_version='v1', kind='Namespace', metadata=meta_data))
     else:
         logger.info(f"Found namespace {namespace}")
+
     return namespace
 
 
 def deploy_helm_chart(logger: Logger, chart: dict[str, CustomResourceDefinition], step_input: Input,
-                      release_name: str) -> Output:
-    properties = step_input.run_properties
-    context = cluster_config(properties.target).context
+                      release_name: str, delete_existing: bool = False) -> Output:
+    context = cluster_config(step_input).context
     namespace = upsert_namespace(logger, step_input, context)
-    return helm.install(logger, chart, step_input, release_name, namespace, context)
+
+    return helm.install(logger, chart, step_input, release_name, namespace, context, delete_existing)
+
+
+def substitute_namespaces(env_vars: dict[str, str], all_projects: set[ProjectName],
+                          projects_to_deploy: set[ProjectName],
+                          pr_identifier: Optional[int]) -> dict[str, str]:
+    env = env_vars.copy()
+
+    def get_namespace_for_linked_project(project_name: ProjectName):
+        is_part_of_same_deploy_set = project_name in projects_to_deploy
+        if is_part_of_same_deploy_set and pr_identifier:
+            return f'pr-{pr_identifier}'
+        return project_name.namespace
+
+    def replace_namespace(env_value, project_name, namespace):
+        search_value = project_name + '.{namespace}'
+        replace_value = project_name + '.' + namespace
+        return env_value.replace(search_value, replace_value)
+
+    for project in all_projects:
+        if project.namespace:
+            linked_project_namespace = get_namespace_for_linked_project(project)
+            for key, value in env.items():
+                replaced_namespace = replace_namespace(value, project.name, linked_project_namespace)
+                updated_pr = replaced_namespace.replace('{PR-NUMBER}',
+                                                        str(pr_identifier)) if pr_identifier else replaced_namespace
+                env[key] = updated_pr
+    return env
```

## mpyl/steps/deploy/k8s/chart.py

```diff
@@ -1,37 +1,62 @@
 """
 Data classes for the composition of Custom Resource Definitions.
 More info: https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/
 """
-
+import itertools
 from dataclasses import dataclass
-from typing import Dict
+from typing import Dict, Optional
 
 from kubernetes.client import V1Deployment, V1Container, V1DeploymentSpec, V1ObjectMeta, V1PodSpec, \
     V1RollingUpdateDeployment, V1LabelSelector, V1ContainerPort, V1EnvVar, V1Service, \
     V1ServiceSpec, V1ServicePort, V1ServiceAccount, V1LocalObjectReference, \
     V1EnvVarSource, V1SecretKeySelector, V1Probe, ApiClient, V1HTTPGetAction, V1ResourceRequirements, \
-    V1PodTemplateSpec, V1DeploymentStrategy, V1Job, V1JobSpec, V1CronJob, V1CronJobSpec, V1JobTemplateSpec
+    V1PodTemplateSpec, V1DeploymentStrategy, V1Job, V1JobSpec, V1CronJob, V1CronJobSpec, V1JobTemplateSpec, V1ConfigMap
 from ruamel.yaml import YAML
 
-from .resources.crd import CustomResourceDefinition, to_dict  # pylint: disable = no-name-in-module
-from .resources.customresources import V1AlphaIngressRoute, V1SealedSecret  # pylint: disable = no-name-in-module
+from . import substitute_namespaces
+from .resources import CustomResourceDefinition, to_dict  # pylint: disable = no-name-in-module
+from .resources.sealed_secret import V1SealedSecret
+from .resources.spark import to_spark_body, get_spark_config_map_data, V1SparkApplication
+from .resources.traefik import V1AlphaIngressRoute, V1AlphaMiddleware, \
+    HostWrapper  # pylint: disable = no-name-in-module
 from ...models import Input, ArtifactType
-from ....project import Project, KeyValueProperty, Probe, Deployment, TargetProperty, Resources, Target
+from ....project import Project, KeyValueProperty, Probe, Deployment, TargetProperty, Resources, Target, Kubernetes, \
+    Job, Traefik, Host, get_env_variables
+from ....stages.discovery import DeploySet
 
 yaml = YAML()
 
 # Determined (unscientifically) to be sensible factors.
 # Based on actual CPU usage, pods rarely use more than 10% of the allocated CPU. 60% usage is healthy, so we
 # scale down to 20% in order to keep some slack.
 # Memory is cheaper, but poses a harder limit (OOM when exceeding limit), so we are more generous than with CPU.
 CPU_REQUEST_SCALE_FACTOR = 0.2
 MEM_REQUEST_SCALE_FACTOR = 0.5
 
 
+def try_parse_target(value: object, target: Target):
+    if isinstance(value, dict):
+        maybe_value = TargetProperty.from_config(value).get_value(target)
+        if maybe_value:
+            return maybe_value
+
+    return value
+
+
+def with_target(dictionary: dict, target: Target) -> dict:
+    def with_targets_parsed(obj):
+        if isinstance(obj, dict):
+            return type(obj)((k, try_parse_target(with_targets_parsed(v), target)) for k, v in obj.items())
+
+        return obj
+
+    return with_targets_parsed(dictionary)
+
+
 @dataclass(frozen=True)
 class ResourceDefaults:
     instances: TargetProperty[int]
     cpus: TargetProperty[float]
     mem: TargetProperty[int]
 
     @staticmethod
@@ -39,61 +64,71 @@
         limit = resources['limit']
         return ResourceDefaults(instances=TargetProperty.from_config(resources['instances']),
                                 cpus=TargetProperty.from_config(limit['cpus']),
                                 mem=TargetProperty.from_config(limit['mem']))
 
 
 @dataclass(frozen=True)
-class KubernetesConfig:
+class DeploymentDefaults:
     resources_defaults: ResourceDefaults
     liveness_probe_defaults: dict
     startup_probe_defaults: dict
+    job_defaults: dict
+    treafik_defaults: dict
+    white_lists: dict
 
     @staticmethod
-    def from_config(values: dict):
-        return KubernetesConfig(resources_defaults=ResourceDefaults.from_config(values['resources']),
-                                liveness_probe_defaults=values['livenessProbe'],
-                                startup_probe_defaults=values['startupProbe'])
+    def from_config(config: dict):
+        deployment_values = config.get('project', {}).get('deployment', {})
+        if deployment_values is None:
+            raise KeyError("Configuration should have project.deployment section")
+        kubernetes = deployment_values.get('kubernetes', {})
+        return DeploymentDefaults(
+            resources_defaults=ResourceDefaults.from_config(kubernetes['resources']),
+            liveness_probe_defaults=kubernetes['livenessProbe'],
+            startup_probe_defaults=kubernetes['startupProbe'],
+            job_defaults=kubernetes.get('job', {}),
+            treafik_defaults=deployment_values.get('traefik', {}),
+            white_lists=config.get('whiteLists', {})
+        )
 
 
 class ChartBuilder:
     step_input: Input
     project: Project
     mappings: dict[int, int]
     env: list[KeyValueProperty]
     sealed_secrets: list[KeyValueProperty]
     deployment: Deployment
     target: Target
     release_name: str
-    kubernetes_config: KubernetesConfig
+    config_defaults: DeploymentDefaults
+    deploy_set: Optional[DeploySet]
 
-    def __init__(self, step_input: Input):
+    def __init__(self, step_input: Input, deploy_set: Optional[DeploySet] = None):
         self.step_input = step_input
         project = self.step_input.project
         self.project = project
         if project.deployment is None:
             raise AttributeError("deployment field should be set")
-        kubernetes_config_dict = step_input.run_properties.config.get('project', {}).get('deployment', {}).get(
-            'kubernetes', {})
-        if kubernetes_config_dict is None:
-            raise KeyError("Configuration should have project.deployment.kubernetes section")
 
-        self.kubernetes_config = KubernetesConfig.from_config(kubernetes_config_dict)
+        self.config_defaults = DeploymentDefaults.from_config(step_input.run_properties.config)
 
         self.deployment = project.deployment
         properties = self.deployment.properties
         self.env = properties.env if properties and properties.env else []
         self.sealed_secrets = properties.sealed_secret if properties and properties.sealed_secret else []
         self.mappings = self.project.kubernetes.port_mappings
         self.target = step_input.run_properties.target
         self.release_name = self.project.name.lower()
+        self.deploy_set = deploy_set
 
     def _to_labels(self) -> Dict:
         run_properties = self.step_input.run_properties
-        app_labels = {'name': self.project.name, 'app.kubernetes.io/version': run_properties.versioning.identifier,
+        app_labels = {'name': self.release_name, 'app.kubernetes.io/version': run_properties.versioning.identifier,
                       'app.kubernetes.io/managed-by': 'Helm', 'app.kubernetes.io/name': self.release_name,
                       'app.kubernetes.io/instance': self.release_name}
 
         if len(self.project.maintainer) > 0:
             app_labels['maintainers'] = ".".join(self.project.maintainer).replace(' ', '_')
             app_labels["maintainer"] = self.project.maintainer[0].replace(' ', '_')
 
@@ -103,16 +138,16 @@
             app_labels['revision'] = run_properties.versioning.revision
 
         return app_labels
 
     def _to_annotations(self) -> Dict:
         return {'description': self.project.description}
 
-    def _to_object_meta(self):
-        return V1ObjectMeta(name=self.project.name, labels=self._to_labels())
+    def _to_object_meta(self, name: Optional[str] = None):
+        return V1ObjectMeta(name=name if name else self.release_name, labels=self._to_labels())
 
     def _to_selector(self):
         return V1LabelSelector(match_labels={"app.kubernetes.io/instance": self.release_name,
                                              "app.kubernetes.io/name": self.release_name})
 
     @staticmethod
     def _to_k8s_model(values: dict, model_type):
@@ -127,45 +162,112 @@
         v1_probe.http_get = V1HTTPGetAction(path='/health' if path is None else path, port='port-0')
         return v1_probe
 
     def to_service(self) -> V1Service:
         service_ports = list(map(lambda key: V1ServicePort(port=key, target_port=self.mappings[key], protocol="TCP",
                                                            name=f"{key}-webservice-port"), self.mappings.keys()))
 
-        return V1Service(api_version='v1', kind='Service', metadata=self._to_object_meta(),
+        return V1Service(api_version='v1', kind='Service',
+                         metadata=V1ObjectMeta(annotations=self._to_annotations(), name=self.release_name,
+                                               labels=self._to_labels()),
                          spec=V1ServiceSpec(type="ClusterIP", ports=service_ports,
                                             selector=self._to_selector().match_labels))
 
     def to_job(self) -> V1Job:
         job_container = V1Container(
-            name=self.project.name, image=self._get_image(), env=self._get_env_vars(), image_pull_policy="Always",
+            name=self.release_name, image=self._get_image(), env=self._get_env_vars(), image_pull_policy="Always",
             resources=self._get_resources()
         )
         pod_template = V1PodTemplateSpec(
             metadata=self._to_object_meta(),
             spec=V1PodSpec(containers=[job_container], service_account=self.release_name,
-                           service_account_name=self.release_name),
+                           service_account_name=self.release_name, restart_policy="Never")
         )
-        return V1Job(api_version='batch/v1', kind='Job', metadata=self._to_object_meta(),
-                     spec=V1JobSpec(ttl_seconds_after_finished=3600, template=pod_template))
+
+        defaults = with_target(self.config_defaults.job_defaults, self.target)
+        specified = defaults | with_target(self.project.job.job, self.target)
+
+        template_dict = to_dict(pod_template)
+        specified['template'] = template_dict
+        spec: V1JobSpec = ChartBuilder._to_k8s_model(specified, V1JobSpec)
+
+        return V1Job(api_version='batch/v1', kind='Job', metadata=self._to_object_meta(), spec=spec)
 
     def to_cron_job(self) -> V1CronJob:
-        values = self._get_kubernetes().cron
+        values = self.project.job.cron
         job_template = V1JobTemplateSpec(spec=self.to_job().spec)
         template_dict = to_dict(job_template)
         values['jobTemplate'] = template_dict
         v1_cron_job_spec: V1CronJobSpec = ChartBuilder._to_k8s_model(values, V1CronJobSpec)
         return V1CronJob(api_version='batch/v1', kind='CronJob', metadata=self._to_object_meta(), spec=v1_cron_job_spec)
 
+    def to_spark_application(self) -> V1SparkApplication:
+        return V1SparkApplication(
+            schedule=self._get_job().cron['schedule'],
+            body=to_spark_body(
+                project_name=self.release_name,
+                env_vars=get_env_variables(self.project, self.target),
+                spark=self._get_job().spark
+            ),
+        )
+
+    def to_spark_config_map(self) -> V1ConfigMap:
+        return V1ConfigMap(
+            api_version='v1',
+            kind='ConfigMap',
+            data=get_spark_config_map_data(),
+            metadata=self._to_object_meta()
+        )
+
+    def __find_default_port(self) -> int:
+        found = next(iter(self.mappings.keys()))
+        if found:
+            return int(found)
+        raise KeyError("No default port found. Did you define a port mapping?")
+
+    def create_host_wrappers(self) -> list[HostWrapper]:
+        default_hosts: list[Host] = Traefik.from_config(self.config_defaults.treafik_defaults).hosts
+
+        hosts: list[Host] = self.deployment.traefik.hosts if self.deployment.traefik else []
+
+        first_host = next(iter(hosts), None)
+        service_port = first_host.service_port if first_host and first_host.service_port else self.__find_default_port()
+
+        configured_addresses = self.config_defaults.white_lists['addresses']
+        address_dictionary = {address['name']: address['values'] for address in configured_addresses}
+
+        def to_white_list(configured: Optional[TargetProperty[list[str]]]) -> dict[str, list[str]]:
+            white_lists = self.config_defaults.white_lists['default'].copy()
+            if configured and configured.get_value(self.target):
+                white_lists.extend(configured.get_value(self.target))
+
+            return dict(filter(lambda x: x[0] in white_lists, address_dictionary.items()))
+
+        return [HostWrapper(host=host, name=self.release_name, index=idx, service_port=service_port,
+                            white_lists=to_white_list(host.whitelists)) for
+                idx, host in enumerate(hosts if hosts else default_hosts)]
+
     def to_ingress_routes(self) -> V1AlphaIngressRoute:
-        if self.deployment.traefik is None:
-            raise AttributeError("deployment.traefik field should be set")
+        hosts = self.create_host_wrappers()
 
-        return V1AlphaIngressRoute(metadata=self._to_object_meta(), hosts=self.deployment.traefik.hosts,
-                                   service_port=123, name=self.release_name, target=self.target)
+        return V1AlphaIngressRoute(metadata=self._to_object_meta(), hosts=hosts, target=self.target,
+                                   pr_number=self.step_input.run_properties.versioning.pr_number)
+
+    def to_middlewares(self) -> dict[str, V1AlphaMiddleware]:
+        hosts: list[HostWrapper] = self.create_host_wrappers()
+
+        def to_metadata(host: HostWrapper) -> V1ObjectMeta:
+            metadata = self._to_object_meta(name=host.full_name)
+            # metadata.annotations = host.white_lists
+            metadata.annotations = {k: ", ".join(v) for k, v in host.white_lists.items()}
+            return metadata
+
+        return {host.full_name: V1AlphaMiddleware(
+            metadata=to_metadata(host),
+            source_ranges=list(itertools.chain(*host.white_lists.values()))) for host in hosts}
 
     def to_service_account(self) -> V1ServiceAccount:
         return V1ServiceAccount(api_version="v1", kind="ServiceAccount", metadata=self._to_object_meta(),
                                 image_pull_secrets=[V1LocalObjectReference("bigdataregistry")])
 
     def to_sealed_secrets(self) -> V1SealedSecret:
         secrets: dict[str, str] = {}
@@ -185,63 +287,84 @@
         mem_request = mem_limit * MEM_REQUEST_SCALE_FACTOR
         return V1ResourceRequirements(limits={'cpu': f'{int(cpus_limit)}m', 'memory': f'{int(mem_limit)}Mi'},
                                       requests={'cpu': f'{int(cpus_request)}m', 'memory': f'{int(mem_request)}Mi'})
 
     def _get_image(self):
         docker_image = self.step_input.required_artifact
         if not docker_image or docker_image.artifact_type != ArtifactType.DOCKER_IMAGE:
-            raise ValueError(f'Required artifact of type {ArtifactType.DOCKER_IMAGE.name} must be defined')
+            raise ValueError(
+                f'Required artifact of type {ArtifactType.DOCKER_IMAGE.name} must be defined')  # pylint: disable=E1101
         return docker_image.spec['image']
 
-    def _get_kubernetes(self):
+    def _get_resources(self):
+        resources = self.project.kubernetes.resources
+        defaults = self.config_defaults.resources_defaults
+        return ChartBuilder._to_resources(resources, defaults, self.target)
+
+    def _get_kubernetes(self) -> Kubernetes:
         kubernetes = self.deployment.kubernetes
         if kubernetes is None:
             raise AttributeError("deployment.kubernetes field should be set")
         return kubernetes
 
-    def _get_resources(self):
-        kubernetes = self._get_kubernetes()
-        resources = kubernetes.resources
-        defaults = self.kubernetes_config.resources_defaults
-        return ChartBuilder._to_resources(resources, defaults, self.target)
+    def _get_job(self) -> Job:
+        job = self._get_kubernetes().job
+        if job is None:
+            raise AttributeError("deployment.kubernetes.job field should be set")
+        return job
 
     def _get_env_vars(self):
-        env_vars = list(
-            filter(lambda v: v.value, map(lambda e: V1EnvVar(name=e.key, value=e.get_value(self.target)), self.env)))
+        raw_env_vars = {e.key: e.get_value(self.target) for e in self.env if e.get_value(self.target) is not None}
+        substituted = substitute_namespaces(raw_env_vars,
+                                            {p.to_name for p in self.deploy_set.all_projects},
+                                            {p.to_name for p in self.deploy_set.projects_to_deploy},
+                                            self.step_input.run_properties.versioning.pr_number)
+
+        env_vars = [V1EnvVar(name=key, value=value) for key, value in substituted.items()]
+
         sealed_for_target = list(
             filter(lambda v: v.get_value(self.target) is not None, self.sealed_secrets))
         sealed_secrets = list(map(lambda e: V1EnvVar(name=e.key, value_from=V1EnvVarSource(
             secret_key_ref=V1SecretKeySelector(key=e.key, name=self.release_name, optional=False))),
                                   sealed_for_target))
         return env_vars + sealed_secrets
 
+    @property
+    def is_cron_job(self) -> bool:
+        return len(self._get_job().cron.keys()) > 0
+
     def to_deployment(self) -> V1Deployment:
 
         ports = [
-            V1ContainerPort(container_port=key, host_port=self.mappings[key], protocol="TCP", name=f'port-{idx}')
+            V1ContainerPort(container_port=self.mappings[key], host_port=key, protocol="TCP", name=f'port-{idx}')
             for idx, key in enumerate(self.mappings.keys())
         ]
 
-        kubernetes = self._get_kubernetes()
-        resources = kubernetes.resources
-        defaults = self.kubernetes_config.resources_defaults
+        project = self.project
+        resources = project.resources
+        kubernetes = project.kubernetes
+        defaults = self.config_defaults.resources_defaults
 
         container = V1Container(
-            name=self.project.name,
+            name=self.release_name,
             image=self._get_image(),
             env=self._get_env_vars(),
             ports=ports,
             image_pull_policy="Always",
             resources=ChartBuilder._to_resources(resources, defaults, self.target),
-            liveness_probe=ChartBuilder._to_probe(kubernetes.liveness_probe,
-                                                  self.kubernetes_config.liveness_probe_defaults,
-                                                  self.target) if kubernetes.liveness_probe else None,
-            startup_probe=ChartBuilder._to_probe(kubernetes.startup_probe,
-                                                 self.kubernetes_config.startup_probe_defaults,
-                                                 self.target) if kubernetes.startup_probe else None
+            liveness_probe=ChartBuilder._to_probe(
+                kubernetes.liveness_probe,
+                self.config_defaults.liveness_probe_defaults,
+                self.target
+            ) if kubernetes.liveness_probe else None,
+            startup_probe=ChartBuilder._to_probe(
+                kubernetes.startup_probe,
+                self.config_defaults.startup_probe_defaults,
+                self.target)
+            if kubernetes.startup_probe else None
         )
 
         instances = resources.instances if resources.instances else defaults.instances
 
         return V1Deployment(
             api_version="apps/v1",
             kind="Deployment",
@@ -257,36 +380,37 @@
                 strategy=V1DeploymentStrategy(
                     rolling_update=V1RollingUpdateDeployment(max_surge="25%", max_unavailable="25%"),
                     type="RollingUpdate"),
                 selector=self._to_selector(),
             ),
         )
 
+    def to_common_chart(self) -> dict[str, CustomResourceDefinition]:
+        chart = {'service-account': self.to_service_account()}
 
-def to_service_chart(builder: ChartBuilder) -> dict[str, CustomResourceDefinition]:
-    chart = {'deployment': builder.to_deployment(), 'serviceaccount': builder.to_service_account(),
-             'service': builder.to_service()}
-    if builder.sealed_secrets:
-        chart['sealedsecrets'] = builder.to_sealed_secrets()
-
-    if builder.deployment.traefik:
-        chart['ingress-https-route'] = builder.to_ingress_routes()
+        if self.sealed_secrets:
+            chart['sealed-secrets'] = self.to_sealed_secrets()
 
-    return chart
+        return chart
 
 
-def to_job_chart(builder: ChartBuilder) -> dict[str, CustomResourceDefinition]:
-    chart = {'job': builder.to_job(), 'serviceaccount': builder.to_service_account()}
+def to_service_chart(builder: ChartBuilder) -> dict[str, CustomResourceDefinition]:
+    return builder.to_common_chart() | {
+        'deployment': builder.to_deployment(),
+        'service': builder.to_service(),
+        'ingress-https-route': builder.to_ingress_routes()
+    } | builder.to_middlewares()
 
-    if builder.sealed_secrets:
-        chart['sealedsecrets'] = builder.to_sealed_secrets()
 
-    return chart
+def to_job_chart(builder: ChartBuilder) -> dict[str, CustomResourceDefinition]:
+    return builder.to_common_chart() | {'job': builder.to_job()}
 
 
 def to_cron_job_chart(builder: ChartBuilder) -> dict[str, CustomResourceDefinition]:
-    chart = {'cronjob': builder.to_cron_job(), 'serviceaccount': builder.to_service_account()}
+    return builder.to_common_chart() | {'cronjob': builder.to_cron_job()}
 
-    if builder.sealed_secrets:
-        chart['sealedsecrets'] = builder.to_sealed_secrets()
 
-    return chart
+def to_spark_job_chart(builder: ChartBuilder) -> dict[str, CustomResourceDefinition]:
+    return builder.to_common_chart() | {
+        'spark': builder.to_spark_application(),
+        'config-map': builder.to_spark_config_map()
+    }
```

## mpyl/steps/deploy/k8s/helm.py

```diff
@@ -2,15 +2,15 @@
 step.
 """
 
 import shutil
 from logging import Logger
 from pathlib import Path
 
-from .resources.crd import to_yaml, CustomResourceDefinition
+from .resources import to_yaml, CustomResourceDefinition
 from ...models import RunProperties, Output, Input
 from ....utilities.subprocess import custom_check_output
 
 
 def to_chart_metadata(chart_name: str, run_properties: RunProperties):
     return f"""apiVersion: v3
 name: {chart_name}
@@ -34,17 +34,31 @@
     my_dictionary: dict[str, str] = dict(map(lambda item: (item[0], to_yaml(item[1])), chart.items()))
 
     for name, template in my_dictionary.items():
         with open(template_path / name, mode='w+', encoding='utf-8') as file:
             file.write(template)
 
 
+def __remove_existing_chart(logger: Logger, chart_name: str, name_space: str, kube_context: str) -> Output:
+    found_chart = custom_check_output(logger, f"helm list -f ^{chart_name}$ -n {name_space}", capture_stdout=True)
+    if chart_name in found_chart.message:
+        cmd = f"helm uninstall {chart_name} -n {name_space} --kube-context {kube_context}"
+        return custom_check_output(Logger("helm"), cmd)
+    return Output(success=True, message=f"No existing chart {chart_name} found to delete")
+
+
 def install(logger: Logger, chart: dict[str, CustomResourceDefinition], step_input: Input, chart_name: str,
-            name_space: str, kube_context: str) -> Output:
+            name_space: str, kube_context: str, delete_existing: bool = False) -> Output:
+    if delete_existing:
+        removed = __remove_existing_chart(logger, chart_name, name_space, kube_context)
+        if not removed.success:
+            return removed
+
     chart_path = Path(step_input.project.target_path) / "chart"
+    logger.info(f"Writing HELM chart to {chart_path}")
     write_chart(chart, chart_path, to_chart_metadata(chart_name, step_input.run_properties))
 
     cmd = f"helm upgrade -i {chart_name} -n {name_space} --kube-context {kube_context} {chart_path}"
     if step_input.dry_run:
         cmd = f"helm upgrade -i {chart_name} -n namespace --kube-context {kube_context} {chart_path} --debug --dry-run"
 
     return custom_check_output(logger, cmd)
```

## mpyl/steps/deploy/k8s/rancher.py

```diff
@@ -1,37 +1,44 @@
 """ Utilities for creating rancher compatible helm charts. """
 
 from dataclasses import dataclass
 
+from ....steps import Input
 from ....project import Target
 
 
 @dataclass(frozen=True)
 class ClusterConfig:
     project_id: str
     cluster_id: str
     cluster_env: str
     context: str
 
+    @staticmethod
+    def from_config(config: dict):
+        return ClusterConfig(project_id=config['clusterId'], cluster_id=config['clusterId'],
+                             cluster_env=config['clusterEnv'], context=config['context'])
+
+
+def cluster_config(step_input: Input):
+    target = step_input.run_properties.target
+    cluster_configs = step_input.run_properties.config['kubernetes']['rancher']['cluster']
 
-def cluster_config(target: Target):
     if target in {Target.PULL_REQUEST, Target.PULL_REQUEST_BASE}:
-        return ClusterConfig(cluster_id='c-z8wzm', project_id='p-k9l47', cluster_env="test",
-                             context="vdb-core-digital-k8s-test")
+        return ClusterConfig.from_config(cluster_configs['test'])
     if target == Target.ACCEPTANCE:
-        return ClusterConfig(cluster_id='c-6mkzg', project_id='p-ckqxz', cluster_env="acce",
-                             context="vdb-core-digital-k8s-acce")
+        return ClusterConfig.from_config(cluster_configs['acceptance'])
     if target == Target.PRODUCTION:
-        return ClusterConfig(cluster_id='c-r8bj6', project_id='p-lb52t', cluster_env="prd",
-                             context="vdb-core-digital-k8s-prod")
+        return ClusterConfig.from_config(cluster_configs['production'])
     return None
 
 
-def rancher_namespace_metadata(namespace: str, target: Target):
-    rancher_config = cluster_config(target)
+def rancher_namespace_metadata(namespace: str, step_input: Input):
+    rancher_config = cluster_config(step_input)
+
     return {
         'annotations': {
             'field.cattle.io/projectId': f'{rancher_config.cluster_id}:{rancher_config.project_id}',
             'lifecycle.cattle.io/create.namespace-auth': 'true'
         },
         'labels': {
             'field.cattle.io/projectId': rancher_config.project_id,
```

## mpyl/steps/deploy/k8s/resources/__init__.py

```diff
@@ -0,0 +1,280 @@
+00000000: 2222 220a 4375 7374 6f6d 2052 6573 6f75  """.Custom Resou
+00000010: 7263 6520 4465 6669 6e69 7469 6f6e 732c  rce Definitions,
+00000020: 2061 6c6c 6f77 2079 6f75 2074 6f20 6372   allow you to cr
+00000030: 6561 7465 2063 7573 746f 6d20 6b38 7320  eate custom k8s 
+00000040: 7265 736f 7572 6365 732c 2062 6573 6964  resources, besid
+00000050: 6573 2074 6865 2064 6566 6175 6c74 206f  es the default o
+00000060: 6e65 732e 0a54 6869 7320 6973 2075 7365  nes..This is use
+00000070: 6675 6c20 666f 7220 6578 616d 706c 6520  ful for example 
+00000080: 7768 656e 2079 6f75 2077 616e 7420 746f  when you want to
+00000090: 2063 6f6e 6669 6775 7265 2061 2073 7065   configure a spe
+000000a0: 6369 6669 6320 6f70 6572 6174 6f72 2c20  cific operator, 
+000000b0: 6c69 6b65 2053 7061 726b 206f 7220 7365  like Spark or se
+000000c0: 616c 6564 2073 6563 7265 7473 2e0a 2222  aled secrets..""
+000000d0: 220a 696d 706f 7274 2070 6b67 7574 696c  ".import pkgutil
+000000e0: 0a66 726f 6d20 696f 2069 6d70 6f72 7420  .from io import 
+000000f0: 5374 7269 6e67 494f 0a66 726f 6d20 7479  StringIO.from ty
+00000100: 7069 6e67 2069 6d70 6f72 7420 4f70 7469  ping import Opti
+00000110: 6f6e 616c 0a0a 696d 706f 7274 206a 736f  onal..import jso
+00000120: 6e73 6368 656d 610a 696d 706f 7274 2073  nschema.import s
+00000130: 6978 0a66 726f 6d20 6a73 6f6e 7363 6865  ix.from jsonsche
+00000140: 6d61 2069 6d70 6f72 7420 5661 6c69 6461  ma import Valida
+00000150: 7469 6f6e 4572 726f 720a 6672 6f6d 206b  tionError.from k
+00000160: 7562 6572 6e65 7465 732e 636c 6965 6e74  ubernetes.client
+00000170: 2069 6d70 6f72 7420 436f 6e66 6967 7572   import Configur
+00000180: 6174 696f 6e2c 2056 314f 626a 6563 744d  ation, V1ObjectM
+00000190: 6574 610a 6672 6f6d 2072 7561 6d65 6c2e  eta.from ruamel.
+000001a0: 7961 6d6c 2069 6d70 6f72 7420 5941 4d4c  yaml import YAML
+000001b0: 0a0a 7961 6d6c 203d 2059 414d 4c28 290a  ..yaml = YAML().
+000001c0: 0a0a 636c 6173 7320 4375 7374 6f6d 5265  ..class CustomRe
+000001d0: 736f 7572 6365 4465 6669 6e69 7469 6f6e  sourceDefinition
+000001e0: 3a0a 2020 2020 6f70 656e 6170 695f 7479  :.    openapi_ty
+000001f0: 7065 7320 3d20 7b0a 2020 2020 2020 2020  pes = {.        
+00000200: 2761 7069 5f76 6572 7369 6f6e 273a 2027  'api_version': '
+00000210: 7374 7227 2c0a 2020 2020 2020 2020 276b  str',.        'k
+00000220: 696e 6427 3a20 2773 7472 272c 0a20 2020  ind': 'str',.   
+00000230: 2020 2020 2027 6d65 7461 6461 7461 273a       'metadata':
+00000240: 2027 5631 4f62 6a65 6374 4d65 7461 272c   'V1ObjectMeta',
+00000250: 0a20 2020 2020 2020 2027 7370 6563 273a  .        'spec':
+00000260: 2027 6469 6374 270a 2020 2020 7d0a 0a20   'dict'.    }.. 
+00000270: 2020 2061 7474 7269 6275 7465 5f6d 6170     attribute_map
+00000280: 203d 207b 0a20 2020 2020 2020 2027 6170   = {.        'ap
+00000290: 695f 7665 7273 696f 6e27 3a20 2761 7069  i_version': 'api
+000002a0: 5665 7273 696f 6e27 2c0a 2020 2020 2020  Version',.      
+000002b0: 2020 276b 696e 6427 3a20 276b 696e 6427    'kind': 'kind'
+000002c0: 2c0a 2020 2020 2020 2020 276d 6574 6164  ,.        'metad
+000002d0: 6174 6127 3a20 276d 6574 6164 6174 6127  ata': 'metadata'
+000002e0: 2c0a 2020 2020 2020 2020 2773 7065 6327  ,.        'spec'
+000002f0: 3a20 2773 7065 6327 0a20 2020 207d 0a0a  : 'spec'.    }..
+00000300: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00000310: 2873 656c 662c 2061 7069 5f76 6572 7369  (self, api_versi
+00000320: 6f6e 3a20 7374 722c 206b 696e 643a 2073  on: str, kind: s
+00000330: 7472 2c20 6d65 7461 6461 7461 3a20 5631  tr, metadata: V1
+00000340: 4f62 6a65 6374 4d65 7461 2c20 7370 6563  ObjectMeta, spec
+00000350: 3a20 6469 6374 2c0a 2020 2020 2020 2020  : dict,.        
+00000360: 2020 2020 2020 2020 206c 6f63 616c 5f76           local_v
+00000370: 6172 735f 636f 6e66 6967 7572 6174 696f  ars_configuratio
+00000380: 6e3d 4e6f 6e65 2c20 7363 6865 6d61 3a20  n=None, schema: 
+00000390: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000003a0: 4e6f 6e65 293a 2020 2320 6e6f 7161 3a20  None):  # noqa: 
+000003b0: 4535 3031 0a20 2020 2020 2020 2022 2222  E501.        """
+000003c0: 5631 4353 4944 7269 7665 7220 2d20 6120  V1CSIDriver - a 
+000003d0: 6d6f 6465 6c20 6465 6669 6e65 6420 696e  model defined in
+000003e0: 204f 7065 6e41 5049 2222 2220 2023 206e   OpenAPI"""  # n
+000003f0: 6f71 613a 2045 3530 310a 2020 2020 2020  oqa: E501.      
+00000400: 2020 6966 206c 6f63 616c 5f76 6172 735f    if local_vars_
+00000410: 636f 6e66 6967 7572 6174 696f 6e20 6973  configuration is
+00000420: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00000430: 2020 206c 6f63 616c 5f76 6172 735f 636f     local_vars_co
+00000440: 6e66 6967 7572 6174 696f 6e20 3d20 436f  nfiguration = Co
+00000450: 6e66 6967 7572 6174 696f 6e28 290a 2020  nfiguration().  
+00000460: 2020 2020 2020 7365 6c66 2e6c 6f63 616c        self.local
+00000470: 5f76 6172 735f 636f 6e66 6967 7572 6174  _vars_configurat
+00000480: 696f 6e20 3d20 6c6f 6361 6c5f 7661 7273  ion = local_vars
+00000490: 5f63 6f6e 6669 6775 7261 7469 6f6e 0a0a  _configuration..
+000004a0: 2020 2020 2020 2020 7365 6c66 2e5f 6170          self._ap
+000004b0: 695f 7665 7273 696f 6e20 3d20 6170 695f  i_version = api_
+000004c0: 7665 7273 696f 6e0a 2020 2020 2020 2020  version.        
+000004d0: 7365 6c66 2e5f 6b69 6e64 203d 206b 696e  self._kind = kin
+000004e0: 640a 2020 2020 2020 2020 7365 6c66 2e5f  d.        self._
+000004f0: 6d65 7461 6461 7461 203d 206d 6574 6164  metadata = metad
+00000500: 6174 610a 2020 2020 2020 2020 7365 6c66  ata.        self
+00000510: 2e5f 7370 6563 203d 2073 7065 630a 2020  ._spec = spec.  
+00000520: 2020 2020 2020 7365 6c66 2e5f 7363 6865        self._sche
+00000530: 6d61 203d 2073 6368 656d 610a 2020 2020  ma = schema.    
+00000540: 2020 2020 7365 6c66 2e64 6973 6372 696d      self.discrim
+00000550: 696e 6174 6f72 203d 204e 6f6e 650a 0a20  inator = None.. 
+00000560: 2020 2020 2020 2069 6620 6170 695f 7665         if api_ve
+00000570: 7273 696f 6e20 6973 206e 6f74 204e 6f6e  rsion is not Non
+00000580: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00000590: 656c 662e 6170 695f 7665 7273 696f 6e20  elf.api_version 
+000005a0: 3d20 6170 695f 7665 7273 696f 6e0a 2020  = api_version.  
+000005b0: 2020 2020 2020 6966 206b 696e 6420 6973        if kind is
+000005c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000005d0: 2020 2020 2020 2073 656c 662e 6b69 6e64         self.kind
+000005e0: 203d 206b 696e 640a 2020 2020 2020 2020   = kind.        
+000005f0: 6966 206d 6574 6164 6174 6120 6973 206e  if metadata is n
+00000600: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00000610: 2020 2020 2073 656c 662e 6d65 7461 6461       self.metada
+00000620: 7461 203d 206d 6574 6164 6174 610a 0a20  ta = metadata.. 
+00000630: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00000640: 2064 6566 2073 6368 656d 6128 7365 6c66   def schema(self
+00000650: 2920 2d3e 204f 7074 696f 6e61 6c5b 7374  ) -> Optional[st
+00000660: 725d 3a0a 2020 2020 2020 2020 7265 7475  r]:.        retu
+00000670: 726e 2073 656c 662e 5f73 6368 656d 610a  rn self._schema.
+00000680: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00000690: 2020 2064 6566 2061 7069 5f76 6572 7369     def api_versi
+000006a0: 6f6e 2873 656c 6629 202d 3e20 7374 723a  on(self) -> str:
+000006b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000006c0: 7365 6c66 2e5f 6170 695f 7665 7273 696f  self._api_versio
+000006d0: 6e0a 0a20 2020 2040 6170 695f 7665 7273  n..    @api_vers
+000006e0: 696f 6e2e 7365 7474 6572 0a20 2020 2064  ion.setter.    d
+000006f0: 6566 2061 7069 5f76 6572 7369 6f6e 2873  ef api_version(s
+00000700: 656c 662c 2061 7069 5f76 6572 7369 6f6e  elf, api_version
+00000710: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00000720: 5f61 7069 5f76 6572 7369 6f6e 203d 2061  _api_version = a
+00000730: 7069 5f76 6572 7369 6f6e 0a0a 2020 2020  pi_version..    
+00000740: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00000750: 6620 6b69 6e64 2873 656c 6629 202d 3e20  f kind(self) -> 
+00000760: 7374 723a 0a20 2020 2020 2020 2072 6574  str:.        ret
+00000770: 7572 6e20 7365 6c66 2e5f 6b69 6e64 0a0a  urn self._kind..
+00000780: 2020 2020 406b 696e 642e 7365 7474 6572      @kind.setter
+00000790: 0a20 2020 2064 6566 206b 696e 6428 7365  .    def kind(se
+000007a0: 6c66 2c20 6b69 6e64 293a 0a20 2020 2020  lf, kind):.     
+000007b0: 2020 2073 656c 662e 5f6b 696e 6420 3d20     self._kind = 
+000007c0: 6b69 6e64 0a0a 2020 2020 4070 726f 7065  kind..    @prope
+000007d0: 7274 790a 2020 2020 6465 6620 6d65 7461  rty.    def meta
+000007e0: 6461 7461 2873 656c 6629 202d 3e20 5631  data(self) -> V1
+000007f0: 4f62 6a65 6374 4d65 7461 3a0a 2020 2020  ObjectMeta:.    
+00000800: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00000810: 5f6d 6574 6164 6174 610a 0a20 2020 2040  _metadata..    @
+00000820: 6d65 7461 6461 7461 2e73 6574 7465 720a  metadata.setter.
+00000830: 2020 2020 6465 6620 6d65 7461 6461 7461      def metadata
+00000840: 2873 656c 662c 206d 6574 6164 6174 6129  (self, metadata)
+00000850: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00000860: 6d65 7461 6461 7461 203d 206d 6574 6164  metadata = metad
+00000870: 6174 610a 0a20 2020 2040 7072 6f70 6572  ata..    @proper
+00000880: 7479 0a20 2020 2064 6566 2073 7065 6328  ty.    def spec(
+00000890: 7365 6c66 2920 2d3e 2064 6963 743a 0a20  self) -> dict:. 
+000008a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000008b0: 6c66 2e5f 7370 6563 0a0a 2020 2020 4073  lf._spec..    @s
+000008c0: 7065 632e 7365 7474 6572 0a20 2020 2064  pec.setter.    d
+000008d0: 6566 2073 7065 6328 7365 6c66 2c20 7370  ef spec(self, sp
+000008e0: 6563 293a 0a20 2020 2020 2020 2069 6620  ec):.        if 
+000008f0: 7365 6c66 2e6c 6f63 616c 5f76 6172 735f  self.local_vars_
+00000900: 636f 6e66 6967 7572 6174 696f 6e2e 636c  configuration.cl
+00000910: 6965 6e74 5f73 6964 655f 7661 6c69 6461  ient_side_valida
+00000920: 7469 6f6e 2061 6e64 2073 7065 6320 6973  tion and spec is
+00000930: 204e 6f6e 653a 2020 2320 6e6f 7161 3a20   None:  # noqa: 
+00000940: 4535 3031 0a20 2020 2020 2020 2020 2020  E501.           
+00000950: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00000960: 7228 2249 6e76 616c 6964 2076 616c 7565  r("Invalid value
+00000970: 2066 6f72 2060 7370 6563 602c 206d 7573   for `spec`, mus
+00000980: 7420 6e6f 7420 6265 2060 4e6f 6e65 6022  t not be `None`"
+00000990: 2920 2023 206e 6f71 613a 2045 3530 310a  )  # noqa: E501.
+000009a0: 2020 2020 2020 2020 7365 6c66 2e5f 7370          self._sp
+000009b0: 6563 203d 2073 7065 630a 0a0a 6465 6620  ec = spec...def 
+000009c0: 746f 5f64 6963 7428 6f62 6a29 3a0a 2020  to_dict(obj):.  
+000009d0: 2020 7265 7375 6c74 203d 207b 7d0a 0a20    result = {}.. 
+000009e0: 2020 2066 6f72 2061 7474 722c 205f 2069     for attr, _ i
+000009f0: 6e20 7369 782e 6974 6572 6974 656d 7328  n six.iteritems(
+00000a00: 6f62 6a2e 6f70 656e 6170 695f 7479 7065  obj.openapi_type
+00000a10: 7329 3a0a 2020 2020 2020 2020 7661 6c75  s):.        valu
+00000a20: 6520 3d20 6765 7461 7474 7228 6f62 6a2c  e = getattr(obj,
+00000a30: 2061 7474 7229 0a20 2020 2020 2020 206b   attr).        k
+00000a40: 6579 203d 206f 626a 2e61 7474 7269 6275  ey = obj.attribu
+00000a50: 7465 5f6d 6170 2e67 6574 2861 7474 7229  te_map.get(attr)
+00000a60: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00000a70: 7374 616e 6365 2876 616c 7565 2c20 6c69  stance(value, li
+00000a80: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+00000a90: 2072 6573 756c 745b 6b65 795d 203d 206c   result[key] = l
+00000aa0: 6973 7428 6d61 7028 0a20 2020 2020 2020  ist(map(.       
+00000ab0: 2020 2020 2020 2020 206c 616d 6264 6120           lambda 
+00000ac0: 783a 2074 6f5f 6469 6374 2878 2920 6966  x: to_dict(x) if
+00000ad0: 2068 6173 6174 7472 2878 2c20 2274 6f5f   hasattr(x, "to_
+00000ae0: 6469 6374 2229 2065 6c73 6520 782c 0a20  dict") else x,. 
+00000af0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00000b00: 616c 7565 0a20 2020 2020 2020 2020 2020  alue.           
+00000b10: 2029 290a 2020 2020 2020 2020 656c 6966   )).        elif
+00000b20: 2068 6173 6174 7472 2876 616c 7565 2c20   hasattr(value, 
+00000b30: 2274 6f5f 6469 6374 2229 3a0a 2020 2020  "to_dict"):.    
+00000b40: 2020 2020 2020 2020 7265 7375 6c74 5b6b          result[k
+00000b50: 6579 5d20 3d20 746f 5f64 6963 7428 7661  ey] = to_dict(va
+00000b60: 6c75 6529 0a20 2020 2020 2020 2065 6c69  lue).        eli
+00000b70: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
+00000b80: 7565 2c20 6469 6374 293a 0a20 2020 2020  ue, dict):.     
+00000b90: 2020 2020 2020 2072 6573 756c 745b 6b65         result[ke
+00000ba0: 795d 203d 2064 6963 7428 6d61 7028 0a20  y] = dict(map(. 
+00000bb0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00000bc0: 616d 6264 6120 6974 656d 3a20 2869 7465  ambda item: (ite
+00000bd0: 6d5b 305d 2c20 746f 5f64 6963 7428 6974  m[0], to_dict(it
+00000be0: 656d 5b31 5d29 290a 2020 2020 2020 2020  em[1])).        
+00000bf0: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
+00000c00: 7472 2869 7465 6d5b 315d 2c20 2274 6f5f  tr(item[1], "to_
+00000c10: 6469 6374 2229 2065 6c73 6520 6974 656d  dict") else item
+00000c20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000c30: 2020 7661 6c75 652e 6974 656d 7328 290a    value.items().
+00000c40: 2020 2020 2020 2020 2020 2020 2929 0a20              )). 
+00000c50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00000c60: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00000c70: 6b65 795d 203d 2076 616c 7565 0a0a 2020  key] = value..  
+00000c80: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00000c90: 0a0a 6465 6620 746f 5f79 616d 6c28 7265  ..def to_yaml(re
+00000ca0: 736f 7572 6365 3a20 6f62 6a65 6374 2920  source: object) 
+00000cb0: 2d3e 2073 7472 3a0a 2020 2020 6465 6620  -> str:.    def 
+00000cc0: 7265 6d6f 7665 5f6e 6f6e 6528 6f62 6a29  remove_none(obj)
+00000cd0: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
+00000ce0: 6e73 7461 6e63 6528 6f62 6a2c 2028 6c69  nstance(obj, (li
+00000cf0: 7374 2c20 7475 706c 652c 2073 6574 2929  st, tuple, set))
+00000d00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00000d10: 7475 726e 2074 7970 6528 6f62 6a29 2872  turn type(obj)(r
+00000d20: 656d 6f76 655f 6e6f 6e65 2878 2920 666f  emove_none(x) fo
+00000d30: 7220 7820 696e 206f 626a 2069 6620 7820  r x in obj if x 
+00000d40: 6973 206e 6f74 204e 6f6e 6529 0a20 2020  is not None).   
+00000d50: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00000d60: 6365 286f 626a 2c20 6469 6374 293a 0a20  ce(obj, dict):. 
+00000d70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000d80: 6e20 7479 7065 286f 626a 2928 2872 656d  n type(obj)((rem
+00000d90: 6f76 655f 6e6f 6e65 286b 292c 2072 656d  ove_none(k), rem
+00000da0: 6f76 655f 6e6f 6e65 2876 2929 0a20 2020  ove_none(v)).   
+00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000dc0: 2020 2020 2020 2020 2020 666f 7220 6b2c            for k,
+00000dd0: 2076 2069 6e20 6f62 6a2e 6974 656d 7328   v in obj.items(
+00000de0: 2920 6966 206b 2069 7320 6e6f 7420 4e6f  ) if k is not No
+00000df0: 6e65 2061 6e64 2076 2069 7320 6e6f 7420  ne and v is not 
+00000e00: 4e6f 6e65 290a 2020 2020 2020 2020 7265  None).        re
+00000e10: 7475 726e 206f 626a 0a0a 2020 2020 7265  turn obj..    re
+00000e20: 736f 7572 6365 5f64 6963 7420 3d20 746f  source_dict = to
+00000e30: 5f64 6963 7428 7265 736f 7572 6365 2920  _dict(resource) 
+00000e40: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
+00000e50: 2068 6173 6174 7472 2872 6573 6f75 7263   hasattr(resourc
+00000e60: 652c 2022 6f70 656e 6170 695f 7479 7065  e, "openapi_type
+00000e70: 7322 2920 616e 6420 6861 7361 7474 7228  s") and hasattr(
+00000e80: 7265 736f 7572 6365 2c20 2261 7474 7269  resource, "attri
+00000e90: 6275 7465 5f6d 6170 2229 2920 656c 7365  bute_map")) else
+00000ea0: 207b 7d0a 2020 2020 7961 6d6c 5f76 616c   {}.    yaml_val
+00000eb0: 7565 7320 3d20 7265 6d6f 7665 5f6e 6f6e  ues = remove_non
+00000ec0: 6528 7265 736f 7572 6365 5f64 6963 7429  e(resource_dict)
+00000ed0: 0a0a 2020 2020 6966 2068 6173 6174 7472  ..    if hasattr
+00000ee0: 2872 6573 6f75 7263 652c 2027 7363 6865  (resource, 'sche
+00000ef0: 6d61 2729 2061 6e64 2072 6573 6f75 7263  ma') and resourc
+00000f00: 652e 7363 6865 6d61 3a0a 2020 2020 2020  e.schema:.      
+00000f10: 2020 7465 6d70 6c61 7465 203d 2070 6b67    template = pkg
+00000f20: 7574 696c 2e67 6574 5f64 6174 6128 5f5f  util.get_data(__
+00000f30: 6e61 6d65 5f5f 2c20 6627 7363 6865 6d61  name__, f'schema
+00000f40: 2f7b 7265 736f 7572 6365 2e73 6368 656d  /{resource.schem
+00000f50: 617d 2729 0a20 2020 2020 2020 2069 6620  a}').        if 
+00000f60: 7465 6d70 6c61 7465 3a0a 2020 2020 2020  template:.      
+00000f70: 2020 2020 2020 7363 6865 6d61 203d 2079        schema = y
+00000f80: 616d 6c2e 6c6f 6164 2874 656d 706c 6174  aml.load(templat
+00000f90: 652e 6465 636f 6465 2827 7574 662d 3827  e.decode('utf-8'
+00000fa0: 2929 0a20 2020 2020 2020 2020 2020 2074  )).            t
+00000fb0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00000fc0: 2020 2020 6a73 6f6e 7363 6865 6d61 2e76      jsonschema.v
+00000fd0: 616c 6964 6174 6528 7961 6d6c 5f76 616c  alidate(yaml_val
+00000fe0: 7565 732c 2073 6368 656d 6129 0a20 2020  ues, schema).   
+00000ff0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00001000: 5661 6c69 6461 7469 6f6e 4572 726f 7220  ValidationError 
+00001010: 6173 2065 7272 3a0a 2020 2020 2020 2020  as err:.        
+00001020: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00001030: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+00001040: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+00001050: 5363 6865 6d61 2076 616c 6964 6174 696f  Schema validatio
+00001060: 6e20 6661 696c 6564 2077 6974 6820 7b65  n failed with {e
+00001070: 7272 2e6d 6573 7361 6765 7d20 6174 207b  rr.message} at {
+00001080: 222e 222e 6a6f 696e 286d 6170 2873 7472  ".".join(map(str
+00001090: 2c20 6572 722e 7363 6865 6d61 5f70 6174  , err.schema_pat
+000010a0: 6829 297d 2729 2066 726f 6d20 6572 720a  h))}') from err.
+000010b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000010c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000010d0: 5661 6c75 6545 7272 6f72 2866 2753 6368  ValueError(f'Sch
+000010e0: 656d 6120 7b72 6573 6f75 7263 652e 7363  ema {resource.sc
+000010f0: 6865 6d61 7d20 6465 6669 6e65 6420 6275  hema} defined bu
+00001100: 7420 6e6f 7420 666f 756e 6420 696e 2070  t not found in p
+00001110: 6163 6b61 6765 2729 0a0a 2020 2020 7374  ackage')..    st
+00001120: 7265 616d 203d 2053 7472 696e 6749 4f28  ream = StringIO(
+00001130: 290a 2020 2020 7961 6d6c 2e64 756d 7028  ).    yaml.dump(
+00001140: 7961 6d6c 5f76 616c 7565 732c 2073 7472  yaml_values, str
+00001150: 6561 6d29 0a0a 2020 2020 7265 7475 726e  eam)..    return
+00001160: 2073 7472 6561 6d2e 6765 7476 616c 7565   stream.getvalue
+00001170: 2829 0a                                  ().
```

## mpyl/steps/test/echo.py

```diff
@@ -1,22 +1,40 @@
 """ Dummy test step to test the framework. """
 
 from logging import Logger
+from pathlib import Path
 
 from .. import Step, Meta
-from ..models import Input, Output, ArtifactType
+from ..models import Input, Output, ArtifactType, input_to_artifact
 from ...project import Stage
+from ...utilities.junit import TEST_OUTPUT_PATH_KEY
+
+SAMPLE_JUNIT_RESULT = """
+<?xml version="1.0" encoding="UTF-8"?>
+<testsuites name="jest tests" tests="1" failures="0" errors="0" time="0.486">
+  <testsuite name="undefined" errors="0" failures="0" skipped="0" timestamp="2023-03-29T02:51:00" time="0.244" tests="1">
+    <testcase classname="Test Echo" name=" fake test case from TestEcho step" time="0.002">
+    </testcase>
+  </testsuite>
+</testsuites>
+""".strip()
 
 
 class TestEcho(Step):
 
     def __init__(self, logger: Logger) -> None:
         super().__init__(logger, Meta(
             name='Echo Test',
             description='Dummy test step to test the framework',
             version='0.0.1',
             stage=Stage.TEST
-        ), ArtifactType.NONE, ArtifactType.NONE)
+        ), produced_artifact=ArtifactType.JUNIT_TESTS, required_artifact=ArtifactType.NONE)
 
     def execute(self, step_input: Input) -> Output:
         self._logger.info(f"Testing project {step_input.project.name}")
-        return Output(success=True, message=f"Tested {step_input.project.name}", produced_artifact=None)
+        path = Path(step_input.project.target_path, "test_results")
+        path.mkdir(parents=True, exist_ok=True)
+        Path(path, "test.xml").write_text(SAMPLE_JUNIT_RESULT, encoding='utf-8')
+
+        artifact = input_to_artifact(artifact_type=ArtifactType.JUNIT_TESTS, step_input=step_input,
+                                     spec={TEST_OUTPUT_PATH_KEY: str(path)})
+        return Output(success=True, message=f"Tested {step_input.project.name}", produced_artifact=artifact)
```

## mpyl/steps/test/sbt.py

```diff
@@ -33,46 +33,47 @@
         if not compile_outcome.success:
             return Output(success=False, message=f"Tests failed to compile for {project_name}",
                           produced_artifact=None)
 
         command_test = self._construct_sbt_command(step_input, sbt_config,
                                                    self._construct_sbt_command_test_with_coverage)
         test_outcome = custom_check_output(self._logger, command_test)
+        artifact = self._extract_test_report(step_input.project, step_input)
         if not test_outcome.success:
             return Output(success=False,
                           message=f"Tests failed to run for {project_name}. No test results have been recorded.",
-                          produced_artifact=None)
-        return Output(success=True, message="Success")
+                          produced_artifact=artifact)
+        return Output(success=True, message="Success", produced_artifact=artifact)
 
     def _test_without_coverage(self, step_input: Input, sbt_config: SbtConfig) -> Output:
         command_test_without_coverage = self._construct_sbt_command(step_input, sbt_config,
                                                                     self._construct_sbt_command_test_without_coverage)
         run_outcome = custom_check_output(self._logger, command_test_without_coverage)
+        artifact = self._extract_test_report(step_input.project, step_input)
         if not run_outcome.success:
             return Output(success=False, message=f"Tests without coverage failed to run for {step_input.project.name}",
-                          produced_artifact=None)
-        return Output(success=True, message="Success")
+                          produced_artifact=artifact)
+        return Output(success=True, message="Success", produced_artifact=artifact)
 
     def execute(self, step_input: Input) -> Output:
         project = step_input.project
         sbt_config = SbtConfig.from_config(config=step_input.run_properties.config)
         self._logger.debug(f'Config {sbt_config}')
 
         test_result = self._test_with_coverage(step_input, sbt_config) if sbt_config.test_with_coverage \
             else self._test_without_coverage(step_input, sbt_config)
 
-        if not test_result.success:
-            return test_result
+        if test_result.produced_artifact:
+            suite = to_test_suites(test_result.produced_artifact)
+            summary = sum_suites(suite)
+            return Output(success=summary.is_success,
+                          message=f"Tests results produced for {project.name} ({summary})",
+                          produced_artifact=test_result.produced_artifact)
 
-        artifact = self._extract_test_report(project, step_input)
-        suite = to_test_suites(artifact)
-        summary = sum_suites(suite)
-        return Output(success=summary.is_success,
-                      message=f"Tests results produced for {project.name} ({summary})",
-                      produced_artifact=artifact)
+        return test_result
 
     @staticmethod
     def _construct_sbt_command_compile_with_coverage(step_input: Input) -> list[str]:
         return [
             f'project {step_input.project.name}',
             'coverageOn',
             'test:compile'
```

## mpyl/utilities/docker/__init__.py

```diff
@@ -1,14 +1,15 @@
 """Docker related utility methods"""
 import logging
 from dataclasses import dataclass
 from logging import Logger
-from typing import Dict, Optional, TypeVar
+from typing import Dict, Optional, Iterator, Iterable, cast, Union
 
-from python_on_whales import docker
+from python_on_whales import docker, Image, Container
+from rich.text import Text
 
 from ...project import Project
 from ...steps.models import Input
 
 
 @dataclass(frozen=True)
 class DockerComposeConfig:
@@ -52,19 +53,26 @@
                 test_target=build_config.get('testTarget', None),
                 docker_file_name=build_config['dockerFileName']
             )
         except KeyError as exc:
             raise KeyError(f'Docker config could not be loaded from {config}') from exc
 
 
-def stream_docker_logging(logger: Logger, generator, task_name: str, level=logging.DEBUG) -> None:
+def execute_with_stream(logger: Logger, container: Container, command: str, task_name: str) -> None:
+    result = cast(Iterator[tuple[str, bytes]], container.execute(command=command.split(' '), stream=True))
+    stream_docker_logging(logger, result, task_name)
+
+
+def stream_docker_logging(logger: Logger, generator: Union[Iterator[str], Iterator[tuple[str, bytes]]], task_name: str,
+                          level=logging.INFO) -> None:
     while True:
         try:
-            output = next(generator)
-            logger.log(level, str(output).strip('\n'))
+            next_item = next(generator)
+            log_line = next_item[1].decode(errors="replace") if isinstance(next_item, tuple) else next_item
+            logger.log(level, Text.from_ansi(log_line))
         except StopIteration:
             logger.info(f'{task_name} complete.')
             break
 
 
 def docker_image_tag(step_input: Input):
     git = step_input.run_properties.versioning
@@ -85,10 +93,18 @@
     :param target: the 'target' within the multi-stage docker image
     :return: True if success, False if failure
     """
     logger.info(f"Building docker image with {file_path} and target {target}")
 
     logs = docker.buildx.build(context_path=root_path, file=file_path, tags=[image_tag], target=target,
                                stream_logs=True)
-    stream_docker_logging(logger=logger, generator=logs, task_name=f'Build {file_path}:{target}')
+    if logs is not None and not isinstance(logs, Image):
+        stream_docker_logging(logger=logger, generator=logs, task_name=f'Build {file_path}:{target}')
     logger.debug(logs)
     return True
+
+
+def login(logger: Logger, docker_config: DockerConfig) -> None:
+    logger.info(f"Logging in with user '{docker_config.user_name}'")
+    docker.login(server=f'https://{docker_config.host_name}', username=docker_config.user_name,
+                 password=docker_config.password)
+    logger.debug(f"Logged in as '{docker_config.user_name}'")
```

## mpyl/utilities/github/__init__.py

```diff
@@ -12,40 +12,45 @@
     private_key_base_64_encoded: Optional[str]
     app_key: str
 
     def __init__(self, config: Dict):
         self.private_app_key_path = config.get('privateKeyPath')
         self.private_key_base_64_encoded = config.get('privateKeyBase64Encoded')
         if not self.private_key_base_64_encoded and not self.private_app_key_path:
-            raise KeyError("Either 'privateKeyPath' or 'privateKeyBase64Encoded' need to be defined")
+            raise KeyError("When github.app is configured, either 'privateKeyPath' "
+                           "or 'privateKeyBase64Encoded' need to be defined")
 
         self.app_key = config['appId']
 
 
-@dataclass
+@dataclass(frozen=True)
 class GithubConfig:
     repository: str
     owner: str
     repo_name: str
     token: str
-    app_config: Optional[GithubAppConfig] = None
+    app_config: dict
 
-    def __init__(self, config: Dict):
+    @staticmethod
+    def from_config(config: Dict):
         github = config['cvs']['github']
-        self.repository = github['repository']
-        parts = self.repository.split('/')
-        self.owner = parts[0]
-        self.repo_name = parts[1]
-        self.token = github['token']
-
-        app_config = github.get('app', {})
-        if app_config:
-            self.app_config = GithubAppConfig(app_config)
+        repo_parts = github['repository'].split('/')
+        return GithubConfig(
+            repository=(github['repository']),
+            owner=repo_parts[0],
+            repo_name=repo_parts[1],
+            token=github['token'],
+            app_config=github.get('app', {})
+        )
+
+    @property
+    def get_app_config(self) -> GithubAppConfig:
+        return GithubAppConfig(self.app_config)
 
 
 def get_pr_for_branch(repo: Repository, branch: str) -> PullRequest:
     pulls = repo.get_pulls(head=f'{repo.full_name}:{branch}').get_page(0)
 
     if len(pulls) == 0:
-        raise ValueError(f'No PR related to {branch} were found')
+        raise ValueError(f'No PR related to {branch} was found. Did you create it yet? `gh pr create --draft`')
 
     return pulls.pop()
```

## mpyl/utilities/jenkins/__init__.py

```diff
@@ -16,15 +16,15 @@
         if not jenkins_config:
             raise KeyError('jenkins should be defined in config')
         return JenkinsConfig(url=jenkins_config['url'], pipelines=jenkins_config['pipelines'],
                              default=jenkins_config['defaultPipeline'])
 
     @property
     def default_pipeline(self) -> str:
-        return self.pipelines[self.default_pipeline]
+        return self.pipelines[self.default]
 
 
 @dataclass(frozen=True)
 class Pipeline:
     target: Target
     tag: str
     url: str
```

## mpyl/utilities/jenkins/runner.py

```diff
@@ -4,42 +4,75 @@
 import signal
 import sys
 import time
 from dataclasses import dataclass
 
 import requests
 from jenkinsapi.build import Build
+from jenkinsapi.custom_exceptions import JenkinsAPIException
 from jenkinsapi.jenkins import Jenkins
 from jenkinsapi.job import Job
 from rich.errors import MarkupError
 from rich.progress import Progress
 from rich.prompt import Confirm
 from rich.status import Status
 from rich.text import Text
 
 from . import Pipeline
 
 
+def stream_utf_8_logs(self, interval=0):
+    """
+    Return generator which streams parts of text console.
+    Workaround for https://github.com/pycontribs/jenkinsapi/pull/843
+    """
+    url = f"{self.baseurl}/logText/progressiveText"
+    size = 0
+    more_data = True
+    while more_data:
+        resp = self.job.jenkins.requester.get_url(
+            url, params={"start": size}
+        )
+        content = resp.content
+        if content:
+            if isinstance(content, str):
+                yield content
+            elif isinstance(content, bytes):
+                yield content.decode(resp.encoding)
+            else:
+                raise JenkinsAPIException(
+                    "Unknown content type for console"
+                )
+        size = resp.headers["X-Text-Size"]
+        more_data = resp.headers.get("X-More-Data")
+        time.sleep(interval)
+
+
+Build.stream_utf_8_logs = stream_utf_8_logs
+
+
 @dataclass
 class JenkinsRunner:
     pipeline: Pipeline
     jenkins: Jenkins
     status: Status
+    follow: bool
 
     def get_job(self, name: str) -> Job:
         try:
             return self.jenkins.get_job(name)
         except KeyError:
             self.status.update(f'Job for {self.pipeline.human_readable()} not found. This could take a while. '
                                'Triggering build scan...')
             requests.post(f'{self.pipeline.pipeline_location()}/build?delay=0#',
                           auth=(self.jenkins.username, self.jenkins.password), timeout=10)
 
             while True:
                 try:
+                    self.jenkins.jobs_container = None  # force update of job info
                     return self.jenkins.get_job(name)
                 except KeyError:
                     self.status.update(f'Waiting for {self.pipeline.human_readable()} to appear...')
                     time.sleep(1)
 
     def await_parameter_build(self, build_job: Job):
         queue = build_job.invoke()
@@ -72,23 +105,25 @@
             start_time = time.time()
 
             def cancel_handler(_sig, _frame):
                 progress.stop()
                 stop_build = Confirm.ask("Stop build?")
                 if stop_build:
                     build_to_follow.stop()
+                else:
+                    sys.exit()
 
             signal.signal(signal.SIGINT, cancel_handler)
-            for line in build_to_follow.stream_logs():
+            for line in build_to_follow.stream_utf_8_logs():
                 current_time = time.time()
                 elapsed_time = current_time - start_time
                 lines = line.rstrip().split('\n')
 
                 try:
-                    text = "".join(lines[-1:])
+                    text = "".join(lines)
                     progress.log(Text.from_ansi(text))
                 except MarkupError:
                     progress.log("Could not render log line")
                 progress.update(build_task, completed=elapsed_time)
             progress.update(build_task, completed=duration_estimation)
 
         build_to_follow.block_until_complete()
@@ -97,15 +132,15 @@
             f'[link={finished_build.get_build_url()}][i]Build[/link] for {self.pipeline.human_readable()} '
             f'ended with outcome {self.to_icon(finished_build)}', markup=True)
         self.status.console.log()
 
         os.system('afplay /System/Library/Sounds/' + ('Glass.aiff' if finished_build.is_good() else 'Sosumi.aiff'))
         sys.exit()
 
-    def run(self):
+    def run(self, pipeline_parameters: dict):
         job: Job = self.get_job(self.pipeline.job_name())
         if not list(job.get_build_ids()):
             self.await_parameter_build(job)
 
         build = job.get_last_build()
         last_build_number = build.get_number()
         if job.is_running():
@@ -114,17 +149,18 @@
             self.status.console.log(f"{build.get_build_url()}")
             self.follow_logs(job, last_build_number, 0)
 
         self.status.update("Starting build...")
 
         last_build = 0
 
-        self.jenkins.build_job(self.pipeline.job_name(), params={})
+        self.jenkins.build_job(self.pipeline.job_name(), params=pipeline_parameters)
 
         if last_build_number > 1:
             last_build = build.get_duration().seconds
             self.status.console.log(f'Last build {last_build_number} {self.to_icon(build)} took'
                                     f' {str(datetime.timedelta(seconds=last_build))}')
 
         new_build_number = last_build_number + 1
 
-        self.follow_logs(job, new_build_number, last_build)
+        if self.follow:
+            self.follow_logs(job, new_build_number, last_build)
```

## mpyl/utilities/junit/__init__.py

```diff
@@ -1,9 +1,8 @@
 """Wrapper around `junitparser`"""
-
 import os
 from dataclasses import dataclass
 from pathlib import Path
 
 from junitparser import JUnitXml, TestSuite
 
 from ...steps.models import Artifact, ArtifactType
@@ -26,16 +25,16 @@
 def to_test_suites(artifact: Artifact) -> list[TestSuite]:
     if artifact.artifact_type != ArtifactType.JUNIT_TESTS:
         raise ValueError(f'Artifact {artifact} should be of type {ArtifactType.JUNIT_TESTS}')
     junit_result_path = artifact.spec[TEST_OUTPUT_PATH_KEY]
 
     xml = JUnitXml()
     for file_name in [fn for fn in os.listdir(junit_result_path) if fn.endswith('.xml')]:
-        xml += JUnitXml.fromfile(Path(junit_result_path, file_name))
+        xml += JUnitXml.fromfile(Path(junit_result_path, file_name).as_posix())
 
     suites = [TestSuite.fromelem(s) for s in xml]
     return sorted(suites, key=lambda s: s.time)
 
 
 def sum_suites(suites: list[TestSuite]) -> TestRunSummary:
     return TestRunSummary(tests=sum(s.tests for s in suites), failures=sum(s.failures for s in suites),
-                          errors=sum(s.failures for s in suites), skipped=sum(s.skipped for s in suites))
+                          errors=sum(s.errors for s in suites), skipped=sum(s.skipped for s in suites))
```

## mpyl/utilities/pyaml_env/__init__.py

```diff
@@ -1,20 +1,24 @@
 """
 Wrapper around `pyaml_env`'s `parse_config`. Sets default values in config to `None`
 """
+from pathlib import Path
 
 from pyaml_env import parse_config as original_parse_config
+from dotenv import load_dotenv
 
 
-def parse_config(path: str) -> dict[str, str]:
+def parse_config(path: Path) -> dict[str, str]:
+    load_dotenv(Path(".env"))
+
     def default_to_none(obj, default_value='N/A'):
         if isinstance(obj, (list, tuple, set)):
             return type(obj)(default_to_none(x) for x in obj if x is not default_value)
         if isinstance(obj, dict):
             return type(obj)((default_to_none(k), default_to_none(v))
                              for k, v in obj.items() if k is not default_value and v is not default_value)
         if obj == default_value:
             return None
         return obj
 
-    parsed = original_parse_config(path)
+    parsed = original_parse_config(str(path))
     return default_to_none(parsed)
```

## mpyl/utilities/repo/__init__.py

```diff
@@ -1,15 +1,17 @@
 """ Defines information about the repository, any changes made to it and the containing projects.
 `mpyl.utilities.repo.Repository` is a facade for the Version Control System.
 At this moment Git is the only supported VCS.
 """
 
+import logging
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Dict
+from typing import Dict, Optional
+from urllib.parse import urlparse
 
 from git import Git, Repo, Remote
 
 from ...project import Project
 
 
 @dataclass(frozen=True)
@@ -18,29 +20,53 @@
     """Ordinal number indicating how this revision ranks historically"""
     hash: str
     """Git hash for this revision"""
     files_touched: set[str]
     """Paths to files that were altered in this hash"""
 
 
+@dataclass(frozen=True)
+class RepoCredentials:
+    url: str
+    user_name: str
+    password: str
+
+    @property
+    def to_url_with_credentials(self):
+        parsed = urlparse(self.url)
+        return f"{parsed.scheme}://{self.user_name}:{self.password}@{parsed.netloc}{parsed.path}"
+
+    @staticmethod
+    def from_config(config: Dict):
+        return RepoCredentials(url=config['url'], user_name=config['userName'], password=config['password'])
+
+
+@dataclass(frozen=True)
 class RepoConfig:
     main_branch: str
+    repo_credentials: Optional[RepoCredentials]
 
-    def __init__(self, config: Dict):
-        self.main_branch = config['cvs']['git']['mainBranch']
+    @staticmethod
+    def from_config(config: Dict):
+        git_config = config['cvs']['git']
+        maybe_remote_config = git_config.get('remote', None)
+        return RepoConfig(
+            main_branch=git_config['mainBranch'],
+            repo_credentials=RepoCredentials.from_config(maybe_remote_config) if maybe_remote_config else None
+        )
 
 
 class Repository:
 
     def __init__(self, config: RepoConfig):
         self._config = config
         self._root_dir = Git().rev_parse('--show-toplevel')
+        self._repo = Repo(self._root_dir)  # pylint: disable=attribute-defined-outside-init
 
     def __enter__(self):
-        self._repo = Repo(self._root_dir)  # pylint: disable=attribute-defined-outside-init
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._repo.close()
         return self
 
     @property
@@ -48,37 +74,92 @@
         return self._repo.head.commit.hexsha
 
     @property
     def get_short_sha(self):
         return self._repo.git.rev_parse(self._repo.head, short=True)
 
     @property
-    def get_branch(self):
-        return self._repo.active_branch.name
+    def get_branch(self) -> Optional[str]:
+        try:
+            return self._repo.active_branch.name
+        except TypeError:
+            return None
+
+    @property
+    def get_tag(self) -> Optional[str]:
+        current_revision = self._repo.head.commit
+        current_tag = self._repo.git.describe(current_revision, tags=True)
+        logging.debug(f"Current revision: {current_revision} tag: {current_tag}")
+        return current_tag
+
+    @property
+    def get_remote_url(self):
+        return self._repo.remote().url
 
     def root_dir(self) -> Path:
         return Path(self._root_dir)
 
+    @property
+    def main_branch(self) -> str:
+        return self._config.main_branch
+
+    @property
+    def latest_tag(self) -> str:
+        return str(sorted(self._repo.tags, key=lambda t: t.commit.committed_datetime)[-1])
+
     def changes_in_branch(self) -> list[Revision]:
         revisions = reversed(list(self._repo.iter_commits(f"{self._config.main_branch}..HEAD")))
         return [Revision(count, str(rev),
-                         self._repo.git.diff_tree(no_commit_id=True, name_only=True, r=str(rev)).splitlines()) for
-                count, rev in enumerate(revisions)]
+                         self._repo.git.diff_tree(no_commit_id=True, name_only=True, r=str(rev)).splitlines())
+                for count, rev in enumerate(revisions)]
 
     def changes_in_branch_including_local(self) -> list[Revision]:
         in_branch = self.changes_in_branch()
-        in_branch.append(Revision(len(in_branch), '', self.changes_in_commit()))
+        in_branch.append(Revision(len(in_branch), self.get_sha, self.changes_in_commit()))
         return in_branch
 
+    def changes_in_tagged_commit(self, current_tag: str) -> list[Revision]:
+        curr_rev_tag = self.get_tag
+
+        if curr_rev_tag != current_tag:
+            logging.error(f"HEAD is not at {curr_rev_tag} not at expected {current_tag}")
+            return []
+
+        return self.changes_in_merge_commit()
+
+    def changes_in_merge_commit(self):
+        parent_revs = self._repo.head.commit.parents
+        if not parent_revs:
+            logging.error("HEAD is not at merge commit, cannot determine changed files.")
+            return []
+        logging.debug(f"Parent revisions: {parent_revs}")
+        files_changed = self._repo.git.diff(f"{str(parent_revs[0])}..{str(parent_revs[1])}",
+                                            name_only=True).splitlines()
+        return [Revision(ord=0, hash=str(self.get_sha), files_touched=files_changed)]
+
+    @property
+    def main_branch_pulled(self) -> bool:
+        branch_names = list(map(lambda n: n.name, self._repo.references))
+        return f'{self._config.main_branch}' in branch_names
+
+    def __get_remote(self) -> Remote:
+        default_remote = self._repo.remote('origin')
+        if 'https:' not in default_remote.url or self._config.repo_credentials is None:
+            return default_remote
+
+        return default_remote.set_url(self._config.repo_credentials.to_url_with_credentials)
+
     def pull_main_branch(self):
-        remote = Remote(self._repo, 'origin')
+        remote = self.__get_remote()
         main = self._config.main_branch
         return remote.fetch(f"+refs/heads/{main}:refs/heads/{main}")
 
     def changes_in_commit(self) -> set[str]:
         changed: set[str] = set(self._repo.git.diff(None, name_only=True).splitlines())
         return changed.union(self._repo.untracked_files)
 
-    def find_projects(self) -> list[str]:
-        """ returns a set of all project.yml files """
-        projects = set(self._repo.git.ls_files(f'**/{Project.project_yaml_path()}').splitlines())
+    def find_projects(self, folder_pattern: str = '') -> list[str]:
+        """ returns a set of all project.yml files
+        :type folder_pattern: project paths are filtered on this pattern
+        """
+        projects = set(self._repo.git.ls_files(f'*{folder_pattern}*/{Project.project_yaml_path()}').splitlines())
         return sorted(projects)
```

## mpyl/utilities/sbt/__init__.py

```diff
@@ -5,39 +5,39 @@
 
 
 @dataclass(frozen=True)
 class SbtConfig:
     java_opts: str
     sbt_opts: str
     sbt_command: str
+    sbt_client_command: str
     test_with_coverage: bool
     verbose: bool
     build_with_client: bool
     test_with_client: bool
 
     @staticmethod
     def from_config(config: Dict):
         sbt_config = config.get('sbt', None)
         if not sbt_config:
             raise KeyError(f"'sbt' could not be loaded from {config}")
         return SbtConfig(
             sbt_command=sbt_config['command'],
+            sbt_client_command=sbt_config['clientCommand'],
             java_opts=sbt_config['javaOpts'],
             sbt_opts=sbt_config['sbtOpts'],
             test_with_coverage=(str(sbt_config['testWithCoverage']).lower() == 'true'),
             verbose=(str(sbt_config['verbose']).lower() == 'true'),
             build_with_client=(str(sbt_config.get('clientMode', {}).get('build')).lower() == 'true'),
             test_with_client=(str(sbt_config.get('clientMode', {}).get('test')).lower() == 'true')
         )
 
     def to_command(self, client_mode: bool, sbt_commands: list[str]):
-        cmd = [self.sbt_command]
+        cmd = [self.sbt_client_command if client_mode else self.sbt_command]
         if self.verbose:
             cmd.append('-v')
-        if client_mode:
-            cmd.append('--client')
         cmd.extend([f'-J{opt}' for opt in self.java_opts.split(' ')])
         cmd.extend([f'-D{opt}' for opt in self.sbt_opts.split(' ')])
 
         joined_commands = "; ".join(sbt_commands)
-        cmd.append(f"'{joined_commands}" if client_mode else joined_commands)
+        cmd.append(joined_commands)
         return cmd
```

## mpyl/utilities/subprocess/__init__.py

```diff
@@ -3,36 +3,50 @@
 import subprocess
 from logging import Logger
 from typing import Union
 
 from ...steps.models import Output
 
 
-def custom_check_output(logger: Logger, command: Union[str, list[str]]) -> Output:
+def custom_check_output(logger: Logger, command: Union[str, list[str]], capture_stdout: bool = False) -> Output:
+    """
+    Wrapper around subprocess.Popen
+    ⚠️ Using this function implies an implicit runtime OS dependency.
+    Avoid this if at all possible. For example, to run docker commands, use the bundled docker client (python-on-whales)
+    which makes the dependency on docker explicit and adds a lot of convenience methods.
+    """
     if isinstance(command, str):
         command = command.split(' ')
 
     command_argument = ' '.join(command)
     logger.info(f"Executing: '{command_argument}'")
     try:
+        if capture_stdout:
+            out = subprocess.check_output(command, stderr=subprocess.STDOUT).decode("utf-8")
+            print(out)
+            return Output(success=True, message=out)
+
         with subprocess.Popen(command, stdout=subprocess.PIPE, text=True) as process:
             if not process.stdout:
                 raise RuntimeError(f'Process {command_argument} does not have an stdout')
 
             for line in iter(process.stdout.readline, ""):
                 if line:
                     print(line.rstrip())
                 if process.poll() is not None:
                     break
-            exit_code = process.wait()
+            success = process.wait() == 0
+            if not success:
+                logger.warning(f"Subprocess failed: {process.stderr.read() if process.stderr else 'No stderr output'}")
 
-            return Output(success=exit_code == 0, message='Subprocess executed successfully')
+            return Output(success=success, message='Subprocess executed successfully')
 
 
     except subprocess.CalledProcessError as exc:
-        logger.warning(f"'{command_argument}': failed with return code: {exc.returncode} err: {exc.stderr.decode()}",
+        logger.warning(f"'{command_argument}': failed with return code: {exc.returncode} err: "
+                       f"{exc.stderr.decode() if exc.stderr else 'No stderr output'}",
                        exc_info=True)
 
     except FileNotFoundError:
         logger.warning(f"'{command_argument}: file not found", exc_info=True)
 
     return Output(success=False, message='Subprocess failed')
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `mpyl/cli/build/jenkins.py` & `mpyl/cli/commands/build/jenkins.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,92 @@
 """Jenkins multibranch pipeline build tool"""
+import subprocess
 from dataclasses import dataclass
+from typing import Optional
 
 import requests
 from github import Github
 from jenkinsapi.jenkins import Jenkins
 from rich.console import Console
+from rich.markdown import Markdown
+from rich.status import Status
 
-from ...project import Target
-from ...utilities.github import GithubConfig, get_pr_for_branch
-from ...utilities.jenkins import JenkinsConfig, Pipeline
-from ...utilities.jenkins.runner import JenkinsRunner
-from ...utilities.repo import RepoConfig
-from ...utilities.repo import Repository
+from ....project import Target
+from ....utilities.github import GithubConfig, get_pr_for_branch
+from ....utilities.jenkins import JenkinsConfig, Pipeline
+from ....utilities.jenkins.runner import JenkinsRunner
+from ....utilities.repo import RepoConfig, Repository
 
 
 @dataclass(frozen=True)
 class JenkinsRunParameters:
     jenkins_user: str
     jenkins_password: str
     config: dict
     pipeline: str
+    pipeline_parameters: dict
+    verbose: bool
+    follow: bool
+    tag: Optional[str] = None
+
+
+def get_token(github_config: GithubConfig):
+    if github_config.token:
+        return github_config.token
+    return subprocess.run(['gh', 'auth', 'token'], stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
+                          check=True).stdout.decode('utf-8').strip()
+
+
+def __get_pr_pipeline(config: dict, git_repo: Repository, pipeline: str, status: Status) -> Optional[Pipeline]:
+    github_config = GithubConfig.from_config(config)
+    github = Github(login_or_token=get_token(github_config))
+
+    repo = github.get_repo(github_config.repository)
+
+    branch = git_repo.get_branch
+    if not branch:
+        status.console.log('Could not determine current branch')
+        return None
+
+    if git_repo.main_branch == branch:
+        status.console.log(f'On main branch ({branch}), cannot determine which PR to build')
+        return None
+
+    pull = get_pr_for_branch(repo, branch)
+
+    return Pipeline(target=Target.PULL_REQUEST, tag=f'{pull.number}', url=pull.html_url, pipeline=pipeline,
+                    body=pull.body, jenkins_config=JenkinsConfig.from_config(config))
 
 
 def run_jenkins(run_config: JenkinsRunParameters):
     log_console = Console(log_path=False, log_time=False)
     with log_console.status('Fetching Github info.. [blue]>gh pr view[/blue]') as status:
         config = run_config.config
-        github_config = GithubConfig(config)
-        with Repository(RepoConfig(config)) as git_repo:
-            try:
-                github = Github(login_or_token=github_config.token)
-                repo = github.get_repo(github_config.repository)
-
-                pull = get_pr_for_branch(repo, git_repo.get_branch)
 
-                jenkins_config = JenkinsConfig.from_config(config)
-                pipeline_info = Pipeline(target=Target.PULL_REQUEST, tag=f'{pull.number}', url=pull.url,
-                                         pipeline=run_config.pipeline, body=pull.body, jenkins_config=jenkins_config)
+        with Repository(RepoConfig.from_config(config)) as git_repo:
+            try:
+                pipeline_info = Pipeline(
+                    target=Target.ACCEPTANCE, tag=run_config.tag, url="https://tag-url",
+                    pipeline=run_config.pipeline, body="",
+                    jenkins_config=JenkinsConfig.from_config(config)) if run_config.tag \
+                    else __get_pr_pipeline(config, git_repo, run_config.pipeline, status)
+                if not pipeline_info:
+                    return
 
                 status.start()
                 status.update(f'Fetching Jenkins info for {pipeline_info.human_readable()} ...')
 
                 runner = JenkinsRunner(pipeline=pipeline_info,
-                                       jenkins=Jenkins(jenkins_config.url, username=run_config.jenkins_user,
-                                                       password=run_config.jenkins_password), status=status)
-                runner.run()
+                                       jenkins=Jenkins(baseurl=JenkinsConfig.from_config(config).url,
+                                                       username=run_config.jenkins_user,
+                                                       password=run_config.jenkins_password),
+                                       status=status,
+                                       follow=run_config.follow)
+                runner.run(run_config.pipeline_parameters)
             except requests.ConnectionError:
                 status.console.bell()
                 status.console.log('⚠️ Could not connect. Are you on VPN?')
             except Exception as exc:
-                status.console.log(f'Unexpected exception: {exc}')
-                status.console.print_exception()
+                status.console.print(Markdown(f'Unexpected exception: {exc}'))
+                if run_config.verbose:
+                    status.console.print_exception()
                 raise exc
```

## Comparing `mpyl/cli/build/mpyl.py` & `mpyl/cli/commands/build/mpyl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 """Simple MPyL build runner"""
 
 import logging
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional
 
+from jsonschema import ValidationError
 from rich.console import Console
 from rich.logging import RichHandler
 from rich.markdown import Markdown
 
-from ...project import load_project, Stage, Project
-from ...reporting.formatting.markdown import run_result_to_markdown
-from ...reporting.targets import Reporter
-from ...stages.discovery import for_stage, find_invalidated_projects_per_stage
-from ...steps.models import RunProperties
-from ...steps.run import RunResult
-from ...steps.steps import Steps
-from ...utilities.repo import Repository, RepoConfig
+from ....project import load_project, Stage, Project
+from ....reporting.formatting.markdown import run_result_to_markdown
+from ....reporting.targets import Reporter
+from ....stages.discovery import for_stage, find_invalidated_projects_per_stage
+from ....steps.models import RunProperties
+from ....steps.run import RunResult
+from ....steps.steps import Steps, ExecutionException
+from ....utilities.repo import Repository, RepoConfig, Revision
 
 
 @dataclass(frozen=True)
 class MpylRunConfig:
     config: dict
     run_properties: RunProperties
 
 
 @dataclass(frozen=True)
 class MpylCliParameters:
     local: bool
+    tag: Optional[str] = None
+    pull_main: bool = False
     verbose: bool = False
     all: bool = False
 
 
 @dataclass(frozen=True)
 class MpylRunParameters:
     run_config: MpylRunConfig
@@ -40,82 +43,95 @@
 
 FORMAT = "%(name)s  %(message)s"
 
 
 def get_build_plan(logger: logging.Logger, repo: Repository, mpyl_run_parameters: MpylRunParameters) -> RunResult:
     params = mpyl_run_parameters.parameters
     logger.info(f"Running with {params}")
-    if not params.local:
-        pull_result = repo.pull_main_branch()
-        logger.info(f'Pulled `{pull_result[0].remote_ref_path.strip()}` to local')
+    branch = repo.get_branch
+    if branch:
+        if repo.main_branch_pulled:
+            logger.info(f'Branch `{repo.main_branch}` already present locally. Skipping pull.')
+        else:
+            logger.info(f'Pulling `{repo.main_branch}` from {repo.get_remote_url}')
+            pull_result = repo.pull_main_branch()
+            logger.info(f'Pulled `{pull_result[0].remote_ref_path.strip()}` to local')
+        changes = repo.changes_in_branch_including_local() if params.local else repo.changes_in_branch()
+    else:
+        changes = repo.changes_in_tagged_commit(params.tag) if params.tag else repo.changes_in_merge_commit()
+    logger.debug(f'Changes: {changes}')
 
-    changes_in_branch = repo.changes_in_branch_including_local() if params.local else repo.changes_in_branch()
-    logger.debug(f'Changes: {changes_in_branch}')
-
-    projects_per_stage: dict[Stage, set[Project]] = find_build_set(repo, changes_in_branch, params.all)
+    projects_per_stage: dict[Stage, set[Project]] = find_build_set(repo, changes, params.all)
     return RunResult(run_properties=mpyl_run_parameters.run_config.run_properties, run_plan=projects_per_stage)
 
 
 def run_mpyl(mpyl_run_parameters: MpylRunParameters, reporter: Optional[Reporter]) -> RunResult:
     params = mpyl_run_parameters.parameters
-    console = Console(markup=True, width=None if params.local else 135, no_color=False, log_path=False,
-                      color_system='256')
+    console_properties = mpyl_run_parameters.run_config.run_properties.console
+    console = Console(markup=True, width=None if params.local else console_properties.width, no_color=False,
+                      log_path=False, color_system='256')
+    print(f"Logging properties: {console_properties}, console: {console}")
     logging.basicConfig(
-        level="DEBUG" if params.verbose else "INFO", format=FORMAT, datefmt="[%X]",
+        level="DEBUG" if params.verbose else console_properties.log_level, format=FORMAT, datefmt="[%X]",
         handlers=[RichHandler(markup=True,
                               console=console, show_path=params.local)]
     )
     logger = logging.getLogger('mpyl')
     try:
-        with Repository(RepoConfig(mpyl_run_parameters.run_config.config)) as repo:
+        with Repository(RepoConfig.from_config(mpyl_run_parameters.run_config.config)) as repo:
 
             run_plan = get_build_plan(logger, repo, mpyl_run_parameters)
 
             if not run_plan.run_plan.items():
                 logger.info("Nothing to do. Exiting..")
                 return run_plan
 
-            logger.info("Building plan:")
+            logger.info("Build plan:")
             console.print(Markdown(f"\n\n{run_result_to_markdown(run_plan)}"))
 
             run_result: RunResult = run_plan
+            if reporter:
+                reporter.send_report(run_plan)
             try:
                 steps = Steps(logger=logger, properties=mpyl_run_parameters.run_config.run_properties)
-                run_result = run_build(run_plan, steps, reporter)
-            except Exception as exc:  # pylint: disable=broad-except
+                run_result = run_build(run_plan, steps, reporter, mpyl_run_parameters.parameters.local)
+            except ValidationError as exc:
+                console.log(f'Schema validation failed {exc.message} at `{".".join(map(str, exc.path))}`')
+                raise exc
+            except ExecutionException as exc:
+                run_result.exception = exc
                 console.log(f'Exception during build execution: {exc}')
                 console.print_exception()
-                run_result.exception = exc
 
-            console.print(run_result.status_line)
             console.print(Markdown(run_result_to_markdown(run_result)))
             return run_result
 
     except Exception as exc:
         console.log(f'Unexpected exception: {exc}')
         console.print_exception()
         raise exc
 
 
-def find_build_set(repo: Repository, changes_in_branch, build_all: bool) -> dict[Stage, set[Project]]:
+def find_build_set(repo: Repository, changes_in_branch: list[Revision], build_all: bool) -> dict[Stage, set[Project]]:
     project_paths = repo.find_projects()
-    all_projects = set(map(lambda p: load_project(Path("."), Path(p), False), project_paths))
+    all_projects = set(map(lambda p: load_project(Path(""), Path(p), False), project_paths))
 
     if build_all:
         return {Stage.BUILD: for_stage(all_projects, Stage.BUILD),
                 Stage.TEST: for_stage(all_projects, Stage.TEST),
-                Stage.DEPLOY: for_stage(all_projects, Stage.DEPLOY)}
+                Stage.DEPLOY: for_stage(all_projects, Stage.DEPLOY),
+                Stage.POST_DEPLOY: for_stage(all_projects, Stage.POST_DEPLOY)}
 
     return find_invalidated_projects_per_stage(all_projects, changes_in_branch)
 
 
-def run_build(accumulator: RunResult, executor: Steps, reporter: Optional[Reporter] = None):
+def run_build(accumulator: RunResult, executor: Steps, reporter: Optional[Reporter] = None, dry_run: bool = True):
     for stage, projects in accumulator.run_plan.items():
         for proj in projects:
-            result = executor.execute(stage, proj, True)
+            result = executor.execute(stage, proj, dry_run)
             accumulator.append(result)
             if reporter:
                 reporter.send_report(accumulator)
 
             if not result.output.success:
                 logging.warning(f'Build failed at {stage} for {proj.name}')
                 return accumulator
```

## Comparing `mpyl/cli/commands/meta_info.py` & `mpyl/cli/meta_info.py`

 * *Files identical despite different names*

## Comparing `mpyl/steps/deploy/k8s/resources/schema/traeffik.schema.yml` & `mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # source: "https://raw.githubusercontent.com/sleighzy/k3s-traefik-v2-kubernetes-crd/master/001-crd.yaml"
 $schema: "http://json-schema.org/draft-07/schema#"
-$id: "http://vandebron.nl/treaffik.schema.yaml"
+$id: "http://vandebron.nl/traefik.ingress.schema.yml"
 description: IngressRoute is the CRD implementation of a Traefik HTTP Router.
 properties:
   apiVersion:
     description: 'APIVersion defines the versioned schema of this representation
     of an object. Servers should convert recognized schemas to the latest
     internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources'
     type: string
```

## Comparing `mpyl-0.0.9.dist-info/LICENSE` & `mpyl-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

