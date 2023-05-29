# Comparing `tmp/cfr-0.5.1.tar.gz` & `tmp/cfr-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-0.5.1.tar", last modified: Wed May 24 03:34:20 2023, max compression
+gzip compressed data, was "cfr-0.5.2.tar", last modified: Mon May 29 21:58:35 2023, max compression
```

## Comparing `cfr-0.5.1.tar` & `cfr-0.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-05-24 03:34:20.195831 cfr-0.5.1/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1516 2023-03-03 14:30:05.000000 cfr-0.5.1/LICENSE
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1771 2023-05-24 03:34:20.195532 cfr-0.5.1/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1207 2023-04-22 19:12:46.000000 cfr-0.5.1/README.md
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-05-24 03:34:20.188119 cfr-0.5.1/bin/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3905 2023-03-03 14:30:05.000000 cfr-0.5.1/bin/cfr
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-05-24 03:34:20.192043 cfr-0.5.1/cfr/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      640 2023-03-24 19:14:09.000000 cfr-0.5.1/cfr/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    20017 2023-05-24 03:32:11.000000 cfr-0.5.1/cfr/climate.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-05-24 03:34:20.195089 cfr-0.5.1/cfr/da/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       22 2023-03-03 14:30:05.000000 cfr-0.5.1/cfr/da/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    16319 2023-03-26 05:47:23.000000 cfr-0.5.1/cfr/da/enkf.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    22484 2023-04-17 17:43:24.000000 cfr-0.5.1/cfr/gcm.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7623 2023-03-03 14:30:05.000000 cfr-0.5.1/cfr/ml.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    65492 2023-05-24 03:15:55.000000 cfr-0.5.1/cfr/proxy.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    44996 2023-04-22 03:20:57.000000 cfr-0.5.1/cfr/psm.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    49933 2023-04-09 06:47:02.000000 cfr-0.5.1/cfr/reconjob.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2311 2023-03-26 06:27:24.000000 cfr-0.5.1/cfr/reconres.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    17993 2023-04-26 03:13:51.000000 cfr-0.5.1/cfr/ts.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    21776 2023-05-24 03:00:31.000000 cfr-0.5.1/cfr/utils.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    54810 2023-04-06 07:30:44.000000 cfr-0.5.1/cfr/visual.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-05-24 03:34:20.194311 cfr-0.5.1/cfr.egg-info/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1771 2023-05-24 03:34:19.000000 cfr-0.5.1/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      373 2023-05-24 03:34:19.000000 cfr-0.5.1/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-05-24 03:34:19.000000 cfr-0.5.1/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-03-03 14:35:18.000000 cfr-0.5.1/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      203 2023-05-24 03:34:19.000000 cfr-0.5.1/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-05-24 03:34:19.000000 cfr-0.5.1/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-05-24 03:34:20.195950 cfr-0.5.1/setup.cfg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1414 2023-05-24 03:32:47.000000 cfr-0.5.1/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 21:58:35.718806 cfr-0.5.2/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.5.2/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1771 2023-05-29 21:58:35.718629 cfr-0.5.2/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.5.2/README.md
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 21:58:35.708847 cfr-0.5.2/bin/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     3905 2022-07-04 04:11:55.000000 cfr-0.5.2/bin/cfr
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 21:58:35.714622 cfr-0.5.2/cfr/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      640 2023-03-24 23:03:50.000000 cfr-0.5.2/cfr/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    20667 2023-05-29 21:16:00.000000 cfr-0.5.2/cfr/climate.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 21:58:35.718135 cfr-0.5.2/cfr/da/
+-rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.5.2/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.5.2/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.5.2/cfr/gcm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.5.2/cfr/ml.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    63265 2023-05-29 21:16:00.000000 cfr-0.5.2/cfr/proxy.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    44993 2023-05-29 21:16:00.000000 cfr-0.5.2/cfr/psm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    49995 2023-05-29 21:16:00.000000 cfr-0.5.2/cfr/reconjob.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.5.2/cfr/reconres.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.5.2/cfr/ts.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    26581 2023-05-29 21:16:00.000000 cfr-0.5.2/cfr/utils.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.5.2/cfr/visual.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-05-29 21:58:35.717304 cfr-0.5.2/cfr.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1771 2023-05-29 21:58:35.000000 cfr-0.5.2/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-05-29 21:58:35.000000 cfr-0.5.2/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-05-29 21:58:35.000000 cfr-0.5.2/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.5.2/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)      203 2023-05-29 21:58:35.000000 cfr-0.5.2/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-05-29 21:58:35.000000 cfr-0.5.2/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-05-29 21:58:35.718864 cfr-0.5.2/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1414 2023-05-29 21:57:43.000000 cfr-0.5.2/setup.py
```

### Comparing `cfr-0.5.1/LICENSE` & `cfr-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-0.5.1/PKG-INFO` & `cfr-0.5.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.5.1
+Version: 0.5.2
 Summary: cfr: the Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: paleocliamte reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.5.1/README.md` & `cfr-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cfr-0.5.1/bin/cfr` & `cfr-0.5.2/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-0.5.1/cfr/__init__.py` & `cfr-0.5.2/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.1/cfr/climate.py` & `cfr-0.5.2/cfr/climate.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,44 +54,48 @@
             raise ValueError('Wrong mode. Should be either "360" or "180".')
 
         da = da.sortby(da['lon'])
         fd = ClimateField(da)
         return fd
 
     def fetch(self, name=None, **load_nc_kws):
