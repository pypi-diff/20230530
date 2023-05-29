# Comparing `tmp/honeybee-idaice-0.2.2.tar.gz` & `tmp/honeybee-idaice-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.2.2.tar", last modified: Mon May 29 12:34:36 2023, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.3.0.tar", last modified: Mon May 29 23:33:41 2023, max compression
```

## Comparing `honeybee-idaice-0.2.2.tar` & `honeybee-idaice-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:34:36.000000 honeybee-idaice-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 12:34:36.000000 honeybee-idaice-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:34:36.000000 honeybee-idaice-0.2.2/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:34:36.000000 honeybee-idaice-0.2.2/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/geometry_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:34:36.000000 honeybee-idaice-0.2.2/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20423 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:34:36.000000 honeybee-idaice-0.2.2/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 12:34:36.000000 honeybee-idaice-0.2.2/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-29 12:34:36.000000 honeybee-idaice-0.2.2/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:34:36.000000 honeybee-idaice-0.2.2/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 12:34:36.000000 honeybee-idaice-0.2.2/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 12:34:36.000000 honeybee-idaice-0.2.2/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 12:34:36.000000 honeybee-idaice-0.2.2/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-29 12:34:36.000000 honeybee-idaice-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-29 12:33:20.000000 honeybee-idaice-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/geometry_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20423 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20537 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-29 23:33:41.000000 honeybee-idaice-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-29 23:32:31.000000 honeybee-idaice-0.3.0/setup.py
```

### Comparing `honeybee-idaice-0.2.2/LICENSE` & `honeybee-idaice-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.2/PKG-INFO` & `honeybee-idaice-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.2.2
+Version: 0.3.0
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Honeybee -> IDA-ICE
 
 A honeybee extension to convert HBJSON files to [IDA ICE](https://www.equa.se/en/ida-ice) `idm` files.
 
-![image](https://github.com/ladybug-tools/honeybee-idaice/assets/2915573/1ea06398-0d00-43ef-a350-1c3cbeacf9a9)
+![image](https://github.com/ladybug-tools/honeybee-idaice/assets/2915573/12840ca3-a94f-4c68-9251-e8eb393bc048)
 
 Two comments on how the model should be prepared.
 
 1. IDA ICE expects the model to be exported at the finish line of the one - and not the center of the wall.
 1. IDA ICE intersects the faces automatically. Do not intersect the faces in HBJSON files.
 
 The exporter only exports the geometry. None of the energy or Radiance properties are exported.
```

### Comparing `honeybee-idaice-0.2.2/README.md` & `honeybee-idaice-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Honeybee -> IDA-ICE
 
 A honeybee extension to convert HBJSON files to [IDA ICE](https://www.equa.se/en/ida-ice) `idm` files.
 
-![image](https://github.com/ladybug-tools/honeybee-idaice/assets/2915573/1ea06398-0d00-43ef-a350-1c3cbeacf9a9)
+![image](https://github.com/ladybug-tools/honeybee-idaice/assets/2915573/12840ca3-a94f-4c68-9251-e8eb393bc048)
 
 Two comments on how the model should be prepared.
 
 1. IDA ICE expects the model to be exported at the finish line of the one - and not the center of the wall.
 1. IDA ICE intersects the faces automatically. Do not intersect the faces in HBJSON files.
 
 The exporter only exports the geometry. None of the energy or Radiance properties are exported.
```

### Comparing `honeybee-idaice-0.2.2/honeybee_idaice/archive.py` & `honeybee-idaice-0.3.0/honeybee_idaice/archive.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.2/honeybee_idaice/cli/translate.py` & `honeybee-idaice-0.3.0/honeybee_idaice/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.2/honeybee_idaice/geometry_utils.py` & `honeybee-idaice-0.3.0/honeybee_idaice/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.2/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.3.0/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.2/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.3.0/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.2/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.3.0/honeybee_idaice/templates/building.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.2/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.3.0/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.2/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.3.0/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.2/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.3.0/honeybee_idaice/templates/room.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.2/honeybee_idaice/writer.py` & `honeybee-idaice-0.3.0/honeybee_idaice/writer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,148 @@
 """Write an idm file from a HBJSON file."""
 import pathlib
 import shutil
 import math
 from typing import List, Union
 
-from honeybee.model import Model, Room, Face, Aperture, Door
+from honeybee.model import Model, Room, Face, Aperture, Door, Shade
 from honeybee.facetype import RoofCeiling, Wall, Floor
-from ladybug_geometry.geometry3d import Point3D, Vector3D, Plane, Face3D
+from ladybug_geometry.geometry3d import Point3D, Vector3D, Plane, Face3D, Polyface3D, \
+    Mesh3D
 from ladybug_geometry.bounding import bounding_box
 
 from .archive import create_idm
 from .geometry_utils import get_floor_boundary, get_ceiling_boundary
 
 
+def _vertices_to_idm(vertices: List[Point3D]) -> str:
+    """Get a string for vertices in IDM format."""
+    vertices = ' '.join(f'({v.x} {v.y} {v.z})' for v in vertices)
+    return vertices
+
+
+def _shade_geometry_to_idm(geometry: Union[Face3D, Polyface3D], name: str):
+    """Create an IDM shade block from a Ladybug geometry.
+
+    Here is an exampel:
+
+        ((AGGREGATE :N "shade1" :T PICT3D)
+            (:PAR :N FILE :V "")
+            (:PAR :N POS :V #(0 0 0.0))
+            (:PAR :N SHADOWING :V :TRUE)
+            ((AGGREGATE :N "geom1" :T GEOM3D)
+            (:PAR :N NPOINTS :V 4)
+            (:PAR :N POINTS :DIM (4 3) :V #2A((-0.874454021453857 -0.59070497751236 -0.941487014293671) (1.0536140203476 -0.0591499991714954 -0.941487014293671) (-1.0536140203476 0.0591499991714954 0.941487014293671) (0.874454021453857 0.59070497751236 0.941487014293671)))
+            (:PAR :N CELLTYPE :V 1)
+            (:PAR :N NCELLS :V 2)
+            (:PAR :N NVERTICES :DIM (2) :V #(3 3))
+            (:PAR :N TOTNVERTS :V 6)
+            (:PAR :N VERTICES :DIM (6) :V #(0 1 2 2 1 3))
+        (:PAR :N PROPERTY :V #(1.0 1.0 1.0 0.699999988079071 1.0 1.0 1.0 0.5 1.0 1.0 1.0 0.0 1.0 1.0 1.0 0.0 0.0))))
+    """
+
+    if isinstance(geometry, Face3D):
+        mesh_3d = geometry.triangulated_mesh3d
+    else:
+        # it is a Polyface3D
+        meshes = [face.triangulated_mesh3d for face in geometry.faces]
+        mesh_3d = Mesh3D.join_meshes(meshes=meshes)
+
+    vertices = mesh_3d.vertices
+    faces = mesh_3d.faces
+    vertices_count = len(vertices)
+    face_count = len(faces)
+    face_length = [len(face) for face in faces]
+    total_vertices = sum(face_length)
+    faces_count = ' '.join(str(f) for f in face_length)
+    joined_faces = ' '.join(' '.join(str(f) for f in ff) for ff in faces)
+
+    shade = f' ((AGGREGATE :N "{name}" :T PICT3D)\n' \
+        '  (:PAR :N FILE :V "")\n' \
+        '  (:PAR :N SHADOWING :V :TRUE)\n' \
+        '  ((AGGREGATE :N "geom1" :T GEOM3D)\n' \
+        f'   (:PAR :N NPOINTS :V {vertices_count})\n' \
+        f'   (:PAR :N POINTS :DIM ({vertices_count} 3) :V #2A({_vertices_to_idm(vertices)}))\n' \
+        '   (:PAR :N CELLTYPE :V 1)\n' \
+        f'   (:PAR :N NCELLS :V {face_count})\n' \
+        f'   (:PAR :N NVERTICES :DIM ({face_count}) :V #({faces_count}))\n' \
+        f'   (:PAR :N TOTNVERTS :V {total_vertices})\n' \
+        f'   (:PAR :N VERTICES :DIM ({total_vertices}) :V #({joined_faces}))\n' \
+        '   (:PAR :N PROPERTY :V #(1.0 1.0 1.0 0.699999988079071 1.0 1.0 1.0 0.5 1.0 1.0 1.0 0.0 1.0 1.0 1.0 0.0 0.0))))'
+
+    return shade
+
+
+def _shade_group_to_idm(shades: List[Shade]) -> str:
+    """Convert a group of shades into a IDM string.
+
+    The files in the shade group should create a closed volume. The translator uses
+    the name of the first shade as the name of the group.
+    """
+    group_geometry = Polyface3D.from_faces(
+        [shade.geometry for shade in shades], tolerance=0.001
+    )
+    shade = shades[0]
+    # remove new lines from the name
+    name = '_'.join(
+        (' '.join(shade.display_name.split()), shade.identifier.replace('Shade_', ''))
+    )
+    return _shade_geometry_to_idm(group_geometry, name)
+
+
+def _shade_to_idm(shade: Shade):
+    shade_geo = shade.geometry
+    name = '_'.join(
+        (' '.join(shade.display_name.split()), shade.identifier.replace('Shade_', ''))
+    )
+    return _shade_geometry_to_idm(shade_geo, name)
+
+
+def shades_to_idm(shades: List[Shade]):
+    """Convert a list of Shades to a IDM string.
+
+    Args:
+        shades: A list of Shade faces.
+
+    Returns:
+        A formatted string that represents this shade in IDM format.
+
+    """
+    if not shades:
+        return ''
+
+    shade_groups = {}
+    no_groups = []
+    for shade in shades:
+        try:
+            group_id = shade.user_data['__group_id__']
+        except (TypeError, KeyError):
+            no_groups.append(shade)
+            continue
+        else:
+            if group_id not in shade_groups:
+                shade_groups[group_id] = [shade]
+            else:
+                shade_groups[group_id].append(shade)
+
+    filtered_groups = {}
+    for k, v in shade_groups.items():
+        if len(v) == 1:
+            no_groups.extend(v)
+        else:
+            filtered_groups[k] = v
+
+    single_shades = '\n'.join([_shade_to_idm(shade) for shade in no_groups])
+    group_shades = '\n'.join(
+        [_shade_group_to_idm(shades) for shades in filtered_groups.values()]
+        )
+
+    return f'((AGGREGATE :N ARCDATA)\n{single_shades}\n{group_shades})'
+
+
 def opening_to_idm(opening: Union[Aperture, Door], is_aperture=True) -> str:
     """Translate a HBJSON aperture to an IDM Window."""
     # name = opening.display_name
     name = opening.identifier
 
     # IDA-ICE looks to apertures from inside the room
     parent: Face3D = opening.parent.geometry.flip()
@@ -336,15 +462,16 @@
         '  (:PAR :N CORNERS :DIM (0 3) :V #2A()))))\n'
 
     sections.append(footer)
 
     return ''.join(sections) + '\n'
 
 
-def model_to_idm(model: Model, out_folder: pathlib.Path, name: str = None):
+def model_to_idm(model: Model, out_folder: pathlib.Path, name: str = None,
+                 debug: bool = True):
     """Translate a Honeybee model to an IDM file."""
     model.convert_to_units(units='Meters')
     __here__ = pathlib.Path(__file__).parent
     templates_folder = __here__.joinpath('templates')
     bldg_name = name or model.display_name
     base_folder = pathlib.Path(out_folder)
     model_folder = base_folder.joinpath(bldg_name)
@@ -387,15 +514,19 @@
                                 door.user_data = {'ignore': True}
                                 break
                         door_tracker.append(center)
 
         # add rooms as zones
         for room in model.rooms:
             bldg.write(f'((CE-ZONE :N "{room.display_name}" :T ZONE))\n')
-        bldg.write(f';[end of {bldg_name}.idm]\n')
+
+        # collect all the shades from room
+        shades_idm = shades_to_idm(model.shades)
+        bldg.write(shades_idm)
+        bldg.write(f'\n;[end of {bldg_name}.idm]\n')
 
     # copy template files
     templates = ['plant.idm', 'ahu.idc', 'ahu.idm', 'plant.idc']
     for template_file in templates:
         target_file = bldg_folder.joinpath(template_file)
         shutil.copy(templates_folder.joinpath(template_file), target_file)
         with target_file.open('a') as outf:
@@ -412,11 +543,12 @@
             rm.write(geometry)
             footer = f'\n;[end of {bldg_name}\\{room_name}.idm]\n'
             rm.write(footer)
 
     idm_file = base_folder.joinpath(f'{bldg_name}.idm')
     create_idm(model_folder, idm_file)
 
-    # clean up the folder - leave it for now for debugging purposes
-    # shutil.rmtree(model_folder)
+    # clean up the folder
+    if not debug:
+        shutil.rmtree(model_folder)
 
     return idm_file
```

### Comparing `honeybee-idaice-0.2.2/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.3.0/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.2/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.3.0/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.2.2
+Version: 0.3.0
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Honeybee -> IDA-ICE
 
 A honeybee extension to convert HBJSON files to [IDA ICE](https://www.equa.se/en/ida-ice) `idm` files.
 
-![image](https://github.com/ladybug-tools/honeybee-idaice/assets/2915573/1ea06398-0d00-43ef-a350-1c3cbeacf9a9)
+![image](https://github.com/ladybug-tools/honeybee-idaice/assets/2915573/12840ca3-a94f-4c68-9251-e8eb393bc048)
 
 Two comments on how the model should be prepared.
 
 1. IDA ICE expects the model to be exported at the finish line of the one - and not the center of the wall.
 1. IDA ICE intersects the faces automatically. Do not intersect the faces in HBJSON files.
 
 The exporter only exports the geometry. None of the energy or Radiance properties are exported.
```

### Comparing `honeybee-idaice-0.2.2/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.3.0/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.2/setup.py` & `honeybee-idaice-0.3.0/setup.py`

 * *Files identical despite different names*

