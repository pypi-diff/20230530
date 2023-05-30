# Comparing `tmp/ssb_project_cli-1.1.1.tar.gz` & `tmp/ssb_project_cli-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_project_cli-1.1.1.tar", max compression
+gzip compressed data, was "ssb_project_cli-1.1.2.tar", max compression
```

## Comparing `ssb_project_cli-1.1.1.tar` & `ssb_project_cli-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1073 2023-05-26 14:07:02.708777 ssb_project_cli-1.1.1/LICENSE
--rw-r--r--   0        0        0     2881 2023-05-26 14:07:02.708777 ssb_project_cli-1.1.1/README.md
--rw-r--r--   0        0        0     2635 2023-05-26 14:07:15.249068 ssb_project_cli-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/__init__.py
--rw-r--r--   0        0        0      171 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/__main__.py
--rw-r--r--   0        0        0        0 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/py.typed
--rw-r--r--   0        0        0      257 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/__init__.py
--rw-r--r--   0        0        0     4305 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/app.py
--rw-r--r--   0        0        0       29 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/__init__.py
--rw-r--r--   0        0        0     3021 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/build.py
--rw-r--r--   0        0        0     3740 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/environment.py
--rw-r--r--   0        0        0     4947 2023-05-26 14:07:15.249068 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/poetry.py
--rw-r--r--   0        0        0     1886 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/prompt.py
--rw-r--r--   0        0        0     1644 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/temp_template_repo.py
--rw-r--r--   0        0        0       69 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build_cmds.md
--rw-r--r--   0        0        0       29 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/clean/__init__.py
--rw-r--r--   0        0        0     3008 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/clean/clean.py
--rw-r--r--   0        0        0       30 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/__init__.py
--rw-r--r--   0        0        0     6285 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/create.py
--rw-r--r--   0        0        0     9618 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/github.py
--rw-r--r--   0        0        0     6057 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/local_repo.py
--rw-r--r--   0        0        0     1631 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/prompt.py
--rw-r--r--   0        0        0      224 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/repo_privacy.py
--rw-r--r--   0        0        0     1303 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/temp_git_repo.py
--rw-r--r--   0        0        0      368 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/settings.py
--rw-r--r--   0        0        0     3209 2023-05-26 14:07:02.712777 ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/util.py
--rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 ssb_project_cli-1.1.1/setup.py
--rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 ssb_project_cli-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-30 13:47:12.702997 ssb_project_cli-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2881 2023-05-30 13:47:12.702997 ssb_project_cli-1.1.2/README.md
+-rw-r--r--   0        0        0     2635 2023-05-30 13:47:24.123110 ssb_project_cli-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/py.typed
+-rw-r--r--   0        0        0      257 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/__init__.py
+-rw-r--r--   0        0        0     4305 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/app.py
+-rw-r--r--   0        0        0       29 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/__init__.py
+-rw-r--r--   0        0        0     3158 2023-05-30 13:47:24.123110 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/build.py
+-rw-r--r--   0        0        0     3740 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/environment.py
+-rw-r--r--   0        0        0     4986 2023-05-30 13:47:24.123110 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/poetry.py
+-rw-r--r--   0        0        0     1886 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/prompt.py
+-rw-r--r--   0        0        0     1644 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/temp_template_repo.py
+-rw-r--r--   0        0        0       69 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build_cmds.md
+-rw-r--r--   0        0        0       29 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/clean/__init__.py
+-rw-r--r--   0        0        0     3008 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/clean/clean.py
+-rw-r--r--   0        0        0       30 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/__init__.py
+-rw-r--r--   0        0        0     6285 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/create.py
+-rw-r--r--   0        0        0     9618 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/github.py
+-rw-r--r--   0        0        0     6057 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/local_repo.py
+-rw-r--r--   0        0        0     1631 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/prompt.py
+-rw-r--r--   0        0        0      224 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/repo_privacy.py
+-rw-r--r--   0        0        0     1303 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/temp_git_repo.py
+-rw-r--r--   0        0        0      368 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/settings.py
+-rw-r--r--   0        0        0     3209 2023-05-30 13:47:12.706997 ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/util.py
+-rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 ssb_project_cli-1.1.2/PKG-INFO
```

### Comparing `ssb_project_cli-1.1.1/LICENSE` & `ssb_project_cli-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.1/README.md` & `ssb_project_cli-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.1/pyproject.toml` & `ssb_project_cli-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-project-cli"
-version = "1.1.1"
+version = "1.1.2"
 description = "SSB Project CLI"
 authors = ["Statistics Norway <stat-dev@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-project-cli"
 repository = "https://github.com/statisticsnorway/ssb-project-cli"
 documentation = "https://ssb-project-cli.readthedocs.io"
```

### Comparing `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/app.py` & `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/app.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/build.py` & `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/build.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,14 +68,16 @@
                 valid_project_git_config,
             )
 
     if running_onprem(JUPYTER_IMAGE_SPEC):
         print(
             ":twisted_rightwards_arrows:\tDetected onprem environment, using proxy for package installation"
         )
