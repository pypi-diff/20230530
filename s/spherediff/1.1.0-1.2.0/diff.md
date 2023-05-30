# Comparing `tmp/spherediff-1.1.0.tar.gz` & `tmp/spherediff-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/kormos/spherediff/dist/.tmp-oulq8aci/spherediff-1.1.0.tar", last modified: Mon May 29 03:17:34 2023, max compression
+gzip compressed data, was "/home/kormos/spherediff/dist/.tmp-yjpk4dce/spherediff-1.2.0.tar", last modified: Tue May 30 02:21:09 2023, max compression
```

## Comparing `spherediff-1.1.0.tar` & `spherediff-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-29 03:17:34.875851 spherediff-1.1.0/
--rw-r--r--   0 kormos    (1000) kormos    (1000)     1068 2023-05-22 22:12:37.000000 spherediff-1.1.0/LICENSE.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)     2906 2023-05-29 03:17:34.875851 spherediff-1.1.0/PKG-INFO
--rw-r--r--   0 kormos    (1000) kormos    (1000)     2410 2023-05-22 22:06:10.000000 spherediff-1.1.0/README.md
--rw-r--r--   0 kormos    (1000) kormos    (1000)      766 2023-05-29 03:16:18.000000 spherediff-1.1.0/pyproject.toml
--rw-r--r--   0 kormos    (1000) kormos    (1000)       38 2023-05-29 03:17:34.875851 spherediff-1.1.0/setup.cfg
--rw-r--r--   0 kormos    (1000) kormos    (1000)       50 2023-05-22 21:59:35.000000 spherediff-1.1.0/setup.py
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-29 03:17:34.875851 spherediff-1.1.0/src/
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-29 03:17:34.875851 spherediff-1.1.0/src/spherediff/
--rw-r--r--   0 kormos    (1000) kormos    (1000)        0 2023-05-08 23:09:07.000000 spherediff-1.1.0/src/spherediff/__init__.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)     8087 2023-05-29 03:14:23.000000 spherediff-1.1.0/src/spherediff/coeffs.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)    11141 2023-05-29 03:14:23.000000 spherediff-1.1.0/src/spherediff/kernel.py
--rwxr-xr-x   0 kormos    (1000) kormos    (1000)     4459 2023-05-29 03:14:23.000000 spherediff-1.1.0/src/spherediff/poly.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)     2333 2023-05-22 05:54:25.000000 spherediff-1.1.0/src/spherediff/sample.py
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-29 03:17:34.875851 spherediff-1.1.0/src/spherediff.egg-info/
--rw-r--r--   0 kormos    (1000) kormos    (1000)     2906 2023-05-29 03:17:34.000000 spherediff-1.1.0/src/spherediff.egg-info/PKG-INFO
--rw-r--r--   0 kormos    (1000) kormos    (1000)      359 2023-05-29 03:17:34.000000 spherediff-1.1.0/src/spherediff.egg-info/SOURCES.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)        1 2023-05-29 03:17:34.000000 spherediff-1.1.0/src/spherediff.egg-info/dependency_links.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)       75 2023-05-29 03:17:34.000000 spherediff-1.1.0/src/spherediff.egg-info/requires.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)       11 2023-05-29 03:17:34.000000 spherediff-1.1.0/src/spherediff.egg-info/top_level.txt
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-30 02:21:09.692022 spherediff-1.2.0/
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     1068 2023-05-22 22:12:37.000000 spherediff-1.2.0/LICENSE.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     4973 2023-05-30 02:21:09.692022 spherediff-1.2.0/PKG-INFO
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     4477 2023-05-30 00:39:12.000000 spherediff-1.2.0/README.md
+-rw-r--r--   0 kormos    (1000) kormos    (1000)      766 2023-05-30 00:39:23.000000 spherediff-1.2.0/pyproject.toml
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       38 2023-05-30 02:21:09.692022 spherediff-1.2.0/setup.cfg
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       50 2023-05-22 21:59:35.000000 spherediff-1.2.0/setup.py
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-30 02:21:09.692022 spherediff-1.2.0/src/
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-30 02:21:09.692022 spherediff-1.2.0/src/spherediff/
+-rw-r--r--   0 kormos    (1000) kormos    (1000)        0 2023-05-08 23:09:07.000000 spherediff-1.2.0/src/spherediff/__init__.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     8087 2023-05-29 03:14:23.000000 spherediff-1.2.0/src/spherediff/coeffs.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)    11140 2023-05-30 02:11:22.000000 spherediff-1.2.0/src/spherediff/kernel.py
+-rwxr-xr-x   0 kormos    (1000) kormos    (1000)     4459 2023-05-29 03:14:23.000000 spherediff-1.2.0/src/spherediff/poly.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     2332 2023-05-30 02:13:29.000000 spherediff-1.2.0/src/spherediff/sample.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     1176 2023-05-29 19:35:49.000000 spherediff-1.2.0/src/spherediff/score.py
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-30 02:21:09.692022 spherediff-1.2.0/src/spherediff.egg-info/
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     4973 2023-05-30 02:21:09.000000 spherediff-1.2.0/src/spherediff.egg-info/PKG-INFO
+-rw-r--r--   0 kormos    (1000) kormos    (1000)      383 2023-05-30 02:21:09.000000 spherediff-1.2.0/src/spherediff.egg-info/SOURCES.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)        1 2023-05-30 02:21:09.000000 spherediff-1.2.0/src/spherediff.egg-info/dependency_links.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       75 2023-05-30 02:21:09.000000 spherediff-1.2.0/src/spherediff.egg-info/requires.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       11 2023-05-30 02:21:09.000000 spherediff-1.2.0/src/spherediff.egg-info/top_level.txt
```

### Comparing `spherediff-1.1.0/LICENSE.txt` & `spherediff-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spherediff-1.1.0/PKG-INFO` & `spherediff-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spherediff
-Version: 1.1.0
+Version: 1.2.0
 Summary: Sample from the diffusion kernel on any n-sphere
 Author-email: Rian Kormos <Rian.Kormos@ucsf.edu>
 Project-URL: Homepage, https://github.com/rckormos/SphereDiff
 Keywords: diffusion,hypersphere,sampling
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -78,7 +78,56 @@
 >>> sample_spherical_kernel(3, means, vars, hemisphere=True)
 array([[ 0.92723597,  0.02336567,  0.37374791],
        [ 0.99421791, -0.03878944, -0.10013055],
        [ 0.15771025,  0.6492883 , -0.74401087],
        [ 0.2418101 , -0.41127436, -0.87885225],
        [-0.11192408, -0.71437847, -0.69075061]])
 ```
+
+The user may also compute the score function of the isotropic Gaussian 
+distribution on the unit n-sphere, defined as the Riemannian gradient 
+of the logarithm of the probability density. This may be done using the 
+`score_spherical_kernel` function, which may be imported as follows:
+
+```
+from spherediff.score import score_spherical_kernel
+```
+
+This function takes four arguments. The first is n, the dimension of the 
+space in which the n-sphere is embedded. The second is a numpy array of 
+shape (N, n) consisting of the n-dimensional unit vectors at which to 
+evaluate the score function. The third is a numpy array of shape (N, n) 
+consisting of the n-dimensional unit vectors at which to center the 
+distributions of which the corresponding score functions will be evaluated. 
+The fourth is a numpy array of shape (N,) consisting of the scalar variance 
+parameters of each distribution.
+
+Example output from `score_spherical_kernel` is:
+
+```
+>>> import numpy as np
+>>> from spherediff.sample import sample_spherical_kernel
+>>> from spherediff.score import score_spherical_kernel
+>>> np.random.seed(42)
+>>> means = np.random.randn(5, 3)
+>>> means /= np.linalg.norm(means, axis=1, keepdims=True)
+>>> means
+array([[ 0.60000205, -0.1670153 ,  0.78237039],
+       [ 0.97717133, -0.15023209, -0.15022156],
+       [ 0.86889694,  0.42224942, -0.25830898],
+       [ 0.63675162, -0.5438697 , -0.54658314],
+       [ 0.09351637, -0.73946664, -0.66666616]])
+>>> vars = 0.1 * np.ones(5)
+>>> x = sample_spherical_kernel(3, means, vars)
+>>> x
+array([[ 0.30027556, -0.53104481,  0.79235472],
+       [ 0.91657116, -0.39288942,  0.07439905],
+       [ 0.81325411,  0.41495422, -0.40795926],
+       [ 0.39907791, -0.44171124, -0.80350981],
+       [ 0.16422958, -0.76019121, -0.62860001]])
+>>> score_spherical_kernel(3, x, means, vars)
+array([[ 0.45383257, -1.4484151 , -0.34370955],
+       [ 2.57268711,  3.50638512, -2.19627206],
+       [ 0.33420178,  5.16225326, -0.64669865],
+       [ 2.62797084,  2.20685896, -1.97070763],
+       [-3.68698876, -0.78777185, -3.71349795]])
+```
```

