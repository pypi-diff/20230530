# Comparing `tmp/gaspery-0.2.0.tar.gz` & `tmp/gaspery-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaspery-0.2.0.tar", last modified: Tue Mar 28 05:27:09 2023, max compression
+gzip compressed data, was "gaspery-0.2.1.tar", last modified: Tue May 30 00:36:20 2023, max compression
```

## Comparing `gaspery-0.2.0.tar` & `gaspery-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 chrislam   (501) staff       (20)        0 2023-03-28 05:27:09.173482 gaspery-0.2.0/
--rw-r--r--   0 chrislam   (501) staff       (20)     1075 2022-12-19 20:13:42.000000 gaspery-0.2.0/LICENSE
--rw-r--r--   0 chrislam   (501) staff       (20)     3789 2023-03-28 05:27:09.173315 gaspery-0.2.0/PKG-INFO
--rw-r--r--   0 chrislam   (501) staff       (20)     3224 2023-01-26 16:15:09.000000 gaspery-0.2.0/README.md
--rw-r--r--   0 chrislam   (501) staff       (20)      600 2023-03-28 05:25:01.000000 gaspery-0.2.0/pyproject.toml
--rw-r--r--   0 chrislam   (501) staff       (20)       38 2023-03-28 05:27:09.173525 gaspery-0.2.0/setup.cfg
--rw-r--r--   0 chrislam   (501) staff       (20)      433 2023-03-28 05:24:46.000000 gaspery-0.2.0/setup.py
-drwxr-xr-x   0 chrislam   (501) staff       (20)        0 2023-03-28 05:27:09.170234 gaspery-0.2.0/src/
-drwxr-xr-x   0 chrislam   (501) staff       (20)        0 2023-03-28 05:27:09.172357 gaspery-0.2.0/src/gaspery/
--rw-r--r--   0 chrislam   (501) staff       (20)      307 2022-12-23 20:26:13.000000 gaspery-0.2.0/src/gaspery/__init__.py
--rw-r--r--   0 chrislam   (501) staff       (20)    10923 2023-03-14 17:56:37.000000 gaspery-0.2.0/src/gaspery/calculate_fi.py
--rw-r--r--   0 chrislam   (501) staff       (20)    16038 2023-03-28 00:23:19.000000 gaspery-0.2.0/src/gaspery/strategies.py
--rw-r--r--   0 chrislam   (501) staff       (20)     1409 2023-02-16 18:12:29.000000 gaspery-0.2.0/src/gaspery/utils.py
-drwxr-xr-x   0 chrislam   (501) staff       (20)        0 2023-03-28 05:27:09.173131 gaspery-0.2.0/src/gaspery.egg-info/
--rw-r--r--   0 chrislam   (501) staff       (20)     3789 2023-03-28 05:27:09.000000 gaspery-0.2.0/src/gaspery.egg-info/PKG-INFO
--rw-r--r--   0 chrislam   (501) staff       (20)      280 2023-03-28 05:27:09.000000 gaspery-0.2.0/src/gaspery.egg-info/SOURCES.txt
--rw-r--r--   0 chrislam   (501) staff       (20)        1 2023-03-28 05:27:09.000000 gaspery-0.2.0/src/gaspery.egg-info/dependency_links.txt
--rw-r--r--   0 chrislam   (501) staff       (20)        8 2023-03-28 05:27:09.000000 gaspery-0.2.0/src/gaspery.egg-info/top_level.txt
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-30 00:36:20.785873 gaspery-0.2.1/
+-rw-r--r--   0 chris      (501) staff       (20)     1075 2023-04-08 21:45:04.000000 gaspery-0.2.1/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)     4226 2023-05-30 00:36:20.785187 gaspery-0.2.1/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     3661 2023-04-08 21:45:04.000000 gaspery-0.2.1/README.md
+-rw-r--r--   0 chris      (501) staff       (20)      600 2023-05-30 00:36:01.000000 gaspery-0.2.1/pyproject.toml
+-rw-r--r--   0 chris      (501) staff       (20)       38 2023-05-30 00:36:20.786271 gaspery-0.2.1/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)      433 2023-05-30 00:35:50.000000 gaspery-0.2.1/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-30 00:36:20.775098 gaspery-0.2.1/src/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-30 00:36:20.779580 gaspery-0.2.1/src/gaspery/
+-rw-r--r--   0 chris      (501) staff       (20)      307 2023-04-08 21:45:05.000000 gaspery-0.2.1/src/gaspery/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    10860 2023-04-09 21:20:17.000000 gaspery-0.2.1/src/gaspery/calculate_fi.py
+-rw-r--r--   0 chris      (501) staff       (20)    16325 2023-05-29 19:30:41.000000 gaspery-0.2.1/src/gaspery/strategies.py
+-rw-r--r--   0 chris      (501) staff       (20)     1345 2023-04-09 21:21:27.000000 gaspery-0.2.1/src/gaspery/utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-30 00:36:20.784462 gaspery-0.2.1/src/gaspery.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     4226 2023-05-30 00:36:20.000000 gaspery-0.2.1/src/gaspery.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      280 2023-05-30 00:36:20.000000 gaspery-0.2.1/src/gaspery.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-30 00:36:20.000000 gaspery-0.2.1/src/gaspery.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)        8 2023-05-30 00:36:20.000000 gaspery-0.2.1/src/gaspery.egg-info/top_level.txt
```

### Comparing `gaspery-0.2.0/LICENSE` & `gaspery-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gaspery-0.2.0/PKG-INFO` & `gaspery-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: gaspery
-Version: 0.2.0
-Summary: Fisher Information-based radial velocity observation scheduling
-Author: Chris Lam
-Author-email: Christopher Lam <c.lam@ufl.edu>
-License: MIT License
-Project-URL: Homepage, https://github.com/cl3425/gaspery
-Project-URL: Bug Tracker, https://github.com/cl3425/gaspery/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ### Gaspery (/gas.pər.ee/)
 
 [Pronunciation Guide](https://user-images.githubusercontent.com/16911363/212941685-d887b375-176f-4c23-b011-5f6968028a33.mp4)
 
 Gaspery is a package that uses the Fisher Information Matrix (FIM) to evaluate different radial velocity (RV) observing strategies. A paper (Lam, Bedell & Zhao, in prep) will also follow this work.
 
 The Fisher Information Matrix describes the amount of information a time series contains on each free parameter input in a model. For exoplanet observers, the free parameter of interest is often the RV semi-amplitude, K. Gaspery is intended to help observational exoplanet astronomers construct the observing strategy that maximizes information (or minimizes uncertainty) on K. However, one can maximize information on any free parameter from any model, given a time series support (x-axis). So, whether you want to extend gaspery to deal with more complex models and problems or want integration with different covariance kernels (we are fully integrated with tinygp), we are happy to field your suggestions on this repo's Git Issues!
@@ -45,14 +29,20 @@
 ### Tutorials
 Start here for usecases! 
 
 - min_observations.ipynb: Given a target, I want to find the minimum number of observations required to reach some threshold for the uncertainty on the RV semi-amplitude, K.
 
 - fixed_budget.ipynb: Given a target AND a fixed allocation of observations, how do I best spend these observing nights to minimize the uncertainty on K? 
 
+- beat_frequencies.ipynb: Given a host star, how do various combinations of planet orbital period and observing cadence interact to produce "beat frequencies" (contours of bad information content due to aliasing)?
+
+- companions.ipynb: Fixed budget, but with more than one planet in a system!
+
+- custom_kernels.ipynb: What if I want to swap out the quasi-periodic Gaussian Process kernel for something more specific to my science case? 
+
 
 ### Src/gaspery
 Source code for the gaspery package.
 
 
 ### Notebooks
 These are where the functions in src/gaspery/ were developed and tested, as well as where figures were made for proposals, presentations, and the paper.
```

### Comparing `gaspery-0.2.0/README.md` & `gaspery-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: gaspery
+Version: 0.2.1
+Summary: Fisher Information-based radial velocity observation scheduling
+Author: Chris Lam
+Author-email: Christopher Lam <c.lam@ufl.edu>
+License: MIT License
+Project-URL: Homepage, https://github.com/cl3425/gaspery
+Project-URL: Bug Tracker, https://github.com/cl3425/gaspery/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ### Gaspery (/gas.pər.ee/)
 
 [Pronunciation Guide](https://user-images.githubusercontent.com/16911363/212941685-d887b375-176f-4c23-b011-5f6968028a33.mp4)
 
 Gaspery is a package that uses the Fisher Information Matrix (FIM) to evaluate different radial velocity (RV) observing strategies. A paper (Lam, Bedell & Zhao, in prep) will also follow this work.
 
 The Fisher Information Matrix describes the amount of information a time series contains on each free parameter input in a model. For exoplanet observers, the free parameter of interest is often the RV semi-amplitude, K. Gaspery is intended to help observational exoplanet astronomers construct the observing strategy that maximizes information (or minimizes uncertainty) on K. However, one can maximize information on any free parameter from any model, given a time series support (x-axis). So, whether you want to extend gaspery to deal with more complex models and problems or want integration with different covariance kernels (we are fully integrated with tinygp), we are happy to field your suggestions on this repo's Git Issues!
@@ -29,14 +45,20 @@
 ### Tutorials
 Start here for usecases! 
 
 - min_observations.ipynb: Given a target, I want to find the minimum number of observations required to reach some threshold for the uncertainty on the RV semi-amplitude, K.
 
 - fixed_budget.ipynb: Given a target AND a fixed allocation of observations, how do I best spend these observing nights to minimize the uncertainty on K? 
 
+- beat_frequencies.ipynb: Given a host star, how do various combinations of planet orbital period and observing cadence interact to produce "beat frequencies" (contours of bad information content due to aliasing)?
+
+- companions.ipynb: Fixed budget, but with more than one planet in a system!
+
+- custom_kernels.ipynb: What if I want to swap out the quasi-periodic Gaussian Process kernel for something more specific to my science case? 
+
 
 ### Src/gaspery
 Source code for the gaspery package.
 
 
 ### Notebooks
 These are where the functions in src/gaspery/ were developed and tested, as well as where figures were made for proposals, presentations, and the paper.
```

### Comparing `gaspery-0.2.0/pyproject.toml` & `gaspery-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaspery"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Christopher Lam", email="c.lam@ufl.edu" },
 ]
 description = "Fisher Information-based radial velocity observation scheduling"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `gaspery-0.2.0/src/gaspery/calculate_fi.py` & `gaspery-0.2.1/src/gaspery/calculate_fi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import numpy as np 
 import scipy
 import pandas as pd
 import random
 from itertools import chain
-import exoplanet
 import astropy 
-import pymc3
-import pymc3_ext
-import celerite2
 from tinygp import kernels, GaussianProcess
 from numpy.linalg import inv, det, solve, cond
 from tqdm import tqdm
 
 import matplotlib.pyplot as plt
 import matplotlib
 
@@ -336,8 +332,8 @@
     rv1 = -K1 * jnp.sin(arg1)
     
     arg2 = (2*jnp.pi/P2)*(t-T0_2)
     rv2 = -K2 * jnp.sin(arg2)
 
     rv_total = rv1 + rv2
     
-    return rv_total
+    return rv_total
```

