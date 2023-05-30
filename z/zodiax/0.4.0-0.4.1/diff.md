# Comparing `tmp/zodiax-0.4.0.tar.gz` & `tmp/zodiax-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodiax-0.4.0.tar", last modified: Sun May  7 07:19:14 2023, max compression
+gzip compressed data, was "zodiax-0.4.1.tar", last modified: Tue May 30 03:28:18 2023, max compression
```

## Comparing `zodiax-0.4.0.tar` & `zodiax-0.4.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 07:19:14.322545 zodiax-0.4.0/
--rw-r--r--   0 louis      (501) staff       (20)       70 2022-11-14 06:22:13.000000 zodiax-0.4.0/.gitignore
--rw-r--r--   0 louis      (501) staff       (20)     1523 2022-11-14 06:12:01.000000 zodiax-0.4.0/LICENSE
--rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-14 11:44:43.000000 zodiax-0.4.0/MANIFEST.ini
--rw-r--r--   0 louis      (501) staff       (20)      488 2023-05-07 07:19:14.322402 zodiax-0.4.0/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     4291 2023-04-11 08:47:45.000000 zodiax-0.4.0/README.md
--rw-r--r--   0 louis      (501) staff       (20)     3030 2023-05-07 07:18:07.000000 zodiax-0.4.0/mkdocs.yml
--rw-r--r--   0 louis      (501) staff       (20)       55 2023-03-09 09:55:10.000000 zodiax-0.4.0/requirements.txt
--rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-07 07:19:14.322586 zodiax-0.4.0/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)     1508 2023-04-11 07:58:40.000000 zodiax-0.4.0/setup.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 07:19:14.319600 zodiax-0.4.0/tests/
--rw-r--r--   0 louis      (501) staff       (20)     3956 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_base.py
--rw-r--r--   0 louis      (501) staff       (20)     1667 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_bayes.py
--rw-r--r--   0 louis      (501) staff       (20)      655 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_eqx.py
--rw-r--r--   0 louis      (501) staff       (20)      332 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_jit.py
--rw-r--r--   0 louis      (501) staff       (20)      630 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_optimisation.py
--rw-r--r--   0 louis      (501) staff       (20)      666 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_serialisation.py
--rw-r--r--   0 louis      (501) staff       (20)      453 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_tree.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 07:19:14.320354 zodiax-0.4.0/zodiax/
--rw-r--r--   0 louis      (501) staff       (20)      472 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)    17880 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/base.py
--rw-r--r--   0 louis      (501) staff       (20)    12793 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/bayes.py
--rw-r--r--   0 louis      (501) staff       (20)     5711 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/eqx.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 07:19:14.322187 zodiax-0.4.0/zodiax/experimental/
--rw-r--r--   0 louis      (501) staff       (20)      238 2023-05-04 01:45:02.000000 zodiax-0.4.0/zodiax/experimental/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     1927 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/experimental/jit.py
--rw-r--r--   0 louis      (501) staff       (20)    17318 2023-04-11 08:47:45.000000 zodiax-0.4.0/zodiax/experimental/serialisation.py
--rw-r--r--   0 louis      (501) staff       (20)     2323 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/optimisation.py
--rw-r--r--   0 louis      (501) staff       (20)     2461 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/tree.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 07:19:14.321484 zodiax-0.4.0/zodiax.egg-info/
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 07:19:14.321782 zodiax-0.4.0/zodiax.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 louis      (501) staff       (20)      391 2022-11-14 11:49:15.000000 zodiax-0.4.0/zodiax.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-14 11:49:15.000000 zodiax-0.4.0/zodiax.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 louis      (501) staff       (20)      488 2023-05-07 07:19:14.000000 zodiax-0.4.0/zodiax.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      691 2023-05-07 07:19:14.000000 zodiax-0.4.0/zodiax.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-07 07:19:14.000000 zodiax-0.4.0/zodiax.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       49 2023-05-07 07:19:14.000000 zodiax-0.4.0/zodiax.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       27 2023-05-07 07:19:14.000000 zodiax-0.4.0/zodiax.egg-info/top_level.txt
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-30 03:28:18.429864 zodiax-0.4.1/
+-rw-r--r--   0 louis      (501) staff       (20)       70 2022-11-14 06:22:13.000000 zodiax-0.4.1/.gitignore
+-rw-r--r--   0 louis      (501) staff       (20)     1523 2022-11-14 06:12:01.000000 zodiax-0.4.1/LICENSE
+-rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-14 11:44:43.000000 zodiax-0.4.1/MANIFEST.ini
+-rw-r--r--   0 louis      (501) staff       (20)      531 2023-05-30 03:28:18.429701 zodiax-0.4.1/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     4291 2023-04-11 08:47:45.000000 zodiax-0.4.1/README.md
+-rw-r--r--   0 louis      (501) staff       (20)     3030 2023-05-07 07:18:07.000000 zodiax-0.4.1/mkdocs.yml
+-rw-r--r--   0 louis      (501) staff       (20)      100 2023-05-30 03:27:12.000000 zodiax-0.4.1/requirements.txt
+-rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-30 03:28:18.429907 zodiax-0.4.1/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)     1825 2023-05-30 03:27:12.000000 zodiax-0.4.1/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-30 03:28:18.426092 zodiax-0.4.1/tests/
+-rw-r--r--   0 louis      (501) staff       (20)     3956 2023-05-07 07:18:07.000000 zodiax-0.4.1/tests/test_base.py
+-rw-r--r--   0 louis      (501) staff       (20)     2023 2023-05-11 08:18:44.000000 zodiax-0.4.1/tests/test_bayes.py
+-rw-r--r--   0 louis      (501) staff       (20)      655 2023-05-07 07:18:07.000000 zodiax-0.4.1/tests/test_eqx.py
+-rw-r--r--   0 louis      (501) staff       (20)      332 2023-05-07 07:18:07.000000 zodiax-0.4.1/tests/test_jit.py
+-rw-r--r--   0 louis      (501) staff       (20)      630 2023-05-07 07:18:07.000000 zodiax-0.4.1/tests/test_optimisation.py
+-rw-r--r--   0 louis      (501) staff       (20)      666 2023-05-07 07:18:07.000000 zodiax-0.4.1/tests/test_serialisation.py
+-rw-r--r--   0 louis      (501) staff       (20)      453 2023-05-07 07:18:07.000000 zodiax-0.4.1/tests/test_tree.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-30 03:28:18.426904 zodiax-0.4.1/zodiax/
+-rw-r--r--   0 louis      (501) staff       (20)      472 2023-05-11 08:19:02.000000 zodiax-0.4.1/zodiax/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)    17880 2023-05-10 13:13:03.000000 zodiax-0.4.1/zodiax/base.py
+-rw-r--r--   0 louis      (501) staff       (20)    13283 2023-05-11 07:25:09.000000 zodiax-0.4.1/zodiax/bayes.py
+-rw-r--r--   0 louis      (501) staff       (20)     5711 2023-05-07 07:18:07.000000 zodiax-0.4.1/zodiax/eqx.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-30 03:28:18.429459 zodiax-0.4.1/zodiax/experimental/
+-rw-r--r--   0 louis      (501) staff       (20)      238 2023-05-04 01:45:02.000000 zodiax-0.4.1/zodiax/experimental/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)     1927 2023-05-07 07:18:07.000000 zodiax-0.4.1/zodiax/experimental/jit.py
+-rw-r--r--   0 louis      (501) staff       (20)    17318 2023-04-11 08:47:45.000000 zodiax-0.4.1/zodiax/experimental/serialisation.py
+-rw-r--r--   0 louis      (501) staff       (20)     2323 2023-05-07 07:18:07.000000 zodiax-0.4.1/zodiax/optimisation.py
+-rw-r--r--   0 louis      (501) staff       (20)     2461 2023-05-07 07:18:07.000000 zodiax-0.4.1/zodiax/tree.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-30 03:28:18.428616 zodiax-0.4.1/zodiax.egg-info/
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-30 03:28:18.429008 zodiax-0.4.1/zodiax.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 louis      (501) staff       (20)      391 2022-11-14 11:49:15.000000 zodiax-0.4.1/zodiax.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-14 11:49:15.000000 zodiax-0.4.1/zodiax.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 louis      (501) staff       (20)      531 2023-05-30 03:28:18.000000 zodiax-0.4.1/zodiax.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      691 2023-05-30 03:28:18.000000 zodiax-0.4.1/zodiax.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-30 03:28:18.000000 zodiax-0.4.1/zodiax.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)      252 2023-05-30 03:28:18.000000 zodiax-0.4.1/zodiax.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       27 2023-05-30 03:28:18.000000 zodiax-0.4.1/zodiax.egg-info/top_level.txt
```

### Comparing `zodiax-0.4.0/LICENSE` & `zodiax-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zodiax-0.4.0/README.md` & `zodiax-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `zodiax-0.4.0/mkdocs.yml` & `zodiax-0.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `zodiax-0.4.0/setup.py` & `zodiax-0.4.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,15 +18,19 @@
     raise RuntimeError("Unable to find version string.")
 
 # DEPENDENCIES
 # 1. What are the required dependencies?
 with open('requirements.txt') as f:
     install_requires = f.read().splitlines()
 # 2. What dependencies required to run the unit tests? (i.e. `pytest --remote-data`)
