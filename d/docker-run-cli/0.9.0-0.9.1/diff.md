# Comparing `tmp/docker-run-cli-0.9.0.tar.gz` & `tmp/docker-run-cli-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/work/data01/reiher/git/ops/docker-run/docker-run/dist/.tmp-1hmq76im/docker-run-cli-0.9.0.tar", last modified: Tue May 30 10:40:04 2023, max compression
+gzip compressed data, was "/work/data01/reiher/git/ops/docker-run/docker-run/dist/.tmp-2azkfucz/docker-run-cli-0.9.1.tar", last modified: Tue May 30 10:53:29 2023, max compression
```

## Comparing `docker-run-cli-0.9.0.tar` & `docker-run-cli-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1123 2023-05-29 13:04:51.000000 docker-run-cli-0.9.0/LICENSE
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       51 2023-05-29 13:04:41.000000 docker-run-cli-0.9.0/MANIFEST.in
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     7348 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/PKG-INFO
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     5151 2023-05-30 10:21:45.000000 docker-run-cli-0.9.0/README.md
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1413 2023-05-30 08:33:27.000000 docker-run-cli-0.9.0/pyproject.toml
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/scripts/
--rwxrwxr-x   0 reiher   (16171) fb-5     (12389)     1620 2023-05-29 13:04:41.000000 docker-run-cli-0.9.0/scripts/activate-python-docker-run-shell-completion
--rwxrwxr-x   0 reiher   (16171) fb-5     (12389)     1102 2023-05-29 13:04:41.000000 docker-run-cli-0.9.0/scripts/docker-run
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       38 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/setup.cfg
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/src/
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/src/docker_run/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       45 2023-05-29 13:30:03.000000 docker-run-cli-0.9.0/src/docker_run/__init__.py
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      107 2023-05-29 13:04:41.000000 docker-run-cli-0.9.0/src/docker_run/__main__.py
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/src/docker_run/bash_completion.d/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     2886 2023-05-29 13:04:41.000000 docker-run-cli-0.9.0/src/docker_run/bash_completion.d/docker-run
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     6110 2023-05-29 13:04:41.000000 docker-run-cli-0.9.0/src/docker_run/core.py
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/src/docker_run/plugins/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)        0 2023-05-29 13:04:41.000000 docker-run-cli-0.9.0/src/docker_run/plugins/__init__.py
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     4566 2023-05-29 13:04:41.000000 docker-run-cli-0.9.0/src/docker_run/plugins/core.py
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      520 2023-05-29 13:04:41.000000 docker-run-cli-0.9.0/src/docker_run/plugins/plugin.py
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      758 2023-05-29 13:04:41.000000 docker-run-cli-0.9.0/src/docker_run/utils.py
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/src/docker_run_cli.egg-info/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     7348 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/src/docker_run_cli.egg-info/PKG-INFO
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      568 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/src/docker_run_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)        1 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/src/docker_run_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      144 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/src/docker_run_cli.egg-info/requires.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       11 2023-05-30 10:40:04.000000 docker-run-cli-0.9.0/src/docker_run_cli.egg-info/top_level.txt
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1123 2023-05-29 13:04:51.000000 docker-run-cli-0.9.1/LICENSE
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)       51 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/MANIFEST.in
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     7348 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/PKG-INFO
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     5151 2023-05-30 10:21:45.000000 docker-run-cli-0.9.1/README.md
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1420 2023-05-30 10:51:17.000000 docker-run-cli-0.9.1/pyproject.toml
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/scripts/
+-rwxrwxr-x   0 reiher   (16171) fb-5     (12389)     1620 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/scripts/activate-python-docker-run-shell-completion
+-rwxrwxr-x   0 reiher   (16171) fb-5     (12389)     1102 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/scripts/docker-run
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)       38 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/setup.cfg
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run/
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)       45 2023-05-30 10:51:33.000000 docker-run-cli-0.9.1/src/docker_run/__init__.py
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)      107 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/__main__.py
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run/bash_completion.d/
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     2886 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/bash_completion.d/docker-run
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     6110 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/core.py
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run/plugins/
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)        0 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/plugins/__init__.py
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     4566 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/plugins/core.py
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)      520 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/plugins/plugin.py
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)      758 2023-05-29 13:04:41.000000 docker-run-cli-0.9.1/src/docker_run/utils.py
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run_cli.egg-info/
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     7348 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)      568 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)        1 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)      151 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run_cli.egg-info/requires.txt
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)       11 2023-05-30 10:53:29.000000 docker-run-cli-0.9.1/src/docker_run_cli.egg-info/top_level.txt
```

### Comparing `docker-run-cli-0.9.0/LICENSE` & `docker-run-cli-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.0/PKG-INFO` & `docker-run-cli-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-cli
-Version: 0.9.0
+Version: 0.9.1
 Summary: 'docker run' and 'docker exec' with useful defaults
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.0 Summary: 'docker run'
+Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.1 Summary: 'docker run'
 and 'docker exec' with useful defaults Author-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> Maintainer-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> License: MIT License Copyright (c) 2023 Institute for
 Automotive Engineering (ika), RWTH Aachen University Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