### Comparing `gaspery-0.2.0/src/gaspery/strategies.py` & `gaspery-0.2.1/src/gaspery/strategies.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import numpy as np 
 import scipy
 import pandas as pd
 import random
-import exoplanet
 import astropy 
-import pymc3
-import pymc3_ext
-import celerite2
 from numpy.linalg import inv, det, solve, cond
 from tqdm import tqdm
 
 import matplotlib.pyplot as plt
 import matplotlib
 
 import jax
@@ -355,21 +351,26 @@
         if twice_flag==False:
 
             while len(strat) < n_obs:
                 
                 # on block
                 for i in range(on):
 
+                    add = True
                     # check if in any off day
                     if len(offs) > 0:
                         for custom_off in offs:
-                            if ~((curr >= custom_off[0]) & (curr <= custom_off[1])):
-                                if len(strat) < n_obs:
-                                    strat.append(curr)
-                                    break
+                            
+                            # if so, tag to don't include
+                            if ((curr >= custom_off[0]) & (curr <= custom_off[1])):
+                                add = False
+
+                        if add == True:
+                            if len(strat) < n_obs:
+                                strat.append(curr)
 
                     elif len(offs) == 0:
                         strat.append(curr)
 
                     curr += 1
 
                 # off block
@@ -379,33 +380,41 @@
         elif twice_flag==True:
 
             while len(strat) < n_obs:
                 
                 # on block
                 for i in range(on):
 
