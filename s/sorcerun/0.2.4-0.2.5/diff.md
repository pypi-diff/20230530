# Comparing `tmp/sorcerun-0.2.4.tar.gz` & `tmp/sorcerun-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorcerun-0.2.4.tar", last modified: Sun May 28 08:29:08 2023, max compression
+gzip compressed data, was "sorcerun-0.2.5.tar", last modified: Tue May 30 19:01:41 2023, max compression
```

## Comparing `sorcerun-0.2.4.tar` & `sorcerun-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:29:08.815688 sorcerun-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-28 08:28:55.000000 sorcerun-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-28 08:29:08.815688 sorcerun-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-28 08:28:55.000000 sorcerun-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 08:29:08.815688 sorcerun-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-28 08:28:55.000000 sorcerun-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:29:08.815688 sorcerun-0.2.4/sorcerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-28 08:29:08.000000 sorcerun-0.2.4/sorcerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-28 08:29:08.000000 sorcerun-0.2.4/sorcerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 08:29:08.000000 sorcerun-0.2.4/sorcerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-28 08:29:08.000000 sorcerun-0.2.4/sorcerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 08:29:08.000000 sorcerun-0.2.4/sorcerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-28 08:29:08.000000 sorcerun-0.2.4/sorcerun.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 08:29:08.815688 sorcerun-0.2.4/sorcerun_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 08:28:55.000000 sorcerun-0.2.4/sorcerun_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-28 08:28:55.000000 sorcerun-0.2.4/sorcerun_package/auth_mongodb_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-28 08:28:55.000000 sorcerun-0.2.4/sorcerun_package/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-28 08:28:55.000000 sorcerun-0.2.4/sorcerun_package/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-28 08:28:55.000000 sorcerun-0.2.4/sorcerun_package/mongodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-28 08:28:55.000000 sorcerun-0.2.4/sorcerun_package/sacred_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:01:41.480824 sorcerun-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-30 19:01:30.000000 sorcerun-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-30 19:01:41.480824 sorcerun-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-30 19:01:30.000000 sorcerun-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:01:41.480824 sorcerun-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-30 19:01:30.000000 sorcerun-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:01:41.480824 sorcerun-0.2.5/sorcerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-30 19:01:41.000000 sorcerun-0.2.5/sorcerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-30 19:01:41.000000 sorcerun-0.2.5/sorcerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:01:41.000000 sorcerun-0.2.5/sorcerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-30 19:01:41.000000 sorcerun-0.2.5/sorcerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 19:01:41.000000 sorcerun-0.2.5/sorcerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 19:01:41.000000 sorcerun-0.2.5/sorcerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:01:41.480824 sorcerun-0.2.5/sorcerun_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:01:30.000000 sorcerun-0.2.5/sorcerun_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-30 19:01:30.000000 sorcerun-0.2.5/sorcerun_package/auth_mongodb_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-05-30 19:01:30.000000 sorcerun-0.2.5/sorcerun_package/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 19:01:30.000000 sorcerun-0.2.5/sorcerun_package/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-30 19:01:30.000000 sorcerun-0.2.5/sorcerun_package/mongodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-30 19:01:30.000000 sorcerun-0.2.5/sorcerun_package/sacred_utils.py
```

### Comparing `sorcerun-0.2.4/LICENSE` & `sorcerun-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.4/PKG-INFO` & `sorcerun-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.4
+Version: 0.2.5
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.4/README.md` & `sorcerun-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.4/setup.py` & `sorcerun-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sorcerun",
-    version="0.2.4",
+    version="0.2.5",
     packages=find_packages(),
     install_requires=[
         "click",
         # "sacred @ git+https://github.com/rajatvd/sacred.git",
         "sacred==0.8.4",
         "pymongo",
         "pyyaml",
```

### Comparing `sorcerun-0.2.4/sorcerun.egg-info/PKG-INFO` & `sorcerun-0.2.5/sorcerun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.4
+Version: 0.2.5
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.4/sorcerun_package/auth_mongodb_option.py` & `sorcerun-0.2.5/sorcerun_package/auth_mongodb_option.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,10 +14,15 @@
     short_flag = "M"
     arg_description = """Path to authentication json file."""
 
     @classmethod
     def apply(cls, args, run):
         with open(args) as f:
             auth = json.loads(f.read())
-        client = MongoClient(**auth["client_kwargs"])
+        atlas = auth.get("atlas_connection_string", 0)
+        if atlas != 0:
+            print(atlas)
+            client = MongoClient(atlas)
+        else:
+            client = MongoClient(**auth["client_kwargs"])
         mongo = MongoObserver.create(db_name=auth["db_name"], client=client)
         run.observers.append(mongo)
```

### Comparing `sorcerun-0.2.4/sorcerun_package/cli.py` & `sorcerun-0.2.5/sorcerun_package/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,20 @@
     """
     Run Omniboard using the details saved in {AUTH_FILE}.
     """
     try:
         with open(AUTH_FILE, "r") as f:
             auth_data = json.load(f)
 
-        mongodb_uri = f"mongodb://{auth_data['client_kwargs']['username']}:{auth_data['client_kwargs']['password']}@{auth_data['client_kwargs']['host']}:{auth_data['client_kwargs']['port']}/{auth_data['db_name']}?authSource=admin"
+        atlas = auth_data.get("atlas_connection_string", 0)
+        mongodb_uri = (
+            f"{atlas}/{auth_data['db_name']}"
+            if atlas != 0
+            else f"mongodb://{auth_data['client_kwargs']['username']}:{auth_data['client_kwargs']['password']}@{auth_data['client_kwargs']['host']}:{auth_data['client_kwargs']['port']}/{auth_data['db_name']}?authSource=admin"
+        )
         # mongodb_uri = f'mongodb://{auth_data["client_kwargs"]["username"]}:{auth_data["client_kwargs"]["password"]}@127.0.0.1:27017/{auth_data["db_name"]}?authSource=admin'
 
         click.echo("Starting Omniboard...")
         with ExitStack() as stack:
             omniboard_process = subprocess.Popen(["omniboard", "--mu", mongodb_uri])
             stack.callback(omniboard_process.terminate)
             omniboard_process.wait()
```

### Comparing `sorcerun-0.2.4/sorcerun_package/mongodb_utils.py` & `sorcerun-0.2.5/sorcerun_package/mongodb_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.4/sorcerun_package/sacred_utils.py` & `sorcerun-0.2.5/sorcerun_package/sacred_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,16 +16,22 @@
 def run_sacred_experiment(adapter_func, config, auth_path=AUTH_FILE):
     experiment_name = getattr(adapter_func, "experiment_name", "sorcerun_experiment")
     ex = Experiment(experiment_name)
 
     with open(auth_path, "r") as f:
         auth_data = json.load(f)
 
+    atlas = auth_data.get("atlas_connection_string", 0)
+    url = (
+        atlas
+        if atlas != 0
+        else f"mongodb://{auth_data['client_kwargs']['username']}:{auth_data['client_kwargs']['password']}@{auth_data['client_kwargs']['host']}:{auth_data['client_kwargs']['port']}",
+    )
     observer = MongoObserver(
-        url=f"mongodb://{auth_data['client_kwargs']['username']}:{auth_data['client_kwargs']['password']}@{auth_data['client_kwargs']['host']}:{auth_data['client_kwargs']['port']}",
+        url=url,
         db_name=auth_data["db_name"],
     )
 
     ex.observers.append(observer)
 
     ex.add_config(config)
```

