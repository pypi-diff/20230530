# Comparing `tmp/symbtools-0.3.3.tar.gz` & `tmp/symbtools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/symbtools-0.3.3.tar", last modified: Tue Dec 21 20:05:28 2021, max compression
+gzip compressed data, was "symbtools-0.3.4.tar", last modified: Tue May 30 11:37:08 2023, max compression
```

## Comparing `symbtools-0.3.3.tar` & `symbtools-0.3.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2021-12-21 20:05:28.019236 symbtools-0.3.3/
--rw-r--r--   0 ck2       (1000) ck2       (1000)     1521 2019-06-02 22:31:47.000000 symbtools-0.3.3/LICENSE
--rw-r--r--   0 ck2       (1000) ck2       (1000)       60 2019-07-04 09:46:32.000000 symbtools-0.3.3/MANIFEST.in
--rw-r--r--   0 ck2       (1000) ck2       (1000)      534 2021-12-21 20:05:28.019236 symbtools-0.3.3/PKG-INFO
--rw-r--r--   0 ck2       (1000) ck2       (1000)     3358 2021-01-05 19:33:43.000000 symbtools-0.3.3/README.md
--rw-r--r--   0 ck2       (1000) ck2       (1000)        7 2019-06-02 22:31:47.000000 symbtools-0.3.3/extra_requirements_mpc.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)       50 2021-12-09 22:24:03.000000 symbtools-0.3.3/requirements.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)       67 2021-12-21 20:05:28.019236 symbtools-0.3.3/setup.cfg
--rw-r--r--   0 ck2       (1000) ck2       (1000)     1165 2019-07-20 15:55:00.000000 symbtools-0.3.3/setup.py
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2021-12-21 20:05:28.019236 symbtools-0.3.3/symbtools/
--rw-r--r--   0 ck2       (1000) ck2       (1000)      222 2019-06-02 22:31:47.000000 symbtools-0.3.3/symbtools/__init__.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     3451 2019-12-11 11:49:41.000000 symbtools-0.3.3/symbtools/auxiliary.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)   130514 2021-12-21 19:42:59.000000 symbtools-0.3.3/symbtools/core.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     1258 2019-06-02 22:31:47.000000 symbtools-0.3.3/symbtools/interactive_aux.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    51064 2021-12-09 22:24:03.000000 symbtools-0.3.3/symbtools/meshtools.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    17984 2020-07-14 08:36:25.000000 symbtools-0.3.3/symbtools/meshtools_.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    37965 2021-07-09 08:19:20.000000 symbtools-0.3.3/symbtools/modeltools.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     9576 2021-12-09 22:24:03.000000 symbtools-0.3.3/symbtools/mpctools.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    16222 2020-12-02 15:30:40.000000 symbtools-0.3.3/symbtools/noncommutativetools.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    10480 2020-12-02 15:30:40.000000 symbtools-0.3.3/symbtools/pickle_tools.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)       22 2021-04-08 07:44:16.000000 symbtools-0.3.3/symbtools/release.py
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2021-12-21 20:05:28.019236 symbtools-0.3.3/symbtools/test/
--rw-r--r--   0 ck2       (1000) ck2       (1000)       36 2019-07-20 15:55:00.000000 symbtools-0.3.3/symbtools/test/__init__.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)      553 2021-12-09 22:24:03.000000 symbtools-0.3.3/symbtools/test/run_all_tests.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     1011 2019-12-11 11:49:41.000000 symbtools-0.3.3/symbtools/test/test_auxiliary.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    48921 2021-12-09 22:24:03.000000 symbtools-0.3.3/symbtools/test/test_core.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    16324 2019-12-11 11:49:41.000000 symbtools-0.3.3/symbtools/test/test_core1.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     1219 2019-12-11 11:49:41.000000 symbtools-0.3.3/symbtools/test/test_core2.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    25034 2021-12-09 22:24:03.000000 symbtools-0.3.3/symbtools/test/test_meshtools.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    22030 2019-12-11 11:49:41.000000 symbtools-0.3.3/symbtools/test/test_modeltools.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     5087 2021-03-16 22:45:25.000000 symbtools-0.3.3/symbtools/test/test_mpctools.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    18153 2021-12-16 22:44:03.000000 symbtools-0.3.3/symbtools/test/test_nctools.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     6727 2020-12-02 14:52:52.000000 symbtools-0.3.3/symbtools/test/test_pickle_tools.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     1200 2019-07-20 15:55:00.000000 symbtools-0.3.3/symbtools/test/test_quick.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     9233 2020-12-02 15:30:40.000000 symbtools-0.3.3/symbtools/test/test_time_deriv.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     5249 2021-12-09 22:24:03.000000 symbtools-0.3.3/symbtools/test/unittesthelper.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)      789 2019-07-03 14:15:28.000000 symbtools-0.3.3/symbtools/test/z_test_core1_test.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    14691 2019-07-20 15:55:00.000000 symbtools-0.3.3/symbtools/time_deriv.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    35570 2020-12-02 15:30:40.000000 symbtools-0.3.3/symbtools/visualisation.py
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2021-12-21 20:05:28.019236 symbtools-0.3.3/symbtools.egg-info/
--rw-r--r--   0 ck2       (1000) ck2       (1000)      534 2021-12-21 20:05:27.000000 symbtools-0.3.3/symbtools.egg-info/PKG-INFO
--rw-r--r--   0 ck2       (1000) ck2       (1000)     1048 2021-12-21 20:05:27.000000 symbtools-0.3.3/symbtools.egg-info/SOURCES.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)        1 2021-12-21 20:05:27.000000 symbtools-0.3.3/symbtools.egg-info/dependency_links.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)       64 2021-12-21 20:05:27.000000 symbtools-0.3.3/symbtools.egg-info/requires.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)       10 2021-12-21 20:05:27.000000 symbtools-0.3.3/symbtools.egg-info/top_level.txt
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-30 11:37:08.679628 symbtools-0.3.4/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1521 2019-06-02 22:31:47.000000 symbtools-0.3.4/LICENSE
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       60 2019-07-04 09:46:32.000000 symbtools-0.3.4/MANIFEST.in
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      515 2023-05-30 11:37:08.679628 symbtools-0.3.4/PKG-INFO
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     3350 2022-12-08 14:33:41.000000 symbtools-0.3.4/README.md
+-rw-r--r--   0 ck2       (1000) ck2       (1000)        7 2019-06-02 22:31:47.000000 symbtools-0.3.4/extra_requirements_mpc.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       50 2021-12-09 22:24:03.000000 symbtools-0.3.4/requirements.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       67 2023-05-30 11:37:08.679628 symbtools-0.3.4/setup.cfg
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1165 2019-07-20 15:55:00.000000 symbtools-0.3.4/setup.py
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-30 11:37:08.647628 symbtools-0.3.4/symbtools/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      222 2019-06-02 22:31:47.000000 symbtools-0.3.4/symbtools/__init__.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     3451 2019-12-11 11:49:41.000000 symbtools-0.3.4/symbtools/auxiliary.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)   131188 2023-05-29 20:47:29.000000 symbtools-0.3.4/symbtools/core.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1258 2019-06-02 22:31:47.000000 symbtools-0.3.4/symbtools/interactive_aux.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    51064 2021-12-09 22:24:03.000000 symbtools-0.3.4/symbtools/meshtools.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    17984 2020-07-14 08:36:25.000000 symbtools-0.3.4/symbtools/meshtools_.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    38344 2022-12-14 22:50:54.000000 symbtools-0.3.4/symbtools/modeltools.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     9576 2021-12-09 22:24:03.000000 symbtools-0.3.4/symbtools/mpctools.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    16222 2020-12-02 15:30:40.000000 symbtools-0.3.4/symbtools/noncommutativetools.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    10480 2020-12-02 15:30:40.000000 symbtools-0.3.4/symbtools/pickle_tools.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       22 2023-05-30 11:33:27.000000 symbtools-0.3.4/symbtools/release.py
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-30 11:37:08.679628 symbtools-0.3.4/symbtools/test/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       36 2019-07-20 15:55:00.000000 symbtools-0.3.4/symbtools/test/__init__.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      553 2022-11-29 20:17:58.000000 symbtools-0.3.4/symbtools/test/run_all_tests.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1011 2019-12-11 11:49:41.000000 symbtools-0.3.4/symbtools/test/test_auxiliary.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    48921 2022-12-08 14:33:38.000000 symbtools-0.3.4/symbtools/test/test_core.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    16324 2019-12-11 11:49:41.000000 symbtools-0.3.4/symbtools/test/test_core1.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1219 2019-12-11 11:49:41.000000 symbtools-0.3.4/symbtools/test/test_core2.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    25034 2021-12-09 22:24:03.000000 symbtools-0.3.4/symbtools/test/test_meshtools.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    22754 2022-12-14 22:58:55.000000 symbtools-0.3.4/symbtools/test/test_modeltools.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     5087 2021-03-16 22:45:25.000000 symbtools-0.3.4/symbtools/test/test_mpctools.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    18153 2022-12-08 14:33:41.000000 symbtools-0.3.4/symbtools/test/test_nctools.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     6727 2020-12-02 14:52:52.000000 symbtools-0.3.4/symbtools/test/test_pickle_tools.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1200 2019-07-20 15:55:00.000000 symbtools-0.3.4/symbtools/test/test_quick.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     9233 2020-12-02 15:30:40.000000 symbtools-0.3.4/symbtools/test/test_time_deriv.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     5249 2021-12-09 22:24:03.000000 symbtools-0.3.4/symbtools/test/unittesthelper.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      789 2019-07-03 14:15:28.000000 symbtools-0.3.4/symbtools/test/z_test_core1_test.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    14691 2019-07-20 15:55:00.000000 symbtools-0.3.4/symbtools/time_deriv.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    35570 2020-12-02 15:30:40.000000 symbtools-0.3.4/symbtools/visualisation.py
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-05-30 11:37:08.655628 symbtools-0.3.4/symbtools.egg-info/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      515 2023-05-30 11:37:08.000000 symbtools-0.3.4/symbtools.egg-info/PKG-INFO
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1048 2023-05-30 11:37:08.000000 symbtools-0.3.4/symbtools.egg-info/SOURCES.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)        1 2023-05-30 11:37:08.000000 symbtools-0.3.4/symbtools.egg-info/dependency_links.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       64 2023-05-30 11:37:08.000000 symbtools-0.3.4/symbtools.egg-info/requires.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       10 2023-05-30 11:37:08.000000 symbtools-0.3.4/symbtools.egg-info/top_level.txt
```

### Comparing `symbtools-0.3.3/LICENSE` & `symbtools-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/PKG-INFO` & `symbtools-0.3.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: symbtools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Symbolic calculations related to dynamical systems.
 Home-page: https://github.com/TUD-RST/symbtools
 Author: Carsten Knoll, Klemens Fritzsche
 Author-email: Carsten.Knoll@tu-dresden.de
 License: BSD3