+                    add = True
                     if len(offs) > 0: # if there are manual offs
 
                         # check if in any off day
                         for custom_off in offs:
-                            if ~((curr >= custom_off[0]) & (curr <= custom_off[1])):
-                                if len(strat) < n_obs:
-                                    strat.append(curr)
-                                    break
+
+                            # if so, tag to don't include
+                            if ((curr >= custom_off[0]) & (curr <= custom_off[1])):
+                                add = False
+
+                        if add == True:
+                            if len(strat) < n_obs:
+                                strat.append(curr)
+                                    
                         try:
                             curr += hours/24
                         except NameError:
                             print("If you turn on the twice_flag, you need to set hours=N, where N is the number of hours between observations in the same night.")
 
                         # observe for the second time that night
                         for custom_off in offs:
-                            if ~((curr >= custom_off[0]) & (curr <= custom_off[1])):
-                                if len(strat) < n_obs:
-                                    strat.append(curr)
-                                    break
+                            if ((curr >= custom_off[0]) & (curr <= custom_off[1])):
+                                add = False
+
+                        if add == True:    
+                            if len(strat) < n_obs:
+                                strat.append(curr)
                                 
                         # cycle back to same time of night the next day
                         curr += (24-hours)/24
 
                     elif len(offs) == 0:
                         strat.append(curr)
                         curr += (24-hours)/24
