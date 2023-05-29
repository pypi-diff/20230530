# Comparing `tmp/django_linear_migrations-2.7.0.tar.gz` & `tmp/django_linear_migrations-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_linear_migrations-2.7.0.tar", last modified: Sat Feb 25 07:21:44 2023, max compression
+gzip compressed data, was "django_linear_migrations-2.8.0.tar", last modified: Mon May 29 23:07:23 2023, max compression
```

## Comparing `django_linear_migrations-2.7.0.tar` & `django_linear_migrations-2.8.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:21:44.760192 django_linear_migrations-2.7.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4126 2023-02-25 07:21:42.000000 django_linear_migrations-2.7.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:58:38.000000 django_linear_migrations-2.7.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:09:56.000000 django_linear_migrations-2.7.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)    13678 2023-02-25 07:21:44.760273 django_linear_migrations-2.7.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)    12277 2023-01-20 11:36:46.000000 django_linear_migrations-2.7.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      460 2023-02-15 21:55:44.000000 django_linear_migrations-2.7.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1678 2023-02-25 07:21:44.760604 django_linear_migrations-2.7.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:21:44.751142 django_linear_migrations-2.7.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:21:44.757201 django_linear_migrations-2.7.0/src/django_linear_migrations/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.7.0/src/django_linear_migrations/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8448 2023-01-17 08:57:33.000000 django_linear_migrations-2.7.0/src/django_linear_migrations/apps.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    25637 2023-02-07 15:19:23.000000 django_linear_migrations-2.7.0/src/django_linear_migrations/compat.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:21:44.758174 django_linear_migrations-2.7.0/src/django_linear_migrations/management/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.7.0/src/django_linear_migrations/management/__init__.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:21:44.758899 django_linear_migrations-2.7.0/src/django_linear_migrations/management/commands/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.7.0/src/django_linear_migrations/management/commands/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3239 2023-01-03 10:31:33.000000 django_linear_migrations-2.7.0/src/django_linear_migrations/management/commands/create_max_migration_files.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1084 2022-11-04 10:44:50.000000 django_linear_migrations-2.7.0/src/django_linear_migrations/management/commands/makemigrations.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7914 2022-11-04 10:44:50.000000 django_linear_migrations-2.7.0/src/django_linear_migrations/management/commands/rebase_migration.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.7.0/src/django_linear_migrations/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:21:44.758051 django_linear_migrations-2.7.0/src/django_linear_migrations.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    13678 2023-02-25 07:21:44.000000 django_linear_migrations-2.7.0/src/django_linear_migrations.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1003 2023-02-25 07:21:44.000000 django_linear_migrations-2.7.0/src/django_linear_migrations.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:21:44.000000 django_linear_migrations-2.7.0/src/django_linear_migrations.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:21:44.000000 django_linear_migrations-2.7.0/src/django_linear_migrations.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-02-25 07:21:44.000000 django_linear_migrations-2.7.0/src/django_linear_migrations.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       25 2023-02-25 07:21:44.000000 django_linear_migrations-2.7.0/src/django_linear_migrations.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:21:44.760012 django_linear_migrations-2.7.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1094 2022-06-03 11:58:39.000000 django_linear_migrations-2.7.0/tests/test_apps.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5495 2023-01-03 10:31:33.000000 django_linear_migrations-2.7.0/tests/test_checks.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7207 2023-01-03 10:31:33.000000 django_linear_migrations-2.7.0/tests/test_create_max_migration_files.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2799 2022-11-04 10:44:50.000000 django_linear_migrations-2.7.0/tests/test_makemigrations.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)    16492 2023-01-03 10:31:33.000000 django_linear_migrations-2.7.0/tests/test_rebase_migration.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.116070 django_linear_migrations-2.8.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4384 2023-05-29 23:07:19.000000 django_linear_migrations-2.8.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2022-06-03 11:58:38.000000 django_linear_migrations-2.8.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:09:56.000000 django_linear_migrations-2.8.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    13835 2023-05-29 23:07:23.116186 django_linear_migrations-2.8.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    12434 2023-05-29 23:04:19.000000 django_linear_migrations-2.8.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      500 2023-02-28 09:05:50.000000 django_linear_migrations-2.8.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1678 2023-05-29 23:07:23.116783 django_linear_migrations-2.8.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.105797 django_linear_migrations-2.8.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.113160 django_linear_migrations-2.8.0/src/django_linear_migrations/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8487 2023-02-27 20:47:44.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/apps.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    25637 2023-02-07 15:19:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/compat.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.114213 django_linear_migrations-2.8.0/src/django_linear_migrations/management/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/management/__init__.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.115052 django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3239 2023-01-03 10:31:33.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/create_max_migration_files.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1084 2022-11-04 10:44:50.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/makemigrations.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8652 2023-05-29 23:04:19.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/rebase_migration.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:39.000000 django_linear_migrations-2.8.0/src/django_linear_migrations/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.114064 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    13835 2023-05-29 23:07:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1003 2023-05-29 23:07:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-29 23:07:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-29 23:07:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-05-29 23:07:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       25 2023-05-29 23:07:23.000000 django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-29 23:07:23.115882 django_linear_migrations-2.8.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1094 2022-06-03 11:58:39.000000 django_linear_migrations-2.8.0/tests/test_apps.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5495 2023-01-03 10:31:33.000000 django_linear_migrations-2.8.0/tests/test_checks.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7207 2023-01-03 10:31:33.000000 django_linear_migrations-2.8.0/tests/test_create_max_migration_files.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2799 2022-11-04 10:44:50.000000 django_linear_migrations-2.8.0/tests/test_makemigrations.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    19076 2023-05-29 23:04:19.000000 django_linear_migrations-2.8.0/tests/test_rebase_migration.py
```

### Comparing `django_linear_migrations-2.7.0/CHANGELOG.rst` & `django_linear_migrations-2.8.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+2.8.0 (2023-05-30)
+------------------
+
+* Extend ``rebase_migration`` to detect Git in-progress merges and select the correct migration to rebase.
+
+  Thanks to Dmitry Sleptsov in `PR #260 <https://github.com/adamchainz/django-linear-migrations/pull/260>`__.
+
 2.7.0 (2023-02-25)
 ------------------
 
 * Support Django 4.2.
 
 2.6.0 (2023-01-03)
 ------------------
