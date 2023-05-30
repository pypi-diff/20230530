# Comparing `tmp/snk-0.6.4.tar.gz` & `tmp/snk-0.6.5.tar.gz`

## Comparing `snk-0.6.4.tar` & `snk-0.6.5.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.4/Dockerfile
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 snk-0.6.4/mkdocs.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.4/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.4/docs/CNAME
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.4/docs/index.md
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snk-0.6.4/docs/reference/cli.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.4/docs/reference/errors.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.4/docs/reference/main.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.4/docs/reference/nest.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.4/snk/__about__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.4/snk/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.4/snk/errors.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 snk-0.6.4/snk/main.py
--rw-r--r--   0        0        0    15584 2020-02-02 00:00:00.000000 snk-0.6.4/snk/nest.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.4/snk/pipeline.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.4/snk/cli/__init__.py
--rw-r--r--   0        0        0    16958 2020-02-02 00:00:00.000000 snk-0.6.4/snk/cli/cli.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 snk-0.6.4/snk/cli/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.4/snk/cli/options.py
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 snk-0.6.4/snk/cli/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.4/tests/.DS_Store
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.4/tests/__init__.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snk-0.6.4/tests/conftest.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.4/tests/test_nest.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 snk-0.6.4/tests/test_pipline_cli.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.6.4/tests/test_snk.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.4/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/cov.fasta
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/bin/snk-basic-pipeline
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/pipeline/.snk
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/pipeline/cli.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/pipeline/config.yaml
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/pipeline/workflow/Snakefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/pipeline/workflow/envs/base.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.4/tests/data/pipeline/workflow/profiles/base/config.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.6.4/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.4/LICENSE.txt
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 snk-0.6.4/README.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 snk-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.5/Dockerfile
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 snk-0.6.5/mkdocs.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.5/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.5/docs/CNAME
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.5/docs/index.md
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 snk-0.6.5/docs/managing_pipelines.md
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snk-0.6.5/docs/reference/cli.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.5/docs/reference/errors.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.5/docs/reference/main.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.5/docs/reference/nest.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.5/snk/__about__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.5/snk/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.5/snk/errors.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 snk-0.6.5/snk/main.py
+-rw-r--r--   0        0        0    16300 2020-02-02 00:00:00.000000 snk-0.6.5/snk/nest.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.5/snk/pipeline.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.5/snk/cli/__init__.py
+-rw-r--r--   0        0        0    18076 2020-02-02 00:00:00.000000 snk-0.6.5/snk/cli/cli.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 snk-0.6.5/snk/cli/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.5/snk/cli/options.py
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 snk-0.6.5/snk/cli/utils.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.5/tests/.DS_Store
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.5/tests/__init__.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snk-0.6.5/tests/conftest.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.5/tests/test_nest.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 snk-0.6.5/tests/test_pipline_cli.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.6.5/tests/test_snk.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.5/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/cov.fasta
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/bin/snk-basic-pipeline
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/.snk
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/cli.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/config.yaml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/resources/data.txt
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/workflow/Snakefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/workflow/envs/base.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.5/tests/data/pipeline/workflow/profiles/base/config.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.6.5/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.5/LICENSE.txt
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 snk-0.6.5/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 snk-0.6.5/PKG-INFO
```

### Comparing `snk-0.6.4/mkdocs.yml` & `snk-0.6.5/mkdocs.yml`

 * *Files 23% similar despite different names*

```diff
@@ -22,10 +22,13 @@
 
 extra:
   social:
     - icon: fontawesome/solid/robot
       link: https://github.com/Wytamma/write-the
       name: Generated with write-the
 
+markdown_extensions:
+  - admonition
+  
 plugins:
 - search
 - mkdocstrings
