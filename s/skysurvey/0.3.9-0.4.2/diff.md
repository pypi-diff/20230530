# Comparing `tmp/skysurvey-0.3.9.tar.gz` & `tmp/skysurvey-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skysurvey-0.3.9.tar", last modified: Tue Dec 20 19:53:35 2022, max compression
+gzip compressed data, was "skysurvey-0.4.2.tar", last modified: Tue May 30 21:07:02 2023, max compression
```

## Comparing `skysurvey-0.3.9.tar` & `skysurvey-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-20 19:53:35.475514 skysurvey-0.3.9/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.3.9/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      257 2022-12-20 19:53:35.475378 skysurvey-0.3.9/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)     2333 2022-09-14 19:00:29.000000 skysurvey-0.3.9/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2022-12-20 19:53:35.475554 skysurvey-0.3.9/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)      632 2022-12-20 19:53:02.000000 skysurvey-0.3.9/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-20 19:53:35.471337 skysurvey-0.3.9/skysurvey/
--rw-r--r--   0 rigault   (2358) staff       (20)       92 2022-12-20 19:52:56.000000 skysurvey-0.3.9/skysurvey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)      398 2022-08-16 14:00:03.000000 skysurvey-0.3.9/skysurvey/config.py
--rw-r--r--   0 rigault   (2358) staff       (20)     7196 2022-09-29 17:14:54.000000 skysurvey-0.3.9/skysurvey/dag.py
--rw-r--r--   0 rigault   (2358) staff       (20)    19776 2022-12-20 19:50:41.000000 skysurvey-0.3.9/skysurvey/dataset.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-20 19:53:35.473076 skysurvey-0.3.9/skysurvey/survey/
--rw-r--r--   0 rigault   (2358) staff       (20)      101 2022-09-17 12:56:09.000000 skysurvey-0.3.9/skysurvey/survey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     8363 2022-12-19 09:32:29.000000 skysurvey-0.3.9/skysurvey/survey/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)    10972 2022-12-17 16:46:15.000000 skysurvey-0.3.9/skysurvey/survey/healpix.py
--rw-r--r--   0 rigault   (2358) staff       (20)     5306 2022-12-17 16:44:36.000000 skysurvey-0.3.9/skysurvey/survey/polygon.py
--rw-r--r--   0 rigault   (2358) staff       (20)     1698 2022-12-20 11:13:58.000000 skysurvey-0.3.9/skysurvey/survey/ztf.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-20 19:53:35.475096 skysurvey-0.3.9/skysurvey/target/
--rw-r--r--   0 rigault   (2358) staff       (20)       67 2022-09-29 07:34:56.000000 skysurvey-0.3.9/skysurvey/target/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     8328 2022-10-06 11:54:26.000000 skysurvey-0.3.9/skysurvey/target/collection.py
--rw-r--r--   0 rigault   (2358) staff       (20)    23105 2022-12-20 19:21:14.000000 skysurvey-0.3.9/skysurvey/target/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.3.9/skysurvey/target/environments.py
--rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.3.9/skysurvey/target/kilonova.py
--rw-r--r--   0 rigault   (2358) staff       (20)     9415 2022-10-06 08:36:21.000000 skysurvey-0.3.9/skysurvey/target/snia.py
--rw-r--r--   0 rigault   (2358) staff       (20)     1927 2022-10-07 13:10:54.000000 skysurvey-0.3.9/skysurvey/target/snii.py
--rw-r--r--   0 rigault   (2358) staff       (20)      606 2022-09-26 14:53:44.000000 skysurvey-0.3.9/skysurvey/target/stars.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2261 2022-10-06 11:55:05.000000 skysurvey-0.3.9/skysurvey/target/timeserie.py
--rw-r--r--   0 rigault   (2358) staff       (20)    15523 2022-12-07 13:53:25.000000 skysurvey-0.3.9/skysurvey/template.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-20 19:53:35.471973 skysurvey-0.3.9/skysurvey.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      257 2022-12-20 19:53:35.000000 skysurvey-0.3.9/skysurvey.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      647 2022-12-20 19:53:35.000000 skysurvey-0.3.9/skysurvey.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2022-12-20 19:53:35.000000 skysurvey-0.3.9/skysurvey.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       10 2022-12-20 19:53:35.000000 skysurvey-0.3.9/skysurvey.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-30 21:07:02.591515 skysurvey-0.4.2/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.4.2/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-05-30 21:07:02.591377 skysurvey-0.4.2/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     2333 2022-09-14 19:00:29.000000 skysurvey-0.4.2/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-30 21:07:02.591559 skysurvey-0.4.2/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)      632 2023-05-30 21:06:14.000000 skysurvey-0.4.2/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-30 21:07:02.586612 skysurvey-0.4.2/skysurvey/
+-rw-r--r--   0 rigault   (2358) staff       (20)       92 2023-05-30 21:06:10.000000 skysurvey-0.4.2/skysurvey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      398 2022-08-16 14:00:03.000000 skysurvey-0.4.2/skysurvey/config.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    12346 2023-05-30 13:23:34.000000 skysurvey-0.4.2/skysurvey/dag.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    26322 2023-05-10 13:33:52.000000 skysurvey-0.4.2/skysurvey/dataset.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-30 21:07:02.588215 skysurvey-0.4.2/skysurvey/survey/
+-rw-r--r--   0 rigault   (2358) staff       (20)      101 2022-09-17 12:56:09.000000 skysurvey-0.4.2/skysurvey/survey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     8645 2023-05-02 20:15:06.000000 skysurvey-0.4.2/skysurvey/survey/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    10973 2023-01-04 15:12:21.000000 skysurvey-0.4.2/skysurvey/survey/healpix.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     5306 2022-12-17 16:44:36.000000 skysurvey-0.4.2/skysurvey/survey/polygon.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     1698 2022-12-20 11:13:58.000000 skysurvey-0.4.2/skysurvey/survey/ztf.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-30 21:07:02.591055 skysurvey-0.4.2/skysurvey/target/
+-rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.4.2/skysurvey/target/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    11766 2023-05-05 08:45:44.000000 skysurvey-0.4.2/skysurvey/target/collection.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    31265 2023-05-30 21:05:06.000000 skysurvey-0.4.2/skysurvey/target/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.4.2/skysurvey/target/environments.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.4.2/skysurvey/target/kilonova.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2342 2023-05-07 10:18:11.000000 skysurvey-0.4.2/skysurvey/target/sncc.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     9879 2023-02-08 13:19:45.000000 skysurvey-0.4.2/skysurvey/target/snia.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-05-10 14:57:36.000000 skysurvey-0.4.2/skysurvey/target/stars.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     6216 2023-05-04 16:01:10.000000 skysurvey-0.4.2/skysurvey/target/timeserie.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    16507 2023-05-26 07:31:27.000000 skysurvey-0.4.2/skysurvey/template.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-30 21:07:02.587095 skysurvey-0.4.2/skysurvey.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-05-30 21:07:02.000000 skysurvey-0.4.2/skysurvey.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      647 2023-05-30 21:07:02.000000 skysurvey-0.4.2/skysurvey.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-05-30 21:07:02.000000 skysurvey-0.4.2/skysurvey.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-05-30 21:07:02.000000 skysurvey-0.4.2/skysurvey.egg-info/top_level.txt
```

### Comparing `skysurvey-0.3.9/LICENSE` & `skysurvey-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.9/README.md` & `skysurvey-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.9/setup.py` & `skysurvey-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.3.9'
+VERSION = '0.4.2'
         
 setup(name='skysurvey',
       version=VERSION,
       description='Simulating Transient in the sky and how to observe them',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/skysurvey',
```

### Comparing `skysurvey-0.3.9/skysurvey/dataset.py` & `skysurvey-0.4.2/skysurvey/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from astropy.table import Table
 
 from .template import Template
 
 
 __all__ = ["DataSet", "get_obsdata"]
 
-
 def get_obsdata(template, observations, parameters, zpsys="ab"):
     """ get observed data using ``sncosmo.realize_lcs()``
 
     Parameters
     ----------
     template: sncosmo.Model
         an sncosmo model from which we can draw observations
@@ -53,14 +52,44 @@
     # realize LC
     list_of_observations = sncosmo.realize_lcs(sncosmo_obs, template, list_of_parameters)
     if len(list_of_observations) == 0:
         return None
     
     return pandas.concat([l.to_pandas().set_index(observations.index) for l in list_of_observations],  keys=parameters.index)
 
+def _get_obsdata_(data, **kwargs):
+    """ internal method to simplify get_obsdata using single input (for map)
+
+    Parameters
+    ----------
+    data: list
+        3 entries:
+        template: sncosmo.Model
+            an sncosmo model from which we can draw observations
+            
+        observations: pandas.DataFrame
+            Dataframe containing the observing infortation.
+            requested entries: TBD
+    
+        parameters: pandas.DataFrame
+            Dataframe containing the target parameters information.
+            These depend on you model. 
+
+    **kwargs goes to get_obsdata
+
+    Returns
+    -------
+    MultiIndex DataFrame
+        all the observations for all targets
+
+    See also
+    --------
+    DataSet.from_targets_and_survey: generate a DataSet from target and survey's object
+    """
+    return get_obsdata(*data, **kwargs)
 
 
 # ================== #
 #                    #
 #    DataSet         #
 #                    #
 # ================== #
@@ -75,15 +104,15 @@
         read_parquet: loads a stored dataset
         """
         self.set_data(data)
         self.set_targets(targets)
         self.set_survey(survey)
         
     @classmethod
-    def from_targets_and_survey(cls, targets, survey, template=None, **kwargs):
+    def from_targets_and_survey(cls, targets, survey, template=None, client=None, **kwargs):
         """ loads a dataset (observed data) given targets and a survey
 
         This first matches the targets (given targets.data[["ra","dec"]]) with the
         survey to find which target has been observed with which field.
         Then simulate the targets lightcurves given the observing data (survey.data).
         
 
@@ -92,28 +121,34 @@
         targets: skysurvey.Target (or child of)
             target data corresponding to the true target parameters  
             (as given by nature)
             
         survey: skysurvey.Survey (or child of)
             sky observation (what was observed when with which situation)
 
+        client: dask.distributed.Client()
+            dask client to use if any. This is used for 
+            parallelization of the lc generation per field.
 
         **kwargs goes to realize_survey_target_lcs
 
         Returns
         -------
         class instance
             the observation data have been derived and stored as self.data
 
         See also
         --------
         read_parquet: loads a stored dataset
         """
-        data = cls.realize_survey_target_lcs(targets, survey, template=template,
+        lightcurves, fieldids = cls.realize_survey_target_lcs(targets, survey, template=template,
+                                                                  client=client,
                                                  **kwargs)
+        data = pandas.concat(lightcurves, keys=fieldids # store fieldid
+                                 ).reset_index(survey.fieldids.names)
         return cls(data, targets=targets, survey=survey)
 
     @classmethod
     def read_parquet(cls, parquetfile, survey=None, targets=None, **kwargs):
         """ loads a stored dataset. 
 
         Only the observation data can be loaded this way, 
@@ -258,19 +293,19 @@
         -------
         pandas.Series
             the number of detected point per target (and per band if per_band=True)
         """
         data = self.data.copy()
         data["detected"] = (data["flux"]/data["fluxerr"])>detlimit
         if per_band:
-            ndetection = data.reset_index().set_index(["level_0","level_1","band"]).groupby(level=[0,2])["detected"].sum()
+            groupby = ["index","band"]
         else:
-            ndetection = data.groupby(level=0)["detected"].sum()
-
-            
+            groupby = "index"
+        
+        ndetection = data.groupby(groupby)["detected"].sum()
         return ndetection
 
 
     def get_target_lightcurve(self, index, detection_only=False, detlimit=5.):
         """ get the observation of the given target.
         
         = short cut to self.data.xs(index) = 
@@ -450,50 +485,68 @@
             results = results.merge(truth, left_index=True, right_index=True)
             
         return results, metas    
     # -------- #
     #  PLOTTER #
     # -------- #
     def show_target_lightcurve(self, ax=None, fig=None, index=None, zp=25,
-                                lc_prop={}, bands=None, 
+                                lc_prop={}, bands=None, show_truth=True,
                                 format_time=True, t0_format="mjd", 
                                 phase_window=None, **kwargs):
         """ if index is None, a random index will be used. 
         if bands is None, the target's observed band will be used.
         """
         from matplotlib.colors import to_rgba
         from .config import get_band_color
         
         if format_time:
             from astropy.time import Time
         if index is None:
             index = np.random.choice(self.obs_index)
 
         # Data
-        obs_ = self.get_target_lightcurve(index)
+        obs_ = self.get_target_lightcurve(index).copy()
         if phase_window is not None:
             t0 = self.targets.data["t0"].loc[index]
             phase_window = np.asarray(phase_window)+t0
             obs_ = obs_[obs_["time"].between(*phase_window)]
 
         coef = 10 ** (-(obs_["zp"] - zp) / 2.5)
         obs_["flux_zp"] = obs_["flux"] * coef
         obs_["fluxerr_zp"] = obs_["fluxerr"] * coef
 
         # Model
         if bands is None:
             bands = np.unique(obs_["band"])
 
+        # = axes and figure = #
+        if ax is None:
+            if fig is None:
+                import matplotlib.pyplot as plt
+                fig = plt.figure(figsize=[7,4])
+            ax = fig.add_subplot(111)
+        else:
+            fig = ax.figure
+        
+        
         colors = get_band_color(bands)
-        fig = self.targets.show_lightcurve(bands, ax=ax, fig=fig, index=index, 
+        if show_truth:
+            fig = self.targets.show_lightcurve(bands, ax=ax, fig=fig, index=index, 
                                            format_time=format_time, t0_format=t0_format, 
                                            zp=zp, colors=colors,
                                            zorder=2, 
                                            **lc_prop)
-        ax = fig.axes[0]
+        elif format_time:
+            from matplotlib import dates as mdates        
+            locator = mdates.AutoDateLocator()
+            formatter = mdates.ConciseDateFormatter(locator)
+            ax.xaxis.set_major_locator(locator)
+            ax.xaxis.set_major_formatter(formatter)
+        else:
+            ax.set_xlabel("time [in day]", fontsize="large")
 
 
 
         for band_, color_ in zip(bands, colors):
             obs_band = obs_[obs_["band"] == band_]
             times = obs_band["time"] if not format_time else Time(obs_band["time"], format=t0_format).datetime
             ax.scatter(times, obs_band["flux_zp"],
@@ -501,93 +554,205 @@
             ax.errorbar(times, obs_band["flux_zp"],
                         yerr= obs_band["fluxerr_zp"],
                         ls="None", marker="None", ecolor=to_rgba(color_, 0.2), 
                         zorder=3,
                         **kwargs)
 
         return fig
+    
     # -------------- #
     #    Statics     #
     # -------------- #
+    @classmethod
+    def realize_survey_target_lcs(cls, targets, survey, template=None,
+                                  template_prop={}, nfirst=None,
+                                  client=None):
+        """ creates the lightcurve of the input targets as they 
+        would be observed by the survey. 
+        = These are split per survey fields. =
+        
+        
+        Parameters
+        ----------
+        targets: skysurvey.Target, skysurvey.TargetCollection
+            target data corresponding to the true target parameters  
+            (as given by nature)
+            
+        survey: skysurvey.Survey (or child of)
+            sky observation (what was observed when with which situation)
+
+        template: Template
+            template to use to generate the lightcurve.
+            If None given, the target's template is used.
+
+        template_prop: dict
+            kwargs for template.get(), setting the template parameters
+            
+        nfirst: int
+            if given, only the first nfrist entries will be considered.
+            This is a debug / test tool.
+        
+        client: dask.distributed.Client()
+            dask client to use if any. This is used for 
+            parallelization of the lc generation per field.
+        
+            
+        Returns
+        -------
+        list, list
+            - list of dataframe (1 per fields, all targets of the field in)
+            - list of fields (fieldid)
+            
+        See also
+        --------
+        from_targets_and_survey: laods the instance given targets and a survey
+        """
+        if hasattr(targets.template, "__iter__"): # collection of single-kind
+            samekind_targets = targets.as_targets()
+            outs = [cls._realize_survey_kindtarget_lcs(t_, survey)
+                        for t_ in samekind_targets]
+            # lightcurves and fields
+            lc_out = [l_ for l,v in outs for l_ in l if l is not None] # list of list of dataframe
+            fieldids_indexes = np.vstack([np.vstack(v) for l,v in outs if v is not None]) # all fields for all cases
+            fieldids_indexes = np.squeeze(fieldids_indexes) # 1-d or n-d ?
+            if len(survey.fieldids.names) > 1: # multi-index
+                fieldids_indexes = pandas.MultiIndex.from_arrays(fieldids_indexes.T, names=survey.fieldids.names)
+            else: # single-index
+                fieldids_indexes = pandas.Index(data=fieldids_indexes, name=survey.fieldids.names[0])
+                
+        else: # input is a single-kind target
+            lc_out, fieldids_indexes = cls._realize_survey_kindtarget_lcs(targets, survey,
+                                                          template=template,
+                                                          template_prop=template_prop,
+                                                          nfirst=nfirst,
+                                                          client=client)
+        return lc_out, fieldids_indexes
+
+        
     @staticmethod
-    def realize_survey_target_lcs(targets, survey, template=None,
-                                  template_prop={}, nfirst=None):
-        """ """
+    def _realize_survey_kindtarget_lcs( targets, survey, template=None,
+                                           template_prop={}, nfirst=None,
+                                           client=None):
+        """ creates the lightcurve of the input single-kind 
+        targets as they  would be observed by the survey. 
+        = These are split per survey fields. =
+        
+        
+        Parameters
+        ----------
+        targets: skysurvey.Target, skysurvey.TargetCollection
+            target data corresponding to the true target parameters  
+            (as given by nature)
+            
+        survey: skysurvey.Survey (or child of)
+            sky observation (what was observed when with which situation)
+
+        template: Template
+            template to use to generate the lightcurve.
+            If None given, the target's template is used.
+
+        template_prop: dict
+            kwargs for template.get(), setting the template parameters
+            
+        nfirst: int
+            if given, only the first nfrist entries will be considered.
+            This is a debug / test tool.
+        
+        client: dask.distributed.Client()
+            dask client to use if any. This is used for 
+            parallelization of the lc generation per field.
+        
+            
+        Returns
+        -------
+        list, list
+            - list of dataframe (1 per fields, all targets of the field in)
+            - list of fields (fieldid)
+            
+        See also
+        --------
+        from_targets_and_survey: laods the instance given targets and a survey
+        """
+        
         if template is None:
             template = targets.template
 
         template_columns = targets.get_template_columns()
 
-        #targets_data = targets.data.copy() if not inplace else targets.data
         dfieldids_ = survey.radec_to_fieldid(targets.data[["ra","dec"]])
         # merge conserves the dtypes of fieldids, not join.
         targets_data = targets.data.merge(dfieldids_, left_index=True, right_index=True)
-
+        if len(targets_data) == 0: # no field containing this target
+            return None, None
 
         # index them per fieldids names.
         target_indexed = targets_data.reset_index().set_index(["index"]+survey.fieldids.names)
         
         # best performance when passing by one groupby calls rather than indexing and xs()
-        gsurvey_indexed = survey.data[["mjd","band","skynoise","gain", "zp"]+survey.fieldids.names].groupby(survey.fieldids.names)
+        gsurvey_indexed = survey.data[["mjd","band","skynoise","gain", "zp"]+survey.fieldids.names
+                                     ].groupby(survey.fieldids.names)
 
         # get list of 
         # This works for any size of fieldids
         names = survey.fieldids.names
         levels = np.arange(1, len(names)+1).tolist()
         if len(levels)==1:
             levels = levels[0] # single index dataframe
 
         fieldids_indexes = target_indexed.groupby(level=levels).size().index
         if nfirst is not None:
             fieldids_indexes = fieldids_indexes[:nfirst]
-        print(f"{len(fieldids_indexes)} field combinations")
+            
         
         # Build a LC for a given index
-        def realize_index_lc(index_):
+        def get_index_lc_input(index_):
             """ """
             try:
-                this_survey = gsurvey_indexed.get_group(index_).copy()#survey_indexed.xs(index_)[["mjd","band","skynoise","gain", "zp"]]
+                this_survey = gsurvey_indexed.get_group(index_).copy()
+                #survey_indexed.xs(index_)[["mjd","band","skynoise","gain", "zp"]]
             except:
                 # no observations for this fieldids 
                 return None
 
             # get() returns copy
-            sncosmo_model = template.get(**template_prop)  
+            sncosmo_model = template.get(**template_prop)
             # survey matching the input fieldids row
 
             # Taking the data we need
-            this_target = target_indexed.xs(index_, level=levels)[template_columns]
-            
-            # Get the lightcurves
-            this_lc = get_obsdata(sncosmo_model, this_survey, this_target)
-            this_lc[names] = index_
+            this_target = target_indexed.xs(index_, level=levels)[template_columns].copy()
+            return sncosmo_model, this_survey, this_target
 
-            return this_lc
+        data = [get_index_lc_input(index_) for index_ in fieldids_indexes]
+        if client is not None:
+            big_future = client.scatter(data) # scatter data
+            futures_ = client.map(_get_obsdata_, big_future)
+            lc_out = client.gather(futures_)
+        else:
+            lc_out = [_get_obsdata_(data_) for data_ in data if data_ is not None]
+
+        return lc_out, fieldids_indexes
 
-        lc_out = [realize_index_lc(index_) for index_ in fieldids_indexes]
-        return pandas.concat(lc_out)
-    
     # ============== #
     #   Properties   #
     # ============== #
     @property
     def data(self):
         """ """
         return self._data
-    
+
     @property
     def targets(self):
         """ """
         return self._targets
-    
+
     @property
     def survey(self):
         """ """
         return self._survey
-        
+
     @property
     def obs_index(self):
         """ index of the observed target """
         if not hasattr(self,"_obs_index") or self._obs_index is None:
             self._obs_index = self.data.index.get_level_values(0).unique().sort_values()
-
+            
         return self._obs_index
```

### Comparing `skysurvey-0.3.9/skysurvey/survey/core.py` & `skysurvey-0.4.2/skysurvey/survey/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,32 +19,38 @@
     def __array__(self):
         """ """
         return self.data.__array__()
     
     # ============== #
     #   Methods      #
     # ============== #    
-    def set_data(self, data):
+    def set_data(self, data, lower_precision=True):
         """ set the observing data 
 
         = It is unlikely you need to use that directly. =
 
         Parameters
         ----------
         data: pandas.DataFrame
              observing data. see REQUIRED_COLUMNS for the list of
              required columns.
 
+        lower_precision: bool
+             change the types from 64 to 32 precision when possible.
+
         Returns
         -------
         None
         """
         if data is not None and not np.in1d(self.REQUIRED_COLUMNS, data.columns).all():
             raise ValueError(f"at least one of the following column name if missing {self.REQUIRED_COLUMNS}")
-        
+
+        if lower_precision and data is not None:
+            data = data.astype( {k: str(v).replace("64","32") for k, v in data.dtypes.to_dict().items()})
+            
         self._data = data
         
     # ------------ #
     #   GETTER     #
     # ------------ #
     def get_fieldcoverage(self, incl_zeros=False, fillna=np.NaN,
                           **kwargs):
```

### Comparing `skysurvey-0.3.9/skysurvey/survey/healpix.py` & `skysurvey-0.4.2/skysurvey/survey/healpix.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         """ get the fieldid of the given (list of) coordinates """
         if type(radec) is pandas.DataFrame:
             ra = np.asarray(radec["ra"].values, dtype="float")
             dec = np.asarray(radec["dec"].values, dtype="float")
         else:
             ra, dec = np.asarray(radec).T
             
-        return hp.ang2pix(self.nside, (90 - ra) * np.pi/180, dec * np.pi/180)
+        return hp.ang2pix(self.nside, dec * np.pi/180,  (90 - ra) * np.pi/180)
 
     # ------- #
     #  draw   #
     # ------- #    
     def draw_random(self, size, 
                     bands, mjd_range, skynoise_range,
                     gain_range=1, zp_range=25,
```

### Comparing `skysurvey-0.3.9/skysurvey/survey/polygon.py` & `skysurvey-0.4.2/skysurvey/survey/polygon.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.9/skysurvey/survey/ztf.py` & `skysurvey-0.4.2/skysurvey/survey/ztf.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.9/skysurvey/target/core.py` & `skysurvey-0.4.2/skysurvey/target/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import warnings
 import numpy as np
 import pandas
 import inspect
-from astropy import cosmology
+from astropy import cosmology, time
 from astropy.utils.decorators import classproperty
 
-__all__ = ["Target", "Transient"]
 
 from ..template import Template
 
 
+__all__ = ["Target", "Transient"]
+
+
 class Target( object ):
 
     _KIND = "unknow"
     _TEMPLATE = None
     _MODEL = None # dict config 
     
     # - Cosmo
@@ -58,27 +59,49 @@
             not implemented yet
         """
         raise NotImplementedError("from_setting is not Implemented ")
 
 
     @classmethod
     def from_data(cls, data, template=None):
-        """ """
+        """ loads the instance given existing data. 
+        
+        This means that the model will be ignored as 
+        data will not be generated but input.
+
+        Parameters
+        ----------
+        data: pandas.DataFrame
+            dataframe containing (at least) the template
+            parameters
+
+        template: str, `sncosmo.Source`, `sncosmo.Model` or skysurvey.Template
+            the template source.
+            - str: any sncosmo model name
+
+        Returns
+        -------
+        instance
+        
+        See also
+        --------
+        from_draw: loads the instance from a random draw of targets given the model
+        """
         this = cls()
 
         if template is not None:
-            self.set_template(template)
+            this.set_template(template)
 
-        this._data = data
+        this.set_data(data)
         return this
         
     @classmethod
     def from_draw(cls, size=None, model=None, template=None,
                       zmax=None, tstart=None, tstop=None,
-                      nyears=None,
+                      zmin=0, nyears=None,
                       **kwargs):
         """ loads the instance from a random draw of targets given the model 
 
         Parameters
         ----------
         size: int, None
             number of target you want to sample
@@ -93,21 +116,30 @@
         template_source: str, None
             name of the template (sncosmo.Model(source)). 
             = leave to None if unsure, cls._TEMPLATE used as default =
 
         zmax: float
             maximum redshift to be simulated.
 
-        tstart: float
+        zmin: float
+            minimum redshift to be simulated.
+
+        tstart: float, str
             starting time of the simulation
-            
-        tstop: float
+            - str, this enters Astropy.Time, e.g. '2020-08-24'
+               and got converted into mjd
+            - float: date mjd
+
+        tstop: float, str
             ending time of the simulation
             (if tstart and nyears are both given, tstop will be
             overwritten by ``tstart+365.25*nyears``
+            - str, this enters Astropy.Time, e.g. '2020-08-24'
+               and got converted into mjd
+            - float: date mjd
 
         nyears: float
             if given, nyears will set:
             - size: it will be the number of target expected up to zmax 
             in the given  number of years. 
             This uses get_rate(zmax).
             - tstop: tstart+365.25*nyears
@@ -129,15 +161,15 @@
 
         if template is not None:
             self.set_template(template)
             
         _ = this.draw(size=size, zmax=zmax, tstart=tstart, tstop=tstop,
                       nyears=nyears, **kwargs)
         return this
-    
+        
     # ------------- # 
     #   Template    #
     # ------------- #
     def set_template(self, template):
         """ set the template 
 
         = unlikely you want to set this directly =
@@ -152,21 +184,21 @@
         from_draw: load the instance by a random draw generation.
         from_setting: loads an instance given model parameters
         """
         import sncosmo
         if type(template) is sncosmo.models.Model: # you provided a sncosmo.model.
             template = Template.from_sncosmo_model(template) # let's build a skysurvey.Template
         elif sncosmo.Source in template.__class__.__mro__ or type(template) is str: # you provided a source
-            template = Template.from_sncosmo_source(template) # let's build a skysurvey.Template
+            template = Template.from_sncosmo(template) # let's build a skysurvey.Template
         else:
             pass # assume it's a template.
             
         self._template = template
         
-    def get_template(self, index=None, **kwargs):
+    def get_template(self, index=None, as_model=False, **kwargs):
         """ get a template (sncosmo.Model) 
 
         Parameters
         ----------
         index: int, None
             index of a target (see self.data.index) to set the 
             template parameters to that of the target.
@@ -180,19 +212,23 @@
             an instance of the template (a sncosmo.Model)
 
         See also
         --------
         get_target_template: get a template set to the target parameters.
         get_template_parameters: get the template parameters for the given target
         """
+        from ..template import Template
         if index is not None:
             prop = self.get_template_parameters(index).to_dict()
             kwargs = {**prop, **kwargs}
 
-        return self.template.get(**kwargs)
+        sncosmo_model = self.template.get(**kwargs)
+        if as_model:
+            return sncosmo_model
+        return Template.from_sncosmo(sncosmo_model)
 
     def get_target_template(self, index, **kwargs):
         """ get a template set to the target parameters.
 
         This is a shortcut to 
         ``get_template(index=index, incl_dust=incl_dust, **kwargs)``
 
@@ -213,14 +249,87 @@
         --------
         get_template: get a template instance (sncosmo.Model)
         get_template_parameters: get the template parameters for the given target
 
         """
         return self.get_template(index=index, **kwargs)
 
+    def get_target_flux(self, index, band, phase, zp=None, zpsys=None):
+        """ Flux through the given bandpass(es) at the given time(s).
+
+        Default return value is flux in photons / s / cm^2. If zp and zpsys
+        are given, flux(es) are scaled to the requested zeropoints.
+
+        Parameters
+        ----------
+        index:
+            index of a target (see self.data.index) to set the 
+            template parameters to that of the target.
+
+        band : str or list_like
+            Name(s) of Bandpass(es) in registry.
+
+        phase : float or list_like
+            phase in day
+
+        zp : float or list_like, optional
+            If given, zeropoint to scale flux to (must also supply ``zpsys``).
+            If not given, flux is not scaled.
+
+        zpsys : str or list_like, optional
+            Name of a magnitude system in the registry, specifying the system
+            that ``zp`` is in.
+
+        Returns
+        -------
+        bandflux : float or `~numpy.ndarray`
+            Flux in photons / s /cm^2, unless `zp` and `zpsys` are
+            given, in which case flux is scaled so that it corresponds
+            to the requested zeropoint. Return value is `float` if all
+            input parameters are scalars, `~numpy.ndarray` otherwise.
+        """
+        template = self.get_target_template(index)
+        return template.bandflux(band, template.get('t0')+phase, zp=zp, zpsys=zpsys)
+
+
+    def clone_target_at_redshifts(self, index, redshifts, as_dataframe=False):
+        """ get a clone of the given target at the given redshifts.
+        This: 
+        (1) copies the index entries, 
+        (2) sets the redshift to the input values
+        (3) redraw the model starting from the redshift (creating a new dataframe)
+        (4, optional) sets a new instance with the updated dataframe
+        
+
+        Parameters
+        ----------
+        index: 
+            index of a target (see self.data.index)
+
+        redshift: list, array
+            new redshifts to clone this target to
+
+        as_dataframe: bool
+            should this return the created new dataframe (True)
+            or a new instance (False)
+
+        Returns
+        -------
+        instance or DataFrame
+        """
+        dd = self.data.loc[index].to_frame().T
+        dd.loc[index, "z"] = redshifts
+        dd = dd.explode("z")
+        dd["z"] = dd["z"].astype(float)
+        data = self.model.redraw_from("z", dd, incl_name=False)
+        if as_dataframe:
+            return data
+        
+        return self.__class__.from_data(data)
+    
     # -------------- #
     #   Getter       #
     # -------------- #
     def get_template_parameters(self, index=None):
         """ get the template parameters for the given target 
         
         This method selects from self.data the parameters that actually
@@ -254,14 +363,79 @@
         """ get the data columns that are template parameters 
         
         Returns
         -------
         pandas.columns
         """
         return self.data.columns[np.in1d(self.data.columns, self.template_parameters)]
+
+
+    # -------------- #
+    #   Apply        #
+    # -------------- #
+    def apply_noise(self, error_model, relat_err=0.01):
+        """ returns a DataFrame corresponding to self.data affected by the noise given in error_model.
+        
+        *Careful*: Only parameters explicitly mentioned in the input error_model will be changed. 
+        This could breaks the natural connection between DAG parameters. 
+        e.g. if magobs is changed, this does not automatically update x0.
+
+        Parameters
+        ----------
+        error_model: dict, DataFrame or ModelDAG
+            error model that will be applied to the data. The keys must correspond.
+            several input format are accepted. 
+            The error_model keys must correspond to the data keys to be affected.
+            - dict: assumed to be an input of a ModelDAG.
+            - ModelDAG: uses draw to generate the dataframe
+            - dataframe: keys must correspond to self.data keys to be affected.
+
+        relat_err: float or None
+            if given, the stored parameters error will randomly drawn (gaussian)
+            around the true input error with a scale corresponding to
+            true_err * relat_err.
+
+        Returns
+        -------
+        DataFrame:
+            self.data with all matching columns from error_model changed {param}.
+            {param}_err columns will be added.
+            
+            
+        Example
+        -------
+        Say you want to affect 'magobs' with a random gaussian noise of 
+        1 +/- 0.1.
+        ```
+        error_model = {'magobs': {"model": np.random.normal, "param": {'loc':1, 'scale':0.1}}}
+        ```
+        With that, the 'magobs' columns with be changed and a magobs_err created. 
+        """
+        from ..dag import ModelDAG
+        if type(error_model) is dict: # assumed to be a model's input
+            error_model = ModelDAG(error_model).draw( len(self.data) )
+        elif type(error_model) is ModelDAG: # assumed to be a model
+            error_model = error_model.draw( len(self.data) )
+        # else: dataframe
+        
+        data_ = self.data.copy()
+        colums = data_.columns[np.in1d(data_.columns, error_model.columns)]
+        
+        
+        for column in colums:
+            err_true = error_model[column]
+            data_[column] = np.random.normal(loc=data_[column], scale=err_true)
+            if relat_err is not None and relat_err>0:
+                err_eff = np.random.normal(loc=err_true, scale=err_true*relat_err)
+            else:
+                err_eff = err_true
+                
+            data_[f"{column}_err"] = err_eff
+            
+        return data_
         
     # -------------- #
     #   Converts     #
     # -------------- #
     def magabs_to_magobs(self, z, magabs, cosmology=None):
         """ converts absolute magnitude into observed magnitude 
         given the (cosmological) redshift and a cosmology 
@@ -375,14 +549,41 @@
         from ..dag import ModelDAG
         if type( model ) is dict:
             from copy import deepcopy
             model = ModelDAG(deepcopy(model), self)
             
         
         self._model = model
+
+
+    def set_data(self, data, incl_template=True):
+        """ attach data  to this instance. 
+
+        Parameters
+        ----------
+        data: pandas.DataFrame
+            dataframe containing (at least) the template
+            parameters
+
+        incl_template: bool
+            if data does not contain the template column
+            should this add it ?
+
+        Return
+        ------
+        None
+        """
+        if "template" not in data and incl_template:
+            if self.template is None:
+                templatename = "unknown"
+            else:
+                templatename = self.template_source.name
+            data["template"] = templatename
+
+        self._data = data
         
     def get_model(self, **kwargs):
         """ get a copy of the model (dict) 
 
         You can change the model you get (not the current model)
         using the kwargs. 
 
@@ -443,15 +644,16 @@
         """
         _ = self.model.change_model(**kwargs)
         
     # -------------- #
     #   Plotter      #
     # -------------- #
     def show_scatter(self, xkey, ykey, ckey=None, ax=None, fig=None, 
-                     index=None, data=None):
+                         index=None, data=None, colorbar=True,
+                         **kwargs):
         """ """
         import matplotlib.pyplot as plt
 
         # ------- #
         #  Data   #
         # ------- #
         if data is None:
@@ -469,35 +671,42 @@
                 import matplotlib.pyplot as plt
                 fig = plt.figure(figsize=[7,4])
             ax = fig.add_subplot(111)
         else:
             fig = ax.figure
 
 
-        ax.scatter(xvalue, yvalue, c=cvalue)
+        sc = ax.scatter(xvalue, yvalue, c=cvalue, **kwargs)
+        if cvalue is not None and colorbar:
+            fig.colorbar(sc, ax=ax)
+            
         return fig
             
     # =============== #
     #   Draw Methods  #
     # =============== #
     def draw(self, size=None,
-                 zmax=None, tstart=None, tstop=None,
+                 zmax=None, zmin=0,
+                 tstart=None, tstop=None,
                  nyears=None,
                  inplace=True, **kwargs):
         """ draws the parameter model (using self.model.draw() 
 
         Parameters
         ----------
         size: int
             = ignored is nyears is not None =
             number of target you want to draw.
 
         zmax: float
             maximum redshift to be simulated.
 
+        zmin: float
+            minimum redshift to be simulated.
+
         tstart: float
             starting time of the simulation
             
         tstop: float
             ending time of the simulation
             (if tstart and nyears are both given, tstop will be
             overwritten by ``tstart+365.25*nyears``
@@ -514,40 +723,61 @@
 
         Returns
         -------
         DataFrame
             the simulated dataframe.
 
         """
+        
         # short cut 
         # -> change the redshift
         if zmax is not None:
             kwargs.setdefault("redshift",{}).update({"zmax": zmax})
             
         elif nyears is not None:
             zmax = self.get_model_parameter("redshift", "zmax", None)
+
+        if zmin is not None and "redshift" in self.model.model:
+            kwargs.setdefault("redshift",{}).update({"zmin": zmin})
             
+        elif nyears is not None:
+            zmin = self.get_model_parameter("redshift", "zmin", None)
+
         if tstop is not None:
+            if type( tstop ) is str:
+                tstop = time.Time(tstop).mjd
+
             kwargs.setdefault("t0",{}).update({"high": tstop})
             
+        # time range:        
         if tstart is not None:
+            if type( tstart ) is str:
+                tstart = time.Time(tstart).mjd
+                
             kwargs.setdefault("t0",{}).update({"low": tstart})
+            if tstop is None and nyears is None: # do 1 year by default
+                kwargs.setdefault("t0",{}).update({"high": tstart+365.25})
+        # tstart is None, then what ?
         elif tstop is not None and nyears is not None:
-            tstart = tstop - 365.25*nyears # fixed later
+            tstart = tstop - 365.25*nyears # fixed later            
         elif nyears is not None:
             tstart = self.get_model_parameter("t0", "low", None)
 
         if nyears is not None:
-            print(zmax)
+            rate_min = self.get_rate(zmin) if (zmin is not None and zmin >0) else 0
             kwargs.setdefault("t0",{}).update({"low": tstart, "high": tstart + 365.25*nyears})
-            size = int(self.get_rate(zmax) * nyears)
+            size = int((self.get_rate(zmax)-rate_min) * nyears)
+            
 
+        # actually draw the data
         data = self.model.draw(size=size, **kwargs)
         if inplace:
-            self._data = data
+            # lower precision
+            data = data.astype( {k: str(v).replace("64","32") for k, v in data.dtypes.to_dict().items()})
+            self.set_data(data)
             
         return data
 
     # ============== #
     #   Properties   #
     # ============== #  
     @classproperty
@@ -723,46 +953,43 @@
                                           **kwargs)
 
     # ------------ #
     #  Model       #
     # ------------ #    
     def magobs_to_amplitude(self, magobs, band="bessellb", zpsys="ab", param_name="amplitude"):
         """ """
-        template = self.get_template()
-        m_current = template._source.peakmag(band,zpsys)
+        template = self.get_template(as_model=True)
+        m_current = template._source.peakmag(band, zpsys)
         return 10.**(0.4 * (m_current - magobs)) * template.get(param_name)
 
     def draw_redshift(self, zmax, zmin=0, zstep=1e-3, size=None):
         """ based on the rate (see get_rate()) """
         xx = np.arange(zmin, zmax, zstep)
         pdf = self.getpdf_redshift(xx)
         return np.random.choice(np.mean([xx[1:],xx[:-1]], axis=0), 
                       size=size, p=pdf/pdf.sum())
             
     # ------------ #
     #  Show LC     #
     # ------------ #
-    def show_lightcurve(self, band, index=None, params=None,
+    def show_lightcurve(self, band, index, params=None,
                             ax=None, fig=None, colors=None,
                             time_range=[-20,50], npoints=500,
                             zp=25, zpsys="ab",
                             format_time=True, t0_format="mjd", 
                             in_mag=False, invert_mag=True, **kwargs):
         """ 
         params: None or dict
         """
         # get the template
         if params is None:
             params = {}
             
-        if index is not None:
-            prop = self.get_template_parameters(index).to_dict()
-            params = {**prop, **params}
-
-        return self.template.show_lightcurve(band, params=params,
+        template = self.get_target_template(index, **params)
+        return template.show_lightcurve(band, params=params,
                                              ax=ax, fig=fig, colors=colors,
                                              time_range=time_range, npoints=npoints,
                                              zp=zp, zpsys=zpsys,
                                              format_time=format_time,
                                              t0_format=t0_format, 
                                              in_mag=in_mag, invert_mag=invert_mag,
                                              **kwargs)
```

### Comparing `skysurvey-0.3.9/skysurvey/target/snia.py` & `skysurvey-0.4.2/skysurvey/target/snia.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,42 +9,55 @@
 
 # ================== #
 #                    #
 # Pre-Defined models #
 #                    #
 # ================== #
 class SNeIaColor( object ):
-    
+
     @staticmethod
     def intrinsic_and_dust(xx="-0.3:1:0.01", cint=-0.05, sigmaint=0.05, tau=0.1):
         """ exponential decay convolved with and intrinsic gaussian color distribution.
 
         Parameters
         ----------
-        
+        xx: str
+            the x-axis of the color distribution. It should be a string with the
+            format "min:max:step". The default is "-0.3:1:0.01".
+            inputs np.r_[xx]
+
+        cint: float
+            the mean of the intrinsic color distribution. The default is -0.05.
+
+        sigmaint: float
+            the standard deviation of the intrinsic color distribution. The default is 0.05.
+
+        tau: float
+            the decay constant of the dust distribution. The default is 0.1.
+
         Returns
         -------
         2d-array:
            xx, pdf
         """
         if type(xx) == str: # assumed r_ input
             xx = eval(f"np.r_[{xx}]")
 
         from scipy import stats
         from scipy.ndimage import gaussian_filter1d
-        # exponential decay center on cint            
+        # exponential decay center on cint
         expon = stats.expon.pdf(xx, loc=-0.05, scale=0.1)
-        # applying gaussian filtering        
+        # applying gaussian filtering
         #  - which require sigmaint in pixel.
         sigmaint_inpix = sigmaint/(xx[1]-xx[0]) # assuming constant step
         pdf = gaussian_filter1d(expon, sigmaint_inpix)
-        
+
         return xx, pdf
 
-    
+
 class SNeIaStretch( object ):
 
     @staticmethod
     def nicolas2021( xx="-4:4:0.05", 
                      mu1=0.33, sigma1=0.64, 
                      mu2=-1.50, sigma2=0.58, a=0.45,
                      redshift=None, fprompt=0.5):
@@ -249,15 +262,15 @@
                             },
                            
                    magobs = {"model": "magabs_to_magobs", # defined in Target (mother of Transients)
                              "input": ["z", "magabs"]},
 
                    x0 = {"model": "magobs_to_amplitude", # defined in Transients
                          "input": ["magobs"],
-                         "param": {"param_name":"x0"}}, #because it needs to call sncosmo_model.get(param_name)
+                         "param": {"param_name": "x0"}}, #because it needs to call sncosmo_model.get(param_name)
                        
                    radec = {"model": "random",
                             "param": dict(ra_range=[0, 360], dec_range=[-30, 90]),
                             "as": ["ra","dec"]}
                     )
```

### Comparing `skysurvey-0.3.9/skysurvey/target/stars.py` & `skysurvey-0.4.2/skysurvey/target/stars.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 
 import numpy as np
 from .core import Target
 
 
 
-class Star( Target ):
 
-    _KIND = "star"
+class StableTarget( Target ):
+    
+    _KIND = "stable"
     _MODEL = dict( radec = {"model":"random",
                                 "param":dict(ra_range=[0, 360], dec_range=[-30, 90]),
                                 "as":["ra","dec"]},
                     magobs = {"model": "random_magobs",
-                                "param": dict(zpmax=22.5)}
+                                "param": dict(zpmax=22.5)},
                    )
     
     @staticmethod
     def random_magobs(size=None, zpmax=22.5, scale=3):
         """ """
         exp_decay = np.random.exponential(scale=scale, size=size)
         return zpmax-exp_decay
+
+    
+class Star( StableTarget ):
+
+    _KIND = "star"
+
```

### Comparing `skysurvey-0.3.9/skysurvey/template.py` & `skysurvey-0.4.2/skysurvey/template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,57 @@
 """ core template tools """
 
 import os
 import numpy as np
 import pandas
 import sncosmo
+from sncosmo.models import _SOURCES
 
 from astropy.utils.decorators import classproperty
 
-__all__ = ["get_sncosmo_model", "Template"]
+__all__ = ["get_sncosmo_model", "Template",
+           "get_sncosmo_sourcenames"]
+
+
+
+SNCOSMO_SOURCES_DF = pandas.DataFrame(_SOURCES.get_loaders_metadata())
+def get_sncosmo_sourcenames(of_type=None, startswith=None, endswith=None):
+    """ get the list of available sncosmo source names
+
+    Parameters
+    ----------
+    of_type: str, list
+        type name (of list of). e.g SN II
+
+    startswith: str
+        the source name should start by this (e.g. v19)
+
+    endswith: str
+        the source name should end by this
+
+    Returns
+    -------
+    list
+        list of names
+
+    """
+    sources = SNCOSMO_SOURCES_DF.copy()
+    if of_type is not None:
+        typenames = sources[sources["type"].isin(np.atleast_1d(of_type))]["name"]
+    else:
+        typenames = sources["name"]
+        
+    if endswith is not None:
+        typenames = typenames[typenames.str.startswith(startswith)]
+    
+    if endswith is not None:
+        typenames = typenames[typenames.str.endswith(endswith)]
+
+    return list(typenames)
+
 
 def get_sncosmo_model(source="salt2",
                              incl_dust=True, 
                              **params):
     """ get the template (sncosmo.Model)
 
     Parameters
@@ -30,15 +70,15 @@
     Returns
     -------
     `sncosmo.Model`
         the sncosmo.Model template
     """
     modelprop = dict(source=source)
     if incl_dust:
-        dust  = sncosmo.CCM89Dust()
+        dust = sncosmo.CCM89Dust()
         modelprop["effects"] = [dust]
         modelprop["effect_names"]=['mw']
         modelprop["effect_frames"]=['obs']
         
     model = sncosmo.Model(**modelprop)
     model.set(**params)
     return model      
@@ -75,17 +115,17 @@
 #                 #
 # =============== #
 class Template( object ):
 
     def __init__(self, sncosmo_model):
         """ """
         self._sncosmo_model = sncosmo_model
-
+        
     @classmethod
-    def from_sncosmo_source(cls, source, incl_dust=True, **kwargs):
+    def from_sncosmo(cls, source, incl_dust=True, **kwargs):
         """ 
         loads the instance given the source name.
 
         Parameters
         ----------
         source : `~sncosmo.Source` or str
             The model for the spectral evolution of the source. If a string
@@ -94,24 +134,23 @@
 
         **kwargs goes to ``get_sncosmo_model(source, **kwargs)``
 
         Returns
         -------
         instance
         """
-        # useless for now but I may change things in init.
-        sncosmo_model = get_sncosmo_model(source, incl_dust=incl_dust,
+        if type(source) != sncosmo.Model:
+            # useless for now but I may change things in init.
+            sncosmo_model = get_sncosmo_model(source, incl_dust=incl_dust,
                                           **kwargs)
+        else:
+            sncosmo_model = source
+            
         return cls(sncosmo_model)
-    
-    @classmethod
-    def from_sncosmo_model(cls, model):
-        """ """
-        return cls(model)
-    
+        
     # ============== #
     #   Methods      #
     # ============== #
     # -------- #
     #  GETTER  #
     # -------- #
     def get(self,**kwargs):
@@ -188,16 +227,15 @@
         if not np.any(sel):
             warnings.warn("no wavelength matched [def range {wmin}, {wmax}], given. {lbdas} ")
 
         flux = np.zeros_like(lbdas)
         if as_phase:
             time += sncosmo_model.get("t0")
         
-        flux[sel] = sncosmo_model.flux(time, lbdas[sel])
-        print(flux[sel])     
+        flux[sel] = sncosmo_model.flux(time, lbdas[sel])  
         return flux
 
     
     # -------- #
     # Plotter  #
     # -------- #
     def show_spectum(self, time, lbdas, params={},
@@ -376,15 +414,15 @@
 class GridTemplate( Template ):
 
     _GRID_OF = None
     
     @staticmethod
     def _read_single_file(filename, sncosmo_source):
         source = sncosmo_source.from_filename(filename)
-        return Template.from_sncosmo_source(source)
+        return Template.from_sncosmo(source)
     
     @classmethod
     def from_filenames(cls, filenames, refindex=0, grid_of=None):
         """ """
         if grid_of is None:
             grid_of = cls.grid_of
```

### Comparing `skysurvey-0.3.9/skysurvey.egg-info/SOURCES.txt` & `skysurvey-0.4.2/skysurvey.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 skysurvey/survey/polygon.py
 skysurvey/survey/ztf.py
 skysurvey/target/__init__.py
 skysurvey/target/collection.py
 skysurvey/target/core.py
 skysurvey/target/environments.py
 skysurvey/target/kilonova.py
+skysurvey/target/sncc.py
 skysurvey/target/snia.py
-skysurvey/target/snii.py
 skysurvey/target/stars.py
 skysurvey/target/timeserie.py
```