### Comparing `spherediff-1.1.0/README.md` & `spherediff-1.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -64,7 +64,56 @@
 >>> sample_spherical_kernel(3, means, vars, hemisphere=True)
 array([[ 0.92723597,  0.02336567,  0.37374791],
        [ 0.99421791, -0.03878944, -0.10013055],
        [ 0.15771025,  0.6492883 , -0.74401087],
        [ 0.2418101 , -0.41127436, -0.87885225],
        [-0.11192408, -0.71437847, -0.69075061]])
 ```
+
+The user may also compute the score function of the isotropic Gaussian 
+distribution on the unit n-sphere, defined as the Riemannian gradient 
+of the logarithm of the probability density. This may be done using the 
+`score_spherical_kernel` function, which may be imported as follows:
+
+```
+from spherediff.score import score_spherical_kernel
+```
+
+This function takes four arguments. The first is n, the dimension of the 
+space in which the n-sphere is embedded. The second is a numpy array of 
+shape (N, n) consisting of the n-dimensional unit vectors at which to 
+evaluate the score function. The third is a numpy array of shape (N, n) 
+consisting of the n-dimensional unit vectors at which to center the 
+distributions of which the corresponding score functions will be evaluated. 
+The fourth is a numpy array of shape (N,) consisting of the scalar variance 
+parameters of each distribution.
+
+Example output from `score_spherical_kernel` is:
+
+```
+>>> import numpy as np
+>>> from spherediff.sample import sample_spherical_kernel
+>>> from spherediff.score import score_spherical_kernel
+>>> np.random.seed(42)
+>>> means = np.random.randn(5, 3)
+>>> means /= np.linalg.norm(means, axis=1, keepdims=True)
+>>> means
+array([[ 0.60000205, -0.1670153 ,  0.78237039],
+       [ 0.97717133, -0.15023209, -0.15022156],
+       [ 0.86889694,  0.42224942, -0.25830898],
+       [ 0.63675162, -0.5438697 , -0.54658314],
+       [ 0.09351637, -0.73946664, -0.66666616]])
+>>> vars = 0.1 * np.ones(5)
+>>> x = sample_spherical_kernel(3, means, vars)
+>>> x
+array([[ 0.30027556, -0.53104481,  0.79235472],
+       [ 0.91657116, -0.39288942,  0.07439905],
+       [ 0.81325411,  0.41495422, -0.40795926],
+       [ 0.39907791, -0.44171124, -0.80350981],
+       [ 0.16422958, -0.76019121, -0.62860001]])
+>>> score_spherical_kernel(3, x, means, vars)
+array([[ 0.45383257, -1.4484151 , -0.34370955],
+       [ 2.57268711,  3.50638512, -2.19627206],
+       [ 0.33420178,  5.16225326, -0.64669865],
+       [ 2.62797084,  2.20685896, -1.97070763],
+       [-3.68698876, -0.78777185, -3.71349795]])
+```
```