```

### Comparing `snk-0.6.4/.github/workflows/publish.yml` & `snk-0.6.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/.github/workflows/tests.yml` & `snk-0.6.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/docs/index.md` & `snk-0.6.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/snk/main.py` & `snk-0.6.5/snk/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,28 +56,31 @@
 @app.command()
 def install(
     ctx: typer.Context,
     pipeline: str = typer.Argument(
         ..., help="Path, URL or Github name (user/repo) of the pipeline to install."
     ),
     name: Optional[str] = typer.Option(
-        None, help="Rename the pipeline (this name will be used to call the CLI.)"
+        None, 
+        "--name",
+        "-n",
+        help="Rename the pipeline (this name will be used to call the CLI.)"
     ),
     tag: Optional[str] = typer.Option(
         None,
         "--tag",
         "-t",
         help="Tag (version) of the pipeline to install. Can specify a branch name, or tag. If None the latest commit will be installed.",
     ),
     config: Optional[Path] = typer.Option(
         None, help="Specify a non-standard config location."
     ),
     resource: Optional[List[Path]] = typer.Option(
         [],
-        help="Specify a resource required to run the pipeline (copied to working dir at runtime).",
+        help="Specify resources additional to the resources folder required by the pipeline (copied to working dir at runtime).",
     ),
     force: Optional[bool] = typer.Option(
         False, "--force", "-f", help="Force install (overwrites existing installs)."
     ),
     editable: Optional[bool] = typer.Option(
         False, "--editable", "-e", help="Whether to install the pipeline in editable mode."
     ),
@@ -94,15 +97,15 @@
     try:
         installed_pipeline = nest.install(
             pipeline,
             editable=editable,
             name=name,
             tag=tag,
             config=config,
-            resources=resource,
+            additional_resources=resource,
             force=force
         )
     except PipelineExistsError as e:
         typer.secho(e, fg="red")
         raise typer.Exit()
     except PipelineNotFoundError as e:
         typer.secho(e, fg="red")
```

### Comparing `snk-0.6.4/snk/nest.py` & `snk-0.6.5/snk/nest.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,26 +89,27 @@
         self,
         pipeline: str,
         editable=False,
         name=None,
         tag=None,
         config: Path = None,
         force=False,
-        resources=[],
+        additional_resources=[],
     ) -> Pipeline:
         """
         Installs a Snakemake pipeline as a CLI.
         Args:
           pipeline (str): The URL of the repo or the path to the local pipeline.
           editable (bool, optional): Whether to install the pipeline in editable mode. Defaults to False.
           name (str, optional): The name of the pipeline. Defaults to None.
           tag (str, optional): The tag of the pipeline. Defaults to None.
           config (Path, optional): The path to the config file. Defaults to None.
           force (bool, optional): Whether to force the installation. Defaults to False.
-          resources (list, optional): A list of additional resources to copy. Defaults to [].
+          additional_resources (list, optional): A list of resources additional to the resources folder to copy. Defaults to [].
+          symlink_resources_folder (bool, optional): Whether to symlink the resources folder instead of copying it. Defaults to False.
         Returns:
           Pipeline: The installed pipeline.
         Examples:
           >>> nest.install('https://github.com/example/repo.git', name='example', tag='v1.0.0')
         """
         def handle_force_installation(name: str):
             try:
@@ -138,16 +139,16 @@
                 handle_force_installation(name)
             pipeline_path = self.local(pipeline_local_path, name, editable)
         try:
             pipeline_executable = self.create_package(pipeline_path)
             self.link_pipeline_executable_to_bin(pipeline_executable)
             if config:
                 self.copy_nonstandard_config(pipeline_path, config)
-            if resources:
-                self.additional_resources(pipeline_path, resources)
+            if additional_resources:
+                self.additional_resources(pipeline_path, additional_resources)
             self._confirm_installation(name)
         except Exception as e:
             # remove any half completed steps
             to_remove = self.get_paths_to_delete(name)
             self.delete_paths(to_remove)
             raise e
         return Pipeline(pipeline_path)
