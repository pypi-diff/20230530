# Comparing `tmp/standard-transform-1.3.1.tar.gz` & `tmp/standard-transform-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard-transform-1.3.1.tar", last modified: Tue Apr 18 00:00:44 2023, max compression
+gzip compressed data, was "standard-transform-1.4.0.tar", last modified: Tue May 30 20:15:23 2023, max compression
```

## Comparing `standard-transform-1.3.1.tar` & `standard-transform-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-18 00:00:44.043508 standard-transform-1.3.1/
--rw-r--r--   0 caseysm    (501) staff       (20)     1079 2022-11-16 18:20:55.000000 standard-transform-1.3.1/LICENSE
--rw-r--r--   0 caseysm    (501) staff       (20)       63 2023-04-10 23:37:06.000000 standard-transform-1.3.1/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)     8147 2023-04-18 00:00:44.043212 standard-transform-1.3.1/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     7821 2023-04-15 06:33:04.000000 standard-transform-1.3.1/README.md
--rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-03-28 05:17:19.000000 standard-transform-1.3.1/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-04-18 00:00:44.043563 standard-transform-1.3.1/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1597 2023-04-10 23:43:10.000000 standard-transform-1.3.1/setup.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-18 00:00:44.040117 standard-transform-1.3.1/standard_transform/
--rw-r--r--   0 caseysm    (501) staff       (20)      270 2023-04-18 00:00:27.000000 standard-transform-1.3.1/standard_transform/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     7066 2023-04-10 23:37:06.000000 standard-transform-1.3.1/standard_transform/base.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-18 00:00:44.041939 standard-transform-1.3.1/standard_transform/data/
--rw-r--r--   0 caseysm    (501) staff       (20)    11518 2023-04-15 02:44:52.000000 standard-transform-1.3.1/standard_transform/data/minnie_um_streamline.json
--rw-r--r--   0 caseysm    (501) staff       (20)     5384 2023-04-10 23:37:06.000000 standard-transform-1.3.1/standard_transform/data/v1dd_um_streamline.json
--rw-r--r--   0 caseysm    (501) staff       (20)     5320 2023-04-18 00:00:02.000000 standard-transform-1.3.1/standard_transform/datasets.py
--rw-r--r--   0 caseysm    (501) staff       (20)     9256 2023-04-10 23:37:06.000000 standard-transform-1.3.1/standard_transform/streamlines.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1973 2023-02-25 05:35:09.000000 standard-transform-1.3.1/standard_transform/utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-18 00:00:44.041293 standard-transform-1.3.1/standard_transform.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)     8147 2023-04-18 00:00:44.000000 standard-transform-1.3.1/standard_transform.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      556 2023-04-18 00:00:44.000000 standard-transform-1.3.1/standard_transform.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-04-18 00:00:44.000000 standard-transform-1.3.1/standard_transform.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-04-18 00:00:44.000000 standard-transform-1.3.1/standard_transform.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-04-18 00:00:44.000000 standard-transform-1.3.1/standard_transform.egg-info/top_level.txt
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-18 00:00:44.042712 standard-transform-1.3.1/test/
--rw-r--r--   0 caseysm    (501) staff       (20)     1394 2023-04-10 23:37:06.000000 standard-transform-1.3.1/test/test_streamline.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3762 2023-02-25 05:39:09.000000 standard-transform-1.3.1/test/test_tform.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-30 20:15:23.198361 standard-transform-1.4.0/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1079 2022-11-16 18:20:55.000000 standard-transform-1.4.0/LICENSE
+-rw-r--r--   0 caseysm    (501) staff       (20)       63 2023-04-10 23:37:06.000000 standard-transform-1.4.0/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)    10455 2023-05-30 20:15:23.198054 standard-transform-1.4.0/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)    10129 2023-05-30 20:14:32.000000 standard-transform-1.4.0/README.md
+-rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-03-28 05:17:19.000000 standard-transform-1.4.0/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-05-30 20:15:23.198433 standard-transform-1.4.0/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1597 2023-04-10 23:43:10.000000 standard-transform-1.4.0/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-30 20:15:23.195490 standard-transform-1.4.0/standard_transform/
+-rw-r--r--   0 caseysm    (501) staff       (20)      270 2023-05-30 20:15:13.000000 standard-transform-1.4.0/standard_transform/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     9322 2023-05-10 18:28:48.000000 standard-transform-1.4.0/standard_transform/base.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-30 20:15:23.196811 standard-transform-1.4.0/standard_transform/data/
+-rw-r--r--   0 caseysm    (501) staff       (20)    11518 2023-04-15 02:44:52.000000 standard-transform-1.4.0/standard_transform/data/minnie_um_streamline.json
+-rw-r--r--   0 caseysm    (501) staff       (20)     5384 2023-04-10 23:37:06.000000 standard-transform-1.4.0/standard_transform/data/v1dd_um_streamline.json
+-rw-r--r--   0 caseysm    (501) staff       (20)     5320 2023-04-18 00:00:02.000000 standard-transform-1.4.0/standard_transform/datasets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    13042 2023-05-10 19:26:25.000000 standard-transform-1.4.0/standard_transform/streamlines.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2125 2023-05-10 18:13:21.000000 standard-transform-1.4.0/standard_transform/utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-30 20:15:23.196477 standard-transform-1.4.0/standard_transform.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)    10455 2023-05-30 20:15:23.000000 standard-transform-1.4.0/standard_transform.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      556 2023-05-30 20:15:23.000000 standard-transform-1.4.0/standard_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-05-30 20:15:23.000000 standard-transform-1.4.0/standard_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-05-30 20:15:23.000000 standard-transform-1.4.0/standard_transform.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-05-30 20:15:23.000000 standard-transform-1.4.0/standard_transform.egg-info/top_level.txt
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-30 20:15:23.197513 standard-transform-1.4.0/test/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1394 2023-04-10 23:37:06.000000 standard-transform-1.4.0/test/test_streamline.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3762 2023-02-25 05:39:09.000000 standard-transform-1.4.0/test/test_tform.py
```

### Comparing `standard-transform-1.3.1/LICENSE` & `standard-transform-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.1/PKG-INFO` & `standard-transform-1.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-transform
-Version: 1.3.1
+Version: 1.4.0
 Summary: Define and repeat basic affine transformation tasks for datasets
 Home-page: https://github.com/ceesem/standard_transform
 Author: Casey Schneider-Mizell
 Author-email: caseys@alleninstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -103,14 +103,50 @@
 
 Similarly, you can put all of these together to get a point in the curvilienar space of the streamline, akin to cylindrical coordinates, where the x axis is radial distance and the y axis is depth along the streamline. For each point, an equivalent location in x,z space is found with the same radial distance and angle as the original x and z.
 ```python
 xyz_rad = streamline.radial_points(xyz0, pts)
 ```
 NOTE! While better than nothing, the Minnie65 streamline is much more accurate on the VISp side of the dataset (low x values) than on the HVA side (high x values). The right approach will involve creating a streamline that is interpolates values as a function of x and z instead of being a constant. To do this, we need to either create a lot more streamlines by hand (not too hard, but time consuming) or automatically generate streamlines from skeletons. This will be the ideal solution, but for now, treat the streamline as a good approximation for the VISp side of the dataset. 
 
