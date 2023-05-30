# Comparing `tmp/PythonicDISORT-0.0.2.tar.gz` & `tmp/PythonicDISORT-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonicDISORT-0.0.2.tar", last modified: Wed Apr 19 15:08:40 2023, max compression
+gzip compressed data, was "PythonicDISORT-0.1.0.tar", last modified: Tue May 30 10:14:07 2023, max compression
```

## Comparing `PythonicDISORT-0.0.2.tar` & `PythonicDISORT-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:08:40.684362 PythonicDISORT-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-19 15:08:40.684362 PythonicDISORT-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-19 15:08:22.000000 PythonicDISORT-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-19 15:08:23.000000 PythonicDISORT-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 15:08:40.684362 PythonicDISORT-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:08:40.680362 PythonicDISORT-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:08:40.680362 PythonicDISORT-0.0.2/src/PythonicDISORT/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 15:08:23.000000 PythonicDISORT-0.0.2/src/PythonicDISORT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-04-19 15:08:23.000000 PythonicDISORT-0.0.2/src/PythonicDISORT/_loop_and_assemble_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-19 15:08:23.000000 PythonicDISORT-0.0.2/src/PythonicDISORT/_one_Fourier_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    20045 2023-04-19 15:08:23.000000 PythonicDISORT-0.0.2/src/PythonicDISORT/pydisort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-19 15:08:23.000000 PythonicDISORT-0.0.2/src/PythonicDISORT/subroutines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:08:40.684362 PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-19 15:08:40.000000 PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-19 15:08:40.000000 PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:08:40.000000 PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-19 15:08:40.000000 PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 15:08:40.000000 PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:14:07.553220 PythonicDISORT-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-30 10:14:07.553220 PythonicDISORT-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-30 10:13:47.000000 PythonicDISORT-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-30 10:13:48.000000 PythonicDISORT-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:14:07.553220 PythonicDISORT-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:14:07.549219 PythonicDISORT-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:14:07.549219 PythonicDISORT-0.1.0/src/PythonicDISORT/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 10:13:48.000000 PythonicDISORT-0.1.0/src/PythonicDISORT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-05-30 10:13:48.000000 PythonicDISORT-0.1.0/src/PythonicDISORT/_loop_and_assemble_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-05-30 10:13:48.000000 PythonicDISORT-0.1.0/src/PythonicDISORT/_one_Fourier_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20125 2023-05-30 10:13:48.000000 PythonicDISORT-0.1.0/src/PythonicDISORT/pydisort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-05-30 10:13:48.000000 PythonicDISORT-0.1.0/src/PythonicDISORT/subroutines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:14:07.553220 PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-30 10:14:07.000000 PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-30 10:14:07.000000 PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:14:07.000000 PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-30 10:14:07.000000 PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 10:14:07.000000 PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/top_level.txt
```

### Comparing `PythonicDISORT-0.0.2/PKG-INFO` & `PythonicDISORT-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonicDISORT
-Version: 0.0.2
+Version: 0.1.0
 Summary: Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 Author-email: Dion HO Jia Xu <dh3065@columbia.edu>
 Project-URL: Homepage, https://github.com/LDEO-CREW/PythonicDISORT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `PythonicDISORT-0.0.2/README.md` & `PythonicDISORT-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `PythonicDISORT-0.0.2/pyproject.toml` & `PythonicDISORT-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 dependencies = [
   "numpy>=1.17.3",
   "scipy>=1.8.0",
 ]
 name = "PythonicDISORT"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="Dion HO Jia Xu", email="dh3065@columbia.edu" },
 ]
 description = "Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `PythonicDISORT-0.0.2/src/PythonicDISORT/_loop_and_assemble_results.py` & `PythonicDISORT-0.1.0/src/PythonicDISORT/_loop_and_assemble_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from PythonicDISORT import subroutines
 from PythonicDISORT.subroutines import _mathscr_v
 from PythonicDISORT._one_Fourier_mode import _one_Fourier_mode 
 from math import pi
 try:
     import autograd.numpy as np
 except ImportError:
     import numpy as np