-        url_dict = {
-            'iCESM_past1000historical/tas': 'https://atmos.washington.edu/~rtardif/LMR/prior/tas_sfc_Amon_iCESM_past1000historical_085001-200512.nc',
-            'iCESM_past1000historical/pr': 'https://atmos.washington.edu/~rtardif/LMR/prior/pr_sfc_Amon_iCESM_past1000historical_085001-200512.nc',
-            'iCESM_past1000historical/d18O': 'https://atmos.washington.edu/~rtardif/LMR/prior/d18O_sfc_Amon_iCESM_past1000historical_085001-200512.nc',
-            'iCESM_past1000historical/psl': 'https://atmos.washington.edu/~rtardif/LMR/prior/psl_sfc_Amon_iCESM_past1000historical_085001-200512.nc',
-            'iCESM_past1000/tas': 'https://atmos.washington.edu/~rtardif/LMR/prior/tas_sfc_Amon_iCESM_past1000_085001-184912.nc',
-            'iCESM_past1000/pr': 'https://atmos.washington.edu/~rtardif/LMR/prior/pr_sfc_Amon_iCESM_past1000_085001-184912.nc',
-            'iCESM_past1000/d18O': 'https://atmos.washington.edu/~rtardif/LMR/prior/d18O_sfc_Amon_iCESM_past1000_085001-184912.nc',
-            'iCESM_past1000/psl': 'https://atmos.washington.edu/~rtardif/LMR/prior/psl_sfc_Amon_iCESM_past1000_085001-184912.nc',
-        }
+        ''' Fetch a gridded climate field from cloud
+
+        Args:
+            name (str): a predifined name or an URL starting with "http"
+        '''
+        url_dict = utils.climfd_url_dict
 
-        if name[:4] != 'http':
-            if name is None:
-                utils.p_warning(f'>>> Choose one from the supported entries: {list(url_dict.keys())}')
-                return None
+        if name is None:
+            utils.p_warning(f'>>> Choose one from the supported entries:')
+            for k in url_dict.keys():
+                utils.p_warning(f'- {k}')
+            return None
 
+        if name in url_dict:
             url = url_dict[name]
         else:
             url = name
 
-        fpath = f'./data/{os.path.basename(url)}'
-        if os.path.exists(fpath):
-            utils.p_hint(f'>>> The target file seems existed at: {fpath} . Loading from it instead of downloading ...')
+        if url[:4] == 'http':
+            # cloud
+            os.makedirs('./data', exist_ok=True)
+            fpath = f'./data/{os.path.basename(url)}'
+            if os.path.exists(fpath):
+                utils.p_hint(f'>>> The target file seems existed at: {fpath} . Loading from it instead of downloading ...')
+            else:
+                utils.download(url, fpath)
+                utils.p_success(f'>>> Downloaded file saved at: {fpath}')
         else:
-            utils.download(url, fpath)
-            utils.p_success(f'>>> Downloaded file saved at: {fpath} .')
+            # local
+            fpath = url
 
-        pdb = self.load_nc(fpath, **load_nc_kws)
+        fd = self.load_nc(fpath, **load_nc_kws)
 
