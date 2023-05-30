# Comparing `tmp/tc_release-0.2.2.tar.gz` & `tmp/tc_release-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tc_release-0.2.2.tar", last modified: Wed Dec  1 19:16:27 2021, max compression
+gzip compressed data, was "tc_release-0.2.3.tar", last modified: Tue May 30 20:19:25 2023, max compression
```

## Comparing `tc_release-0.2.2.tar` & `tc_release-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,38 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-12-01 19:16:27.000000 tc_release-0.2.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)    68573 2021-12-01 19:16:10.000000 tc_release-0.2.2/versioneer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1069 2021-12-01 19:16:10.000000 tc_release-0.2.2/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      681 2021-12-01 19:16:10.000000 tc_release-0.2.2/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2021-12-01 19:16:27.000000 tc_release-0.2.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2021-12-01 19:16:10.000000 tc_release-0.2.2/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2021-12-01 19:16:27.000000 tc_release-0.2.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      125 2021-12-01 19:16:10.000000 tc_release-0.2.2/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-12-01 19:16:27.000000 tc_release-0.2.2/tc_release/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17236 2021-12-01 19:16:10.000000 tc_release-0.2.2/tc_release/tc_release.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       37 2021-12-01 19:16:10.000000 tc_release-0.2.2/tc_release/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      530 2021-12-01 19:16:10.000000 tc_release-0.2.2/tc_release/tcgvl.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2021-12-01 19:16:27.000000 tc_release-0.2.2/tc_release/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2021-12-01 19:16:10.000000 tc_release-0.2.2/tc_release/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-12-01 19:16:27.000000 tc_release-0.2.2/tc_release.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2021-12-01 19:16:27.000000 tc_release-0.2.2/tc_release.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      392 2021-12-01 19:16:27.000000 tc_release-0.2.2/tc_release.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2021-12-01 19:16:27.000000 tc_release-0.2.2/tc_release.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2021-12-01 19:16:27.000000 tc_release-0.2.2/tc_release.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-12-01 19:16:27.000000 tc_release-0.2.2/tc_release.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-12-01 19:16:27.000000 tc_release-0.2.2/tc_release.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.793781 tc_release-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-05-30 20:19:06.000000 tc_release-0.2.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-05-30 20:19:06.000000 tc_release-0.2.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-30 20:19:06.000000 tc_release-0.2.3/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-30 20:19:06.000000 tc_release-0.2.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.789781 tc_release-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.789781 tc_release-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-30 20:19:06.000000 tc_release-0.2.3/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1306 2023-05-30 20:19:06.000000 tc_release-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-05-30 20:19:06.000000 tc_release-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-30 20:19:06.000000 tc_release-0.2.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-30 20:19:06.000000 tc_release-0.2.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-05-30 20:19:06.000000 tc_release-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-30 20:19:06.000000 tc_release-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-05-30 20:19:25.793781 tc_release-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-05-30 20:19:06.000000 tc_release-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.789781 tc_release-0.2.3/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-05-30 20:19:06.000000 tc_release-0.2.3/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-30 20:19:06.000000 tc_release-0.2.3/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1047 2023-05-30 20:19:06.000000 tc_release-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-30 20:19:06.000000 tc_release-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 20:19:25.793781 tc_release-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.789781 tc_release-0.2.3/tc_release/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-30 20:19:06.000000 tc_release-0.2.3/tc_release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-30 20:19:06.000000 tc_release-0.2.3/tc_release/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17600 2023-05-30 20:19:06.000000 tc_release-0.2.3/tc_release/tc_release.py
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-05-30 20:19:06.000000 tc_release-0.2.3/tc_release/tcgvl.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.793781 tc_release-0.2.3/tc_release/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-30 20:19:06.000000 tc_release-0.2.3/tc_release/tests/test_pass.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-30 20:19:06.000000 tc_release-0.2.3/tc_release/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:19:25.793781 tc_release-0.2.3/tc_release.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-30 20:19:25.000000 tc_release-0.2.3/tc_release.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tc_release-0.2.2/README.md` & `tc_release-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tc_release-0.2.2/tc_release/tc_release.py` & `tc_release-0.2.3/tc_release/tc_release.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 # Late import, needs to be after the above on windows
 from git import Repo  # noqa isort:skip
 
 working_dir = os.path.join(os.getcwd(), dirname)
 
 template_file = os.path.join(os.path.dirname(__file__), 'tcgvl.txt')
-with open(template_file, 'r') as fd:
+with open(template_file) as fd:
     GlobalVersion_TcGVL = fd.read()
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description="Properly tags/version your TC project with GIT",
     )
@@ -103,19 +103,35 @@
             "decreases the log level by 10 for each count of -v, starting "
             "at the INFO level (20)."
         ),
     )
     return parser.parse_args()
 
 
-def find(pattern, path):
+def find(pattern: str, path: str) -> list[str]:
+    """
+    Case-insensitive recursive search of ``path`` for ``pattern``.
+
+    Parameters
+    ----------
+    pattern : str
+        The glob pattern to search for (e.g., "*.plcproj")
+
+    path : str
+        The top-level directory to search.
+
+    Returns
+    -------
+    List[str]
+        List of paths matching the pattern.
+    """
     result = []
-    for root, dirs, files in os.walk(path):
+    for root, _, files in os.walk(path):
         for name in files:
-            if fnmatch.fnmatch(name, pattern):
+            if fnmatch.fnmatch(name.lower(), pattern.lower()):
                 result.append(os.path.join(root, name))
     return result
 
 
 # Workaround for Windows file lock issues
 def remove_readonly(func, path, _):
     "Clear the readonly bit and reattempt the removal"
```

### Comparing `tc_release-0.2.2/tc_release/tcgvl.txt` & `tc_release-0.2.3/tc_release/tcgvl.txt`

 * *Files identical despite different names*

