# Comparing `tmp/laminci-0.6.4.tar.gz` & `tmp/laminci-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laminci-0.6.4.tar", last modified: Tue May 30 09:01:21 2023, max compression
+gzip compressed data, was "laminci-0.6.5.tar", last modified: Tue May 30 09:06:27 2023, max compression
```

## Comparing `laminci-0.6.4.tar` & `laminci-0.6.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.6.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.6.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.6.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.6.4/.gitignore
--rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.6.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.6.4/README.md
--rw-r--r--   0        0        0     3052 2023-05-30 09:01:05.110946 laminci-0.6.4/docs/changelog.md
--rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.6.4/docs/guide/index.md
--rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.6.4/docs/guide/quickstart.ipynb
--rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.6.4/docs/index.md
--rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.6.4/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
--rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.6.4/docs/notes/index.md
--rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.6.4/lamin-project.yaml
--rw-r--r--   0        0        0      378 2023-05-30 09:00:53.083383 laminci-0.6.4/laminci/__init__.py
--rw-r--r--   0        0        0     2122 2023-05-26 16:17:30.304228 laminci-0.6.4/laminci/_artifacts.py
--rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.6.4/laminci/_db.py
--rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.6.4/laminci/_docs.py
--rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.6.4/laminci/_env.py
--rw-r--r--   0        0        0     2625 2023-05-30 09:00:30.741020 laminci-0.6.4/laminci/_nox.py
--rw-r--r--   0        0        0      148 2023-05-26 16:33:21.362381 laminci-0.6.4/laminci/db.py
--rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.6.4/laminci/nox.py
--rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.6.4/noxfile.py
--rw-r--r--   0        0        0      708 2023-05-28 21:50:19.140197 laminci-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.6.4/tests/test_artifacts.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 laminci-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.6.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.6.5/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.6.5/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.6.5/.gitignore
+-rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.6.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.6.5/README.md
+-rw-r--r--   0        0        0     3052 2023-05-30 09:01:05.110946 laminci-0.6.5/docs/changelog.md
+-rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.6.5/docs/guide/index.md
+-rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.6.5/docs/guide/quickstart.ipynb
+-rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.6.5/docs/index.md
+-rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.6.5/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
+-rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.6.5/docs/notes/index.md
+-rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.6.5/lamin-project.yaml
+-rw-r--r--   0        0        0      378 2023-05-30 09:06:24.198057 laminci-0.6.5/laminci/__init__.py
+-rw-r--r--   0        0        0     2122 2023-05-26 16:17:30.304228 laminci-0.6.5/laminci/_artifacts.py
+-rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.6.5/laminci/_db.py
+-rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.6.5/laminci/_docs.py
+-rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.6.5/laminci/_env.py
+-rw-r--r--   0        0        0     2745 2023-05-30 09:04:40.786977 laminci-0.6.5/laminci/_nox.py
+-rw-r--r--   0        0        0      148 2023-05-26 16:33:21.362381 laminci-0.6.5/laminci/db.py
+-rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.6.5/laminci/nox.py
+-rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.6.5/noxfile.py
+-rw-r--r--   0        0        0      708 2023-05-28 21:50:19.140197 laminci-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.6.5/tests/test_artifacts.py
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 laminci-0.6.5/PKG-INFO
```

### Comparing `laminci-0.6.4/.github/workflows/build.yml` & `laminci-0.6.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.4/.github/workflows/latest-changes.yml` & `laminci-0.6.5/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.4/.gitignore` & `laminci-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `laminci-0.6.4/.pre-commit-config.yaml` & `laminci-0.6.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.4/docs/changelog.md` & `laminci-0.6.5/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `laminci-0.6.4/docs/guide/quickstart.ipynb` & `laminci-0.6.5/docs/guide/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.6.4/docs/notes/YYYY-MM-DD-my-design-choice.ipynb` & `laminci-0.6.5/docs/notes/YYYY-MM-DD-my-design-choice.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.6.4/laminci/_artifacts.py` & `laminci-0.6.5/laminci/_artifacts.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.4/laminci/_db.py` & `laminci-0.6.5/laminci/_db.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.4/laminci/_env.py` & `laminci-0.6.5/laminci/_env.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.4/laminci/_nox.py` & `laminci-0.6.5/laminci/_nox.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,18 @@
     session.run(*init_instance.split(" "), external=True)
     # go back to the PR branch
     if "GITHUB_HEAD_REF" in os.environ and os.environ["GITHUB_HEAD_REF"] != "":
         session.run("git", "switch", os.environ["GITHUB_HEAD_REF"], external=True)
 
 
 def run_pre_commit(session: Session):
-    session.install("pre-commit")
+    if nox.options.default_venv_backend == "none":
+        session.run(*"pip install pre-commit".split())
+    else:
+        session.install("pre-commit")
     session.run("pre-commit", "install")
     session.run("pre-commit", "run", "--all-files")
 
 
 def run_pytest(session: Session, coverage: bool = True, env: Optional[Mapping] = None):
     package_name = get_package_name()
     coverage_args = (
```

### Comparing `laminci-0.6.4/pyproject.toml` & `laminci-0.6.5/pyproject.toml`

 * *Files identical despite different names*