-        return pdb
+        return fd
 
     def from_np(self, time, lat, lon, value):
         ''' Load data from a `numpy.ndarray`.
         '''
         lat_da = xr.DataArray(lat, dims=['lat'], coords={'lat': lat})
         lon_da = xr.DataArray(lon, dims=['lon'], coords={'lon': lon})
         time_da = xr.DataArray(time, dims=['time'], coords={'time': time})
@@ -564,8 +568,33 @@
 
         return  fd
 
     def geo_mean(self, lat_min=-90, lat_max=90, lon_min=0, lon_max=360):
         ''' Calculate the geographical mean value of the climate field. '''
         m = utils.geo_mean(self.da, lat_min=lat_min, lat_max=lat_max, lon_min=lon_min, lon_max=lon_max)
         ts = EnsTS(time=m['time'].values, value=m.values)
-        return ts
+        return ts
+
+    def index(self, name):
+        if name == 'gm': 
+            return self.geo_mean()
+        elif name == 'nhm': 
+            return self.geo_mean(lat_min=0)
+        elif name == 'shm':
+            return self.geo_mean(lat_max=0)
+        elif name == 'nino3.4':
+            return self.geo_mean(lat_min=-5, lat_max=5, lon_min=np.mod(-170, 360), lon_max=np.mod(-120, 360))
+        elif name == 'nino1+2':
+            return self.geo_mean(lat_min=-10, lat_max=10, lon_min=np.mod(-90, 360), lon_max=np.mod(-80, 360))
+        elif name == 'nino3':
+            return self.geo_mean(lat_min=-5, lat_max=5, lon_min=np.mod(-150, 360), lon_max=np.mod(-90, 360))
+        elif name == 'nino4':
+            return self.geo_mean(lat_min=-5, lat_max=5, lon_min=np.mod(160, 360), lon_max=np.mod(-150, 360))
+        elif name == 'wpi':
+            return self.geo_mean(lat_min=-10, lat_max=10, lon_min=np.mod(120, 360), lon_max=np.mod(150, 360))
+        elif name == 'tpi':
+            v1 = self.geo_mean(lat_min=25, lat_max=45, lon_min=np.mod(140, 360), lon_max=np.mod(-145, 360))
+            v2 = self.geo_mean(lat_min=-10, lat_max=10, lon_min=np.mod(170, 360), lon_max=np.mod(-90, 360))
+            v3 = self.geo_mean(lat_min=-50, lat_max=-15, lon_min=np.mod(150, 360), lon_max=np.mod(-160, 360))
+            return v2 - (v1 + v3)/2
+        else:
+            raise ValueError('Wrong index name.')
```

### Comparing `cfr-0.5.1/cfr/da/enkf.py` & `cfr-0.5.2/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.1/cfr/gcm.py` & `cfr-0.5.2/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.1/cfr/ml.py` & `cfr-0.5.2/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.1/cfr/proxy.py` & `cfr-0.5.2/cfr/proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -888,60 +888,56 @@
         self.type_dict = {}
         for t in self.type_list:
             if t not in self.type_dict:
                 self.type_dict[t] = 1
             else:
                 self.type_dict[t] += 1
 
