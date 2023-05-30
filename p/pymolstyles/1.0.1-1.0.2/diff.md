# Comparing `tmp/pymolstyles-1.0.1.tar.gz` & `tmp/pymolstyles-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymolstyles-1.0.1.tar", max compression
+gzip compressed data, was "pymolstyles-1.0.2.tar", max compression
```

## Comparing `pymolstyles-1.0.1.tar` & `pymolstyles-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-01-20 20:03:27.506072 pymolstyles-1.0.1/LICENSE.md
--rw-r--r--   0        0        0       51 2023-01-20 21:34:09.270609 pymolstyles-1.0.1/README.md
--rw-r--r--   0        0        0      347 2023-01-20 21:30:18.612165 pymolstyles-1.0.1/pymolstyles/__init__.py
--rw-r--r--   0        0        0     4912 2023-01-20 19:56:39.666063 pymolstyles-1.0.1/pymolstyles/environment.py
--rw-r--r--   0        0        0     2077 2023-01-20 19:56:39.666063 pymolstyles-1.0.1/pymolstyles/external/cgo_arrow.py
--rw-r--r--   0        0        0     3172 2023-01-21 02:56:46.488474 pymolstyles-1.0.1/pymolstyles/plots.py
--rw-r--r--   0        0        0      161 2023-01-20 19:56:39.666063 pymolstyles-1.0.1/pymolstyles/resources.py
--rw-r--r--   0        0        0     1384 2023-01-20 21:30:18.612165 pymolstyles-1.0.1/pymolstyles/styles.py
--rw-r--r--   0        0        0     2785 2023-01-24 16:29:16.110759 pymolstyles-1.0.1/pymolstyles/tools.py
--rw-r--r--   0        0        0      236 2023-01-20 21:14:30.481153 pymolstyles-1.0.1/pymolstyles/workspace.py
--rw-r--r--   0        0        0      459 2023-01-26 16:35:07.617927 pymolstyles-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 pymolstyles-1.0.1/setup.py
--rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 pymolstyles-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-20 20:03:27.506072 pymolstyles-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0       51 2023-01-20 21:34:09.270609 pymolstyles-1.0.2/README.md
+-rw-r--r--   0        0        0      347 2023-01-20 21:30:18.612165 pymolstyles-1.0.2/pymolstyles/__init__.py
+-rw-r--r--   0        0        0     4912 2023-01-20 19:56:39.666063 pymolstyles-1.0.2/pymolstyles/environment.py
+-rw-r--r--   0        0        0     2077 2023-01-20 19:56:39.666063 pymolstyles-1.0.2/pymolstyles/external/cgo_arrow.py
+-rw-r--r--   0        0        0     3337 2023-05-30 21:09:31.011841 pymolstyles-1.0.2/pymolstyles/plots.py
+-rw-r--r--   0        0        0      161 2023-01-20 19:56:39.666063 pymolstyles-1.0.2/pymolstyles/resources.py
+-rw-r--r--   0        0        0     1384 2023-01-20 21:30:18.612165 pymolstyles-1.0.2/pymolstyles/styles.py
+-rw-r--r--   0        0        0     2785 2023-01-24 16:29:16.110759 pymolstyles-1.0.2/pymolstyles/tools.py
+-rw-r--r--   0        0        0      236 2023-01-20 21:14:30.481153 pymolstyles-1.0.2/pymolstyles/workspace.py
+-rw-r--r--   0        0        0      459 2023-05-30 21:19:58.027363 pymolstyles-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 pymolstyles-1.0.2/PKG-INFO
```

### Comparing `pymolstyles-1.0.1/LICENSE.md` & `pymolstyles-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pymolstyles-1.0.1/pymolstyles/environment.py` & `pymolstyles-1.0.2/pymolstyles/environment.py`

 * *Files identical despite different names*

### Comparing `pymolstyles-1.0.1/pymolstyles/external/cgo_arrow.py` & `pymolstyles-1.0.2/pymolstyles/external/cgo_arrow.py`

 * *Files identical despite different names*

### Comparing `pymolstyles-1.0.1/pymolstyles/plots.py` & `pymolstyles-1.0.2/pymolstyles/plots.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,30 +54,34 @@
     cmd.isosurface("dens",densf, isovalue)
     cmd.ramp_new("ramp", gradf, [min_surface, max_surface], 'rainbow')
     cmd.set("surface_color", "ramp", "dens")
     cmd.set('transparency', 0.50, 'dens')
     cmd.set('two_sided_lighting',value=1)
 cmd.extend("plot_elpot", plot_elpot)
 
-def plot_sterimol(origin, sterimol_coordinates):
+def plot_sterimol(atoms_coordinates, sterimol_coordinates):
     cmd.delete('*_vector')
 
-    origin = ast.literal_eval(origin)
+    print(atoms_coordinates)
+
+    atoms_coordinates = ast.literal_eval(atoms_coordinates)
     sterimol_coordinates = ast.literal_eval(sterimol_coordinates)
 
-    cmd.pseudoatom('c', pos=origin, elem='Cs')
+    cmd.pseudoatom('a1', pos=atoms_coordinates[0], elem='Cs')
+    cmd.pseudoatom('a2', pos=atoms_coordinates[1], elem='Cs')
     cmd.pseudoatom('L', pos=sterimol_coordinates[0], elem='Cs')
     cmd.pseudoatom('B1', pos=sterimol_coordinates[1], elem='Cs')
     cmd.pseudoatom('B5', pos=sterimol_coordinates[2], elem='Cs')
 
-    cgo_arrow('/c','/L', 0.1, color='red', name='L_vector')
-    cgo_arrow('/c','/B1', 0.1, color='green', name='B1_vector')
-    cgo_arrow('/c','/B5', 0.1, color='blue', name='B5_vector')
+    cgo_arrow('/a1','/L', 0.1, color='red', name='L_vector')
+    cgo_arrow('/a2','/B1', 0.1, color='green', name='B1_vector')
+    cgo_arrow('/a2','/B5', 0.1, color='blue', name='B5_vector')
 
-    cmd.delete('c')
+    cmd.delete('a1')
+    cmd.delete('a2')
     cmd.delete('L')
     cmd.delete('B1')
     cmd.delete('B5')
 cmd.extend('plot_sterimol', plot_sterimol)
 
 
 def plot_buried_volume(bv_name, color='lightblue', radius=3.5):
```

### Comparing `pymolstyles-1.0.1/pymolstyles/styles.py` & `pymolstyles-1.0.2/pymolstyles/styles.py`

 * *Files identical despite different names*

### Comparing `pymolstyles-1.0.1/pymolstyles/tools.py` & `pymolstyles-1.0.2/pymolstyles/tools.py`

 * *Files identical despite different names*

### Comparing `pymolstyles-1.0.1/PKG-INFO` & `pymolstyles-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymolstyles
-Version: 1.0.1
+Version: 1.0.2
 Summary: Scripts for small molecule visualization using PyMOL
 License: GNU GENERAL PUBLIC LICENSE V3
 Author: Attilio Chiavegatti
 Author-email: attiliochiavegatti@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