```

### Comparing `docker-run-cli-0.9.0/README.md` & `docker-run-cli-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.0/pyproject.toml` & `docker-run-cli-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "docker-run-cli"
-version = "0.9.0"
+version = "0.9.1"
 description = "'docker run' and 'docker exec' with useful defaults"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Lennart Reiher", email = "lennart.reiher@rwth-aachen.de"},
     {name = "Jean-Pierre Busch", email = "jean-pierre.busch@rwth-aachen.de"},
 ]
@@ -24,15 +24,15 @@
 ]
 keywords = ["docker", "container"]
 dependencies = []
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
-docker-ros = ["docker-run-docker-ros"]
+docker-ros = ["docker-run-docker-ros>=1.0.1"]
 plugins = ["docker-run-cli[docker-ros]"]
 all = ["docker-run-cli[plugins]", "docker-run-cli[dev]"]
 
 [project.urls]
 "Repository" = "https://github.com/ika-rwth-aachen/docker-run"
 "Bug Tracker" = "https://github.com/ika-rwth-aachen/docker-run/issues"
```

### Comparing `docker-run-cli-0.9.0/scripts/activate-python-docker-run-shell-completion` & `docker-run-cli-0.9.1/scripts/activate-python-docker-run-shell-completion`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.0/scripts/docker-run` & `docker-run-cli-0.9.1/scripts/docker-run`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.0/src/docker_run/bash_completion.d/docker-run` & `docker-run-cli-0.9.1/src/docker_run/bash_completion.d/docker-run`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.0/src/docker_run/core.py` & `docker-run-cli-0.9.1/src/docker_run/core.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.0/src/docker_run/plugins/core.py` & `docker-run-cli-0.9.1/src/docker_run/plugins/core.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.0/src/docker_run/plugins/plugin.py` & `docker-run-cli-0.9.1/src/docker_run/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.0/src/docker_run/utils.py` & `docker-run-cli-0.9.1/src/docker_run/utils.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.0/src/docker_run_cli.egg-info/PKG-INFO` & `docker-run-cli-0.9.1/src/docker_run_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-cli
-Version: 0.9.0
+Version: 0.9.1
 Summary: 'docker run' and 'docker exec' with useful defaults
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.0 Summary: 'docker run'
+Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.1 Summary: 'docker run'
 and 'docker exec' with useful defaults Author-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> Maintainer-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> License: MIT License Copyright (c) 2023 Institute for
 Automotive Engineering (ika), RWTH Aachen University Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
```

### Comparing `docker-run-cli-0.9.0/src/docker_run_cli.egg-info/SOURCES.txt` & `docker-run-cli-0.9.1/src/docker_run_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