-# tests_require = ['pytest', 'pytest-cov', 'pytest-remotedata']
+tests_require = ['pytest']
+docs_require = ['optax', 'matplotlib', 'jupyter', 'jupyterlab', 'tqdm',
+    'chainconsumer', 'numpyro', "mkdocs", "mkdocs-jupyter", 
+    "mkdocs-same-dir", "mkdocs-autorefs", "mkdocs-simple-plugin", 
+    "mkdocstrings-python", "jupyter_contrib_nbextensions"]
 
 
 setuptools.setup(
     python_requires='>=3.8, <4',
     name="zodiax",
     version=find_version("zodiax", "__init__.py"),
     description="Equinox extension for scientific programming",
@@ -37,14 +41,18 @@
     url="https://github.com/LouisDesdoigts/zodiax",
 
     project_urls={
         "Bug Tracker": "https://github.com/LouisDesdoigts/zodiax/issues",
     },
 
     install_requires=install_requires,
+    extras_require={
+        'docs': docs_require, 
+        'tests' : tests_require
+        },
 
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
 
     packages = ["zodiax", "zodiax/experimental"],
```

### Comparing `zodiax-0.4.0/tests/test_base.py` & `zodiax-0.4.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.4.0/tests/test_bayes.py` & `zodiax-0.4.1/tests/test_bayes.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,14 +44,25 @@
     shape_dict = {'param': (1,)}
 
     for param in paths:
         zodiax.bayes.covariance_matrix(pytree, param, loglike_fn, data, 
             shape_dict=shape_dict)
 
 
+def test_covaraince_entropy(create_base):
+    pytree = create_base()
+    data = pytree.model()
+    loglike_fn = zodiax.bayes.poiss_loglike
+    shape_dict = {'param': (1,)}
+    for param in paths:
+        cov = zodiax.bayes.covariance_matrix(pytree, param, loglike_fn, data,
+            shape_dict=shape_dict)
+        zodiax.bayes.covaraince_entropy(cov)
+
+
 def test_self_fisher_matrix(create_base):
     pytree = create_base()
     loglike_fn = zodiax.bayes.poiss_loglike
     shape_dict = {'param': (1,)}
 
     for param in paths:
         zodiax.bayes.self_fisher_matrix(pytree, param, loglike_fn,
```

### Comparing `zodiax-0.4.0/tests/test_eqx.py` & `zodiax-0.4.1/tests/test_eqx.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.4.0/tests/test_optimisation.py` & `zodiax-0.4.1/tests/test_optimisation.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.4.0/tests/test_serialisation.py` & `zodiax-0.4.1/tests/test_serialisation.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.4.0/zodiax/base.py` & `zodiax-0.4.1/zodiax/base.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.4.0/zodiax/bayes.py` & `zodiax-0.4.1/zodiax/bayes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import zodiax
 import jax.numpy as np
 import jax.scipy as jsp
 from jax import hessian, lax, Array
 from typing import Union, List, Any
 
 
-__all__ = ["poiss_loglike", "chi2_loglike", "fisher_matrix",
-    "covariance_matrix", "self_fisher_matrix", "self_covariance_matrix"]
+__all__ = ["poiss_loglike", "chi2_loglike", "covaraince_entropy", 
+    "fisher_matrix", "covariance_matrix", "self_fisher_matrix", 
+    "self_covariance_matrix"]
 
 
 """
 Assumes all pytrees have a .model() function
 TODO: Allow *args and **kwargs to be passed to pytree.model()
     -> Actually kind of hard, since we already have * args and ** kwargs for
     the loglike function
@@ -59,14 +60,32 @@
     -------
     log_likelihood : Array
         Log likelihood of the pytree given the data.
     """
     return jsp.stats.chi2.logpdf(pytree.model(), data, scale=noise).sum()
 
 
+def covaraince_entropy(covariance_matrix : Array) -> Array:
+    """
+    Calculates the entropy of a covariance matrix.
+
+    Parameters
+    ----------
+    covariance_matrix : Array
+        The covariance matrix to calculate the entropy of.
+    
+    Returns
+    -------
+    entropy : Array
+        The entropy of the covariance matrix.
+    """
+    sign, logdet = np.linalg.slogdet(covariance_matrix)
+    return 0.5 * (np.log(2 * np.pi * np.e) + (sign * logdet))
+
+
 def fisher_matrix(
         pytree           : Base(), 
         parameters       : Params,
         loglike_fn       : callable,
         *loglike_args    : Any,
         shape_dict       : dict = {},
         **loglike_kwargs : Any,
```

### Comparing `zodiax-0.4.0/zodiax/eqx.py` & `zodiax-0.4.1/zodiax/eqx.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.4.0/zodiax/experimental/jit.py` & `zodiax-0.4.1/zodiax/experimental/jit.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.4.0/zodiax/experimental/serialisation.py` & `zodiax-0.4.1/zodiax/experimental/serialisation.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.4.0/zodiax/optimisation.py` & `zodiax-0.4.1/zodiax/optimisation.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.4.0/zodiax/tree.py` & `zodiax-0.4.1/zodiax/tree.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.4.0/zodiax.egg-info/SOURCES.txt` & `zodiax-0.4.1/zodiax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