```

### Comparing `PythonicDISORT-0.0.2/src/PythonicDISORT/_one_Fourier_mode.py` & `PythonicDISORT-0.1.0/src/PythonicDISORT/_one_Fourier_mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,89 +28,88 @@
     The labels in this file reference labels in the Jupyter Notebook, especially sections 3 and 5.
 
     """
     # Setup
     # --------------------------------------------------------------------------------------------------------------------------
     ells = np.arange(m, NLeg)
     degree_tile = np.tile(ells, (N, 1)).T
-    fac = np.prod(
-        ells[:, None] + np.arange(-m + 1, m + 1)[None, :], axis=-1, dtype=np.float64
-    )
+    fac = sc.special.poch(ells + m + 1, -2 * m)
     signs = np.empty(NLeg - m)
     signs[::2] = 1
     signs[1::2] = -1
 
     asso_leg_term_pos = sc.special.lpmv(m, degree_tile, mu_arr_pos)
     asso_leg_term_neg = asso_leg_term_pos * signs[:, None]
     asso_leg_term_mu0 = sc.special.lpmv(m, ells, -mu0)
     # --------------------------------------------------------------------------------------------------------------------------
     
     # Generate mathscr_D and mathscr_X (BDRF terms)
     # --------------------------------------------------------------------------------------------------------------------------
     # If h_\ell = 0 for all \ell \geq m, then there is no BDRF contribution
-    if m < NBDRF:
+    if m < NBDRF and np.all(np.isfinite(asso_leg_term_pos[:NBDRF, :])):
         weighted_asso_Leg_coeffs_BDRF = (
-            weighted_Leg_coeffs_BDRF[ells[: (NBDRF - m)]] / fac[: (NBDRF - m)]
+            weighted_Leg_coeffs_BDRF[ells[: (NBDRF - m)]] * fac[: (NBDRF - m)]
         )
-
         mathscr_D_temp = (
             weighted_asso_Leg_coeffs_BDRF[None, :] * asso_leg_term_pos.T[:, :NBDRF]
         )
         mathscr_D_neg = 2 * mathscr_D_temp @ asso_leg_term_neg[:NBDRF, :]
         R = mathscr_D_neg * (mu_arr_pos * W)[None, :]
+
         if I0 > 0:
             mathscr_X_temp = (
                 (mu0 * I0 * (2 - (m == 0)) / pi)
                 * weighted_asso_Leg_coeffs_BDRF
                 * asso_leg_term_mu0[:NBDRF]
             )
             mathscr_X_pos = mathscr_X_temp @ asso_leg_term_pos[:NBDRF, :]
     # --------------------------------------------------------------------------------------------------------------------------
-    
+
     # Loop over NLayers atmospheric layers
     # --------------------------------------------------------------------------------------------------------------------------
     if Nscoeffs > 0 and m == 0:
         G_inv_collect_0 = np.empty((NLayers, NQuad, NQuad))
     G_collect_m = np.empty((NLayers, NQuad, NQuad))
     K_collect_m = np.empty((NLayers, NQuad))
     if I0 > 0:
         B_collect_m = np.zeros((NLayers, NQuad))
-        
+
     for l in range(NLayers):
         # More setup
-        weighted_scaled_Leg_coeffs_l_ells = weighted_scaled_Leg_coeffs[l, :][ells]
+        weighted_asso_Leg_coeffs_l = weighted_scaled_Leg_coeffs[l, :][ells] * fac
         scaled_omega_l = scaled_omega_arr[l]
-        if not np.allclose(weighted_scaled_Leg_coeffs_l_ells, 0):
+        
+        if np.any(weighted_asso_Leg_coeffs_l > 0) and np.all(
+            np.isfinite(asso_leg_term_pos)
+        ):
             # Generate mathscr_D and mathscr_X (BDRF terms)
             # --------------------------------------------------------------------------------------------------------------------------
-            weighted_asso_Leg_coeffs_l = weighted_scaled_Leg_coeffs_l_ells / fac
-
             D_temp = weighted_asso_Leg_coeffs_l[None, :] * asso_leg_term_pos.T
             D_pos = (scaled_omega_l / 2) * D_temp @ asso_leg_term_pos
             D_neg = (scaled_omega_l / 2) * D_temp @ asso_leg_term_neg
 
             if I0 > 0:
                 X_temp = (
                     (scaled_omega_l * I0 * (2 - (m == 0)) / (4 * pi))
                     * weighted_asso_Leg_coeffs_l
                     * asso_leg_term_mu0
                 )
                 X_pos = X_temp @ asso_leg_term_pos
                 X_neg = X_temp @ asso_leg_term_neg
             # --------------------------------------------------------------------------------------------------------------------------
-            
+
             # Assemble the coefficient matrix and additional terms
             # --------------------------------------------------------------------------------------------------------------------------
             alpha = M_inv[:, None] * (D_pos * W[None, :] - np.eye(N))
             beta = M_inv[:, None] * D_neg * W[None, :]
             A = np.vstack([np.hstack([-alpha, -beta]), np.hstack([beta, alpha])])
             if I0 > 0:
                 X_tilde = np.concatenate([-M_inv * X_pos, M_inv * X_neg])
             # --------------------------------------------------------------------------------------------------------------------------
-            
+
             # Diagonalization of coefficient matrix
             # --------------------------------------------------------------------------------------------------------------------------
             K_squared, eigenvecs_GpG = np.linalg.eig((alpha - beta) @ (alpha + beta))
 
             # Eigenvalues arranged negative then positive, from largest to smallest magnitude
             K = np.concatenate([-np.sqrt(K_squared), np.sqrt(K_squared)])
             eigenvecs_GpG = np.hstack([eigenvecs_GpG, eigenvecs_GpG])
@@ -120,37 +119,37 @@
             G_pos = (eigenvecs_GpG - eigenvecs_GmG) / 2
             G_neg = (eigenvecs_GpG + eigenvecs_GmG) / 2
             G = np.vstack([G_pos, G_neg])
             # We only need G^{-1} in special cases
             if Nscoeffs > 0 and m == 0:
                 G_inv = np.linalg.inv(G)
             # --------------------------------------------------------------------------------------------------------------------------
-            
+
             # Particular solution for the sunbeam source
             # --------------------------------------------------------------------------------------------------------------------------
-            if I0 > 0:    
+            if I0 > 0:
                 if Nscoeffs > 0 and m == 0:
                     B = -G / (1 / mu0 + K)[None, :] @ G_inv @ X_tilde
                 else:
                     # This method is more numerically stable
                     LHS = A.copy()
                     np.fill_diagonal(LHS, 1 / mu0 + np.diag(A))
                     B = np.linalg.solve(LHS, -X_tilde)
-                
+
                 B_collect_m[l, :] = B
             # --------------------------------------------------------------------------------------------------------------------------
         else:
             # This is a shortcut to the same results
             K = -1 / mu_arr
             G = np.zeros((NQuad, NQuad))
             G[N:, :N] = np.eye(N)
             G[:N, N:] = np.eye(N)
             if Nscoeffs > 0 and m == 0:
                 G_inv = G
-        
+
         G_collect_m[l, :, :] = G
         K_collect_m[l, :] = K
         if Nscoeffs > 0 and m == 0:
             G_inv_collect_0[l, :, :] = G_inv
     # --------------------------------------------------------------------------------------------------------------------------
 
     ################################## Solve for coefficients of homogeneous solution ##########################################
```

### Comparing `PythonicDISORT-0.0.2/src/PythonicDISORT/pydisort.py` & `PythonicDISORT-0.1.0/src/PythonicDISORT/pydisort.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     of a multi-layer atmosphere with the specified optical properties, boundary conditions
     and sources. Optionally performs delta-M scaling and NT corrections. 
     
         See https://pythonic-disort.readthedocs.io/en/latest/Pythonic-DISORT.html#1.-USER-INPUT-REQUIRED:-Choose-parameters
         for a more detailed explanation of each parameter.
         See https://pythonic-disort.readthedocs.io/en/latest/Pythonic-DISORT.html#2.-PythonicDISORT-modules-and-outputs
         for a more detailed explanation of each output.
+        The notebook also has numerous examples of this function being called.
 
     Parameters
     ----------
     tau_arr : array
         Optical depth of the lower boundary of each atmospheric layer.
     omega_arr : array
         Single-scattering albedo of each atmospheric layer.
@@ -390,15 +391,15 @@
         # --------------------------------------------------------------------------------------------------------------------------
         def u_corrected(tau, phi, return_Fourier_error=False):
             tau = np.atleast_1d(tau)
             phi = np.atleast_1d(phi)
             NT_corrections = TMS_correction(tau, phi)
 
             # We provide two options below, comment and uncomment as desired.
-            # Option 1 is more computationally efficient but would prevent the use of autograd for testing.
+            # Option 2 is more computationally efficient but would prevent the use of autograd for testing.
 
             NT_corrections = NT_corrections + np.concatenate(
                 [np.zeros((N, len(tau), len(phi))), IMS_correction(tau, phi)], axis=0
             )  # Option 1
 
             #NT_corrections[N:, :, :] += IMS_correction(tau, phi)  # Option 2
```

### Comparing `PythonicDISORT-0.0.2/src/PythonicDISORT/subroutines.py` & `PythonicDISORT-0.1.0/src/PythonicDISORT/subroutines.py`

 * *Files identical despite different names*

### Comparing `PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/PKG-INFO` & `PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonicDISORT
-Version: 0.0.2
+Version: 0.1.0
 Summary: Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 Author-email: Dion HO Jia Xu <dh3065@columbia.edu>
 Project-URL: Homepage, https://github.com/LDEO-CREW/PythonicDISORT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

