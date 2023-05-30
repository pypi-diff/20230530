# Comparing `tmp/gamelib-0.0.4.tar.gz` & `tmp/gamelib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamelib-0.0.4.tar", last modified: Thu Dec 15 17:46:25 2022, max compression
+gzip compressed data, was "gamelib-0.0.7.tar", last modified: Tue May 30 19:02:50 2023, max compression
```

## Comparing `gamelib-0.0.4.tar` & `gamelib-0.0.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2022-12-15 17:46:25.955736 gamelib-0.0.4/
--rw-------   0 peffjepin  (1000) peffjepin  (1000)    35149 2022-12-15 16:20:23.000000 gamelib-0.0.4/COPYING
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     2950 2022-12-15 17:46:25.955736 gamelib-0.0.4/PKG-INFO
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     2249 2022-12-15 16:20:23.000000 gamelib-0.0.4/README.md
-drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2022-12-15 17:46:25.952403 gamelib-0.0.4/gamelib/
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     1946 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/__init__.py
-drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2022-12-15 17:46:25.952403 gamelib-0.0.4/gamelib/core/
--rw-------   0 peffjepin  (1000) peffjepin  (1000)        0 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/core/__init__.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     7498 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/core/events.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     7486 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/core/gl.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)    22732 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/core/input.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     4879 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/core/resources.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     3438 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/core/runtime.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     4567 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/core/time.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     4732 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/core/vectors.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     9589 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/core/window.py
-drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2022-12-15 17:46:25.952403 gamelib-0.0.4/gamelib/ecs/
--rw-------   0 peffjepin  (1000) peffjepin  (1000)      118 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/ecs/__init__.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)    45958 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/ecs/base.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     1560 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/ecs/collisions.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     1801 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/ecs/transforms.py
-drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2022-12-15 17:46:25.952403 gamelib-0.0.4/gamelib/geometry/
--rw-------   0 peffjepin  (1000) peffjepin  (1000)      499 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/geometry/__init__.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     2155 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/geometry/base.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)    26405 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/geometry/collisions.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)      835 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/geometry/cube.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     1308 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/geometry/gridmesh.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)      342 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/geometry/loader.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)    16988 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/geometry/transforms.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     3043 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/geometry/wavefront.py
-drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2022-12-15 17:46:25.955736 gamelib-0.0.4/gamelib/rendering/
--rw-------   0 peffjepin  (1000) peffjepin  (1000)      136 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/rendering/__init__.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)      943 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/rendering/_global.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     6301 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/rendering/buffers.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)    18257 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/rendering/camera.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)    16329 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/rendering/gpu.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)    30301 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/rendering/shaders.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)    13034 2022-12-15 17:28:19.000000 gamelib-0.0.4/gamelib/rendering/textures.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     1372 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/rendering/uniforms.py
-drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2022-12-15 17:46:25.955736 gamelib-0.0.4/gamelib/utils/
--rw-------   0 peffjepin  (1000) peffjepin  (1000)       85 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/utils/__init__.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     1658 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/utils/ensure.py
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     4318 2022-12-15 16:20:23.000000 gamelib-0.0.4/gamelib/utils/mark.py
-drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2022-12-15 17:46:25.952403 gamelib-0.0.4/gamelib.egg-info/
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     2950 2022-12-15 17:46:25.000000 gamelib-0.0.4/gamelib.egg-info/PKG-INFO
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     1087 2022-12-15 17:46:25.000000 gamelib-0.0.4/gamelib.egg-info/SOURCES.txt
--rw-------   0 peffjepin  (1000) peffjepin  (1000)        1 2022-12-15 17:46:25.000000 gamelib-0.0.4/gamelib.egg-info/dependency_links.txt
--rw-------   0 peffjepin  (1000) peffjepin  (1000)        1 2022-12-15 16:20:35.000000 gamelib-0.0.4/gamelib.egg-info/not-zip-safe
--rw-------   0 peffjepin  (1000) peffjepin  (1000)      162 2022-12-15 17:46:25.000000 gamelib-0.0.4/gamelib.egg-info/requires.txt
--rw-------   0 peffjepin  (1000) peffjepin  (1000)        8 2022-12-15 17:46:25.000000 gamelib-0.0.4/gamelib.egg-info/top_level.txt
--rw-------   0 peffjepin  (1000) peffjepin  (1000)      209 2022-12-15 16:20:23.000000 gamelib-0.0.4/pyproject.toml
--rw-------   0 peffjepin  (1000) peffjepin  (1000)     1050 2022-12-15 17:46:25.955736 gamelib-0.0.4/setup.cfg
--rw-------   0 peffjepin  (1000) peffjepin  (1000)       69 2022-12-15 16:20:23.000000 gamelib-0.0.4/setup.py
+drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2023-05-30 19:02:50.582293 gamelib-0.0.7/
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)    35149 2022-12-15 16:20:23.000000 gamelib-0.0.7/COPYING
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     2950 2023-05-30 19:02:50.582293 gamelib-0.0.7/PKG-INFO
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     2249 2022-12-15 16:20:23.000000 gamelib-0.0.7/README.md
+drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2023-05-30 19:02:50.578960 gamelib-0.0.7/gamelib/
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     1946 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/__init__.py
+drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2023-05-30 19:02:50.578960 gamelib-0.0.7/gamelib/core/
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)        0 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/core/__init__.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     7498 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/core/events.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     7457 2023-05-30 18:35:42.000000 gamelib-0.0.7/gamelib/core/gl.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)    22732 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/core/input.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     4879 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/core/resources.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     3438 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/core/runtime.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     4567 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/core/time.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     4732 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/core/vectors.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     9589 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/core/window.py
+drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2023-05-30 19:02:50.582293 gamelib-0.0.7/gamelib/ecs/
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)      118 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/ecs/__init__.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)    45958 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/ecs/base.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     1560 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/ecs/collisions.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     1801 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/ecs/transforms.py
+drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2023-05-30 19:02:50.582293 gamelib-0.0.7/gamelib/geometry/
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)      499 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/geometry/__init__.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     2155 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/geometry/base.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)    26405 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/geometry/collisions.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)      835 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/geometry/cube.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     1308 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/geometry/gridmesh.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)      342 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/geometry/loader.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)    16988 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/geometry/transforms.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     3043 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/geometry/wavefront.py
+drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2023-05-30 19:02:50.582293 gamelib-0.0.7/gamelib/rendering/
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)      136 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/rendering/__init__.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)      943 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/rendering/_global.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     6301 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/rendering/buffers.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)    18257 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/rendering/camera.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)    16329 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/rendering/gpu.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)    30301 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/rendering/shaders.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)    13034 2022-12-15 17:28:19.000000 gamelib-0.0.7/gamelib/rendering/textures.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     1372 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/rendering/uniforms.py
+drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2023-05-30 19:02:50.582293 gamelib-0.0.7/gamelib/utils/
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)       85 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/utils/__init__.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     1658 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/utils/ensure.py
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     4318 2022-12-15 16:20:23.000000 gamelib-0.0.7/gamelib/utils/mark.py
+drwx------   0 peffjepin  (1000) peffjepin  (1000)        0 2023-05-30 19:02:50.578960 gamelib-0.0.7/gamelib.egg-info/
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     2950 2023-05-30 19:02:50.000000 gamelib-0.0.7/gamelib.egg-info/PKG-INFO
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     1087 2023-05-30 19:02:50.000000 gamelib-0.0.7/gamelib.egg-info/SOURCES.txt
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)        1 2023-05-30 19:02:50.000000 gamelib-0.0.7/gamelib.egg-info/dependency_links.txt
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)        1 2022-12-15 16:20:35.000000 gamelib-0.0.7/gamelib.egg-info/not-zip-safe
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)      167 2023-05-30 19:02:50.000000 gamelib-0.0.7/gamelib.egg-info/requires.txt
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)        8 2023-05-30 19:02:50.000000 gamelib-0.0.7/gamelib.egg-info/top_level.txt
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)      209 2022-12-15 16:20:23.000000 gamelib-0.0.7/pyproject.toml
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)     1057 2023-05-30 19:02:50.582293 gamelib-0.0.7/setup.cfg
+-rw-------   0 peffjepin  (1000) peffjepin  (1000)       69 2022-12-15 16:20:23.000000 gamelib-0.0.7/setup.py
```

### Comparing `gamelib-0.0.4/COPYING` & `gamelib-0.0.7/COPYING`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/PKG-INFO` & `gamelib-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamelib
-Version: 0.0.4
+Version: 0.0.7
 Summary: gamelib: A library for creating 3d applications in python.
 Home-page: https://github.com/peffjepin/gamelib
 Author: Jeffrey Pepin
 License: GPL-3.0-or-later
 Platform: windows
 Platform: linux
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gamelib-0.0.4/README.md` & `gamelib-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/__init__.py` & `gamelib-0.0.7/gamelib/__init__.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/core/events.py` & `gamelib-0.0.7/gamelib/core/events.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/core/gl.py` & `gamelib-0.0.7/gamelib/core/gl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """This module is largely just a namespace for OpenGL constants.
 
 The dtype variables map to numpy structured dtypes representing the OpenGL
 data model.
 """
 
 import numpy as np
-from moderngl.error import Error
 from moderngl import (
     TRIANGLES,
     TRIANGLE_FAN,
     TRIANGLE_STRIP,
     TRIANGLES_ADJACENCY,
     TRIANGLE_STRIP_ADJACENCY,
     POINTS,
     LINES,
     LINE_STRIP,
     LINE_STRIP_ADJACENCY,
     LINE_LOOP,
     LINES_ADJACENCY,
     PATCHES,
+    Error,
 )
-from moderngl.program import Program as GLShader
+
+from moderngl import Program as GLShader
 
 import gamelib
 from gamelib import utils
 
 ensure_opengl = utils.Ensure(
     lambda: gamelib.get_context() is not None,
     "An active OpenGL Context is required to call this function, "
```

