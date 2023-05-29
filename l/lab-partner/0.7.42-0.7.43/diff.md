# Comparing `tmp/lab-partner-0.7.42.tar.gz` & `tmp/lab-partner-0.7.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-0.7.42.tar", last modified: Mon May 29 22:56:41 2023, max compression
+gzip compressed data, was "lab-partner-0.7.43.tar", last modified: Mon May 29 23:21:11 2023, max compression
```

## Comparing `lab-partner-0.7.42.tar` & `lab-partner-0.7.43.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.447594 lab-partner-0.7.42/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.427593 lab-partner-0.7.42/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.435593 lab-partner-0.7.42/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     2674 2023-05-29 22:56:18.000000 lab-partner-0.7.42/.github/workflows/build-deploy.yml
--rw-r--r--   0 root         (0) root         (0)     3537 2023-05-29 22:56:18.000000 lab-partner-0.7.42/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4298 2023-05-29 22:56:18.000000 lab-partner-0.7.42/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 22:56:18.000000 lab-partner-0.7.42/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 22:56:41.447594 lab-partner-0.7.42/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-29 22:56:18.000000 lab-partner-0.7.42/README.md
--rwxr-xr-x   0 root         (0) root         (0)      841 2023-05-29 22:56:18.000000 lab-partner-0.7.42/build.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.431594 lab-partner-0.7.42/environments/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.435593 lab-partner-0.7.42/environments/local/
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-29 22:56:18.000000 lab-partner-0.7.42/environments/local/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     4368 2023-05-29 22:56:18.000000 lab-partner-0.7.42/environments/local/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.435593 lab-partner-0.7.42/environments/local/telemetry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.435593 lab-partner-0.7.42/environments/local/telemetry/certs/
--rw-r--r--   0 root         (0) root         (0)      985 2023-05-29 22:56:18.000000 lab-partner-0.7.42/environments/local/telemetry/certs/demo-data-prepper.crt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-29 22:56:18.000000 lab-partner-0.7.42/environments/local/telemetry/certs/demo-data-prepper.key
--rw-r--r--   0 root         (0) root         (0)     1444 2023-05-29 22:56:18.000000 lab-partner-0.7.42/environments/local/telemetry/certs/root-ca.pem
--rw-r--r--   0 root         (0) root         (0)     2355 2023-05-29 22:56:18.000000 lab-partner-0.7.42/environments/local/telemetry/certs/test_keystore.p12
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-29 22:56:18.000000 lab-partner-0.7.42/environments/local/telemetry/data-prepper-config.yaml
--rw-r--r--   0 root         (0) root         (0)      228 2023-05-29 22:56:18.000000 lab-partner-0.7.42/environments/local/telemetry/otel-collector-config.yml
--rw-r--r--   0 root         (0) root         (0)      862 2023-05-29 22:56:18.000000 lab-partner-0.7.42/environments/local/telemetry/pipelines.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.431594 lab-partner-0.7.42/images/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.435593 lab-partner-0.7.42/images/cli/
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-29 22:56:18.000000 lab-partner-0.7.42/images/cli/bashrc
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-29 22:56:18.000000 lab-partner-0.7.42/images/cli/cli_sudoers
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 22:56:18.000000 lab-partner-0.7.42/images/cli/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)       35 2023-05-29 22:56:18.000000 lab-partner-0.7.42/images/cli/start-cli.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.435593 lab-partner-0.7.42/images/jupyter/
--rw-r--r--   0 root         (0) root         (0)    33547 2023-05-29 22:56:18.000000 lab-partner-0.7.42/images/jupyter/jupyter_lab_config.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 22:56:18.000000 lab-partner-0.7.42/images/jupyter/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)      363 2023-05-29 22:56:18.000000 lab-partner-0.7.42/images/jupyter/start-jupyter.sh
--rwxr-xr-x   0 root         (0) root         (0)      647 2023-05-29 22:56:18.000000 lab-partner-0.7.42/install_from_source.sh
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-29 22:56:18.000000 lab-partner-0.7.42/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      280 2023-05-29 22:56:18.000000 lab-partner-0.7.42/run.sh
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 22:56:41.447594 lab-partner-0.7.42/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.431594 lab-partner-0.7.42/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.439594 lab-partner-0.7.42/src/lab_partner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 22:56:18.000000 lab-partner-0.7.42/src/lab_partner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.439594 lab-partner-0.7.42/src/lab_partner/docker/
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-29 22:56:18.000000 lab-partner-0.7.42/src/lab_partner/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4440 2023-05-29 22:56:18.000000 lab-partner-0.7.42/src/lab_partner/docker/daemon_info.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-05-29 22:56:18.000000 lab-partner-0.7.42/src/lab_partner/docker/rootless_container.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-05-29 22:56:18.000000 lab-partner-0.7.42/src/lab_partner/docker/run_builder.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-05-29 22:56:18.000000 lab-partner-0.7.42/src/lab_partner/docker/unix_user.py
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-29 22:56:18.000000 lab-partner-0.7.42/src/lab_partner/platform_utils.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-05-29 22:56:18.000000 lab-partner-0.7.42/src/lab_partner/process_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     2677 2023-05-29 22:56:18.000000 lab-partner-0.7.42/src/lab_partner/start_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.439594 lab-partner-0.7.42/src/lab_partner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 22:56:41.000000 lab-partner-0.7.42/src/lab_partner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1916 2023-05-29 22:56:41.000000 lab-partner-0.7.42/src/lab_partner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 22:56:41.000000 lab-partner-0.7.42/src/lab_partner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 22:56:41.000000 lab-partner-0.7.42/src/lab_partner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-29 22:56:41.000000 lab-partner-0.7.42/src/lab_partner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-29 22:56:41.000000 lab-partner-0.7.42/src/lab_partner.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.443594 lab-partner-0.7.42/tools/
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-29 22:56:18.000000 lab-partner-0.7.42/tools/README.md
--rw-r--r--   0 root         (0) root         (0)     1652 2023-05-29 22:56:18.000000 lab-partner-0.7.42/tools/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      846 2023-05-29 22:56:18.000000 lab-partner-0.7.42/tools/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.431594 lab-partner-0.7.42/tools/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.443594 lab-partner-0.7.42/tools/src/lab_partner_tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 22:56:18.000000 lab-partner-0.7.42/tools/src/lab_partner_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.443594 lab-partner-0.7.42/tools/src/lab_partner_tools/compose/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-05-29 22:56:18.000000 lab-partner-0.7.42/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-29 22:56:18.000000 lab-partner-0.7.42/tools/src/lab_partner_tools/dist.py
--rwxr-xr-x   0 root         (0) root         (0)     3276 2023-05-29 22:56:18.000000 lab-partner-0.7.42/tools/src/lab_partner_tools/services.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-05-29 22:56:18.000000 lab-partner-0.7.42/tools/src/lab_partner_tools/web_proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.447594 lab-partner-0.7.42/utils/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 22:56:18.000000 lab-partner-0.7.42/utils/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 22:56:18.000000 lab-partner-0.7.42/utils/README.md
--rw-r--r--   0 root         (0) root         (0)     1743 2023-05-29 22:56:18.000000 lab-partner-0.7.42/utils/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 22:56:18.000000 lab-partner-0.7.42/utils/run.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.431594 lab-partner-0.7.42/utils/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:56:41.447594 lab-partner-0.7.42/utils/src/lab_partner_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 22:56:18.000000 lab-partner-0.7.42/utils/src/lab_partner_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 22:56:18.000000 lab-partner-0.7.42/utils/src/lab_partner_utils/cli_command_factory.py
--rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 22:56:18.000000 lab-partner-0.7.42/utils/src/lab_partner_utils/command_builder.py
--rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 22:56:18.000000 lab-partner-0.7.42/utils/src/lab_partner_utils/commands.py
--rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 22:56:18.000000 lab-partner-0.7.42/utils/src/lab_partner_utils/kernel_launcher.py
--rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 22:56:18.000000 lab-partner-0.7.42/utils/src/lab_partner_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.714043 lab-partner-0.7.43/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.698043 lab-partner-0.7.43/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.702043 lab-partner-0.7.43/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-05-29 23:20:43.000000 lab-partner-0.7.43/.github/workflows/build-deploy.yml
+-rw-r--r--   0 root         (0) root         (0)     3537 2023-05-29 23:20:43.000000 lab-partner-0.7.43/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4298 2023-05-29 23:20:43.000000 lab-partner-0.7.43/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 23:20:43.000000 lab-partner-0.7.43/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 23:21:11.714043 lab-partner-0.7.43/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-29 23:20:43.000000 lab-partner-0.7.43/README.md
+-rwxr-xr-x   0 root         (0) root         (0)      841 2023-05-29 23:20:43.000000 lab-partner-0.7.43/build.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.698043 lab-partner-0.7.43/environments/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.702043 lab-partner-0.7.43/environments/local/
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-29 23:20:43.000000 lab-partner-0.7.43/environments/local/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-05-29 23:20:43.000000 lab-partner-0.7.43/environments/local/docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.706043 lab-partner-0.7.43/environments/local/telemetry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.706043 lab-partner-0.7.43/environments/local/telemetry/certs/
+-rw-r--r--   0 root         (0) root         (0)      985 2023-05-29 23:20:43.000000 lab-partner-0.7.43/environments/local/telemetry/certs/demo-data-prepper.crt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-29 23:20:43.000000 lab-partner-0.7.43/environments/local/telemetry/certs/demo-data-prepper.key
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-05-29 23:20:43.000000 lab-partner-0.7.43/environments/local/telemetry/certs/root-ca.pem
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-05-29 23:20:43.000000 lab-partner-0.7.43/environments/local/telemetry/certs/test_keystore.p12
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-29 23:20:43.000000 lab-partner-0.7.43/environments/local/telemetry/data-prepper-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      228 2023-05-29 23:20:43.000000 lab-partner-0.7.43/environments/local/telemetry/otel-collector-config.yml
+-rw-r--r--   0 root         (0) root         (0)      862 2023-05-29 23:20:43.000000 lab-partner-0.7.43/environments/local/telemetry/pipelines.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.702043 lab-partner-0.7.43/images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.706043 lab-partner-0.7.43/images/cli/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-29 23:20:43.000000 lab-partner-0.7.43/images/cli/bashrc
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-29 23:20:43.000000 lab-partner-0.7.43/images/cli/cli_sudoers
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 23:20:43.000000 lab-partner-0.7.43/images/cli/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)       35 2023-05-29 23:20:43.000000 lab-partner-0.7.43/images/cli/start-cli.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.706043 lab-partner-0.7.43/images/jupyter/
+-rw-r--r--   0 root         (0) root         (0)    33547 2023-05-29 23:20:43.000000 lab-partner-0.7.43/images/jupyter/jupyter_lab_config.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 23:20:43.000000 lab-partner-0.7.43/images/jupyter/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)      363 2023-05-29 23:20:43.000000 lab-partner-0.7.43/images/jupyter/start-jupyter.sh
+-rwxr-xr-x   0 root         (0) root         (0)      647 2023-05-29 23:20:43.000000 lab-partner-0.7.43/install_from_source.sh
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-29 23:20:43.000000 lab-partner-0.7.43/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      280 2023-05-29 23:20:43.000000 lab-partner-0.7.43/run.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 23:21:11.714043 lab-partner-0.7.43/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.702043 lab-partner-0.7.43/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.706043 lab-partner-0.7.43/src/lab_partner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 23:20:43.000000 lab-partner-0.7.43/src/lab_partner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.710043 lab-partner-0.7.43/src/lab_partner/docker/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-29 23:20:43.000000 lab-partner-0.7.43/src/lab_partner/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-05-29 23:20:43.000000 lab-partner-0.7.43/src/lab_partner/docker/daemon_info.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-05-29 23:20:43.000000 lab-partner-0.7.43/src/lab_partner/docker/rootless_container.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-05-29 23:20:43.000000 lab-partner-0.7.43/src/lab_partner/docker/run_builder.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-29 23:20:43.000000 lab-partner-0.7.43/src/lab_partner/docker/unix_user.py
+-rw-r--r--   0 root         (0) root         (0)      154 2023-05-29 23:20:43.000000 lab-partner-0.7.43/src/lab_partner/platform_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-05-29 23:20:43.000000 lab-partner-0.7.43/src/lab_partner/process_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     2668 2023-05-29 23:20:43.000000 lab-partner-0.7.43/src/lab_partner/start_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.710043 lab-partner-0.7.43/src/lab_partner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 23:21:11.000000 lab-partner-0.7.43/src/lab_partner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-05-29 23:21:11.000000 lab-partner-0.7.43/src/lab_partner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 23:21:11.000000 lab-partner-0.7.43/src/lab_partner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 23:21:11.000000 lab-partner-0.7.43/src/lab_partner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-29 23:21:11.000000 lab-partner-0.7.43/src/lab_partner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-29 23:21:11.000000 lab-partner-0.7.43/src/lab_partner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.710043 lab-partner-0.7.43/tools/
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-29 23:20:43.000000 lab-partner-0.7.43/tools/README.md
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-05-29 23:20:43.000000 lab-partner-0.7.43/tools/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      846 2023-05-29 23:20:43.000000 lab-partner-0.7.43/tools/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.702043 lab-partner-0.7.43/tools/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.710043 lab-partner-0.7.43/tools/src/lab_partner_tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 23:20:43.000000 lab-partner-0.7.43/tools/src/lab_partner_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.710043 lab-partner-0.7.43/tools/src/lab_partner_tools/compose/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-05-29 23:20:43.000000 lab-partner-0.7.43/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-29 23:20:43.000000 lab-partner-0.7.43/tools/src/lab_partner_tools/dist.py
+-rwxr-xr-x   0 root         (0) root         (0)     3276 2023-05-29 23:20:43.000000 lab-partner-0.7.43/tools/src/lab_partner_tools/services.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-05-29 23:20:43.000000 lab-partner-0.7.43/tools/src/lab_partner_tools/web_proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.710043 lab-partner-0.7.43/utils/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 23:20:43.000000 lab-partner-0.7.43/utils/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 23:20:43.000000 lab-partner-0.7.43/utils/README.md
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-05-29 23:20:43.000000 lab-partner-0.7.43/utils/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 23:20:43.000000 lab-partner-0.7.43/utils/run.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.702043 lab-partner-0.7.43/utils/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:21:11.714043 lab-partner-0.7.43/utils/src/lab_partner_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 23:20:43.000000 lab-partner-0.7.43/utils/src/lab_partner_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 23:20:43.000000 lab-partner-0.7.43/utils/src/lab_partner_utils/cli_command_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 23:20:43.000000 lab-partner-0.7.43/utils/src/lab_partner_utils/command_builder.py
+-rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 23:20:43.000000 lab-partner-0.7.43/utils/src/lab_partner_utils/commands.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 23:20:43.000000 lab-partner-0.7.43/utils/src/lab_partner_utils/kernel_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 23:20:43.000000 lab-partner-0.7.43/utils/src/lab_partner_utils/utils.py
```

### Comparing `lab-partner-0.7.42/.github/workflows/build-deploy.yml` & `lab-partner-0.7.43/.github/workflows/build-deploy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/.gitignore` & `lab-partner-0.7.43/.gitignore`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/Dockerfile` & `lab-partner-0.7.43/Dockerfile`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/LICENSE.md` & `lab-partner-0.7.43/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/PKG-INFO` & `lab-partner-0.7.43/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.42
+Version: 0.7.43
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.42/build.sh` & `lab-partner-0.7.43/build.sh`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/environments/local/docker-compose.yml` & `lab-partner-0.7.43/environments/local/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/environments/local/telemetry/certs/demo-data-prepper.crt` & `lab-partner-0.7.43/environments/local/telemetry/certs/demo-data-prepper.crt`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/environments/local/telemetry/certs/demo-data-prepper.key` & `lab-partner-0.7.43/environments/local/telemetry/certs/demo-data-prepper.key`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/environments/local/telemetry/certs/root-ca.pem` & `lab-partner-0.7.43/environments/local/telemetry/certs/root-ca.pem`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/environments/local/telemetry/certs/test_keystore.p12` & `lab-partner-0.7.43/environments/local/telemetry/certs/test_keystore.p12`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/environments/local/telemetry/pipelines.yaml` & `lab-partner-0.7.43/environments/local/telemetry/pipelines.yaml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/images/cli/bashrc` & `lab-partner-0.7.43/images/cli/bashrc`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/images/jupyter/jupyter_lab_config.py` & `lab-partner-0.7.43/images/jupyter/jupyter_lab_config.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/install_from_source.sh` & `lab-partner-0.7.43/install_from_source.sh`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/pyproject.toml` & `lab-partner-0.7.43/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/src/lab_partner/docker/daemon_info.py` & `lab-partner-0.7.43/src/lab_partner/docker/daemon_info.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/src/lab_partner/docker/rootless_container.py` & `lab-partner-0.7.43/src/lab_partner/docker/rootless_container.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/src/lab_partner/docker/run_builder.py` & `lab-partner-0.7.43/src/lab_partner/docker/run_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/src/lab_partner/docker/unix_user.py` & `lab-partner-0.7.43/src/lab_partner/docker/unix_user.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/src/lab_partner/process_utils.py` & `lab-partner-0.7.43/src/lab_partner/process_utils.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/src/lab_partner/start_cli.py` & `lab-partner-0.7.43/src/lab_partner/start_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 def start_cli():
     cli_env = {}
     docker_daemon_info = DockerDaemonInfo.build()
     rootless = RootlessDockerContainer(ROOTLESS_DOCKER_NAME, docker_daemon_info)
     if not docker_daemon_info.is_rootless():
         rootless.start_rootless_container(WORKSPACE, NETWORK_NAME)
         # overriding docker_daemon_info if starting the rootless container
-        docker_daemon_info = DockerDaemonInfo.build_via_tcp(ROOTLESS_DOCKER_NAME, ROOTLESS_DOCKER_PORT)
+        docker_daemon_info = DockerDaemonInfo.build_via_tcp('localhost', ROOTLESS_DOCKER_PORT)
         cli_env['DOCKER_HOST'] = f'tcp://localhost:{ROOTLESS_DOCKER_PORT}'
 
     cli_cmd = DockerRunBuilder(f'enclarify/lab-partner-cli:{version()}')
     cli_cmd.options() \
         .with_tty() \
         .with_env('DOCKER_HOST', f'tcp://{ROOTLESS_DOCKER_NAME}:2375') \
         .with_env('ENVIRONMENT', 'LOCAL') \
```