```

### Comparing `django_linear_migrations-2.7.0/LICENSE` & `django_linear_migrations-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.7.0/PKG-INFO` & `django_linear_migrations-2.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_linear_migrations
-Version: 2.7.0
+Version: 2.8.0
 Summary: Ensure your migrations are linear.
 Home-page: https://github.com/adamchainz/django-linear-migrations
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-linear-migrations/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -179,22 +179,28 @@
 This management command can help you fix migration conflicts.
 Following a conflicted “rebase” operation in Git, run it with the name of the app to auto-fix the migrations for:
 
 .. code-block:: console
 
     $ python manage.py rebase_migration <app_label>
 
-The command will use the conflict information in the ``max_migration.txt`` file to determine which migration to rebase.
-It will then rename the migration, edit it to depend on the new migration in your main branch, and update ``max_migration.txt``.
-If Black is installed, it will format the updated migration file with it, like Django’s built-in migration commands (from version 4.1+).
+The command uses the conflict information in the ``max_migration.txt`` file to determine which migration to rebase.
+It automatically detects whether a Git merge or rebase operation is in progress, assuming rebase if a Git repository cannot be found.
+The command then:
+
+1. renames the migration
+2. edits it to depend on the new migration from your main branch
+3. updates ``max_migration.txt``.
+
+If Black is installed, the command formats the updated migration file with it, like Django’s built-in migration commands do (from version 4.1+).
 See below for some examples and caveats.
 
 Note rebasing the migration might not always be the *correct* thing to do.
-If the migrations in main and feature branches have both affected the same models, rebasing the migration to the end may not make sense.
-However, such parallel changes would *normally* cause conflicts in your models files or other parts of the source code as well.
+If the migrations in your main and feature branches have both affected the same models, rebasing the migration to the end may not make sense.
+However, such parallel changes would *normally* cause conflicts in your model files or other parts of the source code as well.
 
 Worked Example
 ^^^^^^^^^^^^^^
 
 Imagine you were working on your project's ``books`` app in a feature branch called ``titles`` and created a migration called ``0002_longer_titles``.
 Meanwhile a commit has been merged to your ``main`` branch with a *different* 2nd migration for ``books`` called ``0002_author_nicknames``.
 Thanks to django-linear-migrations, the ``max_migration.txt`` file will show as conflicted between your feature and main branches.