```

### Comparing `gaspery-0.2.0/src/gaspery/utils.py` & `gaspery-0.2.1/src/gaspery/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import numpy as np 
 import scipy
 import pandas as pd
 import random
-import exoplanet
 import astropy 
-import pymc3
-import pymc3_ext
-import celerite2
 from numpy.linalg import inv, det, solve, cond
 from tqdm import tqdm
 
 import matplotlib.pyplot as plt
 import matplotlib
 
 import jax
```

### Comparing `gaspery-0.2.0/src/gaspery.egg-info/PKG-INFO` & `gaspery-0.2.1/src/gaspery.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaspery
-Version: 0.2.0
+Version: 0.2.1
 Summary: Fisher Information-based radial velocity observation scheduling
 Author: Chris Lam
 Author-email: Christopher Lam <c.lam@ufl.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/cl3425/gaspery
 Project-URL: Bug Tracker, https://github.com/cl3425/gaspery/issues
 Classifier: Programming Language :: Python :: 3
@@ -45,14 +45,20 @@
 ### Tutorials
 Start here for usecases! 
 
 - min_observations.ipynb: Given a target, I want to find the minimum number of observations required to reach some threshold for the uncertainty on the RV semi-amplitude, K.
 
 - fixed_budget.ipynb: Given a target AND a fixed allocation of observations, how do I best spend these observing nights to minimize the uncertainty on K? 
 
+- beat_frequencies.ipynb: Given a host star, how do various combinations of planet orbital period and observing cadence interact to produce "beat frequencies" (contours of bad information content due to aliasing)?
+
+- companions.ipynb: Fixed budget, but with more than one planet in a system!
+
+- custom_kernels.ipynb: What if I want to swap out the quasi-periodic Gaussian Process kernel for something more specific to my science case? 
+
 
 ### Src/gaspery
 Source code for the gaspery package.
 
 
 ### Notebooks
 These are where the functions in src/gaspery/ were developed and tested, as well as where figures were made for proposals, presentations, and the paper.
```