+        if poetry_source_includes_source_name(project_directory):
+            poetry_source_remove(project_directory, lock_update=False)
         poetry_source_add(PIP_INDEX_URL, project_directory)
     elif poetry_source_includes_source_name(project_directory):
         print(
             ":twisted_rightwards_arrows:\tDetected non-onprem environment, removing proxy for package installation"
         )
         poetry_source_remove(project_directory)
```

### Comparing `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/environment.py` & `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/environment.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/poetry.py` & `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/poetry.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,78 +54,84 @@
         "Error showing Poetry source.",
         cwd=cwd,
     )
 
     return source_name in result.stdout.decode("utf-8")
 
 
-def poetry_source_remove(cwd: Path, source_name: str = NEXUS_SOURCE_NAME) -> None:
+def poetry_source_remove(
+    cwd: Path, lock_update: bool = True, source_name: str = NEXUS_SOURCE_NAME
+) -> None:
     """Remove a package installation source for this project.
 
     Args:
         cwd: Path of project to add source to
+        lock_update: Bool used to decide whether to run update_lock
         source_name: Name of source to be removed
     """
     print("Removing Poetry source...")
     execute_command(
         f"poetry source remove {source_name}".split(" "),
         "source-remove",
         "Poetry source successfully removed!",
         "Failed to remove Poetry source.",
         cwd=cwd,
     )
-    print("Refreshing lock file...")
-    execute_command(
-        "poetry lock --no-update".split(" "),
-        "source-remove",
-        "Poetry successfully refreshed lock file!",
-        "Poetry failed to refresh lock file.",
-        cwd=cwd,
-    )
+    if lock_update:
+        update_lock(cwd)
 
 
 def poetry_source_add(
     source_url: str, cwd: Path, source_name: str = NEXUS_SOURCE_NAME
 ) -> None:
     """Add a package installation source for this project.
 
     Args:
         source_url: URL of 'simple' package API of package server
         cwd: Path of project to add source to
         source_name: Name of source to add
     """
     print("Adding package installation source for poetry...")
     execute_command(
-        f"poetry source add --priority=primary {source_name} {source_url}".split(" "),
+        f"poetry source add --priority=default {source_name} {source_url}".split(" "),
         "poetry-source-add",
         "Poetry source successfully added!",
         "Failed to add poetry source.",
         cwd=cwd,
     )
 
     # If the lock is created off-prem, we need to refresh the lock.
     if should_update_lock_file(source_url, cwd):
-        print("Refreshing lock file...")
-        execute_command(
-            "poetry lock --no-update".split(" "),
-            "source-remove",
-            "Poetry successfully refreshed lock file!",
-            "Poetry failed to refresh lock file.",
-            cwd=cwd,
-        )
+        update_lock(cwd)
+
+
+def update_lock(cwd: Path) -> None:
+    """Runs poetry lock --no-update command in CWD.
+
+    Args:
+        cwd: Path of project to add source to.
+    """
+    print("Refreshing lock file...")
+    execute_command(
+        "poetry lock --no-update".split(" "),
+        "update_lock",
+        "Poetry successfully refreshed lock file!",
+        "Poetry failed to refresh lock file.",
+        cwd=cwd,
+    )
 
 
 def should_update_lock_file(source_url: str, cwd: Path) -> bool:
     """Checks if poetry.lock exists and if nexus source is set there.
 
     Args:
         source_url: URL of 'simple' package API of package server
         cwd: Path of project to add source to
     Returns:
-        True if nexus source is not set in lock file, else False.
+        True if source url is not set in lock file, else False.
     """
     lock_file_path = cwd / Path("poetry.lock")
     if os.path.isfile(lock_file_path):
         with open(lock_file_path) as lock_file:
             if source_url in lock_file.read():
                 return False
     else:
```

### Comparing `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/prompt.py` & `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/prompt.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/build/temp_template_repo.py` & `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/build/temp_template_repo.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/clean/clean.py` & `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/clean/clean.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/create.py` & `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/create.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/github.py` & `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/github.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/local_repo.py` & `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/local_repo.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/prompt.py` & `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/prompt.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/create/temp_git_repo.py` & `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/create/temp_git_repo.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.1/src/ssb_project_cli/ssb_project/util.py` & `ssb_project_cli-1.1.2/src/ssb_project_cli/ssb_project/util.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.1.1/PKG-INFO` & `ssb_project_cli-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-project-cli
-Version: 1.1.1
+Version: 1.1.2
 Summary: SSB Project CLI
 Home-page: https://github.com/statisticsnorway/ssb-project-cli
 License: MIT
 Author: Statistics Norway
 Author-email: stat-dev@ssb.no
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 4 - Beta
```

