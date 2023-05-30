# Comparing `tmp/omero-demo-cleanup-0.1.0.tar.gz` & `tmp/omero-demo-cleanup-0.1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-demo-cleanup-0.1.0.tar", last modified: Tue Nov 23 17:31:07 2021, max compression
+gzip compressed data, was "omero-demo-cleanup-0.1.1.dev0.tar", last modified: Tue May 30 11:24:45 2023, max compression
```

## Comparing `omero-demo-cleanup-0.1.0.tar` & `omero-demo-cleanup-0.1.1.dev0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 17:31:07.003521 omero-demo-cleanup-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    17987 2021-11-23 17:31:03.000000 omero-demo-cleanup-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2021-11-23 17:31:07.003521 omero-demo-cleanup-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      841 2021-11-23 17:31:03.000000 omero-demo-cleanup-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-23 17:31:07.003521 omero-demo-cleanup-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2145 2021-11-23 17:31:03.000000 omero-demo-cleanup-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 17:31:07.003521 omero-demo-cleanup-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 17:31:07.003521 omero-demo-cleanup-0.1.0/src/omero/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 17:31:07.003521 omero-demo-cleanup-0.1.0/src/omero/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      370 2021-11-23 17:31:03.000000 omero-demo-cleanup-0.1.0/src/omero/plugins/democleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 17:31:07.003521 omero-demo-cleanup-0.1.0/src/omero_demo_cleanup/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-23 17:31:03.000000 omero-demo-cleanup-0.1.0/src/omero_demo_cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4508 2021-11-23 17:31:03.000000 omero-demo-cleanup-0.1.0/src/omero_demo_cleanup/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9521 2021-11-23 17:31:03.000000 omero-demo-cleanup-0.1.0/src/omero_demo_cleanup/library.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 17:31:07.003521 omero-demo-cleanup-0.1.0/src/omero_demo_cleanup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2021-11-23 17:31:06.000000 omero-demo-cleanup-0.1.0/src/omero_demo_cleanup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      433 2021-11-23 17:31:06.000000 omero-demo-cleanup-0.1.0/src/omero_demo_cleanup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-23 17:31:06.000000 omero-demo-cleanup-0.1.0/src/omero_demo_cleanup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-11-23 17:31:06.000000 omero-demo-cleanup-0.1.0/src/omero_demo_cleanup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-11-23 17:31:06.000000 omero-demo-cleanup-0.1.0/src/omero_demo_cleanup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-23 17:31:06.000000 omero-demo-cleanup-0.1.0/src/omero_demo_cleanup.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:24:45.236095 omero-demo-cleanup-0.1.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-05-30 11:24:39.000000 omero-demo-cleanup-0.1.1.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-30 11:24:45.236095 omero-demo-cleanup-0.1.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-30 11:24:39.000000 omero-demo-cleanup-0.1.1.dev0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:24:45.236095 omero-demo-cleanup-0.1.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-30 11:24:39.000000 omero-demo-cleanup-0.1.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:24:45.232095 omero-demo-cleanup-0.1.1.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:24:45.232095 omero-demo-cleanup-0.1.1.dev0/src/omero/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:24:45.232095 omero-demo-cleanup-0.1.1.dev0/src/omero/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-30 11:24:39.000000 omero-demo-cleanup-0.1.1.dev0/src/omero/plugins/democleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:24:45.232095 omero-demo-cleanup-0.1.1.dev0/src/omero_demo_cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:24:39.000000 omero-demo-cleanup-0.1.1.dev0/src/omero_demo_cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-30 11:24:39.000000 omero-demo-cleanup-0.1.1.dev0/src/omero_demo_cleanup/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12245 2023-05-30 11:24:39.000000 omero-demo-cleanup-0.1.1.dev0/src/omero_demo_cleanup/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:24:45.236095 omero-demo-cleanup-0.1.1.dev0/src/omero_demo_cleanup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-30 11:24:45.000000 omero-demo-cleanup-0.1.1.dev0/src/omero_demo_cleanup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-30 11:24:45.000000 omero-demo-cleanup-0.1.1.dev0/src/omero_demo_cleanup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:24:45.000000 omero-demo-cleanup-0.1.1.dev0/src/omero_demo_cleanup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 11:24:45.000000 omero-demo-cleanup-0.1.1.dev0/src/omero_demo_cleanup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 11:24:45.000000 omero-demo-cleanup-0.1.1.dev0/src/omero_demo_cleanup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:24:45.000000 omero-demo-cleanup-0.1.1.dev0/src/omero_demo_cleanup.egg-info/zip-safe
```

### Comparing `omero-demo-cleanup-0.1.0/LICENSE.txt` & `omero-demo-cleanup-0.1.1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omero-demo-cleanup-0.1.0/setup.py` & `omero-demo-cleanup-0.1.1.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     return long_description
 
 
 long_description = get_long_description()
 
 setup(
     name="omero-demo-cleanup",
-    version="0.1.0",
+    version="0.1.1.dev0",
     packages=["omero_demo_cleanup", "omero.plugins"],
     package_dir={"": "src"},
     description="Plugin for managing the disk space on the demo server.",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Plugins",
         "Intended Audience :: Developers",
```

### Comparing `omero-demo-cleanup-0.1.0/src/omero_demo_cleanup/cli.py` & `omero-demo-cleanup-0.1.1.dev0/src/omero_demo_cleanup/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,21 @@
 
 import argparse
 from functools import wraps
 from typing import Any, Callable
 
 from omero.cli import BaseControl, Parser
 from omero.gateway import BlitzGateway
-from omero_demo_cleanup.library import choose_users, delete_data, resource_usage
+from omero_demo_cleanup.library import (
+    choose_users,
+    delete_data,
+    resource_usage,
+    users_by_id_or_username,
+    users_by_tag,
+)
 
 HELP = """Cleanup disk space on OMERO.server """
 
 
 def gateway_required(func: Callable) -> Callable:
     """
     Decorator which initializes a client (self.client),
@@ -81,19 +87,28 @@
             "--force",
             "-f",
             default=False,
             action="store_true",
             help="Perform the data deletion rather than running in dry-run mode."
             " Default: false.",
         )
+        parser.add_argument(
+            "--ignore-tag",
+            "-t",
+            default="NO DELETE",
+            help="Members tagged with this Tag (Name or ID) or child Tags are ignored.",
+        )
+        parser.add_argument(
+            "--ignore-users",
+            help="Ingore users: Comma-separated IDs and/or user-names.",
+        )
         parser.set_defaults(func=self.cleanup)
 
     @gateway_required
     def cleanup(self, args: argparse.Namespace) -> None:
-
         if args.inodes == 0 and args.gigabytes == 0:
             self.ctx.die(23, "Please specify how much to delete")
 
         try:
             # Perform data deletion.
             self.ctx.err(
                 "Ignoring users who have logged out within the past {} days.".format(
@@ -107,21 +122,25 @@
             if args.gigabytes > 0:
                 self.ctx.err(
                     "Aiming to delete at least {:,} bytes of data.".format(
                         args.gigabytes
                     )
                 )
 
-            stats = resource_usage(self.gateway, minimum_days=args.days)
-            users = choose_users(args.inodes, args.gigabytes * 1000 ** 3, stats)
+            ignore = users_by_tag(self.gateway, args.ignore_tag)
+            ignore.extend(users_by_id_or_username(self.gateway, args.ignore_users))
+            stats = resource_usage(
+                self.gateway, minimum_days=args.days, ignore_users=ignore
+            )
+            users = choose_users(args.inodes, args.gigabytes * 1000**3, stats)
             self.ctx.err(f"Found {len(users)} user(s) for deletion.")
             for user in users:
                 self.ctx.err(
                     'Deleting {} GB of data belonging to "{}" (#{}).'.format(
-                        user.size / 1000 ** 3,
+                        user.size / 1000**3,
                         user.name,
                         user.id,
                     )
                 )
                 dry_run = not args.force
                 if dry_run:
                     self.ctx.err("Despite output, will not actually delete any data.")
```

### Comparing `omero-demo-cleanup-0.1.0/src/omero_demo_cleanup/library.py` & `omero-demo-cleanup-0.1.1.dev0/src/omero_demo_cleanup/library.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     DiskUsage2,
     DiskUsage2Response,
     HandlePrx,
     LegalGraphTargets,
     LegalGraphTargetsResponse,
 )
 from omero.gateway import BlitzGateway
-from omero.rtypes import rlong
+from omero.rtypes import rlong, unwrap
 from omero.sys import ParametersI
 
 # If adjusting UserStats, find_worst, choose_users then check with unit tests.
 
 
 class UserStats:
     # Represents a user and their resource usage.
@@ -177,28 +177,99 @@
             object_ids.append(object_id)
         if object_ids:
             delete.targetObjects[delete_class] = object_ids
     if delete.targetObjects:
         submit(conn, delete, Delete2Response)
 
 
+def exp_to_str(exp):
+    # "user-3" (#6) Charles Darwin
+    full_name = f"{unwrap(exp.firstName)} {unwrap(exp.lastName)}"
+    return f'"{exp.omeName.val}" (#{exp.id.val}) {full_name}'
+
+
+def users_by_id_or_username(conn: BlitzGateway, ignore_users: str) -> List[int]:
+
+    if not ignore_users:
+        return []
+    exclude = []
+    users = ignore_users.split(",")
+    print(f"Ignoring {len(users)} users by ID or Username:")
+    for user_str in users:
+        if user_str.isnumeric():
+            exp = conn.getQueryService().get("Experimenter", int(user_str))
+            print("  " + exp_to_str(exp))
+            exclude.append(exp.id.val)
+        else:
+            exp = conn.getObject("Experimenter", attributes={"omeName": user_str})
+            if exp is None:
+                raise ValueError("Experimenter: %s not found" % user_str)
+            print("  " + exp_to_str(exp._obj))
+            exclude.append(exp.id)
+    return exclude
+
+
+def users_by_tag(conn: BlitzGateway, tag_name: str) -> List[int]:
+    # Get users linked to Tag (Name or ID) or linked to child Tags.
+    if not tag_name or tag_name == "None":
+        print("No Tag chosen for ingoring users")
+        return []
+    exclude = []
+    if tag_name.isnumeric():
+        tag = conn.getObject("Annotation", tag_name)
+    else:
+        tags = list(
+            conn.getObjects("TagAnnotation", attributes={"textValue": tag_name})
+        )
+        tag = tags[0] if len(tags) > 0 else None
+        if len(tags) > 1:
+            ids = [tag.id for tag in tags]
+            raise ValueError(f"Multiple Tags with name: {tag_name} ({ids})")
+    if tag is None:
+        raise ValueError("Tag: %s not found" % tag_name)
+    # Check if this is a Tag Group
+    tag_links = list(conn.getAnnotationLinks("Annotation", parent_ids=[tag.id]))
+
+    # Handle Tagged Experimenters first...
+    links = list(conn.getAnnotationLinks("Experimenter", ann_ids=[tag.id]))
+    exclude.extend([link.parent.id.val for link in links])
+    # If we have NO child Tags, then always print:
+    if len(links) > 0 or len(tag_links) == 0:
+        print(
+            "Ignoring %s users linked to Tag:%s %s:"
+            % (len(links), tag.id, tag.textValue)
+        )
+
+    for link in links:
+        print("  " + exp_to_str(link.parent))
+
+    # Then recursively check any child Tags...
+    if len(tag_links) > 0 or len(links) == 0:
+        print(f"Tag:{tag.id} {tag.textValue} has {len(tag_links)} child Tags...")
+    for link in tag_links:
+        exclude.extend(users_by_tag(conn, str(link.child.id.val)))
+
+    return exclude
+
+
 def find_users(
-    conn: BlitzGateway, minimum_days: int = 0
+    conn: BlitzGateway, minimum_days: int = 0, ignore_users: List[int] = []
 ) -> Tuple[Dict[int, str], Dict[int, int]]:
     # Determine which users' data to consider deleting.
 
     users = {}
 
     for result in conn.getQueryService().projection(
         "SELECT id, omeName FROM Experimenter", None
     ):
         user_id = result[0].val
         user_name = result[1].val
         if user_name not in ("PUBLIC", "guest", "root", "monitoring"):
-            users[user_id] = user_name
+            if user_id not in ignore_users:
+                users[user_id] = user_name
 
     for result in conn.getQueryService().projection(
         "SELECT DISTINCT owner.id FROM Session WHERE closed IS NULL", None
     ):
         user_id = result[0].val
         if user_id in users.keys():
             print(f'Ignoring "{users[user_id]}" (#{user_id}) who is logged in.')
@@ -231,20 +302,24 @@
             )
             del users[user_id]
 
         logouts[user_id] = user_logout
     return users, logouts
 
 
-def resource_usage(conn: BlitzGateway, minimum_days: int = 0) -> List[UserStats]:
+def resource_usage(
+    conn: BlitzGateway, minimum_days: int = 0, ignore_users: List[int] = []
+) -> List[UserStats]:
     # Note users' resource usage.
     # DiskUsage2.targetClasses remains too inefficient so iterate.
 
     user_stats = []
-    users, logouts = find_users(conn, minimum_days=minimum_days)
+    users, logouts = find_users(
+        conn, minimum_days=minimum_days, ignore_users=ignore_users
+    )
     for user_id, user_name in users.items():
         print(f'Finding disk usage of "{user_name}" (#{user_id}).')
         user = {"Experimenter": [user_id]}
         rsp = submit(conn, DiskUsage2(targetObjects=user), DiskUsage2Response)
 
         file_count = 0
         file_size = 0
@@ -273,24 +348,23 @@
     # Perform data deletion.
     stats = resource_usage(conn, minimum_days=minimum_days)
     users = choose_users(excess_file_count, excess_file_size, stats)
     print(f"Found {len(users)} user(s) for deletion.")
     for user in users:
         print(
             'Deleting {} GB of data belonging to "{}" (#{}).'.format(
-                user.size / 1000 ** 3,
+                user.size / 1000**3,
                 user.name,
                 user.id,
             )
         )
         delete_data(conn, user.id, dry_run=dry_run)
 
 
 def main() -> None:
-
     with omero.cli.cli_login() as cli:
         conn = omero.gateway.BlitzGateway(client_obj=cli.get_client())
         try:
             perform_delete(conn)
         except KeyboardInterrupt:
             pass  # ignore
         finally:
```