### Comparing `gamelib-0.0.4/gamelib/core/input.py` & `gamelib-0.0.7/gamelib/core/input.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/core/resources.py` & `gamelib-0.0.7/gamelib/core/resources.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/core/runtime.py` & `gamelib-0.0.7/gamelib/core/runtime.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/core/time.py` & `gamelib-0.0.7/gamelib/core/time.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/core/vectors.py` & `gamelib-0.0.7/gamelib/core/vectors.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/core/window.py` & `gamelib-0.0.7/gamelib/core/window.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/ecs/base.py` & `gamelib-0.0.7/gamelib/ecs/base.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/ecs/collisions.py` & `gamelib-0.0.7/gamelib/ecs/collisions.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/ecs/transforms.py` & `gamelib-0.0.7/gamelib/ecs/transforms.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/geometry/base.py` & `gamelib-0.0.7/gamelib/geometry/base.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/geometry/collisions.py` & `gamelib-0.0.7/gamelib/geometry/collisions.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/geometry/cube.py` & `gamelib-0.0.7/gamelib/geometry/cube.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/geometry/gridmesh.py` & `gamelib-0.0.7/gamelib/geometry/gridmesh.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/geometry/transforms.py` & `gamelib-0.0.7/gamelib/geometry/transforms.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/geometry/wavefront.py` & `gamelib-0.0.7/gamelib/geometry/wavefront.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/rendering/_global.py` & `gamelib-0.0.7/gamelib/rendering/_global.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/rendering/buffers.py` & `gamelib-0.0.7/gamelib/rendering/buffers.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/rendering/camera.py` & `gamelib-0.0.7/gamelib/rendering/camera.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/rendering/gpu.py` & `gamelib-0.0.7/gamelib/rendering/gpu.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/rendering/shaders.py` & `gamelib-0.0.7/gamelib/rendering/shaders.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/rendering/textures.py` & `gamelib-0.0.7/gamelib/rendering/textures.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/rendering/uniforms.py` & `gamelib-0.0.7/gamelib/rendering/uniforms.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/utils/ensure.py` & `gamelib-0.0.7/gamelib/utils/ensure.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib/utils/mark.py` & `gamelib-0.0.7/gamelib/utils/mark.py`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/gamelib.egg-info/PKG-INFO` & `gamelib-0.0.7/gamelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamelib
-Version: 0.0.4
+Version: 0.0.7
 Summary: gamelib: A library for creating 3d applications in python.
 Home-page: https://github.com/peffjepin/gamelib
 Author: Jeffrey Pepin
 License: GPL-3.0-or-later
 Platform: windows
 Platform: linux
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gamelib-0.0.4/gamelib.egg-info/SOURCES.txt` & `gamelib-0.0.7/gamelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gamelib-0.0.4/setup.cfg` & `gamelib-0.0.7/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gamelib
-version = 0.0.4
+version = 0.0.7
 description = gamelib: A library for creating 3d applications in python.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jeffrey Pepin
 url = https://github.com/peffjepin/gamelib
 license = GPL-3.0-or-later
 license_file = COPYING
@@ -26,16 +26,16 @@
 	gamelib.core
 	gamelib.geometry
 	gamelib.ecs
 	gamelib.utils
 install_requires = 
 	moderngl >=5.6, <6.0
 	moderngl-window >=2.4, <3.0
-	numpy == 1.22.0
-	Pillow==9.3.0, < 10
+	numpy >= 1.22.0, <2.0
+	Pillow >=9.3.0, < 10
 	pygame >= 2.1.0, < 3.0
 python_requires = >= 3.8
 zip_safe = no
 
 [options.extras_require]
 testing = 
 	pytest>=6.0
```

