# Comparing `tmp/large-image-source-rasterio-1.22.1.dev2.tar.gz` & `tmp/large-image-source-rasterio-1.22.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-rasterio-1.22.1.dev2.tar", last modified: Tue May 30 14:08:21 2023, max compression
+gzip compressed data, was "large-image-source-rasterio-1.22.1.dev3.tar", last modified: Tue May 30 15:27:05 2023, max compression
```

## Comparing `large-image-source-rasterio-1.22.1.dev2.tar` & `large-image-source-rasterio-1.22.1.dev3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-30 14:08:21.767796 large-image-source-rasterio-1.22.1.dev2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-05-30 14:08:21.000000 large-image-source-rasterio-1.22.1.dev2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-05-30 14:08:21.767796 large-image-source-rasterio-1.22.1.dev2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-05-30 14:08:21.000000 large-image-source-rasterio-1.22.1.dev2/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-30 14:08:21.763796 large-image-source-rasterio-1.22.1.dev2/large_image_source_rasterio/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42753 2023-05-30 14:06:34.000000 large-image-source-rasterio-1.22.1.dev2/large_image_source_rasterio/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-05-30 14:06:34.000000 large-image-source-rasterio-1.22.1.dev2/large_image_source_rasterio/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-30 14:08:21.767796 large-image-source-rasterio-1.22.1.dev2/large_image_source_rasterio.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-05-30 14:08:21.000000 large-image-source-rasterio-1.22.1.dev2/large_image_source_rasterio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-05-30 14:08:21.000000 large-image-source-rasterio-1.22.1.dev2/large_image_source_rasterio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-30 14:08:21.000000 large-image-source-rasterio-1.22.1.dev2/large_image_source_rasterio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-05-30 14:08:21.000000 large-image-source-rasterio-1.22.1.dev2/large_image_source_rasterio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-05-30 14:08:21.000000 large-image-source-rasterio-1.22.1.dev2/large_image_source_rasterio.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-05-30 14:08:21.000000 large-image-source-rasterio-1.22.1.dev2/large_image_source_rasterio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-30 14:08:21.767796 large-image-source-rasterio-1.22.1.dev2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2564 2023-05-30 14:06:34.000000 large-image-source-rasterio-1.22.1.dev2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-30 15:27:05.715318 large-image-source-rasterio-1.22.1.dev3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-05-30 15:27:05.000000 large-image-source-rasterio-1.22.1.dev3/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-05-30 15:27:05.715318 large-image-source-rasterio-1.22.1.dev3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-05-30 15:27:05.000000 large-image-source-rasterio-1.22.1.dev3/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-30 15:27:05.711318 large-image-source-rasterio-1.22.1.dev3/large_image_source_rasterio/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42967 2023-05-30 15:24:54.000000 large-image-source-rasterio-1.22.1.dev3/large_image_source_rasterio/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-05-30 15:24:54.000000 large-image-source-rasterio-1.22.1.dev3/large_image_source_rasterio/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-30 15:27:05.715318 large-image-source-rasterio-1.22.1.dev3/large_image_source_rasterio.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-05-30 15:27:05.000000 large-image-source-rasterio-1.22.1.dev3/large_image_source_rasterio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-05-30 15:27:05.000000 large-image-source-rasterio-1.22.1.dev3/large_image_source_rasterio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-30 15:27:05.000000 large-image-source-rasterio-1.22.1.dev3/large_image_source_rasterio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-05-30 15:27:05.000000 large-image-source-rasterio-1.22.1.dev3/large_image_source_rasterio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-05-30 15:27:05.000000 large-image-source-rasterio-1.22.1.dev3/large_image_source_rasterio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-05-30 15:27:05.000000 large-image-source-rasterio-1.22.1.dev3/large_image_source_rasterio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-30 15:27:05.715318 large-image-source-rasterio-1.22.1.dev3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2564 2023-05-30 15:24:54.000000 large-image-source-rasterio-1.22.1.dev3/setup.py
```

### Comparing `large-image-source-rasterio-1.22.1.dev2/LICENSE` & `large-image-source-rasterio-1.22.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.22.1.dev2/PKG-INFO` & `large-image-source-rasterio-1.22.1.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.22.1.dev2
+Version: 1.22.1.dev3
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.22.1.dev2/README.rst` & `large-image-source-rasterio-1.22.1.dev3/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.22.1.dev2/large_image_source_rasterio/__init__.py` & `large-image-source-rasterio-1.22.1.dev3/large_image_source_rasterio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 import warnings
 from contextlib import suppress
 
 import numpy as np
 import PIL.Image
 import rasterio as rio
 from affine import Affine
