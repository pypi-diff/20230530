# Comparing `tmp/spai-2023.5.30.post2.tar.gz` & `tmp/spai-2023.5.30.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2023.5.30.post2.tar", max compression
+gzip compressed data, was "spai-2023.5.30.post3.tar", max compression
```

## Comparing `spai-2023.5.30.post2.tar` & `spai-2023.5.30.post3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.30.post2/README.md
--rw-r--r--   0        0        0      380 2023-05-30 10:26:38.995933 spai-2023.5.30.post2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.30.post2/spai/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:47:16.135084 spai-2023.5.30.post2/spai/cli/__init__.py
--rw-r--r--   0        0        0     2858 2023-05-30 10:16:39.730147 spai-2023.5.30.post2/spai/cli/cloud.py
--rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.30.post2/spai/cli/commands/__init__.py
--rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.30.post2/spai/cli/commands/hello.py
--rw-r--r--   0        0        0     3165 2023-05-26 11:47:46.887246 spai-2023.5.30.post2/spai/cli/local.py
--rw-r--r--   0        0        0     5617 2023-05-26 12:00:02.150333 spai-2023.5.30.post2/spai/cli/project-template/README.md
--rw-r--r--   0        0        0      648 2023-05-26 11:56:34.213566 spai-2023.5.30.post2/spai/cli/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0     1570 2023-05-26 11:56:34.213566 spai-2023.5.30.post2/spai/cli/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0   780104 2023-05-26 11:56:34.213566 spai-2023.5.30.post2/spai/cli/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0   783403 2023-05-26 11:56:34.213566 spai-2023.5.30.post2/spai/cli/project-template/notebooks/analytics/output.ipynb
--rw-r--r--   0        0        0       54 2023-05-26 11:59:24.882199 spai-2023.5.30.post2/spai/cli/project-template/scripts/downloader/.env.example
--rw-r--r--   0        0        0     1198 2023-05-26 11:56:34.213566 spai-2023.5.30.post2/spai/cli/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0      524 2023-05-26 11:56:34.213566 spai-2023.5.30.post2/spai/cli/project-template/scripts/ndvi/main.py
--rw-r--r--   0        0        0      529 2023-05-26 12:01:08.490568 spai-2023.5.30.post2/spai/cli/project-template/spai.config.yml
--rw-r--r--   0        0        0     1421 2023-05-26 11:56:34.225566 spai-2023.5.30.post2/spai/cli/project-template/uis/map/main.py
--rw-r--r--   0        0        0     3496 2023-05-30 10:15:39.013958 spai-2023.5.30.post2/spai/cli/validate.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.30.post2/spai/data/__init__.py
--rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.30.post2/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.5.30.post2/spai/data/satellite/download.py
--rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.5.30.post2/spai/data/satellite/explore.py
--rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.30.post2/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.5.30.post2/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.5.30.post2/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.30.post2/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.5.30.post2/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.30.post2/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.5.30.post2/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.5.30.post2/spai/image/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.5.30.post2/spai/image/utils.py
--rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.5.30.post2/spai/image/xyz/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.5.30.post2/spai/image/xyz/cache.py
--rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.5.30.post2/spai/image/xyz/errors.py
--rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.5.30.post2/spai/image/xyz/get_image_tile.py
--rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.5.30.post2/spai/image/xyz/image_utils.py
--rw-r--r--   0        0        0     2937 2023-05-30 09:52:23.466805 spai-2023.5.30.post2/spai/main.py
--rw-r--r--   0        0        0     1915 2023-05-26 08:51:56.602852 spai-2023.5.30.post2/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     3605 2023-05-26 08:52:19.331037 spai-2023.5.30.post2/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     2537 2023-05-30 10:26:02.759827 spai-2023.5.30.post2/spai/storage/Storage.py
--rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.5.30.post2/spai/storage/__init__.py
--rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.5.30.post2/spai/storage/minio.py
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 spai-2023.5.30.post2/setup.py
--rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 spai-2023.5.30.post2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.30.post3/README.md
+-rw-r--r--   0        0        0      380 2023-05-30 17:28:06.654999 spai-2023.5.30.post3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.30.post3/spai/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:47:16.135084 spai-2023.5.30.post3/spai/cli/__init__.py
+-rw-r--r--   0        0        0     3997 2023-05-30 17:07:38.527006 spai-2023.5.30.post3/spai/cli/cloud.py
+-rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.30.post3/spai/cli/commands/__init__.py
+-rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.30.post3/spai/cli/commands/hello.py
+-rw-r--r--   0        0        0     3192 2023-05-30 14:36:50.431336 spai-2023.5.30.post3/spai/cli/local.py
+-rw-r--r--   0        0        0     5617 2023-05-26 12:00:02.150333 spai-2023.5.30.post3/spai/cli/project-template/README.md
+-rw-r--r--   0        0        0      648 2023-05-26 11:56:34.213566 spai-2023.5.30.post3/spai/cli/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0     1570 2023-05-26 11:56:34.213566 spai-2023.5.30.post3/spai/cli/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0   780104 2023-05-26 11:56:34.213566 spai-2023.5.30.post3/spai/cli/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0   783403 2023-05-26 11:56:34.213566 spai-2023.5.30.post3/spai/cli/project-template/notebooks/analytics/output.ipynb
+-rw-r--r--   0        0        0       54 2023-05-26 11:59:24.882199 spai-2023.5.30.post3/spai/cli/project-template/scripts/downloader/.env.example
+-rw-r--r--   0        0        0     1198 2023-05-26 11:56:34.213566 spai-2023.5.30.post3/spai/cli/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0      524 2023-05-26 11:56:34.213566 spai-2023.5.30.post3/spai/cli/project-template/scripts/ndvi/main.py
+-rw-r--r--   0        0        0      529 2023-05-26 12:01:08.490568 spai-2023.5.30.post3/spai/cli/project-template/spai.config.yml
+-rw-r--r--   0        0        0     1421 2023-05-26 11:56:34.225566 spai-2023.5.30.post3/spai/cli/project-template/uis/map/main.py
+-rw-r--r--   0        0        0     3692 2023-05-30 17:01:01.845727 spai-2023.5.30.post3/spai/cli/validate.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.30.post3/spai/data/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.30.post3/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.5.30.post3/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.5.30.post3/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.5.30.post3/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.5.30.post3/spai/image/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.5.30.post3/spai/image/utils.py
+-rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.5.30.post3/spai/image/xyz/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.5.30.post3/spai/image/xyz/cache.py
+-rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.5.30.post3/spai/image/xyz/errors.py
+-rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.5.30.post3/spai/image/xyz/get_image_tile.py
+-rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.5.30.post3/spai/image/xyz/image_utils.py
+-rw-r--r--   0        0        0     3065 2023-05-30 16:44:50.254663 spai-2023.5.30.post3/spai/main.py
+-rw-r--r--   0        0        0     1915 2023-05-26 08:51:56.602852 spai-2023.5.30.post3/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     3605 2023-05-26 08:52:19.331037 spai-2023.5.30.post3/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     2537 2023-05-30 10:26:02.759827 spai-2023.5.30.post3/spai/storage/Storage.py
+-rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.5.30.post3/spai/storage/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.5.30.post3/spai/storage/minio.py
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 spai-2023.5.30.post3/setup.py
+-rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 spai-2023.5.30.post3/PKG-INFO
```

### Comparing `spai-2023.5.30.post2/spai/cli/local.py` & `spai-2023.5.30.post3/spai/cli/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,17 +28,17 @@
         notebook,
         f"papermill main.ipynb output.ipynb",
     )
     # papermill can execute notebooks and save output in S3
     # papermill can execute notebooks with params
 
 
