# Comparing `tmp/invoker_terminal-0.0.0.tar.gz` & `tmp/invoker_terminal-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invoker_terminal-0.0.0.tar", last modified: Tue May 30 18:49:36 2023, max compression
+gzip compressed data, was "invoker_terminal-0.1.0.tar", last modified: Fri May 26 06:25:37 2023, max compression
```

## Comparing `invoker_terminal-0.0.0.tar` & `invoker_terminal-0.1.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:49:36.091614 invoker_terminal-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-30 18:49:36.091614 invoker_terminal-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:49:36.087614 invoker_terminal-0.0.0/invoker_terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/ast_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:49:36.091614 invoker_terminal-0.0.0/invoker_terminal/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/commands/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/commands/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/commands/ipfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/commands/new_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/commands/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/commands/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:49:36.091614 invoker_terminal-0.0.0/invoker_terminal/cores/
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/cores/anchor.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/cores/invoker_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/cores/ipfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/cores/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:49:36.091614 invoker_terminal-0.0.0/invoker_terminal/idl/
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/idl/invoker_network_market.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:49:36.091614 invoker_terminal-0.0.0/invoker_terminal/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/inputs/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/inputs/fileinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/inputs/inputbase.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/inputs/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/inputs/rangeinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/inputs/selectinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/inputs/textinput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:49:36.091614 invoker_terminal-0.0.0/invoker_terminal/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/outputs/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:49:36.091614 invoker_terminal-0.0.0/invoker_terminal/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/storage/deployed_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/storage/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:49:36.091614 invoker_terminal-0.0.0/invoker_terminal/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/templates/Dockerfile_template
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/templates/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/invoker_terminal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:49:36.087614 invoker_terminal-0.0.0/invoker_terminal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-30 18:49:36.000000 invoker_terminal-0.0.0/invoker_terminal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-30 18:49:36.000000 invoker_terminal-0.0.0/invoker_terminal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:49:36.000000 invoker_terminal-0.0.0/invoker_terminal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-30 18:49:36.000000 invoker_terminal-0.0.0/invoker_terminal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 18:49:36.000000 invoker_terminal-0.0.0/invoker_terminal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 18:49:36.000000 invoker_terminal-0.0.0/invoker_terminal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:49:36.091614 invoker_terminal-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:49:36.091614 invoker_terminal-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 18:49:20.000000 invoker_terminal-0.0.0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:25:37.743483 invoker_terminal-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-26 06:25:37.743483 invoker_terminal-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:25:37.739483 invoker_terminal-0.1.0/invoker_terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/ast_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:25:37.739483 invoker_terminal-0.1.0/invoker_terminal/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/commands/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/commands/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/commands/ipfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/commands/new_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/commands/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/commands/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:25:37.739483 invoker_terminal-0.1.0/invoker_terminal/cores/
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/cores/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/cores/invoker_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/cores/ipfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/cores/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:25:37.739483 invoker_terminal-0.1.0/invoker_terminal/idl/
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/idl/invoker_network_market.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:25:37.739483 invoker_terminal-0.1.0/invoker_terminal/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/inputs/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/inputs/fileinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/inputs/inputbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/inputs/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/inputs/rangeinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/inputs/selectinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/inputs/textinput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:25:37.739483 invoker_terminal-0.1.0/invoker_terminal/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/outputs/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:25:37.743483 invoker_terminal-0.1.0/invoker_terminal/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/storage/deployed_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/storage/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:25:37.743483 invoker_terminal-0.1.0/invoker_terminal/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/templates/Dockerfile_template
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/templates/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/invoker_terminal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:25:37.739483 invoker_terminal-0.1.0/invoker_terminal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-26 06:25:37.000000 invoker_terminal-0.1.0/invoker_terminal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-26 06:25:37.000000 invoker_terminal-0.1.0/invoker_terminal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:25:37.000000 invoker_terminal-0.1.0/invoker_terminal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-26 06:25:37.000000 invoker_terminal-0.1.0/invoker_terminal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-26 06:25:37.000000 invoker_terminal-0.1.0/invoker_terminal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 06:25:37.000000 invoker_terminal-0.1.0/invoker_terminal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 06:25:37.743483 invoker_terminal-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:25:37.743483 invoker_terminal-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 06:25:28.000000 invoker_terminal-0.1.0/tests/test_base.py
```

### Comparing `invoker_terminal-0.0.0/LICENSE` & `invoker_terminal-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/PKG-INFO` & `invoker_terminal-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoker_terminal
-Version: 0.0.0
+Version: 0.1.0
 Summary: Awesome invoker_terminal created by m00dy
 Home-page: https://github.com/m00dy/invoker-terminal/
 Author: m00dy
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `invoker_terminal-0.0.0/README.md` & `invoker_terminal-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/ast_check.py` & `invoker_terminal-0.1.0/invoker_terminal/ast_check.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/cli.py` & `invoker_terminal-0.1.0/invoker_terminal/cli.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/client.py` & `invoker_terminal-0.1.0/invoker_terminal/client.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/commands/build.py` & `invoker_terminal-0.1.0/invoker_terminal/commands/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import os
 import docker
 from ..ast_check import model_check
 
 
 def cmd_build(args, config):
-    filesTocCheck = ["Dockerfile"]
+    filesTocCheck = ["Dockerfile", "init.py"]
     client = docker.DockerClient(base_url=config["system"]["docker_url"])
     for f in filesTocCheck:
         if not os.path.isfile(f):
             logging.info("Mising file {file}".format(file=f))
             os._exit(1)
     logging.info("Building...")
     try:
```