@@ -159,15 +160,15 @@
           pipeline_dir (Path): The path to the pipeline directory.
           resources (List[Path]): A list of additional resources to copy.
         Examples:
           >>> nest.additional_resources(Path('/path/to/pipeline'), [Path('/path/to/resource1'), Path('/path/to/resource2')])
         """
         # validate_resources(resources)
         snk_config = SnkConfig.from_path(pipeline_dir / ".snk")
-        snk_config.resources += [r for r in resources if r not in snk_config.resources]
+        snk_config.resources += [str(r) for r in resources if r not in snk_config.resources]
         snk_config.to_yaml(pipeline_dir / ".snk")
 
     def copy_nonstandard_config(self, pipeline_dir: Path, config_path: Path):
         """
         Copy a nonstandard config file to the pipeline directory.
         Args:
           pipeline_dir (Path): The path to the pipeline directory.
@@ -193,14 +194,15 @@
         to_delete = []
 
         # remove repo
         pipeline_dir = self.pipelines_dir / pipeline_name
         if pipeline_dir.exists() and pipeline_dir.is_dir():
             to_delete.append(pipeline_dir)
         elif pipeline_dir.is_symlink():
+            # editable 
             to_delete.append(pipeline_dir)
         else:
             raise PipelineNotFoundError(f"Could not find pipeline: {pipeline_name}")
 
         # remove link
         pipeline_bin_executable = self.bin_dir / pipeline_name
         if pipeline_bin_executable.exists() and pipeline_bin_executable.is_symlink():
@@ -262,19 +264,19 @@
         return True
 
     def _check_pipeline_name_available(self, name: str):
         if not name:
             return None
         if name in os.listdir(self.pipelines_dir):
             raise PipelineExistsError(
-                f"Pipeline '{name}' already exists in {self.pipelines_dir}"
+                f"Pipeline '{name}' already exists in SNK_HOME ({self.pipelines_dir})"
             )
-        if name in os.listdir(self.bin_dir):
+        if name in os.listdir(self.bin_dir) and (not (self.bin_dir / name).is_symlink() or str(self.pipelines_dir) not in os.readlink(self.bin_dir / name)):
             raise PipelineExistsError(
-                f"Pipeline '{name}' already exists in {self.bin_dir}"
+                f"File '{name}' already exists in SNK_BIN ({self.bin_dir})" 
             )
 
     def _confirm_installation(self, name: str):
         """
         Confirms that the installation was successful.
         Args:
           name (str): The name of the pipeline.
@@ -405,23 +407,29 @@
           None
         Side Effects:
           Links a pipeline executable to the bin directory.
         Examples:
           >>> Nest.link_pipeline_executable_to_bin('my_executable')
         """
         name = pipeline_executable_path.name
-        os.symlink(pipeline_executable_path.absolute(), self.bin_dir / name)
+        if (self.bin_dir / name).is_symlink() and os.readlink(self.bin_dir / name) == str(pipeline_executable_path):
+            # skip if it's already there
+            return self.bin_dir / name
+        try:
+            os.symlink(pipeline_executable_path.absolute(), self.bin_dir / name)    
+        except FileExistsError:
+            raise PipelineExistsError(f"File '{name}' already exists in SNK_BIN ({self.bin_dir})")    
         return self.bin_dir / name
 
     def validate_SnakeMake_repo(self, repo: Repo):
         """
         Validates a SnakeMake repository.
         Args:
           repo_path (str): The path to the repository.
         Returns:
           bool: True if the repository is valid, False otherwise.
         Examples:
           >>> Nest.validate_SnakeMake_repo('/path/to/repo')
           True
         """
-        print("Skipping validation!")
+        #print("Skipping validation!")
         pass
```

### Comparing `snk-0.6.4/snk/pipeline.py` & `snk-0.6.5/snk/pipeline.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/snk/cli/cli.py` & `snk-0.6.5/snk/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,15 +190,20 @@
         """
         for path in snakemake.SNAKEFILE_CHOICES:
             if (self.pipeline.path / path).exists():
                 return self.pipeline.path / path
         raise FileNotFoundError("Snakefile not found!")
 
     @contextmanager
-    def copy_resources(self, resources: List[Path], cleanup: bool):
+    def copy_resources(
+            self, 
+            resources: List[Path], 
+            cleanup: bool, 
+            symlink_resources_folder: bool = False
+        ):
         """
         Copy resources to the current working directory.
         Args:
           resources (List[Path]): A list of paths to the resources to copy.
           cleanup (bool): If True, the resources will be removed after the function exits.
         Side Effects:
           Copies the resources to the current working directory.