```

### Comparing `django_linear_migrations-2.7.0/README.rst` & `django_linear_migrations-2.8.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -145,22 +145,28 @@
 This management command can help you fix migration conflicts.
 Following a conflicted “rebase” operation in Git, run it with the name of the app to auto-fix the migrations for:
 
 .. code-block:: console
 
     $ python manage.py rebase_migration <app_label>
 
-The command will use the conflict information in the ``max_migration.txt`` file to determine which migration to rebase.
-It will then rename the migration, edit it to depend on the new migration in your main branch, and update ``max_migration.txt``.
-If Black is installed, it will format the updated migration file with it, like Django’s built-in migration commands (from version 4.1+).
+The command uses the conflict information in the ``max_migration.txt`` file to determine which migration to rebase.
+It automatically detects whether a Git merge or rebase operation is in progress, assuming rebase if a Git repository cannot be found.
+The command then:
+
+1. renames the migration
+2. edits it to depend on the new migration from your main branch
+3. updates ``max_migration.txt``.
+
+If Black is installed, the command formats the updated migration file with it, like Django’s built-in migration commands do (from version 4.1+).
 See below for some examples and caveats.
 
 Note rebasing the migration might not always be the *correct* thing to do.
-If the migrations in main and feature branches have both affected the same models, rebasing the migration to the end may not make sense.
-However, such parallel changes would *normally* cause conflicts in your models files or other parts of the source code as well.
+If the migrations in your main and feature branches have both affected the same models, rebasing the migration to the end may not make sense.
+However, such parallel changes would *normally* cause conflicts in your model files or other parts of the source code as well.
 
 Worked Example
 ^^^^^^^^^^^^^^
 
 Imagine you were working on your project's ``books`` app in a feature branch called ``titles`` and created a migration called ``0002_longer_titles``.
 Meanwhile a commit has been merged to your ``main`` branch with a *different* 2nd migration for ``books`` called ``0002_author_nicknames``.
 Thanks to django-linear-migrations, the ``max_migration.txt`` file will show as conflicted between your feature and main branches.
```

### Comparing `django_linear_migrations-2.7.0/setup.cfg` & `django_linear_migrations-2.8.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_linear_migrations
-version = 2.7.0
+version = 2.8.0
 description = Ensure your migrations are linear.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/django-linear-migrations
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
```

### Comparing `django_linear_migrations-2.7.0/src/django_linear_migrations/apps.py` & `django_linear_migrations-2.8.0/src/django_linear_migrations/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,16 @@
             Error(
                 id="dlm.E005",
                 msg=(
                     "Conflicting migrations detected - multiple leaf nodes "
                     + f"detected for these apps:{conflict_msg}"
                 ),
                 hint=(
-                    "Fix the conflict, e.g. with './manage.py makemigrations --merge'."
+                    "Fix the conflict, e.g. with "
+                    + "'./manage.py makemigrations --merge --skip-checks'."
                 ),
             )
         )
         return errors
 
     graph_plan = get_graph_plan(loader=migration_loader, app_labels=app_labels)
     for app_config in first_party_app_configs():
```

### Comparing `django_linear_migrations-2.7.0/src/django_linear_migrations/compat.py` & `django_linear_migrations-2.8.0/src/django_linear_migrations/compat.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.7.0/src/django_linear_migrations/management/commands/create_max_migration_files.py` & `django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/create_max_migration_files.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.7.0/src/django_linear_migrations/management/commands/makemigrations.py` & `django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/makemigrations.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.7.0/src/django_linear_migrations/management/commands/rebase_migration.py` & `django_linear_migrations-2.8.0/src/django_linear_migrations/management/commands/rebase_migration.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,15 +180,37 @@
     lines = max_migration_lines
     if len(lines) <= 1:
         return None
     if not lines[0].startswith("<<<<<<<"):
         return None
     if not lines[-1].startswith(">>>>>>>"):
         return None