-    def fetch(self, db_name=None):
-        url_dict = {
-            'PAGES2k': 'https://github.com/fzhu2e/cfr/raw/main/docsrc/notebooks/data/pages2k.json',
-            'pseudoPAGES2k/ppwn_SNRinf_rta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNRinf_rta.nc',
-            'pseudoPAGES2k/ppwn_SNR10_rta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR10_rta.nc',
-            'pseudoPAGES2k/ppwn_SNR2_rta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR2_rta.nc',
-            'pseudoPAGES2k/ppwn_SNR1_rta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR1_rta.nc',
-            'pseudoPAGES2k/ppwn_SNR0.5_rta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR0.5_rta.nc',
-            'pseudoPAGES2k/ppwn_SNR0.25_rta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR0.25_rta.nc',
-            'pseudoPAGES2k/ppwn_SNRinf_fta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNRinf_fta.nc',
-            'pseudoPAGES2k/ppwn_SNR10_fta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR10_fta.nc',
-            'pseudoPAGES2k/ppwn_SNR2_fta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR2_fta.nc',
-            'pseudoPAGES2k/ppwn_SNR1_fta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR1_fta.nc',
-            'pseudoPAGES2k/ppwn_SNR0.5_fta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR0.5_fta.nc',
-            'pseudoPAGES2k/ppwn_SNR0.25_fta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/ppwn_SNR0.25_fta.nc',
-            'pseudoPAGES2k/tpwn_SNR10_rta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR10_rta.nc',
-            'pseudoPAGES2k/tpwn_SNR2_rta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR2_rta.nc',
-            'pseudoPAGES2k/tpwn_SNR1_rta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR1_rta.nc',
-            'pseudoPAGES2k/tpwn_SNR0.5_rta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR0.5_rta.nc',
-            'pseudoPAGES2k/tpwn_SNR0.25_rta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR0.25_rta.nc',
-            'pseudoPAGES2k/tpwn_SNR10_fta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR10_fta.nc',
-            'pseudoPAGES2k/tpwn_SNR2_fta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR2_fta.nc',
-            'pseudoPAGES2k/tpwn_SNR1_fta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR1_fta.nc',
-            'pseudoPAGES2k/tpwn_SNR0.5_fta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR0.5_fta.nc',
-            'pseudoPAGES2k/tpwn_SNR0.25_fta': 'https://github.com/fzhu2e/paper-pseudoPAGES2k/raw/main/data/tpwn_SNR0.25_fta.nc',
-        }
+    def fetch(self, name=None):
+        ''' Fetch a proxy database from cloud
+
+        Args:
+            name (str): a predifined database name or an URL starting with "http" 
+        '''
+        url_dict = utils.proxydb_url_dict
 
-        if db_name is None:
-            p_warning(f'>>> Choose one from the supported databases: {list(url_dict.keys())}')
+        if name is None:
+            p_warning(f'>>> Choose one from the supported databases:')
+            for k in url_dict.keys():
+                p_warning(f'- {k}')
             return None
 
+        if name in url_dict:
+            url = url_dict[name]
+        else:
+            url = name
+
         read_func = {
             '.json': pd.read_json,
             '.csv': pd.read_csv,
+            '.pkl': pd.read_pickle,
         }
-        url = url_dict[db_name]
-        ext = os.path.splitext(url)[-1]
+        ext = os.path.splitext(url)[-1].lower()
         if ext == '.nc':
-            fpath = '.cfr_download_tmp'
-            if os.path.exists(fpath): os.remove(fpath)
-            utils.download(url, fpath)
-            pdb = self.load_nc(fpath)
-            os.remove(fpath)
-        else:
+            if url[:4] == 'http':
+                # cloud
+                fpath = '.cfr_download_tmp'
+                if os.path.exists(fpath): os.remove(fpath)
+                utils.download(url, fpath, show_bar=False)
+                pdb = self.load_nc(fpath)
+                os.remove(fpath)
+            else:
+                # local
+                pdb = self.load_nc(url)
+        elif ext in read_func:
+            # cloud & local
             df = read_func[ext](url)
             pdb = self.from_df(df)
+        else:
+            raise ValueError('Wrong file extention based on the given URL!')
 
         return pdb
 
     def from_df(self, df, pid_column='paleoData_pages2kID', lat_column='geo_meanLat', lon_column='geo_meanLon', elev_column='geo_meanElev',
                 time_column='year', value_column='paleoData_values', proxy_type_column='paleoData_proxy', archive_type_column='archiveType',
                 value_name_column='paleoData_variableName', value_unit_column='paleoData_units',
                 verbose=False):
```

### Comparing `cfr-0.5.1/cfr/psm.py` & `cfr-0.5.2/cfr/psm.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         for sn in season_list:
             exog_ann = exog.annualize(months=sn)
             df_exog = pd.DataFrame({'time': exog_ann.da.time.values, exog_colname: exog_ann.da.values})
             df_proxy = pd.DataFrame({'time': self.pobj.time, 'proxy': self.pobj.value})
             df = df_proxy.dropna().merge(df_exog.dropna(), how='inner', on='time')
             df.set_index('time', drop=True, inplace=True)
             df.sort_index(inplace=True)
-            df.astype(np.float)
+            df.astype(float)
             if calib_period is not None:
                 mask = (df.index>=calib_period[0]) & (df.index<=calib_period[1])
                 df = clean_df(df, mask=mask)
 
             formula_spell = f'proxy ~ {exog_colname}'
             nobs = len(df)
             if nobs < nobs_lb:
```

### Comparing `cfr-0.5.1/cfr/reconjob.py` & `cfr-0.5.2/cfr/reconjob.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,21 +132,22 @@
 
         Args:
             path (str, optional): the path to the pickle file of the `pandas.DataFrame`. Defaults to None.
             verbose (bool, optional): print verbose information. Defaults to False.
         '''
         path = self.io_cfg('proxydb_path', path, verbose=verbose)
 
-        _, ext =  os.path.splitext(path)
-        if ext.lower() == '.pkl':
-            df = pd.read_pickle(path)
-        else:
-            raise ReadError(f'The extention of the file [{ext}] is not supported. Support list: [.pkl, ] .')
+        # _, ext =  os.path.splitext(path)
+        # if ext.lower() == '.pkl':
+        #     df = pd.read_pickle(path)
+        # else:
+        #     raise ReadError(f'The extention of the file [{ext}] is not supported. Support list: [.pkl, ] .')
 
-        self.proxydb = ProxyDatabase().from_df(df, **kwargs)
+        # self.proxydb = ProxyDatabase().from_df(df, **kwargs)
+        self.proxydb = ProxyDatabase().fetch(name=path)
         if verbose:
             p_success(f'>>> {self.proxydb.nrec} records loaded')
             p_success(f'>>> job.proxydb created')
 
     def filter_proxydb(self, *args, inplace=True, verbose=False, **kwargs):
         ''' Filter the proxy database.
 
@@ -299,30 +300,30 @@
         for vn, path in path_dict.items():
             if rename_dict is None:
                 vn_in_file = vn
             else:
                 vn_in_file = rename_dict[vn]
 
             if anom_period == 'null':