-from pyproj import CRS, Transformer
-from pyproj.exceptions import CRSError
+from rasterio import warp
 from rasterio.enums import ColorInterp, Resampling
 from rasterio.errors import RasterioIOError
 
 import large_image
 from large_image.cache_util import LruCacheMetaclass, methodcache
 from large_image.constants import (TILE_FORMAT_IMAGE, TILE_FORMAT_NUMPY,
                                    TILE_FORMAT_PIL, TileInputUnits,
@@ -54,27 +53,37 @@
 except PackageNotFoundError:
     # package is not installed
     pass
 
 warnings.filterwarnings('ignore', category=rio.errors.NotGeoreferencedWarning, module='rasterio')
 
 
+def make_crs(projection):
+    if isinstance(projection, str):
+        return rio.CRS.from_string(projection)
+    if isinstance(projection, dict):
+        return rio.CRS.from_dict(projection)
+    if isinstance(projection, int):
+        return rio.CRS.from_string(f'EPSG:{projection}')
+    return rio.CRS(projection)
+
+
 class RasterioFileTileSource(GDALBaseFileTileSource, metaclass=LruCacheMetaclass):
     """Provides tile access to geospatial files."""
 
     cacheName = 'tilesource'
     name = 'rasterio'
 
     def __init__(self, path, projection=None, unitsPerPixel=None, **kwargs):
         """Initialize the tile class.
 
         See the base class for other available parameters.
 
         :param path: a filesystem path for the tile source.
-        :param projection: None to use pixel space, otherwise a crs compatible with pyproj.
+        :param projection: None to use pixel space, otherwise a crs compatible with rasterio's CRS.
         :param unitsPerPixel: The size of a pixel at the 0 tile size.
             Ignored if the projection is None.  For projections, None uses the default,
             which is the distance between (-180,0) and (180,0) in EPSG:4326 converted to the
             projection divided by the tile size. crs projections that are not latlong
             (is_geographic is False) must specify unitsPerPixel.
 
         """
@@ -107,15 +116,15 @@
                     raise TileSourceError('netCDF file will not be read via rasterio source.')
 
         # extract default parameters from the image
         self.tileSize = 256
         self._bounds = {}
         self.tileWidth = self.tileSize
         self.tileHeight = self.tileSize
-        self.projection = CRS(projection) if projection else None
+        self.projection = make_crs(projection) if projection else None
 
         # get width and height parameters
         with self._getDatasetLock:
             self.sourceSizeX = self.sizeX = self.dataset.width
             self.sourceSizeY = self.sizeY = self.dataset.height
 
         # netCDF is blacklisted from rasterio so it won't be used.
@@ -207,15 +216,15 @@
         band_frame['max'] = np.append(band_frame['max'], range_max)
 
     def _initWithProjection(self, unitsPerPixel=None):
         """Initialize aspects of the class when a projection is set.
 
         :param unitsPerPixel: optional default to None
         """
-        srcCrs = CRS(4326)
+        srcCrs = make_crs(4326)
         # Since we already converted to bytes decoding is safe here
         dstCrs = self.projection
         if dstCrs.is_geographic:
             raise TileSourceError(
                 'Projection must not be geographic (it needs to use linear '
                 'units, not longitude/latitude).'
             )
@@ -226,16 +235,16 @@
             self.unitsAcrossLevel0 = ProjUnitsAcrossLevel0.get(
                 self.projection.to_string()
             )
             if self.unitsAcrossLevel0 is None:
                 # If unitsPerPixel is not specified, the horizontal distance
                 # between -180,0 and +180,0 is used.  Some projections (such as
                 # stereographic) will fail in this case; they must have a unitsPerPixel specified.
-                equator = Transformer.from_crs(srcCrs, dstCrs, always_xy=True)
-                east, west = equator.itransform([(-180, 0), (180, 0)])
+                east, _ = warp.transform(srcCrs, dstCrs, [-180,], [0,])
+                west, _ = warp.transform(srcCrs, dstCrs, [180,], [0,])
                 self.unitsAcrossLevel0 = abs(east[0] - west[0])
                 if not self.unitsAcrossLevel0:
                     raise TileSourceError(
                         'unitsPerPixel must be specified for this projection'
                     )
                 if len(ProjUnitsAcrossLevel0) >= ProjUnitsAcrossLevel0_MaxSize:
                     ProjUnitsAcrossLevel0.clear()
@@ -289,15 +298,15 @@
                 crs = self.dataset.crs
 
             # if no crs but the file is a NITF or has a valid affine transform then
             # consider it as 4326
             hasTransform = self.dataset.transform != Affine.identity()
             isNitf = self.dataset.driver.lower() in {'NITF'}
             if not crs and (hasTransform or isNitf):
-                crs = CRS(4326)
+                crs = make_crs(4326)
 
             return crs
 
     def _getAffine(self):
         """Get the Affine transformation.
 
         If GCPs are used, get the appropriate Affine for those. Be careful,
@@ -322,15 +331,15 @@
         :returns: an object with the four corners and the projection that was used.
             None if we don't know the original projection.
         """
         if crs is None and 'srs' in kwargs:
             crs = kwargs.get('srs')
 
         # read the crs as a crs if needed
-        dstCrs = CRS(crs) if crs else None
+        dstCrs = make_crs(crs) if crs else None
         strDstCrs = 'none' if dstCrs is None else dstCrs.to_string()
 
         # exit if it's already set
         if strDstCrs in self._bounds:
             return self._bounds[strDstCrs]
 
         # extract the projection information
@@ -366,16 +375,15 @@
 
         # ensure that the coordinates are within the projection limits
         if srcCrs.is_geographic and dstCrs:
 
             # set the vertical bounds
             # some projection system don't cover the poles so we need to adapt
             # the values of ybounds accordingly
-            transformer = Transformer.from_crs(4326, dstCrs, always_xy=True)
-            has_poles = transformer.transform(0, 90)[1] != float('inf')
+            has_poles = warp.transform(4326, dstCrs, [0], [90])[1][0] != float('inf')
             yBounds = 90 if has_poles else 89.999999
 
             # for each corner fix the latitude within -yBounds yBounds
             for k in bounds:
                 bounds[k]['y'] = max(min(bounds[k]['y'], yBounds), -yBounds)
 
             # for each corner rotate longitude until it's within -180, 180
@@ -390,17 +398,16 @@
             if any(v['x'] >= 180 for v in bounds.values()):
                 bounds['ul']['x'] = bounds['ll']['x'] = -180
                 bounds['ur']['x'] = bounds['lr']['x'] = 180
 
         # reproject the pts in the destination coordinate system if necessary
         needProjection = dstCrs and dstCrs != srcCrs
         if needProjection:
-            transformer = Transformer.from_crs(srcCrs, dstCrs, always_xy=True)
             for pt in bounds.values():
-                pt['x'], pt['y'] = transformer.transform(pt['x'], pt['y'])
+                [pt['x']], [pt['y']] = warp.transform(srcCrs, dstCrs, [pt['x']], [pt['y']])
 
         # extract min max coordinates from the corners
         ll = bounds['ll']['x'], bounds['ll']['y']
         ul = bounds['ul']['x'], bounds['ul']['y']
         lr = bounds['lr']['x'], bounds['lr']['y']
         ur = bounds['ur']['x'], bounds['ur']['y']
         bounds['xmin'] = min(ll[0], ul[0], lr[0], ur[0])
@@ -667,23 +674,22 @@
             units = 'base_pixels'
 
         # compute the coordinates if the projection exist
         else:
             if units.startswith('proj4:'):
                 # HACK to avoid `proj4:` prefixes with `WGS84`, etc.
                 units = units.split(':', 1)[1]
-            srcCrs = CRS(units)
+            srcCrs = make_crs(units)
             dstCrs = self.projection  # instance projection -- do not use the CRS native to the file
-            transformer = Transformer.from_crs(srcCrs, dstCrs, always_xy=True)
-            pleft, ptop = transformer.transform(
-                right if left is None else left,
-                bottom if top is None else top)
-            pright, pbottom = transformer.transform(
-                left if right is None else right,
-                top if bottom is None else bottom)
+            [pleft], [ptop] = warp.transform(srcCrs, dstCrs,
+                                             [right if left is None else left],
+                                             [bottom if top is None else top])
+            [pright], [pbottom] = warp.transform(srcCrs, dstCrs,
+                                                 [left if right is None else right],
+                                                 [top if bottom is None else bottom])
             units = 'projection'
 
         # set the corner value in pixel coordinates if the coordinate was initially
         # set else leave it to None
         left = pleft if left is not None else None
         top = ptop if top is not None else None
         right = pright if right is not None else None
@@ -726,16 +732,16 @@
         :returns: left, top, right, bottom bounds in pixels.
         """
         isUnits = units is not None
         units = TileInputUnits.get(units.lower() if isUnits else None, units)
 
         # check if the units is a string or projection material
         isProj = False
-        with suppress(CRSError):
-            isProj = CRS(units) is not None
+        with suppress(rio.errors.CRSError):
+            isProj = make_crs(units) is not None
 
         # convert the coordinates if a projection exist
         if isUnits and isProj:
             left, top, right, bottom, units = self._convertProjectionUnits(
                 left, top, right, bottom, width, height, units, **kwargs
             )
 
@@ -817,20 +823,19 @@
         :param x: the x coordinate it the native projection.
         :param y: the y coordinate it the native projection.
         :param crs: input projection.  None to use the sources's projection.
         :param roundResults: if True, round the results to the nearest pixel.
 
         :return: (x, y) the pixel coordinate.
         """
-        srcCrs = self.projection if crs is None else CRS(crs)
+        srcCrs = self.projection if crs is None else make_crs(crs)
 
         # convert to the native projection
-        dstCrs = CRS(self.getCrs())
-        transformer = Transformer.from_crs(srcCrs, dstCrs, always_xy=True)
-        px, py = transformer.transform(x, y)
+        dstCrs = make_crs(self.getCrs())
+        [px], [py] = warp.transform(srcCrs, dstCrs, [x], [y])
 
         # convert to native pixel coordinates
         af = self._getAffine()
         d = af[1] * af[3] - af[0] * af[4]
         x = (af[2] * af[4] - af[1] * af[5] - af[4] * px + af[1] * py) / d
         y = (af[0] * af[5] - af[2] * af[3] + af[3] * px - af[0] * py) / d
```

### Comparing `large-image-source-rasterio-1.22.1.dev2/large_image_source_rasterio/girder_source.py` & `large-image-source-rasterio-1.22.1.dev3/large_image_source_rasterio/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.22.1.dev2/large_image_source_rasterio.egg-info/PKG-INFO` & `large-image-source-rasterio-1.22.1.dev3/large_image_source_rasterio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.22.1.dev2
+Version: 1.22.1.dev3
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.22.1.dev2/setup.py` & `large-image-source-rasterio-1.22.1.dev3/setup.py`

 * *Files identical despite different names*

