# Comparing `tmp/bhad-0.0.9.tar.gz` & `tmp/bhad-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhad-0.0.9.tar", last modified: Mon Apr  3 11:32:27 2023, max compression
+gzip compressed data, was "bhad-0.1.0.tar", last modified: Tue May 30 09:22:10 2023, max compression
```

## Comparing `bhad-0.0.9.tar` & `bhad-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alexv84   (1000) alexv84   (1000)        0 2023-04-03 11:32:27.129639 bhad-0.0.9/
--rw-rw-r--   0 alexv84   (1000) alexv84   (1000)     2656 2023-04-03 11:32:27.129639 bhad-0.0.9/PKG-INFO
--rw-rw-r--   0 alexv84   (1000) alexv84   (1000)     2132 2023-04-03 10:36:09.000000 bhad-0.0.9/README.md
--rw-rw-r--   0 alexv84   (1000) alexv84   (1000)       38 2023-04-03 11:32:27.129639 bhad-0.0.9/setup.cfg
--rw-rw-r--   0 alexv84   (1000) alexv84   (1000)     1791 2023-04-03 11:29:00.000000 bhad-0.0.9/setup.py
-drwxrwxr-x   0 alexv84   (1000) alexv84   (1000)        0 2023-04-03 11:32:27.129639 bhad-0.0.9/src/
-drwxrwxr-x   0 alexv84   (1000) alexv84   (1000)        0 2023-04-03 11:32:27.129639 bhad-0.0.9/src/bhad/
--rw-rw-r--   0 alexv84   (1000) alexv84   (1000)        0 2023-04-03 10:36:09.000000 bhad-0.0.9/src/bhad/__init__.py
--rw-rw-r--   0 alexv84   (1000) alexv84   (1000)    13722 2023-04-03 10:36:09.000000 bhad-0.0.9/src/bhad/explainer.py
--rw-rw-r--   0 alexv84   (1000) alexv84   (1000)    12053 2023-04-03 10:36:09.000000 bhad-0.0.9/src/bhad/model.py
--rw-rw-r--   0 alexv84   (1000) alexv84   (1000)    26902 2023-04-03 10:36:09.000000 bhad-0.0.9/src/bhad/utils.py
-drwxrwxr-x   0 alexv84   (1000) alexv84   (1000)        0 2023-04-03 11:32:27.129639 bhad-0.0.9/src/bhad.egg-info/
--rw-rw-r--   0 alexv84   (1000) alexv84   (1000)     2656 2023-04-03 11:32:27.000000 bhad-0.0.9/src/bhad.egg-info/PKG-INFO
--rw-rw-r--   0 alexv84   (1000) alexv84   (1000)      266 2023-04-03 11:32:27.000000 bhad-0.0.9/src/bhad.egg-info/SOURCES.txt
--rw-rw-r--   0 alexv84   (1000) alexv84   (1000)        1 2023-04-03 11:32:27.000000 bhad-0.0.9/src/bhad.egg-info/dependency_links.txt
--rw-rw-r--   0 alexv84   (1000) alexv84   (1000)      116 2023-04-03 11:32:27.000000 bhad-0.0.9/src/bhad.egg-info/requires.txt
--rw-rw-r--   0 alexv84   (1000) alexv84   (1000)        5 2023-04-03 11:32:27.000000 bhad-0.0.9/src/bhad.egg-info/top_level.txt
+drwxrwxr-x   0 alexv84   (1000) alexv84   (1000)        0 2023-05-30 09:22:10.930239 bhad-0.1.0/
+-rw-rw-r--   0 alexv84   (1000) alexv84   (1000)     2675 2023-05-30 09:22:10.930239 bhad-0.1.0/PKG-INFO
+-rw-rw-r--   0 alexv84   (1000) alexv84   (1000)     2152 2023-05-23 20:19:05.000000 bhad-0.1.0/README.md
+-rw-rw-r--   0 alexv84   (1000) alexv84   (1000)       38 2023-05-30 09:22:10.930239 bhad-0.1.0/setup.cfg
+-rw-rw-r--   0 alexv84   (1000) alexv84   (1000)     1791 2023-05-30 09:12:45.000000 bhad-0.1.0/setup.py
+drwxrwxr-x   0 alexv84   (1000) alexv84   (1000)        0 2023-05-30 09:22:10.926239 bhad-0.1.0/src/
+drwxrwxr-x   0 alexv84   (1000) alexv84   (1000)        0 2023-05-30 09:22:10.926239 bhad-0.1.0/src/bhad/
+-rw-rw-r--   0 alexv84   (1000) alexv84   (1000)        0 2023-04-03 10:36:09.000000 bhad-0.1.0/src/bhad/__init__.py
+-rw-rw-r--   0 alexv84   (1000) alexv84   (1000)    13722 2023-04-03 10:36:09.000000 bhad-0.1.0/src/bhad/explainer.py
+-rw-rw-r--   0 alexv84   (1000) alexv84   (1000)    12044 2023-05-30 08:58:12.000000 bhad-0.1.0/src/bhad/model.py
+-rw-rw-r--   0 alexv84   (1000) alexv84   (1000)    28813 2023-05-30 08:58:12.000000 bhad-0.1.0/src/bhad/utils.py
+drwxrwxr-x   0 alexv84   (1000) alexv84   (1000)        0 2023-05-30 09:22:10.930239 bhad-0.1.0/src/bhad.egg-info/
+-rw-rw-r--   0 alexv84   (1000) alexv84   (1000)     2675 2023-05-30 09:22:10.000000 bhad-0.1.0/src/bhad.egg-info/PKG-INFO
+-rw-rw-r--   0 alexv84   (1000) alexv84   (1000)      266 2023-05-30 09:22:10.000000 bhad-0.1.0/src/bhad.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexv84   (1000) alexv84   (1000)        1 2023-05-30 09:22:10.000000 bhad-0.1.0/src/bhad.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexv84   (1000) alexv84   (1000)      116 2023-05-30 09:22:10.000000 bhad-0.1.0/src/bhad.egg-info/requires.txt
+-rw-rw-r--   0 alexv84   (1000) alexv84   (1000)        5 2023-05-30 09:22:10.000000 bhad-0.1.0/src/bhad.egg-info/top_level.txt
```

### Comparing `bhad-0.0.9/PKG-INFO` & `bhad-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: bhad
-Version: 0.0.9
+Version: 0.1.0
 Summary: Bayesian Histogram-based Anomaly Detection
 Home-page: https://github.com/AVoss84/bhad
 Author: Alexander Vosseler
 Maintainer: Alexander Vosseler
 Keywords: bayesian-inference,anomaly-detection,unsupervised-learning,explainability
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: interactive
 
 # Bayesian Histogram-based Anomaly Detection (BHAD)
 
