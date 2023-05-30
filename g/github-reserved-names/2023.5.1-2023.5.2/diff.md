# Comparing `tmp/github_reserved_names-2023.5.1.tar.gz` & `tmp/github_reserved_names-2023.5.2.tar.gz`

## Comparing `github_reserved_names-2023.5.1.tar` & `github_reserved_names-2023.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.flake8
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/github_reserved_names.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/noxfile.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/test_github_reserved_names.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.github/release.yml
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/.github/workflows/cron.yml
--rwxr-xr-x   0        0        0     1155 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/bin/check_for_differences
--rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/bin/parse_source_data
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/source_data/reserved-names.json
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/COPYING
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/README.rst
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/pyproject.toml
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/.flake8
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/github_reserved_names.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/noxfile.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/test_github_reserved_names.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/.github/release.yml
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/.github/workflows/cron.yml
+-rwxr-xr-x   0        0        0     1155 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/bin/check_for_differences
+-rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/bin/parse_source_data
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/source_data/reserved-names.json
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/COPYING
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/README.rst
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 github_reserved_names-2023.5.2/PKG-INFO
```

### Comparing `github_reserved_names-2023.5.1/.pre-commit-config.yaml` & `github_reserved_names-2023.5.2/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -8,33 +8,25 @@
       - id: check-vcs-permalinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.270"
+    hooks:
+      - id: ruff
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
-  - repo: https://github.com/PyCQA/flake8
-    rev: "6.0.0"
-    hooks:
-      - id: flake8
-  - repo: https://github.com/asottile/yesqa
-    rev: v1.4.0
-    hooks:
-      - id: yesqa
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
-    hooks:
-      - id: pyupgrade
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - name: black
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.4"
+    rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
```

### Comparing `github_reserved_names-2023.5.1/github_reserved_names.py` & `github_reserved_names-2023.5.2/github_reserved_names.py`

 * *Files identical despite different names*

### Comparing `github_reserved_names-2023.5.1/.github/SECURITY.md` & `github_reserved_names-2023.5.2/.github/SECURITY.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 # Security Policy
 
 ## Supported Versions
 
-In general, only the latest released `github-reserved-names` version is supported
-and will receive updates.
+In general, only the latest released `github-reserved-names` version is supported and will receive updates.
 
 ## Reporting a Vulnerability
 
-To report a security vulnerability, please send an email to
-`Julian+Security` at `GrayVines.com` with subject line `SECURITY (github-reserved-names)`.
+To report a security vulnerability, please send an email to `Julian+Security` at `GrayVines.com` with subject line `SECURITY (github-reserved-names)`.
 
-I will do my best to respond within 48 hours to acknowledge the message
-and discuss further steps.
+I will do my best to respond within 48 hours to acknowledge the message and discuss further steps.
 
-If the vulnerability is accepted, an advisory will be sent out via
-GitHub's security advisory functionality.
+If the vulnerability is accepted, an advisory will be sent out via GitHub's security advisory functionality.
 
-For non-sensitive discussion related to this policy itself, feel free to
-open an issue on the issue tracker.
+For non-sensitive discussion related to this policy itself, feel free to open an issue on the issue tracker.
```

### Comparing `github_reserved_names-2023.5.1/.github/workflows/ci.yml` & `github_reserved_names-2023.5.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `github_reserved_names-2023.5.1/bin/check_for_differences` & `github_reserved_names-2023.5.2/bin/check_for_differences`

 * *Files identical despite different names*

### Comparing `github_reserved_names-2023.5.1/source_data/reserved-names.json` & `github_reserved_names-2023.5.2/source_data/reserved-names.json`

 * *Files identical despite different names*

### Comparing `github_reserved_names-2023.5.1/COPYING` & `github_reserved_names-2023.5.2/COPYING`

 * *Files identical despite different names*

### Comparing `github_reserved_names-2023.5.1/README.rst` & `github_reserved_names-2023.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `github_reserved_names-2023.5.1/pyproject.toml` & `github_reserved_names-2023.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `github_reserved_names-2023.5.1/PKG-INFO` & `github_reserved_names-2023.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github_reserved_names
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: A list of paths that GitHub uses which aren't real users
 Project-URL: Homepage, https://github.com/Julian/github-reserved-names
 Project-URL: Issues, https://github.com/Julian/github-reserved-names/issues/
 Project-URL: Source, https://github.com/Julian/github-reserved-names
 Author: Julian Berman
 Author-email: Julian+github_reserved_names@GrayVines.com
 License: MIT
```