-Platform: UNKNOWN
 Provides-Extra: mpc
 License-File: LICENSE
 
 
     A collection of functions to facilitate the (symbolic) calculations
     associated with the investigation of nonlinear dynamical systems in
     the field of control theory (0.1.10+ has python3 support).
     
-
```

### Comparing `symbtools-0.3.3/README.md` & `symbtools-0.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 Systeme im Rahmen der Regelungs- und Steuerungstheorie auftreten.
 
 Speziell ist im Modul `modeltools` Funktionalität gebündelt, die zur Herleitung,
 Analyse und Numerischen Lösung (Simulation) von Bewegungsgleichungen mechanischer Systeme mit
 und ohne algebraische Nebenbedingungen mit Hilfe der Lagrange-Gleichungen 1. bzw. 2. Art dient.
 
 Eine klassische Dokumentation des Paketes ist in Vorbereitung. Vorerst wird auf die, die
-[Demo-Notebooks](https://nbviewer.jupyter.org/github/TUD-RST/symbtools/tree/master/docs/demo_notebooks/),
-auf die [Unit-Tests](https://github.com/TUD-RST/symbtools/blob/master/symbtools/test/test_modeltools.py)
+[Demo-Notebooks](https://nbviewer.jupyter.org/github/TUD-RST/symbtools/tree/main/docs/demo_notebooks/),
+auf die [Unit-Tests](https://github.com/TUD-RST/symbtools/blob/main/symbtools/test/test_modeltools.py)
 und auf die Docstrings im Quellcode verwiesen.
 Für Fragen und Anregungen stehen die Github-Issue-Funktion sowie der [Paketbereuer](https://tu-dresden.de/ing/elektrotechnik/rst/das-institut/beschaeftigte/carsten-knoll)
 per Mail zur Verfügung.
 
 
 Der Programmcode hat insgesamt den Status von "Forschungscode",
 d.h. das Paket befindet sich nach wie vor in Entwicklung.
@@ -39,16 +39,16 @@
 dynamical systems in the field of control theory.
 
 Especially the module `modeltools` contains functionality wich serves for generating, analizing
 and simulating the equations of motion of mechanical systems based on the Lagrange-Equations of
 1st and 2nd kind.
 
 Classical docs for this package are still in preparation. Meanwhile we refer to the
-[Demo Notebooks](https://nbviewer.jupyter.org/github/TUD-RST/symbtools/tree/master/docs/demo_notebooks/),
-to the [unit tests](https://github.com/TUD-RST/symbtools/blob/master/symbtools/test/test_modeltools.py)
+[Demo Notebooks](https://nbviewer.jupyter.org/github/TUD-RST/symbtools/tree/main/docs/demo_notebooks/),
+to the [unit tests](https://github.com/TUD-RST/symbtools/blob/main/symbtools/test/test_modeltools.py)
 and finally to the docstrings im in the sources. If you have any question feel, free to open an
 issue or to email the [maintainer](https://tu-dresden.de/ing/elektrotechnik/rst/das-institut/beschaeftigte/carsten-knoll).
 
 Note that the package is in development state. Despite that a substantial
 part is covered by unit test, the code will contain bugs with some probability.
```

### Comparing `symbtools-0.3.3/setup.py` & `symbtools-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/auxiliary.py` & `symbtools-0.3.4/symbtools/auxiliary.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/core.py` & `symbtools-0.3.4/symbtools/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -3101,14 +3101,15 @@
     dummy_symbol_list = []
     for X in list(derivs) + list(funcs):
         dummy = next(gen)
         SL.append( (X, dummy) )
         dummy_symbol_list.append(dummy)
 
     regular_symbol_list = list(expr.atoms(sp.Symbol))  # original Symbols
+    regular_symbol_list.sort(key=str)
 
     for atom in list(derivs) + list(funcs) + regular_symbol_list:
         if not atom.is_commutative:
             msg = "At least one atom is not commutative." \
                   "Substituting with numbers might be misleading."
             warnings.warn(msg)
             break
@@ -3283,39 +3284,50 @@
     # the precision increases.
 
     # count the exact zeros
     # !! obsolete?
     #zero_count = [cl.count(0) for cl in (coeffs1, coeffs2, coeffs3)]
 
     # find out the first (w.r.t to the index) non-vanishing coeff
-
-    nz_coeffs1 = np.array([c for c in coeffs1 if c != 0], dtype=sp.Float)
-    nz_coeffs2 = np.array([c for c in coeffs2 if c != 0], dtype=sp.Float)
-    nz_coeffs3 = np.array([c for c in coeffs3 if c != 0], dtype=sp.Float)
-
-    res21_list = []
-    res32_list = []
-
     err_msg = "unexpected behavior of berkowitz coeffs during rank calculation"
     threshold = 1e-2
     for i, (c1, c2, c3) in enumerate(lzip(coeffs1, coeffs2, coeffs3)):
         if 0 in (c1, c2, c3):
             # assume that this coeff indeed vanishes
             continue
 
         q21 = abs(c2/c1)
         q32 = abs(c3/c2)
 
+        # conditions; True -> coeff gets smaller
         res21 = q21 < threshold
         res32 = q32 < threshold
 
         if res21 != res32:
             # one precision-step indicates a vanishing coeff
             # while the other does not
-            raise ValueError(err_msg)
+
+            if not res21 and res32:
+                # this is very odd and should be examined manually
+                raise ValueError(err_msg)
+            else:
+                # there are situations where the coefficient indeed gets smaller with initial
+                # precision increment (-> res21 = True) but then stabilizes (res32 = False)
+                # we need to evaluate with even higher precision
+                M4 = M.subs(rnst).evalf(n=400)
+                coeffs4 = (M4.T*M4).berkowitz()[-1][::-1]
+                c4 = coeffs4[i]
+                q43 = abs(c4/c3)
+                res43 = q43 < threshold
+                if res43:
+                    # coeff does not stabilize -> res32 is inconsistent -> examine manually
+                    raise ValueError(err_msg)
+                else:
+                    # the coeff does indeed stabilze
+                    break
 
         if res21 == False:
             # the coeff has not changed sufficiently due to the precision step
             # this means the coeff is not considered to vanish,
             # i.e. it is the first non-vanishing coeff
             break
```

### Comparing `symbtools-0.3.3/symbtools/interactive_aux.py` & `symbtools-0.3.4/symbtools/interactive_aux.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/meshtools.py` & `symbtools-0.3.4/symbtools/meshtools.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/meshtools_.py` & `symbtools-0.3.4/symbtools/meshtools_.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/modeltools.py` & `symbtools-0.3.4/symbtools/modeltools.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,15 +428,15 @@
 
 
 # noinspection PyPep8Naming
 class DAE_System(object):
     """
     This class encapsulates an differential algebraic equation (DAE).
     """
-    
+
     info = "encapsulate all dae-relevant information"
 
     def __init__(self, mod, parameter_values=None):
         """
         :param mod:                 SymbolicModel-instance
         :param parameter_values:    subs-compatible sequence
         """
@@ -626,15 +626,15 @@
         self.constraints_d_func = st.expr_to_func(xx, self.constraints_d)
 
         zz = st.row_stack(self.mod.tt, self.mod.ttd, self.mod.ttdd)
 
         # this function depends on coordinates ttheta and velocities ttheta_dot and accel
         self.constraints_dd_func = st.expr_to_func(zz, self.constraints_dd)
 
-    def gen_leqs_for_acc_llmd(self, parameter_values=None):
+    def gen_leqs_for_acc_llmd(self, parameter_values=None, debug=None):
         """
         Create a callable function which returns A, bnum of the linear eqn-system
                 A*ww = bnum,
         where ww := (ttheta_dd, llmnd).
 
 
         :return: None, set self.leqs_acc_lmd_func
@@ -719,14 +719,19 @@
 
             ttheta_dd_res = np.linalg.solve(A1, b1 - np.dot(A2, llmd))
 
             return ttheta_dd_res
 
         self.acc_of_lmd_func = acc_of_lmd_func
 
+        if debug is not None:
+            import ipydex
+            debug: ipydex.Container
+            debug.fetch_locals()
+
     def calc_consistent_conf_vel(self, **kwargs):
         """
         This function calculates configurations and velocities which of the mechanical dae system which are
         consistent with the constraints. In general the solution is not unique and thus depends on the initial guess
         (passed via special kwargs: {coord}_estimate; see below). The algebraic equation systems (for configuration
         and velocities) are solved via scipy.optimize.fmin().
 
@@ -850,15 +855,15 @@
         assert np.allclose(min_target_v(sol_v), 0)
 
         arg_v[dep_idcs] = sol_v
         ttheta_dot_cons = arg_v
 
         return ttheta_cons, ttheta_dot_cons
 
-    def calc_consistent_accel_lmd(self, xx, t=0):
+    def calc_consistent_accel_lmd(self, xx, t=0, debug=None):
         """
         This function solves numerically the the equations system
          M(ttheta) * ttheta_dd + ... + H(llmd) = 0
          Constraints_dd(ttheta, ttheta_d, ttheta_dd) = 0
 
         It consists of ntt + nll equations in the same number of variables: (ttheta_dd, llmd).
 
@@ -885,14 +890,22 @@
         self.gen_leqs_for_acc_llmd()
         A, b = self.leqs_acc_lmd_func(*np.r_[xx, external_forces])
         sol = np.linalg.solve(A, b)
 
         acc = sol[:ntt]
         llmd = sol[-nll:]
 
+        if debug is not None:
+            # assume that `debug` is a container
+            debug.A = A
+            debug.b = b
+            debug.external_forces = external_forces
+            debug.sol = sol
+            debug.xx = xx
+
         return acc, llmd
 
     def calc_consistent_init_vals(self, t=0, **kwargs):
         """
         Assume yy = (xx, llmd) and xx = (ttheta, ttheta_d)
         -> return yy_0 and and yyd_0 such that F(t, yy_0, yyd_0) = 0
 
@@ -1183,8 +1196,7 @@
 
     F = st.row_stack(eqns_def, eqns_mech)
 
     P0_bar = F.jacobian(xx)
     P1_bar = F.jacobian(xxd)
 
     return P0_bar, P1_bar
-
```

### Comparing `symbtools-0.3.3/symbtools/mpctools.py` & `symbtools-0.3.4/symbtools/mpctools.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/noncommutativetools.py` & `symbtools-0.3.4/symbtools/noncommutativetools.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/pickle_tools.py` & `symbtools-0.3.4/symbtools/pickle_tools.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/test/run_all_tests.py` & `symbtools-0.3.4/symbtools/test/run_all_tests.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/test/test_auxiliary.py` & `symbtools-0.3.4/symbtools/test/test_auxiliary.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/test/test_core.py` & `symbtools-0.3.4/symbtools/test/test_core.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/test/test_core1.py` & `symbtools-0.3.4/symbtools/test/test_core1.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/test/test_core2.py` & `symbtools-0.3.4/symbtools/test/test_core2.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/test/test_meshtools.py` & `symbtools-0.3.4/symbtools/test/test_meshtools.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/test/test_modeltools.py` & `symbtools-0.3.4/symbtools/test/test_modeltools.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 import symbtools as st
 import numpy as npy
 import symbtools.modeltools as mt
 from symbtools.modeltools import Rz
 import sys
 
 
-from IPython import embed as IPS
-
 
 # noinspection PyPep8Naming
 class ModelToolsTest(unittest.TestCase):
 
     def setUp(self):
         pass
 
@@ -194,25 +192,58 @@
         eres_c = npy.array([-0.2285526,  1.58379902,  0.78539816])
         eres_v = npy.array([0, 0, 0])
 
         self.assertTrue(npy.allclose(ttheta_1, eres_c))
         self.assertTrue(npy.allclose(ttheta_d_1, eres_v))
 
         # in that situation there is no force
-        acc_1, llmd_1 = dae.calc_consistent_accel_lmd((ttheta_1, ttheta_d_1))
+
+        import ipydex
+        debug = ipydex.Container()
+        print("gen_leqs_for_acc_llmd")
+        dae.gen_leqs_for_acc_llmd(debug=debug)
+
+        # ipydex.IPS()
+        for name, value in debug.item_list():
+            if value is debug:
+                continue
+            print(f"{name} = \n{repr(value)}\n- - -\n")
+
+        # ---
+        print("calc_consistent_accel_lmd")
+        debug = ipydex.Container()
+        acc_1, llmd_1 = dae.calc_consistent_accel_lmd((ttheta_1, ttheta_d_1), debug=debug)
+
+        for name, value in debug.item_list():
+            print(f"{name} = \n{value}\n- - -")
+
+        # ipydex.IPS()
+
         # these values seem reasonable but have yet not been checked analytically
+        # (also: the values depend on python version )
+
+        print(acc_1)
+        print(llmd_1)
+
         self.assertTrue(npy.allclose(acc_1, [13.63475466, -1.54473017, -8.75145644]))
         self.assertTrue(npy.allclose(llmd_1, [-0.99339947,  0.58291489]))
 
+        # debug
+        return
+
         # qdot1 ≠ 0
         ttheta_2, ttheta_d_2 = dae.calc_consistent_conf_vel(q1=npy.pi/8*7, qdot1=3, _disp=False)
 
+        # expected results
         eres_c = npy.array([-0.85754267,  0.89969149,  0.875])*npy.pi
         eres_v = npy.array([-3.42862311,  2.39360715,  3.])
 
+        print(ttheta_2, eres_c)
+        print(ttheta_d_2, eres_v)
+
         self.assertTrue(npy.allclose(ttheta_2, eres_c))
         self.assertTrue(npy.allclose(ttheta_d_2, eres_v))
 
         yy_1, yyd_1 = dae.calc_consistent_init_vals(q1=12.7, qdot1=100)
 
         dae.generate_eqns_funcs()
         res = dae.model_func(0, yy_1, yyd_1)
@@ -257,18 +288,18 @@
             # wrong length of external forces
             mt.generate_symbolic_model(T, V, ttheta, [F1, 0, 0])
 
         QQ = sp.Matrix([0, F1])
         mod = mt.generate_symbolic_model(T, V, ttheta, [0, F1])
         mod_1 = mt.generate_symbolic_model(T, V, ttheta, QQ)
         mod_2 = mt.generate_symbolic_model(T, V, ttheta, QQ.T)
-        
+
         self.assertEqual(mod.eqns, mod_1.eqns)
         self.assertEqual(mod.eqns, mod_2.eqns)
-        
+
         mod.eqns.simplify()
 
         M = mod.MM
         M.simplify()
 
         M_ref = Matrix([[l1**2*m1, l1*m1*cos(p1)], [l1*m1*cos(p1), m1 + m0]])
         self.assertEqual(M, M_ref)
@@ -600,13 +631,13 @@
         intern_test(3, 1)
 
 
 def main():
     # remove command line args which should not be passed to the testframework
     if 'all' in sys.argv:
         sys.argv.remove('all')
-    
+
     unittest.main()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `symbtools-0.3.3/symbtools/test/test_mpctools.py` & `symbtools-0.3.4/symbtools/test/test_mpctools.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/test/test_nctools.py` & `symbtools-0.3.4/symbtools/test/test_nctools.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/test/test_pickle_tools.py` & `symbtools-0.3.4/symbtools/test/test_pickle_tools.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/test/test_quick.py` & `symbtools-0.3.4/symbtools/test/test_quick.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/test/test_time_deriv.py` & `symbtools-0.3.4/symbtools/test/test_time_deriv.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/test/unittesthelper.py` & `symbtools-0.3.4/symbtools/test/unittesthelper.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/test/z_test_core1_test.py` & `symbtools-0.3.4/symbtools/test/z_test_core1_test.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/time_deriv.py` & `symbtools-0.3.4/symbtools/time_deriv.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools/visualisation.py` & `symbtools-0.3.4/symbtools/visualisation.py`

 * *Files identical despite different names*

### Comparing `symbtools-0.3.3/symbtools.egg-info/PKG-INFO` & `symbtools-0.3.4/symbtools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: symbtools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Symbolic calculations related to dynamical systems.
 Home-page: https://github.com/TUD-RST/symbtools
 Author: Carsten Knoll, Klemens Fritzsche
 Author-email: Carsten.Knoll@tu-dresden.de
 License: BSD3
-Platform: UNKNOWN
 Provides-Extra: mpc
 License-File: LICENSE
 
 
     A collection of functions to facilitate the (symbolic) calculations
     associated with the investigation of nonlinear dynamical systems in
     the field of control theory (0.1.10+ has python3 support).
     
-
```

### Comparing `symbtools-0.3.3/symbtools.egg-info/SOURCES.txt` & `symbtools-0.3.4/symbtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

