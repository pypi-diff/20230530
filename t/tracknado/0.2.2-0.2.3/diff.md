# Comparing `tmp/tracknado-0.2.2.tar.gz` & `tmp/tracknado-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracknado-0.2.2.tar", last modified: Sat May 27 19:24:33 2023, max compression
+gzip compressed data, was "tracknado-0.2.3.tar", last modified: Tue May 30 11:38:47 2023, max compression
```

## Comparing `tracknado-0.2.2.tar` & `tracknado-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:24:33.143016 tracknado-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:24:33.139016 tracknado-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:24:33.139016 tracknado-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-27 19:24:18.000000 tracknado-0.2.2/.github/workflows/python-publish.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-05-27 19:24:18.000000 tracknado-0.2.2/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-27 19:24:18.000000 tracknado-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-27 19:24:33.143016 tracknado-0.2.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2422 2023-05-27 19:24:18.000000 tracknado-0.2.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-05-27 19:24:18.000000 tracknado-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 19:24:33.143016 tracknado-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-27 19:24:18.000000 tracknado-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:24:33.143016 tracknado-0.2.2/tracknado/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-27 19:24:32.000000 tracknado-0.2.2/tracknado/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:24:33.143016 tracknado-0.2.2/tracknado/old/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3967 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/old/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6644 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/old/grouping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/old/hub_setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6442 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/old/make_hub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2356 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/old/track.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-05-27 19:24:18.000000 tracknado-0.2.2/tracknado/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:24:33.143016 tracknado-0.2.2/tracknado.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-27 19:24:33.000000 tracknado-0.2.2/tracknado.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-27 19:24:33.000000 tracknado-0.2.2/tracknado.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 19:24:33.000000 tracknado-0.2.2/tracknado.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 19:24:33.000000 tracknado-0.2.2/tracknado.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-27 19:24:33.000000 tracknado-0.2.2/tracknado.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 19:24:33.000000 tracknado-0.2.2/tracknado.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:38:47.396930 tracknado-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:38:47.392930 tracknado-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:38:47.392930 tracknado-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-30 11:38:30.000000 tracknado-0.2.3/.github/workflows/python-publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-05-30 11:38:30.000000 tracknado-0.2.3/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-30 11:38:30.000000 tracknado-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-30 11:38:47.396930 tracknado-0.2.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2422 2023-05-30 11:38:30.000000 tracknado-0.2.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-05-30 11:38:30.000000 tracknado-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:38:47.396930 tracknado-0.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-30 11:38:30.000000 tracknado-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:38:47.392930 tracknado-0.2.3/tracknado/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-30 11:38:30.000000 tracknado-0.2.3/tracknado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 11:38:47.000000 tracknado-0.2.3/tracknado/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28734 2023-05-30 11:38:30.000000 tracknado-0.2.3/tracknado/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-05-30 11:38:30.000000 tracknado-0.2.3/tracknado/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:38:47.396930 tracknado-0.2.3/tracknado/old/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3967 2023-05-30 11:38:30.000000 tracknado-0.2.3/tracknado/old/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6644 2023-05-30 11:38:30.000000 tracknado-0.2.3/tracknado/old/grouping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-05-30 11:38:30.000000 tracknado-0.2.3/tracknado/old/hub_setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6442 2023-05-30 11:38:30.000000 tracknado-0.2.3/tracknado/old/make_hub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2356 2023-05-30 11:38:30.000000 tracknado-0.2.3/tracknado/old/track.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-05-30 11:38:30.000000 tracknado-0.2.3/tracknado/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:38:47.396930 tracknado-0.2.3/tracknado.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-30 11:38:47.000000 tracknado-0.2.3/tracknado.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-30 11:38:47.000000 tracknado-0.2.3/tracknado.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:38:47.000000 tracknado-0.2.3/tracknado.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 11:38:47.000000 tracknado-0.2.3/tracknado.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 11:38:47.000000 tracknado-0.2.3/tracknado.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 11:38:47.000000 tracknado-0.2.3/tracknado.egg-info/top_level.txt
```

### Comparing `tracknado-0.2.2/.github/workflows/python-publish.yml` & `tracknado-0.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.2/LICENSE` & `tracknado-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.2/PKG-INFO` & `tracknado-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracknado
-Version: 0.2.2
+Version: 0.2.3
 Summary: CLI library to generate UCSC trackhubs from sequencing data
 Author-email: Alastair Smith <alastair.smith@ndcls.ox.ac.uk>
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tracknado-0.2.2/README.md` & `tracknado-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.2/pyproject.toml` & `tracknado-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.2/tracknado/api.py` & `tracknado-0.2.3/tracknado/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,15 +364,15 @@
 
         if self._supertrack_columns:
             assert all(
                 [c in self.details.columns for c in self._supertrack_columns]
             ), f"SuperTrack columns {self._supertrack_columns} missing"
 
             supertracks = dict()
-            for grouping, df in self.details.groupby(self._supertrack_columns):
+            for grouping, df in self.details.reset_index(drop=True).groupby(self._supertrack_columns, as_index=False):
                 
 
                 if isinstance(grouping, str):
                     track_id = (grouping,)
                 elif len(grouping) == 1:
                     track_id = grouping
                 else:
@@ -488,22 +488,26 @@
             if "supertrack" in self.details.columns:
 
                 for (supertrack, overlay) , df in self.details.groupby(
                     ["supertrack", *self._overlay_columns]
                 ):
                     
                     supertrack_name = self.super_tracks[supertrack].name
-                    overlay_name = "_".join([supertrack_name, *overlay]) + "_overlay"
+
+                    if isinstance(overlay, str):
+                        overlay_name = "_".join([supertrack_name, overlay]) + "_overlay"
+                    else:
+                        overlay_name = "_".join([supertrack_name, *overlay]) + "_overlay"
 
                     overlay_track = trackhub.AggregateTrack(
                         aggregate="transparentOverlay",
                         name=overlay_name,
                     )
 
-                    self.super_tracks[supertrack].add_tracks(overlay)
+                    self.super_tracks[supertrack].add_tracks(overlay_track)
                     overlay_tracks[get_hash(tuple([supertrack, overlay]))] = overlay_track
 
             else:
                 for overlay, df in self.details.groupby(self._overlay_columns):
 
                     overlay_name = "_".join(overlay) if isinstance(overlay, tuple) else overlay
                     overlay_id = tuple(overlay) if isinstance(overlay, tuple) else (overlay,)
```

### Comparing `tracknado-0.2.2/tracknado/cli.py` & `tracknado-0.2.3/tracknado/cli.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.2/tracknado/old/cli.py` & `tracknado-0.2.3/tracknado/old/cli.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.2/tracknado/old/grouping.py` & `tracknado-0.2.3/tracknado/old/grouping.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.2/tracknado/old/hub_setup.py` & `tracknado-0.2.3/tracknado/old/hub_setup.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.2/tracknado/old/make_hub.py` & `tracknado-0.2.3/tracknado/old/make_hub.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.2/tracknado/old/track.py` & `tracknado-0.2.3/tracknado/old/track.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.2/tracknado/utils.py` & `tracknado-0.2.3/tracknado/utils.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2.2/tracknado.egg-info/PKG-INFO` & `tracknado-0.2.3/tracknado.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracknado
-Version: 0.2.2
+Version: 0.2.3
 Summary: CLI library to generate UCSC trackhubs from sequencing data
 Author-email: Alastair Smith <alastair.smith@ndcls.ox.ac.uk>
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

