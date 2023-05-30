# Comparing `tmp/pants_py_deploy-0.0.17-py3-none-any.whl.zip` & `tmp/pants_py_deploy-0.0.18-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11573 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-May-09 17:51 pants_py_deploy/__init__.py
--rw-r--r--  2.0 unx     4820 b- defN 23-May-09 17:51 pants_py_deploy/compose_file.py
--rw-r--r--  2.0 unx     7083 b- defN 23-May-09 17:51 pants_py_deploy/export_env.py
--rw-r--r--  2.0 unx     1453 b- defN 23-May-09 17:51 pants_py_deploy/fields.py
--rw-r--r--  2.0 unx     4812 b- defN 23-May-09 17:51 pants_py_deploy/models.py
--rw-r--r--  2.0 unx    10391 b- defN 23-May-09 17:51 pants_py_deploy/plugin.py
--rw-r--r--  2.0 unx      581 b- defN 23-May-09 17:51 pants_py_deploy/register.py
--rw-r--r--  2.0 unx     2179 b- defN 23-May-09 17:51 pants_py_deploy-0.0.17.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-09 17:51 pants_py_deploy-0.0.17.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-09 17:51 pants_py_deploy-0.0.17.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       16 b- defN 23-May-09 17:51 pants_py_deploy-0.0.17.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1028 b- defN 23-May-09 17:51 pants_py_deploy-0.0.17.dist-info/RECORD
-12 files, 32456 bytes uncompressed, 9823 bytes compressed:  69.7%
+Zip file size: 11593 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-May-30 12:37 pants_py_deploy/__init__.py
+-rw-r--r--  2.0 unx     4820 b- defN 23-May-30 12:37 pants_py_deploy/compose_file.py
+-rw-r--r--  2.0 unx     7083 b- defN 23-May-30 12:37 pants_py_deploy/export_env.py
+-rw-r--r--  2.0 unx     1453 b- defN 23-May-30 12:37 pants_py_deploy/fields.py
+-rw-r--r--  2.0 unx     4812 b- defN 23-May-30 12:37 pants_py_deploy/models.py
+-rw-r--r--  2.0 unx    10518 b- defN 23-May-30 12:37 pants_py_deploy/plugin.py
+-rw-r--r--  2.0 unx      581 b- defN 23-May-30 12:37 pants_py_deploy/register.py
+-rw-r--r--  2.0 unx     2179 b- defN 23-May-30 12:37 pants_py_deploy-0.0.18.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 12:37 pants_py_deploy-0.0.18.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-30 12:37 pants_py_deploy-0.0.18.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-May-30 12:37 pants_py_deploy-0.0.18.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1028 b- defN 23-May-30 12:37 pants_py_deploy-0.0.18.dist-info/RECORD
+12 files, 32583 bytes uncompressed, 9843 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pants_py_deploy/plugin.py
 Comment: 
 
 Filename: pants_py_deploy/register.py
 Comment: 
 
-Filename: pants_py_deploy-0.0.17.dist-info/METADATA
+Filename: pants_py_deploy-0.0.18.dist-info/METADATA
 Comment: 
 
-Filename: pants_py_deploy-0.0.17.dist-info/WHEEL
+Filename: pants_py_deploy-0.0.18.dist-info/WHEEL
 Comment: 
 
-Filename: pants_py_deploy-0.0.17.dist-info/namespace_packages.txt
+Filename: pants_py_deploy-0.0.18.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.17.dist-info/top_level.txt
+Filename: pants_py_deploy-0.0.18.dist-info/top_level.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.17.dist-info/RECORD
+Filename: pants_py_deploy-0.0.18.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pants_py_deploy/plugin.py