-                self.__dict__[tag][vn] = ClimateField().load_nc(
+                self.__dict__[tag][vn] = ClimateField().fetch(
                     path, vn=vn_in_file,
                     time_name=time_name,
                     lat_name=lat_name,
                     lon_name=lon_name,
                     load=load).wrap_lon()
             else:
                 try:
-                    self.__dict__[tag][vn] = ClimateField().load_nc(
+                    self.__dict__[tag][vn] = ClimateField().fetch(
                         path, vn=vn_in_file,
                         time_name=time_name,
                         lat_name=lat_name,
                         lon_name=lon_name,
                         load=load).get_anom(ref_period=anom_period).wrap_lon()
                 except:
-                    self.__dict__[tag][vn] = ClimateField().load_nc(
+                    self.__dict__[tag][vn] = ClimateField().fetch(
                         path, vn=vn_in_file,
                         time_name=time_name,
                         lat_name=lat_name,
                         lon_name=lon_name,
                         load=load).center(ref_period=anom_period).wrap_lon()
 
             self.__dict__[tag][vn].da.name = vn
```

### Comparing `cfr-0.5.1/cfr/reconres.py` & `cfr-0.5.2/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.1/cfr/ts.py` & `cfr-0.5.2/cfr/ts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-
+import os
+import xarray as xr
 import numpy as np
+import cftime
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.colors import LogNorm
 from scipy.stats import pearsonr
 import copy
 from . import utils
 from .utils import (
@@ -14,15 +16,14 @@
     p_fail,
     p_warning,
 )
 
 class EnsTS:
     ''' The class for ensemble timeseries
 
-    Note that annual resolution is assumed so the time axis is in years.
     The ensembles variable should be in shape of (nt, nEns), where nt is the number of years,
     and nEns is the number of ensemble members.
 
     Args:
         time (numpy.array): the time axis of the series
         value (numpy.array): the value axis of the series
         value_name (str): the name of value axis; will be used as ylabel in plots
@@ -35,25 +36,81 @@
     '''
     def __init__(self, time=None, value=None, value_name=None):
         if np.ndim(value) == 1:
             value = value[:, np.newaxis]
 
         if time is not None:
             try:
+                time = [np.datetime64(t) for t in time]
+            except:
+                pass
+
+            try:
                 time = utils.datetime2year_float(time)
             except:
                 pass
 
         self.time = time
         self.value = value
         self.value_name = value_name
 
         if self.value is not None:
             self.refresh()
 
+    def annualize(self, months=list(range(1, 13)), verbose=False):
+        new = self.copy()
+        new.value = []
+        for val in self.value.T:
+            try:
+                new.time, val_ann = utils.annualize(self.time, val, months=months)
+            except:
+                new.time, val_ann = utils.annualize(self.time, val, months=list(range(1, 13)))
+                if verbose: p_warning(f'Record {self.pid} cannot be annualized with months {months}. Use calendar year instead.')
+
+            new.time, val_ann = utils.clean_ts(new.time, val_ann)
+            new.value.append(val_ann)
+        
+        new.value = np.array(new.value).T
+        new.refresh()
+        return new
+
+    def fetch(self, name=None, **from_df_kws):
+        ''' Fetch a proxy database from cloud
+
+        Args:
+            name (str): a predifined database name or an URL starting with "http" 
+        '''
+        url_dict = utils.ensts_url_dict
+
+        if name is None:
+            p_warning(f'>>> Choose one from the supported databases:')
+            for k in url_dict.keys():
+                p_warning(f'- {k}')
+            return None
+
+        if name in url_dict:
+            url = url_dict[name]
+        else:
+            url = name
+
+        read_func = {
+            '.json': pd.read_json,
+            '.csv': pd.read_csv,
+            '.pkl': pd.read_pickle,
+        }
+        ext = os.path.splitext(url)[-1].lower()
+        if ext in read_func:
+            # cloud & local
+            df = read_func[ext](url)
+            ensts = self.from_df(df, **from_df_kws)
+        else:
+            raise ValueError('Wrong file extention based on the given URL!')
+
+        return ensts
+
     def refresh(self):
         self.nt = np.shape(self.value)[0]
         self.nEns = np.shape(self.value)[1]
         self.median = np.nanmedian(self.value, axis=1)
         self.mean = np.nanmean(self.value, axis=1)
         self.std = np.nanstd(self.value, axis=1)
 
@@ -71,32 +128,29 @@
 
     def get_std(self):
         res = self.copy() # copy object to get metadata
         res.value = self.std[:, np.newaxis]
         res.refresh()
         return res
 
-    def from_df(self, df, time_column=None, value_columns=None):
+    def from_df(self, df, time_column='time', value_columns=None):
         ''' Load data from a pandas.DataFrame
 
         Parameters
         ----------
         df : pandas.DataFrame
             The pandas.DataFrame object.
 
         time_column : str
             The label of the column for the time axis.
 
         value_columns : list of str
             The list of the labels for the value axis of the ensemble members.
 
         '''
-        if time_column is None:
-            raise ValueError('`time_column` must be specified!')
-
         if value_columns is None:
             value_columns = list(set(df.columns) - {time_column})
             
         arr = df[value_columns].values
         time = df[time_column].values
         nt = len(time)
         value = np.reshape(arr, (nt, -1))
@@ -463,25 +517,29 @@
             ax.set_title(title, **_title_kwargs)
 
         if 'fig' in locals():
             return fig, ax
         else:
             return ax
 
-    def compare(self, ref_time, ref_value, ref_name='reference', stats=['corr', 'CE'], timespan=None):
+    def compare(self, ref=None, ref_time=None, ref_value=None, ref_name='reference', stats=['corr', 'CE'], timespan=None):
         ''' Compare against a reference timeseries.
 
         Args:
+            ref (cfr.ts.EnsTS): the reference time series object
             ref_time (numpy.array): the time axis of the reference timeseries
             ref_value (numpy.array): the value axis of the reference timeseries
             stats (list, optional): the list of validation statistics to calculate. Defaults to ['corr', 'CE'].
             timespan (tuple, optional): the time period for validation. Defaults to None.
         '''
         new = self.copy()
         new.valid_stats = {}
+        if ref is not None:
+            ref_time = ref.time
+            ref_value = ref.median
         ref_time = np.array(ref_time)
         ref_value = np.array(ref_value)
         new.ref_name = ref_name
 
         recon_value = np.array(self.get_median().value)[:, 0]
         recon_time = np.array(self.get_median().time)
```

### Comparing `cfr-0.5.1/cfr/visual.py` & `cfr-0.5.2/cfr/visual.py`

 * *Files identical despite different names*

### Comparing `cfr-0.5.1/cfr.egg-info/PKG-INFO` & `cfr-0.5.2/cfr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.5.1
+Version: 0.5.2
 Summary: cfr: the Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: paleocliamte reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.5.1/setup.py` & `cfr-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='0.5.1',
+    version='0.5.2',
     description='cfr: the Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