-    return lines[1].strip(), lines[-2].strip()
+    migration_names = (lines[1].strip(), lines[-2].strip())
+    if is_merge_in_progress():
+        # During the merge 'ours' and 'theirs' are swapped in comparison with rebase
+        migration_names = (migration_names[1], migration_names[0])
+    return migration_names
+
+
+def is_merge_in_progress() -> bool:
+    try:
+        subprocess.run(
+            ["git", "rev-parse", "--verify", "MERGE_HEAD"],
+            capture_output=True,
+            check=True,
+            text=True,
+        )
+    except (FileNotFoundError, subprocess.SubprocessError):
+        # Either:
+        # - `git` is not available, or broken
+        # - there is no git repository
+        # - no merge head exists, so assume rebasing
+        return False
+    # Merged head exists, we are merging
+    return True
 
 
 def migration_applied(app_label: str, migration_name: str) -> bool:
     Migration = MigrationRecorder.Migration
     for alias in connections:
         try:
             if (
```

### Comparing `django_linear_migrations-2.7.0/src/django_linear_migrations.egg-info/PKG-INFO` & `django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-linear-migrations
-Version: 2.7.0
+Version: 2.8.0
 Summary: Ensure your migrations are linear.
 Home-page: https://github.com/adamchainz/django-linear-migrations
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-linear-migrations/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -179,22 +179,28 @@
 This management command can help you fix migration conflicts.
 Following a conflicted “rebase” operation in Git, run it with the name of the app to auto-fix the migrations for:
 
 .. code-block:: console
 
     $ python manage.py rebase_migration <app_label>
 
-The command will use the conflict information in the ``max_migration.txt`` file to determine which migration to rebase.
-It will then rename the migration, edit it to depend on the new migration in your main branch, and update ``max_migration.txt``.
-If Black is installed, it will format the updated migration file with it, like Django’s built-in migration commands (from version 4.1+).
+The command uses the conflict information in the ``max_migration.txt`` file to determine which migration to rebase.
+It automatically detects whether a Git merge or rebase operation is in progress, assuming rebase if a Git repository cannot be found.
+The command then:
+
+1. renames the migration
+2. edits it to depend on the new migration from your main branch
+3. updates ``max_migration.txt``.
+
+If Black is installed, the command formats the updated migration file with it, like Django’s built-in migration commands do (from version 4.1+).
 See below for some examples and caveats.
 
 Note rebasing the migration might not always be the *correct* thing to do.
-If the migrations in main and feature branches have both affected the same models, rebasing the migration to the end may not make sense.
-However, such parallel changes would *normally* cause conflicts in your models files or other parts of the source code as well.
+If the migrations in your main and feature branches have both affected the same models, rebasing the migration to the end may not make sense.
+However, such parallel changes would *normally* cause conflicts in your model files or other parts of the source code as well.
 
 Worked Example
 ^^^^^^^^^^^^^^
 
 Imagine you were working on your project's ``books`` app in a feature branch called ``titles`` and created a migration called ``0002_longer_titles``.
 Meanwhile a commit has been merged to your ``main`` branch with a *different* 2nd migration for ``books`` called ``0002_author_nicknames``.
 Thanks to django-linear-migrations, the ``max_migration.txt`` file will show as conflicted between your feature and main branches.
```

### Comparing `django_linear_migrations-2.7.0/src/django_linear_migrations.egg-info/SOURCES.txt` & `django_linear_migrations-2.8.0/src/django_linear_migrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.7.0/tests/test_apps.py` & `django_linear_migrations-2.8.0/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.7.0/tests/test_checks.py` & `django_linear_migrations-2.8.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.7.0/tests/test_create_max_migration_files.py` & `django_linear_migrations-2.8.0/tests/test_create_max_migration_files.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.7.0/tests/test_makemigrations.py` & `django_linear_migrations-2.8.0/tests/test_makemigrations.py`

 * *Files identical despite different names*

### Comparing `django_linear_migrations-2.7.0/tests/test_rebase_migration.py` & `django_linear_migrations-2.8.0/tests/test_rebase_migration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import os
+import subprocess
 import sys
 import time
 from functools import partial
 from textwrap import dedent
 from unittest import mock
 
 import pytest
@@ -434,40 +436,107 @@
         result = module.find_migration_names(["not_a_marker", "0002_author_nicknames"])
         assert result is None
 
     def test_none_when_no_second_marker(self):
         result = module.find_migration_names(["<<<<<<<", "0002_author_nicknames"])
         assert result is None
 
-    def test_works_with_two_way_merge(self):
+    def test_works_with_two_way_merge_during_rebase(self):
         result = module.find_migration_names(
             [
                 "<<<<<<<",
                 "0002_author_nicknames",
                 "=======",
                 "0002_longer_titles",
                 ">>>>>>>",
             ]
         )
         assert result == ("0002_author_nicknames", "0002_longer_titles")
 
-    def test_works_with_three_way_merge(self):
+    def test_works_with_three_way_merge_during_rebase(self):
         result = module.find_migration_names(
             [
                 "<<<<<<<",
                 "0002_author_nicknames",
                 "|||||||",
                 "0001_initial",
                 "=======",
                 "0002_longer_titles",
                 ">>>>>>>",
             ]
         )
         assert result == ("0002_author_nicknames", "0002_longer_titles")
 
+    def test_works_with_two_way_merge_during_merge(self):
+        with mock.patch.object(module, "is_merge_in_progress", return_value=True):
+            result = module.find_migration_names(
+                [
+                    "<<<<<<<",
+                    "0002_longer_titles",
+                    "=======",
+                    "0002_author_nicknames",
+                    ">>>>>>>",
+                ]
+            )
+        assert result == ("0002_author_nicknames", "0002_longer_titles")
+
+    def test_works_with_three_way_merge_during_merge(self):
+        with mock.patch.object(module, "is_merge_in_progress", return_value=True):
+            result = module.find_migration_names(
+                [
+                    "<<<<<<<",
+                    "0002_longer_titles",
+                    "|||||||",
+                    "0001_initial",
+                    "=======",
+                    "0002_author_nicknames",
+                    ">>>>>>>",
+                ]
+            )
+        assert result == ("0002_author_nicknames", "0002_longer_titles")
+
+
+class IsMergeInProgressTests(SimpleTestCase):
+    @pytest.fixture(autouse=True)
+    def tmp_path_fixture(self, tmp_path):
+        self.tmp_path = tmp_path
+        self.subprocess_run = partial(subprocess.run, cwd=tmp_path, check=True)
+
+    def setUp(self):
+        orig = os.getcwd()
+        os.chdir(self.tmp_path)
+        self.addCleanup(os.chdir, orig)
+
+    def test_no_git_command(self):
+        with mock.patch.dict(os.environ, {"PATH": ""}):
+            result = module.is_merge_in_progress()
+        assert result is False
+
+    def test_no_git_dir(self):
+        result = module.is_merge_in_progress()
+        assert result is False
+
+    def test_git_dir_no_merge(self):
+        self.subprocess_run(["git", "init"])
+        result = module.is_merge_in_progress()
+        assert result is False
+
+    def test_git_dir_merge(self):
+        self.subprocess_run(["git", "init", "-b", "main"])
+        self.subprocess_run(["git", "config", "user.email", "hacker@example.com"])
+        self.subprocess_run(["git", "config", "user.name", "A Hacker"])
+        self.subprocess_run(["git", "commit", "--allow-empty", "-m", "A"])
+        self.subprocess_run(["git", "switch", "--orphan", "other"])
+        self.subprocess_run(["git", "commit", "--allow-empty", "-m", "B"])
+        self.subprocess_run(
+            ["git", "merge", "--no-commit", "--allow-unrelated-histories", "main"]
+        )
+        result = module.is_merge_in_progress()
+        assert result is True
+
 
 class MigrationAppliedTests(TestCase):
     def test_table_does_not_exist(self):
         with connection.cursor() as cursor:
             cursor.execute("DROP TABLE django_migrations")
 
         result = module.migration_applied("testapp", "0001_initial")
```