+## Transforming skeletons
+
+Standard transform has the capability to transform [MeshParty skeletons](https://github.com/sdorkenw/MeshParty/), MeshWorks, and MeshWork annotations using streamline or affine transformation objects. Both streamline and transform objects have similar functionality.
+
+To transform the vertices of a skeleton or meshwork object with the affine transform:
+```python
+#skeleton
+skel_transformed = tform.apply_skeleton(skel)
+#meshwork
+mw_transformed = tform.apply_meshwork_vertices(mw)
+```
+will return a new skeleton object with the transformed vertices. Use the argument `inplace=True` to modify the original object.
+
+For a streamline transform, you can straighten the skeleton along the streamline coordinates. Note that this will relocate the soma or other root location to (0,0,0).
+```python
+# Streamline transform
+skel_straightened = streamline.transform_skeleton_vertices(skel)
+mw_straightened = streamline.transform_meshwork_vertices(mw)
+```
+Similarly, this will return a new object by default, but you can set `inplace=True` to modify the original object.
+By default, this will use the root location of the skeleton as the anchor for the streamline.
+To use a different point, you can specify a `root_loc`.
+Other arguments follow the function `streamline.radial_points`.
+
+Meshwork objects can also have annotations in dataframes as well as vertices. In order to transform these points, we need to specify both the name of the dataframe table and the columns to transform as a dictionary.
+```python
+# Affine transform
+mw_anno_transformed = tform.apply_meshwork_annotations(mw, anno_dict)
+# Streamline transform
+mw_anno_straightened = streamline.transform_meshwork_annotations(mw, anno_dict)
+```
+Here, `anno_dict` is a dictionary whose keys are the table names and the column is one or more dataframe columns where each row contains a 3-element point to transform.
+For example, to transform the `ctr_pt_position` column of the `pre_syn` table, you would pass `anno_dict={'pre_syn': 'ctr_pt_position'}`.
+Similar inplace argument are available as above, as well as `radial_point` arguments for the streamline version.
+Note that if you want to transform both annotation and morphology for meshwork files, you should call both the vertex transform and annotation transform functions.
+
 ## Datasets
 
 Datasets are a convenient way to store a transform and streamline together, and are the easiest way to get started.
 There are two datasets currently available, `minnie65` and `v1dd`.
 To get a dataset, simply import it and initialize it.
 Datasets have a transform and streamline, and can be used to transform points or get streamline information.
 For example, to transform a particular location in v1dd
```

### Comparing `standard-transform-1.3.1/README.md` & `standard-transform-1.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -93,14 +93,50 @@
 
 Similarly, you can put all of these together to get a point in the curvilienar space of the streamline, akin to cylindrical coordinates, where the x axis is radial distance and the y axis is depth along the streamline. For each point, an equivalent location in x,z space is found with the same radial distance and angle as the original x and z.
 ```python
 xyz_rad = streamline.radial_points(xyz0, pts)
 ```
 NOTE! While better than nothing, the Minnie65 streamline is much more accurate on the VISp side of the dataset (low x values) than on the HVA side (high x values). The right approach will involve creating a streamline that is interpolates values as a function of x and z instead of being a constant. To do this, we need to either create a lot more streamlines by hand (not too hard, but time consuming) or automatically generate streamlines from skeletons. This will be the ideal solution, but for now, treat the streamline as a good approximation for the VISp side of the dataset. 
 
+## Transforming skeletons
+
+Standard transform has the capability to transform [MeshParty skeletons](https://github.com/sdorkenw/MeshParty/), MeshWorks, and MeshWork annotations using streamline or affine transformation objects. Both streamline and transform objects have similar functionality.
+
+To transform the vertices of a skeleton or meshwork object with the affine transform:
+```python
+#skeleton
+skel_transformed = tform.apply_skeleton(skel)
+#meshwork
+mw_transformed = tform.apply_meshwork_vertices(mw)
+```
+will return a new skeleton object with the transformed vertices. Use the argument `inplace=True` to modify the original object.
+
+For a streamline transform, you can straighten the skeleton along the streamline coordinates. Note that this will relocate the soma or other root location to (0,0,0).
+```python
+# Streamline transform
+skel_straightened = streamline.transform_skeleton_vertices(skel)
+mw_straightened = streamline.transform_meshwork_vertices(mw)
+```
+Similarly, this will return a new object by default, but you can set `inplace=True` to modify the original object.
+By default, this will use the root location of the skeleton as the anchor for the streamline.
+To use a different point, you can specify a `root_loc`.
+Other arguments follow the function `streamline.radial_points`.
+
+Meshwork objects can also have annotations in dataframes as well as vertices. In order to transform these points, we need to specify both the name of the dataframe table and the columns to transform as a dictionary.
+```python
+# Affine transform
+mw_anno_transformed = tform.apply_meshwork_annotations(mw, anno_dict)
+# Streamline transform
+mw_anno_straightened = streamline.transform_meshwork_annotations(mw, anno_dict)
+```
+Here, `anno_dict` is a dictionary whose keys are the table names and the column is one or more dataframe columns where each row contains a 3-element point to transform.
+For example, to transform the `ctr_pt_position` column of the `pre_syn` table, you would pass `anno_dict={'pre_syn': 'ctr_pt_position'}`.
+Similar inplace argument are available as above, as well as `radial_point` arguments for the streamline version.
+Note that if you want to transform both annotation and morphology for meshwork files, you should call both the vertex transform and annotation transform functions.
+
 ## Datasets
 
 Datasets are a convenient way to store a transform and streamline together, and are the easiest way to get started.
 There are two datasets currently available, `minnie65` and `v1dd`.
 To get a dataset, simply import it and initialize it.
 Datasets have a transform and streamline, and can be used to transform points or get streamline information.
 For example, to transform a particular location in v1dd
```

### Comparing `standard-transform-1.3.1/setup.py` & `standard-transform-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.1/standard_transform/base.py` & `standard-transform-1.4.0/standard_transform/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from scipy.spatial.transform import Rotation as R
 import pandas as pd
 import numpy as np
 from collections.abc import Iterable
-from .utils import get_dataframe_points
+from .utils import get_dataframe_points, is_list_like
 
 class ScaleTransform(object):
     def __init__(self, scaling):
         if not isinstance(scaling, Iterable):
             scaling = np.array(3 * [scaling]).reshape(1, 3)
         else:
             if len(scaling) != 3:
@@ -205,11 +205,83 @@
         else:
             out = self.apply(pts, as_int)
             if return_array:
                 return out
             else:
                 return out.tolist()
 
+    def apply_skeleton(self, sk, inplace=False):
+        """Apply transformation to a meshparty Skeleton
+
+        Parameters
+        ----------
+        sk : meshparty.Skeleton
+            Skeleton to transform
+        inplace : bool, optional
+            If True, transform vertices in place, by default False
+
+        Returns
+        -------
+        Skeleton
+            Skeleton with transformed vertices
+        """
+        if not inplace:
+            sk = sk.copy()
+        sk.vertices = self.apply(sk._rooted.vertices)
+        return sk
+    
+    def apply_meshwork_vertices(self, nrn, inplace=False):
+        """Apply transformation to mesh and skeleton vertices of a meshparty Meshwork
+
+        Parameters
+        ----------
+        nrn : meshparty.meshwork.Meshwork
+            Object to transform
+        inplace : bool, optional
+            If True, transform vertices in place, by default False
+
+        Returns
+        -------
+        Skeleton
+            Skeleton with transformed vertices
+        """
+
+        if not inplace:
+            nrn = nrn.copy()
+        curr_mask = nrn.mesh.node_mask
+        nrn.reset_mask()
+        nrn.mesh.vertices = self.apply( nrn.mesh.vertices )
+        nrn.skeleton.vertices = self.apply( nrn.skeleton.vertices )
+        nrn.apply_mask(curr_mask)
+        return nrn
+
+    def apply_meshwork_annotations(self, nrn, anno_dict, inplace=False):
+        """Apply transformations to annotations in a meshwork
+
+        Parameters
+        ----------
+        nrn : meshwork.Meshwork
+            Object to transform
+        anno_dict : dict
+            Dictionary whose keys are annotation tables in the meshwork and whose values are the columns to transform (string or list of strings)
+        inplace : bool, optional
+            If True, transform vertices in place, by default False
+
+        Returns
+        -------
+        meshwork
+            Object with transformed annotation positions.
+        """
+        if not inplace:
+            nrn = nrn.copy()
+        for tbl in anno_dict:
+            vs = anno_dict[tbl]
+            if not is_list_like(vs):
+                vs = [vs]
+            for v in vs:
+                nrn.anno[tbl]._data[v] = self.apply(nrn.anno[tbl]._data[v])
+        return nrn
+
 
 def identity_transform():
     "Returns the same points provided"
     return TransformSequence()
```

### Comparing `standard-transform-1.3.1/standard_transform/data/minnie_um_streamline.json` & `standard-transform-1.4.0/standard_transform/data/minnie_um_streamline.json`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.1/standard_transform/data/v1dd_um_streamline.json` & `standard-transform-1.4.0/standard_transform/data/v1dd_um_streamline.json`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.1/standard_transform/datasets.py` & `standard-transform-1.4.0/standard_transform/datasets.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.1/standard_transform/streamlines.py` & `standard-transform-1.4.0/standard_transform/streamlines.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from scipy import interpolate
 from .base import identity_transform
-
+from .utils import is_list_like
 
 class Streamline(object):
     def __init__(self, points, tform=None, transform_points=True):
         """Build a streamline object to determine distances from a curving pia-to-white matter axis
 
         Parameters
         ----------
@@ -232,9 +232,93 @@
         xm = np.mean(xyz[:, 0])
         zm = np.mean(xyz[:, 2])
         base_pt = np.array([xm, depth_from, zm])
         sl_pts = self.streamline_at(base_pt, xyz[:, 1], return_as_point=True)
         depths = self.depth_between(base_pt, sl_pts, transform_points=False)
         return depths
 
+    def transform_skeleton_vertices(self, sk, root_loc=None, depth_from=0, delta=0.1, inplace=False):
+        """Transforms skeleton vertices to the post-transform coordinate system via the radial points function.
+        Parameters
+        ----------
+        sk : trimesh.skeleton.Skeleton
+            Skeleton to transform
+        root_loc : np.ndarray, optional
+            3 element array of the root location, by default None. If none, selects the skeleton root.
+        depth_from : numeric, optional
+            Sets the post-transform y coordinate to use for zero depth, by default 0.
+        delta : float, optional
+            Sets the resolution of the depth measurement. Smaller values are more accurate, by default 0.1
+        inplace : bool, optional
+            If True, transform the vertices in place, by default False
+        """
+        if not inplace:
+            sk = sk.copy()
+        if root_loc is None:
+            root_loc = sk.root_position
+        verts_all = sk._rooted.vertices
+        sk.vertices = self.radial_points( root_loc, verts_all, depth_from=depth_from, delta=delta )
+        return sk
+
+    def transform_meshwork_vertices(self, nrn, root_loc=None, depth_from=0, delta=0.1, inplace=False):
+        """Transforms meshwork vertices to the post-transform coordinate system.
+
+        Parameters
+        ----------
+        root_loc : np.ndarray, optional
+            3 element array of the root location, by default None
+        inplace : bool, optional
+            If True, transform the vertices in place, by default False
+
+        Returns
+        -------
+        np.ndarray
+            Nx3 array of transformed vertices
+        """
+        if not inplace:
+            nrn = nrn.copy()
+        curr_mask = nrn.mesh.node_mask
+        if root_loc is None:
+            root_loc = nrn.skeleton.root_position
+        nrn.mesh.vertices = self.radial_points( root_loc, nrn.mesh.vertices, depth_from=depth_from, delta=delta )
+        nrn.skeleton.vertices = self.radial_points( root_loc, nrn.skeleton.vertices, depth_from=depth_from, delta=delta )        
+        nrn.apply_mask(curr_mask)
+        return nrn
+
+    def transform_meshwork_annotations(self, nrn, anno_dict, root_loc=None, depth_from=0, delta=0.1, inplace=False):
+        """Transforms meshwork annotations to the post-transform coordinate system via the radial points function.
+
+        Parameters
+        ----------
+        nrn : meshwork.Meshwork
+            File to transform
+        anno_dict : dict
+            Dictionary whose keys are annotation tables in the meshwork and whose values are the columns to transform (string or list of strings)
+        root_loc : array-like, optional
+            location of the root for computing radial points, by default None. If None, uses the root of the meshwork skeleton.
+        depth_from : int, optional
+            Sets the post-transform y coordinate to use for zero depth, by default 0.
+        delta : float, optional
+            Sets the resolution of the depth measurement. Smaller values are more accurate, by default 0.1
+        inplace : bool, optional
+            If True, transform the vertices in place, by default False
+
+        Returns
+        -------
+        meshwork
+            Object with transformed annotation positions.
+        """
+        if not inplace:
+            nrn = nrn.copy()
+
+        if root_loc is None:
+            root_loc = nrn.skeleton.root_position
+        for tbl in anno_dict:
+            vs = anno_dict[tbl]
+            if not is_list_like(vs):
+                vs = [vs]
+            for v in vs:
+                nrn.anno[tbl]._data[v] = self.radial_points(root_loc, np.vstack(nrn.anno[tbl]._data[v].values), depth_from=depth_from, delta=delta).tolist()
+        return nrn
+
 
 identity_streamline = Streamline(points=np.array([[0, 0, 0], [0, 1000, 0]]))
```

### Comparing `standard-transform-1.3.1/standard_transform/utils.py` & `standard-transform-1.4.0/standard_transform/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,8 +48,17 @@
     return np.vstack(df[cols].values)
 
 
 def get_dataframe_points(pt_col, df):
     if is_split_position(pt_col, df):
         return assemble_split_points(pt_col, df)
     else:
-        return np.vstack(df[pt_col].values)
+        return np.vstack(df[pt_col].values)
+    
+def is_list_like(x):
+    if isinstance(x, str):
+        return False
+    try:
+        len(x)
+        return True
+    except:
+        return False
```

### Comparing `standard-transform-1.3.1/standard_transform.egg-info/PKG-INFO` & `standard-transform-1.4.0/standard_transform.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-transform
-Version: 1.3.1
+Version: 1.4.0
 Summary: Define and repeat basic affine transformation tasks for datasets
 Home-page: https://github.com/ceesem/standard_transform
 Author: Casey Schneider-Mizell
 Author-email: caseys@alleninstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -103,14 +103,50 @@
 
 Similarly, you can put all of these together to get a point in the curvilienar space of the streamline, akin to cylindrical coordinates, where the x axis is radial distance and the y axis is depth along the streamline. For each point, an equivalent location in x,z space is found with the same radial distance and angle as the original x and z.
 ```python
 xyz_rad = streamline.radial_points(xyz0, pts)
 ```
 NOTE! While better than nothing, the Minnie65 streamline is much more accurate on the VISp side of the dataset (low x values) than on the HVA side (high x values). The right approach will involve creating a streamline that is interpolates values as a function of x and z instead of being a constant. To do this, we need to either create a lot more streamlines by hand (not too hard, but time consuming) or automatically generate streamlines from skeletons. This will be the ideal solution, but for now, treat the streamline as a good approximation for the VISp side of the dataset. 
 
+## Transforming skeletons
+
+Standard transform has the capability to transform [MeshParty skeletons](https://github.com/sdorkenw/MeshParty/), MeshWorks, and MeshWork annotations using streamline or affine transformation objects. Both streamline and transform objects have similar functionality.
+
+To transform the vertices of a skeleton or meshwork object with the affine transform:
+```python
+#skeleton
+skel_transformed = tform.apply_skeleton(skel)
+#meshwork
+mw_transformed = tform.apply_meshwork_vertices(mw)
+```
+will return a new skeleton object with the transformed vertices. Use the argument `inplace=True` to modify the original object.
+
+For a streamline transform, you can straighten the skeleton along the streamline coordinates. Note that this will relocate the soma or other root location to (0,0,0).
+```python
+# Streamline transform
+skel_straightened = streamline.transform_skeleton_vertices(skel)
+mw_straightened = streamline.transform_meshwork_vertices(mw)
+```
+Similarly, this will return a new object by default, but you can set `inplace=True` to modify the original object.
+By default, this will use the root location of the skeleton as the anchor for the streamline.
+To use a different point, you can specify a `root_loc`.
+Other arguments follow the function `streamline.radial_points`.
+
+Meshwork objects can also have annotations in dataframes as well as vertices. In order to transform these points, we need to specify both the name of the dataframe table and the columns to transform as a dictionary.
+```python
+# Affine transform
+mw_anno_transformed = tform.apply_meshwork_annotations(mw, anno_dict)
+# Streamline transform
+mw_anno_straightened = streamline.transform_meshwork_annotations(mw, anno_dict)
+```
+Here, `anno_dict` is a dictionary whose keys are the table names and the column is one or more dataframe columns where each row contains a 3-element point to transform.
+For example, to transform the `ctr_pt_position` column of the `pre_syn` table, you would pass `anno_dict={'pre_syn': 'ctr_pt_position'}`.
+Similar inplace argument are available as above, as well as `radial_point` arguments for the streamline version.
+Note that if you want to transform both annotation and morphology for meshwork files, you should call both the vertex transform and annotation transform functions.
+
 ## Datasets
 
 Datasets are a convenient way to store a transform and streamline together, and are the easiest way to get started.
 There are two datasets currently available, `minnie65` and `v1dd`.
 To get a dataset, simply import it and initialize it.
 Datasets have a transform and streamline, and can be used to transform points or get streamline information.
 For example, to transform a particular location in v1dd
```

### Comparing `standard-transform-1.3.1/standard_transform.egg-info/SOURCES.txt` & `standard-transform-1.4.0/standard_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.1/test/test_streamline.py` & `standard-transform-1.4.0/test/test_streamline.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.1/test/test_tform.py` & `standard-transform-1.4.0/test/test_tform.py`

 * *Files identical despite different names*

