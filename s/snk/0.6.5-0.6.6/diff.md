# Comparing `tmp/snk-0.6.5.tar.gz` & `tmp/snk-0.6.6.tar.gz`

## Comparing `snk-0.6.5.tar` & `snk-0.6.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.5/Dockerfile
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 snk-0.6.5/mkdocs.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.5/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.5/docs/CNAME
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.5/docs/index.md
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 snk-0.6.5/docs/managing_pipelines.md
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snk-0.6.5/docs/reference/cli.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.5/docs/reference/errors.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.5/docs/reference/main.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.5/docs/reference/nest.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.5/snk/__about__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.5/snk/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.5/snk/errors.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 snk-0.6.5/snk/main.py
--rw-r--r--   0        0        0    16300 2020-02-02 00:00:00.000000 snk-0.6.5/snk/nest.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.5/snk/pipeline.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.5/snk/cli/__init__.py
--rw-r--r--   0        0        0    18076 2020-02-02 00:00:00.000000 snk-0.6.5/snk/cli/cli.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 snk-0.6.5/snk/cli/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.5/snk/cli/options.py
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 snk-0.6.5/snk/cli/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.5/tests/.DS_Store
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.5/tests/__init__.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snk-0.6.5/tests/conftest.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.5/tests/test_nest.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 snk-0.6.5/tests/test_pipline_cli.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.6.5/tests/test_snk.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.5/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/cov.fasta
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/bin/snk-basic-pipeline
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/.snk
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/cli.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/config.yaml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/resources/data.txt
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/workflow/Snakefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/workflow/envs/base.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/workflow/profiles/base/config.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.6.5/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.5/LICENSE.txt
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 snk-0.6.5/README.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 snk-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.6/Dockerfile
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 snk-0.6.6/mkdocs.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.6/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.6/docs/CNAME
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.6/docs/index.md
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 snk-0.6.6/docs/managing_pipelines.md
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snk-0.6.6/docs/reference/cli.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.6/docs/reference/errors.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.6/docs/reference/main.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.6/docs/reference/nest.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.6/snk/__about__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.6/snk/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.6/snk/errors.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 snk-0.6.6/snk/main.py
+-rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 snk-0.6.6/snk/nest.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.6/snk/pipeline.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.6/snk/cli/__init__.py
+-rw-r--r--   0        0        0    18076 2020-02-02 00:00:00.000000 snk-0.6.6/snk/cli/cli.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 snk-0.6.6/snk/cli/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.6/snk/cli/options.py
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 snk-0.6.6/snk/cli/utils.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.6/tests/.DS_Store
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.6/tests/__init__.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snk-0.6.6/tests/conftest.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.6/tests/test_nest.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 snk-0.6.6/tests/test_pipline_cli.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.6.6/tests/test_snk.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.6/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.6/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.6/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.6/tests/data/cov.fasta
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.6/tests/data/bin/snk-basic-pipeline
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 snk-0.6.6/tests/data/pipeline/.snk
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.6/tests/data/pipeline/cli.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk-0.6.6/tests/data/pipeline/config.yaml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk-0.6.6/tests/data/pipeline/resources/data.txt
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.6/tests/data/pipeline/workflow/Snakefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.6/tests/data/pipeline/workflow/envs/base.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.6/tests/data/pipeline/workflow/profiles/base/config.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.6.6/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.6/LICENSE.txt
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 snk-0.6.6/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 snk-0.6.6/PKG-INFO
```

### Comparing `snk-0.6.5/mkdocs.yml` & `snk-0.6.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/.github/workflows/publish.yml` & `snk-0.6.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/.github/workflows/tests.yml` & `snk-0.6.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/docs/index.md` & `snk-0.6.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/docs/managing_pipelines.md` & `snk-0.6.6/docs/managing_pipelines.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/snk/main.py` & `snk-0.6.6/snk/main.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/snk/nest.py` & `snk-0.6.6/snk/nest.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
           pipeline_dir (Path): The path to the pipeline directory.
           resources (List[Path]): A list of additional resources to copy.
         Examples:
           >>> nest.additional_resources(Path('/path/to/pipeline'), [Path('/path/to/resource1'), Path('/path/to/resource2')])
         """
         # validate_resources(resources)
         snk_config = SnkConfig.from_path(pipeline_dir / ".snk")
-        snk_config.resources += [str(r) for r in resources if r not in snk_config.resources]
+        snk_config.add_resources(resources, pipeline_dir)
         snk_config.to_yaml(pipeline_dir / ".snk")
 
     def copy_nonstandard_config(self, pipeline_dir: Path, config_path: Path):
         """
         Copy a nonstandard config file to the pipeline directory.
         Args:
           pipeline_dir (Path): The path to the pipeline directory.
```

### Comparing `snk-0.6.5/snk/pipeline.py` & `snk-0.6.6/snk/pipeline.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/snk/cli/cli.py` & `snk-0.6.6/snk/cli/cli.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/snk/cli/config.py` & `snk-0.6.6/snk/cli/config.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/snk/cli/utils.py` & `snk-0.6.6/snk/cli/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/tests/.DS_Store` & `snk-0.6.6/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/tests/conftest.py` & `snk-0.6.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/tests/test_nest.py` & `snk-0.6.6/tests/test_nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/tests/test_pipline_cli.py` & `snk-0.6.6/tests/test_pipline_cli.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/tests/test_snk.py` & `snk-0.6.6/tests/test_snk.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/tests/utils.py` & `snk-0.6.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/tests/data/artic_v4.1.bed` & `snk-0.6.6/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/tests/data/config.yaml` & `snk-0.6.6/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/tests/data/cov.fasta` & `snk-0.6.6/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/LICENSE.txt` & `snk-0.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/README.md` & `snk-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/pyproject.toml` & `snk-0.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snk-0.6.5/PKG-INFO` & `snk-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snk
-Version: 0.6.5
+Version: 0.6.6
 Project-URL: Documentation, https://github.com/wytamma/snk#readme
 Project-URL: Issues, https://github.com/wytamma/snk/issues
 Project-URL: Source, https://github.com/wytamma/snk
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