@@ -212,21 +217,42 @@
 
         def copy_resource(src, dst):
             if src.is_dir():
                 shutil.copytree(src, dst)
             else:
                 shutil.copy(src, dst)
 
-        def remove_resource(resource):
-            if resource.is_dir():
+        def symlink_resource(src, dst):
+            target_is_directory = src.is_dir()
+            os.symlink(src, dst, target_is_directory=target_is_directory)
+
+        def remove_resource(resource: Path):
+            if resource.is_symlink():
+                resource.unlink()
+            elif resource.is_dir():
                 shutil.rmtree(resource)
             else:
                 os.remove(resource)
 
         try:
+            # 
+            resources_folder = self.pipeline.path / 'resources'
+            destination = Path(".") / 'resources'
+            if destination.exists():
+                typer.secho(
+                    "Resources folder exists! Skipping...\n",
+                    fg=typer.colors.RED,
+                )
+            else:
+                if resources_folder.exists():
+                    if symlink_resources_folder:
+                        symlink_resource(resources_folder, destination)
+                    else:
+                        copy_resource(resources_folder, destination)
+                    copied_resources.append(destination)
             for resource in resources:
                 abs_path = self.pipeline.path / resource
                 destination = Path(".") / resource.name
                 if not destination.exists():
                     # make sure you don't delete files that are already there...
                     copy_resource(abs_path, destination)
                     copied_resources.append(destination)
