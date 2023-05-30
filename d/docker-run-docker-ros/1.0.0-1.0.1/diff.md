# Comparing `tmp/docker-run-docker-ros-1.0.0.tar.gz` & `tmp/docker-run-docker-ros-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/work/data01/reiher/git/ops/docker-run/docker-run-docker-ros/dist/.tmp-wzjgsrtc/docker-run-docker-ros-1.0.0.tar", last modified: Mon May 29 13:44:54 2023, max compression
+gzip compressed data, was "/work/data01/reiher/git/ops/docker-run/docker-run-docker-ros/dist/.tmp-mbix80ld/docker-run-docker-ros-1.0.1.tar", last modified: Tue May 30 10:52:45 2023, max compression
```

## Comparing `docker-run-docker-ros-1.0.0.tar` & `docker-run-docker-ros-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-29 13:44:54.000000 docker-run-docker-ros-1.0.0/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1123 2023-05-29 13:04:51.000000 docker-run-docker-ros-1.0.0/LICENSE
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     3983 2023-05-29 13:44:54.000000 docker-run-docker-ros-1.0.0/PKG-INFO
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1862 2023-05-29 13:04:41.000000 docker-run-docker-ros-1.0.0/README.md
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1047 2023-05-29 13:04:41.000000 docker-run-docker-ros-1.0.0/pyproject.toml
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       38 2023-05-29 13:44:54.000000 docker-run-docker-ros-1.0.0/setup.cfg
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-29 13:44:54.000000 docker-run-docker-ros-1.0.0/src/
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-29 13:44:54.000000 docker-run-docker-ros-1.0.0/src/docker_run/
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-29 13:44:54.000000 docker-run-docker-ros-1.0.0/src/docker_run/plugins/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1608 2023-05-29 13:04:41.000000 docker-run-docker-ros-1.0.0/src/docker_run/plugins/docker_ros.py
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-29 13:44:54.000000 docker-run-docker-ros-1.0.0/src/docker_run_docker_ros.egg-info/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     3983 2023-05-29 13:44:54.000000 docker-run-docker-ros-1.0.0/src/docker_run_docker_ros.egg-info/PKG-INFO
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      313 2023-05-29 13:44:54.000000 docker-run-docker-ros-1.0.0/src/docker_run_docker_ros.egg-info/SOURCES.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)        1 2023-05-29 13:44:54.000000 docker-run-docker-ros-1.0.0/src/docker_run_docker_ros.egg-info/dependency_links.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       11 2023-05-29 13:44:54.000000 docker-run-docker-ros-1.0.0/src/docker_run_docker_ros.egg-info/requires.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       11 2023-05-29 13:44:54.000000 docker-run-docker-ros-1.0.0/src/docker_run_docker_ros.egg-info/top_level.txt
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1123 2023-05-29 13:04:51.000000 docker-run-docker-ros-1.0.1/LICENSE
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     3983 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/PKG-INFO
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1862 2023-05-29 13:04:41.000000 docker-run-docker-ros-1.0.1/README.md
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1058 2023-05-30 10:50:48.000000 docker-run-docker-ros-1.0.1/pyproject.toml
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)       38 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/setup.cfg
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run/
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run/plugins/
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1608 2023-05-30 10:50:42.000000 docker-run-docker-ros-1.0.1/src/docker_run/plugins/docker_ros.py
+drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)     3983 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/PKG-INFO
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)      313 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/SOURCES.txt
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)        1 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/dependency_links.txt
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)       22 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/requires.txt
+-rw-rw-r--   0 reiher   (16171) fb-5     (12389)       11 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/top_level.txt
```

### Comparing `docker-run-docker-ros-1.0.0/LICENSE` & `docker-run-docker-ros-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-run-docker-ros-1.0.0/PKG-INFO` & `docker-run-docker-ros-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-docker-ros
-Version: 1.0.0
+Version: 1.0.1
 Summary: docker-run plugin for Docker images built by docker-ros
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
```

### Comparing `docker-run-docker-ros-1.0.0/README.md` & `docker-run-docker-ros-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `docker-run-docker-ros-1.0.0/pyproject.toml` & `docker-run-docker-ros-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "docker-run-docker-ros"
-version = "1.0.0"
+version = "1.0.1"
 description = "docker-run plugin for Docker images built by docker-ros"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Lennart Reiher", email = "lennart.reiher@rwth-aachen.de"},
     {name = "Jean-Pierre Busch", email = "jean-pierre.busch@rwth-aachen.de"},
 ]
@@ -19,13 +19,13 @@
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Operating System :: POSIX :: Linux",
 ]
 keywords = ["docker", "container", "ros"]
-dependencies = ["docker-run"]
+dependencies = ["docker-run-cli>=0.9.1"]
 requires-python = ">=3.7"
 
 [project.urls]
 "Repository" = "https://github.com/ika-rwth-aachen/docker-run"
 "Bug Tracker" = "https://github.com/ika-rwth-aachen/docker-run/issues"
```

### Comparing `docker-run-docker-ros-1.0.0/src/docker_run/plugins/docker_ros.py` & `docker-run-docker-ros-1.0.1/src/docker_run/plugins/docker_ros.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from typing import Any, Dict, List
 
 from docker_run.utils import runCommand
 from docker_run.plugins.plugin import Plugin
 
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 
 class DockerRosPlugin(Plugin):
 
     TARGET_MOUNT = "/docker-ros/ws/src/target"
 
     @classmethod
```

### Comparing `docker-run-docker-ros-1.0.0/src/docker_run_docker_ros.egg-info/PKG-INFO` & `docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-docker-ros
-Version: 1.0.0
+Version: 1.0.1
 Summary: docker-run plugin for Docker images built by docker-ros
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
```