### Comparing `lab-partner-0.7.42/src/lab_partner.egg-info/PKG-INFO` & `lab-partner-0.7.43/src/lab_partner.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.42
+Version: 0.7.43
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.42/src/lab_partner.egg-info/SOURCES.txt` & `lab-partner-0.7.43/src/lab_partner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/tools/pyproject.toml` & `lab-partner-0.7.43/tools/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/tools/setup.cfg` & `lab-partner-0.7.43/tools/setup.cfg`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml` & `lab-partner-0.7.43/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/tools/src/lab_partner_tools/dist.py` & `lab-partner-0.7.43/tools/src/lab_partner_tools/dist.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/tools/src/lab_partner_tools/services.py` & `lab-partner-0.7.43/tools/src/lab_partner_tools/services.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/tools/src/lab_partner_tools/web_proxy.py` & `lab-partner-0.7.43/tools/src/lab_partner_tools/web_proxy.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/utils/LICENSE.md` & `lab-partner-0.7.43/utils/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/utils/pyproject.toml` & `lab-partner-0.7.43/utils/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/utils/src/lab_partner_utils/cli_command_factory.py` & `lab-partner-0.7.43/utils/src/lab_partner_utils/cli_command_factory.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/utils/src/lab_partner_utils/command_builder.py` & `lab-partner-0.7.43/utils/src/lab_partner_utils/command_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/utils/src/lab_partner_utils/commands.py` & `lab-partner-0.7.43/utils/src/lab_partner_utils/commands.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/utils/src/lab_partner_utils/kernel_launcher.py` & `lab-partner-0.7.43/utils/src/lab_partner_utils/kernel_launcher.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.42/utils/src/lab_partner_utils/utils.py` & `lab-partner-0.7.43/utils/src/lab_partner_utils/utils.py`

 * *Files identical despite different names*