@@ -237,15 +263,15 @@
         finally:
             if not cleanup:
                 return
             for copied_resource in copied_resources:
                 if copied_resource.exists():
                     if self.verbose:
                         typer.secho(
-                            f"Deleting '{resource.name}' resource...",
+                            f"Deleting '{copied_resource.name}' resource...",
                             fg=typer.colors.YELLOW,
                         )
                     remove_resource(copied_resource)
 
     def run(
         self,
         ctx: typer.Context,
@@ -399,15 +425,19 @@
         if configs:
             args.extend(["--config", *configs])
         if verbose:
             typer.secho(f"snakemake {' '.join(args)}\n", fg=typer.colors.MAGENTA)
 
         self.snk_config.add_resources(resource, self.pipeline.path)
 
-        with self.copy_resources(self.snk_config.resources, cleanup=not keep_resources):
+        with self.copy_resources(
+            self.snk_config.resources, 
+            cleanup=not keep_resources, 
+            symlink_resources_folder=self.snk_config.symlink_resources_folder
+        ):
             try:
                 snakemake.main(args)
             except SystemExit as e:
                 status = int(str(e))
                 if status:
                     sys.exit(status)
         if not keep_snakemake and Path(".snakemake").exists():
```

### Comparing `snk-0.6.4/snk/cli/config.py` & `snk-0.6.5/snk/cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 class SnkConfig:
     """
     SNK config holds dynamic cli config and option annotations.
     """
 
     resources: List[Path] = field(default_factory=list)
     annotations: dict = field(default_factory=dict)
-
+    symlink_resources_folder: bool = False
+    
     @classmethod
     def from_path(cls, snk_config_path: Path):
         """
         Load and validate SNK config from .snk file.
         """
         if snk_config_path.exists():
             snk_config_dict = snakemake.load_configfile(snk_config_path)
```

### Comparing `snk-0.6.4/snk/cli/utils.py` & `snk-0.6.5/snk/cli/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/tests/.DS_Store` & `snk-0.6.5/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/tests/conftest.py` & `snk-0.6.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/tests/test_nest.py` & `snk-0.6.5/tests/test_nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/tests/test_pipline_cli.py` & `snk-0.6.5/tests/test_pipline_cli.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/tests/test_snk.py` & `snk-0.6.5/tests/test_snk.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/tests/utils.py` & `snk-0.6.5/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/tests/data/artic_v4.1.bed` & `snk-0.6.5/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/tests/data/config.yaml` & `snk-0.6.5/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/tests/data/cov.fasta` & `snk-0.6.5/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/LICENSE.txt` & `snk-0.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/README.md` & `snk-0.6.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# snk
+# SNK (Snek)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/snk.svg)](https://pypi.org/project/snk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/snk.svg)](https://pypi.org/project/snk)
 [![write-the - docs](https://badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://write-the.wytamma.com/)
 -----
 
 **Table of Contents**
@@ -15,15 +15,15 @@
 
 ```console
 pip install snk
 ```
 
 ## About
 
-Snk is a SnakeMake pipeline management system. Snk allows you to install SnakeMake pipelines as Command Line Interfaces (CLIs). Using a pipeline as a CLI increases its interoperability and allows complex pipelines to be used as modular components in a larger system.
+Snk (pronounced snek) is a SNaKemake pipeline management system. Snk allows you to install Snakemake pipelines as Command Line Interfaces (CLIs). Using a pipeline as a CLI increases its interoperability and allows complex pipelines to be used as modular components in a larger system. Snk, using python magic, will dynamic genrate the pipeline CLI using the pipeline configuration file.
 
 ## Basic Use
 
 ### Install a pipeline as a CLI
 
 ```
 snk install snakemake-workflows/rna-seq-star-deseq2
@@ -58,15 +58,15 @@
 ```
 
 You can also configure the pipeline using a config file. 
 
 ```
 rna-seq-star-deseq2 config # print the config 
 rna-seq-star-deseq2 config > config.yml # save the config 
-rna-seq-star-deseq2 run --configfile config.yml # run with config 
+rna-seq-star-deseq2 run --config config.yml # run with config 
 ```
 
 # how it works
 
 When installing a pipeline snk will
 
 - create directory `$PYTHON_BIN_DIR/../snk/pipelines/PIPELINE`
```

### Comparing `snk-0.6.4/pyproject.toml` & `snk-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snk-0.6.4/PKG-INFO` & `snk-0.6.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snk
-Version: 0.6.4
+Version: 0.6.5
 Project-URL: Documentation, https://github.com/wytamma/snk#readme
 Project-URL: Issues, https://github.com/wytamma/snk/issues
 Project-URL: Source, https://github.com/wytamma/snk
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,15 @@
 Requires-Dist: art
 Requires-Dist: gitpython
 Requires-Dist: makefun
 Requires-Dist: snakemake
 Requires-Dist: typer[all]
 Description-Content-Type: text/markdown
 
-# snk
+# SNK (Snek)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/snk.svg)](https://pypi.org/project/snk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/snk.svg)](https://pypi.org/project/snk)
 [![write-the - docs](https://badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://write-the.wytamma.com/)
 -----
 
 **Table of Contents**
@@ -41,15 +41,15 @@
 
 ```console
 pip install snk
 ```
 
 ## About
 
-Snk is a SnakeMake pipeline management system. Snk allows you to install SnakeMake pipelines as Command Line Interfaces (CLIs). Using a pipeline as a CLI increases its interoperability and allows complex pipelines to be used as modular components in a larger system.
+Snk (pronounced snek) is a SNaKemake pipeline management system. Snk allows you to install Snakemake pipelines as Command Line Interfaces (CLIs). Using a pipeline as a CLI increases its interoperability and allows complex pipelines to be used as modular components in a larger system. Snk, using python magic, will dynamic genrate the pipeline CLI using the pipeline configuration file.
 
 ## Basic Use
 
 ### Install a pipeline as a CLI
 
 ```
 snk install snakemake-workflows/rna-seq-star-deseq2
@@ -84,15 +84,15 @@
 ```
 
 You can also configure the pipeline using a config file. 
 
 ```
 rna-seq-star-deseq2 config # print the config 
 rna-seq-star-deseq2 config > config.yml # save the config 
-rna-seq-star-deseq2 run --configfile config.yml # run with config 
+rna-seq-star-deseq2 run --config config.yml # run with config 
 ```
 
 # how it works
 
 When installing a pipeline snk will
 
 - create directory `$PYTHON_BIN_DIR/../snk/pipelines/PIPELINE`
```