### Comparing `invoker_terminal-0.0.0/invoker_terminal/commands/daemon.py` & `invoker_terminal-0.1.0/invoker_terminal/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/commands/deploy.py` & `invoker_terminal-0.1.0/invoker_terminal/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/commands/init.py` & `invoker_terminal-0.1.0/invoker_terminal/commands/init.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/commands/new_task.py` & `invoker_terminal-0.1.0/invoker_terminal/commands/new_task.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/commands/status.py` & `invoker_terminal-0.1.0/invoker_terminal/commands/status.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/commands/test.py` & `invoker_terminal-0.1.0/invoker_terminal/commands/test.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/commands/wallet.py` & `invoker_terminal-0.1.0/invoker_terminal/commands/wallet.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/constants.py` & `invoker_terminal-0.1.0/invoker_terminal/constants.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/cores/anchor.py` & `invoker_terminal-0.1.0/invoker_terminal/cores/anchor.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/cores/invoker_init.py` & `invoker_terminal-0.1.0/invoker_terminal/cores/invoker_init.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/cores/ipfs.py` & `invoker_terminal-0.1.0/invoker_terminal/cores/ipfs.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/idl/invoker_network_market.json` & `invoker_terminal-0.1.0/invoker_terminal/idl/invoker_network_market.json`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/inputs/decorators.py` & `invoker_terminal-0.1.0/invoker_terminal/inputs/decorators.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/inputs/numberinput.py` & `invoker_terminal-0.1.0/invoker_terminal/inputs/numberinput.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/inputs/rangeinput.py` & `invoker_terminal-0.1.0/invoker_terminal/inputs/rangeinput.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/inputs/textinput.py` & `invoker_terminal-0.1.0/invoker_terminal/inputs/textinput.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/outputs/output.py` & `invoker_terminal-0.1.0/invoker_terminal/outputs/output.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/server.py` & `invoker_terminal-0.1.0/invoker_terminal/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,23 @@
     print("Daemon quitting..do some cleanup")
 
 
 # Restrict to a particular path.
 class RequestHandler(SimpleXMLRPCRequestHandler):
     rpc_paths = ("/RPC2",)
 
+
+# Create server
+# server = SimpleXMLRPCServer(("localhost", 10001),
+#                            requestHandler=RequestHandler)
+# server.register_introspection_functions()
+
+# Register pow() function; this will use the value of
+# pow.__name__ as the name, which is just 'pow'.
+
 import logging
 from logging.handlers import RotatingFileHandler
 
 logger = None
 
 quitFlag = 0
 
@@ -384,16 +393,17 @@
     process = current_process()
     atexit.register(exit_handler)
     # report if daemon process
     logging.info(f"Daemon process: {process.daemon}")
     host = config["system"]["xml_rpc_addr"]
     port = config["system"]["xml_rpc_port"]
     server = SimpleXMLRPCServer(
-        (host, int(port)), requestHandler=RequestHandler, logRequests=False
+        (host, int(port)), requestHandler=RequestHandler
     )
+    server.register_function(pow)
     server.register_function(quit)
     server.register_function(isAlive)
     server.register_function(get_contracts_list)
 
     threads = []
     threads.append(
         threading.Thread(target=account_listener, args=(argz, config))
```

### Comparing `invoker_terminal-0.0.0/invoker_terminal/storage/deployed_models.py` & `invoker_terminal-0.1.0/invoker_terminal/storage/deployed_models.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/templates/model.py` & `invoker_terminal-0.1.0/invoker_terminal/templates/model.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal/utils.py` & `invoker_terminal-0.1.0/invoker_terminal/utils.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/invoker_terminal.egg-info/PKG-INFO` & `invoker_terminal-0.1.0/invoker_terminal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoker-terminal
-Version: 0.0.0
+Version: 0.1.0
 Summary: Awesome invoker_terminal created by m00dy
 Home-page: https://github.com/m00dy/invoker-terminal/
 Author: m00dy
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `invoker_terminal-0.0.0/invoker_terminal.egg-info/SOURCES.txt` & `invoker_terminal-0.1.0/invoker_terminal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.0/setup.py` & `invoker_terminal-0.1.0/setup.py`

 * *Files identical despite different names*