-Python implementation of the BHAD algorithm as presented in [Vosseler, A. (2022): Unsupervised Insurance Fraud Prediction Based on Anomaly Detector Ensembles, Risks, 10(7), 132](https://www.mdpi.com/2227-9091/10/7/132) and [Vosseler, A. (2022): BHAD: Fast unsupervised anomaly detection using Bayesian histograms](https://www.researchgate.net/publication/364265660_BHAD_Fast_unsupervised_anomaly_detection_using_Bayesian_histograms). The code follows scikit-learn's standard API for [outlier detection](https://scikit-learn.org/stable/modules/outlier_detection.html). 
+Python implementation of the BHAD algorithm as presented in [Vosseler, A. (2023): BHAD: Explainable anomaly detection using Bayesian histograms](https://www.researchgate.net/publication/364265660_BHAD_Fast_unsupervised_anomaly_detection_using_Bayesian_histograms). The ***bhad* package** follows Scikit-learn's standard API for [outlier detection](https://scikit-learn.org/stable/modules/outlier_detection.html). 
+<!--- The *bhad* package has been presented on *PyCon DE & PyData Berlin 2023*, you can watch the presentation [here](https://vimeo.com/user/171811262/folder/15825490). --> 
 
 ## Installation
 
 ```bash
 pip install bhad
 ```
```

### Comparing `bhad-0.0.9/README.md` & `bhad-0.1.0/src/bhad.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,26 @@
+Metadata-Version: 2.1
+Name: bhad
+Version: 0.1.0
+Summary: Bayesian Histogram-based Anomaly Detection
+Home-page: https://github.com/AVoss84/bhad
+Author: Alexander Vosseler
+Maintainer: Alexander Vosseler
+Keywords: bayesian-inference,anomaly-detection,unsupervised-learning,explainability
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: interactive
+
 # Bayesian Histogram-based Anomaly Detection (BHAD)
 
-Python implementation of the BHAD algorithm as presented in [Vosseler, A. (2022): Unsupervised Insurance Fraud Prediction Based on Anomaly Detector Ensembles, Risks, 10(7), 132](https://www.mdpi.com/2227-9091/10/7/132) and [Vosseler, A. (2022): BHAD: Fast unsupervised anomaly detection using Bayesian histograms](https://www.researchgate.net/publication/364265660_BHAD_Fast_unsupervised_anomaly_detection_using_Bayesian_histograms). The code follows scikit-learn's standard API for [outlier detection](https://scikit-learn.org/stable/modules/outlier_detection.html). 
+Python implementation of the BHAD algorithm as presented in [Vosseler, A. (2023): BHAD: Explainable anomaly detection using Bayesian histograms](https://www.researchgate.net/publication/364265660_BHAD_Fast_unsupervised_anomaly_detection_using_Bayesian_histograms). The ***bhad* package** follows Scikit-learn's standard API for [outlier detection](https://scikit-learn.org/stable/modules/outlier_detection.html). 
+<!--- The *bhad* package has been presented on *PyCon DE & PyData Berlin 2023*, you can watch the presentation [here](https://vimeo.com/user/171811262/folder/15825490). --> 
 
 ## Installation
 
 ```bash
 pip install bhad
 ```
 
@@ -44,8 +60,8 @@
 local_expl = Explainer(pipe.named_steps['model'], pipe.named_steps['discrete']).fit()
 
 local_expl.get_explanation(nof_feat_expl = 5, append = False)   # individual explanations
 
 local_expl.global_feat_imp                                      # global explanation
 ```
 
-A detailed toy example using synthetic data for anomaly detection can be found [here](https://github.com/AVoss84/bhad/blob/main/src/notebooks/Toy_Example.ipynb) and an example using the Titanic dataset illustrating model explanability can be found [here](https://github.com/AVoss84/bhad/blob/main/src/notebooks/Titanic_Example.ipynb).
+A detailed toy example using synthetic data for anomaly detection can be found [here](https://github.com/AVoss84/bhad/blob/main/src/notebooks/Toy_Example.ipynb) and an example using the Titanic dataset illustrating model explanability can be found [here](https://github.com/AVoss84/bhad/blob/main/src/notebooks/Titanic_Example.ipynb).
```

### Comparing `bhad-0.0.9/setup.py` & `bhad-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name='bhad',                            # This is the name of the package-distribution (as shown on pypi)
-    version='0.0.9',                               # The release version
+    version='0.1.0',                               # The release version
     author="Alexander Vosseler",                   # Full name of the author
     maintainer = "Alexander Vosseler",
     url='https://github.com/AVoss84/bhad',
     description="Bayesian Histogram-based Anomaly Detection",
     long_description=long_description,             # Long description read from the the readme file
     long_description_content_type="text/markdown",
     keywords = ["bayesian-inference", "anomaly-detection", "unsupervised-learning", "explainability"],
```

### Comparing `bhad-0.0.9/src/bhad/explainer.py` & `bhad-0.1.0/src/bhad/explainer.py`

 * *Files identical despite different names*

### Comparing `bhad-0.0.9/src/bhad/model.py` & `bhad-0.1.0/src/bhad/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import (List, Optional, Union)
-from copy import deepcopy
+#from copy import deepcopy
 import warnings
 import pandas as pd
 import numpy as np
 from sklearn.base import BaseEstimator, OutlierMixin
 from sklearn.preprocessing import OneHotEncoder
 import bhad.utils as utils
 
@@ -58,15 +58,15 @@
         return: scores
         """  
         assert isinstance(X, pd.DataFrame), 'X must be of type pd.DataFrame'
         selected_col = X.columns[~X.columns.isin(self.exclude_col)] 
         if len(self.exclude_col)>0:
                 print("Features",self.exclude_col, 'excluded.')  
             
-        df = deepcopy(X[selected_col].astype(object)) 
+        df = X[selected_col].astype(object).copy() 
         self.df_shape = df.shape  
         self.columns = df.select_dtypes(include=['object', 'category']).columns.tolist()  # use only categorical (including discretized numerical)
         if len(self.columns)!= self.df_shape[1] : 
                 warnings.warn('Not all features in X are categorical!!')
         self.df = df
         
         # Apply one-hot encoder to categorical -> sparse dummy matrix
@@ -77,15 +77,15 @@
         self.df_one = self.enc.fit_transform(df).toarray()   
         assert all(np.sum(self.df_one, axis=1) == df.shape[1]), 'Row sums must be equal to number of features!!'
         if self.verbose : 
             print("Matrix dimension after one-hot encoding:", self.df_one.shape)  
         self.columns_onehot_ = self.enc.get_feature_names_out()
         
         # Prior parameters and sufficient statistics:
-        #----------------------------------------------
+        #---------------------------------------------
         self.alphas = np.array([self.alpha]*self.df_one.shape[1])           # Dirichlet concentration parameters; aka pseudo counts
         self.freq = self.df_one.sum(axis=0)                                 # suff. statistics of multinomial likelihood
         self.log_pred = np.log((self.alphas + self.freq)/np.sum(self.alphas + self.freq))  # log posterior predictive probabilities for single trial / multinoulli
 
         # Duplicate list of marg. freq. in an array for elementwise multiplication  
         # i.e. Repeat counts for each obs. i =1...n
         #---------------------------------------------------------------------------   
@@ -164,15 +164,15 @@
         scores : numpy.array, shape (n_samples,)
             The outlier score of the input samples centered arount threshold 
             value.
         """
         if self.verbose : 
             print("\nScore input data.")
             print("Apply fitted one-hot encoder.")        
-        df = deepcopy(X)    
+        df = X.copy()    
         self.df_one = self.enc_.transform(df).toarray()     # apply fitted one-hot encoder to categorical -> sparse dummy matrix
         assert all(np.sum(self.df_one, axis=1) == df.shape[1]), 'Row sums must be equal to number of features!!'
         
         # Update suff. stat with abs. freq. of new data points/levels
         self.freq_updated_ = self.freq_ + self.df_one.sum(axis=0)      
         #freq_updated = np.log(np.exp(self.freq) + self.df_one + alpha)    # multinomial-dirichlet
         
@@ -180,15 +180,15 @@
         self.log_pred = np.log((self.alphas + self.freq_updated_)/np.sum(self.alphas + self.freq_updated_))   
         self.f_mat = self.freq_updated_ * self.df_one           # get level specific counts for X, e.g. test set
         f_mat_bayes = self.log_pred * self.df_one  
         self.scores = pd.Series(np.apply_along_axis(np.sum, 1, f_mat_bayes), index=X.index) 
 
         # If you already have it from fit then just output it:
         if hasattr(self, 'X_') and X.equals(self.X_):    
-            self.f_mat = deepcopy(self.f_mat_)    # current f_mat (here based on X_train)
+            self.f_mat = self.f_mat_.copy()    # current f_mat (here based on X_train)
             return self.scores_
         else:    
             return self.scores
     
     
     def decision_function(self, X : pd.DataFrame) -> np.array:
         """
```

### Comparing `bhad-0.0.9/src/bhad/utils.py` & `bhad-0.1.0/src/bhad/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-import os, sys, warnings, functools, math, time
-from typing import (List, Tuple)
+import os, warnings, functools, time
+from functools import wraps
+from typing import List, Tuple, Dict
 import numpy as np
 import pandas as pd
 from pandas.api.types import CategoricalDtype
-from sklearn.base import BaseEstimator, OutlierMixin, TransformerMixin
+from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_is_fitted
 #from sklearn.preprocessing import OneHotEncoder
 from scipy.special import loggamma
 from scipy.integrate import simpson
 from scipy.sparse import csr_matrix
 from scipy.stats import wishart, bernoulli, norm
 #from scipy.stats import t as student
 from scipy.optimize import minimize_scalar
 #from math import floor, ceil
-from copy import deepcopy
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d import Axes3D
-from functools import wraps
-from tqdm.auto import tqdm   
+#from tqdm.auto import tqdm   
 
 
 # timer decorator for any function func:
 def timer(func):
     """Print the runtime of the decorated function"""
     @wraps(func)
     def wrapper_timer(*args, **kwargs):
@@ -98,14 +97,35 @@
             if self.verbose : 
                 warnings.warn("'\nNote: lower != 0 not supported currently, will be set to None!'")
             self.lower = None 
     
     def __del__(self):
         class_name = self.__class__.__name__
         #print(class_name, "destroyed")
+
+    def __repr__(self):
+        return f"Discretize(columns = {self.columns}, nbins = {self.nof_bins}, lower = {self.lower}, k = {self.k}, round_intervals = {self.round_intervals}, eps = {self.eps}, make_labels = {self.make_labels}, prior_gamma = {self.prior_gamma}, prior_max_M = {self.prior_max_M}, verbose = {self.verbose})"
+    
+    def log_post_pmf_nof_bins(self, feature_values : np.array)-> Dict[int, float]:
+        """
+        Evaluate log posterior prob. measure of number of bins (over grid of supported values)
+        see paper section 'posteriors'.
+
+        Args:
+            feature_values (np.array): univariate variable values
+
+        Returns:
+            Dict[int, float]: grid of number of bin values with log-pmf values
+        """
+        # 'Integrate out' out hyperparameter gamma from joint prior via Simpson's rule:
+        log_marg_prior_nbins = {m : np.log(1e-10 + simpson(np.array([geometric_prior(M = m, gamma = g, max_M = self.prior_max_M, log = False) for g in self.gamma_grid]), self.gamma_grid)) for m in range(1, self.prior_max_M, 1)}
+        
+        # Evaluate log posterior prob. measure of number of bins (over grid of supported values):
+        return {m : log_marg_prior_nbins[m] + log_marglike_nbins(M = m, y = feature_values) for m in range(1,self.prior_max_M, 1)}
+
     
     #@timer
     def fit(self, X : pd.DataFrame)-> 'Discretize':
         
             assert isinstance(X, pd.DataFrame), 'Input X must be pandas dataframe!'
             # Set a maximum number of bins [1,max_M]:
             if self.prior_max_M is None:
@@ -116,47 +136,44 @@
                 if self.verbose:
                     print(f"Setting maximum number of bins {self.prior_max_M }.")
 
             if X.index[0] != 0:    
                 X.reset_index(drop=True, inplace=True)     # Need this to conform with 0...n-1 index in explainer and elsewhere 
                 if self.verbose: 
                     print("Resetting index of input dataframe.")    
-            df_new = deepcopy(X)
+            df_new = X.copy()
             self.nbins = self.nof_bins    # initialize (might be changed in case of low variance features) 
             self.cat_columns = df_new.select_dtypes(include=['object','category']).columns.tolist()  # categorical (for later reference in postproc.)
             if not self.columns:
                 self.columns = df_new.select_dtypes(include=[np.number, 'float', 'int']).columns.tolist()    # numeric features only
 
             if self.verbose:
                 print(f"Input shape: {X.shape}")
                 print(f"Used {len(self.columns)} numeric feature(s) and {len(self.cat_columns)} categorical feature(s).")      
 
             df_new[self.columns] = df_new[self.columns].astype(float)        
-            ptive_inf = float ('inf')
-            ntive_inf = float('-inf')
-            self.df_orig = deepcopy(df_new[self.columns + self.cat_columns])   # train data with non-discretized values for numeric features for model explainer
+            ptive_inf, ntive_inf = float ('inf'), float('-inf')
+            self.df_orig = df_new[self.columns + self.cat_columns].copy()   # train data with non-discretized values for numeric features for model explainer
 
             for col in self.columns:
                     v = df_new[col].values       # values of feature col
                     #---------------------------------------------------
                     # Determine optimal number of bins per feature
                     # using its Bayesian Maximum A-Posteriori estimate: 
                     #---------------------------------------------------
                     if self.nof_bins is None:
                         if self.verbose : 
                             print("Determining optimal number of bins for numeric features")
                         #print(f'FD rule: {freedman_diaconis(v)}')
                         #print(f'Sturges: {1 + ceil(np.log2(len(v)))}')
                         
-                        # Evaluate log joint posterior of grid of number of bin values:
-                        #---------------------------------------------------------------
-                        log_marg_prior_nbins = {m : np.log(1e-10 + simpson(np.array([geometric_prior(M = m, gamma = g, max_M = self.prior_max_M, log = False) for g in self.gamma_grid]), self.gamma_grid)) for m in range(1, self.prior_max_M, 1)}
-                        
-                        lpr = {m : log_marg_prior_nbins[m] + log_marglike_nbins(M = m, y = v) for m in range(1,self.prior_max_M, 1)}
-                      
+                        # Evaluate log posterior prob. measure of number of bins:
+                        #---------------------------------------------------------
+                        lpr = self.log_post_pmf_nof_bins(feature_values = v)
+
                         # Compute K_MAP for each feature:
                         #---------------------------------
                         self.nbins = max(lpr, key=lpr.get)    
                         if self.verbose: 
                             print('Feature {} using {} bins'.format(col, self.nbins))
                     
                     # Add some low variance white noise 
@@ -177,23 +194,24 @@
                     if self.lower is None:
                       bounds = np.linspace(min(v)-self.k*np.std(v), max(v)+self.k*np.std(v), num = self.nbins+1)  
                       bs, labels = [], ['0']    # add -Inf as lower bound
                     else:
                       bounds = np.linspace(self.lower, max(v)+self.k*np.std(v), num = self.nbins+1)
                       bs, labels = [],[]
 
-                    bs = [(bounds[i], bounds[i+1]) for i in range(len(bounds)-1)]    
+                    bs = [(bounds[i], bounds[i+1]) for i in range(len(bounds)-1)]   
 
                     # Add +Inf as upper bound    
                     #--------------------------
                     bs.insert(len(bs),(bounds[len(bounds)-1], ptive_inf))   
                     
                     # Add -Inf as lower bound    
                     #--------------------------
-                    if self.lower is None: bs[0] = (ntive_inf, bs[0][1]) 
+                    if self.lower is None: 
+                        bs[0] = (ntive_inf, bs[0][1]) 
                       
                     # Make left closed [..) interval to be save in cases like: [0,..)
                     #--------------------------------------------------------------------
                     my_bins = pd.IntervalIndex.from_tuples(bs, closed='left')   
                     self.save_binnings[col] = my_bins
                     assert (self.nbins + 1) == len(set(my_bins)), 'Your created bins in '+str(col)+' are not unique my_bins!'
                     x = pd.cut(v, bins = my_bins, duplicates = "drop", include_lowest = True)
@@ -202,61 +220,62 @@
                     df_new[col] = x.astype(object)
                     #self.counts_binned[col] = df_new[col].value_counts()
                     if self.nof_bins is not None: 
                         self.nbins = self.nof_bins             # resetting nbins, in case of zero variance features...
 
             # Tag as fitted for sklearn compatibility: 
             # https://scikit-learn.org/stable/developers/develop.html#estimated-attributes
-            self.X_ = deepcopy(df_new)
+            self.X_ = df_new.copy()
             self.columns_ = self.columns
             self.nbins_ = self.nbins 
             self.xindex_fitted_ = df_new.index
             self.save_binnings_ = self.save_binnings 
             #self.counts_binned_ = self.counts_binned 
             self.lower_ = self.lower 
             self.k_ = self.k 
             self.eps_ = self.eps 
             self.make_labels_ = self.make_labels 
-            self.df_orig_ = deepcopy(self.df_orig)
+            self.df_orig_ = self.df_orig.copy()
             if self.verbose and (self.nof_bins is not None): 
                 print("Binned continous features into", self.nbins,"bins.")
             return self
     
     #@timer
     def transform(self, X : pd.DataFrame)-> pd.DataFrame:
         
         if X.index[0] != 0:    
             X.reset_index(drop=True, inplace=True)     # Need this to conform with 0...n-1 index in explainer and elsewhere 
             if self.verbose: 
                print("Reseting index of input dataframe.")    
 
-        df_new = deepcopy(X)
+        df_new = X.copy()
         self.cat_columns = df_new.select_dtypes(include=['object', 'category']).columns.tolist()  # categorical (for later reference in postproc.)
         numerical_columns = df_new.select_dtypes(include=[np.number, 'float', 'int']).columns.tolist()    # numeric features only
 
         # Check if columns in X and X_train are compatible:
         for col in numerical_columns: 
             assert col in self.columns_, 'Column {} not among loaded X_train columns!'.format(col)
         df_new[self.columns_] = df_new[self.columns_].astype(float)   
 
         # Update & Keep for model explainer
-        self.df_orig = deepcopy(df_new[self.columns_ + self.cat_columns])  
+        self.df_orig = df_new[self.columns_ + self.cat_columns].copy()  
 
         # if you already have it from fit then just output it
         if hasattr(self, 'X_') and (len(self.xindex_fitted_) == X.shape[0]):
             return self.X_
 
         # Map new values to discrete training buckets/bins: 
-        for ind, row in df_new.iterrows(): 
+        for row in df_new.itertuples():
+            ind = row.Index
             row_values = []
             try:
                 for c in self.columns_:
                     bin_c = self.save_binnings_[c]
-                    if ~np.isnan(row[c]):
-                        row_values.append(list(bin_c[bin_c.contains(row[c])])[0])
+                    if ~np.isnan(getattr(row, c)):
+                        row_values.append(list(bin_c[bin_c.contains(getattr(row, c))])[0])
                     else:
                         row_values.append(np.nan)    
                 df_new.loc[ind, self.columns_] = row_values
             except Exception as ex:
                 print(ex)        
         return df_new
 
@@ -285,31 +304,39 @@
         datrng = datmax - datmin
         result = int((datrng / bw) + 1)
     return result
 
 
 def log_marglike_nbins(M : int, y : np.array)-> float:
     """
-    Log posterior of number of bins M
+    Log-posterior of number of bins M
     using conjugate Jeffreys' prior for the bin probabilities 
-    and a flat improper prior for the number of bins. This is therefore equivalent to the marginal
-    log-likelihood of the number of bins  
+    and a flat improper prior for the number of bins. 
+    This is therefore equivalent to the marginal log-likelihood 
+    of the number of bins. 
+
+    Args:
+        M (int): number of bins parameter
+        y (np.array): univariate sample data points 
+
+    Returns:
+        float: log posterior probability value
     """
     N = len(y)
     counts, _ = np.histogram(y, bins = np.linspace(min(y), max(y), M+1))   # evenly spaced bins
     post_M = N*np.log(M) + loggamma(M/2) -M*loggamma(1/2) -loggamma(N + M/2) + np.sum(loggamma(counts + 1/2)) 
     return post_M
 
 
 def exp_normalize(x : np.array)-> np.array:
     """Exp-normalize trick
     https://timvieira.github.io/blog/post/2014/02/11/exp-normalize-trick/
 
     Args:
-        x (np.array): _description_
+        x (np.array): sample data points
 
     Returns:
         np.array: Normalized input array
     """
     b = x.max()
     y = np.exp(x - b)
     return y / y.sum()
@@ -338,20 +365,25 @@
 
 # def log_joint_post_nbins_gamma(m : int, gamma : float, y : np.array, max_M : int = 100)-> float:
 #     """
 #     Log joint posterior of number of bins M and gamma
 #     """  
 #     return log_marglike_nbins(m, y) + geometric_prior(m, gamma, max_M, log = True)
 
-
 def bart_simpson_density(x : np.array, m : int = 4)-> np.array:
     """
     Calculate density of Bart Simpson distr. aka The Claw
     (see Larry Wasserman, All of nonparametric statistics, section 6)
-    m: number of mixture components 
+
+    Args:
+        x (np.array): discrete grid over support of the distribution
+        m (int, optional): number of mixture components. Defaults to 4.
+
+    Returns:
+        np.array: density values
     """
     mix = 0
     for j in range(m+1):
         mix += norm.pdf(x, loc=(j/2)-1, scale=0.1)
     return 0.5*norm.pdf(x, loc=0, scale=1) + 0.1*mix
 
 
@@ -362,15 +394,15 @@
     """
     return bart_simpson_density(x, m = 4) / norm.pdf(x, loc=0, scale=1)    # target/proposal  
 
 
 def rbartsim(MCsim : int = 10**4, seed : int = None, verbose : bool = True)-> np.array:
     """
     Sample from Bart Simpson density via Accept-Reject algorithm, 
-    see for example Robert, Casella
+    see e.g. Robert, Casella
     """
     if seed: 
         np.random.seed(seed) 
     result = minimize_scalar(lambda t: -accratio(t))    # maximize function
     M = -result.fun 
     u = np.random.uniform(0,1,size=MCsim)
     x = np.random.normal(0,1,size=MCsim)    # candidate draws
@@ -385,15 +417,15 @@
 class mvt2mixture:
     
     def __init__(self, thetas : dict = {'mean1' : None, 'mean2' : None, \
                                'Sigma1' : None, 'Sigma2' : None, \
                                'nu1': None, 'nu2': None}, seed : int = None, gaussian : bool = False, **figure_param):
         """
         Multivariate 2-component Student-t mixture random generator. 
-        Direct random sampling via using the Student-t representation as a continous scale mixture distr.   
+        Direct random sampling using the Student-t representation as a continous scale mixture distr.   
         -------
         Input:
         -------
         thetas: Component-wise parameters; note that Sigma1,2 are the scale matrices of the 
                 Wishart priors of the precision matrices of the Student-t's.
         gaussian: boolean, generate from Gaussian mixture if True, otherwise from Student-t    
         seed: set seed for rng.
@@ -490,68 +522,81 @@
         self.kwargs = kwargs
         self.exclude_col = exclude_columns
         self.prefix_sep_ = prefix_sep
         self.verbose = verbose
         self.unique_categories_, self.value2name_ = dict(), dict()
         if self.verbose : 
             print("One-hot encoding categorical features.")
+        
+    def __repr__(self):
+        return f"onehot_encoder(exclude_columns = {self.exclude_col}, prefix_sep = {self.prefix_sep_}, oos_token = {self.oos_token_}, verbose = {self.verbose})"
 
     #@timer
     def fit(self, X: pd.DataFrame)-> 'onehot_encoder':
 
         self.selected_col = X.columns[~X.columns.isin(self.exclude_col)] 
         if self.exclude_col:
             print("Features",self.exclude_col, 'excluded.')  
-        df = deepcopy(X[self.selected_col])
+        df = X[self.selected_col].copy()
+        df.columns = [str(c) for c in df.columns]    # force columns to strings
+
         for z, var in enumerate(df.columns):         # loop over columns
             self.unique_categories_[var] = df[var].unique().tolist()
             # Add 'Unknown/Others' bucket to levels for unseen levels:
             df[var] = df[var].astype(CategoricalDtype(self.unique_categories_[var] + [self.oos_token_]))    # add unknown catgory for out of sample levels
             one = pd.get_dummies(df[var], prefix_sep = self.prefix_sep_, prefix=var, **self.kwargs)
             if z>0:
                dummy = pd.concat([dummy, one], axis=1, sort=False)
             else:
-               dummy = deepcopy(one)
+               dummy = one.copy()
 
             # Leave out the 'OTHERS'/oos_token_ buckets here for consistency:
             self.value2name_[var] = {level_orig:dummy_name for level_orig, dummy_name in zip(self.unique_categories_[var], list(one.columns)[:-1])}
 
         self.dummyX_ = dummy         
         self.columns_ = list(self.dummyX_.columns) # all final column names in sparse dummy matrix
         self.names2index_ = {dummy_names:z for z, dummy_names in enumerate(self.columns_)} 
         self.X_ = df
         return self    
 
     #@timer
     def transform(self, X: pd.DataFrame)-> csr_matrix:
-        
+        """Map X values to respective bins and encode as one-hot
+
+        Args:
+            X (pd.DataFrame): Discretized/Binned input dataframe
+
+        Returns:
+            csr_matrix: Dummy/One-hot matrix
+        """
         check_is_fitted(self)        # Check if fit had been called
+
         self.selected_col = X.columns[~X.columns.isin(self.exclude_col)]
 
         # If you already have it from fit then just output it
         if hasattr(self, 'X_') and self.X_.equals(X):
             return self.dummyX_
  
-        df = deepcopy(X[self.selected_col])
-        ohm = np.zeros((df.shape[0],len(self.columns_)))
-        for r, my_tuple in enumerate(df.itertuples(index=False)):    # loop over rows
-            my_index = []
-            for z, col in enumerate(df.columns):
-                raw_level_list = list(self.value2name_[col].keys())
-                mask = my_tuple[z] == np.array(raw_level_list)
-                if any(mask): 
-                    index = np.where(mask)[0][0]
-                    dummy_name = self.value2name_[col][raw_level_list[index]]
-                else:
-                    dummy_name = col + self.prefix_sep_ + self.oos_token_
-                my_index.append(self.names2index_[dummy_name])
-            targets = np.array(my_index).reshape(-1)
-            ohm[r,targets] = 1    
-        return csr_matrix(ohm) 
-        
+        df = X[self.selected_col].copy()
+        df.columns = [str(c) for c in df.columns]    # force columns to strings
+        ohm = np.zeros((df.shape[0], len(self.columns_)))
+
+        for col in df.columns:
+            raw_level_list = np.array(list(self.value2name_[col].keys()))   # take advantage of vectorized operations
+            mask = np.isin(df[col].values, raw_level_list)        # use vectorized operations 
+
+            binned_values = df[col].values 
+            oos_dummy_name = col + self.prefix_sep_ + self.oos_token_
+            # set 'Others' category in case no overlap of input interval with train set intervals ('bins')
+            dummy_names = np.array([self.value2name_[col][binned_values[z]] if m else oos_dummy_name for z, m in zip(np.arange(len(mask)), mask)])
+            
+            my_index = np.array([self.names2index_[dummy_name] for dummy_name in dummy_names])
+            ohm[np.arange(df.shape[0]), my_index] = 1      
+        return csr_matrix(ohm)   
+
 
     def get_feature_names_out(self, input_features : list = None)-> np.array: 
         """
         Get feature names as used in one-hot encoder, 
         i.e. after binning/disretizing
 
         Returns:
@@ -559,15 +604,15 @@
         """
         check_is_fitted(self)
 
         if input_features is None:
             input_features = self.selected_col
         self.dummy_names, self.dummy_names_index, self.dummy_names_by_feat = [], {}, {}
         for col_name in input_features:
-            mask = [col_name+self.prefix_sep_ in col for col in self.columns_]
+            mask = [str(col_name)+self.prefix_sep_ in col for col in self.columns_]
             if any(mask):
                 index = np.where(np.array(mask))[0]
                 self.dummy_names_index[col_name] = index
                 full_dummy_names_feat = np.array(self.columns_)[index].tolist()
                 # Remove separator from pandas get_dummy to retrieve original bin names from discretize fct.:
                 # Note: self.prefix_sep_ = '__' must be kept here!
                 dummy_name_2_orig_val = [item.split('__')[1] for item in full_dummy_names_feat] #{item: item.split('__')[1] for item in full_dummy_names_feat}
```

### Comparing `bhad-0.0.9/src/bhad.egg-info/PKG-INFO` & `bhad-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,11 @@
-Metadata-Version: 2.1
-Name: bhad
-Version: 0.0.9
-Summary: Bayesian Histogram-based Anomaly Detection
-Home-page: https://github.com/AVoss84/bhad
-Author: Alexander Vosseler
-Maintainer: Alexander Vosseler
-Keywords: bayesian-inference,anomaly-detection,unsupervised-learning,explainability
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: interactive
-
 # Bayesian Histogram-based Anomaly Detection (BHAD)
 
-Python implementation of the BHAD algorithm as presented in [Vosseler, A. (2022): Unsupervised Insurance Fraud Prediction Based on Anomaly Detector Ensembles, Risks, 10(7), 132](https://www.mdpi.com/2227-9091/10/7/132) and [Vosseler, A. (2022): BHAD: Fast unsupervised anomaly detection using Bayesian histograms](https://www.researchgate.net/publication/364265660_BHAD_Fast_unsupervised_anomaly_detection_using_Bayesian_histograms). The code follows scikit-learn's standard API for [outlier detection](https://scikit-learn.org/stable/modules/outlier_detection.html). 
+Python implementation of the BHAD algorithm as presented in [Vosseler, A. (2023): BHAD: Explainable anomaly detection using Bayesian histograms](https://www.researchgate.net/publication/364265660_BHAD_Fast_unsupervised_anomaly_detection_using_Bayesian_histograms). The ***bhad* package** follows Scikit-learn's standard API for [outlier detection](https://scikit-learn.org/stable/modules/outlier_detection.html). 
+<!--- The *bhad* package has been presented on *PyCon DE & PyData Berlin 2023*, you can watch the presentation [here](https://vimeo.com/user/171811262/folder/15825490). --> 
 
 ## Installation
 
 ```bash
 pip install bhad
 ```
```