### Comparing `spherediff-1.1.0/pyproject.toml` & `spherediff-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spherediff"
-version = "1.1.0"
+version = "1.2.0"
 description = "Sample from the diffusion kernel on any n-sphere"
 readme = "README.md"
 authors = [{name = "Rian Kormos", email = "Rian.Kormos@ucsf.edu"}]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License", 
     "Programming Language :: Python",
```

### Comparing `spherediff-1.1.0/src/spherediff/coeffs.py` & `spherediff-1.2.0/src/spherediff/coeffs.py`

 * *Files identical despite different names*

### Comparing `spherediff-1.1.0/src/spherediff/kernel.py` & `spherediff-1.2.0/src/spherediff/kernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         mean += dmean
         if np.abs(dmean).max() < 1e-14:
             converged = True
         else:
             converged = False
         # update coeffs_l and coeffs_lp1 
         coeffs_lp2 = np.empty(len(coeffs_lp1) + 1)
-        prefactor = 2. ** ((n + 1) // 2)
+        prefactor = 2. ** ((n + 1) % 2)
         factor1 = (2 * l + n) / (2 * l + 4)
         factor2 = (l + n - 2) / (l + 2)
         coeffs_lp2[0] = factor1 * coeffs_lp1[1] - factor2 * coeffs_l[0]
         coeffs_lp2[1] = \
             factor1 * (coeffs_lp1[2] + prefactor * coeffs_lp1[0]) - \
             factor2 * coeffs_l[1]
         for k in range(2, len(coeffs_lp2) - 2):
```

### Comparing `spherediff-1.1.0/src/spherediff/poly.py` & `spherediff-1.2.0/src/spherediff/poly.py`

 * *Files identical despite different names*

### Comparing `spherediff-1.1.0/src/spherediff/sample.py` & `spherediff-1.2.0/src/spherediff/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,22 +44,22 @@
         n-sphere.
 
     Returns
     -------
     phi_opt : np.array [N]
         Array of angles phi for which the CDF is u_phi.
     """
-    phi = angle_mean(n, var) 
+    phi = angle_mean(n, var)
     phi[var == 0.] = 0.
     counter, d_phi = 0, np.ones_like(phi)
     idxs = np.logical_and(np.abs(d_phi) > 1e-14, var > 0.)
     while np.any(idxs) and counter < 1000:
         pdf, cdf = kernel(n, var[idxs], phi[idxs])
         if hemisphere:
             pdf_rev, cdf_rev = kernel(n, var[idxs], np.pi - phi[idxs])
             pdf = pdf + pdf_rev
             cdf = 1. + cdf - cdf_rev
         d_phi = (cdf - u_phi[idxs]) / pdf
         phi[idxs] = phi[idxs] - d_phi
-        idxs[idxs] = np.abs(d_phi) > 1e-14
+        idxs[idxs] = np.abs(d_phi) > 1e-12
         counter += 1
     return phi
```

### Comparing `spherediff-1.1.0/src/spherediff.egg-info/PKG-INFO` & `spherediff-1.2.0/src/spherediff.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spherediff
-Version: 1.1.0
+Version: 1.2.0
 Summary: Sample from the diffusion kernel on any n-sphere
 Author-email: Rian Kormos <Rian.Kormos@ucsf.edu>
 Project-URL: Homepage, https://github.com/rckormos/SphereDiff
 Keywords: diffusion,hypersphere,sampling
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -78,7 +78,56 @@
 >>> sample_spherical_kernel(3, means, vars, hemisphere=True)
 array([[ 0.92723597,  0.02336567,  0.37374791],
        [ 0.99421791, -0.03878944, -0.10013055],
        [ 0.15771025,  0.6492883 , -0.74401087],
        [ 0.2418101 , -0.41127436, -0.87885225],
        [-0.11192408, -0.71437847, -0.69075061]])
 ```
+
+The user may also compute the score function of the isotropic Gaussian 
+distribution on the unit n-sphere, defined as the Riemannian gradient 
+of the logarithm of the probability density. This may be done using the 
+`score_spherical_kernel` function, which may be imported as follows:
+
+```
+from spherediff.score import score_spherical_kernel
+```
+
+This function takes four arguments. The first is n, the dimension of the 
+space in which the n-sphere is embedded. The second is a numpy array of 
+shape (N, n) consisting of the n-dimensional unit vectors at which to 
+evaluate the score function. The third is a numpy array of shape (N, n) 
+consisting of the n-dimensional unit vectors at which to center the 
+distributions of which the corresponding score functions will be evaluated. 
+The fourth is a numpy array of shape (N,) consisting of the scalar variance 
+parameters of each distribution.
+
+Example output from `score_spherical_kernel` is:
+
+```
+>>> import numpy as np
+>>> from spherediff.sample import sample_spherical_kernel
+>>> from spherediff.score import score_spherical_kernel
+>>> np.random.seed(42)
+>>> means = np.random.randn(5, 3)
+>>> means /= np.linalg.norm(means, axis=1, keepdims=True)
+>>> means
+array([[ 0.60000205, -0.1670153 ,  0.78237039],
+       [ 0.97717133, -0.15023209, -0.15022156],
+       [ 0.86889694,  0.42224942, -0.25830898],
+       [ 0.63675162, -0.5438697 , -0.54658314],
+       [ 0.09351637, -0.73946664, -0.66666616]])
+>>> vars = 0.1 * np.ones(5)
+>>> x = sample_spherical_kernel(3, means, vars)
+>>> x
+array([[ 0.30027556, -0.53104481,  0.79235472],
+       [ 0.91657116, -0.39288942,  0.07439905],
+       [ 0.81325411,  0.41495422, -0.40795926],
+       [ 0.39907791, -0.44171124, -0.80350981],
+       [ 0.16422958, -0.76019121, -0.62860001]])
+>>> score_spherical_kernel(3, x, means, vars)
+array([[ 0.45383257, -1.4484151 , -0.34370955],
+       [ 2.57268711,  3.50638512, -2.19627206],
+       [ 0.33420178,  5.16225326, -0.64669865],
+       [ 2.62797084,  2.20685896, -1.97070763],
+       [-3.68698876, -0.78777185, -3.71349795]])
+```
```

