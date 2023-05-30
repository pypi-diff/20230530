# Comparing `tmp/simplegeomap-0.0.22.tar.gz` & `tmp/simplegeomap-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simplegeomap-0.0.22.tar", last modified: Tue May 23 15:04:17 2023, max compression
+gzip compressed data, was "dist/simplegeomap-0.0.23.tar", last modified: Tue May 30 12:23:11 2023, max compression
```

## Comparing `simplegeomap-0.0.22.tar` & `simplegeomap-0.0.23.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-23 15:04:17.000000 simplegeomap-0.0.22/
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-05-23 15:04:17.000000 simplegeomap-0.0.22/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.22/README.md
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-23 15:04:17.000000 simplegeomap-0.0.22/simplegeomap.egg-info/
--rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-05-23 15:04:16.000000 simplegeomap-0.0.22/simplegeomap.egg-info/dependency_links.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-05-23 15:04:16.000000 simplegeomap-0.0.22/simplegeomap.egg-info/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-05-23 15:04:16.000000 simplegeomap-0.0.22/simplegeomap.egg-info/top_level.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)       51 2023-05-23 15:04:16.000000 simplegeomap-0.0.22/simplegeomap.egg-info/requires.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-05-23 15:04:16.000000 simplegeomap-0.0.22/simplegeomap.egg-info/SOURCES.txt
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-23 15:04:17.000000 simplegeomap-0.0.22/simplegeomap/
--rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.22/simplegeomap/__init__.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     6846 2023-05-23 12:33:25.000000 simplegeomap-0.0.22/simplegeomap/simplegeomap.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     4594 2023-02-11 07:38:14.000000 simplegeomap-0.0.22/simplegeomap/util.py
--rw-rw-r--   0 burak     (1000) burak     (1000)      626 2023-05-23 15:02:43.000000 simplegeomap-0.0.22/setup.py
--rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-05-23 15:04:17.000000 simplegeomap-0.0.22/setup.cfg
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-30 12:23:11.000000 simplegeomap-0.0.23/
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-05-30 12:23:11.000000 simplegeomap-0.0.23/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.23/README.md
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-30 12:23:11.000000 simplegeomap-0.0.23/simplegeomap.egg-info/
+-rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-05-30 12:23:10.000000 simplegeomap-0.0.23/simplegeomap.egg-info/dependency_links.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-05-30 12:23:10.000000 simplegeomap-0.0.23/simplegeomap.egg-info/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-05-30 12:23:10.000000 simplegeomap-0.0.23/simplegeomap.egg-info/top_level.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)       51 2023-05-30 12:23:10.000000 simplegeomap-0.0.23/simplegeomap.egg-info/requires.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-05-30 12:23:11.000000 simplegeomap-0.0.23/simplegeomap.egg-info/SOURCES.txt
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-30 12:23:11.000000 simplegeomap-0.0.23/simplegeomap/
+-rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.23/simplegeomap/__init__.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     6774 2023-05-30 12:14:00.000000 simplegeomap-0.0.23/simplegeomap/simplegeomap.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     5459 2023-05-30 12:11:42.000000 simplegeomap-0.0.23/simplegeomap/util.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)      626 2023-05-30 12:17:42.000000 simplegeomap-0.0.23/setup.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-05-30 12:23:11.000000 simplegeomap-0.0.23/setup.cfg
```

### Comparing `simplegeomap-0.0.22/PKG-INFO` & `simplegeomap-0.0.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.22
+Version: 0.0.23
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.22/README.md` & `simplegeomap-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.22/simplegeomap.egg-info/PKG-INFO` & `simplegeomap-0.0.23/simplegeomap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.22
+Version: 0.0.23
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.22/simplegeomap/simplegeomap.py` & `simplegeomap-0.0.23/simplegeomap/simplegeomap.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pygeodesy.sphericalNvector import LatLon
 import pandas as pd, zipfile, sys, os, csv, io
 import matplotlib.pyplot as plt
 import numpy as np, json, shapefile
-from simplegeomap.util import gltiles
+from simplegeomap.util import gltiles, QuadTreeInterpolator
 
 GWIDTH = 200
 
 def plot_water_df(df,clat,clon,zoom,ax):
     MAX = 60
     CENTER_DIST = (40000. / MAX)*(zoom+1)
     p1 = LatLon(clat,clon) 