```diff
@@ -270,22 +270,27 @@
 
 
 @rule
 async def fix_docker_compose(
     request: DockerComposeFileFixer.Batch,
     compose_files: ComposeFiles,
 ) -> FixResult:
+    batch_files = set(request.files)
     input_snapshot = request.snapshot
     digest_contents = await Get(DigestContents, Digest, input_snapshot.digest)
     updated_contents = modify_existing_compose(compose_files, digest_contents)
     updates_paths = {file_content.path for file_content in updated_contents}
     new_files = compose_files.paths_managed.keys() - updates_paths
     new_contents = create_compose_files(new_files, compose_files)
-    all_contents = updated_contents + new_contents
-    output_snapshot = await Get(Snapshot, CreateDigest(all_contents))
+    batch_contents = [
+        content
+        for content in updated_contents + new_contents
+        if content.path in batch_files
+    ]
+    output_snapshot = await Get(Snapshot, CreateDigest(batch_contents))
     return FixResult(
         input=input_snapshot,
         output=output_snapshot,
         stdout="",
         stderr="",
         tool_name=DockerComposeFileFixer.tool_name,
     )
```

## Comparing `pants_py_deploy-0.0.17.dist-info/METADATA` & `pants_py_deploy-0.0.18.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pants-py-deploy
-Version: 0.0.17
+Version: 0.0.18
 Summary: Make it easy to maintain docker-compose files and helm-charts across projects with pants-py-deploy
 Home-page: https://github.com/EspenAlbert/py-libs
 Author: Espen Albert
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: <3.10,>=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: compose-chart-export (==0.0.17)
-Requires-Dist: docker-compose-parser (==0.0.17)
-Requires-Dist: model-lib (==0.0.17)
+Requires-Dist: compose-chart-export (==0.0.19)
+Requires-Dist: docker-compose-parser (==0.0.18)
+Requires-Dist: model-lib (==0.0.18)
 Requires-Dist: pantsbuild.pants (<2.17,>=2.16.0a0)
-Requires-Dist: zero-3rdparty (==0.0.17)
+Requires-Dist: zero-3rdparty (==0.0.18)
 
 # Pants py_deploy plugin
 - Purpose: Make it easy to maintain docker-compose files and helm-charts across projects
 - Goals
   - Support updating services.{service_name}.
     - `environment` by scanning source code
     - `ports` by scanning source code
```

## Comparing `pants_py_deploy-0.0.17.dist-info/RECORD` & `pants_py_deploy-0.0.18.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pants_py_deploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pants_py_deploy/compose_file.py,sha256=jc1kyOuc0XsBISQCm9yNs_yuwTVfwwY1T6HuXjYdp1c,4820
 pants_py_deploy/export_env.py,sha256=z0a7Sa2Lc4_7cFf9oH7rdoHjUqHgU-e6oshAQ9bm1Yg,7083
 pants_py_deploy/fields.py,sha256=EJwG5FndUPw17-AOVaNseZDmRZuVK46u6ZFYUMrAMlo,1453
 pants_py_deploy/models.py,sha256=PJHV-PFCayRC9KxpoTMjpO0iWiaO3H6q85xE6U4hnRs,4812
-pants_py_deploy/plugin.py,sha256=kIFZWHDQq6-jKl9Lnojmize5RR_aPukFEWqyUZEUjJg,10391
+pants_py_deploy/plugin.py,sha256=pI1ng6qKkC-Jo8PLZP7A6Td9tt6vpqjuiQBuMpK0eTs,10518
 pants_py_deploy/register.py,sha256=S9bQzA268aY9NXSfW-PvRuRKPvuFT-B86A3FvNbK53E,581
-pants_py_deploy-0.0.17.dist-info/METADATA,sha256=0kCmStqcO6pfNLni1_TO2n1rPYO4IzVfqg0ZP4ykJy0,2179
-pants_py_deploy-0.0.17.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pants_py_deploy-0.0.17.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pants_py_deploy-0.0.17.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
-pants_py_deploy-0.0.17.dist-info/RECORD,,
+pants_py_deploy-0.0.18.dist-info/METADATA,sha256=nFPingRWKvgO2OBgeZ-DrTr1Vi7pVHNhNxLYFwL1n3k,2179
+pants_py_deploy-0.0.18.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pants_py_deploy-0.0.18.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pants_py_deploy-0.0.18.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
+pants_py_deploy-0.0.18.dist-info/RECORD,,
```