-def run_api(api, dir):
+def run_api(api, dir, port, host):
     os.chdir(dir)
-    os.system(f"python apis/{api.name}/main.py")
+    os.system(f"python apis/{api.name}/main.py --port {port} --host {host}")
 
 
 def run_ui(ui, dir):
     os.chdir(dir)
     os.system(ui.command)
 
 
@@ -49,46 +49,43 @@
 
 
 def run_local(dir, config, typer):
     typer.echo(f"Deploying locally...")
     keep_alive = False
     processes = []
     if config.scripts:
-        typer.echo(f"Deploying scripts...")
-        for (
-            script
-        ) in (
-            config.scripts
-        ):  # the order affects in the execution of the scheduled tasks
+        for script in config.scripts:
+            # the order affects in the execution of the scheduled tasks
+            typer.echo(f"Deploying scripts...")
             # # TODO: reqs, env
             if script.run_on_start:
                 run_script((script, dir, typer))
             if script.run_every:
                 keep_alive = True
-                schedule.every(script.run_every).seconds.do(
+                schedule.every(script.run_every).minutes.do(
                     run_script, (script, dir, typer)
                 )  # if a task goes after another than takes more time than the scheduled time, it will have to wait
     if config.notebooks:
         typer.echo(f"Deploying notebooks...")
         for notebook in config.notebooks:
             # TODO: reqs, env
             if notebook.run_on_start:
                 run_notebook((notebook, dir, typer))
             if notebook.run_every:
                 keep_alive = True
-                schedule.every(notebook.run_every).seconds.do(
+                schedule.every(notebook.run_every).minutes.do(
                     run_notebook, (notebook, dir, typer)
                 )
     if config.apis:
         typer.echo(f"Deploying apis...")
         for api in config.apis:
             typer.echo(f"Running api '{api.name}'...")
             # TODO: reqs, env
             # load_dotenv(f"{dir}/apis/{api.name}/.env")
-            p = Process(target=run_api, args=(api, dir))
+            p = Process(target=run_api, args=(api, dir, api.port, api.host))
             p.start()
             processes.append(p)
     if config.uis:
         typer.echo(f"Deploying uis...")
         for ui in config.uis:
             typer.echo(f"Running ui '{ui.name}'...")
             # TODO: reqs, env
```

### Comparing `spai-2023.5.30.post2/spai/cli/project-template/README.md` & `spai-2023.5.30.post3/spai/cli/project-template/README.md`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/cli/project-template/apis/analytics/main.py` & `spai-2023.5.30.post3/spai/cli/project-template/apis/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/cli/project-template/apis/xyz/main.py` & `spai-2023.5.30.post3/spai/cli/project-template/apis/xyz/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/cli/project-template/notebooks/analytics/main.ipynb` & `spai-2023.5.30.post3/spai/cli/project-template/notebooks/analytics/main.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/cli/project-template/notebooks/analytics/output.ipynb` & `spai-2023.5.30.post3/spai/cli/project-template/notebooks/analytics/output.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/cli/project-template/scripts/downloader/main.py` & `spai-2023.5.30.post3/spai/cli/project-template/scripts/downloader/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/cli/project-template/scripts/ndvi/main.py` & `spai-2023.5.30.post3/spai/cli/project-template/scripts/ndvi/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/cli/project-template/spai.config.yml` & `spai-2023.5.30.post3/spai/cli/project-template/spai.config.yml`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/cli/project-template/uis/map/main.py` & `spai-2023.5.30.post3/spai/cli/project-template/uis/map/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/cli/validate.py` & `spai-2023.5.30.post3/spai/cli/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,29 @@
 
 
 class NotebookConfig(BaseModel):
     name: str
     command: Union[str, None] = None
     run_every: Union[int, None] = None  # seconds
     run_on_start: bool = True
+    storage: Union[str, None] = None  # folder to bind in cloud
 
 
 class APIConfig(BaseModel):
     name: str
     command: Union[str, None] = None
+    port: int = 8000
+    host: str = "0.0.0.0"
+    storage: Union[str, None] = None  # folder to bind in cloud
 
 
 class UIConfig(BaseModel):
     name: str
     command: str  # steamlit, javascript, ...
+    port: int = 3000
 
 
 class Config(BaseModel):
     project: Union[str, None] = None
     scripts: Union[List[ScriptConfig], None] = None
     notebooks: Union[List[NotebookConfig], None] = None
     apis: Union[List[APIConfig], None] = None
```

### Comparing `spai-2023.5.30.post2/spai/data/satellite/download.py` & `spai-2023.5.30.post3/spai/data/satellite/download.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/data/satellite/explore.py` & `spai-2023.5.30.post3/spai/data/satellite/explore.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2023.5.30.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/image/utils.py` & `spai-2023.5.30.post3/spai/image/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/image/xyz/cache.py` & `spai-2023.5.30.post3/spai/image/xyz/cache.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/image/xyz/errors.py` & `spai-2023.5.30.post3/spai/image/xyz/errors.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/image/xyz/get_image_tile.py` & `spai-2023.5.30.post3/spai/image/xyz/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/image/xyz/image_utils.py` & `spai-2023.5.30.post3/spai/image/xyz/image_utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/main.py` & `spai-2023.5.30.post3/spai/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,60 +33,61 @@
     return typer.echo(f"Project {project} created")
 
 
 @app.command()
 def run(
     dir: Path = typer.Option(Path("."), "-d"),
     cloud: bool = typer.Option(False, "-c", "--cloud"),
+    rebuild: bool = typer.Option(False, "-r", "--rebuild"),  # force rebuild image
 ):
     # make sure dir is absolute
     dir = Path(dir).resolve()
     # load and validate config
     config = load_and_validate_config(dir, typer, cloud)
     # print(config)
     # run project
     if cloud:
-        return deploy_and_run_cloud(dir, config, typer)
+        return deploy_and_run_cloud(dir, config, typer, rebuild)
     return run_local(dir, config, typer)
 
 
 # API_URL = "http://localhost:8000"
-API_URL = "http://148.113.137.45:8010"
+# API_URL = "http://148.113.137.45:8002"
+API_URL = "https://spai.api.dev.earthpulse.ai"
 
 
 @app.command()
 def list(
     project: str = typer.Option(None, "-p", "--project"),
 ):
     project = "asd"
     response = requests.get(f"{API_URL}/projects/{project}")
     if response.status_code == 200:
-        data = response.json()
-        scripts = [k for k in data.keys()]
-        if len(scripts) == 0:
-            return typer.echo(f"No scripts running in project '{project}'.")
-        return typer.echo(f"Scripts in project '{project}': {scripts}")
+        services = response.json()
+        if len(services) == 0:
+            return typer.echo(f"No services running in project '{project}'.")
+        return typer.echo(f"Services in project '{project}': {services}")
     return typer.echo(response.json()["detail"])
 
 
 @app.command()
 def stop(
     project: str = typer.Option(None, "-p", "--project"),
 ):
     # list services
     project = "asd"
     response = requests.get(f"{API_URL}/projects/{project}")
-    data = response.json()
-    scripts = [k for k in data.keys()]
-    if len(scripts) == 0:
-        return typer.echo(f"No scripts running in project '{project}'.")
+    services = response.json()
+    if len(services) == 0:
+        return typer.echo(f"No services running in project '{project}'.")
     # delete services
-    for script in scripts:
-        typer.echo(f"Stopping script '{script}'...")
-        response = requests.get(f"{API_URL}/stop/script/{script}")
+    for service in services:
+        service_type, name = service.split(".")
+        typer.echo(f"Stopping service '{name}'...")
+        response = requests.get(f"{API_URL}/stop/{service_type}/{name}")
         if response.status_code == 200:
             typer.echo(f"Stopped.")
         else:
             typer.echo("Something went wrong.")
             typer.echo(response.json()["detail"])
     return typer.echo(f"Stopped all scripts in project '{project}'.")
```

### Comparing `spai-2023.5.30.post2/spai/storage/BaseStorage.py` & `spai-2023.5.30.post3/spai/storage/BaseStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/storage/CloudStorage.py` & `spai-2023.5.30.post3/spai/storage/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/storage/Storage.py` & `spai-2023.5.30.post3/spai/storage/Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/spai/storage/minio.py` & `spai-2023.5.30.post3/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.30.post2/setup.py` & `spai-2023.5.30.post3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ['minio>=7.1.15,<8.0.0', 'pandas>=2.0.2,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['spai = spai.main:app']}
 
 setup_kwargs = {
     'name': 'spai',
-    'version': '2023.5.30.post2',
+    'version': '2023.5.30.post3',
     'description': '',
     'long_description': '',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