@@ -84,16 +84,14 @@
     return lats,lons, np.unique(glatints), np.unique(glonints)
 
 def find_tile(lat,lon):
     res = [lat >= x[0] and lon < x[1] and lon >= x[2] and lon < x[3] for x in gltiles.values()]
     return res.index(True)
 
 def plot_elevation(clat,clon,zoom,levels=None,ax=None):
-    import scipy.interpolate
-    from scipy.ndimage import gaussian_filter
     if not ax: fig, ax = plt.subplots()    
     data_dir = os.path.dirname(__file__)
     npz_file = data_dir + "/gltiles.npz"
     tkeys = np.array(list(gltiles.keys()))
     CENTER_DIST = 2000 * zoom
 
     glat,glon,glatints,glonints = create_grid(clat,clon,CENTER_DIST)
@@ -125,19 +123,19 @@
     np.random.seed(0)
     ridx = np.random.choice(range(len(interpx)), size=8*1000, replace=False)
 
     interpx = interpx[ridx]
     interpy = interpy[ridx]
     interpz = interpz[ridx]
 
-    interp = scipy.interpolate.LinearNDInterpolator(list(zip(interpx, interpy)), interpz)
+    q = QuadTreeInterpolator(interpx, interpy, interpz)
+    interp = np.vectorize(q.interpolate,otypes=[np.float])
 
     newx,newy = np.meshgrid(glon,glat)
     newz = interp(newx,newy)
-    newz = gaussian_filter(newz, sigma=1.0)
     if not levels:
         CS=plt.contour(newx,newy,newz,cmap=plt.cm.binary,levels=[500,1000,1500,2000,3000])
     else:
         CS=plt.contour(newx,newy,newz,cmap=plt.cm.binary,levels=levels)
     plt.clabel(CS, fontsize=10, inline=1)
     
 def plot_line(regarr,ax,color='black',linestyle='solid'):
```

### Comparing `simplegeomap-0.0.22/simplegeomap/util.py` & `simplegeomap-0.0.23/simplegeomap/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pygeodesy.sphericalNvector import LatLon, perimeterOf, meanOf
-import matplotlib.pyplot as plt
+import matplotlib.pyplot as plt, quads
 import numpy as np, shapefile, glob
 import pandas as pd, os
 
 gltiles = {
     "a10g": [50, 90, -180, -90, 1, 6098, 10800, 4800],
     "b10g": [50, 90, -90, 0, 1, 3940, 10800, 4800],
     "c10g": [50, 90, 0, 90, -30, 4010, 10800, 4800],
@@ -99,13 +99,40 @@
                 mid = meanOf(latlons)
                 res.append([mid.lat,mid.lon,per,type,geo])
 
     df = pd.DataFrame(res)
     df.columns = ['lat','lon','perimeter','type','polygon']
     df.to_csv('/tmp/lake_river.csv',index=None)
 
+def cdist(p1,p2):    
+    distances = np.linalg.norm(p1 - p2, axis=1)
+    return distances
+
+class QuadTreeInterpolator:
+    def __init__(self, x, y, z):
+        self.x = x
+        self.y = y
+        self.z = z
+        self.tree = quads.QuadTree((np.mean(x), np.mean(y)), 100, 100)
+        for xx,yy,zz in zip(x,y,z):
+            self.tree.insert((xx,yy),data=zz)
+
+    def interp_cell(self, x, y, points):
+        a = np.array([x,y]).reshape(-1,2)
+        b = np.array(points)[:,:2]
+        ds = cdist(a,b)
+        ds = ds / np.sum(ds)
+        ds = 1. - ds
+        c = np.array(points)[:,2]
+        iz = np.sum(c * ds) / np.sum(ds)
+        return iz
+            
+    def interpolate(self,x,y):
+        res = self.tree.nearest_neighbors((x,y), count=4)
+        points = np.array([[c.x, c.y, c.data] for c in res])
+        return self.interp_cell(x, y, points)
 
 if __name__ == "__main__": 
     
     #preprocess_GSHHS()
     preprocess_GLOBE()
```

### Comparing `simplegeomap-0.0.22/setup.py` & `simplegeomap-0.0.23/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 readme=open("README.md").read()
 
 setuptools.setup(
     name='simplegeomap',    
-    version='0.0.22',
+    version='0.0.23',
     description="Simple offline map plot utility, for country borders, elevation, water",
     long_description=readme,
     long_description_content_type="text/markdown",    
     install_requires=['pandas','pygeodesy','matplotlib','numpy','pyshp','scipy','zarr'],
     include_package_data=True,
     url="https://github.com/burakbayramli/simplegeomap",
     author="Burak Bayramli",
```

